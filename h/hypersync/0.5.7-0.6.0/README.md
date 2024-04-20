# Comparing `tmp/hypersync-0.5.7.tar.gz` & `tmp/hypersync-0.6.0.tar.gz`

## Comparing `hypersync-0.5.7.tar` & `hypersync-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 hypersync-0.5.7/Cargo.toml
--rw-r--r--   0     1001      127     2921 2024-03-27 15:15:06.000000 hypersync-0.5.7/.github/workflows/publish.yml
--rw-r--r--   0     1001      127      699 2024-03-27 15:15:06.000000 hypersync-0.5.7/.gitignore
--rw-r--r--   0     1001      127    16725 2024-03-27 15:15:06.000000 hypersync-0.5.7/LICENSE
--rw-r--r--   0     1001      127      137 2024-03-27 15:15:06.000000 hypersync-0.5.7/README.md
--rw-r--r--   0     1001      127     4840 2024-03-27 15:15:06.000000 hypersync-0.5.7/erc20.abi.json
--rw-r--r--   0     1001      127     3232 2024-03-27 15:15:06.000000 hypersync-0.5.7/examples/all-erc20.py
--rw-r--r--   0     1001      127     2694 2024-03-27 15:15:06.000000 hypersync-0.5.7/examples/top-usdt.py
--rw-r--r--   0     1001      127     5558 2024-03-27 15:15:06.000000 hypersync-0.5.7/examples/wallet.py
--rw-r--r--   0     1001      127     1906 2024-03-27 15:15:06.000000 hypersync-0.5.7/examples/watch.py
--rw-r--r--   0     1001      127     8434 2024-03-27 15:15:06.000000 hypersync-0.5.7/hypersync/__init__.py
--rw-r--r--   0     1001      127     2752 2024-03-27 15:15:06.000000 hypersync-0.5.7/src/config.rs
--rw-r--r--   0     1001      127     4241 2024-03-27 15:15:06.000000 hypersync-0.5.7/src/decode.rs
--rw-r--r--   0     1001      127    13229 2024-03-27 15:15:06.000000 hypersync-0.5.7/src/from_arrow.rs
--rw-r--r--   0     1001      127    20412 2024-03-27 15:15:06.000000 hypersync-0.5.7/src/lib.rs
--rw-r--r--   0     1001      127     7062 2024-03-27 15:15:06.000000 hypersync-0.5.7/src/query.rs
--rw-r--r--   0     1001      127     6949 2024-03-27 15:15:06.000000 hypersync-0.5.7/src/types.rs
--rw-r--r--   0     1001      127     9153 2024-03-27 15:15:06.000000 hypersync-0.5.7/test.py
--rw-r--r--   0     1001      127    82103 2024-03-27 15:15:06.000000 hypersync-0.5.7/Cargo.lock
--rw-r--r--   0     1001      127      561 2024-03-27 15:15:06.000000 hypersync-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 hypersync-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 hypersync-0.6.0/Cargo.toml
+-rw-r--r--   0     1001      127     2983 2024-04-20 23:46:42.000000 hypersync-0.6.0/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      699 2024-04-20 23:46:42.000000 hypersync-0.6.0/.gitignore
+-rw-r--r--   0     1001      127    16725 2024-04-20 23:46:42.000000 hypersync-0.6.0/LICENSE
+-rw-r--r--   0     1001      127      137 2024-04-20 23:46:42.000000 hypersync-0.6.0/README.md
+-rw-r--r--   0     1001      127     4840 2024-04-20 23:46:42.000000 hypersync-0.6.0/erc20.abi.json
+-rw-r--r--   0     1001      127     3232 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/all-erc20.py
+-rw-r--r--   0     1001      127      959 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/simple-blocks-and-transaction-hashes.py
+-rw-r--r--   0     1001      127      902 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/simple-blocks-and-transactions.py
+-rw-r--r--   0     1001      127     1201 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/simple-logs-of-event.py
+-rw-r--r--   0     1001      127      935 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/simple-logs.py
+-rw-r--r--   0     1001      127     2694 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/top-usdt.py
+-rw-r--r--   0     1001      127     5558 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/wallet.py
+-rw-r--r--   0     1001      127     1906 2024-04-20 23:46:42.000000 hypersync-0.6.0/examples/watch.py
+-rw-r--r--   0     1001      127     9132 2024-04-20 23:46:42.000000 hypersync-0.6.0/hypersync/__init__.py
+-rw-r--r--   0     1001      127     2752 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/config.rs
+-rw-r--r--   0     1001      127     4241 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/decode.rs
+-rw-r--r--   0     1001      127    13235 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/from_arrow.rs
+-rw-r--r--   0     1001      127    20356 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      127     7062 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/query.rs
+-rw-r--r--   0     1001      127     6949 2024-04-20 23:46:42.000000 hypersync-0.6.0/src/types.rs
+-rw-r--r--   0     1001      127     9152 2024-04-20 23:46:42.000000 hypersync-0.6.0/test.py
+-rw-r--r--   0     1001      127    82944 2024-04-20 23:46:42.000000 hypersync-0.6.0/Cargo.lock
+-rw-r--r--   0     1001      127      604 2024-04-20 23:46:42.000000 hypersync-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      671 1970-01-01 00:00:00.000000 hypersync-0.6.0/PKG-INFO
```

### Comparing `hypersync-0.5.7/Cargo.toml` & `hypersync-0.6.0/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "hypersync"
-version = "0.5.7"
+version = "0.6.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "hypersync"
 crate-type = ["cdylib"]
 
