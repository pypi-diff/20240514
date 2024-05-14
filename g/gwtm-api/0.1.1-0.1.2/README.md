# Comparing `tmp/gwtm_api-0.1.1.tar.gz` & `tmp/gwtm_api-0.1.2.tar.gz`

## Comparing `gwtm_api-0.1.1.tar` & `gwtm_api-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/__init__.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/alert.py
--rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/candidate.py
--rw-r--r--   0        0        0    11115 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/event_tools.py
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/instrument.py
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/pointing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/core/__init__.py
--rw-r--r--   0        0        0    11385 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/core/apimodels.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/core/baseapi.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/core/tmcache.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/src/gwtm_api/core/util.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/tests/candidate_test.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/tests/instrument_test.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/tests/pointing_tests.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/LICENSE
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/README.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 gwtm_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/__init__.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/alert.py
+-rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/candidate.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/event_tools.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/instrument.py
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/pointing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/core/__init__.py
+-rw-r--r--   0        0        0    11385 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/core/apimodels.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/core/baseapi.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/core/tmcache.py
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/src/gwtm_api/core/util.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/tests/candidate_test.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/tests/instrument_test.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/tests/pointing_tests.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/README.md
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 gwtm_api-0.1.2/PKG-INFO
```

### Comparing `gwtm_api-0.1.1/requirements.txt` & `gwtm_api-0.1.2/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -109,25 +109,28 @@
     #   h5py
     #   healpy
     #   lalsuite
     #   ligo-skymap
     #   lscsoft-glue
     #   matplotlib
     #   numcodecs
+    #   pandas
     #   ptemcee
     #   pyerfa
     #   python-ligo-lw
     #   reproject
     #   scipy
     #   zarr
 packaging==24.0
     # via
     #   astropy
     #   dask
     #   matplotlib
+pandas==2.2.2
+    # via gwtm_api (pyproject.toml)
 partd==1.4.2
     # via dask
 pillow==10.3.0
     # via
     #   ligo-skymap
     #   matplotlib
 ptemcee==1.0.0
@@ -142,21 +145,23 @@
     # via lscsoft-glue
 pyparsing==3.1.2
     # via matplotlib
 python-dateutil==2.9.0.post0
     # via
     #   lalsuite
     #   matplotlib
+    #   pandas
     #   python-ligo-lw
 python-ligo-lw==1.8.3
     # via ligo-skymap
 pytz==2024.1
     # via
     #   astroplan
     #   ligo-skymap
+    #   pandas
 pyyaml==6.0.1
     # via
     #   astropy
     #   dask
     #   python-ligo-lw
 reproject==0.13.1
     # via ligo-skymap
@@ -187,13 +192,15 @@
     # via
     #   dask
     #   partd
 tqdm==4.66.4
     # via
     #   ligo-skymap
     #   python-ligo-lw
+tzdata==2024.1
+    # via pandas
 urllib3==2.2.1
     # via requests
 zarr==2.18.0
     # via reproject
 zipp==3.18.1
     # via importlib-metadata
```

### Comparing `gwtm_api-0.1.1/.github/workflows/python-publish.yml` & `gwtm_api-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/src/gwtm_api/alert.py` & `gwtm_api-0.1.2/src/gwtm_api/alert.py`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/src/gwtm_api/candidate.py` & `gwtm_api-0.1.2/src/gwtm_api/candidate.py`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/src/gwtm_api/event_tools.py` & `gwtm_api-0.1.2/src/gwtm_api/event_tools.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import List
+from typing import Any, List, Tuple
 import ligo.skymap.plot  # noqa: F401
 from matplotlib import pyplot as plt
 from matplotlib.patches import Polygon
 import numpy as np
+import pandas as pd
 import astropy
 
 import healpy as hp
 from ligo.skymap.postprocess.util import find_greedy_credible_levels
 
-from .pointing import Pointing as Pointing
-from .instrument import Instrument as Instrument
-from .instrument import Footprint as Footprint
+from . import Pointing, Instrument, Footprint, Candidate
 from .alert import Alert as Alert
