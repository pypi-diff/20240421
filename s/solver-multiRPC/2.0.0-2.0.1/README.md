# Comparing `tmp/solver-multiRPC-2.0.0.tar.gz` & `tmp/solver-multiRPC-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver-multiRPC-2.0.0.tar", last modified: Sat Jan 27 10:31:42 2024, max compression
+gzip compressed data, was "solver-multiRPC-2.0.1.tar", last modified: Sun Apr 21 14:55:57 2024, max compression
```

## Comparing `solver-multiRPC-2.0.0.tar` & `solver-multiRPC-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rorschach  (1000) rorschach  (1000)        0 2024-01-27 10:31:42.517776 solver-multiRPC-2.0.0/
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)     3430 2024-01-27 10:31:42.517776 solver-multiRPC-2.0.0/PKG-INFO
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)     2954 2023-11-12 08:25:13.000000 solver-multiRPC-2.0.0/README.md
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      103 2023-11-05 15:14:39.000000 solver-multiRPC-2.0.0/pyproject.toml
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      582 2024-01-27 10:31:42.517776 solver-multiRPC-2.0.0/setup.cfg
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      377 2024-01-27 10:12:18.000000 solver-multiRPC-2.0.0/setup.py
-drwxrwxr-x   0 rorschach  (1000) rorschach  (1000)        0 2024-01-27 10:31:42.513776 solver-multiRPC-2.0.0/src/
-drwxrwxr-x   0 rorschach  (1000) rorschach  (1000)        0 2024-01-27 10:31:42.513776 solver-multiRPC-2.0.0/src/multirpc/
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)       51 2024-01-27 10:11:05.000000 solver-multiRPC-2.0.0/src/multirpc/__init__.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)     4044 2024-01-27 10:11:05.000000 solver-multiRPC-2.0.0/src/multirpc/async_multi_rpc_interface.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)    20107 2024-01-27 10:05:20.000000 solver-multiRPC-2.0.0/src/multirpc/base_multi_rpc_interface.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      353 2024-01-27 10:05:20.000000 solver-multiRPC-2.0.0/src/multirpc/constants.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      742 2024-01-27 10:05:20.000000 solver-multiRPC-2.0.0/src/multirpc/exceptions.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)     6431 2024-01-27 10:05:20.000000 solver-multiRPC-2.0.0/src/multirpc/gas_estimation.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)    22215 2023-11-19 15:21:14.000000 solver-multiRPC-2.0.0/src/multirpc/multi_rpc_interface.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)     4094 2024-01-27 10:07:30.000000 solver-multiRPC-2.0.0/src/multirpc/sync_multi_rpc_interface.py
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)     3778 2024-01-27 10:05:20.000000 solver-multiRPC-2.0.0/src/multirpc/utils.py
-drwxrwxr-x   0 rorschach  (1000) rorschach  (1000)        0 2024-01-27 10:31:42.517776 solver-multiRPC-2.0.0/src/solver_multiRPC.egg-info/
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)     3430 2024-01-27 10:31:42.000000 solver-multiRPC-2.0.0/src/solver_multiRPC.egg-info/PKG-INFO
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)      548 2024-01-27 10:31:42.000000 solver-multiRPC-2.0.0/src/solver_multiRPC.egg-info/SOURCES.txt
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)        1 2024-01-27 10:31:42.000000 solver-multiRPC-2.0.0/src/solver_multiRPC.egg-info/dependency_links.txt
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)        9 2024-01-27 10:31:42.000000 solver-multiRPC-2.0.0/src/solver_multiRPC.egg-info/requires.txt
--rw-rw-r--   0 rorschach  (1000) rorschach  (1000)        9 2024-01-27 10:31:42.000000 solver-multiRPC-2.0.0/src/solver_multiRPC.egg-info/top_level.txt
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-04-21 14:55:57.902405 solver-multiRPC-2.0.1/
+-rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-04-21 14:55:57.902405 solver-multiRPC-2.0.1/PKG-INFO
+-rw-rw-r--   0 mba       (1000) mba       (1000)     2955 2024-04-21 14:40:19.000000 solver-multiRPC-2.0.1/README.md
+-rw-rw-r--   0 mba       (1000) mba       (1000)      103 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.1/pyproject.toml
+-rw-rw-r--   0 mba       (1000) mba       (1000)      582 2024-04-21 14:55:57.902405 solver-multiRPC-2.0.1/setup.cfg
+-rw-rw-r--   0 mba       (1000) mba       (1000)      376 2024-04-21 14:53:17.000000 solver-multiRPC-2.0.1/setup.py
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-04-21 14:55:57.898405 solver-multiRPC-2.0.1/src/
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-04-21 14:55:57.898405 solver-multiRPC-2.0.1/src/multirpc/
+-rw-rw-r--   0 mba       (1000) mba       (1000)       51 2024-01-30 13:14:22.000000 solver-multiRPC-2.0.1/src/multirpc/__init__.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     4044 2024-04-21 14:55:31.000000 solver-multiRPC-2.0.1/src/multirpc/async_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)    20185 2024-04-21 14:55:31.000000 solver-multiRPC-2.0.1/src/multirpc/base_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)      353 2024-04-21 14:55:31.000000 solver-multiRPC-2.0.1/src/multirpc/constants.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)      742 2024-04-21 14:55:31.000000 solver-multiRPC-2.0.1/src/multirpc/exceptions.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     6431 2024-04-21 14:55:31.000000 solver-multiRPC-2.0.1/src/multirpc/gas_estimation.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)    22215 2024-04-21 14:55:31.000000 solver-multiRPC-2.0.1/src/multirpc/multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     4182 2024-04-21 14:55:31.000000 solver-multiRPC-2.0.1/src/multirpc/sync_multi_rpc_interface.py
+-rw-rw-r--   0 mba       (1000) mba       (1000)     3778 2024-04-21 14:55:31.000000 solver-multiRPC-2.0.1/src/multirpc/utils.py
+drwxrwxr-x   0 mba       (1000) mba       (1000)        0 2024-04-21 14:55:57.902405 solver-multiRPC-2.0.1/src/solver_multiRPC.egg-info/
+-rw-r--r--   0 mba       (1000) mba       (1000)     3455 2024-04-21 14:55:57.000000 solver-multiRPC-2.0.1/src/solver_multiRPC.egg-info/PKG-INFO
+-rw-rw-r--   0 mba       (1000) mba       (1000)      548 2024-04-21 14:55:57.000000 solver-multiRPC-2.0.1/src/solver_multiRPC.egg-info/SOURCES.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        1 2024-04-21 14:55:57.000000 solver-multiRPC-2.0.1/src/solver_multiRPC.egg-info/dependency_links.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-04-21 14:55:57.000000 solver-multiRPC-2.0.1/src/solver_multiRPC.egg-info/requires.txt
+-rw-rw-r--   0 mba       (1000) mba       (1000)        9 2024-04-21 14:55:57.000000 solver-multiRPC-2.0.1/src/solver_multiRPC.egg-info/top_level.txt
```

### Comparing `solver-multiRPC-2.0.0/PKG-INFO` & `solver-multiRPC-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: solver-multiRPC
-Version: 2.0.0
+Version: 2.0.1
 Summary: Use multiple rpc for reliability
 Home-page: https://github.com/SYMM-IO/solver-multiRPC.git
 Author: rorschach
 Author-email: rorschach45001@gmail.com
 Project-URL: Bug Tracker, https://github.com/SYMM-IO/solver-multiRPC
 Keywords: multiRPC solver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 
 # solver-MultiRpc: Reliable Ethereum Interactions with Multiple RPCs
 
 `solver-MultiRpc` is a Python package designed to enhance the reliability of Ethereum smart contract interactions by utilizing multiple RPC (Remote Procedure Call) endpoints. If one RPC fails, the system can fall back to another, ensuring a higher success rate for your operations.
 
 ## Features
 
 - **Multiple RPC Support**: Seamlessly switch between different RPCs to ensure uninterrupted interactions.
 - **Gas Management**: Fetch gas prices from multiple sources to ensure transactions are sent with an appropriate fee.
 - **Robust Error Handling**: Designed to handle failures gracefully, increasing the reliability of your applications.
 - **Easy-to-use API**: Interact with Ethereum smart contracts using a simple and intuitive API.
 
