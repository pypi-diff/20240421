# Comparing `tmp/pokerengine-1.1.5.tar.gz` & `tmp/pokerengine-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerengine-1.1.5.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pokerengine-1.1.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pokerengine-1.1.5.tar` & `pokerengine-1.1.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.clang-format
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.github/dependabot.yaml
--rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.gitignore
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 pokerengine-1.1.5/CMakeLists.txt
--rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.1.5/README.md
--rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.1.5/examples/hand_straight.py
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/bits.hpp
--rw-r--r--   0        0        0     7514 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/card/card.hpp
--rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/card/cards.hpp
--rw-r--r--   0        0        0     3206 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/card/hand.hpp
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/constants.hpp
--rw-r--r--   0        0        0    31475 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/engine.hpp
--rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/enums.hpp
--rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/evaluator/evaluation.hpp
--rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/evaluator/evaluation_result.hpp
--rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/evaluator/lookup_tables.hpp
--rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/evaluator/result.hpp
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/pokerengine.hpp
--rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pycard.hpp
--rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pyconstants.hpp
--rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pyengine.hpp
--rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pyenums.hpp
--rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/pyevaluation.hpp
--rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/python/python.hpp
--rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/string.hpp
--rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/types.hpp
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.1.5/include/pokerengine/vector.hpp
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.1.5/licenses/MIT
--rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/__init__.py
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/card.py
--rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/constants.py
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/engine.py
--rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/enums.py
--rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/evaluation.py
--rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/__init__.pyi
--rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/card.pyi
--rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/constants.pyi
--rw-r--r--   0        0        0     7863 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/engine.pyi
--rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/__init__.pyi
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/action.pyi
--rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/combination.pyi
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/position.pyi
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/rank.pyi
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/round.pyi
--rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/state.pyi
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/enums/suit.pyi
--rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/evaluation.pyi
--rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine/pokerengine_core/utils.pyi
--rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.1.5/src/pokerengine.cpp
--rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.1.6/.clang-format
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.1.6/.github/dependabot.yaml
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.1.6/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.1.6/.gitignore
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 pokerengine-1.1.6/CMakeLists.txt
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.1.6/README.md
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.1.6/examples/hand_straight.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/bits.hpp
+-rw-r--r--   0        0        0     7514 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/card/card.hpp
+-rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/card/cards.hpp
+-rw-r--r--   0        0        0     3364 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/card/hand.hpp
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/constants.hpp
+-rw-r--r--   0        0        0    31475 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/engine.hpp
+-rw-r--r--   0        0        0     3119 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/enums.hpp
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/evaluator/evaluation.hpp
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/evaluator/evaluation_result.hpp
+-rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/evaluator/lookup_tables.hpp
+-rw-r--r--   0        0        0     5387 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/evaluator/result.hpp
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/pokerengine.hpp
+-rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/python/pycard.hpp
+-rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/python/pyconstants.hpp
+-rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/python/pyengine.hpp
+-rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/python/pyenums.hpp
+-rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/python/pyevaluation.hpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/python/python.hpp
+-rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/string.hpp
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/types.hpp
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.1.6/include/pokerengine/vector.hpp
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.1.6/licenses/MIT
+-rw-r--r--   0        0        0     1190 2022-11-09 12:37:21.000000 pokerengine-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/__init__.py
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/card.py
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/constants.py
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/engine.py
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/enums.py
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/evaluation.py
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/__init__.pyi
+-rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/card.pyi
+-rw-r--r--   0        0        0      672 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/constants.pyi
+-rw-r--r--   0        0        0     7863 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/engine.pyi
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/enums/__init__.pyi
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/enums/action.pyi
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/enums/combination.pyi
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/enums/position.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/enums/rank.pyi
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/enums/round.pyi
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/enums/state.pyi
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/enums/suit.pyi
+-rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/evaluation.pyi
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine/pokerengine_core/utils.pyi
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.1.6/src/pokerengine.cpp
+-rw-r--r--   0        0        0      703 2022-11-09 12:37:21.000000 pokerengine-1.1.6/PKG-INFO
```

### Comparing `pokerengine-1.1.5/.clang-format` & `pokerengine-1.1.6/.clang-format`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/.github/workflows/pre-commit-updater.yml` & `pokerengine-1.1.6/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/.gitignore` & `pokerengine-1.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/.pre-commit-config.yaml` & `pokerengine-1.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/CMakeLists.txt` & `pokerengine-1.1.6/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.12)
 
-project(pokerengine VERSION 1.1.5)
+project(pokerengine VERSION 1.1.6)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 
 set(LIBRARY_NAME pokerengine_core)
```

