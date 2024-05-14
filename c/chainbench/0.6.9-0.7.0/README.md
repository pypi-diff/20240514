# Comparing `tmp/chainbench-0.6.9.tar.gz` & `tmp/chainbench-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.6.9.tar", max compression
+gzip compressed data, was "chainbench-0.7.0.tar", max compression
```

## Comparing `chainbench-0.6.9.tar` & `chainbench-0.7.0.tar`

### file list

```diff
@@ -1,62 +1,59 @@
--rw-r--r--   0        0        0    11357 2024-05-03 10:41:50.862102 chainbench-0.6.9/LICENSE
--rw-r--r--   0        0        0    12165 2024-05-03 10:41:50.862102 chainbench-0.6.9/README.md
--rw-r--r--   0        0        0        0 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/__main__.py
--rw-r--r--   0        0        0    15103 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/main.py
--rw-r--r--   0        0        0        0 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     1607 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/arbitrum/general.py
--rw-r--r--   0        0        0     1392 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/avalanche/archive.py
--rw-r--r--   0        0        0     1481 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     1268 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/base/archive.py
--rw-r--r--   0        0        0     1570 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/base/general.py
--rw-r--r--   0        0        0     2760 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     1158 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/ethereum/consensus.py
--rw-r--r--   0        0        0     2776 2024-05-03 10:41:50.862102 chainbench-0.6.9/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      344 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/all.py
--rw-r--r--   0        0        0     1272 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/debug_trace.py
--rw-r--r--   0        0        0      427 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0     4252 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0     1655 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0     1005 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/fantom/archive.py
--rw-r--r--   0        0        0     1245 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/fantom/general.py
--rw-r--r--   0        0        0     1931 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0     1183 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/optimism/archive.py
--rw-r--r--   0        0        0     1523 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/optimism/general.py
--rw-r--r--   0        0        0     2897 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0     1121 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/ronin/general.py
--rw-r--r--   0        0        0      366 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/solana/all.py
--rw-r--r--   0        0        0     1415 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/solana/general.py
--rw-r--r--   0        0        0     2223 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/profile/starknet/wallet.py
--rw-r--r--   0        0        0      599 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     6482 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/blockchain.py
--rw-r--r--   0        0        0     5934 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/ethereum.py
--rw-r--r--   0        0        0    18785 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/evm.py
--rw-r--r--   0        0        0     6037 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/solana.py
--rw-r--r--   0        0        0     2284 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/test_data/starknet.py
--rw-r--r--   0        0        0       24 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/__init__.py
--rw-r--r--   0        0        0       18 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/discovery/__init__.py
--rw-r--r--   0        0        0      977 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/discovery/clients.json
--rw-r--r--   0        0        0    55080 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/discovery/methods.json
--rw-r--r--   0        0        0     5499 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/tools/discovery/rpc.py
--rw-r--r--   0        0        0      416 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/__init__.py
--rw-r--r--   0        0        0     2895 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/ethereum.py
--rw-r--r--   0        0        0     4622 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/evm.py
--rw-r--r--   0        0        0     5252 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/http.py
--rw-r--r--   0        0        0      889 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/__init__.py
--rw-r--r--   0        0        0      516 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/common.py
--rw-r--r--   0        0        0     9082 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/ethereum.py
--rw-r--r--   0        0        0    10278 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/evm.py
--rw-r--r--   0        0        0     9421 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/methods/solana.py
--rw-r--r--   0        0        0     7242 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/solana.py
--rw-r--r--   0        0        0     3680 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/user/starknet.py
--rw-r--r--   0        0        0        0 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/__init__.py
--rw-r--r--   0        0        0     6218 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/cli.py
--rw-r--r--   0        0        0    12953 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/event.py
--rw-r--r--   0        0        0     6347 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/http.py
--rw-r--r--   0        0        0     2419 2024-05-03 10:41:50.866102 chainbench-0.6.9/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3453 2024-05-03 10:41:50.870102 chainbench-0.6.9/chainbench/util/notify.py
--rw-r--r--   0        0        0      870 2024-05-03 10:41:50.870102 chainbench-0.6.9/chainbench/util/rng.py
--rw-r--r--   0        0        0      337 2024-05-03 10:41:50.870102 chainbench-0.6.9/chainbench/util/rpc.py
--rw-r--r--   0        0        0      455 2024-05-03 10:41:50.870102 chainbench-0.6.9/chainbench/util/timer.py
--rw-r--r--   0        0        0      991 2024-05-03 10:41:50.870102 chainbench-0.6.9/pyproject.toml
--rw-r--r--   0        0        0    12837 1970-01-01 00:00:00.000000 chainbench-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 15:20:25.775396 chainbench-0.7.0/LICENSE
+-rw-r--r--   0        0        0    12382 2024-05-14 15:20:25.775396 chainbench-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/__main__.py
+-rw-r--r--   0        0        0    15901 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/main.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     1277 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/arbitrum/general.py
+-rw-r--r--   0        0        0     1110 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/avalanche/archive.py
+-rw-r--r--   0        0        0     1175 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     1010 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/base/archive.py
+-rw-r--r--   0        0        0     1240 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/base/general.py
+-rw-r--r--   0        0        0      846 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     1212 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/ethereum/consensus.py
+-rw-r--r--   0        0        0      935 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      425 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/all.py
+-rw-r--r--   0        0        0      903 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/debug_trace.py
+-rw-r--r--   0        0        0      281 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0      807 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0      532 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0      807 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/fantom/archive.py
+-rw-r--r--   0        0        0      987 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/fantom/general.py
+-rw-r--r--   0        0        0     2012 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0      949 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/optimism/archive.py
+-rw-r--r--   0        0        0     1205 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/optimism/general.py
+-rw-r--r--   0        0        0      998 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0      899 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/ronin/general.py
+-rw-r--r--   0        0        0      452 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/solana/all.py
+-rw-r--r--   0        0        0     1204 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/solana/general.py
+-rw-r--r--   0        0        0     2223 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/starknet/wallet.py
+-rw-r--r--   0        0        0      599 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     6484 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/blockchain.py
+-rw-r--r--   0        0        0     5934 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/ethereum.py
+-rw-r--r--   0        0        0    19240 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0     6037 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/solana.py
+-rw-r--r--   0        0        0     2284 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/starknet.py
+-rw-r--r--   0        0        0       24 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/discovery/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/discovery/clients.json
+-rw-r--r--   0        0        0    55080 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/discovery/methods.json
+-rw-r--r--   0        0        0     5499 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/discovery/rpc.py
+-rw-r--r--   0        0        0      497 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     1459 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/common.py
+-rw-r--r--   0        0        0    10599 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/http.py
+-rw-r--r--   0        0        0      216 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/__init__.py
+-rw-r--r--   0        0        0    11937 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/ethereum.py
+-rw-r--r--   0        0        0    21316 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/evm.py
+-rw-r--r--   0        0        0    22218 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/solana.py
+-rw-r--r--   0        0        0     3694 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/starknet.py
+-rw-r--r--   0        0        0      573 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/tag.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     6480 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/cli.py
+-rw-r--r--   0        0        0    13147 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/event.py
+-rw-r--r--   0        0        0     6347 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/http.py
+-rw-r--r--   0        0        0     2419 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3453 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/notify.py
+-rw-r--r--   0        0        0      870 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/rng.py
+-rw-r--r--   0        0        0      455 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/timer.py
+-rw-r--r--   0        0        0      991 2024-05-14 15:20:25.783396 chainbench-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    13054 1970-01-01 00:00:00.000000 chainbench-0.7.0/PKG-INFO
```

### Comparing `chainbench-0.6.9/LICENSE` & `chainbench-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/README.md` & `chainbench-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 - `--headless`: Runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
 - `--autoquit`: Tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
 - `--help`: Displays the help message.
 - `--debug-trace-methods`: Enables tasks tagged with debug or trace to be executed
 - `-E, --exclude-tags`: Exclude tasks tagged with custom tags from the test. You may specify this option multiple times.
 - `--use-latest-blocks`: Use latest blocks for test data generation and runs a background process to update the test data with latest blocks.
 - `--size`: Specifies the test data size. Available values are XS, S, M, L, XL. Default is S.
