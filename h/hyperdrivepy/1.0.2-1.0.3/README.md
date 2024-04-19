# Comparing `tmp/hyperdrivepy-1.0.2.tar.gz` & `tmp/hyperdrivepy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdrivepy-1.0.2.tar", last modified: Thu Apr 18 00:15:06 2024, max compression
+gzip compressed data, was "hyperdrivepy-1.0.3.tar", last modified: Fri Apr 19 21:07:14 2024, max compression
```

## Comparing `hyperdrivepy-1.0.2.tar` & `hyperdrivepy-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:15:06.054545 hyperdrivepy-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-18 00:15:06.054545 hyperdrivepy-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:15:06.050546 hyperdrivepy-1.0.2/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:15:06.050546 hyperdrivepy-1.0.2/python/hyperdrivepy/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/hyperdrive_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/hyperdrive_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:15:06.050546 hyperdrivepy-1.0.2/python/hyperdrivepy/pypechain_types/
--rw-r--r--   0 runner    (1001) docker     (127)   251847 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py
--rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/pypechain_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/pypechain_types/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/python/hyperdrivepy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:15:06.054545 hyperdrivepy-1.0.2/python/hyperdrivepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-18 00:15:06.000000 hyperdrivepy-1.0.2/python/hyperdrivepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 00:15:06.000000 hyperdrivepy-1.0.2/python/hyperdrivepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:15:06.000000 hyperdrivepy-1.0.2/python/hyperdrivepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:15:05.000000 hyperdrivepy-1.0.2/python/hyperdrivepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 00:15:06.000000 hyperdrivepy-1.0.2/python/hyperdrivepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:15:06.054545 hyperdrivepy-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:15:06.054545 hyperdrivepy-1.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/src/hyperdrive_state.rs
--rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/src/hyperdrive_state_methods.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/src/hyperdrive_utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/src/pool_config.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/src/pool_info.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-18 00:15:00.000000 hyperdrivepy-1.0.2/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.320318 hyperdrivepy-1.0.3/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.320318 hyperdrivepy-1.0.3/python/hyperdrivepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20357 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/hyperdrive_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/hyperdrive_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/
+-rw-r--r--   0 runner    (1001) docker     (127)   255141 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/python/hyperdrivepy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:07:14.000000 hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:07:14.324319 hyperdrivepy-1.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/hyperdrive_state.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16359 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/hyperdrive_state_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/hyperdrive_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/pool_config.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/pool_info.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-19 21:07:10.000000 hyperdrivepy-1.0.3/src/utils.rs
```

### Comparing `hyperdrivepy-1.0.2/Cargo.toml` & `hyperdrivepy-1.0.3/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "hyperdrivepy"
 edition = "2021"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     "Dylan Paiton",
     "Matt Brown",
     "Sheng Lundquist",
 ]
 description = "Python wrappers for the Hyperdrive AMM"