@@ -18,17 +18,21 @@
 serde_json = "1"
 serde = { version = "1", features = ["derive"] }
 
 alloy-json-abi = "0.6"
 alloy-dyn-abi = "0.6"
 alloy-primitives = "0.6"
 
-skar-client = "0.16.3"
-skar-net-types = "0.2"
-skar-format = "0.2"
+skar-client = "0.18"
+skar-net-types = "0.3"
+skar-format = "0.3"
 
 anyhow = "1"
-arrow2 = { version = "0.18" }
+polars-arrow = { version = "0.38" }
 prefix-hex = "0.7.1"
 env_logger = "0.11"
 itertools = "0.12.1"
-hex = "0.4.3"
+faster-hex = "0.9.0"
+
+[profile.no_lto]
+inherits = "release"
+lto = "off"
```

### Comparing `hypersync-0.5.7/.github/workflows/publish.yml` & `hypersync-0.6.0/.github/workflows/publish.yml`

 * *Files 15% similar despite different names*

```diff
@@ -23,18 +23,19 @@
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: x86_64
-          args: --release --out dist --find-interpreter
+          args: --skip-auditwheel --release --out dist --find-interpreter
           sccache: 'true'
-          manylinux: auto
-          before-script-linux: yum install -y capnproto capnproto-devel
+          container: 'off'
+          manylinux: 'manylinux2014'
+          before-script-linux: sudo apt-get install -y capnproto libcapnp-dev
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
   windows:
```

### Comparing `hypersync-0.5.7/.gitignore` & `hypersync-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/LICENSE` & `hypersync-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/erc20.abi.json` & `hypersync-0.6.0/erc20.abi.json`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/examples/all-erc20.py` & `hypersync-0.6.0/examples/all-erc20.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/examples/top-usdt.py` & `hypersync-0.6.0/examples/top-usdt.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/examples/wallet.py` & `hypersync-0.6.0/examples/wallet.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/examples/watch.py` & `hypersync-0.6.0/examples/watch.py`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/hypersync/__init__.py` & `hypersync-0.6.0/hypersync/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,23 @@
     EXTRA_DATA = 'extra_data'
     SIZE = 'size'
     GAS_LIMIT = 'gas_limit'
     GAS_USED = 'gas_used'
     TIMESTAMP = 'timestamp'
     UNCLES = 'uncles'
     BASE_FEE_PER_GAS = 'base_fee_per_gas'
+    BLOB_GAS_USED = 'blob_gas_used'
+    EXCESS_BLOB_GAS = 'excess_blob_gas'
+    PARENT_BEACON_BLOCK_ROOT = 'parent_beacon_block_root'
+    WITHDRAWALS_ROOT = 'withdrawals_root'
+    WITHDRAWALS = 'withdrawals'
+    L1_BLOCK_NUMBER = 'l1_block_number'
+    SEND_COUNT = 'send_count'
+    SEND_ROOT = 'send_root'
+    MIX_HASH = 'mix_hash'
 
 class TransactionField(StrEnum):
     BLOCK_HASH = 'block_hash'
     BLOCK_NUMBER = 'block_number'
     FROM = 'from'
     GAS = 'gas'
     GAS_PRICE = 'gas_price'
