# Comparing `tmp/disco-tif-0.0.2.tar.gz` & `tmp/disco-tif-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disco-tif-0.0.2.tar", last modified: Wed Apr 17 13:30:45 2024, max compression
+gzip compressed data, was "disco-tif-0.0.3.tar", last modified: Tue May 14 14:00:32 2024, max compression
```

## Comparing `disco-tif-0.0.2.tar` & `disco-tif-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 13:30:45.740183 disco-tif-0.0.2/
--rw-r--r--   0 bbloss     (501) staff       (20)      157 2024-04-17 13:28:35.000000 disco-tif-0.0.2/HISTORY.md
--rw-r--r--   0 bbloss     (501) staff       (20)     1077 2024-04-17 12:41:43.000000 disco-tif-0.0.2/LICENSE.md
--rw-r--r--   0 bbloss     (501) staff       (20)      177 2024-04-17 08:10:11.000000 disco-tif-0.0.2/MANIFEST.in
--rw-r--r--   0 bbloss     (501) staff       (20)      502 2024-04-17 13:30:45.739960 disco-tif-0.0.2/PKG-INFO
--rw-r--r--   0 bbloss     (501) staff       (20)     5149 2024-04-17 13:23:53.000000 disco-tif-0.0.2/README.md
-drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 13:30:45.738670 disco-tif-0.0.2/disco_tif/
--rw-r--r--   0 bbloss     (501) staff       (20)        0 2024-04-16 12:56:23.000000 disco-tif-0.0.2/disco_tif/__init__.py
--rw-r--r--   0 bbloss     (501) staff       (20)     1980 2024-04-16 13:04:31.000000 disco-tif-0.0.2/disco_tif/geotiff_plotting.py
--rw-r--r--   0 bbloss     (501) staff       (20)     8979 2024-04-16 16:04:04.000000 disco-tif-0.0.2/disco_tif/hillshades_pca.py
--rw-r--r--   0 bbloss     (501) staff       (20)    19512 2024-04-17 12:13:28.000000 disco-tif-0.0.2/disco_tif/process_sb_tiff.py
--rw-r--r--   0 bbloss     (501) staff       (20)     8901 2024-04-16 13:18:49.000000 disco-tif-0.0.2/disco_tif/write_mapfile.py
-drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-04-17 13:30:45.739710 disco-tif-0.0.2/disco_tif.egg-info/
--rw-r--r--   0 bbloss     (501) staff       (20)      502 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/PKG-INFO
--rw-r--r--   0 bbloss     (501) staff       (20)      352 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/SOURCES.txt
--rw-r--r--   0 bbloss     (501) staff       (20)        1 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/dependency_links.txt
--rw-r--r--   0 bbloss     (501) staff       (20)       62 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/requires.txt
--rw-r--r--   0 bbloss     (501) staff       (20)       10 2024-04-17 13:30:45.000000 disco-tif-0.0.2/disco_tif.egg-info/top_level.txt
--rw-r--r--   0 bbloss     (501) staff       (20)       38 2024-04-17 13:30:45.740232 disco-tif-0.0.2/setup.cfg
--rw-r--r--   0 bbloss     (501) staff       (20)      855 2024-04-17 13:29:39.000000 disco-tif-0.0.2/setup.py
+drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-05-14 14:00:32.583298 disco-tif-0.0.3/
+-rw-r--r--   0 bbloss     (501) staff       (20)      157 2024-04-17 13:28:35.000000 disco-tif-0.0.3/HISTORY.md
+-rw-r--r--   0 bbloss     (501) staff       (20)     1077 2024-04-17 12:41:43.000000 disco-tif-0.0.3/LICENSE.md
+-rw-r--r--   0 bbloss     (501) staff       (20)      177 2024-04-17 08:10:11.000000 disco-tif-0.0.3/MANIFEST.in
+-rw-r--r--   0 bbloss     (501) staff       (20)      510 2024-05-14 14:00:32.583037 disco-tif-0.0.3/PKG-INFO
+-rw-r--r--   0 bbloss     (501) staff       (20)     5149 2024-04-17 13:23:53.000000 disco-tif-0.0.3/README.md
+drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-05-14 14:00:32.581592 disco-tif-0.0.3/disco_tif/
+-rw-r--r--   0 bbloss     (501) staff       (20)        0 2024-05-09 08:45:10.000000 disco-tif-0.0.3/disco_tif/__init__.py
+-rw-r--r--   0 bbloss     (501) staff       (20)     2402 2024-05-09 16:12:22.000000 disco-tif-0.0.3/disco_tif/geotiff_plotting.py
+-rw-r--r--   0 bbloss     (501) staff       (20)     9625 2024-05-09 16:06:45.000000 disco-tif-0.0.3/disco_tif/hillshades_pca.py
+-rw-r--r--   0 bbloss     (501) staff       (20)    22341 2024-05-10 10:35:55.000000 disco-tif-0.0.3/disco_tif/look_up_tables.py
+-rw-r--r--   0 bbloss     (501) staff       (20)    28219 2024-05-14 13:41:38.000000 disco-tif-0.0.3/disco_tif/process_sb_tiff.py
+-rw-r--r--   0 bbloss     (501) staff       (20)     9185 2024-05-09 16:15:31.000000 disco-tif-0.0.3/disco_tif/write_mapfile.py
+drwxr-xr-x   0 bbloss     (501) staff       (20)        0 2024-05-14 14:00:32.582754 disco-tif-0.0.3/disco_tif.egg-info/
+-rw-r--r--   0 bbloss     (501) staff       (20)      510 2024-05-14 14:00:32.000000 disco-tif-0.0.3/disco_tif.egg-info/PKG-INFO
+-rw-r--r--   0 bbloss     (501) staff       (20)      380 2024-05-14 14:00:32.000000 disco-tif-0.0.3/disco_tif.egg-info/SOURCES.txt
+-rw-r--r--   0 bbloss     (501) staff       (20)        1 2024-05-14 14:00:32.000000 disco-tif-0.0.3/disco_tif.egg-info/dependency_links.txt
+-rw-r--r--   0 bbloss     (501) staff       (20)       70 2024-05-14 14:00:32.000000 disco-tif-0.0.3/disco_tif.egg-info/requires.txt
+-rw-r--r--   0 bbloss     (501) staff       (20)       10 2024-05-14 14:00:32.000000 disco-tif-0.0.3/disco_tif.egg-info/top_level.txt
+-rw-r--r--   0 bbloss     (501) staff       (20)       38 2024-05-14 14:00:32.583358 disco-tif-0.0.3/setup.cfg
+-rw-r--r--   0 bbloss     (501) staff       (20)      826 2024-05-14 13:52:37.000000 disco-tif-0.0.3/setup.py
```

### Comparing `disco-tif-0.0.2/LICENSE.md` & `disco-tif-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `disco-tif-0.0.2/README.md` & `disco-tif-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `disco-tif-0.0.2/disco_tif/hillshades_pca.py` & `disco-tif-0.0.3/disco_tif/hillshades_pca.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,124 +1,171 @@
-import os
+# import os
 import rasterio
-import earthpy as et
+# import earthpy as et
 import earthpy.spatial as es
-import earthpy.plot as ep
-import matplotlib as mpl
-from matplotlib import pyplot as plt
-from matplotlib.colors import LinearSegmentedColormap
-import datetime
+# import earthpy.plot as ep
+# import matplotlib as mpl
+# from matplotlib import pyplot as plt
+# from matplotlib.colors import LinearSegmentedColormap
+# import datetime
 import numpy as np
-import pandas as pd
+# import pandas as pd
 import sklearn.decomposition
 
-#import process_sb_tiff
+# import process_sb_tiff
 import disco_tif.geotiff_plotting
 
 #################################################
 
 def build_hs_az_al(start_al, al_inc, num_al_angles, start_az, num_az_angles):
-    azimuths = np.linspace(start_az, start_az+360, num_az_angles+1) # degrees 0=360, number of divisions + 1 because start=end
-    filt = azimuths>=360
-    while filt.sum()>0:
+    """description
+Input Parameters:
+    - start_al:
+    
+    - al_inc:
+    
+    - num_al_angles:
+    
+    - start_az:
+    
+    - num_az_angles
+    """
+    azimuths = np.linspace(start_az, start_az+360, num_az_angles+1)  # degrees 0=360, number of divisions + 1 because start=end
+    filt = azimuths >= 360
+    while filt.sum() > 0:
         azimuths[filt] = azimuths[filt]-360
