# Comparing `tmp/dlcalc-0.1.2.tar.gz` & `tmp/dlcalc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlcalc-0.1.2.tar", last modified: Fri May 10 06:53:05 2024, max compression
+gzip compressed data, was "dlcalc-0.1.3.tar", last modified: Tue May 14 02:13:52 2024, max compression
```

## Comparing `dlcalc-0.1.2.tar` & `dlcalc-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:53:05.281983 dlcalc-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 06:53:05.281983 dlcalc-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-10 06:52:59.000000 dlcalc-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:53:05.277983 dlcalc-0.1.2/dlcalc/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-10 06:52:59.000000 dlcalc-0.1.2/dlcalc/summarize_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-05-10 06:52:59.000000 dlcalc-0.1.2/dlcalc/training_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:53:05.281983 dlcalc-0.1.2/dlcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 06:53:05.000000 dlcalc-0.1.2/dlcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-10 06:53:05.000000 dlcalc-0.1.2/dlcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:53:05.000000 dlcalc-0.1.2/dlcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 06:53:05.000000 dlcalc-0.1.2/dlcalc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 06:53:05.000000 dlcalc-0.1.2/dlcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 06:53:05.000000 dlcalc-0.1.2/dlcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-10 06:52:59.000000 dlcalc-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:53:05.281983 dlcalc-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:13:52.827536 dlcalc-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 02:13:52.827536 dlcalc-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-14 02:13:48.000000 dlcalc-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:13:52.823536 dlcalc-0.1.3/dlcalc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-14 02:13:48.000000 dlcalc-0.1.3/dlcalc/summarize_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-14 02:13:48.000000 dlcalc-0.1.3/dlcalc/training_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 02:13:52.827536 dlcalc-0.1.3/dlcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 02:13:52.000000 dlcalc-0.1.3/dlcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-14 02:13:48.000000 dlcalc-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 02:13:52.827536 dlcalc-0.1.3/setup.cfg
```

### Comparing `dlcalc-0.1.2/PKG-INFO` & `dlcalc-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: dlcalc
-Version: 0.1.2
+Version: 0.1.3
 Author-email: Justin Chiu <jfc4050@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: PyYAML>=6.0.1
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: ruff>=0.4.3; extra == "dev"
 
 # dlcalc