@@ -72,14 +81,23 @@
     GAS_USED = 'gas_used'
     CONTRACT_ADDRESS = 'contract_address'
     LOGS_BLOOM = 'logs_bloom'
     TYPE = 'type'
     ROOT = 'root'
     STATUS = 'status'
     SIGHASH = 'sighash'
+    TX_Y_PARITY = 'tx_y_parity'
+    TX_ACCESS_LIST = 'tx_access_list'
+    TX_L1_FEE = 'tx_l1_fee'
+    TX_L1_GAS_PRICE = 'tx_l1_gas_price'
+    TX_L1_GAS_USED = 'tx_l1_gas_used'
+    TX_L1_FEE_SCALAR = 'tx_l1_fee_scalar'
+    TX_GAS_USED_FOR_L1 = 'tx_gas_used_for_l1'
+    MAX_FEE_PER_BLOB_GAS = 'max_fee_per_blob_gas'
+    BLOB_VERSIONED_HASHES = 'blob_versioned_hashes'
 
 class LogField(StrEnum):
     REMOVED = 'removed'
     LOG_INDEX = 'log_index'
     TRANSACTION_INDEX = 'transaction_index'
     TRANSACTION_HASH = 'transaction_hash'
     BLOCK_HASH = 'block_hash'
```

### Comparing `hypersync-0.5.7/src/config.rs` & `hypersync-0.6.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/src/decode.rs` & `hypersync-0.6.0/src/decode.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/src/from_arrow.rs` & `hypersync-0.6.0/src/from_arrow.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use anyhow::Result;
-use arrow2::array::{BinaryArray, BooleanArray, UInt64Array, UInt8Array};
+use polars_arrow::array::{BinaryArray, BooleanArray, UInt64Array, UInt8Array};
 use skar_client::ArrowBatch;
 
 use crate::types::{Block, Log, Transaction};
 
 pub trait FromArrow: Sized {
     fn from_arrow(batch: &ArrowBatch) -> Result<Vec<Self>>;
 }
```

### Comparing `hypersync-0.5.7/src/lib.rs` & `hypersync-0.6.0/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     prelude::*,
 };
 use pyo3_asyncio::tokio::future_into_py;
 
 use std::{collections::BTreeMap, sync::Arc};
 
 use anyhow::{Context, Result};
-use arrow2::array::StructArray;
-use arrow2::datatypes::{DataType, Field};
-use arrow2::ffi;
+use polars_arrow::array::StructArray;
+use polars_arrow::datatypes::{ArrowDataType as DataType, Field};
+use polars_arrow::ffi;
 use skar_client::ArrowBatch;
 
 use from_arrow::FromArrow;
 
 mod config;
 mod decode;
 mod from_arrow;
@@ -297,34 +297,34 @@
                 .map_err(|e| PyValueError::new_err(format!("{:?}", e)))?;
         Ok(query.into_py(py))
     }
 }
 
 // helper function to decode hex string as address
 fn hex_str_address_to_byte_array(hex_str: &str) -> Result<[u8; 20], String> {
-    match hex::decode(hex_str) {
-        Ok(bytes) if bytes.len() == 20 => {
-            let mut array = [0u8; 20];
-            array.copy_from_slice(&bytes);
-            Ok(array)
-        }
-        Ok(_) => Err("Decoded hex does not fit into a 20-byte array.".into()),
+    if hex_str.len() != 40 {
+        return Err("address must be 40 hex characters".to_owned());
+    }
+
+    let mut dst = [0u8; 20];
+    match faster_hex::hex_decode(hex_str.as_bytes(), &mut dst) {
+        Ok(()) => Ok(dst),
         Err(e) => Err(format!("Failed to decode hex string: {}", e)),
     }
 }
 
 // helper function to decode hex string as topic0
 fn hex_str_topic0_to_byte_array(hex_str: &str) -> Result<[u8; 32], String> {
-    match hex::decode(hex_str) {
-        Ok(bytes) if bytes.len() == 32 => {
-            let mut array = [0u8; 32];
-            array.copy_from_slice(&bytes);
-            Ok(array)
-        }
-        Ok(_) => Err("Decoded hex does not fit into a 32-byte array.".into()),
+    if hex_str.len() != 64 {
+        return Err("topic0 must be 64 hex characters".to_owned());
+    }
+
+    let mut dst = [0u8; 32];
+    match faster_hex::hex_decode(hex_str.as_bytes(), &mut dst) {
+        Ok(()) => Ok(dst),
         Err(e) => Err(format!("Failed to decode hex string: {}", e)),
     }
 }
 
 #[pyclass]
 #[pyo3(get_all)]
 #[derive(Clone, Debug)]
```

### Comparing `hypersync-0.5.7/src/query.rs` & `hypersync-0.6.0/src/query.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/src/types.rs` & `hypersync-0.6.0/src/types.rs`

 * *Files identical despite different names*

### Comparing `hypersync-0.5.7/test.py` & `hypersync-0.6.0/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
             )
         )
         execution_time = (time.time() - start_time) * 1000
         total_time += execution_time
     avg_time = total_time / NUM_BENCHMARK_RUNS
     print(f"create_parquet_folder time: {format(execution_time, '.9f')}ms")
 