+- '--batch': Runs the test using batch requests. This will send multiple requests in a single batch request. The number of requests in a batch can be specified using the `--batch-size` flag. Default batch size is 10.
 
 You may also run `chainbench start --help` for the full list of parameters and flags.
 
 ### Profiles
 Default profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
 
 You may use the following command to list all profiles available out of the box:
```

### Comparing `chainbench-0.6.9/chainbench/main.py` & `chainbench-0.7.0/chainbench/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 from multiprocessing import Process
 from pathlib import Path
 
 import click
 import gevent.pool
 from click import Context, Parameter
 
-from chainbench.user.methods import (
-    all_method_classes,
-    all_methods,
-    get_subclass_functions,
-)
+from chainbench.user import get_subclass_tasks
+from chainbench.user.common import all_method_classes, all_methods
 from chainbench.util.cli import (
     ContextData,
     LocustOptions,
     ensure_results_dir,
     get_base_path,
     get_profile_path,
     get_profiles,
@@ -148,14 +145,25 @@
     default=[],
     help="Add a monitor to collect additional data or metrics. "
     "You may specify this option multiple times for different monitors",
     type=click.Choice(["head-lag-monitor"], case_sensitive=False),
     multiple=True,
 )
 @click.option(
+    "--batch",
+    is_flag=True,
+    help="Run tests in batch mode. This will make requests in batches for json-rpc methods. The number of requests in "
+    "a batch can be specified using the `--batch-size` flag",
+)
+@click.option(
+    "--batch-size",
+    default=10,
+    help="The number of requests in " "a batch for json-rpc methods. This flag is only used when `--batch` flag is set",
+)
+@click.option(
     "--debug-trace-methods",
     is_flag=True,
     help="Enable tasks tagged with debug or trace to be executed",
 )
 @click.option(
     "-E",
     "--exclude-tags",
@@ -190,14 +198,16 @@
     results_dir: Path,
     headless: bool,
     autoquit: bool,
     target: str | None,
     run_id: str | None,
     notify: str | None,
     monitor: list[str],
+    batch: bool,
+    batch_size: int,
     debug_trace_methods: bool,
     exclude_tags: list[str],
     timescale: bool,
     pg_host: str | None,
     pg_port: int,
     pg_username: str,
     pg_password: str | None,
@@ -290,39 +300,52 @@
 
     custom_exclude_tags: list[str] = []
     if exclude_tags:
         for tag in exclude_tags:
             custom_exclude_tags.append(tag)
 
     if not debug_trace_methods:
-        custom_exclude_tags = custom_exclude_tags + ["trace", "debug"]
+        custom_exclude_tags.extend(["trace", "debug"])
+
+    custom_tags: list[str] = []
+
+    if batch:
+        custom_tags = ["batch_single" if method else "batch"]
+    else:
+        if method:
+            custom_tags.append("single")
+        else:
+            custom_exclude_tags.append("single")
+        custom_exclude_tags.extend(["batch", "batch_single"])
 
     locust_options = LocustOptions(
         profile_path=profile_path,
         host=host,
         port=port,
         test_time=test_time,
         users=users,
         spawn_rate=spawn_rate,
         log_level=log_level,
         results_path=results_path,
         workers=workers,
         headless=headless,
         target=target,
+        custom_tags=custom_tags,
         exclude_tags=custom_exclude_tags,
         timescale=timescale,
         pg_host=pg_host,
         pg_port=pg_port,
         pg_username=pg_username,
         pg_password=pg_password,
         override_plan_name=test_plan,
         use_latest_blocks=use_latest_blocks,
         size=size,
         method=method,
         enable_class_picker=enable_class_picker,
+        batch_size=batch_size,
     )
     # Start the Locust master
     master_command = locust_options.get_master_command()
 
     if headless:
         click.echo("Starting master in headless mode")
     else:
@@ -459,14 +482,14 @@
 
 @_list.command(
     help="Lists all available methods.",
 )
 def methods() -> None:
     for method_class in all_method_classes:
         click.echo(f"\nMethods for {method_class.__name__}:")
-        task_list = get_subclass_functions(method_class)
+        task_list = get_subclass_tasks(method_class)
         for task in task_list:
             click.echo(f"- {method_class.task_to_method(task.name)}")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `chainbench-0.6.9/chainbench/profile/arbitrum/general.py` & `chainbench-0.7.0/chainbench/profile/base/general.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
-Arbitrum profile.
+Base profile.
+```
 """
 
 from locust import constant_pacing
 
-from chainbench.user.http import assign_tasks
-from chainbench.user.methods import EvmMethods
+from chainbench.user.protocol.evm import EvmUser
 
 
-class ArbitrumProfile(EvmMethods):
+class BaseProfile(EvmUser):
     wait_time = constant_pacing(1)
-    tasks = assign_tasks(
-        {
-            EvmMethods.eth_call_task: 1007,
-            EvmMethods.eth_get_block_by_number_task: 592,
-            EvmMethods.eth_get_logs_task: 397,
-            EvmMethods.eth_chain_id_task: 186,
-            EvmMethods.eth_get_transaction_receipt_task: 168,
-            EvmMethods.eth_block_number_task: 165,
-            EvmMethods.eth_get_block_by_hash_task: 61,
-            EvmMethods.eth_get_balance_task: 50,
-            EvmMethods.debug_trace_transaction_task: 48,
-            EvmMethods.eth_estimate_gas_task: 28,
-            EvmMethods.eth_gas_price_task: 22,
-            EvmMethods.eth_get_transaction_count_task: 17,
-            EvmMethods.eth_get_transaction_by_hash_task: 14,
-            EvmMethods.eth_get_block_receipts_task: 12,
-            EvmMethods.debug_trace_block_by_number_task: 12,
-            EvmMethods.eth_get_code_task: 7,
-            EvmMethods.eth_max_priority_fee_per_gas_task: 5,
-            EvmMethods.web3_client_version_task: 3,
-            EvmMethods.debug_trace_block_by_hash_task: 3,
-            EvmMethods.net_listening_task: 2,
-            EvmMethods.net_version_task: 2,
-            EvmMethods.eth_syncing_task: 1,
-            EvmMethods.eth_fee_history_task: 1,
-            EvmMethods.eth_get_transaction_by_block_hash_and_index_task: 1,
-            EvmMethods.debug_trace_call_task: 1,
-        }
-    )
+    rpc_calls = {
+        EvmUser.eth_call: 1051,
+        EvmUser.eth_get_transaction_receipt: 967,
+        EvmUser.eth_get_block_by_number: 375,
+        EvmUser.eth_get_logs: 158,
+        EvmUser.eth_chain_id: 150,
+        EvmUser.debug_trace_transaction: 116,
+        EvmUser.eth_block_number: 114,
+        EvmUser.eth_get_block_receipts: 63,
+        EvmUser.eth_get_balance: 57,
+        EvmUser.eth_get_block_by_hash: 41,
+        EvmUser.trace_block: 28,
+        EvmUser.web3_client_version: 21,
+        EvmUser.eth_get_transaction_count: 15,
+        EvmUser.eth_get_code: 9,
+        EvmUser.eth_get_transaction_by_hash: 9,
+        EvmUser.debug_trace_block_by_hash: 8,
+        EvmUser.eth_gas_price: 6,
+        EvmUser.eth_estimate_gas: 2,
+        EvmUser.debug_trace_block_by_number: 2,
+        EvmUser.eth_syncing: 1,
+        EvmUser.eth_fee_history: 1,
+        EvmUser.eth_max_priority_fee_per_gas: 1,
+        EvmUser.net_version: 1,
+        EvmUser.debug_trace_call: 1,
+        EvmUser.net_listening: 1,
+    }
+
+    tasks = EvmUser.expand_tasks(rpc_calls)
```

### Comparing `chainbench-0.6.9/chainbench/profile/ethereum/consensus.py` & `chainbench-0.7.0/chainbench/profile/ethereum/consensus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 Ethereum Beacon profile.
 """
 
 from locust import constant_pacing
 
-from chainbench.user.methods.ethereum import EthBeaconMethods
+from chainbench.user.protocol.ethereum import EthBeaconUser
 
 # mypy: ignore_errors
 
 
-class EthereumBeaconProfile(EthBeaconMethods):
+class EthereumBeaconProfile(EthBeaconUser):
     wait_time = constant_pacing(1)
-    tasks = {
-        EthBeaconMethods.eth_v1_beacon_states_validators_random_ids_task: 698,
-        EthBeaconMethods.eth_v1_beacon_states_validators_head_task: 23,
-        EthBeaconMethods.eth_v1_beacon_states_head_committees_random_epoch_task: 10,
-        EthBeaconMethods.eth_v1_beacon_states_validators_random_status_task: 10,
-        EthBeaconMethods.eth_v1_beacon_states_random_state_id_finality_checkpoints_task: 10,
-        EthBeaconMethods.eth_v2_beacon_blocks_random_block_id_task: 8,
-        EthBeaconMethods.eth_v2_beacon_blocks_head_task: 6,
-        EthBeaconMethods.eth_v1_beacon_headers_head_task: 4,
-        EthBeaconMethods.eth_v1_config_spec_task: 3,
-        EthBeaconMethods.eth_v1_node_health_task: 2,
-        EthBeaconMethods.eth_v2_beacon_blocks_finalized_task: 1,
-        EthBeaconMethods.eth_v1_beacon_headers_random_block_id_task: 1,
-        EthBeaconMethods.eth_v1_node_version_task: 1,
-    }
+    tasks = EthBeaconUser.expand_tasks(
+        {
+            EthBeaconUser.eth_v1_beacon_states_validators_random_ids_task: 698,
+            EthBeaconUser.eth_v1_beacon_states_validators_head_task: 23,
+            EthBeaconUser.eth_v1_beacon_states_head_committees_random_epoch_task: 10,
+            EthBeaconUser.eth_v1_beacon_states_validators_random_status_task: 10,
+            EthBeaconUser.eth_v1_beacon_states_random_state_id_finality_checkpoints_task: 10,
+            EthBeaconUser.eth_v2_beacon_blocks_random_block_id_task: 8,
+            EthBeaconUser.eth_v2_beacon_blocks_head_task: 6,
+            EthBeaconUser.eth_v1_beacon_headers_head_task: 4,
+            EthBeaconUser.eth_v1_config_spec_task: 3,
+            EthBeaconUser.eth_v1_node_health_task: 2,
+            EthBeaconUser.eth_v2_beacon_blocks_finalized_task: 1,
+            EthBeaconUser.eth_v1_beacon_headers_random_block_id_task: 1,
+            EthBeaconUser.eth_v1_node_version_task: 1,
+        }
+    )
```

### Comparing `chainbench-0.6.9/chainbench/profile/ethereum/general.py` & `chainbench-0.7.0/chainbench/profile/starknet/wallet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,111 +1,83 @@
 """
-Ethereum profile.
+StarkNet profile.
 
 Chart:
 ```mermaid
 %%{init: {'theme':'forest'}}%%
 pie title Methods Distribution
-    "eth_call" : 100
-    "eth_getTransactionReceipt" : 24
-    "eth_blockNumber" : 19
-    "eth_getBalance" : 12
-    "eth_chainId" : 11
-    "eth_getBlockByNumber" : 9
-    "eth_getTransactionByHash" : 8
-    "Others" : 12
+    "starknet_call" : 54
+    "starket_chainId" : 25
+    "starknet_getClassHashAt" : 17
+    "starknet_getTransactionReceipt" : 3
+    "Others" : 1
 ```
 """
 
-from locust import constant_pacing, tag, task
+from locust import constant_pacing, task
 
-from chainbench.user import EvmUser
+from chainbench.user import StarkNetUser
 from chainbench.util.rng import get_rng
 
 
-class EthereumProfile(EvmUser):
+class StarkNetWalletProfile(StarkNetUser):
     wait_time = constant_pacing(1)
-    weight = 487
 
-    @task(100)
+    @task(435)
     def call_task(self):
-        self.make_rpc_call(
-            name="call",
-            method="eth_call",
-            params=self._erc20_eth_call_params_factory(get_rng()),
-        ),
-
-    @task(24)
-    def get_transaction_receipt_task(self):
-        self.make_rpc_call(
-            name="get_transaction_receipt",
-            method="eth_getTransactionReceipt",
-            params=self._transaction_by_hash_params_factory(get_rng()),
-        ),
-
-    @task(19)
-    def block_number_task(self):
-        self.make_rpc_call(
-            name="block_number",
-            method="eth_blockNumber",
-        ),
+        self.make_rpc_call(name="call", method="starknet_call", params=self._call_params_factory(get_rng())),
 
-    @task(12)
-    def get_balance_task(self):
+    @task(200)
+    def chain_id_task(self):
         self.make_rpc_call(
-            name="get_balance",
-            method="eth_getBalance",
-            params=self._get_account_and_block_number_params_factory_latest(get_rng()),
+            name="chain_id",
+            method="starknet_chainId",
         ),
 
-    @task(11)
-    def chain_id_task(self):
+    @task(133)
+    def get_class_hash_at_task(self):
         self.make_rpc_call(
-            name="chain_id",
-            method="eth_chainId",
+            name="get_class_hash_at",
+            method="starknet_getClassHashAt",
+            params=self._get_class_params_factory(get_rng()),
         ),
 
-    @task(9)
-    def get_block_by_number_task(self):
+    @task(21)
+    def get_transaction_receipt_task(self):
         self.make_rpc_call(
-            name="get_block_by_number",
-            method="eth_getBlockByNumber",
-            params=self._block_params_factory(),
+            name="get_transaction_receipt",
+            method="starknet_getTransactionReceipt",
+            params=self._get_tx_hash_params_factory(get_rng()),
         ),
 
-    @task(8)
-    def get_transaction_by_hash_task(self):
+    @task(3)
+    def get_class_at_task(self):
         self.make_rpc_call(
-            name="get_transaction_by_hash",
-            method="eth_getTransactionByHash",
-            params=self._transaction_by_hash_params_factory(get_rng()),
+            name="get_class_at",
+            method="starknet_getClassAt",
+            params=self._get_class_params_factory(get_rng()),
         ),
 
-    @tag("debug")
     @task(3)
-    def trace_transaction_task(self):
+    def get_nonce_task(self):
         self.make_rpc_call(
-            name="trace_transaction",
-            method="debug_traceTransaction",
-            params=self._transaction_by_hash_params_factory(get_rng()),
+            name="get_nonce",
+            method="starknet_getNonce",
+            params=["latest", self._get_contract_address(get_rng())],
         ),
 
     @task(2)
-    def client_version_task(self):
+    def simulate_transaction_task(self):
         self.make_rpc_call(
-            name="client_version",
-            method="web3_clientVersion",
+            name="simulate_transaction",
+            method="starknet_simulateTransaction",
+            params=self._simulate_transaction_params_factory(get_rng()),
+            path="/rpc/v0.3",
         ),
 
-
-class EthGetLogsProfile(EvmUser):
-    wait_time = constant_pacing(10)
-    weight = 13
-
-    @tag("get-logs")
-    @task
-    def get_logs_task(self):
+    @task(1)
+    def estimate_fee_task(self):
         self.make_rpc_call(
-            name="get_logs",
-            method="eth_getLogs",
-            params=self._get_logs_params_factory(get_rng()),
+            name="estimate_fee",
+            method="starknet_estimateFee",
+            params=self._estimate_fee_params_factory(get_rng()),
         ),
```

### Comparing `chainbench-0.6.9/chainbench/profile/evm/light.py` & `chainbench-0.7.0/chainbench/profile/oasis/general.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,72 @@
-"""
-EVM profile (light mode).
-"""
-
 from locust import constant_pacing, task
 
 from chainbench.user import EvmUser
 from chainbench.util.rng import get_rng
 
+# TODO: Update Oasis profile to new format and update tutorial in documentation
 
-class EvmLightProfile(EvmUser):
-    wait_time = constant_pacing(1)
 
-    @task
-    def get_transaction_receipt_task(self):
-        self.make_rpc_call(
-            name="get_transaction_receipt",
-            method="eth_getTransactionReceipt",
-            params=self._transaction_by_hash_params_factory(get_rng()),
-        ),
+class OasisProfile(EvmUser):
+    wait_time = constant_pacing(1)
 
     @task
-    def block_number_task(self):
+    def get_block_by_number_task(self):
         self.make_rpc_call(
-            name="block_number",
-            method="eth_blockNumber",
+            name="get_block_by_number",
+            method="eth_getBlockByNumber",
+            params=self._block_params_factory(),
         ),
 
     @task
     def get_balance_task(self):
         self.make_rpc_call(
             name="get_balance",
             method="eth_getBalance",
-            params=self._get_account_and_block_number_params_factory_latest(get_rng()),
+            params=self._get_balance_params_factory(get_rng()),
         ),
 
     @task
-    def chain_id_task(self):
+    def get_transaction_count_task(self):
         self.make_rpc_call(
-            name="chain_id",
-            method="eth_chainId",
+            name="get_transaction_count",
+            method="eth_getTransactionCount",
+            params=self._get_balance_params_factory(get_rng()),
         ),
 
     @task
-    def get_block_by_number_task(self):
+    def get_code_task(self):
         self.make_rpc_call(
-            name="get_block_by_number",
-            method="eth_getBlockByNumber",
-            params=self._block_params_factory(),
+            name="get_code",
+            method="eth_getCode",
+            params=self._get_balance_params_factory(get_rng()),
         ),
 
     @task
     def get_transaction_by_hash_task(self):
         self.make_rpc_call(
             name="get_transaction_by_hash",
             method="eth_getTransactionByHash",
             params=self._transaction_by_hash_params_factory(get_rng()),
         ),
 
     @task
-    def client_version_task(self):
+    def get_block_number_task(self):
+        self.make_rpc_call(
+            name="block_number",
+            method="eth_blockNumber",
+        ),
+
+    @task
+    def get_syncing_task(self):
+        self.make_rpc_call(
+            name="get_syncing",
+            method="eth_syncing",
+        ),
+
+    @task
+    def get_block_transaction_count_by_number_task(self):
         self.make_rpc_call(
-            name="client_version",
-            method="web3_clientVersion",
+            name="get_block_transaction_count_by_number",
+            method="eth_getBlockTransactionCountByNumber",
+            params=self._random_block_number_params_factory(get_rng()),
         ),
```

### Comparing `chainbench-0.6.9/chainbench/test_data/__init__.py` & `chainbench-0.7.0/chainbench/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/test_data/blockchain.py` & `chainbench-0.7.0/chainbench/test_data/blockchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from chainbench.util.http import HttpClient
 from chainbench.util.rng import RNG, get_rng
 
 logger = logging.getLogger(__name__)
 
 Account = str
 TxHash = str
-Tx = dict[str, t.Any]
+Tx = t.Dict[str, t.Any]
 BlockNumber = int
 BlockHash = str
 
 
 def parse_hex_to_int(value: str) -> int:
     return int(value, 16)
```

### Comparing `chainbench-0.6.9/chainbench/test_data/ethereum.py` & `chainbench-0.7.0/chainbench/test_data/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/test_data/evm.py` & `chainbench-0.7.0/chainbench/test_data/evm.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,14 +332,25 @@
                 "0x3c4e17b9056272ce1b49f6900d8cfd6171a1869d",
                 "0x29c6f8349a028e1bdfc68bfa08bdee7bc5d47e16",
                 "0xa959726154953bae111746e265e6d754f48570e6",
                 "0x04ef1d4f687bb20eedcf05c7f710c078ba39f328",
                 "0x067fbff8990c58ab90bae3c97241c5d736053f77",
             ],
         },
