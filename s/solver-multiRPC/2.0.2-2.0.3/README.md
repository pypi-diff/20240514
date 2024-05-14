# Comparing `tmp/solver-multiRPC-2.0.2.tar.gz` & `tmp/solver-multiRPC-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver-multiRPC-2.0.2.tar", last modified: Mon Apr 22 08:21:43 2024, max compression
+gzip compressed data, was "solver-multiRPC-2.0.3.tar", last modified: Tue May 14 12:15:44 2024, max compression
```

## Comparing `solver-multiRPC-2.0.2.tar` & `solver-multiRPC-2.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-04-22 08:21:43.767638 solver-multiRPC-2.0.2/
--rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-04-22 08:21:43.767638 solver-multiRPC-2.0.2/PKG-INFO
--rw-rw-r--   0 mba       (1000) mba       (1000)     2955 2024-04-21 14:40:19.000000 solver-multiRPC-2.0.2/README.md
--rw-rw-r--   0 mba       (1000) mba       (1000)      103 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.2/pyproject.toml
--rw-rw-r--   0 mba       (1000) mba       (1000)      582 2024-04-22 08:21:43.767638 solver-multiRPC-2.0.2/setup.cfg
--rw-rw-r--   0 mba       (1000) mba       (1000)      376 2024-04-22 08:21:41.000000 solver-multiRPC-2.0.2/setup.py
-drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-04-22 08:21:43.767638 solver-multiRPC-2.0.2/src/
-drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-04-22 08:21:43.767638 solver-multiRPC-2.0.2/src/multirpc/
--rw-rw-r--   0 mba       (1000) mba       (1000)       51 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.2/src/multirpc/__init__.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     4044 2024-04-22 08:20:25.000000 solver-multiRPC-2.0.2/src/multirpc/async_multi_rpc_interface.py
--rw-rw-r--   0 mba       (1000) mba       (1000)    20185 2024-04-22 08:20:25.000000 solver-multiRPC-2.0.2/src/multirpc/base_multi_rpc_interface.py
--rw-rw-r--   0 mba       (1000) mba       (1000)      353 2024-04-22 08:20:25.000000 solver-multiRPC-2.0.2/src/multirpc/constants.py
--rw-rw-r--   0 mba       (1000) mba       (1000)      742 2024-04-22 08:20:25.000000 solver-multiRPC-2.0.2/src/multirpc/exceptions.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     6431 2024-04-22 08:20:25.000000 solver-multiRPC-2.0.2/src/multirpc/gas_estimation.py
--rw-rw-r--   0 mba       (1000) mba       (1000)    22215 2024-04-22 08:20:25.000000 solver-multiRPC-2.0.2/src/multirpc/multi_rpc_interface.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     4192 2024-04-22 08:20:25.000000 solver-multiRPC-2.0.2/src/multirpc/sync_multi_rpc_interface.py
--rw-rw-r--   0 mba       (1000) mba       (1000)     3778 2024-04-22 08:20:25.000000 solver-multiRPC-2.0.2/src/multirpc/utils.py
-drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-04-22 08:21:43.767638 solver-multiRPC-2.0.2/src/solver_multiRPC.egg-info/
--rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-04-22 08:21:43.000000 solver-multiRPC-2.0.2/src/solver_multiRPC.egg-info/PKG-INFO
--rw-rw-r--   0 mba       (1000) mba       (1000)      548 2024-04-22 08:21:43.000000 solver-multiRPC-2.0.2/src/solver_multiRPC.egg-info/SOURCES.txt
--rw-rw-r--   0 mba       (1000) mba       (1000)        1 2024-04-22 08:21:43.000000 solver-multiRPC-2.0.2/src/solver_multiRPC.egg-info/dependency_links.txt
--rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-04-22 08:21:43.000000 solver-multiRPC-2.0.2/src/solver_multiRPC.egg-info/requires.txt
--rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-04-22 08:21:43.000000 solver-multiRPC-2.0.2/src/solver_multiRPC.egg-info/top_level.txt
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/
+-rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/PKG-INFO
+-rw-rw-r--   0 mba       (1000) mba       (1000)     2955 2024-04-21 14:40:19.000000 solver-multiRPC-2.0.3/README.md
+-rw-rw-r--   0 mba       (1000) mba       (1000)      103 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.3/pyproject.toml
+-rw-rw-r--   0 mba       (1000) mba       (1000)      582 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/setup.cfg
+-rw-rw-r--   0 mba       (1000) mba       (1000)      376 2024-05-14 12:14:23.000000 solver-multiRPC-2.0.3/setup.py
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-05-14 12:15:44.383063 solver-multiRPC-2.0.3/src/
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/src/multirpc/
+-rw-rw-r--   0 mba       (1000) mba       (1000)       51 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.3/src/multirpc/__init__.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     4348 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/async_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)    22692 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/base_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)      608 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/constants.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     1351 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/exceptions.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     6620 2024-05-14 11:16:22.000000 solver-multiRPC-2.0.3/src/multirpc/gas_estimation.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     4618 2024-05-14 11:18:21.000000 solver-multiRPC-2.0.3/src/multirpc/sync_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     7243 2024-05-14 11:18:19.000000 solver-multiRPC-2.0.3/src/multirpc/tx_trace.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     5010 2024-05-14 11:18:23.000000 solver-multiRPC-2.0.3/src/multirpc/utils.py
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-05-14 12:15:44.387063 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/
+-rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/PKG-INFO
+-rw-rw-r--   0 mba       (1000) mba       (1000)      537 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/SOURCES.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        1 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/dependency_links.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/requires.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-05-14 12:15:44.000000 solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/top_level.txt
```

### Comparing `solver-multiRPC-2.0.2/PKG-INFO` & `solver-multiRPC-2.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solver-multiRPC
-Version: 2.0.2
+Version: 2.0.3
 Summary: Use multiple rpc for reliability
 Home-page: https://github.com/SYMM-IO/solver-multiRPC.git
 Author: rorschach
 Author-email: rorschach45001@gmail.com
 Project-URL: Bug Tracker, https://github.com/SYMM-IO/solver-multiRPC
 Keywords: multiRPC solver
 Classifier: Programming Language :: Python :: 3