-
 async def test_send_req():
     client = hypersync.HypersyncClient()
     total_time = 0
     for _ in range(NUM_BENCHMARK_RUNS):
         start_time = time.time()
         res = await client.send_req(QUERY)
         execution_time = (time.time() - start_time) * 1000
```

### Comparing `hypersync-0.5.7/Cargo.lock` & `hypersync-0.6.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -51,28 +51,34 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
 dependencies = [
  "alloc-no-stdlib",
 ]
 
 [[package]]
+name = "allocator-api2"
+version = "0.2.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
+
+[[package]]
 name = "alloy-dyn-abi"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2919acdad13336bc5dc26b636cdd6892c2f27fb0d4a58320a00c2713cf6a4e9a"
 dependencies = [
  "alloy-json-abi",
  "alloy-primitives",
  "alloy-sol-type-parser",
  "alloy-sol-types",
  "const-hex",
  "itoa",
  "serde",
  "serde_json",
- "winnow 0.6.5",
+ "winnow 0.6.6",
 ]
 
 [[package]]
 name = "alloy-json-abi"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24ed0f2a6c3a1c947b4508522a53a190dba8f94dcd4e3e1a5af945a498e78f2f"
@@ -120,30 +126,30 @@
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86ec0a47740b20bc5613b8712d0d321d031c4efc58e9645af96085d5cccfc27"
 dependencies = [
  "const-hex",
  "dunce",
  "heck",
- "indexmap 2.2.5",
+ "indexmap",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
  "syn-solidity",
  "tiny-keccak",
 ]
 
 [[package]]
 name = "alloy-sol-type-parser"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0045cc89524e1451ccf33e8581355b6027ac7c6e494bb02959d4213ad0d8e91d"
 dependencies = [
- "winnow 0.6.5",
+ "winnow 0.6.6",
 ]
 
 [[package]]
 name = "alloy-sol-types"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad09ec5853fa700d12d778ad224dcdec636af424d29fad84fb9a2f16a5b0ef09"