-        filt = azimuths>=360
+        filt = azimuths >= 360
     azimuths = azimuths[:-1].astype(int).tolist()
     azimuths = sorted(azimuths)
     print(f"azimuths = {azimuths}")
     
     altitudes = np.linspace(start_al, (al_inc*num_al_angles)+start_al, num_al_angles+1)
     altitudes = altitudes[:-1].astype(int).tolist()
     print(f"altitudes = {altitudes}")
     return azimuths, altitudes
 
 def write_raster_dict_data_to_geotiff(single_band_tiff_path, origprofile, raster_data_dict, len_hs=None):
+    """description
+Input Parameters:
+    - single_band_tiff_path:
+    
+    - origprofile:
+    
+    - raster_data_dict:
+    
+    - len_hs=None
+    """
     for key, value in raster_data_dict.items():
         if 'component' in key:
             assert len_hs is not None, "'len_hs' cannot be none if passing in a pca_dictionary_object"
             new_tiff_path = f"{single_band_tiff_path.split('.tif')[0]}_hillshade_pca{len_hs}-{key}.tif"
         else:
             new_tiff_path = f"{single_band_tiff_path.split('.tif')[0]}_hillshade_{key}.tif"
         
         newprofile = origprofile.copy()
-        newprofile.update(dtype=str((value[0,0]).dtype), nodata=np.nan)
+        newprofile.update(dtype=str((value[0, 0]).dtype), nodata=np.nan)
            
         with rasterio.open(new_tiff_path, 'w', **newprofile) as dst:
             dst.write(arr=value, indexes=1, masked=True)
     
         print(f"New single-channel geotiff generated successfully: '{new_tiff_path}'")
         
 
 def MakeHillShadePCA(hillshades, plot_figures=False, raster_data=None, cmap='terrain', n_components=3):
+    """description
+Input Parameters:
+    - hillshades:
+    
+    - plot_figures=False:
+    
+    - raster_data=None:
+    
+    - cmap='terrain':
+    
+    - n_components=3
+    """
     if plot_figures:
         assert raster_data is not None, "raster data must be supplied if plot_figures is true"
         
     NoNanIndicies = np.argwhere(~np.isnan(hillshades[list(hillshades.keys())[0]].flatten())).flatten()
 
     n_samples = len(NoNanIndicies)
     n_features = len(hillshades.keys())
     assert n_features >= 4, "There must be at least 4 hillshades to produce a PCA"
     
     flat_hillshades = np.ones([n_samples, n_features]) * np.nan
     
-    feature_ind=-1
+    feature_ind = -1
     for key, value in hillshades.items():
-        feature_ind+=1
+        feature_ind += 1
         value = value.flatten()
         value = value[NoNanIndicies]
-        flat_hillshades[:,feature_ind]=value
+        flat_hillshades[:, feature_ind] = value
     
-    assert np.isnan(flat_hillshades).sum()==0, "There can be no NaN's when performing a pca"
+    assert np.isnan(flat_hillshades).sum() == 0, "There can be no NaN's when performing a pca"
     
-    pca = sklearn.decomposition.PCA(n_components = n_components)
+    pca = sklearn.decomposition.PCA(n_components=n_components)
     
     pcaout = pca.fit(flat_hillshades).transform(flat_hillshades)
-    pcaout
-    
-    pcaout.shape
-    
+
     data = hillshades[list(hillshades.keys())[0]]
     
     nrow = data.shape[0]
     ncol = data.shape[1]
     nlay = len(pcaout[0])
     
     dumarray = np.ones([nrow * ncol])*np.nan
     
-    pcaComponents={}
-    for ilay in range(0,len(pcaout[0])):
+    pcaComponents = {}
+    for ilay in range(0, len(pcaout[0])):
         tdat = dumarray.copy()
         nowdat = pcaout[:, ilay]
         tdat[NoNanIndicies] = nowdat
-        pcaComponents[f'component_{ilay+1}'] = tdat.reshape([nrow,ncol], order='C')
+        pcaComponents[f'component_{ilay+1}'] = tdat.reshape([nrow, ncol], order='C')
     
     if plot_figures:
         # plot the pca outputs
         disco_tif.geotiff_plotting.plot_greyband_only(raster_data_dict=pcaComponents,
-                                                               nrows=1,
-                                                               ncols=n_components)
+                                                      nrows=1,
+                                                      ncols=n_components)
         disco_tif.geotiff_plotting.plot_color_raster_with_greyscale_overlay(raster_data=raster_data,
-                                                                                     cmap=cmap,
-                                                                                     raster_data_dict=pcaComponents,
-                                                                                     nrows=1,
-                                                                                     ncols=n_components)
+                                                                            cmap=cmap,
+                                                                            raster_data_dict=pcaComponents,
+                                                                            nrows=1,
+                                                                            ncols=n_components)
     
     # pcaComponents['component_1_0_1'] = (           pcaComponents['component_1'] - np.nanmin(pcaComponents['component_1'])) / \
     #                                    (np.nanmax(pcaComponents['component_1']) - np.nanmin(pcaComponents['component_1']))
     
     # pcaComponents['component_2_0_1'] = (           pcaComponents['component_2'] - np.nanmin(pcaComponents['component_2'])) / \
     #                                    (np.nanmax(pcaComponents['component_2']) - np.nanmin(pcaComponents['component_2']))
     
     # pcaComponents['component_3_0_1'] = (           pcaComponents['component_3'] - np.nanmin(pcaComponents['component_3'])) / \
     #                                    (np.nanmax(pcaComponents['component_3']) - np.nanmin(pcaComponents['component_3']))
                                                                                                                    
     return pcaComponents
     
 
 def build_hillshade(single_band_tiff_path, data_min_max,  hs_azimuths, hs_altitudes, cmap='terrain', process_pca=False, plot_figures=False):
+    """description
+Input Parameters:
+    - single_band_tiff_path:
+    
+    - data_min_max:
+    
+    - hs_azimuths:
+    
+    - hs_altitudes:
+    
+    - cmap='terrain':
+    
+    - process_pca=False:
+    
+    - plot_figures=False
+    """
     # read geotiff and minimally process for the colormap function
     with rasterio.open(single_band_tiff_path, 'r') as src:
         data = src.read(1)  # Read the first band
         no_data_value = src.nodata  # Get the no-data value from the GeoTIFF
         epsg_code = src.crs.to_epsg() if src.crs else None
         origprofile = src.profile
         width = src.width 
@@ -128,54 +175,54 @@
     # Clip data values to the specified range
     clipped_data = np.clip(data, data_min_max[0], data_min_max[1])
     
     nan_data = data.copy().astype(float)
     nan_clipped_data = clipped_data.copy().astype(float)
     
     if no_data_value is not None:
-        nan_data[data==no_data_value]=np.nan
-        nan_clipped_data[data==no_data_value]=np.nan
+        nan_data[data == no_data_value] = np.nan
+        nan_clipped_data[data == no_data_value] = np.nan
 
     #
     if plot_figures:
         # Plot the data
         disco_tif.geotiff_plotting.plot_singleband_raster(raster_data=nan_clipped_data,
-                                                cmap=cmap,
-                                                title=f"{single_band_tiff_path} Without Hillshade",
-                                                ax=None)
+                                                          cmap=cmap,
+                                                          title=f"{single_band_tiff_path} Without Hillshade",
+                                                          ax=None)
        
     # calculate the hillshade for  all combination fo azimuths and altitudes
     num_hillshades = len(hs_azimuths) * len(hs_altitudes)
     # it it expensive to generate all of these hillshades and do the pca on them => we limit the number to something reasonable # 8 azimuths at 3 angles will produce 24 hillshades. ### what is reasonable here?
     max_num_hs = 24