+        324: {
+            "name": "zksync-mainnet",
+            "start_block": 1,
+            "contract_addresses": [
+                "0x000000000000000000000000000000000000800A",
+                "0x96e4069B746bD88Db76eE126acfDA537DdcEe6FF",
+                "0x1d17CBcF0D6D143135aE902365D2E5e2A16538D4",
+                "0x4E14EC08875c88f9B0Cf2A075F481EDa0143d1f0",
+                "0x5B09802d62d213c4503B4b1Ef5F727ef62c9F4eF",
+            ],
+        },
         # TODO: Move StarkNet out of EVMNetwork
         23448594291968334: {
             "name": "starknet-mainnet",
             "start_block": 100000,
             "contract_addresses": [],
         },
     }
```

### Comparing `chainbench-0.6.9/chainbench/test_data/solana.py` & `chainbench-0.7.0/chainbench/test_data/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/test_data/starknet.py` & `chainbench-0.7.0/chainbench/test_data/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/tools/discovery/clients.json` & `chainbench-0.7.0/chainbench/tools/discovery/clients.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/tools/discovery/methods.json` & `chainbench-0.7.0/chainbench/tools/discovery/methods.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/tools/discovery/rpc.py` & `chainbench-0.7.0/chainbench/tools/discovery/rpc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/user/methods/ethereum.py` & `chainbench-0.7.0/chainbench/user/protocol/ethereum.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,117 @@
+import logging
 import typing as t
 
 from locust import task
 