@@ -200,17 +206,17 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.80"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "ark-ff"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b3235cc41ee7a12aaaf2c575a2ad7b46713a8a50bda2fc3b003a04845c05dd6"
 dependencies = [
@@ -344,56 +350,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 dependencies = [
  "serde",
 ]
 
 [[package]]
-name = "arrow-format"
-version = "0.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07884ea216994cdc32a2d5f8274a8bee979cfe90274b83f86f440866ee3132c7"
-dependencies = [
- "planus",
- "serde",
-]
-
-[[package]]
-name = "arrow2"
-version = "0.18.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "963fef509b757bcbbf9e5ffa23bcb345614d99f4f6f531f97417b27b8604d389"
-dependencies = [
- "ahash",
- "arrow-format",
- "base64",
- "bytemuck",
- "chrono",
- "dyn-clone",
- "either",
- "ethnum",
- "fallible-streaming-iterator",
- "foreign_vec",
- "futures",
- "getrandom",
- "hash_hasher",
- "hashbrown 0.14.3",
- "indexmap 1.9.3",
- "json-deserializer",
- "lexical-core",
- "lz4",
- "num-traits",
- "parquet2",
- "rustc_version 0.4.0",
- "simdutf8",
- "streaming-iterator",
- "zstd",
-]
-
-[[package]]
 name = "async-stream"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
 dependencies = [
  "async-stream-impl",
  "futures-core",
@@ -404,50 +368,56 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.77"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
+name = "atoi_simd"
+version = "0.15.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ae037714f313c1353189ead58ef9eec30a8e8dc101b2622d461418fd59e28a9"
+
+[[package]]
 name = "auto_impl"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c87f3f15e7794432337fc718554eaa4dc8f04c9677a950ffe366f20a162ae42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -491,17 +461,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
@@ -518,17 +488,17 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "brotli"
-version = "3.4.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "516074a47ef4bce09577a3b379392300159ce5b1ba2e501ff1c819950066100f"
+checksum = "d640d25bc63c50fb1f0b545ffd80207d2e10a4c965530809b40ba3386825c391"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
  "brotli-decompressor",
 ]
 
 [[package]]
@@ -539,64 +509,64 @@
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.3"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byte-slice-cast"
 version = "1.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3ac9f8b63eca6fd385229b3675f6cc0dc5c8a5c8a54a59d4f52ffd670d87b0c"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.3"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "965ab7eb5f8f97d2a083c799f3a1b994fc397b2fe2da5d1da1626ce15a39f2b1"
+checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "capnp"
-version = "0.19.2"
+version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4bfb7088540597aa9a835f445dae750aa0792f84d253c6cd515940486e98e00"
+checksum = "b11832e6fb7a695c4a63cc42bd97bd2cda7165cd850caf5aff9a3d0e617720ed"
 dependencies = [
  "embedded-io",
 ]
 
 [[package]]
 name = "capnpc"
 version = "0.19.0"
@@ -604,48 +574,49 @@
 checksum = "c75ba30e0f08582d53c2f3710cf4bb65ff562614b1ba86906d7391adffe189ec"
 dependencies = [
  "capnp",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.89"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0ba8f7aaa012f30d5b2861462f6708eccd49c3c39863fe083a308035f63d723"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.35"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaf5903dcbc0a39312feb77df2ff4c76387d591b9fc7b04a238dcf8bb62639a"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
 name = "const-hex"
-version = "1.11.1"
+version = "1.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efbd12d49ab0eaf8193ba9175e45f56bbc2e4b27d57b8cfe62aa47942a46b9a9"
+checksum = "5ba00838774b4ab0233e355d26710fbfc8327a05c017f6dc4873f876d1f79f78"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "hex",
  "proptest",
  "serde",
 ]
@@ -747,17 +718,17 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "der"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fffa369a668c8af7dbf8b5e56c9f744fbd399949ed171606040001947de40b1c"
+checksum = "f55bf8e7b65898637379c1b74eb1551107c8294ed26d855ceb9fd1a09cfc9bc0"
 dependencies = [
  "const-oid",
  "zeroize",
 ]
 
 [[package]]
 name = "derivative"
@@ -839,17 +810,17 @@
  "rfc6979",
  "signature",
  "spki",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "elliptic-curve"
 version = "0.13.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6043086bf7973472e0c7dff2142ea0b680d30e18d9cc40f267efbf222bd47"
 dependencies = [
@@ -870,17 +841,17 @@
 name = "embedded-io"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "edd0f118536f44f5ccd48bcb8b111bdc3de888b58c74639dfb034a357d0f206d"
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "env_filter"
 version = "0.1.0"
@@ -929,27 +900,33 @@
 [[package]]
 name = "fallible-streaming-iterator"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7360491ce676a36bf9bb3c56c1aa791658183a54d2744120f27285738d90465a"
 
 [[package]]
+name = "fast-float"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
+
+[[package]]
 name = "faster-hex"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2a2b11eda1d40935b26cf18f6833c526845ae8c41e58d09af6adeb6f0269183"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "fastrange-rs"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e90a1392cd6ec5ebe42ccaf251f2b7ba6be654c377f05c913f3898bfb2172512"
 
@@ -1075,15 +1052,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1121,17 +1098,17 @@
  "typenum",
  "version_check",
  "zeroize",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -1151,50 +1128,40 @@
  "ff",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.24"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap 2.2.5",
+ "indexmap",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
-name = "hash_hasher"
-version = "2.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
-
-[[package]]
-name = "hashbrown"
-version = "0.12.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
-
-[[package]]
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 dependencies = [
  "ahash",
+ "allocator-api2",
+ "rayon",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
@@ -1305,25 +1272,25 @@
  "rustls",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
 name = "hypersync"
-version = "0.5.7"
+version = "0.6.0"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-json-abi",
  "alloy-primitives",
  "anyhow",
- "arrow2",
  "dict_derive",
  "env_logger",
- "hex",
+ "faster-hex",
  "itertools 0.12.1",
+ "polars-arrow",
  "prefix-hex",
  "pyo3",
  "pyo3-asyncio",
  "serde",
  "serde_json",
  "skar-client",
  "skar-format",
@@ -1359,37 +1326,27 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
-dependencies = [
- "autocfg",
- "hashbrown 0.12.3",
-]
-
-[[package]]
-name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.3",
+ "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
@@ -1409,46 +1366,37 @@
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "json-deserializer"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f63b421e16eb4100beb677af56f0b4f3a4f08bab74ef2af079ce5bb92c2683f"
-dependencies = [
- "indexmap 1.9.3",
-]
-
-[[package]]
 name = "k256"
 version = "0.13.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "956ff9b67e26e1a6a866cb758f12c6f8746208489e3e4a4b5580802f2f0a587b"
 dependencies = [
  "cfg-if",
  "ecdsa",
@@ -1471,78 +1419,14 @@
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
-name = "lexical-core"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2cde5de06e8d4c2faabc400238f9ae1c74d5412d03a7bd067645ccbc47070e46"
-dependencies = [
- "lexical-parse-float",
- "lexical-parse-integer",
- "lexical-util",
- "lexical-write-float",
- "lexical-write-integer",
-]
-
-[[package]]
-name = "lexical-parse-float"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "683b3a5ebd0130b8fb52ba0bdc718cc56815b6a097e28ae5a6997d0ad17dc05f"
-dependencies = [
- "lexical-parse-integer",
- "lexical-util",
- "static_assertions",
-]
-
-[[package]]
-name = "lexical-parse-integer"
-version = "0.8.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d0994485ed0c312f6d965766754ea177d07f9c00c9b82a5ee62ed5b47945ee9"
-dependencies = [
- "lexical-util",
- "static_assertions",
-]
-
-[[package]]
-name = "lexical-util"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5255b9ff16ff898710eb9eb63cb39248ea8a5bb036bea8085b1a767ff6c4e3fc"
-dependencies = [
- "static_assertions",
-]
-
-[[package]]
-name = "lexical-write-float"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "accabaa1c4581f05a3923d1b4cfd124c329352288b7b9da09e766b0668116862"
-dependencies = [
- "lexical-util",
- "lexical-write-integer",
- "static_assertions",
-]
-
-[[package]]
-name = "lexical-write-integer"
-version = "0.8.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1b6f3d1f4422866b68192d62f77bc5c700bee84f3069f2469d7bc8c77852446"
-dependencies = [
- "lexical-util",
- "static_assertions",
-]
-
-[[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libm"
@@ -1590,23 +1474,23 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -1630,14 +1514,36 @@
 dependencies = [
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "multiversion"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4851161a11d3ad0bf9402d90ffc3967bf231768bfd7aeb61755ad06dbf1a142"
+dependencies = [
+ "multiversion-macros",
+ "target-features",
+]
+
+[[package]]
+name = "multiversion-macros"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "79a74ddee9e0c27d2578323c13905793e91622148f138ba29738f9dddb835e90"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "target-features",
+]
+
+[[package]]
 name = "num-bigint"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
 dependencies = [
  "autocfg",
  "num-integer",
@@ -1744,60 +1650,41 @@
 checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
 dependencies = [
  "async-trait",
  "futures",
 ]
 
 [[package]]
-name = "parquet2"
-version = "0.17.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "579fe5745f02cef3d5f236bfed216fd4693e49e4e920a13475c6132233283bce"
-dependencies = [
- "async-stream",
- "brotli",
- "flate2",
- "futures",
- "lz4",
- "parquet-format-safe",
- "seq-macro",
- "snap",
- "streaming-decompression",
- "xxhash-rust",
- "zstd",
-]
-
-[[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pest"
-version = "2.7.8"
+version = "2.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56f8023d0fb78c8e03784ea1c7f3fa36e68a723138990b8d5a47d916b651e7a8"
+checksum = "311fb059dee1a7b802f036316d790138c613a4e8b180c822e3925a662e9f0c95"
 dependencies = [
  "memchr",
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1823,14 +1710,128 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
+name = "polars-arrow"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "25197f40d71f82b2f79bb394f03e555d3cc1ce4db1dd052c28318721c71e96ad"
+dependencies = [
+ "ahash",
+ "atoi_simd",
+ "bytemuck",
+ "chrono",
+ "dyn-clone",
+ "either",
+ "ethnum",
+ "fast-float",
+ "foreign_vec",
+ "getrandom",
+ "hashbrown",
+ "itoa",
+ "lz4",
+ "multiversion",
+ "num-traits",
+ "polars-arrow-format",
+ "polars-error",
+ "polars-utils",
+ "ryu",
+ "simdutf8",
+ "streaming-iterator",
+ "strength_reduce",
+ "version_check",
+ "zstd",
+]
+
+[[package]]
+name = "polars-arrow-format"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b0ef2474af9396b19025b189d96e992311e6a47f90c53cd998b36c4c64b84c"
+dependencies = [
+ "planus",
+ "serde",
+]
+
+[[package]]
+name = "polars-compute"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c354515f73cdbbad03c2bf723fcd68e6825943b3ec503055abc8a8cb08ce46bb"
+dependencies = [
+ "bytemuck",
+ "either",
+ "num-traits",
+ "polars-arrow",
+ "polars-error",
+ "polars-utils",
+ "strength_reduce",
+ "version_check",
+]
+
+[[package]]
+name = "polars-error"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d66dd0ce51f8bd620eb8bd376502fe68a2b1a446d5433ecd2e75270b0755ce76"
+dependencies = [
+ "polars-arrow-format",
+ "simdutf8",
+ "thiserror",
+]
+
+[[package]]
+name = "polars-parquet"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8824ee00fbbe83d69553f2711014c50361238d210ed81a7a297695b7db97d42"
+dependencies = [
+ "ahash",
+ "async-stream",
+ "base64",
+ "brotli",
+ "ethnum",
+ "flate2",
+ "futures",
+ "lz4",
+ "num-traits",
+ "parquet-format-safe",
+ "polars-arrow",
+ "polars-error",
+ "polars-utils",
+ "seq-macro",
+ "simdutf8",
+ "snap",
+ "streaming-decompression",
+ "zstd",
+]
+
+[[package]]
+name = "polars-utils"
+version = "0.38.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "694656a7d2b0cd8f07660dbc8d0fb7a81066ff57a452264907531d805c1e58c4"
+dependencies = [
+ "ahash",
+ "bytemuck",
+ "hashbrown",
+ "indexmap",
+ "num-traits",
+ "once_cell",
+ "polars-error",
+ "raw-cpuid",
+ "rayon",
+ "smartstring",
+ "version_check",
+]
+
+[[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "ppv-lite86"
@@ -1890,30 +1891,30 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proptest"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31b476131c3c86cb68032fdc5cb6d5a1045e3e42d96b69fa599fd77701e1f5bf"
 dependencies = [
  "bit-set",
  "bit-vec",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "lazy_static",
  "num-traits",
  "rand",
  "rand_chacha",
  "rand_xorshift",
  "regex-syntax",
  "rusty-fork",
@@ -1978,41 +1979,41 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -2055,18 +2056,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d25bf25ec5ae4a3f1b92f929810509a2f53d7dca2f50b794ff57e3face536c8f"
 dependencies = [
  "rand_core",
 ]
 
 [[package]]
+name = "raw-cpuid"
+version = "11.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -2085,17 +2095,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -2108,23 +2118,23 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
-version = "0.11.24"
+version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6920094eb85afde5e4a138be3f2de8bbdf28000f0029e72c45025a56b042251"
+checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -2190,17 +2200,17 @@
 dependencies = [
  "bytes",
  "rustc-hex",
 ]
 
 [[package]]
 name = "ruint"
-version = "1.12.0"
+version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49b1d9521f889713d1221270fdd63370feca7e5c71a18745343402fa86e4f04f"
+checksum = "8f308135fef9fc398342da5472ce7c484529df23743fb7c734e0f3d472971e62"
 dependencies = [
  "alloy-rlp",
  "ark-ff 0.3.0",
  "ark-ff 0.4.2",
  "bytes",
  "fastrlp",
  "num-bigint",
@@ -2250,30 +2260,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver 1.0.22",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.21.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "7fecbfb7b1444f477b345853b1fce097a2c6fb637b2bfb87e6bc5db0f043fae4"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -2372,37 +2382,37 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2452,30 +2462,31 @@
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "skar-client"
-version = "0.16.3"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d8ae35edf67dd8b3f8c5e4c1f9e594b1c6e8f0b5cbd781cdc5cec1b5a10b47f"
+checksum = "a0ef43bae6c714fa1ed747532a809c9415328f7be7f054d3cf8ea9847b9cd057"
 dependencies = [
  "alloy-dyn-abi",
  "alloy-json-abi",
  "anyhow",
  "arrayvec",
- "arrow2",
  "capnp",
  "faster-hex",
  "fastrange-rs",
  "futures",
  "log",
  "num_cpus",
- "parquet2",
+ "polars-arrow",
+ "polars-compute",
+ "polars-parquet",
  "rand",
  "rayon",
  "reqwest",
  "ruint",
  "serde",
  "serde_json",
  "skar-format",
@@ -2485,62 +2496,73 @@
  "tokio-util",
  "url",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "skar-format"
-version = "0.2.2"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a248a5fd84f9bc6e477f634afe0d32336a157b7f5c69ffe805909468b7b3c66e"
+checksum = "ae433aec0a99f9c87ea22ed4e798d81a69229598a42cc8904bd36a2148131322"
 dependencies = [
  "arrayvec",
  "derive_more",
  "faster-hex",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "skar-net-types"
-version = "0.2.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e8c487850640607daecf59d5bea52d872e91b03d8ae482792847ec7d8ab3629"
+checksum = "e3596a4d186329574a82227cb84902ab18be31d023a2b1e2c8c0e8dacf7b4c74"
 dependencies = [
  "arrayvec",
  "capnp",
  "capnpc",
  "serde",
  "skar-format",
 ]
 
 [[package]]
 name = "skar-schema"
-version = "0.1.1"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e6ec948f32f41d3aed59d29b1c59156e362fefd35f0114532dee3c87723f548"
+checksum = "7b4ad11f8b8320e0eee209d0e95ddc6116ca456d41c07a5520ac2329bee65904"
 dependencies = [
  "anyhow",
- "arrow2",
+ "polars-arrow",
 ]
 
 [[package]]
 name = "slab"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
+
+[[package]]
+name = "smartstring"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
+dependencies = [
+ "autocfg",
+ "static_assertions",
+ "version_check",
+]
 
 [[package]]
 name = "snap"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b6b67fb9a61334225b5b790716f609cd58395f895b3fe8b328786812a40bc3b"
 
@@ -2588,14 +2610,20 @@
 [[package]]
 name = "streaming-iterator"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b2231b7c3057d5e4ad0156fb3dc807d900806020c5ffa3ee6ff2c8c76fb8520"
 
 [[package]]
+name = "strength_reduce"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
+
+[[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
@@ -2606,17 +2634,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2624,15 +2652,15 @@
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cb3d0961cd53c23ea94eeec56ba940f636f6394788976e9f16ca5ee0aca7464a"
 dependencies = [
  "paste",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
@@ -2661,14 +2689,20 @@
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
+name = "target-features"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c1bbb9f3c5c463a01705937a24fdabc5047929ac764b2d5b9cf681c1f5041ed5"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
@@ -2680,30 +2714,30 @@
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tiny-keccak"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
@@ -2724,17 +2758,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
@@ -2747,15 +2781,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
@@ -2787,15 +2821,15 @@
 
 [[package]]
 name = "toml_edit"
 version = "0.20.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "396e4d48bbb2b7554c944bde63101b5ae446cff6ec4a24227428f15eb72ef338"
 dependencies = [
- "indexmap 2.2.5",
+ "indexmap",
  "toml_datetime",
  "winnow 0.5.40",
 ]
 
 [[package]]
 name = "tower-service"
 version = "0.3.2"
@@ -2961,15 +2995,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2995,15 +3029,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -3037,15 +3071,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -3057,125 +3091,132 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winnow"
 version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dffa400e67ed5a4dd237983829e66475f0a4a26938c4b04c21baede6262215b8"
+checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
@@ -3214,15 +3255,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
@@ -3234,33 +3275,32 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.12.4"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a27595e173641171fc74a1232b7b1c7a7cb6e18222c11e9dfb9888fa424c53c"
+checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.6"
+version = "7.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee98ffd0b48ee95e6c5168188e44a54550b1564d9d530ee21d5f0eaed1069581"
+checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
 dependencies = [
- "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
 version = "2.0.9+zstd.1.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

### Comparing `hypersync-0.5.7/pyproject.toml` & `hypersync-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,7 +14,9 @@
     "Topic :: Database :: Front-Ends",
     "Topic :: Software Development :: Libraries",
 ]
 dynamic = ["version"]
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
+profile = "no_lto"
+skip-auditwheel = false
```

### Comparing `hypersync-0.5.7/PKG-INFO` & `hypersync-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hypersync
-Version: 0.5.7
+Version: 0.6.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: strenum >=0.4.15, <0.4.16
```

