# Comparing `tmp/ninjabook-0.1.5.tar.gz` & `tmp/ninjabook-0.1.6.tar.gz`

## Comparing `ninjabook-0.1.5.tar` & `ninjabook-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 ninjabook-0.1.5/Cargo.toml
--rw-r--r--   0      501       20     2886 2024-04-16 19:47:29.000000 ninjabook-0.1.5/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-04-16 19:47:29.000000 ninjabook-0.1.5/.gitignore
--rw-r--r--   0      501       20    28312 2024-04-17 14:00:28.000000 ninjabook-0.1.5/src/lib.rs
--rw-r--r--   0      501       20     8348 2024-04-17 14:11:07.000000 ninjabook-0.1.5/Cargo.lock
--rw-r--r--   0      501       20      389 2024-04-16 20:58:00.000000 ninjabook-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 ninjabook-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 ninjabook-0.1.6/Cargo.toml
+-rw-r--r--   0      501       20     2886 2024-04-17 14:19:01.000000 ninjabook-0.1.6/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      686 2024-04-17 14:19:01.000000 ninjabook-0.1.6/.gitignore
+-rw-r--r--   0      501       20    29149 2024-04-21 16:08:01.000000 ninjabook-0.1.6/src/lib.rs
+-rw-r--r--   0      501       20     7860 2024-04-21 16:22:08.000000 ninjabook-0.1.6/Cargo.lock
+-rw-r--r--   0      501       20      389 2024-04-17 14:19:01.000000 ninjabook-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 ninjabook-0.1.6/PKG-INFO
```

### Comparing `ninjabook-0.1.5/Cargo.toml` & `ninjabook-0.1.6/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [package]
 name = "ninjabook"
-version = "0.1.5"
+version = "0.1.6"
 edition = "2021"
 summary = "A lightweight and high performance orderbook"
 homepage = "https://github.com/ninja-quant/ninjabook"
 repository = "https://github.com/ninja-quant/ninjabook"
 license = "MIT"
 categories = ["algorithms", "data-structures"]
 keywords = ["orderbook", "trading", "crypto", "hft"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ninjabook"
 crate-type = ["cdylib"]
 
 [dependencies]
-serde = "1.0.197"
 pyo3 = {version = "0.20.0", features = ["abi3-py38"]}
```

### Comparing `ninjabook-0.1.5/.github/workflows/CI.yml` & `ninjabook-0.1.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `ninjabook-0.1.5/.gitignore` & `ninjabook-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ninjabook-0.1.5/src/lib.rs` & `ninjabook-0.1.6/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,58 @@
             self.last_updated,
             self.last_sequence,
             self.inv_tick_size
         )
     }
 
     #[inline]
+    pub fn process_raw(
+        &mut self,
+        timestamp: u64,
+        seq: u64,
+        is_trade: bool,
+        is_buy: bool,
+        price: f64,
+        size: f64,
+    ) {
+        let event = Event {
+            timestamp,
+            seq,
+            is_trade,
+            is_buy,
+            price,
+            size,
+        };
+
+        self.process(event);
+    }
+
+    #[inline]
+    pub fn process_stream_bbo_raw(
+        &mut self,
+        timestamp: u64,
+        seq: u64,
+        is_trade: bool,
+        is_buy: bool,
+        price: f64,
+        size: f64,
+    ) -> Option<(Option<Level>, Option<Level>)> {
+        let event = Event {
+            timestamp,
+            seq,
+            is_trade,
+            is_buy,
+            price,
+            size,
+        };
+
+        self.process_stream_bbo(event)
+    }
+
+    #[inline]
     pub fn process(&mut self, event: Event) {
         if event.timestamp < self.last_updated || event.seq < self.last_sequence {
             return;
         }
 
         match event.is_trade {
             true => self.process_trade(event),
```

### Comparing `ninjabook-0.1.5/Cargo.lock` & `ninjabook-0.1.6/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,17 @@
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ninjabook"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "pyo3",
- "serde",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
@@ -193,34 +192,14 @@
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "serde"
-version = "1.0.197"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
-dependencies = [
- "serde_derive",
-]
-
-[[package]]
-name = "serde_derive"
-version = "1.0.197"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
```