+
 ## Installation
 
 Install `solver-MultiRpc` using pip:
 
 ```bash
 pip install solver-multiRPC
 ```
```

### Comparing `solver-multiRPC-2.0.0/README.md` & `solver-multiRPC-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ## Features
 
 - **Multiple RPC Support**: Seamlessly switch between different RPCs to ensure uninterrupted interactions.
 - **Gas Management**: Fetch gas prices from multiple sources to ensure transactions are sent with an appropriate fee.
 - **Robust Error Handling**: Designed to handle failures gracefully, increasing the reliability of your applications.
 - **Easy-to-use API**: Interact with Ethereum smart contracts using a simple and intuitive API.
 
+
 ## Installation
 
 Install `solver-MultiRpc` using pip:
 
 ```bash
 pip install solver-multiRPC
 ```
```

### Comparing `solver-multiRPC-2.0.0/setup.cfg` & `solver-multiRPC-2.0.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multirpc
-version = 2.0.0
+version = 2.0.1
 author = rorschach
 author_email = rorschach45001@gmail.com
 description = Use multiple rpc for reliability
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SYMM-IO/
 project_urls =
```

### Comparing `solver-multiRPC-2.0.0/src/multirpc/async_multi_rpc_interface.py` & `solver-multiRPC-2.0.1/src/multirpc/async_multi_rpc_interface.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.0/src/multirpc/base_multi_rpc_interface.py` & `solver-multiRPC-2.0.1/src/multirpc/base_multi_rpc_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import asyncio
 import logging
 import time