-from .core.util import instrument_color
+from .core.util import instrument_color, gc_dist
+
 
 def plot_coverage(api_token: str, graceid: str, pointings: List[Pointing] = [],
-    cache=False, projection='astro hours mollweide'):
+    cache=False, projection='astro hours mollweide') -> None:
     
     if len(pointings) == 0 and graceid is None:
         raise Exception("Pointings list or graceid is required")
 
     if len(pointings) == 0 and graceid is not None:
         pointings = Pointing.get(graceid = graceid, api_token=api_token, status='completed')
 
@@ -137,15 +137,15 @@
     plt.legend(bbox_to_anchor=(0, 0), loc="lower left",
                 bbox_transform=fig.transFigure,  ncol=4)
     plt.title(f"Reported Coverage for {graceid}")
     plt.show()
 
 
 def calculate_coverage(api_token: str, graceid: str, pointings: List[Pointing] = [],
-    cache=False, approximate=True):
+    cache=False, approximate=True) -> Tuple[float, float]:
     DECam_id = 38
     if len(pointings) == 0 and graceid is None:
         raise Exception("Pointings list or graceid is required")
 
     if len(pointings) == 0 and graceid is not None:
         pointings = Pointing.get(graceid = graceid, api_token=api_token, status='completed')
 
@@ -231,15 +231,15 @@
             #probs.append(prob)
             
     prob = np.sum(skymap[deduped_indices])
     area = pixarea * len(deduped_indices)
     return prob, area
 
 def renormalize_skymap(api_token: str, graceid: str, pointings: List[Pointing] = [],
-    cache=False):
+    cache=False) -> Any:
 
 
     if len(pointings) == 0 and graceid is None:
         raise Exception("Pointings list or graceid is required")
 
     if len(pointings) == 0 and graceid is not None:
         pointings = Pointing.get(graceid = graceid, api_token=api_token, status='completed')
@@ -302,8 +302,84 @@
             qps.extend(qp)
 
             deduped_indices=list(dict.fromkeys(qps))
 
     skymap[deduped_indices] = 0
     normed_skymap = skymap/np.sum(skymap)
 
-    return normed_skymap
+    return normed_skymap
+
+
+def candidate_coverage(api_token: str, candidate: Candidate, pointings: List[Pointing] = None, distance_thresh: float = 5.0) -> List[Pointing]:
+    '''
+    inputs:
+        api_token: str - valid GWTM api_token
+        candidate: Candidate - the candidate you want to evaluate the coverage for
+        pointings: List[Pointing] - you can query for your own pointings to evaluate the coverage. default = []
+        distance_threshold: float - distance in degrees. Only evaluate the pointings that are this distance from the candidate. default = 5.0 (deg)
+                
+    returns all pointings associated with the graceid that have had that candidate in its FOV
+    '''
+
+    #set an arbitarily high nside
+    skymap_nside = 1024
+    #find our candidates healpix
+    candidate_healpix = hp.ang2pix(skymap_nside, candidate.ra, candidate.dec, lonlat=True, nest=True)
+
+    #query for all pointings
+    if not pointings:
+        pointings = Pointing.get(api_token=api_token, graceid=candidate.graceid)
+
+    #convert them a pandas dataframe for vectorized distance culling
+    pointings_df = pd.DataFrame([x.__dict__ for x in pointings])
+
+    #calculate the distance for each pointing from the candidate, and cull them
+    pointings_df["_DIST"] = gc_dist(
+        pointings_df["ra"], pointings_df["dec"], candidate.ra, candidate.dec
+    )
+    culled_pointings = pointings_df.loc[pointings_df["_DIST"] < distance_thresh]
+
+    #return nothing if there aren't any pointings associated
+    if len(culled_pointings) == 0:
+        return []
+
+    #grab the instrument information for each pointing
+    instrument_ids = culled_pointings["instrumentid"].values.tolist()
+    instruments = Instrument.get(api_token=api_token, ids=instrument_ids, include_footprint=True)
+
+    vals = zip(
+        culled_pointings["ra"].values,
+        culled_pointings["dec"].values,
+        culled_pointings["pos_angle"].values,
+        culled_pointings["id"].values,
+        culled_pointings["instrumentid"].values
+    )
+
+    return_ids = []
+
+    #iterate over our pointing values
+    for pra, pdec, ppos_angle, pid, pinstid in vals:
+        #project the instrument footprint for each pointing
+        instrument = [x for x in instruments if x.id == pinstid][0]
+        projected = instrument.project(pra, pdec, ppos_angle)
+
+        #prepare the polygon for hp.query_polygon
+        polygon_arr = []
+        for ccd in projected:
+            ra_deg, dec_deg = zip(*[(coord_deg[0], coord_deg[1])
+                                    for coord_deg in ccd])
+            
+            list_o_coords = []
+            for x, y in zip(ra_deg, dec_deg):
+                list_o_coords.append((x, y))
+            polygon_arr.append(list_o_coords)
+        
+        #query the polygons and append the pointing.id if the healpix pixel is in the polygon query
+        for j,arr in enumerate(polygon_arr):
+            ras_poly = [x[0] for x in arr][:-1]
+            decs_poly = [x[1] for x in arr][:-1]
+            xyzpoly = astropy.coordinates.spherical_to_cartesian(1, np.deg2rad(decs_poly), np.deg2rad(ras_poly))
+            qp = hp.query_polygon(skymap_nside,np.array(xyzpoly).T, nest=True)
+            if candidate_healpix in qp:
+                return_ids.append(pid)
+    #so she goes
+    return [x for x in pointings if x.id in return_ids]
```

### Comparing `gwtm_api-0.1.1/src/gwtm_api/instrument.py` & `gwtm_api-0.1.2/src/gwtm_api/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import datetime
 import json
 import hashlib
 from typing import List
 import numpy as np
 
 from .pointing import Pointing
