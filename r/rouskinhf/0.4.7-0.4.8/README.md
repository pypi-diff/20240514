# Comparing `tmp/rouskinhf-0.4.7.tar.gz` & `tmp/rouskinhf-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouskinhf-0.4.7.tar", last modified: Fri Dec 22 01:05:12 2023, max compression
+gzip compressed data, was "rouskinhf-0.4.8.tar", last modified: Tue May 14 17:04:12 2024, max compression
```

## Comparing `rouskinhf-0.4.7.tar` & `rouskinhf-0.4.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2023-12-22 01:05:12.802863 rouskinhf-0.4.7/
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.4.7/LICENSE
--rw-r--r--   0 yvesmartin   (501) staff       (20)       25 2023-12-11 16:47:32.000000 rouskinhf-0.4.7/MANIFEST.in
--rw-r--r--   0 yvesmartin   (501) staff       (20)     8254 2023-12-22 01:05:12.802607 rouskinhf-0.4.7/PKG-INFO
--rw-r--r--   0 yvesmartin   (501) staff       (20)     6497 2023-12-09 21:56:49.000000 rouskinhf-0.4.7/README.md
--rw-r--r--   0 yvesmartin   (501) staff       (20)      840 2023-12-22 01:03:13.000000 rouskinhf-0.4.7/pyproject.toml
--rw-r--r--   0 yvesmartin   (501) staff       (20)      164 2023-12-11 16:44:18.000000 rouskinhf-0.4.7/requirements.txt
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2023-12-22 01:05:12.801590 rouskinhf-0.4.7/rouskinhf/
--rw-r--r--   0 yvesmartin   (501) staff       (20)      163 2023-12-22 01:03:27.000000 rouskinhf-0.4.7/rouskinhf/__init__.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     2818 2023-12-18 05:49:03.000000 rouskinhf-0.4.7/rouskinhf/conversion.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)    11028 2023-12-22 01:03:20.000000 rouskinhf-0.4.7/rouskinhf/datapoint.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)      656 2023-12-18 05:49:03.000000 rouskinhf-0.4.7/rouskinhf/env.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     6560 2023-12-18 05:49:03.000000 rouskinhf-0.4.7/rouskinhf/filter.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     4134 2023-12-18 05:49:03.000000 rouskinhf-0.4.7/rouskinhf/hf.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     6665 2023-12-18 05:49:03.000000 rouskinhf-0.4.7/rouskinhf/list_datapoints.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     5927 2023-12-12 02:27:22.000000 rouskinhf-0.4.7/rouskinhf/parsers.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1846 2023-12-11 16:44:18.000000 rouskinhf-0.4.7/rouskinhf/path.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     6630 2023-12-11 16:44:18.000000 rouskinhf-0.4.7/rouskinhf/rnastructure.py
--rw-r--r--   0 yvesmartin   (501) staff       (20)     2779 2023-12-22 01:03:20.000000 rouskinhf-0.4.7/rouskinhf/util.py
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2023-12-22 01:05:12.802381 rouskinhf-0.4.7/rouskinhf.egg-info/
--rw-r--r--   0 yvesmartin   (501) staff       (20)     8254 2023-12-22 01:05:12.000000 rouskinhf-0.4.7/rouskinhf.egg-info/PKG-INFO
--rw-r--r--   0 yvesmartin   (501) staff       (20)      436 2023-12-22 01:05:12.000000 rouskinhf-0.4.7/rouskinhf.egg-info/SOURCES.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)        1 2023-12-22 01:05:12.000000 rouskinhf-0.4.7/rouskinhf.egg-info/dependency_links.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)       10 2023-12-22 01:05:12.000000 rouskinhf-0.4.7/rouskinhf.egg-info/top_level.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)       38 2023-12-22 01:05:12.802902 rouskinhf-0.4.7/setup.cfg
--rw-r--r--   0 yvesmartin   (501) staff       (20)      205 2023-12-11 16:46:01.000000 rouskinhf-0.4.7/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2024-05-14 17:04:12.112992 rouskinhf-0.4.8/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1141 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)       25 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/MANIFEST.in
+-rw-r--r--   0 ymdt       (501) staff       (20)     3747 2024-05-14 17:04:12.112805 rouskinhf-0.4.8/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)     1990 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/README.md
+-rw-r--r--   0 ymdt       (501) staff       (20)      840 2024-05-14 17:00:15.000000 rouskinhf-0.4.8/pyproject.toml
+-rw-r--r--   0 ymdt       (501) staff       (20)      164 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/requirements.txt
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2024-05-14 17:04:12.111955 rouskinhf-0.4.8/rouskinhf/
+-rw-r--r--   0 ymdt       (501) staff       (20)      163 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2818 2024-05-14 16:54:39.000000 rouskinhf-0.4.8/rouskinhf/conversion.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    11049 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/datapoint.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      656 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/env.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6723 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/filter.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     4122 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/hf.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6665 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/list_datapoints.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     5927 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/parsers.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1846 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6630 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/rnastructure.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      585 2024-05-14 16:58:41.000000 rouskinhf-0.4.8/rouskinhf/test.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2862 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/rouskinhf/util.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2024-05-14 17:04:12.112618 rouskinhf-0.4.8/rouskinhf.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)     3747 2024-05-14 17:04:12.000000 rouskinhf-0.4.8/rouskinhf.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      454 2024-05-14 17:04:12.000000 rouskinhf-0.4.8/rouskinhf.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2024-05-14 17:04:12.000000 rouskinhf-0.4.8/rouskinhf.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       10 2024-05-14 17:04:12.000000 rouskinhf-0.4.8/rouskinhf.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2024-05-14 17:04:12.113027 rouskinhf-0.4.8/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      205 2024-05-14 16:45:49.000000 rouskinhf-0.4.8/setup.py
```

### Comparing `rouskinhf-0.4.7/LICENSE` & `rouskinhf-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.4.7/pyproject.toml` & `rouskinhf-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['rouskinhf']
 
 [project]
 name =  "rouskinhf"