```

### Comparing `solver-multiRPC-2.0.2/README.md` & `solver-multiRPC-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.2/setup.cfg` & `solver-multiRPC-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.2/src/multirpc/async_multi_rpc_interface.py` & `solver-multiRPC-2.0.3/src/multirpc/async_multi_rpc_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 import logging
-from typing import Union, Dict, Optional, TypeVar
+from typing import Union, Dict, Optional, List
 
 from eth_typing import Address, ChecksumAddress
 from web3._utils.contracts import encode_transaction_data  # noqa
 from web3.types import BlockData, BlockIdentifier, TxReceipt
 
 from . import BaseMultiRpc
 from .base_multi_rpc_interface import BaseContractFunction
+from .constants import ViewPolicy
+from .exceptions import DontHaveThisRpcType
 from .gas_estimation import GasEstimation, GasEstimationMethod
-from .utils import TxPriority, NestedDict
+from .utils import TxPriority, NestedDict, ContractFunctionType
 
 logging.basicConfig(level=logging.INFO)
 
 
-class ContractFunctionType:
-    View = "view"
-    Transaction = "transaction"
-
-
-T = TypeVar("T")
-
-
 class AsyncMultiRpc(BaseMultiRpc):
     """
     This class is used to be more sure when running web3 view calls and sending transactions by using of multiple RPCs.
     """
 
     def __init__(
             self,
             rpc_urls: NestedDict,
             contract_address: Union[Address, ChecksumAddress, str],
             contract_abi: Dict,
+            view_policy: ViewPolicy = ViewPolicy.MostUpdated,
             gas_estimation: Optional[GasEstimation] = None,
             gas_limit: int = 1_000_000,
             gas_upper_bound: int = 26_000,
             apm=None,
             enable_gas_estimation: bool = False,
             is_proof_authority: bool = False,
     ):
-        super().__init__(rpc_urls, contract_address, contract_abi, gas_estimation, gas_limit, gas_upper_bound, apm,
-                         enable_gas_estimation, is_proof_authority)
+        super().__init__(rpc_urls, contract_address, contract_abi, view_policy, gas_estimation, gas_limit,
+                         gas_upper_bound, apm, enable_gas_estimation, is_proof_authority)
 
         for func_abi in self.contract_abi:
             if func_abi.get("stateMutability") in ("view", "pure"):
                 function_type = ContractFunctionType.View
             elif func_abi.get("type") == "function":
                 function_type = ContractFunctionType.Transaction
             else:
@@ -58,14 +53,17 @@
 
     async def get_tx_receipt(self, tx_hash) -> TxReceipt:
         return await super().get_tx_receipt(tx_hash)
 
     async def get_block(self, block_identifier: BlockIdentifier, full_transactions: bool = False) -> BlockData:
         return await super().get_block(block_identifier, full_transactions)
 
+    async def get_block_number(self) -> List[int]:
+        return await super().get_block_number()
+
     class ContractFunction(BaseContractFunction):
         def __call__(self, *args, **kwargs):
             cf = AsyncMultiRpc.ContractFunction(self.name, self.abi, self.mr, self.typ)
             cf.args = args
             cf.kwargs = kwargs
             return cf
 
@@ -77,14 +75,16 @@
                 gas_upper_bound: int = None,
                 wait_for_receipt: int = 90,
                 priority: TxPriority = TxPriority.Low,
                 gas_estimation_method: GasEstimationMethod = None,
                 block_identifier: Union[str, int] = 'latest',
                 enable_gas_estimation: Optional[bool] = None,
         ):
