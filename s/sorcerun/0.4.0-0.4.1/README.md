# Comparing `tmp/sorcerun-0.4.0.tar.gz` & `tmp/sorcerun-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorcerun-0.4.0.tar", last modified: Tue May  7 17:03:15 2024, max compression
+gzip compressed data, was "sorcerun-0.4.1.tar", last modified: Mon May 13 22:53:47 2024, max compression
```

## Comparing `sorcerun-0.4.0.tar` & `sorcerun-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:03:15.666714 sorcerun-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-07 17:03:11.000000 sorcerun-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 17:03:15.666714 sorcerun-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-07 17:03:11.000000 sorcerun-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:03:15.666714 sorcerun-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-07 17:03:11.000000 sorcerun-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:03:15.666714 sorcerun-0.4.0/sorcerun/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/auth_mongodb_option.py
--rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/grid_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/grid_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/incense_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/mongodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-07 17:03:11.000000 sorcerun-0.4.0/sorcerun/sacred_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:03:15.666714 sorcerun-0.4.0/sorcerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 17:03:15.000000 sorcerun-0.4.0/sorcerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:53:47.540440 sorcerun-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-13 22:53:43.000000 sorcerun-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-13 22:53:47.540440 sorcerun-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-13 22:53:43.000000 sorcerun-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 22:53:47.540440 sorcerun-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-13 22:53:43.000000 sorcerun-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:53:47.540440 sorcerun-0.4.1/sorcerun/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/auth_mongodb_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/grid_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/grid_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/incense_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/mongodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-13 22:53:43.000000 sorcerun-0.4.1/sorcerun/sacred_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 22:53:47.540440 sorcerun-0.4.1/sorcerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 22:53:47.000000 sorcerun-0.4.1/sorcerun.egg-info/top_level.txt
```

### Comparing `sorcerun-0.4.0/LICENSE` & `sorcerun-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/PKG-INFO` & `sorcerun-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.4.0
+Version: 0.4.1
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: sacred
 Requires-Dist: pymongo
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: incense
 Requires-Dist: xarray
 Requires-Dist: tqdm
 Requires-Dist: streamlit
+Requires-Dist: ipdb
 
 Computational experiments can be boiled down to calling a function with some inputs. A common form of analysis is to see how the results of the function varies with different inputs. Sorcerun is a tool built on top of [`sacred`](https://github.com/IDSIA/sacred) that facilitates **logging** each function call to avoid having to repeat experiments that have already been run.
```

### Comparing `sorcerun-0.4.0/README.md` & `sorcerun-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/setup.py` & `sorcerun-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sorcerun",
-    version="0.4.0",
+    version="0.4.1",
     packages=find_packages(),
     install_requires=[
         "click",
         # "sacred @ git+https://github.com/rajatvd/sacred.git",
         "sacred",
         "pymongo",
         "pyyaml",
         "scikit-learn",
         "incense",
         "xarray",
         "tqdm",
         "streamlit",
+        "ipdb"
     ],
     entry_points="""
         [console_scripts]
         sorcerun=sorcerun.cli:sorcerun
     """,
     long_description="Computational experiments can be boiled down to calling a function with some inputs. A common form of analysis is to see how the results of the function varies with different inputs. Sorcerun is a tool built on top of [`sacred`](https://github.com/IDSIA/sacred) that facilitates **logging** each function call to avoid having to repeat experiments that have already been run.",
 )
```

### Comparing `sorcerun-0.4.0/sorcerun/adapter.py` & `sorcerun-0.4.1/sorcerun/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     norms = np.linalg.norm(X, axis=0)
     X /= norms
 
     # generate a Gaussian sketch matrix of size k x d
     S = np.random.randn(k, d) / np.sqrt(k)
 
     # sketch the data
-
     Y = S @ X
 
     # measure distortion for each data point
     new_norms = np.linalg.norm(Y, axis=0)
 
     distortions = np.abs(new_norms - 1)
 
@@ -31,11 +30,13 @@
 
     output = (
         f"mean distortion: {distortions.mean()}, max distortion: {distortions.max()}"
     )
     return output
 
 
+adapter.experiment_name = "jl_lemma_test"
+
 if __name__ == "__main__":
     from config import config
 
     print(adapter(config, DummyRun()))
```

### Comparing `sorcerun-0.4.0/sorcerun/auth_mongodb_option.py` & `sorcerun-0.4.1/sorcerun/auth_mongodb_option.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/sorcerun/cli.py` & `sorcerun-0.4.1/sorcerun/cli.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/sorcerun/config.py` & `sorcerun-0.4.1/sorcerun/config.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/sorcerun/grid_config.py` & `sorcerun-0.4.1/sorcerun/grid_config.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/sorcerun/grid_plotter.py` & `sorcerun-0.4.1/sorcerun/grid_plotter.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,27 +11,64 @@
 st.title("Grid Plotter")
 # show current working directory
 working_dir = os.getcwd()
 st.write(f"Current working directory: `{working_dir}`")
 
 st.title("Settings")
 