-version = "0.4.7"
+version = "0.4.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to manipulate data for our DMS prediction models."
 readme = "README.md"
```

### Comparing `rouskinhf-0.4.7/rouskinhf/conversion.py` & `rouskinhf-0.4.8/rouskinhf/conversion.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.4.7/rouskinhf/datapoint.py` & `rouskinhf-0.4.8/rouskinhf/datapoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         >>> datapoint = Datapoint(reference='reference', sequence='AACCGG', structure=[[1, 2], [3, -1]])
         >>> datapoint._assert_structure()
         False
         """
         sequence = self.sequence
         structure = self.structure
 
-        if structure is None:
+        if structure is None or structure == [[]]:
             return True
         return (
             all(
                 # check boundaries
                 [
                     0 <= pair[0] < len(sequence)
                     and 0 <= pair[1] < len(sequence)
```

### Comparing `rouskinhf-0.4.7/rouskinhf/env.py` & `rouskinhf-0.4.8/rouskinhf/env.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.4.7/rouskinhf/filter.py` & `rouskinhf-0.4.8/rouskinhf/filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,17 +108,20 @@
                 "dms" if "dms" in row and not type(row["dms"]) == float else "shape"
             )
             if (
                 (not "structure" in row)
                 or (row["structure"] is None)
                 or (type(row["structure"]) == float and np.isnan(row["structure"]))
                 or len(row["structure"]) == 0
+                or row['structure'] == [[]]
             ):
                 return 1  #  if you can't calculate the AUROC, don't filter it out
 
+            if row[signal] is None or (type(row[signal]) == float and np.isnan(row[signal])):
+                return 1
             sig = np.array(row[signal])
             if signal == "dms":  # mask G/T/U bases for DMS
                 mask_UKN = np.array([s in "GTU" for s in row["sequence"].upper()])
                 sig[mask_UKN] = UKN
 
             isUnpaired = np.ones_like(sig)
             isUnpaired[np.array(row["structure"]).flatten()] = 0
```

### Comparing `rouskinhf-0.4.7/rouskinhf/hf.py` & `rouskinhf-0.4.8/rouskinhf/hf.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,28 +23,28 @@
     path = Path(name=name, root=path)
 
     if force_download:
         os.system(f"rm -rf {path.get_main_folder()}")
 
     if not exists(path.get_data_json()):
         print("{}: Downloading dataset from HuggingFace Hub...".format(name))
-        download_dataset(name)
+        download_dataset(path)
         print(
             "{}: Download complete. File saved at {}".format(name, path.get_data_json())
         )
 
     return json.load(open(path.get_data_json(), "r"))
 
 
-def download_dataset(name: str, root="data"):
+def download_dataset(path: Path):
     """Download a dataset from HuggingFace Hub. The name corresponds to the name of the dataset on HuggingFace Hub."""
     snapshot_download(
-        repo_id="rouskinlab/" + name,
+        repo_id="rouskinlab/" + path.name,
         repo_type="dataset",
-        local_dir=Path(name, root).get_main_folder(),
+        local_dir=dirname(path.get_data_json()),
         token=Env.get_hf_token(),
         allow_patterns=["data.json"],
     )
 
 
 def name_from_path(datapath: str):
     if datapath.split("/")[-1] == "data.json":
```

### Comparing `rouskinhf-0.4.7/rouskinhf/list_datapoints.py` & `rouskinhf-0.4.8/rouskinhf/list_datapoints.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.4.7/rouskinhf/parsers.py` & `rouskinhf-0.4.8/rouskinhf/parsers.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.4.7/rouskinhf/path.py` & `rouskinhf-0.4.8/rouskinhf/path.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.4.7/rouskinhf/rnastructure.py` & `rouskinhf-0.4.8/rouskinhf/rnastructure.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.4.7/rouskinhf/util.py` & `rouskinhf-0.4.8/rouskinhf/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,16 @@
             data.items()
         ):  # write the datapoints one by one to avoid memory issues
             remove_keys = []
             for k, v in attr.items():
                 if (
                     v is None
                     or (type(v) == float and np.isnan(v))
-                    or (hasattr(v, "__iter__") and not len(v))
+                    # or (hasattr(v, "__iter__") and not len(v))
                 ):
                     remove_keys.append(k)
+                if isinstance(v, np.ndarray):
+                    v = v.tolist()
             for k in remove_keys:
                 del attr[k]
             f.write(str({ref: attr})[1:-1].replace("'", '"'))
             f.write(",\n" if idx != len(data) - 1 else "\n}")
```

