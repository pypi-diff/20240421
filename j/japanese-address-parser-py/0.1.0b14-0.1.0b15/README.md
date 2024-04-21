# Comparing `tmp/japanese_address_parser_py-0.1.0b14.tar.gz` & `tmp/japanese_address_parser_py-0.1.0b15.tar.gz`

## Comparing `japanese_address_parser_py-0.1.0b14.tar` & `japanese_address_parser_py-0.1.0b15.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0     1001      127      749 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/Cargo.toml
--rw-r--r--   0     1001      127     1065 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/LICENSE
--rw-r--r--   0     1001      127     4410 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/api/city_master_api.rs
--rw-r--r--   0     1001      127     4915 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/api/prefecture_master_api.rs
--rw-r--r--   0     1001      127     2775 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/api.rs
--rw-r--r--   0     1001      127     1794 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/entity.rs
--rw-r--r--   0     1001      127     1326 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/err.rs
--rw-r--r--   0     1001      127       64 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/lib.rs
--rw-r--r--   0     1001      127     3131 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/adapter/orthographical_variant_adapter.rs
--rw-r--r--   0     1001      127     2794 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/adapter/vague_expression_adapter.rs
--rw-r--r--   0     1001      127       74 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/adapter.rs
--rw-r--r--   0     1001      127      570 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/filter/fullwidth_character.rs
--rw-r--r--   0     1001      127     7292 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/filter/invalid_town_name_format.rs
--rw-r--r--   0     1001      127     3393 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/filter/non_kanji_block_number.rs
--rw-r--r--   0     1001      127      162 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/filter.rs
--rw-r--r--   0     1001      127     3769 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/read_city.rs
--rw-r--r--   0     1001      127     2293 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/read_house_number.rs
--rw-r--r--   0     1001      127     1739 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/read_prefecture.rs
--rw-r--r--   0     1001      127     7124 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/read_town.rs
--rw-r--r--   0     1001      127     9275 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser.rs
--rw-r--r--   0     1001      127     3695 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/util/converter.rs
--rw-r--r--   0     1001      127     7165 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/util/sequence_matcher.rs
--rw-r--r--   0     1001      127       45 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/util.rs
--rw-r--r--   0     1001      127     2826 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/README.md
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b14/python/Cargo.toml
--rw-r--r--   0     1001      127     3282 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/python/README.md
--rw-r--r--   0     1001      127      823 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/python/japanese_address_parser_py.pyi
--rw-r--r--   0     1001      127     1426 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/python/src/lib.rs
--rw-r--r--   0     1001      127    35920 2024-04-20 11:50:29.000000 japanese_address_parser_py-0.1.0b14/Cargo.lock
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b14/Cargo.toml
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b14/pyproject.toml
--rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b14/PKG-INFO
+-rw-r--r--   0     1001      127      749 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/Cargo.toml
+-rw-r--r--   0     1001      127     1065 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/LICENSE
+-rw-r--r--   0     1001      127     4410 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/api/city_master_api.rs
+-rw-r--r--   0     1001      127     4915 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/api/prefecture_master_api.rs
+-rw-r--r--   0     1001      127     2775 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/api.rs
+-rw-r--r--   0     1001      127     1794 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/entity.rs
+-rw-r--r--   0     1001      127     1326 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/err.rs
+-rw-r--r--   0     1001      127       64 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/lib.rs
+-rw-r--r--   0     1001      127     3131 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/adapter/orthographical_variant_adapter.rs
+-rw-r--r--   0     1001      127     2794 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/adapter/vague_expression_adapter.rs
+-rw-r--r--   0     1001      127       74 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/adapter.rs
+-rw-r--r--   0     1001      127      570 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/filter/fullwidth_character.rs
+-rw-r--r--   0     1001      127     7292 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/filter/invalid_town_name_format.rs
+-rw-r--r--   0     1001      127     3393 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/filter/non_kanji_block_number.rs
+-rw-r--r--   0     1001      127      162 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/filter.rs
+-rw-r--r--   0     1001      127     3769 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/read_city.rs
+-rw-r--r--   0     1001      127     2293 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/read_house_number.rs
+-rw-r--r--   0     1001      127     1739 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/read_prefecture.rs
+-rw-r--r--   0     1001      127     7124 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser/read_town.rs
+-rw-r--r--   0     1001      127     9275 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/parser.rs
+-rw-r--r--   0     1001      127     3695 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/util/converter.rs
+-rw-r--r--   0     1001      127     8133 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/util/sequence_matcher.rs
+-rw-r--r--   0     1001      127       45 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/core/src/util.rs
+-rw-r--r--   0     1001      127     2826 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/README.md
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b15/python/Cargo.toml
+-rw-r--r--   0     1001      127     3282 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/python/README.md
+-rw-r--r--   0     1001      127      823 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/python/japanese_address_parser_py.pyi
+-rw-r--r--   0     1001      127     1426 2024-04-21 12:02:42.000000 japanese_address_parser_py-0.1.0b15/python/src/lib.rs
+-rw-r--r--   0     1001      127    35920 2024-04-21 12:02:46.000000 japanese_address_parser_py-0.1.0b15/Cargo.lock
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b15/Cargo.toml
+-rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b15/pyproject.toml
+-rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b15/PKG-INFO
```

### Comparing `japanese_address_parser_py-0.1.0b14/core/Cargo.toml` & `japanese_address_parser_py-0.1.0b15/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/LICENSE` & `japanese_address_parser_py-0.1.0b15/core/LICENSE`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/api/city_master_api.rs` & `japanese_address_parser_py-0.1.0b15/core/src/api/city_master_api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/api/prefecture_master_api.rs` & `japanese_address_parser_py-0.1.0b15/core/src/api/prefecture_master_api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/api.rs` & `japanese_address_parser_py-0.1.0b15/core/src/api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/entity.rs` & `japanese_address_parser_py-0.1.0b15/core/src/entity.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/err.rs` & `japanese_address_parser_py-0.1.0b15/core/src/err.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/adapter/orthographical_variant_adapter.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/adapter/orthographical_variant_adapter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/adapter/vague_expression_adapter.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/adapter/vague_expression_adapter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/filter/fullwidth_character.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/filter/fullwidth_character.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/filter/invalid_town_name_format.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/filter/invalid_town_name_format.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/filter/non_kanji_block_number.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/filter/non_kanji_block_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/read_city.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/read_city.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/read_house_number.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/read_house_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/read_prefecture.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/read_prefecture.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser/read_town.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser/read_town.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/parser.rs` & `japanese_address_parser_py-0.1.0b15/core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/util/converter.rs` & `japanese_address_parser_py-0.1.0b15/core/src/util/converter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/core/src/util/sequence_matcher.rs` & `japanese_address_parser_py-0.1.0b15/core/src/util/sequence_matcher.rs`

 * *Files 11% similar despite different names*