+# Checkbox to decide whether to show all grid ids or only the ones with tags
+show_all_grids = not st.checkbox("Show only tagged grids", value=False)
+
+# Extract grid ids
+name_to_gid = {}
+for f in os.listdir(GRID_OUTPUTS):
+    if os.path.isdir(os.path.join(GRID_OUTPUTS, f)):
+        gid = f
+        tags_file = os.path.join(GRID_OUTPUTS, gid, f"{gid}-tags.txt")
+
+        tags = ""
+        if os.path.exists(tags_file):
+            with open(tags_file, "r") as f:
+                tags = f" tags: {f.read().strip()}"
+
+        if show_all_grids or tags:
+            name_to_gid[f"{gid}{tags}"] = gid
 
-# Extract all grid ids (they are the names of the subdirectories in GRID_OUTPUTS)
-grid_ids = [
-    f for f in os.listdir(GRID_OUTPUTS) if os.path.isdir(os.path.join(GRID_OUTPUTS, f))
-]
 
 # Select a grid id
-grid_id = st.selectbox("Choose a Grid ID", grid_ids)
+name = st.selectbox("Choose a Grid ID", list(name_to_gid.keys()))
+grid_id = name_to_gid[name]
+
+# Add a text box to modify tags for the selected grid id
+tags_file = os.path.join(GRID_OUTPUTS, grid_id, f"{grid_id}-tags.txt")
+tags = ""
+if os.path.exists(tags_file):
+    with open(tags_file, "r") as f:
+        tags = f.read().strip()
+
+new_tags = st.text_input("Tags", value=tags)
+
+# Add a button to save the tags
+if st.button("Save tags"):
+    # delete the tags file if the new tags are empty
+    if not new_tags:
+        if os.path.exists(tags_file):
+            os.remove(tags_file)
+    else:
+        with open(tags_file, "w") as f:
+            f.write(new_tags)
+    st.rerun()
+
+st.write(f"Selected grid id: `{grid_id}`")
 
 
 # Load the netcdf file for the selected grid id as an xarray
 grid_output_dir = os.path.join(GRID_OUTPUTS, grid_id)
 netcdf_file = os.path.join(grid_output_dir, f"{grid_id}.nc")
+
 data = xr.open_dataarray(netcdf_file)
 
 # get dims with more than 1 coordinate
 dims = sorted([dim for dim in data.dims if len(data[dim]) > 1 and dim != "metric"])
 
 # get metric names
 
@@ -120,14 +157,16 @@
         st.text("")
         log_y = st.checkbox("Log scale y axis", value=False)
     with col3y:
         y_label = st.text_input("Y label", value="metric")
 # Remaining dims
 remaining_dims = sorted(list(set(new_dims) - set([x_axis, "metric"])))
 
+# Choose a style for the plot
+style = st.text_input("Line style", value="o-")
 
 # Choose plot dimensions to include within a single plot
 st.subheader("Choose dimensions that are kept fixed in each plot")
 fixed_dims_per_plot = st.multiselect(
     "Fixed dims per plot",
     remaining_dims,
 )
@@ -195,15 +234,15 @@
 
                 # check if y is all nans or infs, if so, don't plot
                 good_inds = np.isfinite(y)
 
                 # dont_plot = y.isnull().all().item() or (y == float("inf")).all().item()
                 dont_plot = not np.any(good_inds)
                 if not dont_plot:
-                    plt.plot(x, y, "-o", label=label)
+                    plt.plot(x, y, style, label=label)
                     # add regression line slope
                     if len(x) > 1 and show_slope:
                         x_to_regress = np.log(x) if log_x else x
                         y_to_regress = np.log(y) if log_y else y
 
                         # remove nans and infs
                         keep_inds = np.isfinite(x_to_regress) & np.isfinite(
```

### Comparing `sorcerun-0.4.0/sorcerun/incense_utils.py` & `sorcerun-0.4.1/sorcerun/incense_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/sorcerun/mongodb_utils.py` & `sorcerun-0.4.1/sorcerun/mongodb_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/sorcerun/sacred_utils.py` & `sorcerun-0.4.1/sorcerun/sacred_utils.py`

 * *Files identical despite different names*

### Comparing `sorcerun-0.4.0/sorcerun.egg-info/PKG-INFO` & `sorcerun-0.4.1/sorcerun.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sorcerun
-Version: 0.4.0
+Version: 0.4.1
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: sacred
 Requires-Dist: pymongo
 Requires-Dist: pyyaml
 Requires-Dist: scikit-learn
 Requires-Dist: incense
 Requires-Dist: xarray
 Requires-Dist: tqdm
 Requires-Dist: streamlit
+Requires-Dist: ipdb
 
 Computational experiments can be boiled down to calling a function with some inputs. A common form of analysis is to see how the results of the function varies with different inputs. Sorcerun is a tool built on top of [`sacred`](https://github.com/IDSIA/sacred) that facilitates **logging** each function call to avoid having to repeat experiments that have already been run.
```