-from chainbench.user.ethereum import EthBeaconUser
+from chainbench.test_data.ethereum import EthBeaconTestData
+from chainbench.user.http import HttpUser
 
+logger = logging.getLogger(__name__)
 
-class EthBeaconMethods(EthBeaconUser):
+
+class EthBeaconBaseUser(HttpUser):
+    abstract = True
+    test_data = EthBeaconTestData()
+
+    def eth_beacon_blocks_request(
+        self,
+        name: str = "eth_beacon_blocks",
+        version: str = "v1",
+        block_id: int | str = "head",
+        path: str | None = None,
+    ):
+        url_path = f"/eth/{version}/beacon/blocks/{block_id}"
+        if path:
+            url_path += "/" + path.strip("/")
+        self.get(
+            name=name,
+            path=url_path,
+        )
+
+    def eth_v1_beacon_states_validators_request(
+        self,
+        name: str = "eth_v1_beacon_states_validators",
+        state_id: int | str = "head",
+        validator_status: str | None = None,
+        validator_ids: list[str] | None = None,
+    ):
+        params: dict[str, t.Any] = {}
+        if validator_status:
+            params = {"status": validator_status}
+        if validator_ids:
+            params = {"id": validator_ids}
+
+        self.get(
+            name=name,
+            path=f"/eth/v1/beacon/states/{state_id}/validators",
+            params=params,
+        )
+
+    def eth_v1_beacon_states_sync_committees_request(
+        self,
+        name: str = "eth_v1_beacon_states_sync_committees",
+        state_id: int | str = "head",
+        epoch: int | None = None,
+    ):
+        params: dict[str, t.Any] = {}
+        if epoch:
+            params = {"epoch": epoch}
+        self.get(
+            name=name,
+            path=f"/eth/v1/beacon/states/{state_id}/sync_committees",
+            params=params,
+        )
+
+    def eth_v1_beacon_headers_request(
+        self,
+        name: str = "eth_v1_beacon_headers",
+        block_id: int | str | None = None,
+        slot: int | None = None,
+        parent_root: str | None = None,
+    ):
+        path = ""
+        if block_id is not None:
+            path = f"/{block_id}"
+        params: dict[str, t.Any] = {}
+        if slot is not None:
+            params["slot"] = slot
+        if parent_root is not None:
+            params["parent_root"] = parent_root
+        self.get(name=name, path="/eth/v1/beacon/headers" + path, params=params)
+
+    def eth_v1_beacon_states_committees_request(
+        self,
+        name: str = "eth_v1_beacon_states_committees",
+        state_id: int | str = "head",
+        epoch: int | None = None,
+        committee_index: int | None = None,
+        slot: int | None = None,
+    ):
+        params: dict[str, t.Any] = {}
+        if epoch is not None:
+            params["epoch"] = epoch
+        if committee_index is not None:
+            params["committee_index"] = committee_index
+        if slot is not None:
+            params["slot"] = slot
+        self.get(name=name, path=f"/eth/v1/beacon/states/{state_id}/committees", params=params)
+
+
+class EthBeaconUser(EthBeaconBaseUser):
     abstract = True
 
     @staticmethod
     def task_to_method(task_name: str) -> str:
         task_name_stripped = task_name.replace("_task", "")
         return f"{task_name_stripped}"
 