```diff
@@ -7,29 +7,23 @@
     MoreThanOneCandidateExist(Vec<String>),
     NoCandidateExist,
 }
 
 impl SequenceMatcher {
     pub fn get_most_similar_match(
         input: &str,
-        possibilities: &Vec<String>,
+        possibilities: &[String],
         threshold: Option<f64>,
     ) -> Result<String, Error> {
         let mut highest_similarity: f64 = 0.0;
         let mut highest_matches: Vec<String> = vec![];
-        let length_of_longest_possibility = possibilities.iter().map(|x| x.len()).max().unwrap();
+        let length_of_longest_possibility = Self::get_length_of_longest_one(possibilities).unwrap();
+        let input = Self::cut_text(input, length_of_longest_possibility);
         for possibility in possibilities {
-            let similarity = Self::evaluate_match_ratio(
-                possibility,
-                if input.len() > length_of_longest_possibility {
-                    input.get(0..length_of_longest_possibility).unwrap()
-                } else {
-                    input
-                },
-            );
+            let similarity = Self::evaluate_match_ratio(possibility, &input);
             if similarity >= highest_similarity {
                 if similarity > highest_similarity {
                     highest_matches.clear();
                 }
                 if threshold.is_none() || similarity > threshold.unwrap() {
                     highest_matches.push(possibility.clone());
                 }
@@ -39,28 +33,58 @@
         match &highest_matches.len() {
             0 => Err(Error::NoCandidateExist),
             1 => Ok(highest_matches.first().unwrap().clone()),
             _ => Err(Error::MoreThanOneCandidateExist(highest_matches)),
         }
     }
 
+    fn get_length_of_longest_one(text_list: &[String]) -> Option<usize> {
+        text_list.iter().map(|x| x.chars().count()).max()
+    }
+
+    fn cut_text(input: &str, length: usize) -> String {
+        if input.chars().count() > length {
+            input.chars().take(length).collect::<String>()
+        } else {
+            input.to_string()
+        }
+    }
+
     fn evaluate_match_ratio(left: &str, right: &str) -> f64 {
         if left == right {
             return 1.0;
         }
         lcs_seq::normalized_similarity(left.chars(), right.chars())
     }
 }
 
 #[cfg(test)]
 mod tests {
     use crate::util::sequence_matcher::Error::{MoreThanOneCandidateExist, NoCandidateExist};
     use crate::util::sequence_matcher::SequenceMatcher;
 
     #[test]
+    fn get_length_of_longest_one() {
+        assert_eq!(SequenceMatcher::get_length_of_longest_one(&vec![]), None);
+        assert_eq!(
+            SequenceMatcher::get_length_of_longest_one(&generate_city_name_list()),
+            Some(8)
+        );
+    }
+
+    #[test]
+    fn cut_text() {
+        let city_name = "南会津郡檜枝岐村";
+        assert_eq!(SequenceMatcher::cut_text(city_name, 0), "");
+        assert_eq!(SequenceMatcher::cut_text(city_name, 1), "南");
+        assert_eq!(SequenceMatcher::cut_text(city_name, 8), "南会津郡檜枝岐村");
+        assert_eq!(SequenceMatcher::cut_text(city_name, 9), "南会津郡檜枝岐村");
+    }
+
+    #[test]
     fn evaluate_match_ratio_一致度100() {
         assert_eq!(
             SequenceMatcher::evaluate_match_ratio("相馬郡新地町", "相馬郡新地町"),
             1.0
         );
     }
 
@@ -78,15 +102,66 @@
             SequenceMatcher::evaluate_match_ratio("相馬郡新地町", "福島市"),
             0.0
         );
     }
 
     #[test]
     fn get_most_similar_match() {
-        let possibilities = vec![
+        let possibilities = generate_city_name_list();
+        let result = SequenceMatcher::get_most_similar_match(
+            "西郷村大字熊倉字折口原40番地",
+            &possibilities,
+            None,
+        );
+        assert!(result.is_ok());
+        assert_eq!(result.unwrap(), "西白河郡西郷村");
+        let result = SequenceMatcher::get_most_similar_match(
+            "小野町大字小野新町字舘廻",
+            &possibilities,
+            None,
+        );
+        assert!(result.is_ok());
+        assert_eq!(result.unwrap(), "田村郡小野町");
+        let result = SequenceMatcher::get_most_similar_match(
+            "桑折町大字谷地字道下22番地7",
+            &possibilities,
+            None,
+        );
+        assert!(result.is_ok());
+        assert_eq!(result.unwrap(), "伊達郡桑折町");
+    }
+
+    #[test]
+    fn get_most_similar_match_類似度が同じものが複数ある場合() {
+        let possibilities = vec!["周智郡森町".to_string(), "茅部郡森町".to_string()];
+        assert_eq!(
+            SequenceMatcher::evaluate_match_ratio("森町", &possibilities[0]),
+            SequenceMatcher::evaluate_match_ratio("森町", &possibilities[1])
+        );
+        let result = SequenceMatcher::get_most_similar_match("森町", &possibilities, None);
+        assert!(result.is_err());
+        assert_eq!(
+            result.err().unwrap(),
+            MoreThanOneCandidateExist(vec!["周智郡森町".to_string(), "茅部郡森町".to_string()])
+        );
+    }
+
+    #[test]
+    fn get_most_similar_match_マッチ候補が一つもない場合() {
+        let result = SequenceMatcher::get_most_similar_match(
+            "上町",
+            &vec!["上村".to_string(), "下町".to_string()],
+            Some(0.9),
+        );
+        assert!(result.is_err());
+        assert_eq!(result.err().unwrap(), NoCandidateExist);
+    }
+
+    fn generate_city_name_list() -> Vec<String> {
+        vec![
             "福島市".to_string(),
             "会津若松市".to_string(),
             "郡山市".to_string(),
             "いわき市".to_string(),
             "白河市".to_string(),
             "須賀川市".to_string(),
             "喜多方市".to_string(),
@@ -138,57 +213,10 @@
             "双葉郡川内村".to_string(),
             "双葉郡大熊町".to_string(),
             "双葉郡双葉町".to_string(),
             "双葉郡浪江町".to_string(),
             "双葉郡葛尾村".to_string(),
             "相馬郡新地町".to_string(),
             "相馬郡飯舘村".to_string(),
-        ];
-        let result = SequenceMatcher::get_most_similar_match(
-            "西郷村大字熊倉字折口原40番地",
-            &possibilities,
-            None,
-        );
-        assert!(result.is_ok());
-        assert_eq!(result.unwrap(), "西白河郡西郷村");
-        let result = SequenceMatcher::get_most_similar_match(
-            "小野町大字小野新町字舘廻",
-            &possibilities,
-            None,
-        );
-        assert!(result.is_ok());
-        assert_eq!(result.unwrap(), "田村郡小野町");
-        let result = SequenceMatcher::get_most_similar_match(
-            "桑折町大字谷地字道下22番地7",
-            &possibilities,
-            None,
-        );
-        assert!(result.is_ok());
-        assert_eq!(result.unwrap(), "伊達郡桑折町");
-    }
-
-    #[test]
-    fn get_most_similar_match_類似度が同じものが複数ある場合() {
-        let possibilities = vec!["周智郡森町".to_string(), "茅部郡森町".to_string()];
-        assert_eq!(
-            SequenceMatcher::evaluate_match_ratio("森町", &possibilities[0]),
-            SequenceMatcher::evaluate_match_ratio("森町", &possibilities[1])
-        );
-        let result = SequenceMatcher::get_most_similar_match("森町", &possibilities, None);
-        assert!(result.is_err());
-        assert_eq!(
-            result.err().unwrap(),
-            MoreThanOneCandidateExist(vec!["周智郡森町".to_string(), "茅部郡森町".to_string()])
-        );
-    }
-
-    #[test]
-    fn get_most_similar_match_マッチ候補が一つもない場合() {
-        let result = SequenceMatcher::get_most_similar_match(
-            "上町",
-            &vec!["上村".to_string(), "下町".to_string()],
-            Some(0.9),
-        );
-        assert!(result.is_err());
-        assert_eq!(result.err().unwrap(), NoCandidateExist);
+        ]
     }
 }
```