@@ -158,15 +159,15 @@
 
 
     @staticmethod
     def get(
             api_token: str, id: int = None, ids: List[int] = None, name: str = None,
             names: List[str] = None, type: apimodels.instrument_type = None,
             include_footprint=False, approximate_footprint=True, urlencode=False
-        ):
+        ) -> List[Instrument]:
         get_dict = util.non_none_locals(locals=locals())
 
         r_json = {
             "d_json":get_dict
         }
 
         api = baseapi.api(target="instruments")
```

### Comparing `gwtm_api-0.1.1/src/gwtm_api/pointing.py` & `gwtm_api-0.1.2/src/gwtm_api/pointing.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,14 +177,15 @@
             completed_after: datetime.datetime = None, completed_before: datetime.datetime = None,
             planned_after: datetime.datetime = None, planned_before: datetime.datetime = None,
             user: str = None, users: List[str] = None, band: apimodels.bandpass = None, 
             bands: List[apimodels.bandpass] = None, central_wave: float = None, bandwidth: float = None, 
             wavelength_regime: List[float] = None, wavelength_unit: apimodels.wavelength_units = None,
             energy_regime: List[float] = None, energy_unit: apimodels.energy_units = None,
             frequency_regime: List[float] = None, frequency_unit: apimodels.frequency_units = None,