-    def method_to_task_function(self, method: str) -> t.Callable:
-        return getattr(self, f"{method}_task")
+    @classmethod
+    def method_to_task_function(cls, method: str) -> t.Callable:
+        return getattr(cls, f"{method}_task")
 
     def eth_v1_beacon_states_head_fork_task(self):
         self.get(
             name="eth_v1_beacon_states_head_fork",
             path="/eth/v1/beacon/states/head/fork",
         )
 
@@ -228,11 +321,11 @@
     def eth_v1_node_version_task(self):
         self.get(
             name="eth_v1_node_version",
             path="/eth/v1/node/version",
         )
 
 
-class TestEthMethod(EthBeaconMethods):
+class TestEthMethod(EthBeaconUser):
     @task
     def run_task(self) -> None:
         self.method_to_task_function(self.environment.parsed_options.method)()
```

### Comparing `chainbench-0.6.9/chainbench/user/starknet.py` & `chainbench-0.7.0/chainbench/user/protocol/starknet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import typing as t
 
 from chainbench.test_data import StarkNetTestData
 from chainbench.test_data.blockchain import Account, TxHash
+from chainbench.user.http import JsonRpcUser
 from chainbench.util.rng import RNG
 
-from .http import JsonRpcUser
-
 
 class StarkNetUser(JsonRpcUser):
     abstract = True
     test_data = StarkNetTestData()
 
     @staticmethod
     def _call_params_factory(rng: RNG) -> dict[str, t.Any]:
