# Comparing `tmp/polars_candle-0.1.0.tar.gz` & `tmp/polars_candle-0.1.1.tar.gz`

## Comparing `polars_candle-0.1.0.tar` & `polars_candle-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 polars_candle-0.1.0/Cargo.toml
--rw-r--r--   0      501       20      864 2024-01-08 17:43:11.000000 polars_candle-0.1.0/.gitignore
--rw-r--r--   0      501       20      552 2024-01-09 17:36:18.000000 polars_candle-0.1.0/Makefile
--rw-r--r--   0      501       20     3228 2024-04-19 13:36:20.000000 polars_candle-0.1.0/README.md
--rw-r--r--   0      501       20       48 2024-04-02 11:10:49.000000 polars_candle-0.1.0/polars_candle/__init__.py
--rw-r--r--   0      501       20     1184 2024-04-19 12:18:58.000000 polars_candle-0.1.0/polars_candle/candle_ext.py
--rw-r--r--   0      501       20      215 2024-04-19 12:14:27.000000 polars_candle-0.1.0/src/build.rs
--rw-r--r--   0      501       20     2682 2024-04-19 12:18:11.000000 polars_candle-0.1.0/src/candle_ext/embed.rs
--rw-r--r--   0      501       20       11 2024-04-17 16:05:56.000000 polars_candle-0.1.0/src/candle_ext/mod.rs
--rw-r--r--   0      501       20      217 2024-04-19 12:14:27.000000 polars_candle-0.1.0/src/lib.rs
--rw-r--r--   0      501       20      850 2024-04-19 11:49:37.000000 polars_candle-0.1.0/tests/test_candle.py
--rw-r--r--   0      501       20    97628 2024-04-18 12:14:40.000000 polars_candle-0.1.0/Cargo.lock
--rw-r--r--   0      501       20      446 2024-04-18 13:40:05.000000 polars_candle-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 polars_candle-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      964 1970-01-01 00:00:00.000000 polars_candle-0.1.1/Cargo.toml
+-rw-r--r--   0      501       20      864 2024-01-08 17:43:11.000000 polars_candle-0.1.1/.gitignore
+-rw-r--r--   0      501       20      552 2024-01-09 17:36:18.000000 polars_candle-0.1.1/Makefile
+-rw-r--r--   0      501       20     3228 2024-04-19 13:36:20.000000 polars_candle-0.1.1/README.md
+-rw-r--r--   0      501       20       48 2024-04-02 11:10:49.000000 polars_candle-0.1.1/polars_candle/__init__.py
+-rw-r--r--   0      501       20     1327 2024-04-21 08:41:41.000000 polars_candle-0.1.1/polars_candle/candle_ext.py
+-rw-r--r--   0      501       20      215 2024-04-19 12:14:27.000000 polars_candle-0.1.1/src/build.rs
+-rw-r--r--   0      501       20     2809 2024-04-21 09:07:33.000000 polars_candle-0.1.1/src/candle_ext/embed.rs
+-rw-r--r--   0      501       20       11 2024-04-17 16:05:56.000000 polars_candle-0.1.1/src/candle_ext/mod.rs
+-rw-r--r--   0      501       20      217 2024-04-19 12:14:27.000000 polars_candle-0.1.1/src/lib.rs
+-rw-r--r--   0      501       20     1304 2024-04-21 08:42:19.000000 polars_candle-0.1.1/tests/test_candle.py
+-rw-r--r--   0      501       20    95069 2024-04-21 09:07:08.000000 polars_candle-0.1.1/Cargo.lock
+-rw-r--r--   0      501       20      445 2024-04-20 17:29:10.000000 polars_candle-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 polars_candle-0.1.1/PKG-INFO
```

### Comparing `polars_candle-0.1.0/.gitignore` & `polars_candle-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.0/Makefile` & `polars_candle-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.0/README.md` & `polars_candle-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.0/polars_candle/candle_ext.py` & `polars_candle-0.1.1/polars_candle/candle_ext.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,29 +26,31 @@
 	...     pl.col("text").candle.embed_text("bert-base-uncased")
 	... )
 	"""
 
 	def __init__(self, expr: pl.Expr) -> None:
 		self._expr = expr
 
-	def embed_text(self, model_repo: str) -> pl.Expr:
+	def embed_text(self, model_repo: str, pooling: Literal["max", "sum", "mean"] = "mean") -> pl.Expr:
 		"""
 		Embed text using a pre-trained model.
 
 		Parameters
 		----------
 		model_repo
 			The repository name of the text embedding model to use. E.g. "sentence-transformers/all-MiniLM-L6-v2".