+            depth_gt: float = None, depth_lt: float = None, depth_unit: apimodels.depth_unit = None,
             base: str = "https://treasuremap.space/api/", api_version: str ="v1", urlencode: bool = False, 
         ) -> List[Pointing]:
 
         get_dict = util.non_none_locals(locals=locals())
 
         r_json = {
             "d_json":get_dict
@@ -202,8 +203,32 @@
                 else:
                     pointing_json = p
                 ret.append(Pointing(kwdict=pointing_json))
             return ret
         else:
             raise Exception(f"Error in Pointing.get(). Request: {req.text[0:1000]}")
         
-        
+    
+    @staticmethod
+    def request_doi(
+            api_token: str, graceid: str = None, id: int = None, ids: List[int] = None, creators: dict = None, 
+            doi_group_id: int = None, base: str = "https://treasuremap.space/api/", api_version: str ="v1"
+    ) -> str:
+        if all([x is None for x in [graceid, id, ids]]):
+            raise Exception("Invalid parameters to request DOI. Must specify \'graceid\', pointing \'id\', or list of \'ids\'")
+        
+        get_dict = util.non_none_locals(locals=locals())
+
+        r_json = {
+            "d_json":get_dict
+        }
+
+        api = baseapi.api(target="request_doi", base=base, api_version=api_version)
+        req = api._post(r_json=r_json)
+
+        if req.status_code == 200:
+            request_json = json.loads(req.text)
+            return request_json["DOI URL"]
+        else:
+            raise Exception(f"Error in Pointing.get(). Request: {req.text[0:1000]}")
+
+        return ""
```

### Comparing `gwtm_api-0.1.1/src/gwtm_api/core/apimodels.py` & `gwtm_api-0.1.2/src/gwtm_api/core/apimodels.py`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/src/gwtm_api/core/baseapi.py` & `gwtm_api-0.1.2/src/gwtm_api/core/baseapi.py`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/src/gwtm_api/core/tmcache.py` & `gwtm_api-0.1.2/src/gwtm_api/core/tmcache.py`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/src/gwtm_api/core/util.py` & `gwtm_api-0.1.2/src/gwtm_api/core/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,18 +79,37 @@
     theta = np.deg2rad(theta_deg)
     return np.matrix([
         [np.cos(theta), -np.sin(theta), 0],
         [np.sin(theta), np.cos(theta), 0],
         [0, 0, 1]
     ])
 
+
 def instrument_color(integer):
     #GWTM friendly colors
     colorlist=[
         '#ffe119', '#4363d8', '#f58231', '#42d4f4', '#f032e6', 
         '#fabebe', '#469990', '#e6beff', '#9A6324', '#fffac8', 
         '#800000', '#aaffc3', '#000075', '#a9a9a9'
     ]
     try:
         return colorlist[integer]
     except:  # noqa: E722
         return COLORS[integer]
+
+
+def gc_dist(lon1, lat1, lon2, lat2) -> np.ndarray:
+    '''
+        function that calculates the distance between two points
+            p1 (lon1, lat1) or (ra1, dec1)
+            p2 (lon2, lat2) or (ra2, dec2)
+
+            can be np.array()
+            returns np.array()
+    '''
+    lon1 = np.radians(lon1)
+    lat1 = np.radians(lat1)
+    
+    lon2 = np.radians(lon2)
+    lat2 = np.radians(lat2)
+
+    return np.degrees(2*np.arcsin(np.sqrt( (np.sin((lat1-lat2)*0.5))**2 + np.cos(lat1)*np.cos(lat2)*(np.sin((lon1-lon2)*0.5))**2 )))
```

### Comparing `gwtm_api-0.1.1/tests/candidate_test.py` & `gwtm_api-0.1.2/tests/candidate_test.py`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/tests/instrument_test.py` & `gwtm_api-0.1.2/tests/instrument_test.py`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/tests/pointing_tests.py` & `gwtm_api-0.1.2/tests/pointing_tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,32 +19,34 @@
     #   statuses xx
     #   bands xx
     #   wavelength_regimes xx
     #   frequency_regimes 
     #   energy_regimes
 
     #testing graceids
-    pointings = gwtm_api.Pointing.get(graceids=["GW190814", "S190425z"], api_token=API_TOKEN)
+    # pointings = gwtm_api.Pointing.get(graceids=["GW190814", "S190425z"], api_token=API_TOKEN)
     
-    users_t = [6,7]
-    pointings = gwtm_api.Pointing.get(users=users_t, api_token=API_TOKEN)
+    # users_t = [6,7]
+    # pointings = gwtm_api.Pointing.get(users=users_t, api_token=API_TOKEN)
 
     # statuses = ['completed']
     # pointings = gwtm_api.Pointing.get(status=statuses, graceid="GW190814", api_token=API_TOKEN)
 
     # bands = ['XRT', 'u', 'V']
     # pointings = gwtm_api.Pointing.get(bands=bands, graceid="GW190814", api_token=API_TOKEN)
 
     # ids = [3811, 3812, 3813, 3814, 3815, 3816, 3817, 3818, 3819, 3820, 3821, 3822, 3823, 3824, 3825, 3826, 3827, 3828, 3829, 3830]
     # pointings = gwtm_api.Pointing.get(ids=ids, graceid="GW190814", api_token=API_TOKEN)
     # pointings = gwtm_api.Pointing.get(id=ids[0], graceid="GW190814", api_token=API_TOKEN)
 
     # pointings = gwtm_api.Pointing.get(wavelength_regime=["0", 45], wavelength_unit='nanometer', graceid='GW190814', api_token=API_TOKEN)
     # pointings = gwtm_api.Pointing.get(energy_regime="[0,5200]", energy_unit='keV', graceid='GW190814', api_token=API_TOKEN)
     # pointings = gwtm_api.Pointing.get(frequency_regime=[0, 500], frequency_unit='THz', graceid='GW190814', api_token=API_TOKEN, urlencode=True)
+
+    pointings = gwtm_api.Pointing.get(depth_lt=15, graceid="MS181101ab", api_token=API_TOKEN, base="http://127.0.0.1:5000/api/")
     print(len(pointings))
 
     for p in pointings[0:2]:
         p.dump()
     #testing users
     return 
 
@@ -91,10 +93,15 @@
         )
     ]
 
     batch = gwtm_api.Pointing.batch_post(pointings=batch, graceid='MS181101ab', api_token=API_TOKEN)
     for b in batch:
         b.dump()
 