```

### Comparing `chainbench-0.6.9/chainbench/util/cli.py` & `chainbench-0.7.0/chainbench/util/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,27 +114,29 @@
     port: int
     users: int
     workers: int
     spawn_rate: int
     test_time: str
     log_level: str
     results_path: Path
+    custom_tags: list[str]
     exclude_tags: list[str]
     target: str
     headless: bool = False
     timescale: bool = False
     pg_host: str | None = None
     pg_port: int | None = None
     pg_username: str | None = None
     pg_password: str | None = None
     override_plan_name: str | None = None
     use_latest_blocks: bool = False
     size: str | None = None
     method: str | None = None
     enable_class_picker: bool = False
+    batch_size: int | None = None
 
     def get_master_command(self) -> str:
         """Generate master command."""
         command = (
             f"locust -f {self.profile_path} --master "
             f"--master-bind-host {self.host} --master-bind-port {self.port} "
             f"--web-host {self.host} "
@@ -173,19 +175,25 @@
 
         if self.headless:
             command += " --headless"
 
         if len(self.exclude_tags) > 0:
             command += f" --exclude-tags {' '.join(self.exclude_tags)}"
 
+        if len(self.custom_tags) > 0:
+            command += f" --tags {' '.join(self.custom_tags)}"
+
         if self.use_latest_blocks:
             command += " --use-latest-blocks True"
 
         if self.method is not None:
             command += f" --method {self.method}"
+
+        if self.batch_size is not None:
+            command += f" --batch-size {self.batch_size}"
         return command
 
 
 @dataclass
 class ContextData:
     workers: list[subprocess.Popen] = field(default_factory=list)
     master: subprocess.Popen | None = None
```

### Comparing `chainbench-0.6.9/chainbench/util/event.py` & `chainbench-0.7.0/chainbench/util/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from locust.env import Environment
 from locust.rpc import Message
 from locust.runners import STATE_CLEANUP, MasterRunner, WorkerRunner
 
 from chainbench.test_data import Block, EvmTestData, TestData
 from chainbench.test_data.blockchain import BlockNotFoundError, InvalidBlockError
 from chainbench.test_data.evm import ChainId
-from chainbench.user.methods import all_methods
+from chainbench.user.common import all_methods
 from chainbench.util.timer import Timer
 
 logger = logging.getLogger(__name__)
 
 
 def cli_custom_arguments(parser: LocustArgumentParser):
     parser.add_argument(
@@ -30,14 +30,21 @@
     parser.add_argument(
         "--size",
         type=str,
         default=None,
         help="Set the size of the test data. e.g. --size S",
         include_in_web_ui=False,
     )
+    parser.add_argument(
+        "--batch-size",
+        type=int,
+        default=10,
+        help="Set the batch size for batch requests. Default is 10.",
+        include_in_web_ui=True,
+    )
 
     # TODO - limit choices to the methods that are available in the selected user class
     parser.add_argument(
         "--method",
         type=str,
         default="eth_blockNumber",
         choices=list(all_methods.keys()),
```

### Comparing `chainbench-0.6.9/chainbench/util/http.py` & `chainbench-0.7.0/chainbench/util/http.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/util/monitor.py` & `chainbench-0.7.0/chainbench/util/monitor.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/util/notify.py` & `chainbench-0.7.0/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/chainbench/util/rng.py` & `chainbench-0.7.0/chainbench/util/rng.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.6.9/pyproject.toml` & `chainbench-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.6.9"
+version = "0.7.0"
 description = ""
 authors = [
     "Egor Molodik <egor.molodik@chainstack.com>",
     "Erwin Wee <erwin.wee@chainstack.com>"
 ]
 maintainers = ["Erwin Wee <erwin.wee@chainstack.com>"]
 readme = "README.md"
```

### Comparing `chainbench-0.6.9/PKG-INFO` & `chainbench-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.6.9
+Version: 0.7.0
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Maintainer: Erwin Wee
 Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -139,14 +139,15 @@
 - `--headless`: Runs the benchmark in headless mode, meaning that no graphical user interface (GUI) will be displayed during the test. This is useful for running the test on a remote server or when the GUI is not needed.
 - `--autoquit`: Tells the Chainbench tool to automatically quit after the test has finished. This is useful for running the benchmark in an automated environment where manual intervention is not desired.
 - `--help`: Displays the help message.
 - `--debug-trace-methods`: Enables tasks tagged with debug or trace to be executed
 - `-E, --exclude-tags`: Exclude tasks tagged with custom tags from the test. You may specify this option multiple times.
 - `--use-latest-blocks`: Use latest blocks for test data generation and runs a background process to update the test data with latest blocks.
 - `--size`: Specifies the test data size. Available values are XS, S, M, L, XL. Default is S.
+- '--batch': Runs the test using batch requests. This will send multiple requests in a single batch request. The number of requests in a batch can be specified using the `--batch-size` flag. Default batch size is 10.
 
 You may also run `chainbench start --help` for the full list of parameters and flags.
 
 ### Profiles
 Default profiles are located in the [`profile`](chainbench/profile) directory. For a tutorial on how to create custom profiles, please refer to [this document](docs/PROFILE.md).
 
 You may use the following command to list all profiles available out of the box:
```