+[![PyPI version](https://badge.fury.io/py/dlcalc.svg)](https://badge.fury.io/py/dlcalc)
 ![checks](https://github.com/jfc4050/dlcalc/actions/workflows/python-app.yml/badge.svg)
 
 random command line tools for deep learning
 
-install CLI
+## Installation
 ```bash
+pip install dlcalc
+```
+
+or
+
+```bash
+git clone https://github.com/jfc4050/dlcalc
+cd dlcalc
 pip install -e .
 ```
 
 ## Tools
 ### 3D Training Calculator
 calculator for estimating various performance characteristics of 3D parallel
 transformer model training:
```

### Comparing `dlcalc-0.1.2/README.md` & `dlcalc-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # dlcalc
+[![PyPI version](https://badge.fury.io/py/dlcalc.svg)](https://badge.fury.io/py/dlcalc)
 ![checks](https://github.com/jfc4050/dlcalc/actions/workflows/python-app.yml/badge.svg)
 
 random command line tools for deep learning
 
-install CLI
+## Installation
 ```bash
+pip install dlcalc
+```
+
+or
+
+```bash
+git clone https://github.com/jfc4050/dlcalc
+cd dlcalc
 pip install -e .
 ```
 
 ## Tools
 ### 3D Training Calculator
 calculator for estimating various performance characteristics of 3D parallel
 transformer model training:
```

### Comparing `dlcalc-0.1.2/dlcalc/summarize_checkpoint.py` & `dlcalc-0.1.3/dlcalc/summarize_checkpoint.py`

 * *Files identical despite different names*

### Comparing `dlcalc-0.1.2/dlcalc/training_3d.py` & `dlcalc-0.1.3/dlcalc/training_3d.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     print_section_header("CONFIG")
     print(json.dumps(cfg, indent=2))
 
     sequence_len = cfg["data"]["seqlen"]
     microbatch_sz = cfg["data"]["microbatch_sz"]
     hidden_sz = cfg["model"]["hidden_sz"]
 
-    model_def = ThreeDParallelModel(
+    model_repr = ThreeDParallelModel(
         parallelism_cfg=ParallelConfig(
             tp=cfg["parallelism"]["tp"],
             pp=cfg["parallelism"]["pp"],
             dp=cfg["parallelism"]["dp"],
             vpp=cfg["parallelism"]["vpp"],
             sp_enabled=cfg["parallelism"]["sp"],
             zero_level=ParallelConfig.ZeroLevel(cfg["parallelism"]["zero_level"]),
@@ -60,83 +60,99 @@
         act_ckpting_type=ActivationCheckpointingType.from_str(
             cfg["performance"]["activation_checkpointing_type"]
         ),
         bucket_size_bytes=int(cfg["parallelism"]["bucket_size_mb"] * 1e6),
     )
 
     machine_spec = MachineSpec.from_str(cfg["hardware"]["node_type"])
-    cluster_size = model_def.parallelism_cfg.world_size()
+    cluster_size = model_repr.parallelism_cfg.world_size()
     print(machine_spec)
     print("n_devices: ", cluster_size)
     print("n_nodes: ", safe_divide(cluster_size, machine_spec.n_devices))
 
     ###################################################################################
+    # DATA
+    ###################################################################################
+    print_section_header("DATA")
+    gbs = cfg["data"]["gbs"]
+    mbs = cfg["data"]["microbatch_sz"]
+
+    bs_per_mp_rank = safe_divide(gbs, model_repr.parallelism_cfg.dp)
+    n_microbatches_per_mp_rank = safe_divide(bs_per_mp_rank, mbs)
+
+    print(f"gbs = {gbs}")
+    print(f"gbs/pipeline = {bs_per_mp_rank}")
+    print(f"n_microbatches/pipeline = {n_microbatches_per_mp_rank}")
+
+    ###################################################################################
     # MEMORY ANALYSIS
     ###################################################################################
 
     print_section_header("[MEMORY] STATES")
-    print(f"total params: {model_def.get_total_n_params(partitioned=False) * 1e-9:.2f}B")
-    print(model_def.states)
+    print(f"total params: {model_repr.get_total_n_params(partitioned=False) * 1e-9:.2f}B")
+    print(model_repr.states)
 
     # activations
     print_section_header("[MEMORY] TRAINING ACTIVATIONS")
-    per_microbatch_per_layer_per_inflight = model_def.activation_size_per_microbatch_per_layer()
-    print("act/layer/inflight:", per_microbatch_per_layer_per_inflight)
-    max_inflight_microbatches = model_def.max_inflight_microbatches()
-    layers_per_pp_stage = model_def.layers_per_pp_stage()
-    vpp_penalty = model_def.vpp_penalty()
+    act_size_per_layer_per_inflight_microbatch = (
+        model_repr.activation_size_per_microbatch_per_layer()
+    )
+    print("act/layer/inflight:", act_size_per_layer_per_inflight_microbatch)
+    max_inflight_microbatches = model_repr.parallelism_cfg.pp  # 1F1B
+    layers_per_pp_stage = model_repr.layers_per_pp_stage()
+    vpp_penalty = model_repr.vpp_penalty()
     print(f"VPP memory penalty = {vpp_penalty:.2f}")
     act_memory = (
-        per_microbatch_per_layer_per_inflight
-        * max_inflight_microbatches
+        act_size_per_layer_per_inflight_microbatch
+        * max(n_microbatches_per_mp_rank, max_inflight_microbatches)
         * math.ceil(vpp_penalty * layers_per_pp_stage)
     )
     print(
         f"act/pp_stage = "
         f"per_microbatch_per_layer_per_inflight * "
         f"{max_inflight_microbatches} * "
         f"{math.ceil(vpp_penalty * layers_per_pp_stage)} = "
         f"{act_memory}"
     )
 
     print_section_header("[MEMORY] TOTAL")
     print(
-        f"total mem (GiB) = {(model_def.states.total_bytes(partitioned=True) + act_memory.bytes()) / (1024 ** 3):.3f}GiB"
+        f"total mem (GiB) = {(model_repr.states.total_bytes(partitioned=True) + act_memory.bytes()) / (1024 ** 3):.3f}GiB"
     )
 
     ###################################################################################
     # PERF ANALYSIS
     ###################################################################################
     print_section_header("GEMMs (note numbers calculated for 100% flops+bandwidth utilization)")
     for proj_name, weight_repr in [
-        ("QKV", model_def.qkv_weight),
-        ("ATTN_OUT", model_def.attn_out_weight),
-        ("MLP1", model_def.mlp_up_weight),
-        ("MLP2", model_def.mlp_down_weight),
+        ("QKV", model_repr.qkv_weight),
+        ("ATTN_OUT", model_repr.attn_out_weight),
+        ("MLP1", model_repr.mlp_up_weight),
+        ("MLP2", model_repr.mlp_down_weight),
     ]:
         weight_partitioned_shape = weight_repr.shape(partitioned=True)
         weight_unpartitioned_shape = weight_repr.shape(partitioned=False)
         flops = compute_gemm_flops(
             weight_partitioned_shape,
-            seqlen=model_def.sequence_len,
-            batch_sz=model_def.microbatch_sz,
+            seqlen=model_repr.sequence_len,
+            batch_sz=model_repr.microbatch_sz,
         )
         print(f"{proj_name} {weight_unpartitioned_shape} --tp--> {weight_partitioned_shape}")
         print(
             f"\tCOMPUTE: {flops * 1e-12:.2f} TFLOPs -> "
             f"{flops/machine_spec.device_spec.peak_flops * 1000:.3f} ms"
         )
-        bytes_per_element = model_def.bits_per_parameter // 8
+        bytes_per_element = model_repr.bits_per_parameter // 8
         gemm_input_dim, gemm_output_dim = weight_partitioned_shape
         weight_bytes = bytes_per_element * product(weight_partitioned_shape)
         input_bytes = bytes_per_element * product(
-            (model_def.sequence_len, model_def.microbatch_sz, gemm_input_dim)
+            (model_repr.sequence_len, model_repr.microbatch_sz, gemm_input_dim)
         )
         output_bytes = bytes_per_element * product(
-            (model_def.sequence_len, model_def.microbatch_sz, gemm_output_dim)
+            (model_repr.sequence_len, model_repr.microbatch_sz, gemm_output_dim)
         )
         print(
             f"\tLOAD INPUT: {input_bytes * 1e-9:.2f} GB -> "
             f"{input_bytes / (machine_spec.device_spec.mem_bandwidth_bytes_per_sec) * 1000:.3f} ms"
         )
         print(
             f"\tLOAD_WEIGHT: {weight_bytes * 1e-9:.2f} GB -> "
@@ -147,50 +163,48 @@
             f"{output_bytes / (machine_spec.device_spec.mem_bandwidth_bytes_per_sec) * 1000:.3f} ms"
         )
 
     print_section_header("TP COMMUNICATION")
     # TODO. assumes SP, analysis pretty similar if not SP though
     activation_size = Size(
         numel=sequence_len * microbatch_sz * hidden_sz,
-        bits_per_element=model_def.bits_per_parameter,
+        bits_per_element=model_repr.bits_per_parameter,
     )
     print(
-        f"TP all-gather: {activation_size}: {get_tp_all_gather_comm_time_s(size=activation_size, n_participants=model_def.parallelism_cfg.tp, machine_spec=machine_spec) * 1000:.3f} ms"
+        f"TP all-gather: {activation_size}: {get_tp_all_gather_comm_time_s(size=activation_size, n_participants=model_repr.parallelism_cfg.tp, machine_spec=machine_spec) * 1000:.3f} ms"
     )
     print(
-        f"TP reduce-scatter: {activation_size}: {get_tp_reduce_scatter_comm_time_s(size=activation_size, n_participants=model_def.parallelism_cfg.tp, machine_spec=machine_spec) * 1000:.3f} ms"
+        f"TP reduce-scatter: {activation_size}: {get_tp_reduce_scatter_comm_time_s(size=activation_size, n_participants=model_repr.parallelism_cfg.tp, machine_spec=machine_spec) * 1000:.3f} ms"
     )
 
     print_section_header("PIPELINE BUBBLE")
-    gbs = cfg["data"]["gbs"]
-    mbs = cfg["data"]["microbatch_sz"]
+
     vpp = cfg["parallelism"]["vpp"]
-    bs_per_dp = safe_divide(gbs, model_def.parallelism_cfg.dp)
-    n_microbatches = safe_divide(bs_per_dp, mbs)
-    print(f"gbs = {gbs}")
-    print(f"gbs/pipeline = {bs_per_dp}")
+    bs_per_mp_rank = safe_divide(gbs, model_repr.parallelism_cfg.dp)
+    n_microbatches_per_mp_rank = safe_divide(bs_per_mp_rank, mbs)
+
     print(f"VPP pipeline bubble multiplier = {(1 / vpp):.2f}")
     print(
-        f"pipeline bubble fraction = {(1 / vpp) * (model_def.parallelism_cfg.pp - 1) / n_microbatches:.2f}"
+        f"pipeline bubble fraction = {(1 / vpp) * (model_repr.parallelism_cfg.pp - 1) / n_microbatches_per_mp_rank:.2f}"
     )
 
     print_section_header("DP COMMUNICATION")
-    if model_def.parallelism_cfg.zero_level != ParallelConfig.ZeroLevel.PARTITION_OPTIMIZER:
+    if model_repr.parallelism_cfg.zero_level != ParallelConfig.ZeroLevel.PARTITION_OPTIMIZER:
         raise NotImplementedError
     else:
         ###############################################################################
         # compute the backward time for a single microbatch.
         ###############################################################################
         # NOTE: this is fully sequential, there's no other microbatches to overlap with
         single_microbatch_bwd_flops = (
             2  # FLOPs/MAC
             * 2  # factor for backward only (2 GEMMs per op)
-            * model_def.microbatch_sz
-            * model_def.sequence_len
-            * model_def.get_total_n_params(partitioned=True)
+            * model_repr.microbatch_sz
+            * model_repr.sequence_len
+            * model_repr.get_total_n_params(partitioned=True)
         )
 
         # divide by single pipeline stage TFLOPs, since its just for single
         # microbatch there's only one active pipeline stage at a time
         single_microbatch_bwd_time = single_microbatch_bwd_flops / machine_spec.total_flops()
         print(
             f"single MP rank, single microbatch bwd compute time {single_microbatch_bwd_time:.2f} s (if 100% FLOPs utilization)"
@@ -198,48 +212,54 @@
         print()
 
         ###############################################################################
         # DP comm times
         ###############################################################################
         # grads are reduced in full-precision
         # params are all-gathered in half-precision
-        mp_params_size = model_def.states.params_shard.size(partitioned=True)
+        mp_params_size = model_repr.states.params_shard.size(partitioned=True)
         # TODO. precisions here assume we are doing AMP
-        grad_bucket_size = model_def.grad_bucket_size()
-        param_bucket_size = model_def.param_bucket_size()
+        grad_bucket_size = model_repr.grad_bucket_size()
+        param_bucket_size = model_repr.param_bucket_size()
+        # full BW should be divided along all MP ranks within a single node, since
+        # they are each participating in their own DP collectives. We make the
+        # assumption here that TP is the only form of MP we do within node.
+        mp_degree_in_node = model_repr.parallelism_cfg.tp
         grad_bucket_reduce_scatter_time_s = get_dp_reduce_scatter_comm_time_s(
             size=grad_bucket_size,
-            n_participants=model_def.parallelism_cfg.dp,
+            n_participants=model_repr.parallelism_cfg.dp,
+            mp_degree_in_node=mp_degree_in_node,
             machine_spec=machine_spec,
         )
-        print(f"reduce_scatter(grad_bucket) time = {grad_bucket_reduce_scatter_time_s:.2f}s")
+        print(f"reduce_scatter(grad_bucket) time = {grad_bucket_reduce_scatter_time_s:.3f}s")
         param_bucket_all_gather_time_s = get_dp_all_gather_comm_time_s(
             size=param_bucket_size,
-            n_participants=model_def.parallelism_cfg.dp,
+            n_participants=model_repr.parallelism_cfg.dp,
+            mp_degree_in_node=mp_degree_in_node,
             machine_spec=machine_spec,
         )
-        print(f"all_gather(param_bucket) time = {param_bucket_all_gather_time_s:.2f}s")
+        print(f"all_gather(param_bucket) time = {param_bucket_all_gather_time_s:.3f}s")
         print()
 
         n_grad_buckets = int(math.ceil(mp_params_size.numel() / grad_bucket_size.numel()))
         n_param_buckets = int(math.ceil(mp_params_size.numel() / param_bucket_size.numel()))
         print(f"reduce_scatter n_buckets = {n_grad_buckets}")
         print(f"all_gather n_buckets = {n_param_buckets}")
         print()
 
         print(
-            f"reduce_scatter(all_grads) time = {grad_bucket_reduce_scatter_time_s * n_grad_buckets:.2f}s"
+            f"reduce_scatter(all_grads) time = {grad_bucket_reduce_scatter_time_s * n_grad_buckets:.3f}s"
         )
         print(
-            f"all_gather(all_params) time = {param_bucket_all_gather_time_s * n_param_buckets:.2f}s"
+            f"all_gather(all_params) time = {param_bucket_all_gather_time_s * n_param_buckets:.3f}s"
         )
 
     print_section_header("WEAK SCALING")
-    full_dp_comm_vol_factor = (model_def.parallelism_cfg.dp - 1) / model_def.parallelism_cfg.dp
-    for dp in range(1, min(model_def.parallelism_cfg.dp, 8) + 1):
+    full_dp_comm_vol_factor = (model_repr.parallelism_cfg.dp - 1) / model_repr.parallelism_cfg.dp
+    for dp in range(1, min(model_repr.parallelism_cfg.dp, 8) + 1):
         factor = (dp - 1) / dp
         print(f"DP={dp} -> {(factor / full_dp_comm_vol_factor) * 100:.2f}% scaling degradation")
     print("...")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dlcalc-0.1.2/dlcalc.egg-info/PKG-INFO` & `dlcalc-0.1.3/dlcalc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: dlcalc
-Version: 0.1.2
+Version: 0.1.3
 Author-email: Justin Chiu <jfc4050@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: PyYAML>=6.0.1
 Provides-Extra: dev
 Requires-Dist: mypy>=1.10.0; extra == "dev"
 Requires-Dist: ruff>=0.4.3; extra == "dev"
 
 # dlcalc
+[![PyPI version](https://badge.fury.io/py/dlcalc.svg)](https://badge.fury.io/py/dlcalc)
 ![checks](https://github.com/jfc4050/dlcalc/actions/workflows/python-app.yml/badge.svg)
 
 random command line tools for deep learning
 
-install CLI
+## Installation
 ```bash
+pip install dlcalc
+```
+
+or
+
+```bash
+git clone https://github.com/jfc4050/dlcalc
+cd dlcalc
 pip install -e .
 ```
 
 ## Tools
 ### 3D Training Calculator
 calculator for estimating various performance characteristics of 3D parallel
 transformer model training:
```

### Comparing `dlcalc-0.1.2/pyproject.toml` & `dlcalc-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dlcalc"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Justin Chiu", email = "jfc4050@gmail.com"}
 ]
 requires-python = ">=3.9"
 dependencies = [
     "PyYAML>=6.0.1"
 ]
```