-    assert num_hillshades<=max_num_hs, f"Only {max_num_hs} azimuth-altidude combinations can be used to calculate a Hillshade PCA but {num_hillshades} were provided"
+    assert num_hillshades <= max_num_hs, f"Only {max_num_hs} azimuth-altitude combinations can be used to calculate a Hillshade PCA but {num_hillshades} were provided"
 
     hillshades = {}
     for az_ind, my_azimuth in enumerate(hs_azimuths):
         for al_ind, my_altitude in enumerate(hs_altitudes):
             # Create and plot the hillshade with earthpy
             txt_my_azimuth = f"00{my_azimuth}"[-3:]
             txt_my_altitude = f"0{my_altitude}"[-2:]
             hskey = f'az{txt_my_azimuth}_al{txt_my_altitude}'
             hillshades[hskey] = es.hillshade(nan_data, azimuth=my_azimuth, altitude=my_altitude)
 
     if plot_figures:
         # plot the hillshades 
         disco_tif.geotiff_plotting.plot_greyband_only(raster_data_dict=hillshades,
-                                                               nrows=max([len(hs_azimuths), len(hs_altitudes)]),
-                                                               ncols=min([len(hs_azimuths), len(hs_altitudes)]))
+                                                      nrows=max([len(hs_azimuths), len(hs_altitudes)]),
+                                                      ncols=min([len(hs_azimuths), len(hs_altitudes)]))
         # plot geotiff overlain with the hillshades
         disco_tif.geotiff_plotting.plot_color_raster_with_greyscale_overlay(raster_data=nan_clipped_data,
-                                                                                     raster_data_dict=hillshades,
-                                                                                     nrows=max([len(hs_azimuths), len(hs_altitudes)]),
-                                                                                     ncols=min([len(hs_azimuths), len(hs_altitudes)]),
-                                                                                     cmap=cmap)
+                                                                            raster_data_dict=hillshades,
+                                                                            nrows=max([len(hs_azimuths), len(hs_altitudes)]),
+                                                                            ncols=min([len(hs_azimuths), len(hs_altitudes)]),
+                                                                            cmap=cmap)
 
     write_raster_dict_data_to_geotiff(single_band_tiff_path, origprofile, hillshades)
 
     if not process_pca:
         return hillshades
     elif process_pca:
-        assert num_hillshades>=4, f'Need at least 4 azimuth-altitude combinations, only {num_hillshades} were provided'
+        assert num_hillshades >= 4, f'Need at least 4 azimuth-altitude combinations, only {num_hillshades} were provided'
         pcaComponents = MakeHillShadePCA(hillshades, plot_figures, raster_data=nan_clipped_data, cmap=cmap)
         write_raster_dict_data_to_geotiff(single_band_tiff_path, origprofile, pcaComponents, len_hs=len(hillshades.keys()))
         return hillshades, pcaComponents
```

### Comparing `disco-tif-0.0.2/disco_tif/process_sb_tiff.py` & `disco-tif-0.0.3/disco_tif/process_sb_tiff.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,419 +1,555 @@
 import os
 import rasterio
-import earthpy as et
-import earthpy.spatial as es
+# import earthpy as et
+# import earthpy.spatial as es
 import earthpy.plot as ep
 import matplotlib as mpl
 from matplotlib import pyplot as plt
 from matplotlib.colors import LinearSegmentedColormap
 import datetime
 import numpy as np
-import pandas as pd
-import sklearn.decomposition
+# import pandas as pd
+# import sklearn.decomposition
+import copy
+
+import disco_tif.look_up_tables
 
 ######################################
 
-def nowTime():
+
+def now_time():
     return datetime.datetime.now().strftime("%H:%M:%S")
 def now():
     return datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
 def snow():
     return datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
 def today():
     return datetime.datetime.now().strftime("%Y-%m-%d")
 def stoday():
     return datetime.datetime.now().strftime("%Y%m%d")
 
 ######################################
 
+
 def hex_to_rgb(hexcolor):
     if '#' in hexcolor:
         hexcolor = hexcolor.split('#')[1]
     rgb = []
     for i in (0, 2, 4):
         decimal = int(hexcolor[i:i+2], 16)
         rgb.append(decimal)
     return rgb[0], rgb[1], rgb[2]
+
+
 def rgb_to_hex(r, g, b):
     return '#{:02x}{:02x}{:02x}'.format(r, g, b)
-           
+
+
 ######################################
 
 # define custom color steps  - Order matters