```

### Comparing `hyperdrivepy-1.0.2/LICENSE` & `hyperdrivepy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/PKG-INFO` & `hyperdrivepy-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdrivepy
-Version: 1.0.2
+Version: 1.0.3
 Project-URL: Homepage, https://github.com/delvtech/hyperdrive-bindings
 Project-URL: Issues, https://github.com/delvtech/hyperdrive-bindings/issues
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hyperdrivepy-1.0.2/pyproject.toml` & `hyperdrivepy-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperdrivepy"
-version = "1.0.2"
+version = "1.0.3"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 readme = "README.md"
```

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy/hyperdrive_state.py` & `hyperdrivepy-1.0.3/python/hyperdrivepy/hyperdrive_state.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy/hyperdrive_utils.py` & `hyperdrivepy-1.0.3/python/hyperdrivepy/hyperdrive_utils.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py` & `hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/IHyperdriveContract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # consumers have too many opinions on line length
 # pylint: disable=line-too-long
 
 
 from __future__ import annotations
 
-from typing import Any, Iterable, NamedTuple, Sequence, Type, cast
+from typing import Any, Iterable, NamedTuple, Sequence, Type, cast, overload
 
 from eth_abi.codec import ABICodec
 from eth_abi.registry import registry as default_registry
 from eth_account.signers.local import LocalAccount
 from eth_typing import ChecksumAddress, HexStr
 from hexbytes import HexBytes
 from typing_extensions import Self
@@ -659,41 +659,86 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(list[bytes], rename_returned_types(structs, return_types, raw_values))
 
 
-class IHyperdriveNameContractFunction(ContractFunction):
+class IHyperdriveNameContractFunction0(ContractFunction):
     """ContractFunction for the name method."""
 
     def __call__(self, tokenId: int) -> IHyperdriveNameContractFunction:  # type: ignore
-        clone = super().__call__(dataclass_to_tuple(tokenId))
-        self.kwargs = clone.kwargs
-        self.args = clone.args
-        return self
+        super().__call__()  # type: ignore
+        return cast(IHyperdriveNameContractFunction, self)
 
     def call(
         self,
         transaction: TxParams | None = None,
         block_identifier: BlockIdentifier = "latest",
         state_override: CallOverride | None = None,
         ccip_read_enabled: bool | None = None,
     ) -> str:
         """returns str."""
         # Define the expected return types from the smart contract call
 
         return_types = str
 
         # Call the function
+        raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
+
+        return cast(str, rename_returned_types(structs, return_types, raw_values))
+
+
+class IHyperdriveNameContractFunction1(ContractFunction):
+    """ContractFunction for the name method."""
+
+    def __call__(self) -> IHyperdriveNameContractFunction:  # type: ignore
+        super().__call__()  # type: ignore
+        return cast(IHyperdriveNameContractFunction, self)
 
+    def call(
+        self,
+        transaction: TxParams | None = None,
+        block_identifier: BlockIdentifier = "latest",
+        state_override: CallOverride | None = None,
+        ccip_read_enabled: bool | None = None,
+    ) -> str:
+        """returns str."""
+        # Define the expected return types from the smart contract call
+
+        return_types = str
+
+        # Call the function
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
+
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
+class IHyperdriveNameContractFunction(ContractFunction):
+    """ContractFunction for the name method."""
+
+    # super() call methods are generic, while our version adds values & types
+    # pylint: disable=arguments-differ# disable this warning when there is overloading
+    # pylint: disable=function-redefined
+
+    @overload
+    def __call__(self, tokenId: int) -> IHyperdriveNameContractFunction0:  # type: ignore
+        ...
+
+    @overload
+    def __call__(self) -> IHyperdriveNameContractFunction1:  # type: ignore
+        ...
+
+    def __call__(self, *args) -> IHyperdriveNameContractFunction:  # type: ignore
+        clone = super().__call__(*(dataclass_to_tuple(arg) for arg in args))
+        self.kwargs = clone.kwargs
+        self.args = clone.args
+        return self  # type: ignore
+
+
 class IHyperdriveNoncesContractFunction(ContractFunction):
     """ContractFunction for the nonces method."""
 
     def __call__(self, owner: str) -> IHyperdriveNoncesContractFunction:  # type: ignore
         clone = super().__call__(dataclass_to_tuple(owner))
         self.kwargs = clone.kwargs
         self.args = clone.args
@@ -1387,14 +1432,41 @@
 
         # Call the function
 
         raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
         return cast(str, rename_returned_types(structs, return_types, raw_values))
 
 
+class IHyperdriveVersionContractFunction(ContractFunction):
+    """ContractFunction for the version method."""
+
+    def __call__(self) -> IHyperdriveVersionContractFunction:  # type: ignore
+        clone = super().__call__()
+        self.kwargs = clone.kwargs
+        self.args = clone.args
+        return self
+
+    def call(
+        self,
+        transaction: TxParams | None = None,
+        block_identifier: BlockIdentifier = "latest",
+        state_override: CallOverride | None = None,
+        ccip_read_enabled: bool | None = None,
+    ) -> str:
+        """returns str."""
+        # Define the expected return types from the smart contract call
+
+        return_types = str
+
+        # Call the function
+
+        raw_values = super().call(transaction, block_identifier, state_override, ccip_read_enabled)
+        return cast(str, rename_returned_types(structs, return_types, raw_values))
+
+
 class IHyperdriveContractFunctions(ContractFunctions):
     """ContractFunctions for the IHyperdrive contract."""
 
     PERMIT_TYPEHASH: IHyperdrivePERMIT_TYPEHASHContractFunction
 
     addLiquidity: IHyperdriveAddLiquidityContractFunction
 
@@ -1488,14 +1560,16 @@
 
     transferFrom: IHyperdriveTransferFromContractFunction
 
     transferFromBridge: IHyperdriveTransferFromBridgeContractFunction
 
     vaultSharesToken: IHyperdriveVaultSharesTokenContractFunction
 
+    version: IHyperdriveVersionContractFunction
+
     def __init__(
         self,
         abi: ABI,
         w3: "Web3",
         address: ChecksumAddress | None = None,
         decode_tuples: bool | None = False,
     ) -> None:
@@ -1888,14 +1962,22 @@
             "vaultSharesToken",
             w3=w3,
             contract_abi=abi,
             address=address,
             decode_tuples=decode_tuples,
             function_identifier="vaultSharesToken",
         )
+        self.version = IHyperdriveVersionContractFunction.factory(
+            "version",
+            w3=w3,
+            contract_abi=abi,
+            address=address,
+            decode_tuples=decode_tuples,
+            function_identifier="version",
+        )
 
 
 class IHyperdriveAddLiquidityContractEvent(ContractEvent):
     """ContractEvent for AddLiquidity."""
 
     # super() get_logs and create_filter methods are generic, while our version adds values & types
     # pylint: disable=arguments-differ
@@ -5987,14 +6069,21 @@
             "name": "name",
             "inputs": [{"name": "tokenId", "type": "uint256", "internalType": "uint256"}],
             "outputs": [{"name": "", "type": "string", "internalType": "string"}],
             "stateMutability": "view",
         },
         {
             "type": "function",
+            "name": "name",
+            "inputs": [],
+            "outputs": [{"name": "", "type": "string", "internalType": "string"}],
+            "stateMutability": "pure",
+        },
+        {
+            "type": "function",
             "name": "nonces",
             "inputs": [{"name": "owner", "type": "address", "internalType": "address"}],
             "outputs": [{"name": "", "type": "uint256", "internalType": "uint256"}],
             "stateMutability": "view",
         },
         {
             "type": "function",
@@ -6272,14 +6361,21 @@
             "type": "function",
             "name": "vaultSharesToken",
             "inputs": [],
             "outputs": [{"name": "", "type": "address", "internalType": "address"}],
             "stateMutability": "view",
         },
         {
+            "type": "function",
+            "name": "version",
+            "inputs": [],
+            "outputs": [{"name": "", "type": "string", "internalType": "string"}],
+            "stateMutability": "pure",
+        },
+        {
             "type": "event",
             "name": "AddLiquidity",
             "inputs": [
                 {"name": "provider", "type": "address", "indexed": True, "internalType": "address"},
                 {"name": "lpAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "baseAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
                 {"name": "vaultShareAmount", "type": "uint256", "indexed": False, "internalType": "uint256"},
```

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py` & `hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/IHyperdriveTypes.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy/pypechain_types/utilities.py` & `hyperdrivepy-1.0.3/python/hyperdrivepy/pypechain_types/utilities.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy/types.py` & `hyperdrivepy-1.0.3/python/hyperdrivepy/types.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy/utils.py` & `hyperdrivepy-1.0.3/python/hyperdrivepy/utils.py`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy.egg-info/PKG-INFO` & `hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdrivepy
-Version: 1.0.2
+Version: 1.0.3
 Project-URL: Homepage, https://github.com/delvtech/hyperdrive-bindings
 Project-URL: Issues, https://github.com/delvtech/hyperdrive-bindings/issues
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `hyperdrivepy-1.0.2/python/hyperdrivepy.egg-info/SOURCES.txt` & `hyperdrivepy-1.0.3/python/hyperdrivepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/src/hyperdrive_state.rs` & `hyperdrivepy-1.0.3/src/hyperdrive_state.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/src/hyperdrive_state_methods.rs` & `hyperdrivepy-1.0.3/src/hyperdrive_state_methods.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/src/hyperdrive_utils.rs` & `hyperdrivepy-1.0.3/src/hyperdrive_utils.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/src/lib.rs` & `hyperdrivepy-1.0.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/src/pool_config.rs` & `hyperdrivepy-1.0.3/src/pool_config.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/src/pool_info.rs` & `hyperdrivepy-1.0.3/src/pool_info.rs`

 * *Files identical despite different names*

### Comparing `hyperdrivepy-1.0.2/src/utils.rs` & `hyperdrivepy-1.0.3/src/utils.rs`

 * *Files identical despite different names*