-get_pointing_test()
-post_pointing_test()
-batch_pointing_post()
+def request_doi_test():
+    doi_url = gwtm_api.Pointing.request_doi(api_token=API_TOKEN, graceid='MS181101ab')
+    print(doi_url)
+
+#get_pointing_test()
+#post_pointing_test()
+#batch_pointing_post()
+request_doi_test()
```

### Comparing `gwtm_api-0.1.1/LICENSE` & `gwtm_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwtm_api-0.1.1/README.md` & `gwtm_api-0.1.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -77,14 +77,46 @@
 batch = [
   gwtm_api.Candidate(...),
   gwtm_api.Candidate(...)
 ]
 gwtm_api.Pointing.batch_post(candidates=batch, graceid="GRACEID", api_token=API_TOKEN)
 ```
 
+### PUT
+Update a GWTM candidate record
+```python
+import gwtm_api
+candidate = gwtm_api.Candidate.get(api_token=API_TOKEN, id=CANDIDATE_ID)
+my_candidate = candidate[0]
+update_payload = {
+    "tns_name": "AT2017gfo",
+    "tns_url": "https://www.wis-tns.org/object/2017gfo"
+    "associated_galaxy": "NGC 4993"
+    "associated_galaxy_redshift": 0.009727
+}
+my_candidate.put(api_token=API_TOKEN, payload=update_payload)
+
+#or similarly
+candidate = gwtm_api.Candidate(id=CANDIDATE_ID, api_token=API_TOKEN) #this will envoke the GET endpoint if it has an id and api token
+candidate.tns_name = "AT2017gfo"
+candidate.tns_url = "https://www.wis-tns.org/object/2017gfo"
+candidate.associated_galaxy = "NGC 4993"
+candidate.associated_galaxy_redshift = 0.009727
+candidate.put(api_token=API_TOKEN)
+```
+
+### Delete
+```python
+candidate = gwtm_api.Candidate(id=21, api_token=API_TOKEN)
+candidate.delete(api_token=API_TOKEN)
+
+#or batch delete with a list of ids
+gwtm_api.Candidate.batch_delete(api_token=API_TOKEN, ids=[id1, id2....], verbose=True)
+```
+
 ## Instruments
 Query for instrument information that have been submitted to the Treasure Map
 ```python
 import gwtm_api
 
 instruments = gwtm_api.Instrument.get(name="ZTF", api_token=API_TOKEN)
 ```
@@ -139,7 +171,18 @@
 renormalized_skymap = gwtm_api.event_tools.renormalize_skymap(
     graceid="GW190814",
     api_token=API_TOKEN,
     pointings=pointings,
     cache=True
 )
 ```