+import web3
 from abc import ABC
 from concurrent.futures import ThreadPoolExecutor
-from time import sleep
-from typing import List, Union, Tuple, Coroutine, Dict, Optional, Callable, TypeVar
-
-import web3
 from eth_account import Account
 from eth_account.datastructures import SignedTransaction
 from eth_account.signers.local import LocalAccount
 from eth_typing import Address, ChecksumAddress
 from multicallable.async_multicallable import AsyncCall, AsyncMulticall
 from requests import ConnectionError, ReadTimeout, HTTPError
+from time import sleep
+from typing import List, Union, Tuple, Coroutine, Dict, Optional, Callable, TypeVar
 from web3 import Web3, AsyncWeb3
 from web3._utils.contracts import encode_transaction_data  # noqa
 from web3.contract import Contract
 from web3.exceptions import TimeExhausted, TransactionNotFound, BlockNotFound
 from web3.types import BlockData, BlockIdentifier, TxReceipt
 
 from .exceptions import (
@@ -91,15 +90,15 @@
         Args:
             address: sender public_key
             private_key: sender private key
         """
         self.address = Web3.to_checksum_address(address)
         self.private_key = private_key
 
-    async def setup(self) -> None:
+    async def setup(self, multicall_custom_address: str = None) -> None:
         self.providers = await create_web3_from_rpc(self.rpc_urls, self.is_proof_authority)
         self.chain_id = await calculate_chain_id(self.providers)
 
         if self.gas_estimation is None:
             self.gas_estimation = GasEstimation(
                 self.chain_id,
                 reduce_list_of_list(self.providers['transaction'].values()),
@@ -110,15 +109,15 @@
         for wb3_k, wb3_v in self.providers.items():  # type: Tuple, List[web3.AsyncWeb3]
             multi_calls = []
             contracts = []
             for wb3 in wb3_v:
                 rpc_url = wb3.provider.endpoint_uri
                 try:
                     mc = AsyncMulticall()
-                    await mc.setup(w3=wb3)
+                    await mc.setup(w3=wb3, custom_address=multicall_custom_address)
                     multi_calls.append(mc)
                     contracts.append(
                         wb3.eth.contract(self.contract_address, abi=self.contract_abi)
                     )
                 except (ConnectionError, ReadTimeout, asyncio.TimeoutError) as e:
                     # fixme: at least we should retry not ignoring rpc
                     logging.warning(f"Ignore rpc {rpc_url} because of {e}")
```

### Comparing `solver-multiRPC-2.0.0/src/multirpc/exceptions.py` & `solver-multiRPC-2.0.1/src/multirpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.0/src/multirpc/gas_estimation.py` & `solver-multiRPC-2.0.1/src/multirpc/gas_estimation.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.0/src/multirpc/multi_rpc_interface.py` & `solver-multiRPC-2.0.1/src/multirpc/multi_rpc_interface.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.0/src/multirpc/sync_multi_rpc_interface.py` & `solver-multiRPC-2.0.1/src/multirpc/sync_multi_rpc_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
             contract_abi: Dict,
             gas_estimation: Optional[GasEstimation] = None,
             gas_limit: int = 1_000_000,
             gas_upper_bound: int = 26_000,
             apm=None,
             enable_gas_estimation: bool = False,
             is_proof_authority: bool = False,
+            multicall_custom_address: str = None
     ):
         super().__init__(rpc_urls, contract_address, contract_abi, gas_estimation, gas_limit, gas_upper_bound, apm,
                          enable_gas_estimation, is_proof_authority)
 
         for func_abi in self.contract_abi:
             if func_abi.get("stateMutability") in ("view", "pure"):
                 function_type = ContractFunctionType.View
@@ -49,15 +50,15 @@
                 function_type = ContractFunctionType.Transaction
             else:
                 continue
             self.functions.__setattr__(
                 func_abi["name"],
                 self.ContractFunction(func_abi["name"], func_abi, self, function_type),
             )
-        asyncio.run(self.setup())
+        asyncio.run(self.setup(custom_address=multicall_custom_address))
 
     def get_nonce(self, address: Union[Address, ChecksumAddress, str]) -> int:
         return asyncio.run(super()._get_nonce(address))
 
     def get_tx_receipt(self, tx_hash) -> TxReceipt:
         return asyncio.run(super().get_tx_receipt(tx_hash))
```

### Comparing `solver-multiRPC-2.0.0/src/multirpc/utils.py` & `solver-multiRPC-2.0.1/src/multirpc/utils.py`

 * *Files identical despite different names*

### Comparing `solver-multiRPC-2.0.0/src/solver_multiRPC.egg-info/PKG-INFO` & `solver-multiRPC-2.0.1/src/solver_multiRPC.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: solver-multiRPC
-Version: 2.0.0
+Version: 2.0.1
 Summary: Use multiple rpc for reliability
 Home-page: https://github.com/SYMM-IO/solver-multiRPC.git
 Author: rorschach
 Author-email: rorschach45001@gmail.com
 Project-URL: Bug Tracker, https://github.com/SYMM-IO/solver-multiRPC
 Keywords: multiRPC solver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 
 # solver-MultiRpc: Reliable Ethereum Interactions with Multiple RPCs
 
 `solver-MultiRpc` is a Python package designed to enhance the reliability of Ethereum smart contract interactions by utilizing multiple RPC (Remote Procedure Call) endpoints. If one RPC fails, the system can fall back to another, ensuring a higher success rate for your operations.
 
 ## Features
 
 - **Multiple RPC Support**: Seamlessly switch between different RPCs to ensure uninterrupted interactions.
 - **Gas Management**: Fetch gas prices from multiple sources to ensure transactions are sent with an appropriate fee.
 - **Robust Error Handling**: Designed to handle failures gracefully, increasing the reliability of your applications.
 - **Easy-to-use API**: Interact with Ethereum smart contracts using a simple and intuitive API.
 
+
 ## Installation
 
 Install `solver-MultiRpc` using pip:
 
 ```bash
 pip install solver-multiRPC
 ```
```

### Comparing `solver-multiRPC-2.0.0/src/solver_multiRPC.egg-info/SOURCES.txt` & `solver-multiRPC-2.0.1/src/solver_multiRPC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

