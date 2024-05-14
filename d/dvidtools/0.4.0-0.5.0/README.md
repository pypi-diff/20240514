# Comparing `tmp/dvidtools-0.4.0.tar.gz` & `tmp/dvidtools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvidtools-0.4.0.tar", last modified: Fri Sep  2 08:43:21 2022, max compression
+gzip compressed data, was "dvidtools-0.5.0.tar", last modified: Tue May 14 08:36:15 2024, max compression
```

## Comparing `dvidtools-0.4.0.tar` & `dvidtools-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,25 @@
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2022-09-02 08:43:21.720350 dvidtools-0.4.0/
--rw-r--r--   0 philipps   (501) staff       (20)     1236 2019-03-07 05:11:38.000000 dvidtools-0.4.0/.gitignore
--rw-r--r--   0 philipps   (501) staff       (20)    35149 2018-12-02 19:03:16.000000 dvidtools-0.4.0/LICENSE
--rw-r--r--   0 philipps   (501) staff       (20)       25 2019-04-04 21:05:28.000000 dvidtools-0.4.0/MANIFEST.in
--rw-r--r--   0 philipps   (501) staff       (20)     3141 2022-09-02 08:43:21.719511 dvidtools-0.4.0/PKG-INFO
--rw-r--r--   0 philipps   (501) staff       (20)     2099 2022-09-02 08:42:31.000000 dvidtools-0.4.0/README.md
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2022-09-02 08:43:21.629941 dvidtools-0.4.0/docs/
--rw-r--r--   0 philipps   (501) staff       (20)      580 2019-03-07 03:44:51.000000 dvidtools-0.4.0/docs/Makefile
--rw-r--r--   0 philipps   (501) staff       (20)     5744 2021-03-04 13:48:35.000000 dvidtools-0.4.0/docs/conf.py
--rw-r--r--   0 philipps   (501) staff       (20)     4000 2022-08-08 09:37:52.000000 dvidtools-0.4.0/docs/index.rst
--rw-r--r--   0 philipps   (501) staff       (20)      140 2022-08-08 09:19:59.000000 dvidtools-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2022-09-02 08:43:21.631552 dvidtools-0.4.0/docs/src/
--rw-r--r--   0 philipps   (501) staff       (20)     1088 2022-08-08 09:17:06.000000 dvidtools-0.4.0/docs/src/api.rst
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2022-09-02 08:43:21.642611 dvidtools-0.4.0/dvid/
--rw-r--r--   0 philipps   (501) staff       (20)      221 2021-08-11 10:02:33.000000 dvidtools-0.4.0/dvid/__init__.py
--rw-r--r--   0 philipps   (501) staff       (20)      239 2021-08-11 10:04:12.000000 dvidtools-0.4.0/dvid/config.py
--rw-r--r--   0 philipps   (501) staff       (20)     3281 2022-03-01 09:48:13.000000 dvidtools-0.4.0/dvid/decode.py
--rw-r--r--   0 philipps   (501) staff       (20)    81605 2022-08-07 23:15:57.000000 dvidtools-0.4.0/dvid/fetch.py
--rw-r--r--   0 philipps   (501) staff       (20)    18212 2022-08-07 17:22:54.000000 dvidtools-0.4.0/dvid/meshing.py
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2022-09-02 08:43:21.704842 dvidtools-0.4.0/dvid/model/
--rw-r--r--   0 philipps   (501) staff       (20) 33116974 2019-04-04 21:32:08.000000 dvidtools-0.4.0/dvid/model/model.pkl
--rw-r--r--   0 philipps   (501) staff       (20)      998 2019-04-04 21:32:08.000000 dvidtools-0.4.0/dvid/model/scaler.pkl
--rw-------   0 philipps   (501) staff       (20)    15701 2021-03-05 12:34:43.000000 dvidtools-0.4.0/dvid/tip.py
--rw-r--r--   0 philipps   (501) staff       (20)    16014 2021-08-19 09:17:25.000000 dvidtools-0.4.0/dvid/utils.py
-drwxr-xr-x   0 philipps   (501) staff       (20)        0 2022-09-02 08:43:21.718222 dvidtools-0.4.0/dvidtools.egg-info/
--rw-------   0 philipps   (501) staff       (20)     3141 2022-09-02 08:43:21.000000 dvidtools-0.4.0/dvidtools.egg-info/PKG-INFO
--rw-------   0 philipps   (501) staff       (20)      504 2022-09-02 08:43:21.000000 dvidtools-0.4.0/dvidtools.egg-info/SOURCES.txt
--rw-r--r--   0 philipps   (501) staff       (20)        1 2022-09-02 08:43:21.000000 dvidtools-0.4.0/dvidtools.egg-info/dependency_links.txt
--rw-r--r--   0 philipps   (501) staff       (20)        1 2018-12-13 14:18:56.000000 dvidtools-0.4.0/dvidtools.egg-info/not-zip-safe
--rw-------   0 philipps   (501) staff       (20)      145 2022-09-02 08:43:21.000000 dvidtools-0.4.0/dvidtools.egg-info/requires.txt
--rw-r--r--   0 philipps   (501) staff       (20)        5 2022-09-02 08:43:21.000000 dvidtools-0.4.0/dvidtools.egg-info/top_level.txt
--rw-r--r--   0 philipps   (501) staff       (20)       81 2022-09-02 08:36:24.000000 dvidtools-0.4.0/pyproject.toml
--rw-------   0 philipps   (501) staff       (20)      114 2021-03-09 17:05:17.000000 dvidtools-0.4.0/requirements.txt
--rw-r--r--   0 philipps   (501) staff       (20)       38 2022-09-02 08:43:21.720487 dvidtools-0.4.0/setup.cfg
--rw-------   0 philipps   (501) staff       (20)     1892 2022-09-02 08:34:48.000000 dvidtools-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:36:15.228433 dvidtools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-14 08:36:12.000000 dvidtools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 08:36:12.000000 dvidtools-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-14 08:36:15.228433 dvidtools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-14 08:36:12.000000 dvidtools-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:36:15.228433 dvidtools-0.5.0/dvid/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-14 08:36:12.000000 dvidtools-0.5.0/dvid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-14 08:36:12.000000 dvidtools-0.5.0/dvid/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-14 08:36:12.000000 dvidtools-0.5.0/dvid/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91354 2024-05-14 08:36:12.000000 dvidtools-0.5.0/dvid/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18212 2024-05-14 08:36:12.000000 dvidtools-0.5.0/dvid/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15701 2024-05-14 08:36:12.000000 dvidtools-0.5.0/dvid/tip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15990 2024-05-14 08:36:12.000000 dvidtools-0.5.0/dvid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:36:15.228433 dvidtools-0.5.0/dvidtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-14 08:36:15.000000 dvidtools-0.5.0/dvidtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-14 08:36:15.000000 dvidtools-0.5.0/dvidtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:36:15.000000 dvidtools-0.5.0/dvidtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:36:15.000000 dvidtools-0.5.0/dvidtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-14 08:36:15.000000 dvidtools-0.5.0/dvidtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 08:36:15.000000 dvidtools-0.5.0/dvidtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-14 08:36:12.000000 dvidtools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:36:15.228433 dvidtools-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-14 08:36:12.000000 dvidtools-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:36:15.228433 dvidtools-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-14 08:36:12.000000 dvidtools-0.5.0/tests/test_fetching.py
```

### Comparing `dvidtools-0.4.0/LICENSE` & `dvidtools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvidtools-0.4.0/PKG-INFO` & `dvidtools-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: dvidtools
-Version: 0.4.0
-Summary: Fetch data from DVID server
-Home-page: https://github.com/flyconnectome/dvid_tools
-Author: Philipp Schlegel
-Author-email: pms70@cam.ac.uk
-License: GNU GPL V3
-Project-URL: Documentation, https://dvidtools.readthedocs.io
-Project-URL: Source, https://github.com/flyconnectome/dvid_tools
-Keywords: DVID API fetch neuron segmentation
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: extras
-License-File: LICENSE
-
 [![Documentation Status](https://readthedocs.org/projects/dvidtools/badge/?version=latest)](http://dvidtools.readthedocs.io/en/latest/?badge=latest)[![Tests](https://github.com/flyconnectome/dvid_tools/actions/workflows/test-package.yml/badge.svg)](https://github.com/flyconnectome/dvid_tools/actions/workflows/test-package.yml)
 
 # dvidtools
 Python tools to fetch data from [DVID](https://github.com/janelia-flyem/dvid) servers.
 
 Find the documentation [here](https://dvidtools.readthedocs.io).
 
@@ -35,25 +9,25 @@
 [neuprint-python](https://github.com/connectome-neuprint/neuprint-python).
 
 ## What can `dvidtools` do for you?
 
 - get/set user bookmarks
 - get/set neuron annotations (names)
 - download precomputed meshes, skeletons (SWCs) and ROIs
+- generate meshes or skeletons from scratch
 - get basic neuron info (# of voxels/synapses)
-- get synapses
-- get connectivity (adjacency matrix, connectivity table)
+- fetch synapses
+- fetch connectivity (adjacency matrix, connectivity table)
 - retrieve labels (TODO, to split, etc)
 - map positions to body IDs
-- mesh or skeletonize sparsevols
 - detect potential open ends (based on a script by [Stephen Plaza](https://github.com/stephenplaza))
 
 ## Install
 
-Make sure you have [Python 3](https://www.python.org) (3.6 or later),
+Make sure you have [Python 3](https://www.python.org) (3.8 or later),
 [pip](https://pip.pypa.io/en/stable/installing/). Then run this:
 
 ```bash
 pip3 install dvidtools
 ```
 
 To install the dev version straight from Github:
```

### Comparing `dvidtools-0.4.0/dvid/decode.py` & `dvidtools-0.5.0/dvid/decode.py`

 * *Files identical despite different names*

### Comparing `dvidtools-0.4.0/dvid/fetch.py` & `dvidtools-0.5.0/dvid/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,17 +37,19 @@
 
 __all__ = ['add_bookmarks', 'edit_annotation', 'get_adjacency', 'get_annotation',
            'get_assignment_status', 'get_available_rois',
            'get_body_position', 'get_connections',
            'get_connectivity', 'get_labels_in_area', 'get_last_mod',
            'locs_to_ids', 'get_n_synapses', 'get_roi', 'get_sparsevol',
            'get_segmentation_info', 'get_skeletons', 'get_skeleton_mutation',
+           'has_skeleton', 'has_mesh',
            'get_synapses', 'get_user_bookmarks', 'setup', 'snap_to_body',
            'get_meshes', 'list_projects', 'get_master_node', 'get_sparsevol_size',
-           'get_sizes', 'ids_exist', 'skeletonize_neuron', 'mesh_neuron']
+           'get_sizes', 'ids_exist', 'skeletonize_neuron', 'mesh_neuron',
+           'find_lost_ids', 'update_ids', "get_branch_history"]
 
 
 def dvid_session(appname=DEFAULT_APPNAME, user=None):
     """Return a default requests.Session() object.
 
     Automatically appends the 'u' and 'app' query string parameters to every
     request. The Session object is cached, so this function will return the same
@@ -170,35 +172,42 @@
     elif isinstance(x, str):
         x = [int(x)]
 
     # At this point we expect a list, set or array
     if not isinstance(x, (list, set, np.ndarray)):
         raise TypeError(f'Unexpected data type for body ID(s): "{type(x)}"')
 
-    out = []
-    with ThreadPoolExecutor(max_workers=max_threads) as executor:
-        futures = {}
-        for bid in x:
-            f = executor.submit(__get_ngmesh,
-                                bid,
-                                output=output,
-                                on_error=on_error,
-                                server=server, node=node)
-            futures[f] = bid
+    if len(x) > 1:
+        out = []
+        with ThreadPoolExecutor(max_workers=max_threads) as executor:
+            futures = {}
+            for bid in x:
+                f = executor.submit(__get_ngmesh,
+                                    bid,
+                                    output=output,
+                                    on_error=on_error,
+                                    server=server, node=node)
+                futures[f] = bid
+
+            with tqdm(desc='Fetching',
+                    total=len(x),
+                    leave=False,
+                    disable=not progress) as pbar:
+                for f in as_completed(futures):
+                    res = f.result()
+                    # Skip neurons that caused an error
+                    if res is not None:
+                        out.append(res)
+                    pbar.update(1)
+    else:
+        out = [__get_ngmesh(x[0], output=output, on_error=on_error,
+                           server=server, node=node)]
 
-        with tqdm(desc='Fetching',
-                  total=len(x),
-                  leave=False,
-                  disable=not progress) as pbar:
-            for f in as_completed(futures):
-                res = f.result()
-                # Skip neurons that caused an error
-                if res is not None:
-                    out.append(res)
-                pbar.update(1)
+    # Drop `None`
+    out = [o for o in out if o is not None]
 
     if (output == 'auto' and navis) or (output == 'navis'):
         out = navis.NeuronList(out)
 
     return out
 
 
@@ -243,14 +252,75 @@
     if (output == 'auto' and navis) or (output == 'navis'):
         n = navis.MeshNeuron(m, id=bodyid, mutation_id=m.mutation_id)
         return n
 
     return m
 
 
+def has_mesh(x, max_threads=10, progress=True, server=None, node=None):
+    """Check if given body has a mesh.
+
+    Parameters
+    ----------
+    x :         int | str | list thereof
+                ID(s) of body to check.
+    server :    str, optional
+                If not provided, will try reading from global.
+    node :      str, optional
+                If not provided, will try reading from global.
+
+    Returns
+    -------
+    has_mesh :  np.array
+                Contains True if body has a mesh, False otherwise. Note
+                that False can also mean that the ID just doesn't exist. Use
+                ``dvidtools.ids_exist`` to check for that.
+
+    """
+    server, node, user = eval_param(server, node)
+
+    if isinstance(x, pd.DataFrame):
+        if "bodyId" in x.columns:
+            x = x["bodyId"].values
+        elif "bodyid" in x.columns:
+            x = x["bodyid"].values
+        else:
+            raise ValueError('DataFrame must have "bodyId" column.')
+    elif isinstance(x, int):
+        x = [x]
+    elif isinstance(x, str):
+        x = [int(x)]
+
+    base_url = urllib.parse.urljoin(server,
+                                    'api/node/{}/{}_meshes/key'.format(node,
+                                                                           config.segmentation))
+
+    results = {}
+    with ThreadPoolExecutor(max_workers=max_threads) as executor:
+        futures = {}
+        for bid in x:
+            f = executor.submit(_has_mesh, url=f"{base_url}/{bid}.ngmesh")
+            futures[f] = bid
+
+        with tqdm(
+            desc="Checking", total=len(x), leave=False, disable=not progress
+        ) as pbar:
+            for f in as_completed(futures):
+                pbar.update(1)
+                results[futures[f]] = f.result() == 200
+
+    return np.array([results[bid] for bid in x])
+
+
+def _has_mesh(url):
+    # No need to raise for status here
+    r = dvid_session().head(url)
+    return r.status_code
+
+
 def get_skeletons(x, save_to=None, output='auto', on_error='warn',
                   check_mutation=False, max_threads=5, progress=True,
                   server=None, node=None):
     """Fetch skeleton for given body ID.
 
     Parameters
     ----------
@@ -310,14 +380,16 @@
     Grab a neuron and save it directly to a file
 
     >>> dt.get_skeleton(485775679, save_to='~/Downloads/', output=None)
 
     """
     if output == 'navis' and not navis:
         raise ImportError('Please install `navis`: pip3 install navis')
+    elif output == 'auto' and navis:
+        output = 'navis'
 
     if on_error not in ("warn", "skip", "raise"):
         raise ValueError('`on_error` must be either "warn", "skip" or "raise"')
 
     if max_threads < 1:
         raise ValueError('`max_threads` must be >= 1')
 
@@ -358,19 +430,26 @@
         with tqdm(desc='Fetching',
                   total=len(x),
                   leave=False,
                   disable=not progress) as pbar:
             for f in as_completed(futures):
                 res = f.result()
                 pbar.update(1)
-                if on_error == "skip" and res is None:
-                    continue
+                # If this neuron didn't produce a result
+                if res is None:
+                    # Skip entirely
+                    if on_error == "skip":
+                        continue
+                    # if just warn and output is supposed to be navis
+                    # return an empty neuron
+                    elif output == 'navis':
+                        res = navis.TreeNeuron(None, id=futures[f])
                 out.append(res)
 
-    if (output == 'auto' and navis) or (output == 'navis'):
+    if output == 'navis':
         out = navis.NeuronList(out)
 
     return out
 
 
 def __get_skeleton(bodyid, save_to=None, output='auto', on_error='raise',
                    check_mutation=False, server=None, node=None):
@@ -436,14 +515,75 @@
         n.header = header
         n.mutation_id = getattr(swc, 'mutation_id', None)
         return n
 
     return swc
 
 
+def has_skeleton(x, max_threads=10, progress=True, server=None, node=None):
+    """Check if given body has a skeleton.
+
+    Parameters
+    ----------
+    x :         int | str | list thereof
+                ID(s) of body to check.
+    server :    str, optional
+                If not provided, will try reading from global.
+    node :      str, optional
+                If not provided, will try reading from global.
+
+    Returns
+    -------
+    has_skeleton :  np.array
+                Contains True if body has a skeleton, False otherwise. Note
+                that False can also mean that the ID just doesn't exist. Use
+                ``dvidtools.ids_exist`` to check for that.
+
+    """
+    server, node, user = eval_param(server, node)
+
+    if isinstance(x, pd.DataFrame):
+        if "bodyId" in x.columns:
+            x = x["bodyId"].values
+        elif "bodyid" in x.columns:
+            x = x["bodyid"].values
+        else:
+            raise ValueError('DataFrame must have "bodyId" column.')
+    elif isinstance(x, int):
+        x = [x]
+    elif isinstance(x, str):
+        x = [int(x)]
+
+    base_url = urllib.parse.urljoin(server,
+                                    'api/node/{}/{}_skeletons/key'.format(node,
+                                                                           config.segmentation))
+
+    results = {}
+    with ThreadPoolExecutor(max_workers=max_threads) as executor:
+        futures = {}
+        for bid in x:
+            f = executor.submit(_has_skeleton, url=f"{base_url}/{bid}_swc")
+            futures[f] = bid
+
+        with tqdm(
+            desc="Fetching", total=len(x), leave=False, disable=not progress
+        ) as pbar:
+            for f in as_completed(futures):
+                pbar.update(1)
+                results[futures[f]] = f.result() == 200
+
+    return np.array([results[bid] for bid in x])
+
+
+def _has_skeleton(url):
+    # No need to raise for status here
+    r = dvid_session().head(url)
+    return r.status_code
+
+
 def __old_get_skeleton(bodyid, save_to=None, xform=None, root=None, soma=None,
                        heal=False, check_mutation=True, server=None, node=None,
                        verbose=True, **kwargs):
     """Download skeleton as SWC file.
 
     Parameters
     ----------
@@ -757,15 +897,14 @@
     """
     server, node, user = eval_param(server, node)
 
     r = dvid_session().get(urllib.parse.urljoin(server,
                                                 'api/node/{}/{}_annotations/key/{}'.format(node,
                                                                                            config.body_labels,
                                                                                            bodyid)))
-
     try:
         return r.json()
     except BaseException:
         if verbose:
             print(r.text)
         return {}
 
@@ -1573,14 +1712,15 @@
     return voxels
 
 
 def mesh_neuron(bodyid,
                 scale='COARSE',
                 step_size=1,
                 bbox=None,
+                on_error='raise',
                 parallel=False,
                 progress=True,
                 server=None,
                 node=None,
                 **kwargs):
     """Create mesh for given neuron(s).
 
@@ -1595,14 +1735,19 @@
     step_size : int, optional
                 Step size for marching cube algorithm.
                 Higher values = faster but coarser.
     bbox :      list | None, optional
                 Bounding box to which to restrict the meshing to. Must be in
                 `scale=0` coordinates.
                 Format: ``[x_min, x_max, y_min, y_max, z_min, z_max]``.
+    on_error :  "raise" | "warn" | "ignore"
+                What to do if an error occurs. If "raise", will raise the
+                exception. If "warn", will print a warning and continue.
+                If "ignore", will ignore the error and continue. Note that
+                for "warn" and "ignore" the function may return `None`.
     parallel :  bool | int
                 Whether to run meshing in parallel on multiple cores if
                 `bodyid` is more than one neuron. If `parallel` is integer will
                 use that many cores. Otherwise defaults to half the available
                 cores.
     progress :  bool
                 Whether to show a progress bar when meshing multiple neurons.
@@ -1631,14 +1776,15 @@
         if len(bodyid) == 1:
             bodyid = bodyid[0]
         else:
             func = partial(mesh_neuron,
                            scale=scale,
                            step_size=step_size,
                            bbox=bbox,
+                           on_error=on_error,
                            server=server,
                            node=node,
                            **kwargs)
 
             if not parallel:
                 return [func(b) for b in tqdm(bodyid,
                                               desc='Meshing',
@@ -1658,44 +1804,51 @@
                               leave=False,
                               disable=not progress) as pbar:
                         for f in as_completed(futures):
                             meshes.append(f.result())
                             pbar.update(1)
                 return meshes
 
-    bodyid = utils.parse_bid(bodyid)
-
-    voxels = get_sparsevol(bodyid,
-                           scale=scale,
-                           ret_type='INDEX',
-                           save_to=None,
-                           bbox=bbox,
-                           server=server,
-                           node=node)
+    try:
+        bodyid = utils.parse_bid(bodyid)
 
-    defaults = dict(chunk_size=200 if scale in (0, 1, 2, 3, 4) else None,
-                    merge_fragments=True,
-                    pad_chunks=True)
-    defaults.update(kwargs)
+        voxels = get_sparsevol(bodyid,
+                            scale=scale,
+                            ret_type='INDEX',
+                            save_to=None,
+                            bbox=bbox,
+                            server=server,
+                            node=node)
+
+        defaults = dict(chunk_size=200 if scale in (0, 1, 2, 3, 4) else None,
+                        merge_fragments=True,
+                        pad_chunks=True)
+        defaults.update(kwargs)
 
-    # Get voxel sizes based on scale
-    info = get_segmentation_info(server, node)['Extended']
+        # Get voxel sizes based on scale
+        info = get_segmentation_info(server, node)['Extended']
 
-    vsize = {'COARSE': [s * 8 for s in info['BlockSize']]}
-    vsize.update({i: np.array(info['VoxelSize']) * 2**i for i in range(info['MaxDownresLevel'])})
+        vsize = {'COARSE': [s * 8 for s in info['BlockSize']]}
+        vsize.update({i: np.array(info['VoxelSize']) * 2**i for i in range(info['MaxDownresLevel'])})
 
-    mesh = meshing.mesh_from_voxels(voxels,
-                                    spacing=vsize[scale],
-                                    step_size=step_size,
-                                    **defaults)
+        mesh = meshing.mesh_from_voxels(voxels,
+                                        spacing=vsize[scale],
+                                        step_size=step_size,
+                                        **defaults)
 
-    # Track the ID just in case
-    mesh.id = bodyid
+        # Track the ID just in case
+        mesh.id = bodyid
 
-    return mesh
+        return mesh
+    except BaseException:
+        if on_error == 'raise':
+            raise
+        elif on_error == 'warn':
+            warnings.warn(f'Error meshing {bodyid}.')
+        return None
 
 
 @lru_cache(None)
 def get_segmentation_info(server=None, node=None):
     """Return segmentation info as dictionary (cached).
 
     Parameters
@@ -2297,21 +2450,155 @@
 
     Returns
     -------
     master :        str
                     ID of master node.
 
     """
+    return get_branch_history(id=id, branch='master', server=server)[0]
+
+
+def get_branch_history(id, branch='master', server=None):
+    """Get list of version UUIDs for the given branch name.
+
+    Starts with the current leaf and works back to the root.
+
+    Parameters
+    ----------
+    id :            str
+                    UUID of a node in the branch to trace.
+    branch :        str
+                    Which branch to follow.
+    server :        str, optional
+                    If not provided will fall back to globally defined server.
+
+    Returns
+    -------
+    uuids :         list of str
+                    IDs sorted from current head to root.
+
+    """
     server, _, _ = eval_param(server)
 
     url = utils.make_url(server, f'api/repo/{id}/branch-versions/master')
 
     r = dvid_session().get(url)
 
     try:
         r.raise_for_status()
     except HTTPError:
         raise HTTPError(f'{r.status_code} {r.reason}: {r.text}')
     except BaseException:
         raise
 
-    return r.json()[0]
+    return r.json()
+
+
+def find_lost_ids(bodyid, branch='master', progress=True, server=None, node=None):
+    """Find the last occurrence of given body ID(s).
+
+    Parameters
+    ----------
+    bodyid :    int | list thereof
+                Body ID(s) to search for.
+    branch :    str
+                Which branch of the tree to track.
+    server :    str, optional
+                If not provided, will try reading from global.
+    node :      str, optional
+                If not provided, will try reading from global.
+
+    """
+    server, node, user = eval_param(server, node)
+
+    if isinstance(bodyid, int):
+        bodyid = [bodyid]
+
+    bodyid = np.asarray(bodyid).astype(int)
+
+    # Get node history
+    hist = get_branch_history(id=node, server=server, branch=branch)
+
+    last_seen = np.full(len(bodyid), None)
+    miss = last_seen == None
+    for n in tqdm(hist, desc='Searching', leave=False, disable=not progress):
+        ex = ids_exist(bodyid[miss], progress=False, node=n, server=server)
+        last_seen[np.where(miss)[0][ex]] = n
+
+        miss = last_seen == None
+        if not any(miss):
+            break
+
+    return last_seen
+
+
+def update_ids(bodyid, scale=3, sample=.01,
+               progress=True, server=None, node=None):
+    """Update (lost) body ID(s).
+
+    The way this work is:
+        1. Find the last node that an ID was seen in.
+        2. Get the coarse voxels for that neuron.
+        3. Find the body ID corresponding to those coarse voxels in given node.
+
+    Parameters
+    ----------
+    bodyid :    int | list thereof
+                Body ID(s) to update.
+    scale :     int | "coarse"
+                Which scale to use. Lower = more accurate but slower.
+    sample :    float [0-1], optional
+                If float between 0 and 1 we will only check a fraction of the
+                voxels (faster).
+    branch :    str
+                Which branch of the tree to track.
+    server :    str, optional
+                If not provided, will try reading from global.
+    node :      str, optional
+                If not provided, will try reading from global.
+
+    """
+    server, node, user = eval_param(server, node)
+
+    if isinstance(bodyid, int):
+        bodyid = [bodyid]
+
+    bodyid = np.asarray(bodyid).astype(int)
+
+    miss = ~ids_exist(bodyid, server=server, node=node)
+    new_ids = bodyid.copy()
+    conf = np.zeros(len(new_ids))
+    conf[miss] = 0
+
+    if any(miss):
+        info = get_segmentation_info(server, node)['Extended']
+        vsize = {'COARSE': [s * 8 for s in info['BlockSize']]}
+        vsize.update({i: np.array(info['VoxelSize']) * 2**i for i in range(info['MaxDownresLevel'])})
+
+        missing = bodyid[miss]
+
+        last_seen = find_lost_ids(missing, progress=progress, server=server, node=node)
+
+        miss_ix = np.where(miss)[0]
+        for i, ix in enumerate(tqdm(miss_ix, desc='Updating', leave=False, disable=not progress)):
+            sv = get_sparsevol(bodyid[ix], scale=scale, node=last_seen[i], server=server)
+
+            if sample:
+                sv = sv[:max(1, int(len(sv) * sample))]
+
+            _ids, _cnt = np.unique(locs_to_ids(sv * vsize[scale] / info['VoxelSize'],
+                                               progress=progress,
+                                               node=node, server=server),
+                                   return_counts=True)
+            srt = np.argsort(_cnt)[::-1]
+            new_ids[ix] = _ids[srt[0]]
+            if len(_ids) > 1:
+                conf[ix] = (_cnt[srt[0]] - _cnt[srt[1]]) / (_cnt[srt[0]] + _cnt[srt[1]])
+            else:
+                conf[ix] = 1
+
+    df = pd.DataFrame()
+    df['old_id'] = bodyid
+    df['new_id'] = new_ids
+    df['confidence'] = conf
+
+    return df
```

### Comparing `dvidtools-0.4.0/dvid/meshing.py` & `dvidtools-0.5.0/dvid/meshing.py`

 * *Files identical despite different names*

### Comparing `dvidtools-0.4.0/dvid/tip.py` & `dvidtools-0.5.0/dvid/tip.py`

 * *Files identical despite different names*

### Comparing `dvidtools-0.4.0/dvid/utils.py` & `dvidtools-0.5.0/dvid/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,11 +518,11 @@
     """
     # Generate the URL
     url = args[0]
     for arg in args[1:]:
         arg_str = str(arg)
         joiner = '' if url.endswith('/') else '/'
         relative = arg_str[1:] if arg_str.startswith('/') else arg_str
-        url = requests.compat.urljoin(url + joiner, relative)
+        url = url + joiner + relative
     if GET:
         url += '?{}'.format(urllib.parse.urlencode(GET))
     return url
```

### Comparing `dvidtools-0.4.0/dvidtools.egg-info/PKG-INFO` & `dvidtools-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 Metadata-Version: 2.1
 Name: dvidtools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Fetch data from DVID server
 Home-page: https://github.com/flyconnectome/dvid_tools
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://dvidtools.readthedocs.io
 Project-URL: Source, https://github.com/flyconnectome/dvid_tools
 Keywords: DVID API fetch neuron segmentation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: extras
 License-File: LICENSE
+Requires-Dist: numpy>=1.15.3
+Requires-Dist: pandas>=0.23.4
+Requires-Dist: setuptools>=40.5.0
+Requires-Dist: tqdm>=4.28.1
+Requires-Dist: scikit-image>=0.14.1
+Requires-Dist: scipy
+Requires-Dist: requests
+Requires-Dist: trimesh
+Requires-Dist: networkx
+Provides-Extra: extras
+Requires-Dist: scikit-learn==0.20.3; extra == "extras"
 
 [![Documentation Status](https://readthedocs.org/projects/dvidtools/badge/?version=latest)](http://dvidtools.readthedocs.io/en/latest/?badge=latest)[![Tests](https://github.com/flyconnectome/dvid_tools/actions/workflows/test-package.yml/badge.svg)](https://github.com/flyconnectome/dvid_tools/actions/workflows/test-package.yml)
 
 # dvidtools
 Python tools to fetch data from [DVID](https://github.com/janelia-flyem/dvid) servers.
 
 Find the documentation [here](https://dvidtools.readthedocs.io).
@@ -35,25 +44,25 @@
 [neuprint-python](https://github.com/connectome-neuprint/neuprint-python).
 
 ## What can `dvidtools` do for you?
 
 - get/set user bookmarks
 - get/set neuron annotations (names)
 - download precomputed meshes, skeletons (SWCs) and ROIs
+- generate meshes or skeletons from scratch
 - get basic neuron info (# of voxels/synapses)
-- get synapses
-- get connectivity (adjacency matrix, connectivity table)
+- fetch synapses
+- fetch connectivity (adjacency matrix, connectivity table)
 - retrieve labels (TODO, to split, etc)
 - map positions to body IDs
-- mesh or skeletonize sparsevols
 - detect potential open ends (based on a script by [Stephen Plaza](https://github.com/stephenplaza))
 
 ## Install
 
-Make sure you have [Python 3](https://www.python.org) (3.6 or later),
+Make sure you have [Python 3](https://www.python.org) (3.8 or later),
 [pip](https://pip.pypa.io/en/stable/installing/). Then run this:
 
 ```bash
 pip3 install dvidtools
 ```
 
 To install the dev version straight from Github:
```

### Comparing `dvidtools-0.4.0/setup.py` & `dvidtools-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,18 @@
 
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
 
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     install_requires=requirements,
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     extras_require={'extras': ['scikit-learn==0.20.3']},
     include_package_data=True,
     zip_safe=False
 )
```

