# Comparing `tmp/interprocesspyobjects-1.0.5.tar.gz` & `tmp/interprocesspyobjects-1.0.6.tar.gz`

## Comparing `interprocesspyobjects-1.0.5.tar` & `interprocesspyobjects-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/ipc_py_objects/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/ipc_py_objects/versions/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/ipc_py_objects/versions/v_0/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/ipc_py_objects/versions/v_1/__init__.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/LICENSE.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/NOTICE
--rw-r--r--   0        0        0    39743 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/README.md
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    44366 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/ipc_py_objects/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/ipc_py_objects/versions/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/ipc_py_objects/versions/v_0/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/ipc_py_objects/versions/v_1/__init__.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/LICENSE.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/NOTICE
+-rw-r--r--   0        0        0    46186 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/README.md
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    50809 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.6/PKG-INFO
```

### Comparing `interprocesspyobjects-1.0.5/ipc_py_objects/__init__.py` & `interprocesspyobjects-1.0.6/ipc_py_objects/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 """
 
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2024 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 __status__ = "Production"
 
 
 from .versions import *
```

### Comparing `interprocesspyobjects-1.0.5/ipc_py_objects/versions/__init__.py` & `interprocesspyobjects-1.0.6/ipc_py_objects/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.5/ipc_py_objects/versions/v_0/__init__.py` & `interprocesspyobjects-1.0.6/ipc_py_objects/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.5/ipc_py_objects/versions/v_1/__init__.py` & `interprocesspyobjects-1.0.6/ipc_py_objects/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.5/.gitignore` & `interprocesspyobjects-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.5/LICENSE.md` & `interprocesspyobjects-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.5/NOTICE` & `interprocesspyobjects-1.0.6/NOTICE`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.5/README.md` & `interprocesspyobjects-1.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 # InterProcessPyObjects package
 
 > InterProcessPyObjects is a part of the [Cengal](https://github.com/FI-Mihej/Cengal) library. If you have any questions or would like to participate in discussions, feel free to join the [Cengal Discord](https://discord.gg/TAy7xNgR). Your support and involvement are greatly appreciated as Cengal evolves.
 
 This high-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency. By minimizing the need for frequent serialization-deserialization, it enhances overall speed and responsiveness. The package offers a comprehensive suite of functionalities designed to support a diverse array of Python types and facilitate asynchronous IPC, optimizing performance for demanding applications.
 
-![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+![Throughput GiB/s](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+
+![Dict performance comparison](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartDictPerformanceComparison.png)
 
 ## API State
 
 Stable. Guaranteed to not have braking changes in the future (see bellow for details).
 
 Any hypothetical further API-breaking changes will lead to new module creation within the package. An old version will continue its existence and continue to be importable by an explicit address (see Details bellow).
 
@@ -691,33 +693,35 @@
 * RAM: 32 GBytes, DDR3, dual channel, 655 MHz
 * OS: Ubuntu 20.04.6 LTS under WSL2. Windows 10
 
 </details>
 
 ### Throughput GiB/s
 
+![Throughput GiB/s](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+
+<details>
+<summary title="Benchmarks results"><kbd> Benchmarks results </kbd></summary>
+
 #### Refference results (sysbench)
 
 ```bash
 sysbench memory --memory-oper=write run
 ```
 
 ```
 5499.28 MiB/sec
 ```
 
 #### Results
 
-![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+![Throughput GiB/s](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
 
 `*` [multiprocessing.shared_memory.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__shared_memory.py) - simple implementation. This is a simple implementation because it uses a similar approach to the one used in `uvloop.*`, `asyncio.*`, `multiprocessing.Queue`, and `multiprocessing.Pipe` benchmarking scripts. Similar implementations are expected to be used by the majority of projects.
 
-<details>
-<summary title="Benchmarks results table"><kbd> Benchmarks results table </kbd></summary>
-
 #### Benchmarks results table
 
 | Approach                        | sync/async | Throughput GiB/s |
 |---------------------------------|------------|------------------|
 | InterProcessPyObjects (sync)    | sync       | 3.770            |
 | InterProcessPyObjects + uvloop  | async      | 3.222            |
 | InterProcessPyObjects + asyncio | async      | 3.079            |
@@ -726,20 +730,14 @@
 | asyncio + cengal.Streams        | async      | 0.942            |
 | uvloop.Streams                  | async      | 0.922            |
 | asyncio.Streams                 | async      | 0.784            |
 | asyncio.UnixDomainSockets       | async      | 0.708            |
 | multiprocessing.Queue           | sync       | 0.669            |
 | multiprocessing.Pipe            | sync       | 0.469            |
 
-</details>
-
-
-<details>
-<summary title="Benchmark scripts"><kbd> Benchmark scripts </kbd></summary>
-
 #### Benchmark scripts
 
 * InterProcessPyObjects - Sync:
     * [sender.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__transfer_sync__sender.py)
     * [receiver.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__transfer_sync__receiver.py)
 * InterProcessPyObjects - Async (uvloop):
     * [sender.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__transfer_uvloop__sender.py)
@@ -754,14 +752,179 @@
 * [asyncio.Streams.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__asyncio_streams.py)
 * [asyncio.UnixDomainSockets.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__asyncio_unix_domain_sockets.py)
 * [multiprocessing.Queue.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__multiprocess_queue.py)
 * [multiprocessing.Pipe.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__multiprocess_pipe.py)
 
 </details>
 
+### Shared Dict Performance
+
+![Dict performance comparison](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartDictPerformanceComparison.png)
+
+<details>
+<summary title="Benchmarks results"><kbd> Benchmarks results </kbd></summary>
+
+#### Competitors
+
+##### multiprocessing.Manager - dict
+
+Pros:
+
+* Part of the standard library
+
+Cons:
+
+* Slowest solution
+* Values are read-only unless they are an explicit instances of `multiprocessing.Manager` supported types (types inherited from `multiprocessing.BaseProxy` like `multiprocessing.DictProxy` or `multiprocessing.ListProxy`)
+
+Benchmark scripts:
+
+* [dict__python__multiprocess_dict.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__python__multiprocess_dict.py)
+
+##### UltraDict
+
+Pros:
+
+* Relatively fast writes
+* Fast repetitive reads of an unchanged values
+* Has built in inter-process synchronization mechanism
+
+Cons:
+
+* Relies on pickle on an each change
+* Non-dictionary values are read-only from the multiprocessing perspective
+
+Benchmark scripts:
+
+* [dict__thirdparty__ultradict.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__thirdparty__ultradict.py)
+
+##### shared_memory_dict
+
+Pros:
+
+* At least faster than 'multiprocessing.Manager - dict' solution
+
+Cons:
+
+* Second slowest solution
+* Relies on pickle on an each change
+* Values (even lists or dicts) are read-only from the multiprocessing perspective
+* Can not be initialized from the other `dict` nor even from the other `SharedMemoryDict` instance: you need to manually put an each key-value pair into it using loop
+* Has known issues with inter-process synchronization. Is is better for developer to use their own external inter-process synchronization mechanisms (from `multiprocessing.Manager` for example)
+
+Benchmark scripts:
+
+* [dict__thirdparty__shared_memory_dict.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__thirdparty__shared_memory_dict.py)
+
+##### InterProcessPyObjects - IntEnumListStruct
+
+Pros:
+
+* Fastest solution: 15.6 times faster than `UltraDict`
+* Good for structures: when all fields are already known
+* Support any InterProcessPyObjects' supported data types as values
+* Values of mutable types are naturally mutable: developer do not need to prepare and change their data explicitly
+
+Cons:
+
+* Can use only IntEnum (int) keys
+* Fixed size of a size of a provided IntEnum
+
+Benchmark scripts:
+
+* [dict__shared_objects__intenum_list.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__shared_objects__intenum_list.py)
+
+Message sender example:
+
+```python
+class CompanyMetrics(IntEnum):
+    income = 0
+    employees = 1
+    avg_salary = 2
+    annual_income = 3
+    in_a_good_state = 4
+    emails = 5
+    websites = 6
+
+company_metrics: List = intenum_dict_to_list({  # lists with IntEnum indexes are blazing-fast alternative to dictionaries
+    CompanyMetrics.websites: ['http://company.com', 'http://company.org'],
+    CompanyMetrics.avg_salary: 3_000.0,
+    CompanyMetrics.employees: 10,
+    CompanyMetrics.in_a_good_state: True,
+})  # Unmentioned fields will be filled with Null values
+company_metrics_mapped: List = shared_memory.value.put_message(company_metrics)
+```
+
+Message receiver example:
+
+```python
+company_metrics: List = shared_memory.value.take_message()
+k = company_metrics[CompanyMetrics.avg_salary]
+company_metrics[CompanyMetrics.avg_salary] = 5_000.0
+company_metrics[CompanyMetrics.avg_salary] += 1.1
+```
+
+##### InterProcessPyObjects - Dataclass
+
+Pros:
+
+* Fast. Second fastest solution: around 2 times faster than `UltraDict`
+* Good for structures and object: when all fields are already known
+* Works with objects naturally - without an explicit preparation or changes from the developer's side
+* Support any InterProcessPyObjects' supported data types as values
+* Supports `dataclass` as well as other objects
+* Supports object's methods
+* Fields of mutable types are naturally mutable: developer do not need to prepare and change their data explicitly
+* Does not relies on frequent data pickle: uses pickle only for an initial object construction but not for the fields updates
+
+Cons:
+
+* Set of fields is fixed by the set of fields of an original object
+
+Benchmark scripts:
+
+* [dict__shared_objects__static_obj.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__shared_objects__static_obj.py)
+
+##### InterProcessPyObjects - Dict
+
+Pros:
+
+* Slightly faster than `SharedMemoryDict`
+* Works with objects naturally - without an explicit preparation or changes from the developer's side
+* Support any InterProcessPyObjects' supported data types as values
+* Support any InterProcessPyObjects' supported Hashable data types as keys
+* Values of mutable types are naturally mutable: developer do not need to prepare and change their data explicitly
+* Does not relies on pickle
+* Speed optimizations are architectures and planned for an implementation
+
+Cons:
+
+* Speed optimization implementation are in progress - not released yet
+
+Benchmark scripts:
+
+* [dict__shared_objects__dict.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__shared_objects__dict.py)
+
+#### Results
+
+![Dict performance comparison](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartDictPerformanceComparison.png)
+
+#### Benchmarks results table
+
+| Approach                                  | increments/s |
+|-------------------------------------------|--------------|
+| InterProcessPyObjects - IntEnumListStruct | 1189730      |
+| InterProcessPyObjects - Dataclass         | 143091       |
+| UltraDict                                 | 76214        |
+| InterProcessPyObjects - Dict              | 44285        |
+| SharedMemoryDict                          | 42862        |
+| multiprocessing.Manager - dict            | 2751         |
+
+</details>
+
 ## Todo
 
 - [ ] Connect more than two processes
 - [ ] Use third-party fast hashing implementations instead of or in addition to built in `hash()` call
 - [ ] Continuous performance improvements
 
 ## Conclusion
```

### Comparing `interprocesspyobjects-1.0.5/pyproject.toml` & `interprocesspyobjects-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.5/PKG-INFO` & `interprocesspyobjects-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: InterProcessPyObjects
-Version: 1.0.5
+Version: 1.0.6
 Summary: This high-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency
 Project-URL: Homepage, https://github.com/FI-Mihej/InterProcessPyObjects
 Author-email: ButenkoMS <gtalk@butenkoms.space>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
 License-File: NOTICE
 Keywords: Android,IPC,Linux,Windows,cengal,crossplatform,iOS,inter-process communication,macOS,multiprocessing,shared dict,shared memory,shared numpy ndarray,shared object,shared objects,shared set,shared torch Tensor
@@ -98,15 +98,17 @@
 
 # InterProcessPyObjects package
 
 > InterProcessPyObjects is a part of the [Cengal](https://github.com/FI-Mihej/Cengal) library. If you have any questions or would like to participate in discussions, feel free to join the [Cengal Discord](https://discord.gg/TAy7xNgR). Your support and involvement are greatly appreciated as Cengal evolves.
 
 This high-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency. By minimizing the need for frequent serialization-deserialization, it enhances overall speed and responsiveness. The package offers a comprehensive suite of functionalities designed to support a diverse array of Python types and facilitate asynchronous IPC, optimizing performance for demanding applications.
 
-![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+![Throughput GiB/s](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+
+![Dict performance comparison](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartDictPerformanceComparison.png)
 
 ## API State
 
 Stable. Guaranteed to not have braking changes in the future (see bellow for details).
 
 Any hypothetical further API-breaking changes will lead to new module creation within the package. An old version will continue its existence and continue to be importable by an explicit address (see Details bellow).
 
@@ -783,33 +785,35 @@
 * RAM: 32 GBytes, DDR3, dual channel, 655 MHz
 * OS: Ubuntu 20.04.6 LTS under WSL2. Windows 10
 
 </details>
 
 ### Throughput GiB/s
 
+![Throughput GiB/s](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+
+<details>
+<summary title="Benchmarks results"><kbd> Benchmarks results </kbd></summary>
+
 #### Refference results (sysbench)
 
 ```bash
 sysbench memory --memory-oper=write run
 ```
 
 ```
 5499.28 MiB/sec
 ```
 
 #### Results
 
-![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
+![Throughput GiB/s](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
 
 `*` [multiprocessing.shared_memory.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__shared_memory.py) - simple implementation. This is a simple implementation because it uses a similar approach to the one used in `uvloop.*`, `asyncio.*`, `multiprocessing.Queue`, and `multiprocessing.Pipe` benchmarking scripts. Similar implementations are expected to be used by the majority of projects.
 
-<details>
-<summary title="Benchmarks results table"><kbd> Benchmarks results table </kbd></summary>
-
 #### Benchmarks results table
 
 | Approach                        | sync/async | Throughput GiB/s |
 |---------------------------------|------------|------------------|
 | InterProcessPyObjects (sync)    | sync       | 3.770            |
 | InterProcessPyObjects + uvloop  | async      | 3.222            |
 | InterProcessPyObjects + asyncio | async      | 3.079            |
@@ -818,20 +822,14 @@
 | asyncio + cengal.Streams        | async      | 0.942            |
 | uvloop.Streams                  | async      | 0.922            |
 | asyncio.Streams                 | async      | 0.784            |
 | asyncio.UnixDomainSockets       | async      | 0.708            |
 | multiprocessing.Queue           | sync       | 0.669            |
 | multiprocessing.Pipe            | sync       | 0.469            |
 
-</details>
-
-
-<details>
-<summary title="Benchmark scripts"><kbd> Benchmark scripts </kbd></summary>
-
 #### Benchmark scripts
 
 * InterProcessPyObjects - Sync:
     * [sender.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__transfer_sync__sender.py)
     * [receiver.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__transfer_sync__receiver.py)
 * InterProcessPyObjects - Async (uvloop):
     * [sender.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/shared_objects__transfer_uvloop__sender.py)
@@ -846,14 +844,179 @@
 * [asyncio.Streams.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__asyncio_streams.py)
 * [asyncio.UnixDomainSockets.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__asyncio_unix_domain_sockets.py)
 * [multiprocessing.Queue.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__multiprocess_queue.py)
 * [multiprocessing.Pipe.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/plain_python__send_bytes__multiprocess_pipe.py)
 
 </details>
 
+### Shared Dict Performance
+
+![Dict performance comparison](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartDictPerformanceComparison.png)
+
+<details>
+<summary title="Benchmarks results"><kbd> Benchmarks results </kbd></summary>
+
+#### Competitors
+
+##### multiprocessing.Manager - dict
+
+Pros:
+
+* Part of the standard library
+
+Cons:
+
+* Slowest solution
+* Values are read-only unless they are an explicit instances of `multiprocessing.Manager` supported types (types inherited from `multiprocessing.BaseProxy` like `multiprocessing.DictProxy` or `multiprocessing.ListProxy`)
+
+Benchmark scripts:
+
+* [dict__python__multiprocess_dict.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__python__multiprocess_dict.py)
+
+##### UltraDict
+
+Pros:
+
+* Relatively fast writes
+* Fast repetitive reads of an unchanged values
+* Has built in inter-process synchronization mechanism
+
+Cons:
+
+* Relies on pickle on an each change
+* Non-dictionary values are read-only from the multiprocessing perspective
+
+Benchmark scripts:
+
+* [dict__thirdparty__ultradict.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__thirdparty__ultradict.py)
+
+##### shared_memory_dict
+
+Pros:
+
+* At least faster than 'multiprocessing.Manager - dict' solution
+
+Cons:
+
+* Second slowest solution
+* Relies on pickle on an each change
+* Values (even lists or dicts) are read-only from the multiprocessing perspective
+* Can not be initialized from the other `dict` nor even from the other `SharedMemoryDict` instance: you need to manually put an each key-value pair into it using loop
+* Has known issues with inter-process synchronization. Is is better for developer to use their own external inter-process synchronization mechanisms (from `multiprocessing.Manager` for example)
+
+Benchmark scripts:
+
+* [dict__thirdparty__shared_memory_dict.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__thirdparty__shared_memory_dict.py)
+
+##### InterProcessPyObjects - IntEnumListStruct
+
+Pros:
+
+* Fastest solution: 15.6 times faster than `UltraDict`
+* Good for structures: when all fields are already known
+* Support any InterProcessPyObjects' supported data types as values
+* Values of mutable types are naturally mutable: developer do not need to prepare and change their data explicitly
+
+Cons:
+
+* Can use only IntEnum (int) keys
+* Fixed size of a size of a provided IntEnum
+
+Benchmark scripts:
+
+* [dict__shared_objects__intenum_list.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__shared_objects__intenum_list.py)
+
+Message sender example:
+
+```python
+class CompanyMetrics(IntEnum):
+    income = 0
+    employees = 1
+    avg_salary = 2
+    annual_income = 3
+    in_a_good_state = 4
+    emails = 5
+    websites = 6
+
+company_metrics: List = intenum_dict_to_list({  # lists with IntEnum indexes are blazing-fast alternative to dictionaries
+    CompanyMetrics.websites: ['http://company.com', 'http://company.org'],
+    CompanyMetrics.avg_salary: 3_000.0,
+    CompanyMetrics.employees: 10,
+    CompanyMetrics.in_a_good_state: True,
+})  # Unmentioned fields will be filled with Null values
+company_metrics_mapped: List = shared_memory.value.put_message(company_metrics)
+```
+
+Message receiver example:
+
+```python
+company_metrics: List = shared_memory.value.take_message()
+k = company_metrics[CompanyMetrics.avg_salary]
+company_metrics[CompanyMetrics.avg_salary] = 5_000.0
+company_metrics[CompanyMetrics.avg_salary] += 1.1
+```
+
+##### InterProcessPyObjects - Dataclass
+
+Pros:
+
+* Fast. Second fastest solution: around 2 times faster than `UltraDict`
+* Good for structures and object: when all fields are already known
+* Works with objects naturally - without an explicit preparation or changes from the developer's side
+* Support any InterProcessPyObjects' supported data types as values
+* Supports `dataclass` as well as other objects
+* Supports object's methods
+* Fields of mutable types are naturally mutable: developer do not need to prepare and change their data explicitly
+* Does not relies on frequent data pickle: uses pickle only for an initial object construction but not for the fields updates
+
+Cons:
+
+* Set of fields is fixed by the set of fields of an original object
+
+Benchmark scripts:
+
+* [dict__shared_objects__static_obj.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__shared_objects__static_obj.py)
+
+##### InterProcessPyObjects - Dict
+
+Pros:
+
+* Slightly faster than `SharedMemoryDict`
+* Works with objects naturally - without an explicit preparation or changes from the developer's side
+* Support any InterProcessPyObjects' supported data types as values
+* Support any InterProcessPyObjects' supported Hashable data types as keys
+* Values of mutable types are naturally mutable: developer do not need to prepare and change their data explicitly
+* Does not relies on pickle
+* Speed optimizations are architectures and planned for an implementation
+
+Cons:
+
+* Speed optimization implementation are in progress - not released yet
+
+Benchmark scripts:
+
+* [dict__shared_objects__dict.py](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/asyncio/ashared_memory_manager/versions/v_0/development/dict__shared_objects__dict.py)
+
+#### Results
+
+![Dict performance comparison](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartDictPerformanceComparison.png)
+
+#### Benchmarks results table
+
+| Approach                                  | increments/s |
+|-------------------------------------------|--------------|
+| InterProcessPyObjects - IntEnumListStruct | 1189730      |
+| InterProcessPyObjects - Dataclass         | 143091       |
+| UltraDict                                 | 76214        |
+| InterProcessPyObjects - Dict              | 44285        |
+| SharedMemoryDict                          | 42862        |
+| multiprocessing.Manager - dict            | 2751         |
+
+</details>
+
 ## Todo
 
 - [ ] Connect more than two processes
 - [ ] Use third-party fast hashing implementations instead of or in addition to built in `hash()` call
 - [ ] Continuous performance improvements
 
 ## Conclusion
```