+
+### Candidate Coerage
+For a given `candidate`, find which instruments have `pointing` footprints that overlap with the candidate's position. The user can potentially constrain which instruments have observed a candidate pre/post post discovery. User's can pass in a list of `pointings`, or it will default to all `pointings` for the `candidate's` associated graceid. The function also accepts a `distance_thresh` (in degrees) to limit the calculation to only the pointings centered within the threshold distance from the candidate. 
+
+```python
+my_candidate = gwtm_api.Candidate.get(...)
+pointings_list = gwtm_api.event_tools.candidate_coverage(
+    api_token=API_TOKEN,
+    candidate=my_candidate
+)
+```
```

### Comparing `gwtm_api-0.1.1/pyproject.toml` & `gwtm_api-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gwtm_api"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Samuel Wyatt", email="samuel.d.wyatt@nasa.gov" },
 ]
 description = "A python API wrapper for the Gravitational Wave Treasure Map"
 readme = "README.md"
 requires-python = ">=3.10"
 
 dependencies = [
   "astropy",
   "healpy",
   "requests",
   "ligo.skymap",
-  "matplotlib"
+  "matplotlib",
+  "pandas"
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `gwtm_api-0.1.1/PKG-INFO` & `gwtm_api-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: gwtm_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python API wrapper for the Gravitational Wave Treasure Map
 Project-URL: Homepage, https://github.com/TheTreasureMap/gwtm_api
 Project-URL: Bug Tracker, https://github.com/TheTreasureMap/gwtm_api/issues
 Author-email: Samuel Wyatt <samuel.d.wyatt@nasa.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: astropy
 Requires-Dist: healpy
 Requires-Dist: ligo-skymap
 Requires-Dist: matplotlib
+Requires-Dist: pandas
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # gwtm_api
 
 A python wrapper for the [Gravitational Wave Treasure Map](http://treasuremap.space).
 In order to interact with the web API, you will need to [register](http://treasuremap.space/register) an account with the GWTM. Once verified you will recieve an `API_TOKEN` to pass into all api endpoints.
@@ -96,14 +97,46 @@
 batch = [
   gwtm_api.Candidate(...),
   gwtm_api.Candidate(...)
 ]
 gwtm_api.Pointing.batch_post(candidates=batch, graceid="GRACEID", api_token=API_TOKEN)
 ```
 
+### PUT
+Update a GWTM candidate record
+```python
+import gwtm_api
+candidate = gwtm_api.Candidate.get(api_token=API_TOKEN, id=CANDIDATE_ID)
+my_candidate = candidate[0]
+update_payload = {
+    "tns_name": "AT2017gfo",
+    "tns_url": "https://www.wis-tns.org/object/2017gfo"
+    "associated_galaxy": "NGC 4993"
+    "associated_galaxy_redshift": 0.009727
+}
+my_candidate.put(api_token=API_TOKEN, payload=update_payload)
+
+#or similarly
+candidate = gwtm_api.Candidate(id=CANDIDATE_ID, api_token=API_TOKEN) #this will envoke the GET endpoint if it has an id and api token
+candidate.tns_name = "AT2017gfo"
+candidate.tns_url = "https://www.wis-tns.org/object/2017gfo"
+candidate.associated_galaxy = "NGC 4993"
+candidate.associated_galaxy_redshift = 0.009727
+candidate.put(api_token=API_TOKEN)
+```
+
+### Delete
+```python
+candidate = gwtm_api.Candidate(id=21, api_token=API_TOKEN)
+candidate.delete(api_token=API_TOKEN)
+
+#or batch delete with a list of ids
+gwtm_api.Candidate.batch_delete(api_token=API_TOKEN, ids=[id1, id2....], verbose=True)
+```
+
 ## Instruments
 Query for instrument information that have been submitted to the Treasure Map
 ```python
 import gwtm_api
 
 instruments = gwtm_api.Instrument.get(name="ZTF", api_token=API_TOKEN)
 ```
@@ -158,7 +191,18 @@
 renormalized_skymap = gwtm_api.event_tools.renormalize_skymap(
     graceid="GW190814",
     api_token=API_TOKEN,
     pointings=pointings,
     cache=True
 )
 ```
+
+### Candidate Coerage
+For a given `candidate`, find which instruments have `pointing` footprints that overlap with the candidate's position. The user can potentially constrain which instruments have observed a candidate pre/post post discovery. User's can pass in a list of `pointings`, or it will default to all `pointings` for the `candidate's` associated graceid. The function also accepts a `distance_thresh` (in degrees) to limit the calculation to only the pointings centered within the threshold distance from the candidate. 
+
+```python
+my_candidate = gwtm_api.Candidate.get(...)
+pointings_list = gwtm_api.event_tools.candidate_coverage(
+    api_token=API_TOKEN,
+    candidate=my_candidate
+)
+```
```