### Comparing `japanese_address_parser_py-0.1.0b14/README.md` & `japanese_address_parser_py-0.1.0b15/README.md`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/python/README.md` & `japanese_address_parser_py-0.1.0b15/python/README.md`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/python/japanese_address_parser_py.pyi` & `japanese_address_parser_py-0.1.0b15/python/japanese_address_parser_py.pyi`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/python/src/lib.rs` & `japanese_address_parser_py-0.1.0b15/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b14/Cargo.lock` & `japanese_address_parser_py-0.1.0b15/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "japanese-address-parser"
-version = "0.1.0-beta.14"
+version = "0.1.0-beta.15"
 dependencies = [
  "itertools",
  "js-sys",
  "nom",
  "rapidfuzz",
  "regex",
  "reqwest",
@@ -613,15 +613,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python"
-version = "0.1.0-beta.14"
+version = "0.1.0-beta.15"
 dependencies = [
  "japanese-address-parser",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -943,15 +943,15 @@
  "quote",
  "syn",
  "test-case-core",
 ]
 
 [[package]]
 name = "tests"
-version = "0.1.0-beta.14"
+version = "0.1.0-beta.15"
 dependencies = [
  "csv",
  "japanese-address-parser",
  "serde",
  "tokio",
 ]
 
@@ -1120,15 +1120,15 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm"
-version = "0.1.0-beta.14"
+version = "0.1.0-beta.15"
 dependencies = [
  "console_error_panic_hook",
  "japanese-address-parser",
  "serde-wasm-bindgen",
  "wasm-bindgen",
  "wasm-bindgen-futures",
 ]
```

### Comparing `japanese_address_parser_py-0.1.0b14/PKG-INFO` & `japanese_address_parser_py-0.1.0b15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: japanese-address-parser-py
-Version: 0.1.0b14
+Version: 0.1.0b15
 Classifier: Topic :: Text Processing
 Classifier: Programming Language :: Rust
 Classifier: Typing :: Typed
 Summary: A Rust Library to parse japanese addresses.
 Keywords: converter,utility,geo,rust
 Author: Yuuki Toriyama <github@toriyama.dev>
 Author-email: Yuuki Toriyama <github@toriyama.dev>
```