+            if self.mr.providers.get(self.typ) is None:
+                raise DontHaveThisRpcType(f"Doesn't have {self.typ} RPCs")
             if self.typ == ContractFunctionType.View:
                 return await self.mr._call_view_function(
                     self.name, block_identifier, *self.args, **self.kwargs,
                 )
             elif self.typ == ContractFunctionType.Transaction:
                 return await self.mr._call_tx_function(
                     func_name=self.name,
```

### Comparing `solver-multiRPC-2.0.2/src/multirpc/base_multi_rpc_interface.py` & `solver-multiRPC-2.0.3/src/multirpc/base_multi_rpc_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 import asyncio
 import logging
 import time
-import web3
 from abc import ABC
 from concurrent.futures import ThreadPoolExecutor
+from time import sleep
+from typing import List, Union, Tuple, Coroutine, Dict, Optional, TypeVar
+
+import web3
 from eth_account import Account
 from eth_account.datastructures import SignedTransaction
 from eth_account.signers.local import LocalAccount
 from eth_typing import Address, ChecksumAddress
 from multicallable.async_multicallable import AsyncCall, AsyncMulticall
 from requests import ConnectionError, ReadTimeout, HTTPError
-from time import sleep
-from typing import List, Union, Tuple, Coroutine, Dict, Optional, Callable, TypeVar
 from web3 import Web3, AsyncWeb3
 from web3._utils.contracts import encode_transaction_data  # noqa
 from web3.contract import Contract
 from web3.exceptions import TimeExhausted, TransactionNotFound, BlockNotFound
 from web3.types import BlockData, BlockIdentifier, TxReceipt
 
+from .constants import mrpc_cntr, ViewPolicy
 from .exceptions import (
     FailedOnAllRPCs,
     TransactionFailedStatus,
-    Web3InterfaceException, TransactionValueError, GetBlockFailed,
+    Web3InterfaceException, TransactionValueError, GetBlockFailed, DontHaveThisRpcType, NotValidViewPolicy,
 )
 from .gas_estimation import GasEstimation, GasEstimationMethod
+from .tx_trace import TxTrace
 from .utils import TxPriority, get_span_proper_label_from_provider, get_unix_time, NestedDict, create_web3_from_rpc, \
     calculate_chain_id, reduce_list_of_list
 
 logging.basicConfig(level=logging.INFO)
 
-
-class ContractFunctionType:
-    View = "view"
-    Transaction = "transaction"
-
-
 T = TypeVar("T")
 
 
 class BaseMultiRpc(ABC):
     """
     This class is used to be more sure when running web3 view calls and sending transactions by using of multiple RPCs.
     """
 
     def __init__(
             self,
             rpc_urls: NestedDict,
             contract_address: Union[Address, ChecksumAddress, str],
             contract_abi: Dict,
+            view_policy: ViewPolicy = ViewPolicy.MostUpdated,
             gas_estimation: Optional[GasEstimation] = None,
             gas_limit: int = 1_000_000,
             gas_upper_bound: int = 26_000,
             apm=None,
             enable_gas_estimation: bool = False,
             is_proof_authority: bool = False,
     ):
@@ -64,14 +62,15 @@
         self.apm = apm
 
         self.contracts: NestedDict = NestedDict({'transaction': None, 'view': None})
         self.multi_calls: NestedDict = NestedDict({'transaction': None, 'view': None})
 
         self.functions = type("functions", (object,), {})()
 
+        self.view_policy = view_policy
         self.gas_limit = gas_limit
         self.gas_upper_bound = gas_upper_bound
         self.enable_gas_estimation = enable_gas_estimation
         self.providers = None
         self.address = None
         self.private_key = None
         self.chain_id = None
@@ -87,22 +86,24 @@
         """
         Set public key and private key for sending transactions. If these values set, there is no need to pass address,
         private_key in "call" function.
         Args:
             address: sender public_key
             private_key: sender private key
         """
+        mrpc_cntr.incr_cur_func()
         self.address = Web3.to_checksum_address(address)
         self.private_key = private_key
 
     async def setup(self, multicall_custom_address: str = None) -> None:
+        mrpc_cntr.incr_cur_func()
         self.providers = await create_web3_from_rpc(self.rpc_urls, self.is_proof_authority)
         self.chain_id = await calculate_chain_id(self.providers)
 
-        if self.gas_estimation is None:
+        if self.gas_estimation is None and self.providers.get('transaction'):
             self.gas_estimation = GasEstimation(
                 self.chain_id,
                 reduce_list_of_list(self.providers['transaction'].values()),
                 # GasEstimationMethod.METAMASK,
             )
 
         is_rpc_provided = False
@@ -127,35 +128,46 @@
                 self.multi_calls[wb3_k] = multi_calls
                 self.contracts[wb3_k] = contracts
 
         if not is_rpc_provided:
             raise ValueError("No available rpc provided")
 
     @staticmethod
-    async def __gather_tasks(execution_list: List[Coroutine]) -> List[any]:
+    async def __gather_tasks(execution_list: List[Coroutine], view_policy: ViewPolicy = ViewPolicy.MostUpdated) \
+            -> List[any]:
         """
         Get an execution list and wait for all to end. If all executable raise an exception, it will raise a
         'Web3InterfaceException' exception, otherwise returns all results which has no exception
         Args:
             execution_list:
 
         Returns:
 
         """
-        with ThreadPoolExecutor() as executor:
-            base_results = executor.map(asyncio.run, execution_list)
-        results = [res for res in base_results if not isinstance(res, Exception)]
-        if len(results) == 0:
-            exceptions = [res for res in base_results if isinstance(res, Exception)]
-            for exc in exceptions:
-                logging.exception(exc)
-            raise Web3InterfaceException(
-                f"All of RPCs raise exception. first exception: {exceptions[0]}"
-            )
-        return results
+
+        mrpc_cntr.incr_cur_func()
+
+        if view_policy == view_policy.MostUpdated:  # wait for all task to be completed
+            with ThreadPoolExecutor() as executor:
+                base_results = executor.map(asyncio.run, execution_list)
+            results = [res for res in base_results if not isinstance(res, Exception)]
+            if len(results) == 0:
+                exceptions = [res for res in base_results if isinstance(res, Exception)]
+                for exc in exceptions:
+                    logging.exception(exc)
+                raise FailedOnAllRPCs(f"All of RPCs raise exception. first exception: {exceptions[0]}")
+            return results
+        elif view_policy == view_policy.FirstSuccess:  # wait to at least 1 task completed
+            return [await BaseMultiRpc.__execute_batch_tasks(
+                execution_list,
+                [HTTPError, ConnectionError],
+                FailedOnAllRPCs
+            )]
+
+        raise NotValidViewPolicy()
 
     async def __call_view_function(self,
                                    func_name: str,
                                    block_identifier: Union[str, int] = 'latest',
                                    *args, **kwargs) -> List[any]:
         """
         Calling view function 'func_name' by using of multicall
@@ -164,30 +176,33 @@
             func_name: view function name
             *args:
             **kwargs:
 
         Returns:
             the results of multicallable object for each rpc
         """
+        mrpc_cntr.incr_cur_func()
         for contracts, multi_calls in zip(self.contracts['view'].values(),
                                           self.multi_calls['view'].values()):  # type: any, List[AsyncMulticall]
             rpc_bracket = list(map(lambda c: c.w3.provider.endpoint_uri, contracts))
 
             calls = [AsyncCall(cont, func_name, args, kwargs) for cont in contracts]
             execution_list = [mc.call([call], block_identifier=block_identifier) for mc, call in
                               zip(multi_calls, calls)]
             try:
-                return await self.__gather_tasks(execution_list)
+                return await self.__gather_tasks(execution_list, view_policy=self.view_policy)
             except (Web3InterfaceException, asyncio.TimeoutError):
                 logging.info(f"Can't call view function from this list of rpc({rpc_bracket})")
         raise Web3InterfaceException("All of RPCs raise exception.")
 
     async def _get_nonce(self, address: Union[Address, ChecksumAddress, str]) -> int:
+        mrpc_cntr.incr_cur_func()
         address = Web3.to_checksum_address(address)
-        for providers in self.providers['view'].values():
+        providers_4_nonce = self.providers.get('view') or self.providers['transaction']
+        for providers in providers_4_nonce.values():
             execution_list = [
                 prov.eth.get_transaction_count(address) for prov in providers
             ]
             try:
                 return max(await self.__gather_tasks(execution_list))
             except (Web3InterfaceException, asyncio.TimeoutError) as e:
                 logging.warning(f"get_nounce: {e}")
@@ -208,100 +223,128 @@
         return tx_params
 
     @staticmethod
     async def _build_transaction(contract: Contract, func_name: str, func_args: Tuple,
                                  func_kwargs: Dict, tx_params: Dict) -> Coroutine:
         func_args = func_args or []
         func_kwargs = func_kwargs or {}
-        return await contract.functions.__getattribute__(func_name)(
-            *func_args, **func_kwargs
-        ).build_transaction(tx_params)
+        return await contract.functions.__getattribute__(func_name)(*func_args, **func_kwargs
+                                                                    ).build_transaction(tx_params)
 
     async def _build_and_sign_transaction(
             self, contract: Contract, provider: AsyncWeb3, func_name: str, func_args: Tuple,
             func_kwargs: Dict, signer_private_key: str, tx_params: Dict,
             enable_gas_estimation: bool) -> SignedTransaction:
+        mrpc_cntr.incr_cur_func()
         try:
+            mrpc_cntr('_build_and_sign_transaction end')
             tx = await self._build_transaction(contract, func_name, func_args, func_kwargs, tx_params)
             account: LocalAccount = Account.from_key(signer_private_key)
             if enable_gas_estimation:
                 estimate_gas = await provider.eth.estimate_gas(tx)
                 logging.info(f"gas_estimation({estimate_gas} gas needed) is successful")
             return account.sign_transaction(tx)
         except Exception as e:
-            logging.error(
-                "exception in build and sign transaction: %s, %s",
-                e.__class__.__name__,
-                str(e),
-            )
+            logging.error("exception in build and sign transaction: %s, %s", e.__class__.__name__, str(e))
+            mrpc_cntr(f'unknown ex {e.__class__.__name__}')
             raise
 
-    async def _send_transaction(self, provider: web3.AsyncWeb3, raw_transaction: any,
-                                cancel_event: asyncio.Event) -> Tuple[AsyncWeb3, any]:
+    async def _send_transaction(self, provider: web3.AsyncWeb3, raw_transaction: any) -> Tuple[AsyncWeb3, any]:
+        mrpc_cntr.incr_cur_func()
         rpc_url = provider.provider.endpoint_uri
         try:
             rpc_label_prefix = get_span_proper_label_from_provider(rpc_url)
             transaction = await provider.eth.send_raw_transaction(raw_transaction)
             self._logger_params(**{f"{rpc_label_prefix}_post_send_time": get_unix_time()})
             self._logger_params(tx_send_time=int(time.time() * 1000))
-            cancel_event.set()
+            mrpc_cntr('_send_transaction end')
             return provider, transaction
         except ValueError as e:
             logging.error(f"RPC({rpc_url}) value error: {str(e)}")
+            mrpc_cntr(f'ValueError {str(e)[:30]}')
             t_bnb_flag = "transaction would cause overdraft" in str(e).lower() and (await provider.eth.chain_id) == 97
             if not (
                     t_bnb_flag or
                     'nonce too low' in str(e).lower() or
                     'already known' in str(e).lower() or
                     'transaction underpriced' in str(e).lower() or
                     'account suspended' in str(e).lower() or
                     'exceeds the configured cap' in str(e).lower()
             ):
                 logging.exception("_send_transaction_exception")
                 raise
         except (ConnectionError, ReadTimeout, HTTPError) as e:  # FIXME complete list
             logging.debug(f"network exception in send transaction: {e.__class__.__name__}, {str(e)}")
+            mrpc_cntr(f'net ex {e.__class__.__name__}')
         except Exception as e:
             # FIXME needs better exception handling
             logging.error(f"exception in send transaction: {e.__class__.__name__}, {str(e)}")
+            mrpc_cntr(f'unknown ex {e.__class__.__name__}')
 
-    async def _wait_and_get_tx_receipt(self, provider: AsyncWeb3, tx, timeout: float, cancel_event: asyncio.Event) \
-            -> AsyncWeb3:
+    def _handle_tx_trace(self, trace: TxTrace, func_name: str, func_args: Tuple, func_kwargs: Dict):
+        """
+        hedger must override this method
+        """
+        # if DevEnv:
+        #     if "out of gas" in trace.text():
+        #         raise InsufficientGasBalance(f'out of gas in {func_name}')
+        #     if "PartyBFacet: Will be liquidatable" in trace.text():
+        #         raise PartyBWillBeLiquidatable(f'partyB will be liquidatable in {func_name}')
+        #     if "LibMuon: TSS not verified" in trace.text():
+        #         raise TssNotVerified(Web3.to_hex(tx), func_name, func_args, func_kwargs, trace)
+        #     if trace.ok():
+        #         logging.error(f'TraceTransaction({func_name}): {trace.result().long_error()}')
+        #         mrpc_cntr(f'tr-failed-{func_name}-{trace.result().long_error()}')
+        #         apm.capture_message(param_message={
+        #             'message': f'tr failed ({func_name}, {trace.result().first_usable_error()}): %s',
+        #             'params': (trace.text(),),
+        #         })
+        pass
+
+    async def _wait_and_get_tx_receipt(self, provider: AsyncWeb3, tx, timeout: float,
+                                       func_name: str, func_args: Tuple, func_kwargs: Dict) -> AsyncWeb3:
+        mrpc_cntr.incr_cur_func()
         con_err_count = tx_err_count = 0
         rpc_url = provider.provider.endpoint_uri
         while True:
             try:
-                receipt = await provider.eth.wait_for_transaction_receipt(tx, timeout=timeout)
                 self._logger_params(received_provider=rpc_url)
-                if receipt.status != 1:
-                    raise TransactionFailedStatus(Web3.to_hex(tx))
-                cancel_event.set()
+                if (await provider.eth.wait_for_transaction_receipt(tx, timeout=timeout)).status != 1:
+                    trace = TxTrace(Web3.to_hex(tx))
+                    self._handle_tx_trace(trace, func_name, func_args, func_kwargs)
+                    raise TransactionFailedStatus(Web3.to_hex(tx), func_name, func_args, func_kwargs, trace)
                 return provider
             except ConnectionError:
                 if con_err_count >= 5:
                     raise
                 con_err_count += 1
                 sleep(5)
             except (TimeExhausted, TransactionNotFound):
                 if tx_err_count >= 1:  # double-check the endpoint_uri
                     raise
                 tx_err_count += 1
                 timeout *= 2
 
     @staticmethod
     async def __execute_batch_tasks(
-            execution_params_list: List[Tuple],
-            task_factory: Callable[..., Coroutine[any, any, T]],
+            execution_list: List[Coroutine],
             exception_handler: Optional[List[type[BaseException]]] = None,
             final_exception: Optional[type[BaseException]] = None
     ) -> T:
+
+        async def exec_task(task: Coroutine, cancel_event: asyncio.Event):
+            res = await task
+            cancel_event.set()
+            return res
+
+        mrpc_cntr.incr_cur_func()
         cancel_event = asyncio.Event()
         tasks = [
-            asyncio.create_task(task_factory(*params, cancel_event=cancel_event))
-            for params in execution_params_list
+            asyncio.create_task(exec_task(task, cancel_event=cancel_event))
+            for task in execution_list
         ]
         not_completed_tasks = tasks.copy()
         result = None
         exception = None
 
         while len(not_completed_tasks) > 0:
             task, not_completed_tasks = await asyncio.wait(
@@ -341,64 +384,65 @@
             private_key: str,
             wait_for_receipt: int,
             providers: List[AsyncWeb3],
             contracts: List[Contract],
             tx_params: Dict,
             enable_gas_estimation: bool,
     ) -> str:
+        mrpc_cntr.incr_cur_func()
         signed_transaction = await self._build_and_sign_transaction(
             contracts[0], providers[0], func_name, func_args, func_kwargs, private_key, tx_params, enable_gas_estimation
         )
         tx_hash = Web3.to_hex(signed_transaction.hash)
         self._logger_params(tx_hash=tx_hash)
 
-        execution_tx_params_list = [
-            (p, signed_transaction.rawTransaction) for p in providers
+        execution_tx_list = [
+            self._send_transaction(p, signed_transaction.rawTransaction) for p in providers
         ]
         result = await self.__execute_batch_tasks(
-            execution_tx_params_list,
-            self._send_transaction,
+            execution_tx_list,
             [TransactionValueError],
             FailedOnAllRPCs
         )
         provider, tx = result
 
         logging.info(f"success tx: {provider= }, {tx= }")
         rpc_url = provider.provider.endpoint_uri
         self._logger_params(sent_provider=rpc_url)
 
         if not wait_for_receipt:
             return tx_hash
-        execution_receipt_params_list = [
-            (p, tx, wait_for_receipt) for p in providers
+        execution_receipt_list = [
+            self._wait_and_get_tx_receipt(p, tx, wait_for_receipt, func_name, func_args, func_kwargs) for p in providers
         ]
         _ = await self.__execute_batch_tasks(
-            execution_receipt_params_list,
-            self._wait_and_get_tx_receipt,
+            execution_receipt_list,
             [TimeExhausted, TransactionNotFound, ConnectionError],
         )
 
         return tx_hash
 
     async def _call_view_function(self,
                                   func_name: str,
                                   block_identifier: Union[str, int] = 'latest',
                                   *args, **kwargs) -> bytes:
+        mrpc_cntr.incr_cur_func()
         results = await self.__call_view_function(func_name, block_identifier, *args, **kwargs)
         max_block_number = results[0][0]
         max_index = 0
         for i, result in enumerate(results):
             if result[0] > max_block_number:
                 max_block_number = result[0]
                 max_index = i
         return results[max_index][2][0]
 
     async def _call_tx_function(self, address: str, gas_limit: int, gas_upper_bound: int, priority: TxPriority,
                                 gas_estimation_method: GasEstimationMethod,
                                 enable_gas_estimation: Optional[bool] = None, **kwargs):
+        mrpc_cntr.incr_cur_func()
         nonce = await self._get_nonce(address)
         tx_params = await self._get_tx_params(
             nonce, address, gas_limit, gas_upper_bound, priority, gas_estimation_method
         )
         enable_gas_estimation = self.enable_gas_estimation if enable_gas_estimation is None else enable_gas_estimation
         for p, c in zip(
                 self.providers['transaction'].values(), self.contracts['transaction'].values()
@@ -408,71 +452,70 @@
                                             enable_gas_estimation=enable_gas_estimation)
             except (TransactionFailedStatus, TransactionValueError):
                 raise
             except (ConnectionError, ReadTimeout, TimeExhausted, TransactionNotFound, FailedOnAllRPCs):
                 pass
         raise Web3InterfaceException("All of RPCs raise exception.")
 
+    def check_for_view(self):
+        if self.providers.get('view') is None:
+            raise DontHaveThisRpcType(f"Doesn't have view RPCs")
+
     async def get_tx_receipt(self, tx_hash) -> TxReceipt:
-        async def _get_tx_receipt(p: AsyncWeb3, transaction_hash, cancel_event: asyncio.Event) -> TxReceipt:
-            try:
-                receipt = await p.eth.wait_for_transaction_receipt(transaction_hash)
-                cancel_event.set()
-                return receipt
-            except Exception:
-                raise
+        mrpc_cntr.incr_cur_func()
+
+        self.check_for_view()
 
         exceptions = (HTTPError, ConnectionError, ReadTimeout, ValueError, TimeExhausted, TransactionNotFound)
 
         last_exception = None
         for provider in self.providers['view'].values():  # type: List[AsyncWeb3]
-            execution_tx_params_list = [(p, tx_hash) for p in provider]
+            execution_tx_list = [p.eth.wait_for_transaction_receipt(tx_hash) for p in provider]
             try:
                 return await self.__execute_batch_tasks(
-                    execution_tx_params_list,
-                    _get_tx_receipt,
+                    execution_tx_list,
                     list(exceptions),
                     TransactionFailedStatus
                 )
             except exceptions as e:
                 last_exception = e
                 pass
             except TransactionFailedStatus:
                 raise
         raise last_exception
 
     async def get_block(self, block_identifier: BlockIdentifier, full_transactions: bool = False) -> BlockData:
-        async def _get_block(p: AsyncWeb3, block_number: BlockIdentifier, full_tx: bool,
-                             cancel_event: asyncio.Event) -> BlockData:
-            try:
-                receipt = await p.eth.get_block(block_number, full_tx)
-                cancel_event.set()
-                return receipt
-            except Exception:
-                raise
+        mrpc_cntr.incr_cur_func()
+
+        self.check_for_view()
 
         exceptions = (HTTPError, ConnectionError, ReadTimeout, ValueError, TimeExhausted, BlockNotFound)
 
         last_exception = None
         for provider in self.providers['view'].values():  # type: List[AsyncWeb3]
-            execution_tx_params_list = [(p, block_identifier, full_transactions) for p in provider]
+            execution_tx_params_list = [p.eth.get_block(block_identifier, full_transactions) for p in provider]
             try:
                 return await self.__execute_batch_tasks(
                     execution_tx_params_list,
-                    _get_block,
                     list(exceptions),
                     GetBlockFailed
                 )
             except exceptions as e:
                 last_exception = e
                 pass
             except GetBlockFailed:
                 raise
         raise last_exception
 
+    async def get_block_number(self) -> List[int]:
+        mrpc_cntr.incr_cur_func()
+        self.check_for_view()
+        execution_list = [asyncio.to_thread(provider.eth.get_block_number) for provider in self.providers['view']]
+        return await self.__gather_tasks(execution_list)
+
 
 class BaseContractFunction:
     def __init__(self, name: str, abi: Dict, multi_rpc_web3: BaseMultiRpc, typ: str):
         self.name = name
         self.mr = multi_rpc_web3
         self.typ = typ
         self.abi = abi
```

### Comparing `solver-multiRPC-2.0.2/src/multirpc/gas_estimation.py` & `solver-multiRPC-2.0.3/src/multirpc/gas_estimation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 from _decimal import Decimal
 from decimal import Decimal
 from typing import Callable, Union
 from typing import List, Dict, Optional
 
 import requests
-from requests import JSONDecodeError, RequestException, ReadTimeout
+from requests import JSONDecodeError, RequestException, ReadTimeout, ConnectionError
 from web3 import Web3, AsyncWeb3
 from web3.types import Wei
 
+from .constants import ChainIdToGas, FixedValueGas, DEFAULT_API_PROVIDER, GasEstimationMethod, RequestTimeout, DevEnv, \
+    GasFromRpcChainIds
 from .exceptions import OutOfRangeTransactionFee, FailedToGetGasPrice
 from .utils import TxPriority
-from .constants import ChainIdToGas, FixedValueGas, DEFAULT_API_PROVIDER, GasEstimationMethod, RequestTimeout, DevEnv
 
 
 class GasEstimation:
 
     def __init__(
             self,
             chain_id: int,
@@ -103,15 +104,15 @@
             rpc_url = provider.provider.endpoint_uri
             try:
                 gas_price = await provider.eth.gas_price
                 self.__logger_params(gas_price=str(gas_price / 1e9), gas_price_provider=rpc_url)
                 if gas_price / 1e9 <= gas_upper_bound:
                     found_gas_below_upper_bound = True
                     break
-            except (ConnectionError, ReadTimeout) as e:
+            except (ConnectionError, ReadTimeout, ValueError) as e:
                 logging.error(f"Failed to get gas price from {rpc_url}, {e=}")
 
         if gas_price is None:
             raise FailedToGetGasPrice("Non of RCP could provide gas price!")
         if not found_gas_below_upper_bound:
             raise OutOfRangeTransactionFee(
                 f"gas price exceeded. {gas_upper_bound=} but it is {gas_price / 1e9}"
@@ -132,14 +133,17 @@
     ) -> Dict[str, Wei]:
         if method := self.gas_estimation_method.get(method) or self.gas_estimation_method.get(self.default_method):
             try:
                 return await method(priority, gas_upper_bound)
             except FailedToGetGasPrice as e:
                 raise e
         gas_params = {}
+
+        if DevEnv or self.chain_id in GasFromRpcChainIds:
+            return await self._get_gas_from_rpc(priority, gas_upper_bound)
         for method_key in self.method_sorted_priority:
             try:
                 gas_params = await self.gas_estimation_method[method_key](priority, gas_upper_bound)
                 break
             except (FailedToGetGasPrice, OutOfRangeTransactionFee) as e:
                 logging.warning(f"This method({method_key}) failed to provide gas with this error: {e}")
                 continue
```

### Comparing `solver-multiRPC-2.0.2/src/multirpc/sync_multi_rpc_interface.py` & `solver-multiRPC-2.0.3/src/multirpc/sync_multi_rpc_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,99 @@
 import asyncio
 import logging
-from typing import Union, Dict, Optional, TypeVar
+from typing import Union, Dict, Optional, List
 
 from eth_typing import Address, ChecksumAddress
 from web3._utils.contracts import encode_transaction_data  # noqa
 from web3.types import BlockData, BlockIdentifier, TxReceipt
 
 from . import BaseMultiRpc
 from .base_multi_rpc_interface import BaseContractFunction
+from .constants import ViewPolicy
+from .exceptions import DontHaveThisRpcType
 from .gas_estimation import GasEstimation, GasEstimationMethod
-from .utils import TxPriority, NestedDict
+from .utils import TxPriority, NestedDict, ContractFunctionType, thread_safe
 
 logging.basicConfig(level=logging.INFO)
 
 
-class ContractFunctionType:
-    View = "view"
-    Transaction = "transaction"
-
-
-T = TypeVar("T")
-
-
 class MultiRpc(BaseMultiRpc):
     """
     This class is used to be more sure when running web3 view calls and sending transactions by using of multiple RPCs.
     """
 
+    @thread_safe
     def __init__(
             self,
             rpc_urls: NestedDict,
             contract_address: Union[Address, ChecksumAddress, str],
             contract_abi: Dict,
+            view_policy: ViewPolicy = ViewPolicy.MostUpdated,
             gas_estimation: Optional[GasEstimation] = None,
             gas_limit: int = 1_000_000,
             gas_upper_bound: int = 26_000,
             apm=None,
             enable_gas_estimation: bool = False,
             is_proof_authority: bool = False,
             multicall_custom_address: str = None
     ):
-        super().__init__(rpc_urls, contract_address, contract_abi, gas_estimation, gas_limit, gas_upper_bound, apm,
-                         enable_gas_estimation, is_proof_authority)
+        super().__init__(rpc_urls, contract_address, contract_abi, view_policy, gas_estimation, gas_limit,
+                         gas_upper_bound, apm, enable_gas_estimation, is_proof_authority)
 
         for func_abi in self.contract_abi:
             if func_abi.get("stateMutability") in ("view", "pure"):
                 function_type = ContractFunctionType.View
             elif func_abi.get("type") == "function":
                 function_type = ContractFunctionType.Transaction
             else:
                 continue
             self.functions.__setattr__(
                 func_abi["name"],
                 self.ContractFunction(func_abi["name"], func_abi, self, function_type),
             )
         asyncio.run(self.setup(multicall_custom_address=multicall_custom_address))
 
+    @thread_safe
     def get_nonce(self, address: Union[Address, ChecksumAddress, str]) -> int:
         return asyncio.run(super()._get_nonce(address))
 
+    @thread_safe
     def get_tx_receipt(self, tx_hash) -> TxReceipt:
         return asyncio.run(super().get_tx_receipt(tx_hash))
 
+    @thread_safe
     def get_block(self, block_identifier: BlockIdentifier, full_transactions: bool = False) -> BlockData:
         return asyncio.run(super().get_block(block_identifier, full_transactions))
 
+    @thread_safe
+    def get_block_number(self) -> List[int]:
+        return asyncio.run((super().get_block_number()))
+
     class ContractFunction(BaseContractFunction):
         def __call__(self, *args, **kwargs):
             cf = MultiRpc.ContractFunction(self.name, self.abi, self.mr, self.typ)
             cf.args = args
             cf.kwargs = kwargs
             return cf
 
+        @thread_safe
         def call(
                 self,
                 address: str = None,
                 private_key: str = None,
                 gas_limit: int = None,
                 gas_upper_bound: int = None,
                 wait_for_receipt: int = 90,
                 priority: TxPriority = TxPriority.Low,
                 gas_estimation_method: GasEstimationMethod = None,
                 block_identifier: Union[str, int] = 'latest',
                 enable_gas_estimation: Optional[bool] = None,
         ):
+            if self.mr.providers.get(self.typ) is None:
+                raise DontHaveThisRpcType(f"Doesn't have {self.typ} RPCs")
             if self.typ == ContractFunctionType.View:
                 return asyncio.run(self.mr._call_view_function(
                     self.name, block_identifier, *self.args, **self.kwargs,
                 ))
             elif self.typ == ContractFunctionType.Transaction:
                 return asyncio.run(self.mr._call_tx_function(
                     func_name=self.name,
```

### Comparing `solver-multiRPC-2.0.2/src/solver_multiRPC.egg-info/PKG-INFO` & `solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solver-multiRPC
-Version: 2.0.2
+Version: 2.0.3
 Summary: Use multiple rpc for reliability
 Home-page: https://github.com/SYMM-IO/solver-multiRPC.git
 Author: rorschach
 Author-email: rorschach45001@gmail.com
 Project-URL: Bug Tracker, https://github.com/SYMM-IO/solver-multiRPC
 Keywords: multiRPC solver
 Classifier: Programming Language :: Python :: 3
```

### Comparing `solver-multiRPC-2.0.2/src/solver_multiRPC.egg-info/SOURCES.txt` & `solver-multiRPC-2.0.3/src/solver_multiRPC.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup.py
 src/multirpc/__init__.py
 src/multirpc/async_multi_rpc_interface.py
 src/multirpc/base_multi_rpc_interface.py
 src/multirpc/constants.py
 src/multirpc/exceptions.py
 src/multirpc/gas_estimation.py
-src/multirpc/multi_rpc_interface.py
 src/multirpc/sync_multi_rpc_interface.py
+src/multirpc/tx_trace.py
 src/multirpc/utils.py
 src/solver_multiRPC.egg-info/PKG-INFO
 src/solver_multiRPC.egg-info/SOURCES.txt
 src/solver_multiRPC.egg-info/dependency_links.txt
 src/solver_multiRPC.egg-info/requires.txt
 src/solver_multiRPC.egg-info/top_level.txt
```

