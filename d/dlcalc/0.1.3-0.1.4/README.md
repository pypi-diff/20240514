# Comparing `tmp/dlcalc-0.1.3.tar.gz` & `tmp/dlcalc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlcalc-0.1.3.tar", last modified: Tue May 14 02:13:52 2024, max compression
+gzip compressed data, was "dlcalc-0.1.4.tar", last modified: Tue May 14 18:23:09 2024, max compression
```

## Comparing `dlcalc-0.1.3.tar` & `dlcalc-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:13:52.827536 dlcalc-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 02:13:52.827536 dlcalc-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-14 02:13:48.000000 dlcalc-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:13:52.823536 dlcalc-0.1.3/dlcalc/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-14 02:13:48.000000 dlcalc-0.1.3/dlcalc/summarize_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-14 02:13:48.000000 dlcalc-0.1.3/dlcalc/training_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:13:52.827536 dlcalc-0.1.3/dlcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-14 02:13:48.000000 dlcalc-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:13:52.827536 dlcalc-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:09.479992 dlcalc-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 18:23:09.479992 dlcalc-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-14 18:23:05.000000 dlcalc-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:09.479992 dlcalc-0.1.4/dlcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-14 18:23:05.000000 dlcalc-0.1.4/dlcalc/summarize_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-14 18:23:05.000000 dlcalc-0.1.4/dlcalc/training_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 18:23:09.479992 dlcalc-0.1.4/dlcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 18:23:09.000000 dlcalc-0.1.4/dlcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 18:23:09.000000 dlcalc-0.1.4/dlcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 18:23:09.000000 dlcalc-0.1.4/dlcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 18:23:09.000000 dlcalc-0.1.4/dlcalc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 18:23:09.000000 dlcalc-0.1.4/dlcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 18:23:09.000000 dlcalc-0.1.4/dlcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-14 18:23:05.000000 dlcalc-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 18:23:09.479992 dlcalc-0.1.4/setup.cfg
```

### Comparing `dlcalc-0.1.3/PKG-INFO` & `dlcalc-0.1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlcalc
-Version: 0.1.3
+Version: 0.1.4
 Author-email: Justin Chiu <jfc4050@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: PyYAML>=6.0.1
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: ruff>=0.4.3; extra == "dev"
```

### Comparing `dlcalc-0.1.3/README.md` & `dlcalc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dlcalc-0.1.3/dlcalc/summarize_checkpoint.py` & `dlcalc-0.1.4/dlcalc/summarize_checkpoint.py`

 * *Files identical despite different names*

### Comparing `dlcalc-0.1.3/dlcalc/training_3d.py` & `dlcalc-0.1.4/dlcalc/training_3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,27 +94,29 @@
     # activations
     print_section_header("[MEMORY] TRAINING ACTIVATIONS")
     act_size_per_layer_per_inflight_microbatch = (
         model_repr.activation_size_per_microbatch_per_layer()
     )
     print("act/layer/inflight:", act_size_per_layer_per_inflight_microbatch)
     max_inflight_microbatches = model_repr.parallelism_cfg.pp  # 1F1B
+    print("max(inflight):", max_inflight_microbatches)
     layers_per_pp_stage = model_repr.layers_per_pp_stage()
-    vpp_penalty = model_repr.vpp_penalty()
-    print(f"VPP memory penalty = {vpp_penalty:.2f}")
+    print("layers/pp:", layers_per_pp_stage)
+    vpp_multiplier = model_repr.vpp_penalty()
+    print(f"VPP memory multiplier = {vpp_multiplier:.2f}")
     act_memory = (
         act_size_per_layer_per_inflight_microbatch
-        * max(n_microbatches_per_mp_rank, max_inflight_microbatches)
-        * math.ceil(vpp_penalty * layers_per_pp_stage)
+        * min(n_microbatches_per_mp_rank, max_inflight_microbatches)
+        * math.ceil(vpp_multiplier * layers_per_pp_stage)
     )
     print(
         f"act/pp_stage = "
         f"per_microbatch_per_layer_per_inflight * "
         f"{max_inflight_microbatches} * "
-        f"{math.ceil(vpp_penalty * layers_per_pp_stage)} = "
+        f"{math.ceil(vpp_multiplier * layers_per_pp_stage)} = "
         f"{act_memory}"
     )
 
     print_section_header("[MEMORY] TOTAL")
     print(
         f"total mem (GiB) = {(model_repr.states.total_bytes(partitioned=True) + act_memory.bytes()) / (1024 ** 3):.3f}GiB"
     )
```

### Comparing `dlcalc-0.1.3/dlcalc.egg-info/PKG-INFO` & `dlcalc-0.1.4/dlcalc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlcalc
-Version: 0.1.3
+Version: 0.1.4
 Author-email: Justin Chiu <jfc4050@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: PyYAML>=6.0.1
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: ruff>=0.4.3; extra == "dev"
```

### Comparing `dlcalc-0.1.3/pyproject.toml` & `dlcalc-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dlcalc"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     {name = "Justin Chiu", email = "jfc4050@gmail.com"}
 ]
 requires-python = ">=3.9"
 dependencies = [
     "PyYAML>=6.0.1"
 ]
```