### Comparing `pokerengine-1.1.5/examples/hand_straight.py` & `pokerengine-1.1.6/examples/hand_straight.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/bits.hpp` & `pokerengine-1.1.6/include/pokerengine/bits.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/card/card.hpp` & `pokerengine-1.1.6/include/pokerengine/card/card.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/card/cards.hpp` & `pokerengine-1.1.6/include/pokerengine/card/cards.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/card/hand.hpp` & `pokerengine-1.1.6/include/pokerengine/card/hand.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 //
-// Created by copper_boy on 7/4/23.
+// Created by copper_boy on 7/4/constants::HAND_SIZE3.
 //
 
 #ifndef POKERENGINE_HAND_HPP
 #define POKERENGINE_HAND_HPP
 
 #include <array>
 #include <compare>
 #include <cstdint>
 #include <stdexcept>
 #include <string>
 #include <type_traits>
 
 #include "card/card.hpp"
+#include "constants.hpp"
 #include "pokerengine.hpp"
 #include "types.hpp"
 
 namespace pokerengine {
 template < typename T >
 using is_card = std::is_same< T, typename pokerengine::card >;
 
@@ -34,39 +35,39 @@
 
 namespace v1 {
 template < typename T, bool allow_duplicates, size_t N, std::enable_if_t< is_card_or_rank_v< T >, int > = 0 >
 class hand_helper {
 public:
     hand_helper() = delete;
 
-    template < std::enable_if_t< N == 2, int > = 0 >
+    template < std::enable_if_t< N == constants::HAND_SIZE, int > = 0 >
     hand_helper(T first, T second) noexcept(allow_duplicates) : value_{ first, second } {
         if (!allow_duplicates &&
             (static_cast< card >(static_cast< card >(static_cast< card >(first))) == second)) {
             throw std::runtime_error{ "Tried to create hand with equal input" };
         }
     }
 
-    template < std::enable_if_t< is_card_v< T > && N == 2, int > = 0 >
+    template < std::enable_if_t< is_card_v< T > && N == constants::HAND_SIZE, int > = 0 >
     hand_helper(uint8_t first, uint8_t second) noexcept(allow_duplicates)
             : hand_helper{ T{ first }, T{ second } } {
     }
 
-    template < std::enable_if_t< N == 2, int > = 0 >
+    template < std::enable_if_t< N == constants::HAND_SIZE, int > = 0 >
     explicit hand_helper(std::string_view str)
             : hand_helper(T{ str.substr(0 * char_count, char_count) },
                           T{ str.substr(1 * char_count, char_count) }) {
-        if (str.size() != 2 * char_count) {
+        if (str.size() != constants::HAND_SIZE * char_count) {
             throw std::runtime_error{ "Tried to create a hand with a string of wrong size" };
         }
     }
 
     auto operator<=>(const hand_helper &other) const noexcept -> std::strong_ordering = default;
 
-    template < std::enable_if_t< N == 2, int > = 0 >
+    template < std::enable_if_t< N == constants::HAND_SIZE, int > = 0 >
     explicit operator std::string() const {
         auto iterable = get_value();
         return std::string{ iterable.front() } + std::string{ iterable.back() };
     }
 
     template < typename Indices = std::make_index_sequence< N > >
     [[nodiscard]] auto as_bitset() const noexcept -> types::bit_set {
@@ -94,11 +95,11 @@
         return static_cast< types::bit_set >((get_value()[I].as_bitset() | ...));
     }
 
     std::array< T, N > value_;
 };
 } // namespace v1
 
-using hand = actual::hand_helper< card, false, 2 >;
+using hand = actual::hand_helper< card, false, constants::HAND_SIZE >;
 } // namespace pokerengine
 
 #endif // POKERENGINE_HAND_HPP
```

### Comparing `pokerengine-1.1.5/include/pokerengine/constants.hpp` & `pokerengine-1.1.6/include/pokerengine/constants.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 const std::string CARDS_STRING =
                 "2c3c4c5c6c7c8c9cTcJcQcKcAc2d3d4d5d6d7d8d9dTdJdQdKdAd2h3h4h5h6h7h8h9hThJhQh"
                 "KhAh2s3s4s5s6s7s8s9sTsJsQsKsAs";
 
 const uint64_t CARD_SET_FULL = 0xFFFFFFFFFFFFFFFF >> (64 - DECK_SIZE);
 
 const uint8_t BOARD_SIZE = 5;
+const uint8_t HAND_SIZE = 2;
 
 const uint8_t MIN_PLAYERS = 2;
 const uint8_t MAX_PLAYERS = 7;
 
 template < size_t A = 0, size_t B = 1 >
     requires(A >= 0 && B > 0 && A < B)
 const float RAKE = 1.0f * A / B;
```

### Comparing `pokerengine-1.1.5/include/pokerengine/engine.hpp` & `pokerengine-1.1.6/include/pokerengine/engine.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/enums.hpp` & `pokerengine-1.1.6/include/pokerengine/enums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/evaluator/evaluation.hpp` & `pokerengine-1.1.6/include/pokerengine/evaluator/evaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/evaluator/evaluation_result.hpp` & `pokerengine-1.1.6/include/pokerengine/evaluator/evaluation_result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/evaluator/lookup_tables.hpp` & `pokerengine-1.1.6/include/pokerengine/evaluator/lookup_tables.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/evaluator/result.hpp` & `pokerengine-1.1.6/include/pokerengine/evaluator/result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/python/pycard.hpp` & `pokerengine-1.1.6/include/pokerengine/python/pycard.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/python/pyconstants.hpp` & `pokerengine-1.1.6/include/pokerengine/python/pyconstants.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     constants.attr("SUITS") = pokerengine::constants::SUITS;
     constants.attr("DECK_SIZE") = pokerengine::constants::DECK_SIZE;
     constants.attr("CARD_INDEX_MIN") = pokerengine::constants::CARD_INDEX_MIN;
     constants.attr("CARD_INDEX_MAX") = pokerengine::constants::CARD_INDEX_MAX;
     constants.attr("CARDS_STRING") = pokerengine::constants::CARDS_STRING;
     constants.attr("CARD_SET_FULL") = pokerengine::constants::CARD_SET_FULL;
     constants.attr("BOARD_SIZE") = pokerengine::constants::BOARD_SIZE;
+    constants.attr("HAND_SIZE") = pokerengine::constants::HAND_SIZE;
     constants.attr("MIN_PLAYERS") = pokerengine::constants::MIN_PLAYERS;
     constants.attr("MAX_PLAYERS") = pokerengine::constants::MAX_PLAYERS;
     constants.attr("RAKE01") = pokerengine::constants::RAKE< 0, 1 >;
     constants.attr("RAKE_MULTI01") = pokerengine::constants::RAKE_MULTI< 0, 1 >;
     constants.attr("OFFSET_MINOR") = pokerengine::constants::OFFSET_MINOR;
     constants.attr("OFFSET_MAJOR") = pokerengine::constants::OFFSET_MAJOR;
     constants.attr("OFFSET_TYPE") = pokerengine::constants::OFFSET_TYPE;
```

### Comparing `pokerengine-1.1.5/include/pokerengine/python/pyengine.hpp` & `pokerengine-1.1.6/include/pokerengine/python/pyengine.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/python/pyenums.hpp` & `pokerengine-1.1.6/include/pokerengine/python/pyenums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/python/pyevaluation.hpp` & `pokerengine-1.1.6/include/pokerengine/python/pyevaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/string.hpp` & `pokerengine-1.1.6/include/pokerengine/string.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/include/pokerengine/vector.hpp` & `pokerengine-1.1.6/include/pokerengine/vector.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/licenses/MIT` & `pokerengine-1.1.6/licenses/MIT`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/pyproject.toml` & `pokerengine-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core==0.6.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "pokerengine"
-version = "1.1.5"
+version = "1.1.6"
 description = "Poker Library"
 readme = "README.md"
 authors = [
     {name = "raindinners"}
 ]
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `pokerengine-1.1.5/src/pokerengine/constants.py` & `pokerengine-1.1.6/src/pokerengine/constants.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/src/pokerengine/enums.py` & `pokerengine-1.1.6/src/pokerengine/enums.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/src/pokerengine/pokerengine_core/card.pyi` & `pokerengine-1.1.6/src/pokerengine/pokerengine_core/card.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/src/pokerengine/pokerengine_core/constants.pyi` & `pokerengine-1.1.6/src/pokerengine/pokerengine_core/constants.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 SUITS: Final[int] = ...
 DECK_SIZE: Final[int] = ...
 CARD_INDEX_MIN: Final[int] = ...
 CARD_INDEX_MAX: Final[int] = ...
 CARDS_STRING: Final[str] = ...
 CARD_SET_FULL: Final[int] = ...
 BOARD_SIZE: Final[int] = ...
+HAND_SIZE: Final[int] = ...
 MIN_PLAYERS: Final[int] = ...
 MAX_PLAYERS: Final[int] = ...
 RAKE01: Final[float] = ...
 RAKE_MULTI01: Final[float] = ...
 OFFSET_MINOR: Final[int] = ...
 OFFSET_MAJOR: Final[int] = ...
 OFFSET_TYPE: Final[int] = ...
```

### Comparing `pokerengine-1.1.5/src/pokerengine/pokerengine_core/engine.pyi` & `pokerengine-1.1.6/src/pokerengine/pokerengine_core/engine.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/src/pokerengine/pokerengine_core/evaluation.pyi` & `pokerengine-1.1.6/src/pokerengine/pokerengine_core/evaluation.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/src/pokerengine.cpp` & `pokerengine-1.1.6/src/pokerengine.cpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.1.5/PKG-INFO` & `pokerengine-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerengine
-Version: 1.1.5
+Version: 1.1.6
 Summary: Poker Library
 Keywords: raindinners,engine,poker,texas,holdem,texas-holdem,texas_holdem,pybind11,scikit-build-core,fast,c++,magic_enum,stubs,python-stubs,python_stubs,pythonstubs,py-stubs,py_stubs,pystubs
 Author: raindinners
 Requires-Python: >=3.8
 Provides-Extra: dev
 Provides-Extra: build
 Requires-Dist: black~=23.10.0; extra == "dev"
```