-EMerald_custom_colors_hexcolorcodes = ['#0000ff', # Blue
-                                       '#01ffff', # Cyan
-                                       '#3fca3f', # Green
-                                       '#f19898', # Salmon
-                                       '#deb201', # Tan
-                                       '#896651', # Brown
-                                       '#f1bfff', # Light_Purple
-                                       '#fffafc', # Near_White
+EMerald_custom_colors_hexcolorcodes = ['#0000ff',  # Blue
+                                       '#01ffff',  # Cyan
+                                       '#3fca3f',  # Green
+                                       '#f19898',  # Salmon
+                                       '#deb201',  # Tan
+                                       '#896651',  # Brown
+                                       '#f1bfff',  # Light_Purple
+                                       '#fffafc',  # Near_White
                                       ]
 
+# define the number of the colors for the colormap
 colormap_length = 256
 
 ######################################
 
-def build_EMerald_terrain_colormap(breaks_by_percentages):
-    EMerald_custom_colors_rgb=[]
-    for hexcode in EMerald_custom_colors_hexcolorcodes:
+
+def build_custom_colormap(breaks_by_percentages, custom_color_hex, new_cmap_name="Custom_Colormap"):
+    """ Function to take a sorted array of percentage-break-points (i.e. breaks_by_percentages) and applies it to the color-list (i.e. custom_color_hex) colormap. The length of the breaks_by_percentages array should be the same length as custom_color_hex (length=8 for EMerald_custom_colors_hexcolorcodes) and range from 0 to 1
+
+Input Parameters:
+    - breaks_by_percentages: List of breakpoints in decimal-percentages of data. [0.0, 0.3, 0.6, 0.9, 1.0]
+        - note - if starting and ending points are not at 0 and 1, respectively, the program will prepend and append the list with 0 and 1.
+            The program will also copy the first and last colors in custom_color_hex to the new low and high percentages appended
+
+    - custom_color_hex: List of color hex codes to generate the colormap from. i.e. ['#000000', '#aaaaaa', '#dddddd', '#eeeeee', '#ffffff']
+
+    - new_cmap_name: String name to use for the generation of the new cmap.
+        defualt: "Custom_Colormap"
+    """
+    breaks_by_percentages = copy.deepcopy(breaks_by_percentages)
+    custom_color_hex = copy.deepcopy(custom_color_hex)
+
+    if len(breaks_by_percentages) != len(custom_color_hex):  # it's ok for these to be different, but only by 1. we just omit the dark blue color if using EMerald_custom_colormap
+        custom_color_hex = custom_color_hex[1:]
+    else:
+        pass
+
+    assert len(breaks_by_percentages) == len(custom_color_hex), "The length of the breaks_by_percentages list but be the same as the length of custom_color_hex"
+
+    if breaks_by_percentages[0] != 0:
+        breaks_by_percentages.insert(0, 0)
+        custom_color_hex.insert(0, custom_color_hex[0])
+    if breaks_by_percentages[-1] != 1:
+        breaks_by_percentages.append(1)
+        custom_color_hex.append(custom_color_hex[-1])
+
+    custom_color_rgb = []
+    for hexcode in custom_color_hex:
         temp = hex_to_rgb(hexcode) 
-        EMerald_custom_colors_rgb.append([np.round(temp[0]/(colormap_length-1), 3), 
+        custom_color_rgb.append([np.round(temp[0]/(colormap_length-1), 3), 
                                           np.round(temp[1]/(colormap_length-1), 3), 
                                           np.round(temp[2]/(colormap_length-1), 3)])
-    colorarray = np.array(EMerald_custom_colors_rgb)
-    colorarray
+    custom_color_array = np.array(custom_color_rgb)
 
-    if breaks_by_percentages[1]==0: # if second entry is 0 we know that there are no negative numbers and we should ignore blue
-        sn=1
+    if breaks_by_percentages[1] == 0:  # if second entry is 0 we know that there are no negative numbers and we should ignore blue
+        sn = 1
     else:
-        sn=0
-    EMeraldCustomColormap_cdict = {'red':   [(breaks_by_percentages[ijk],  colorarray[ijk,0], colorarray[ijk,0]) for ijk in range(sn, len(breaks_by_percentages))],
-                         'green': [(breaks_by_percentages[ijk],  colorarray[ijk,1], colorarray[ijk,1]) for ijk in range(sn, len(breaks_by_percentages))],
-                         'blue':  [(breaks_by_percentages[ijk],  colorarray[ijk,2], colorarray[ijk,2]) for ijk in range(sn, len(breaks_by_percentages))],
-                        }
-    EMeraldCustomColormap = LinearSegmentedColormap("EMerald_Custom_Colormap", EMeraldCustomColormap_cdict, N=colormap_length)
-    EMeraldCustomColormap
-    
+        sn = 0
+
+    # print(f"breaks_by_percentages = {breaks_by_percentages}")
+    CustomColormap_cdict = {'red':   [(breaks_by_percentages[ijk],  custom_color_array[ijk, 0], custom_color_array[ijk, 0]) for ijk in range(sn, len(breaks_by_percentages))],
+                            'green': [(breaks_by_percentages[ijk],  custom_color_array[ijk, 1], custom_color_array[ijk, 1]) for ijk in range(sn, len(breaks_by_percentages))],
+                            'blue':  [(breaks_by_percentages[ijk],  custom_color_array[ijk, 2], custom_color_array[ijk, 2]) for ijk in range(sn, len(breaks_by_percentages))],
+                           }
+    CustomColormap = LinearSegmentedColormap(new_cmap_name, CustomColormap_cdict, N=colormap_length)
+
+    return CustomColormap
+
+
+def build_EMerald_terrain_colormap(breaks_by_percentages):
+    EMeraldCustomColormap = build_custom_colormap(breaks_by_percentages=breaks_by_percentages,
+                                                  custom_color_hex=copy.deepcopy(EMerald_custom_colors_hexcolorcodes),
+                                                  new_cmap_name="EMerald_Custom_Colormap")
     return EMeraldCustomColormap
 
 ######################################
 
-def make_percentile_array(data_min_max, data, no_data_value, cmap_method='pseudo_hist_norm', plot_histograms=False):
+
+def make_percentile_array(data_min_max,
+                          data,
+                          no_data_value,
+                          cmap_method='pseudo_hist_norm',
+                          color_list=None,
+                          plot_histograms=False):
+    """Function to build a data driven percentile array based on the cmap method specified.
+Input Parameters:
+    - data_min_max: list containing the minimum and maximum values to display. values outside this range will be saturated to the end members.
+        ex: [min, max]
+
+    - data: 2D array of cell values of the raster.
+        ex: ([[x1y1, ..., xny1], [x1y2, ..., xny2], ..., [x1yn, ..., xnyn]])
+
+    - no_data_value: Value that specifies the no_data_value
+    
+    - cmap_method: parameter to tell the program how to bin the data. Options are 'pseudo_hist_norm', or 'pseudo_linear'
+        Default:  'pseudo_hist_norm'
+
+    - color_list: list of colors, global variable
+        Default: EMerald_custom_colors_hexcolorcodes
+    
+    - plot_histograms: boolean parameter for plotting the percentage break points on top of a histogram of the data
+        Default:  False
+    """
+    if color_list is None:
+        color_list = copy.deepcopy(EMerald_custom_colors_hexcolorcodes)
+    else:
+        color_list = copy.deepcopy(color_list)
+
     if data_min_max is not None:
-        assert len(data_min_max)==2, 'len of data_min_max must be 2'
+        assert len(data_min_max) == 2, 'len of data_min_max must be 2'
         assert data_min_max[0] < data_min_max[1], 'first value must be less than second value'
         assert data_min_max[1] > 0, 'This should really be a bigger number, but at least this will save dividing by a zero...'
 
-    datatype = str(data[0,0].dtype)
-    num_color = len(EMerald_custom_colors_hexcolorcodes)
-    bz_num_color = 1 #number of colors for below zero
-    az_num_color = num_color-bz_num_color-1 # number of intervals
-
-    z_data = data.copy()
-    z_data = z_data.flatten()
-    bz_data = z_data[z_data<0]
-    az_data = z_data[z_data>=0]
-    norm_az_data = (az_data.copy() - np.min(az_data)) / (np.max(az_data) - np.min(az_data)) # shift to zero, then normalize by the range
-
-    if cmap_method=='pseudo_linear':
-        az_min=np.max([0, data_min_max[0]]) # above_zero_min: if data_min_max[0]<0, then 0; if data_min_max[0]>=0, then data_min_max[0].
-        #print(f"az_min = {az_min}")
-        az_data_breaks = np.round(np.linspace(az_min, data_min_max[1], az_num_color+1))
-        #print(f"az_data_breaks = {az_data_breaks}")
+    color_list = color_list.copy()
+
+    datatype = str(data[0, 0].dtype)
+
+    if data_min_max[0] < 0:
+        bz_num_color = 1  # number of colors for below zero
+    else:
+        bz_num_color = 0  # number of colors for below zero
+        color_list = color_list[1:]
+
+    num_color = len(color_list)
+    az_num_color = num_color-bz_num_color  # number of intervals
+
+    clip_data = data.copy()
+    clip_data = clip_data.flatten()
+    # clip_data = clip_data.astype(float)
+    if no_data_value is not None:
+        clip_data = clip_data[clip_data != no_data_value]
+    clip_data = np.clip(clip_data, data_min_max[0], data_min_max[1])
+    az_clip_data = clip_data.copy()
+    az_clip_data = az_clip_data[az_clip_data >= 0]
+
+    if cmap_method == 'pseudo_linear':
+        az_min = np.max([0, data_min_max[0]])  # above_zero_min: if data_min_max[0]<0, then 0; if data_min_max[0]>=0, then data_min_max[0].
+        # print(f"az_min = {az_min}")
+        az_data_breaks = np.round(np.linspace(az_min, data_min_max[1], az_num_color))
+        # print(f"az_data_breaks = {az_data_breaks}")
         
-    elif cmap_method=='pseudo_hist_norm':
-        my_percentiles = np.linspace(0, 100, az_num_color+1)
+    elif cmap_method == 'pseudo_hist_norm':
+        my_percentiles = np.linspace(0, 100, az_num_color)
         my_percentiles = my_percentiles[1:-1]
-        #print(f"my_percentiles = {my_percentiles}")
+        # print(f"my_percentiles = {my_percentiles}")
         
-        az_data_breaks = np.percentile(a=az_data, q=my_percentiles)
-        if data_min_max[0]<0:
-            az_data_breaks = np.insert(az_data_breaks, 0, 0) #prepend with: if data_min_max[0]<0, then 0; 
+        az_data_breaks = np.percentile(a=az_clip_data, q=my_percentiles)
+        if data_min_max[0] < 0:
+            az_data_breaks = np.insert(az_data_breaks, 0, 0)  # prepend with: if data_min_max[0]<0, then 0;
         else:    
-            az_data_breaks = np.insert(az_data_breaks, 0, data_min_max[0]) #prepend with: if data_min_max[0]>=0, then data_min_max[0]
+            az_data_breaks = np.insert(az_data_breaks, 0, data_min_max[0])  # prepend with: if data_min_max[0]>=0, then data_min_max[0]
         az_data_breaks = np.append(az_data_breaks, data_min_max[1])
-        #print(f"az_data_breaks = {az_data_breaks}")
+        # print(f"az_data_breaks = {az_data_breaks}")
     
-    data_breaks = [data_min_max[0]]
-    #print(f"data_breaks = {data_breaks}")
+    if data_min_max[0] < 0:
+        data_breaks = [data_min_max[0]]
+    else:
+        data_breaks = []
+    # print(f"data_breaks = {data_breaks}")
     data_breaks.extend(az_data_breaks)
     data_breaks = np.array(data_breaks)
     data_breaks = data_breaks.astype(datatype).tolist()
-    #print(f"data_breaks = {data_breaks}")
+    # print(f"data_breaks = {data_breaks}")
     
-    percentile_breaks = np.round((np.array(data_breaks) - data_min_max[0]) / (data_min_max[1] - data_min_max[0]), 4)
-    percentile_breaks = percentile_breaks.tolist()
-    #print(f"percentile_breaks = {percentile_breaks}")
+    no_dum_data = data.copy()
+    no_dum_data = no_dum_data.flatten()
+    no_dum_data = no_dum_data.astype(float)
+    if no_data_value is not None:
+        no_dum_data[no_dum_data == no_data_value] = np.nan
+    abs_min_max = [np.nanmin(no_dum_data), np.nanmax(no_dum_data)]
 
     if plot_histograms:
-        no_dum_data = data.copy()
-        no_dum_data = no_dum_data.flatten()
-        no_dum_data = no_dum_data.astype(float)
-        if no_data_value is not None:
-            no_dum_data[no_dum_data==no_data_value] = np.nan
-        norm_no_dum_data = (no_dum_data.copy() - data_min_max[0]) / (data_min_max[1] - data_min_max[0]) # shift to zero, then normalize by the range
+        norm_no_dum_data = (no_dum_data.copy() - abs_min_max[0]) / (abs_min_max[1] - abs_min_max[0]) # shift to zero, then normalize by the range
         
-        fig, axs = plt.subplots(nrows=2, ncols=1, sharey=True)
-        
-        axs[0].hist(no_dum_data, bins=min(data_min_max[1]-data_min_max[0], 100))
-        ylimits = axs[0].get_ylim()
-        for db in data_breaks:
-            axs[0].plot([db, db], [0, ylimits[1]])
-        axs[0].set_title('Breaks by data values')
-    
-        axs[1].hist(norm_no_dum_data, bins=min(data_min_max[1]-data_min_max[0], 100))
-        for pb in percentile_breaks:
-            axs[1].plot([pb, pb], [0, ylimits[1]])
-        axs[1].set_title('Breaks by percentage of data')
+        fig, ax = plt.subplots(nrows=1, ncols=1, sharey=True, figsize=[12, 3])
+
+        ax.hist(no_dum_data, bins=min(abs_min_max[1]-abs_min_max[0], 100))
+        ylimits = ax.get_ylim()
+        ax.plot([abs_min_max[0], abs_min_max[0]], [0, ylimits[1]], c='k', ls=":", lw=1, label=abs_min_max[0])
+        for ii, db in enumerate(data_breaks):
+            ax.plot([db, db], [0, ylimits[1]], c='k', lw=2, label=None)
+            ax.plot([db, db], [0, ylimits[1]], c=color_list[ii], lw=1, label=db)
+        ax.plot([abs_min_max[1], abs_min_max[1]], [0, ylimits[1]], c='k', ls="--", lw=1, label=abs_min_max[1])
+        ax.set_ylim(ylimits)
+        ax.legend(loc='center right', bbox_to_anchor=(1.11, 0.5))
+        ax.set_title('Breaks by data values')
         
-        plt.tight_layout(); plt.show()
+        plt.tight_layout()
+        plt.show()
 
-    return percentile_breaks, data_breaks
+    return data_breaks
 
 ######################################
 
-def calc_data_min_max(data, no_data_value, clip_perc, min_max_method='percentile'):
-    if min_max_method=='data_absolute':
+
+def calc_data_min_max(data, no_data_value, clip_perc=None, min_max_method='data_absolute'):
+    """Function to calculate the min max values of the data
+Input Parameters:
+    - data: 2D array of cell values of the raster.
+        ex: ([[x1y1, ..., xny1], [x1y2, ..., xny2], ..., [x1yn, ..., xnyn]])
+
+    - no_data_value: value the defines the no-data-value
+    
+    - clip_perc: list of percentile (quartile) values to clip the data to. i.e. [1, 99] for clip to the fist and 99th percentiles of the data (essentially, exclude erroneous high or low points). This is only relevant if the min_max_method is 'percentile'.
+        Default: None
+        
+    - min_max_method: defines how to define the min_max method. Options are: 'data_absolute', or 'percentile'
+        Default:  'data_absolute'
+    """
+    if min_max_method == 'data_absolute':
         # using absolute min max from data
         if no_data_value is not None:
-            data_min_max = [np.min(data[data!=no_data_value]), np.max(data[data!=no_data_value])]
+            data_min_max = [np.min(data[data != no_data_value]), np.max(data[data != no_data_value])]
         else:
             data_min_max = [np.min(data), np.max(data)]
         
-    elif min_max_method=='percentile':
+    elif min_max_method == 'percentile':
         # using percentiles of data (defined in the import statement)
         if no_data_value is not None:
-            data_min_max = np.percentile(a=data[data!=no_data_value], q=clip_perc)
+            data_min_max = np.percentile(a=data[data != no_data_value], q=clip_perc)
         else:
             data_min_max = np.percentile(a=data, q=clip_perc)
         data_min_max = np.round(data_min_max)
         data_min_max = data_min_max.astype(int)
         data_min_max = list(data_min_max)
     return data_min_max
 
 ######################################
 
-def build_1_component_color_tables(cmap, data_breaks, data, no_data_value, new_multiband_lut_path):
-    EMerald_colors_rgb = pd.DataFrame()
-    for ii in range(0, len(cmap)):
-        hexcolor = cmap[ii]
-        EMerald_colors_rgb.loc[ii, ['r']] = hex_to_rgb(hexcolor)[0]
-        EMerald_colors_rgb.loc[ii, ['g']] = hex_to_rgb(hexcolor)[1]
-        EMerald_colors_rgb.loc[ii, ['b']] = hex_to_rgb(hexcolor)[2]
-    
-    if len(EMerald_colors_rgb) == len(data_breaks):
-        EMerald_colors_rgb['data_val'] = np.array(data_breaks)
-    else:
-        print("there's an odd mismatch in length of 'EMerald_colors_rgb' and 'data_breaks'")
 
-    outfilepaths=[]
-    for rgb in ['r', 'g', 'b']:
-        lut_str = f"{EMerald_colors_rgb.loc[0, 'data_val']}: {EMerald_colors_rgb.loc[0, rgb]}" 
-        for row in range(1, len(EMerald_colors_rgb)):
-                lut_str = f"{lut_str}, {EMerald_colors_rgb.loc[row, 'data_val']}: {int(np.round(EMerald_colors_rgb.loc[row, rgb]))}"
-        tname=f"{new_multiband_lut_path}_{rgb}.lut"
-        outfilepaths.append(tname)
-        with open(tname, 'w') as lut_file_out:
-            lut_file_out.write(lut_str)
-    
-    lut_str = f"{np.array(no_data_value, dtype=data[0,0].dtype).tolist()}: 0, {data_breaks[0]}: 255, {data_breaks[-1]}:255"
-    tname=f"{new_multiband_lut_path}_a.lut"
-    outfilepaths.append(tname)    
-    with open(tname, 'w') as lut_file_out:
-        lut_file_out.write(lut_str)
+def rast_dat_to_uint8_data(rast_dat, data_min_max, no_data_value):
+    """Function to map raster data to uint8 data. no-data values are mapped to 0 if they exist and then data would be mapped 1-255. If no_data is none then the data will be mapped 0-255
 
-    return outfilepaths
+    """
+    rast_dat_with_nan = rast_dat.copy().astype(float)
     
-######################################
+    if no_data_value is not None:
+        filt = rast_dat == no_data_value
+        rast_dat_with_nan[filt] = np.nan
 
-def build_4_component_color_tables(single_band_tiff_path, cmap, data, no_data_value, percentile_breaks, data_breaks, outfile):
-    pathparts = single_band_tiff_path.split(os.path.sep)
-    destfolder = ''
-    for part in pathparts[:-1]:
-        destfolder=f"{destfolder}{part}{os.path.sep}"
+    clip_rast_dat_with_nan = np.clip(rast_dat_with_nan, data_min_max[0], data_min_max[1],)
     
-    index_breaks = np.round([id * 255 for id in percentile_breaks]).astype(int).tolist()
-    index_breaks
+    if no_data_value is None:
+        uint8_rast_dat_with_dumb = (np.round(((clip_rast_dat_with_nan - data_min_max[0]) / (data_min_max[1] - data_min_max[0])) * 255))
+    elif no_data_value is not None:
+        uint8_rast_dat_with_dumb = (np.round(((clip_rast_dat_with_nan - data_min_max[0]) / (data_min_max[1] - data_min_max[0])) * 254)+1)
+
+    if no_data_value is not None:
+        uint8_rast_dat_with_dumb[filt] = 0
+    uint8_rast_dat_with_dumb = uint8_rast_dat_with_dumb.astype('uint8')
+    return uint8_rast_dat_with_dumb
 
-    ph_colormap_df = pd.DataFrame((cmap._lut * 255).astype('uint8'), columns=['red', 'green', 'blue', 'alpha']).iloc[:256,:]
-    ph_colormap_df.loc[index_breaks,'data_breaks'] = data_breaks
-    ph_colormap_df['data_breaks'] = ph_colormap_df['data_breaks'].interpolate(method='linear').astype(type(data_breaks[0]))
-    
-    nan_ph_colormap_df = ph_colormap_df.copy()
-    nan_ph_colormap_df.loc[-1] = [0, 0, 0, 0, np.array(no_data_value, dtype=data[0,0].dtype).tolist()]
-    nan_ph_colormap_df.index = nan_ph_colormap_df.index + 1  # shifting index
-    nan_ph_colormap_df = nan_ph_colormap_df.sort_index()  # sorting by index
-    
-    #outfile = os.path.join(destfolder, outfile)
-    
-    qgisfile = f"{outfile}_qgis_color_table.txt"
-    ph_colormap_df.to_csv(qgisfile, index=False, header=False, columns=['data_breaks', 'red', 'green', 'blue', 'alpha', 'data_breaks'])
-    with open(qgisfile, 'r') as inlut:
-        origstuff=inlut.read()
-    with open(qgisfile, 'w') as outlut:
-        outlut.seek(0)
-        outlut.write(f"# EMerald Generated Color Map Export File for {single_band_tiff_path}\n")
-        outlut.write("INTERPOLATION:INTERPOLATED\n")
-        outlut.write(origstuff)
-
-    rgba_lut_file = f"{outfile}_lut.lut"
-    ph_colormap_df.to_csv(rgba_lut_file, index=False, header=False, columns=['data_breaks', 'red', 'green', 'blue', 'alpha'])
-    nan_rgba_lut_file = f"{outfile}_NaN_lut.lut"
-    nan_ph_colormap_df.to_csv(nan_rgba_lut_file, index=False, header=False, columns=['data_breaks', 'red', 'green', 'blue', 'alpha'])
-    
-    return [qgisfile, rgba_lut_file]
-    
 ######################################
 
-def make_rgba_tiff_from_single_Band(single_band_tiff_path, 
+
+def make_rgba_tiff_from_single_Band(single_band_tiff_path,
                                     data_min_max=None, 
                                     min_max_method='percentile', 
-                                    clip_perc=[1, 99], 
+                                    clip_perc=(1, 99),
                                     color_palette_name=None, 
                                     cmap_method='pseudo_hist_norm',
-                                    output_tif=False,
-                                    generate_lookup_tables=False,
-                                    plot_rgba_raster=False,
-                                   ):
-    '''Function to take a single band geotiff file, apply a colormap to the data, and write a rgba geotiff to file
+                                    output_tif='single_band_rgba',
+                                    generate_QGIS_lut=True,
+                                    generate_rgba_luts=False,
+                                    generate_data_uint8_lut=False,
+                                    generate_uint8_luts=False,
+                                    plot_rgba_raster=False):
+    """Function to take a single band geotiff file, apply a colormap to the data, and write a rgba geotiff to file
 
 Input parameters:
  - single_band_tiff_path: 
      complete path to single-band-geotiff
 
  - data_min_max: 
-     default = None
+     Default: None
      Can take a list of lenth: 2, ex: [0, 500]
-     if not spcified, this function will automatically apply min/max values based on the clip_perc values
+     if not specified, this function will automatically calculate min/max values based on the min_max_method.
  
  - min_max_method:
-     default = 'percentile'; only relevant if data_min_max==None.
+     Default: 'percentile'; only relevant if data_min_max==None.
      Also accepts 'data_absolute'. 
-     'percentile' uses the percentiles used in clip_perc. 
-     'data_absolute' uses the minimum and maximum values of the data
+     'percentile' uses the percentiles supplied in clip_perc.
+     'data_absolute' uses the minimum and maximum values of the data supplied to the function
  
  - clip_perc
-     default = [1, 99]; only relevant if data_min_max==None.
+     Default: [1, 99]; only relevant if data_min_max==None.
      Percentile values to clip the data values to if no data_min_max is specified.
  
  - color_palette_name
-     default = None
+     Default: None
      Desired color pallet based on matplotlib colormaps. 
      https://matplotlib.org/stable/users/explain/colors/colormaps.html
-     If None, the funtion will automatically create a new "EMerald_Custom_Colormap"
+     If None, the function will automatically create a new "EMerald_Custom_Colormap"
  
- - cmap_method:
-     defualt = 'pseudo_hist_norm'
-     Method to determine where the color breaks should be. Also accepts 'pseudo_linear'
+ - cmap_method: Method to determine where the color breaks should be. Also accepts 'pseudo_linear'
+     Default: 'pseudo_hist_norm'
      'pseudo_hist_norm' will produce a linear colormap for data values below 0 and a histogram normalized colormap for the positive values
      'pseudo_linear' will produce a linear colormap for data values below 0 and a separate linear colormap for the positive values.
 
- - output_tif:
-     default = False
-     If new geotiff are desired as outputs this must be set to True
+ - output_tif: Write colorized geotiffs to file.
+     Default: 'single_band_rgba'
+     Options include:
+         'single_band_rgba', 'multi_band_rgba', None
 
  - generate_lookup_tables:
-     defaule = False
+     Default = False
      If set to True look up tables will be generated and written to file. This includes a look up table that can be applied to the single-band geotiff in QGIS and maybe other GIS software.
 
- - plot_rgba_raster
-     default=False
-     If set to True this will generate new matplotlib figures.
-    '''
+ - generate_QGIS_lut: Option to write a GIS software compatible colorization file to disk
+     Default: True
+
+ - generate_rgba_luts: Option to write data values to rgba look-up-tables to disk.
+     Default: False
+
+ - generate_data_uint8_lut: Option to write look-up-table to covert data to uint8 values.
+     Default: False
+
+ - generate_uint8_luts: Option to write uint8-data values to rgba look-up-tables to disk.
+     Default: False
+
+ - plot_rgba_raster: option to plot raster to screen. If set to True this will generate new matplotlib figures.
+     Default: False
+    """
 
     if data_min_max is not None:
-        assert len(data_min_max)==2, "len of data_min_max must be 2"
+        assert len(data_min_max) == 2, "len of data_min_max must be 2"
         assert data_min_max[0] < data_min_max[1], "first value must be less than second value"
         assert data_min_max[1] > 0, "This should really be a bigger number, but at least this will save dividing by a zero..."
-    assert len(clip_perc)==2, "len of data_min_max must be 2"
+    assert len(clip_perc) == 2, "len of data_min_max must be 2"
     assert clip_perc[0] < clip_perc[1], "first value must be less than second value"
         
     # 1. Read the Single-Band GeoTIFF:
     # Open the single-band GeoTIFF
     with rasterio.open(single_band_tiff_path, 'r') as src:
         data = src.read(1)  # Read the first band
         origprofile = src.profile
         extent = src.bounds
         size = (src.width, src.height)
         epsg_code = src.crs.to_epsg() if src.crs else None
         no_data_value = src.nodata  # Get the no-data value from the GeoTIFF
 
-    no_data_value = np.array(no_data_value, dtype=data[0,0].dtype).tolist()
+    no_data_value = np.array(no_data_value, dtype=data[0, 0].dtype).tolist()
     if data_min_max is None:
         data_min_max = calc_data_min_max(data, no_data_value, clip_perc, min_max_method=min_max_method)
 
-    # Clip data values to the specified range
-    clipped_data = np.clip(data, data_min_max[0], data_min_max[1])
-    
-    # Normalize the clipped data to the [0, 1] range
-    normalized_data = (clipped_data - data_min_max[0]) / (data_min_max[1] - data_min_max[0]) # shift to zero, divide by the range
-
-    # clip the data to the min-max values specified
-    clipped_data_with_dum = clipped_data.copy()
-    if no_data_value is not None:
-        clipped_data_with_dum[data==no_data_value]=no_data_value # since int is a valid datatype we can reuse the no-data-value (iff it's outside our min-max range)
-    
     # make percentile ranges
-    percentile_breaks, data_breaks = make_percentile_array(data_min_max, 
-                                                           clipped_data_with_dum, 
-                                                           no_data_value,
-                                                           cmap_method=cmap_method)
-    #print(f"percentile_breaks = {percentile_breaks}")
-    #print(f"data_breaks = {data_breaks}")
+    data_breaks = make_percentile_array(data_min_max=data_min_max,
+                                        data=data.copy(),
+                                        no_data_value=no_data_value,
+                                        color_list=EMerald_custom_colors_hexcolorcodes,
+                                        cmap_method=cmap_method,
+                                        plot_histograms=True)
 
     # 2. Generate a custom colormap (EMeraldCustomColormap):
     if color_palette_name is None:
         color_palette_name = "EMeraldCustomTerrain"
-        EMeraldCustomColormap = build_EMerald_terrain_colormap(percentile_breaks)
+        percentile_breaks = (data_breaks - data_min_max[0]) / (data_min_max[1] - data_min_max[0])
+        EMeraldCustomColormap = build_EMerald_terrain_colormap(percentile_breaks)  # only valid for data clipped to this range
     else:
         EMeraldCustomColormap = mpl.colormaps.get_cmap(color_palette_name)
-    EMeraldCustomColormap(0) #need this line for it to make a lut?!?
-    #print(EMeraldCustomColormap._lut)
+    EMeraldCustomColormap(0)  # need this line for it to make a lut?!?
+    # print(EMeraldCustomColormap._lut)
     
     # define output name
     sbpath, ext = os.path.splitext(single_band_tiff_path)
-    suffix=f"{color_palette_name}_{data_min_max[0]}_to_{data_min_max[1]}_{cmap_method}"
-    new_multiband_lut_path = f"{sbpath}_{suffix}"
-    new_multiband_tiff_path = f"{sbpath}_rgba_{suffix}"
+    suffix = f"{color_palette_name}_{data_min_max[0]}_to_{data_min_max[1]}_{cmap_method}"
+    lut_outpath_base = f"{sbpath}_{suffix}"
+
+    short_files = True
+    # short_files=False
     
+    if generate_QGIS_lut:
+        disco_tif.look_up_tables.rast_dat_to_QGIS_lut(cmap=EMerald_custom_colors_hexcolorcodes,
+                                                      data_breaks=data_breaks,
+                                                      dtype=data[0, 0].dtype,
+                                                      output_GIS_lut_path=lut_outpath_base,
+                                                      path_to_orig_geotiff=single_band_tiff_path,
+                                                      short_file=short_files)
+    if generate_rgba_luts:
+        disco_tif.look_up_tables.rast_dat_to_single_channel_rgba_luts(cmap=EMerald_custom_colors_hexcolorcodes,
+                                                                      data_breaks=data_breaks,
+                                                                      dtype=data[0, 0].dtype,
+                                                                      no_data_value=None,
+                                                                      lut_outpath_base=lut_outpath_base,
+                                                                      short_file=short_files)
+        disco_tif.look_up_tables.rast_dat_to_multi_channel_rgba_lut(cmap=EMerald_custom_colors_hexcolorcodes,
+                                                                    data_breaks=data_breaks,
+                                                                    dtype=data[0, 0].dtype,
+                                                                    no_data_value=None,
+                                                                    lut_outpath_base=lut_outpath_base,
+                                                                    short_file=short_files)
+        # disco_tif.look_up_tables.rast_dat_to_single_channel_rgba_luts(cmap=EMerald_custom_colors_hexcolorcodes,
+        #                                                               data_breaks=data_breaks,
+        #                                                               dtype=data[0, 0].dtype,
+        #                                                               no_data_value=no_data_value,
+        #                                                               lut_outpath_base=lut_outpath_base,
+        #                                                               short_file=short_files)
+        # disco_tif.look_up_tables.rast_dat_to_multi_channel_rgba_lut(cmap=EMerald_custom_colors_hexcolorcodes,
+        #                                                             data_breaks=data_breaks,
+        #                                                             dtype=data[0, 0].dtype,
+        #                                                             no_data_value=no_data_value,
+        #                                                             lut_outpath_base=lut_outpath_base,
+        #                                                             single_band_tiff_path=None,
+        #                                                             short_file=short_files)
+    if generate_data_uint8_lut:
+        disco_tif.look_up_tables.data_to_uint8_lut(data_breaks=data_breaks,
+                                                   no_data_value=no_data_value,
+                                                   lut_outpath_base=lut_outpath_base)
+        # disco_tif.look_up_tables.data_to_uint8_lut(data_breaks=data_breaks,
+        #                                            no_data_value=None,
+        #                                            lut_outpath_base=lut_outpath_base)
+    if generate_uint8_luts:
+        disco_tif.look_up_tables.uint8dat_to_single_channel_rgba_luts(cmap=EMerald_custom_colors_hexcolorcodes,
+                                                                      data_breaks=data_breaks,
+                                                                      dtype=data[0, 0].dtype,
+                                                                      no_data_value=no_data_value,
+                                                                      lut_outpath_base=lut_outpath_base,
+                                                                      short_file=short_files)
+        disco_tif.look_up_tables.uint8dat_to_multi_channel_rgba_lut(cmap=EMerald_custom_colors_hexcolorcodes,
+                                                                    data_breaks=data_breaks,
+                                                                    dtype=data[0, 0].dtype,
+                                                                    no_data_value=no_data_value,
+                                                                    lut_outpath_base=lut_outpath_base,
+                                                                    short_file=short_files)
+        # disco_tif.look_up_tables.uint8dat_to_single_channel_rgba_luts(cmap=EMerald_custom_colors_hexcolorcodes,
+        #                                                               data_breaks=data_breaks,
+        #                                                               dtype=data[0, 0].dtype,
+        #                                                               no_data_value=None,
+        #                                                               lut_outpath_base=lut_outpath_base,
+        #                                                               short_file=short_files)
+        # disco_tif.look_up_tables.uint8dat_to_multi_channel_rgba_lut(cmap=EMerald_custom_colors_hexcolorcodes,
+        #                                                             data_breaks=data_breaks,
+        #                                                             dtype=data[0, 0].dtype,
+        #                                                             no_data_value=None,
+        #                                                             lut_outpath_base=lut_outpath_base,
+        #                                                             single_band_tiff_path=None,
+        #                                                             short_file=short_files)
+
+    data_with_nan = data.copy().astype(float)
+    if no_data_value is not None:
+        data_with_nan[data == no_data_value] = np.nan
+    clip_data_with_nan = np.clip(data_with_nan, data_min_max[0], data_min_max[1],)
+
     if plot_rgba_raster:
-        # clip the data to the min-max values specified
-        clipped_data_with_nan = clipped_data.copy().astype(float)
-        if no_data_value is not None:
-            clipped_data_with_nan[data==no_data_value]=np.nan
-    
         figsize = [15, 9]
-        fig,ax=plt.subplots(1,1,figsize=figsize)
-        ep.plot_bands(clipped_data_with_nan,
-                      cmap = EMeraldCustomColormap,
+        fig, ax = plt.subplots(1, 1, figsize=figsize)
+        ep.plot_bands(clip_data_with_nan,
+                      # data_with_nan,
+                      cmap=EMeraldCustomColormap,
                       title=f"{sbpath.split(os.path.sep)[-1]}\n{suffix.replace('_', ' ')}",
-                      ax=ax,
-                     )
+                      ax=ax)
         plt.tight_layout()
-        plt.show()    
+        plt.show()
 
-    if generate_lookup_tables:
-        outfilepaths = build_1_component_color_tables(cmap=EMerald_custom_colors_hexcolorcodes,
-                                                      data_breaks=data_breaks,
-                                                      data=data,
-                                                      no_data_value=no_data_value,
-                                                      new_multiband_lut_path=new_multiband_lut_path )
-        for fp in outfilepaths:
-            print(f"Wrote 1component LUT files to: '{fp}'")
-    
-        outfilepaths = build_4_component_color_tables(single_band_tiff_path=single_band_tiff_path,
-                                                      cmap=EMeraldCustomColormap,
-                                                      data=data,
-                                                      no_data_value=no_data_value,
-                                                      percentile_breaks=percentile_breaks,
-                                                      data_breaks=data_breaks,
-                                                      outfile=new_multiband_tiff_path)
-        for fp in outfilepaths:
-            print(f"wrote 4component Lut files to: '{fp}''")
-    
-    if output_tif:
-        # apply EMeraldCustomColormap to data
-        rgba_data = EMeraldCustomColormap(normalized_data) * (colormap_length-1)  # Scale to 0-255 range
+    outfilepath = {}
+
+    if 'single_band_rgba' in output_tif:
+        tif_outpath_base = lut_outpath_base
+
+        uint8_rast_dat = rast_dat_to_uint8_data(rast_dat=data, data_min_max=data_min_max, no_data_value=no_data_value)
+
+        rgba_lut_dict = disco_tif.look_up_tables.rgba_lut_dict_builder(cmap=EMerald_custom_colors_hexcolorcodes,
+                                                                       data_breaks=data_breaks,
+                                                                       no_data_value=no_data_value,
+                                                                       dtype=data[0, 0].dtype)
+
+        new_uint8_rgba_lut_dict = disco_tif.look_up_tables.short_data_lut_to_long_uint8_lut(rgba_lut_dict, no_data_value=no_data_value)
+
+        newprofile = origprofile.copy()
+        if no_data_value is None:
+            newprofile.update(dtype='uint8', nodata=None)  # RGBA format
+        elif no_data_value is not None:
+            newprofile.update(dtype='uint8', nodata=0)  # RGBA format
         
-        # 3. Convert to RGB Channels:
-        rgb_data = rgba_data[:, :, :3]  # Extract RGB channels
+        with rasterio.open(f"{tif_outpath_base}.tif", 'w', **newprofile) as dst:
+            dst.write(uint8_rast_dat, indexes=1)
+            dst.write_colormap(1, new_uint8_rgba_lut_dict)
+
+        print(f"\nNew single-channel colorized geotiff written to: \n\t- '{tif_outpath_base}.tif'\n")
+
+        outfilepath['single-band-tiff'] = f"{tif_outpath_base}.tif"
+
+    if 'multi_band_rgba' in output_tif:
+        normalized_data_with_nan = (clip_data_with_nan - data_min_max[0]) / (data_min_max[1] - data_min_max[0])
+        rgba_data = EMeraldCustomColormap(normalized_data_with_nan) * (colormap_length-1)  # Scale to 0-255 range
         
-        # 4. Generate an Alpha Channel:
-        alpha_channel = (data != no_data_value).astype('uint8') * (colormap_length-1)
+        alpha_channel = (data != no_data_value).astype('uint8') * (colormap_length-1)  # 0 or 255
+
         rgba_data[:, :, 3] = alpha_channel
-        
-        # 5. Write the New RGBA GeoTIFF:
+
         newprofile = origprofile.copy()
         newprofile.update(count=4, dtype='uint8', nodata=None)  # RGBA format
-        
+
+        new_multiband_tiff_path = f"{sbpath}_rgba_{suffix}"
+
         with rasterio.open(f"{new_multiband_tiff_path}.tif", 'w', **newprofile) as dst:
-            dst.write(rgba_data[:, :, 0].astype('uint8'), 1) #red
-            dst.write(rgba_data[:, :, 1].astype('uint8'), 2) #green
-            dst.write(rgba_data[:, :, 2].astype('uint8'), 3) #blue
-            dst.write(rgba_data[:, :, 3].astype('uint8'), 4) #alpha
+            dst.write(rgba_data[:, :, 0].round().astype('uint8'), 1)  # red
+            dst.write(rgba_data[:, :, 1].round().astype('uint8'), 2)  # green
+            dst.write(rgba_data[:, :, 2].round().astype('uint8'), 3)  # blue
+            dst.write(rgba_data[:, :, 3].round().astype('uint8'), 4)  # alpha
     
-        print(f"New RGBA geotiff '{new_multiband_tiff_path}' generated successfully!")
-    return EMeraldCustomColormap, data_breaks, percentile_breaks
+        print(f"\nNew 4-channel colorized geotiff written to: \n\t- '{new_multiband_tiff_path}.tif'\n")
+        outfilepath['multi-band-tiff'] = f"{new_multiband_tiff_path}.tif"
 
-######################################
+    return EMeraldCustomColormap, data_breaks, outfilepath
```

### Comparing `disco-tif-0.0.2/disco_tif/write_mapfile.py` & `disco-tif-0.0.3/disco_tif/write_mapfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,62 +11,73 @@
     return datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
 def today():
     return datetime.datetime.now().strftime("%Y-%m-%d")
 def stoday():
     return datetime.datetime.now().strftime("%Y%m%d")
 
 def generate_LUT_based_mapfile(single_band_tiff_path, mapfile_path, writeLUTs=True, writeTifs=False, writeHillshades=True):
-    '''
-    funtion to take two geotiffs (single band and multiband) and generate a multi-layer mapsource mapfile
+    """Function to take two geotiffs (single band and multiband) and generate a multi-layer mapsource mapfile
     single_band_tiff_path: path to single band geotiff
     rgba_tiff_path: path to multiband geotiff
     mapfile_path: path of output mapfile
-    '''
+    - single_band_tiff_path:
+    
+    - mapfile_path:
+    
+    - writeLUTs:
+        Default: True:
+    
+    - writeTifs:
+        Default: False:
+    
+    - writeHillshades:
+        Default: True
+    """
 
-    #print(f"single_band_tiff_path = {single_band_tiff_path}")
+    # print(f"single_band_tiff_path = {single_band_tiff_path}")
     single_band_tiff_dir = os.path.dirname(single_band_tiff_path)
-    #print(f"single_band_tiff_dir  = {single_band_tiff_dir}")
+    # print(f"single_band_tiff_dir  = {single_band_tiff_dir}")
     single_band_file = (single_band_tiff_path.split(single_band_tiff_dir)[1]).split(os.path.sep)[1]
-    #print(f"single_band_file  = {single_band_file}")
+    # print(f"single_band_file  = {single_band_file}")
     
     lut_files_1b = []
     lut_files_4b = []
     for file in os.listdir(single_band_tiff_dir):
         if file.startswith(os.path.splitext(single_band_file)[0]):
             if file.endswith("_r.lut"):
                 lut_files_1b.append(file[:-6])
             elif np.logical_and('rgba' in file, file.endswith(".lut")):
                 lut_files_4b.append(file)
-    #print(f"lut_files = {lut_files}")
+    # print(f"lut_files = {lut_files}")
 
     hillshade_files = []
     tif_files = []
     for file in os.listdir(single_band_tiff_dir):
         if file.startswith(os.path.splitext(single_band_file)[0]):
-            #if file.endswith("hillshade.tif"):
+            # if file.endswith("hillshade.tif"):
             if np.logical_and('hillshade' in file, file.endswith(".tif")):
                 hillshade_files.append(file)
             elif file.endswith(".tif"):
                 tif_files.append(file)
-    tif_files = [tiff for tiff in tif_files if tiff!=single_band_file]
+    tif_files = [tiff for tiff in tif_files if tiff != single_band_file]
     hillshade_files = sorted(hillshade_files)
     tif_files = sorted(tif_files)
 
     # Open the single-band GeoTIFF
     with rasterio.open(single_band_tiff_path, 'r') as src:
         data = src.read(1)  # Read the first band
-        #origprofile = src.profile
+        # origprofile = src.profile
         extent = src.bounds
         size = (src.width, src.height)
         epsg_code = src.crs.to_epsg() if src.crs else None
         no_data_value = src.nodata  # Get the no-data value from the GeoTIFF
 
-    no_data_value = np.array(no_data_value, dtype=data[0,0].dtype).tolist()
-    data_min_max = np.min(data[data!=no_data_value]), np.max(data)
-    #print(data_min_max)
+    no_data_value = np.array(no_data_value, dtype=data[0, 0].dtype).tolist()
+    data_min_max = np.min(data[data != no_data_value]), np.max(data)
+    # print(data_min_max)
     
     # Define the paths to your GeoTIFF files
     name = single_band_file.split('.')[0]
 
     # Create a basic Mapfile template
     mapfile_template = f"""## Mapfile written on {today()} at {nowTime()}
 MAP
@@ -133,16 +144,16 @@
     END
 """
 
     if writeTifs:
         for tiff in tif_files:
             # Open the single-band GeoTIFF
             with rasterio.open(os.path.join(single_band_tiff_dir, tiff), 'r') as src:
-                #data = src.read(1)  # Read the first band
-                #origprofile = src.profile
+                # data = src.read(1)  # Read the first band
+                # origprofile = src.profile
                 extent = src.bounds
                 size = (src.width, src.height)
                 epsg_code = src.crs.to_epsg() if src.crs else None
             mapfile_template = f"""{mapfile_template}
     LAYER
         NAME "{tiff.split('.')[0]}"
         DATA "{tiff}"
@@ -155,16 +166,16 @@
     END
 """
 
     if writeHillshades:
         for hillshade in hillshade_files:
             # Open the single-band GeoTIFF
             with rasterio.open(os.path.join(single_band_tiff_dir, hillshade), 'r') as src:
-                #data = src.read(1)  # Read the first band
-                #origprofile = src.profile
+                # data = src.read(1)  # Read the first band
+                # origprofile = src.profile
                 extent = src.bounds
                 size = (src.width, src.height)
                 epsg_code = src.crs.to_epsg() if src.crs else None
             mapfile_template = f"""{mapfile_template}
     LAYER
         NAME "{hillshade.split('.')[0]}"
         DATA "{hillshade}"
@@ -190,20 +201,25 @@
         mapfile.write(mapfile_template)
 
     print(f"Mapfile '{mapfile_path}' generated successfully!")
 
 ######################################
 
 def generate_tiff_based_mapfile(single_band_tiff_path, rgba_tiff_path, mapfile_path):
-    '''
-    funtion to take two geotiffs (single band and multiband) and generate a multi-layer mapsource mapfile
+    """Function to take two geotiffs (single band and multiband) and generate a multi-layer MapSource mapfile
     single_band_tiff_path: path to single band geotiff
     rgba_tiff_path: path to multiband geotiff
     mapfile_path: path of output mapfile
-    '''
+
+    - single_band_tiff_path:
+    
+    - rgba_tiff_path:
+    
+    - mapfile_path
+    """
     # Open the single-band GeoTIFF
     with rasterio.open(single_band_tiff_path, 'r') as src:
         data = src.read(1)  # Read the first band
         origprofile = src.profile
         extent = src.bounds
         size = (src.width, src.height)
         epsg_code = src.crs.to_epsg() if src.crs else None
```