+		pooling
+			The pooling strategy to use. One of "max", "sum", or "mean".
 
 		Returns
 		-------
 		Expr
 			An expression with the embedded text.
 		"""
 
 		return register_plugin_function(
 			plugin_path=Path(__file__).parent,
 			function_name="embed_text",
 			args=[self._expr],
-			kwargs={"model_repo": model_repo},
+			kwargs={"model_repo": model_repo, "pooling": pooling},
 			is_elementwise=True,
 		)
```

### Comparing `polars_candle-0.1.0/src/candle_ext/embed.rs` & `polars_candle-0.1.1/src/candle_ext/embed.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 // Needed for the `polars_expr` macro
 #![allow(clippy::unused_unit)]
 
-use glowrs::SentenceTransformer;
+use glowrs::{SentenceTransformer, PoolingStrategy};
 use polars::error::PolarsResult;
 use polars::prelude::*;
 use pyo3_polars::derive::polars_expr;
 use serde::Deserialize;
 
 // Output functions
 fn array_f32_output(_: &[Field]) -> PolarsResult<Field> {
     Ok(Field::new(
         "array_float",
         DataType::List(Box::new(DataType::Float32)),
     ))
 }
 
+
 #[derive(Deserialize)]
 pub struct EmbeddingKwargs {
     /// Huggingface model repository name
     pub model_repo: String,
+
+    /// Pooling strategy
+    pub pooling: PoolingStrategy,
 }
 
 #[polars_expr(output_type_func=array_f32_output)]
 pub fn embed_text(s: &[Series], kwargs: EmbeddingKwargs) -> PolarsResult<Series> {
     let ca = s[0].str()?;
     let name = ca.name();
     let len = ca.len();
 
     let model = SentenceTransformer::from_repo_string(&kwargs.model_repo)
-        .map_err(|e| polars_err!(ComputeError: "Failed to load model: {}", e))?;
+        .map_err(|e| polars_err!(ComputeError: "Failed to load model: {}", e))?
+        .with_pooling_strategy(kwargs.pooling);
 
     let sentences: Vec<Option<&str>> = ca.into_iter().collect();
 
     // Seperate sentences into those with Some and None
     let (some_sentences_idx, _): (Vec<_>, Vec<_>) = sentences
         .iter()
         .enumerate()
```

### Comparing `polars_candle-0.1.0/tests/test_candle.py` & `polars_candle-0.1.1/tests/test_candle.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,7 +25,24 @@
     )
     print(df)
     assert df["s_embedding"].dtype == pl.Array
 
     df = df.explode("s_embedding")
 
     assert df["s_embedding"].dtype == pl.Float32
+
+
+def test_pooling():
+    df = pl.DataFrame({"s": ["This is a sentence", "This is another sentence"]})
+
+    df = df.with_columns(
+        pl.col("s")
+        .candle.embed_text("Snowflake/snowflake-arctic-embed-xs", pooling="max")
+        .alias("s_embedding")
+    )
+    print(df)
+    assert df["s_embedding"].dtype == pl.Array
+
+    df = df.explode("s_embedding")
+
+    assert df["s_embedding"].dtype == pl.Float32
+    assert df["s_embedding"].max() > 0.0
```

### Comparing `polars_candle-0.1.0/Cargo.lock` & `polars_candle-0.1.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -63,62 +63,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "anstream"
-version = "0.6.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d664a92ecae85fd0a7392615844904654d1d5f5514837f471ddef4a057aba1b6"
-dependencies = [
- "anstyle",
- "anstyle-parse",
- "anstyle-query",
- "anstyle-wincon",
- "colorchoice",
- "utf8parse",
-]
-
-[[package]]
-name = "anstyle"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7079075b41f533b8c61d2a4d073c4676e1f8b249ff94a393b0595db304e0dd87"
-
-[[package]]
-name = "anstyle-parse"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
-dependencies = [
- "utf8parse",
-]
-
-[[package]]
-name = "anstyle-query"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
-dependencies = [
- "windows-sys 0.52.0",
-]
-
-[[package]]
-name = "anstyle-wincon"
-version = "3.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
-dependencies = [
- "anstyle",
- "windows-sys 0.52.0",
-]
-
-[[package]]
 name = "anyhow"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "080e9890a082662b09c1ad45f567faeeb47f22b5fb23895fbe1e651e718e25ca"
 
 [[package]]
 name = "argminmax"
@@ -384,60 +336,14 @@
 dependencies = [
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
-name = "clap"
-version = "4.4.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52bdc885e4cacc7f7c9eedc1ef6da641603180c783c41a15c264944deeaab642"
-dependencies = [
- "clap_builder",
- "clap_derive",
-]
-
-[[package]]
-name = "clap_builder"
-version = "4.4.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb7fb5e4e979aec3be7791562fcba452f94ad85e954da024396433e0e25a79e9"
-dependencies = [
- "anstream",
- "anstyle",
- "clap_lex",
- "strsim",
-]
-
-[[package]]
-name = "clap_derive"
-version = "4.4.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9804afaaf59a91e75b022a30fb7229a7901f60c755489cc61c9b423b836442"
-dependencies = [
- "heck",
- "proc-macro2",
- "quote",
- "syn 2.0.59",
-]
-
-[[package]]
-name = "clap_lex"
-version = "0.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "702fc72eb24e5a1e48ce58027a675bc24edd52096d5397d4aea7c6dd9eca0bd1"
-
-[[package]]
-name = "colorchoice"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
-
-[[package]]
 name = "comfy-table"
 version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c64043d6c7b7a4c58e39e7efccfdea7b93d885a795d0c054a69dbbf4dd52686"
 dependencies = [
  "crossterm",
  "strum",
@@ -580,76 +486,76 @@
 checksum = "9395df0cab995685664e79cc35ad6302bf08fb9c5d82301875a183affe1278b1"
 dependencies = [
  "half",
 ]
 
 [[package]]
 name = "darling"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 1.0.109",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.14.4"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "derive_builder"
-version = "0.12.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d67778784b508018359cbc8696edb3db78160bab2c2a28ba7f56ef6932997f8"
+checksum = "0350b5cb0331628a5916d6c5c0b72e97393b8b6b03b47a9284f4e7f5a405ffd7"
 dependencies = [
  "derive_builder_macro",
 ]
 
 [[package]]
 name = "derive_builder_core"
-version = "0.12.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c11bdc11a0c47bc7d37d582b5285da6849c96681023680b906673c5707af7b0f"
+checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "derive_builder_macro"
-version = "0.12.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ebcda35c7a396850a55ffeac740804b40ffec779b98fffbb1738f4033f0ee79e"
+checksum = "206868b8242f27cecce124c19fd88157fbd0dd334df2587f36417bafbc85097b"
 dependencies = [
  "derive_builder_core",
- "syn 1.0.109",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "dirs"
 version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44c45a9d03d6676652bcb5e724c7e988de1acad23a711b5217ab9cbecbec2225"
@@ -1082,17 +988,17 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "glowrs"
-version = "0.1.9"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56e3a2a7443ad4715abe87dd188f83bd497707901b2c34bf7a08021d7e856bc6"
+checksum = "2032d988976b786ca0949036bd97b1ae2bfa2c60318d9e93517ed19a8818ef0d"
 dependencies = [
  "anyhow",
  "candle-core",
  "candle-nn",
  "candle-transformers",
  "hf-hub",
  "once_cell",
@@ -1362,14 +1268,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "itoap"
@@ -2025,15 +1940,15 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-candle"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "anyhow",
  "chrono",
  "glowrs",
  "ndarray",
  "polars",
  "pyo3",
@@ -2561,15 +2476,15 @@
 [[package]]
 name = "rayon-cond"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "059f538b55efd2309c9794130bc149c6a553db90e9d99c2030785c82f0bd7df9"
 dependencies = [
  "either",
- "itertools",
+ "itertools 0.11.0",
  "rayon",
 ]
 
 [[package]]
 name = "rayon-core"
 version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2630,36 +2545,30 @@
 version = "1.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
- "regex-syntax 0.8.2",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.8.2",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb5fb1acd8a1a18b3dd5be62d25485eb770e05afb408a9627d14d451bae12da"
-
-[[package]]
-name = "regex-syntax"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
@@ -3207,36 +3116,35 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokenizers"
-version = "0.15.0"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "062b8a9613d6017633b80fb55fbb33f1aff006c36225a3025630753398034b3c"
+checksum = "e500fad1dd3af3d626327e6a3fe5050e664a6eaa4708b8ca92f1794aaf73e6fd"
 dependencies = [
  "aho-corasick",
- "clap",
  "derive_builder",
  "esaxx-rs",
  "getrandom",
  "indicatif",
- "itertools",
+ "itertools 0.12.1",
  "lazy_static",
  "log",
  "macro_rules_attribute",
  "monostate",
  "onig",
  "paste",
  "rand",
  "rayon",
  "rayon-cond",
  "regex",
- "regex-syntax 0.7.5",
+ "regex-syntax",
  "serde",
  "serde_json",
  "spm_precompiled",
  "thiserror",
  "unicode-normalization-alignments",
  "unicode-segmentation",
  "unicode_categories",
@@ -3439,20 +3347,14 @@
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
-name = "utf8parse"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
-
-[[package]]
 name = "uuid"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
 dependencies = [
  "getrandom",
 ]
```

### Comparing `polars_candle-0.1.0/PKG-INFO` & `polars_candle-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.3
 Name: polars_candle
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Summary: A text embedding extension for the Polars Dataframe library.
+Keywords: polars,dataframe,embedding,nlp,candle
 Author: Wouter Doppenberg <wouterdoppenberg@gmail.com>
 Author-email: Wouter Doppenberg <wouterdoppenberg@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # `polars-candle`
```

