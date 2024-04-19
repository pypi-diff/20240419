# Comparing `tmp/pokerengine-1.0.tar.gz` & `tmp/pokerengine-1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pokerengine-1.0a0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pokerengine-1.0.tar` & `pokerengine-1.0a0.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 pokerengine-1.0/.clang-format
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pokerengine-1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pokerengine-1.0/CMakeLists.txt
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 pokerengine-1.0/test.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pokerengine-1.0/.github/dependabot.yaml
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pokerengine-1.0/.github/workflows/pre-commit-updater.yml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pokerengine-1.0/examples/hand_straight.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/bits.hpp
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/constants.hpp
--rw-r--r--   0        0        0    32014 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/engine.hpp
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/enums.hpp
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/pokerengine.hpp
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/string.hpp
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/types.hpp
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/vector.hpp
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/card/card.hpp
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/card/cards.hpp
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/card/hand.hpp
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/evaluator/evaluation.hpp
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/evaluator/evaluation_result.hpp
--rw-r--r--   0        0        0   136152 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/evaluator/lookup_tables.hpp
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/evaluator/result.hpp
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/python/pycard.hpp
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/python/pyconstants.hpp
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/python/pyengine.hpp
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/python/pyenums.hpp
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/python/pyevaluation.hpp
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pokerengine-1.0/include/pokerengine/python/python.hpp
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pokerengine-1.0/licenses/MIT
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine.cpp
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/card.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/constants.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/engine.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/enums.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/evaluation.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/__init__.pyi
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/card.pyi
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/constants.pyi
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/engine.pyi
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/evaluation.pyi
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/utils.pyi
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/enums/__init__.pyi
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/enums/action.pyi
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/enums/combination.pyi
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/enums/position.pyi
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/enums/rank.pyi
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/enums/round.pyi
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/enums/state.pyi
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pokerengine-1.0/src/pokerengine/pokerengine_core/enums/suit.pyi
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pokerengine-1.0/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pokerengine-1.0/README.md
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 pokerengine-1.0/pyproject.toml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pokerengine-1.0/PKG-INFO
+-rw-r--r--   0        0        0     3831 2022-11-09 12:37:21.000000 pokerengine-1.0a0/.clang-format
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 pokerengine-1.0a0/.github/dependabot.yaml
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 pokerengine-1.0a0/.github/workflows/pre-commit-updater.yml
+-rw-r--r--   0        0        0      578 2022-11-09 12:37:21.000000 pokerengine-1.0a0/.gitignore
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 pokerengine-1.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2007 2022-11-09 12:37:21.000000 pokerengine-1.0a0/CMakeLists.txt
+-rw-r--r--   0        0        0       33 2022-11-09 12:37:21.000000 pokerengine-1.0a0/README.md
+-rw-r--r--   0        0        0      970 2022-11-09 12:37:21.000000 pokerengine-1.0a0/examples/hand_straight.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/bits.hpp
+-rw-r--r--   0        0        0     7684 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/card/card.hpp
+-rw-r--r--   0        0        0     2663 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/card/cards.hpp
+-rw-r--r--   0        0        0     3223 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/card/hand.hpp
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/constants.hpp
+-rw-r--r--   0        0        0    31164 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/engine.hpp
+-rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/enums.hpp
+-rw-r--r--   0        0        0     4460 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/evaluator/evaluation.hpp
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/evaluator/evaluation_result.hpp
+-rw-r--r--   0        0        0   136152 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/evaluator/lookup_tables.hpp
+-rw-r--r--   0        0        0     5389 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/evaluator/result.hpp
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/pokerengine.hpp
+-rw-r--r--   0        0        0     8217 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/python/pycard.hpp
+-rw-r--r--   0        0        0     1856 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/python/pyconstants.hpp
+-rw-r--r--   0        0        0    11836 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/python/pyengine.hpp
+-rw-r--r--   0        0        0     5720 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/python/pyenums.hpp
+-rw-r--r--   0        0        0     2586 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/python/pyevaluation.hpp
+-rw-r--r--   0        0        0      240 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/python/python.hpp
+-rw-r--r--   0        0        0     1327 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/string.hpp
+-rw-r--r--   0        0        0      278 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/types.hpp
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 pokerengine-1.0a0/include/pokerengine/vector.hpp
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 pokerengine-1.0a0/licenses/MIT
+-rw-r--r--   0        0        0     1136 2022-11-09 12:37:21.000000 pokerengine-1.0a0/pyproject.toml
+-rw-r--r--   0        0        0      301 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/__init__.py
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/card.py
+-rw-r--r--   0        0        0      782 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/constants.py
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/engine.py
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/enums.py
+-rw-r--r--   0        0        0      253 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/evaluation.py
+-rw-r--r--   0        0        0      323 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/__init__.pyi
+-rw-r--r--   0        0        0     7462 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/card.pyi
+-rw-r--r--   0        0        0      644 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/constants.pyi
+-rw-r--r--   0        0        0     7789 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/engine.pyi
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/enums/__init__.pyi
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/enums/action.pyi
+-rw-r--r--   0        0        0      320 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/enums/combination.pyi
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/enums/position.pyi
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/enums/rank.pyi
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/enums/round.pyi
+-rw-r--r--   0        0        0      204 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/enums/state.pyi
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/enums/suit.pyi
+-rw-r--r--   0        0        0     2418 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/evaluation.pyi
+-rw-r--r--   0        0        0      149 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine/pokerengine_core/utils.pyi
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 pokerengine-1.0a0/src/pokerengine.cpp
+-rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 pokerengine-1.0a0/PKG-INFO
```

### Comparing `pokerengine-1.0/.clang-format` & `pokerengine-1.0a0/.clang-format`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/.pre-commit-config.yaml` & `pokerengine-1.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/CMakeLists.txt` & `pokerengine-1.0a0/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 cmake_minimum_required(VERSION 3.12)
 
-project(pokerengine VERSION 1.0)
+project(pokerengine VERSION 0.6)
 
 set(CMAKE_CXX_STANDARD 20)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS OFF)
 
 set(POKERENGINE_INCLUDE_DIR ${PROJECT_SOURCE_DIR}/include/pokerengine)
 set(POKERENGINE_SOURCE_DIR ${PROJECT_SOURCE_DIR}/src)
```

### Comparing `pokerengine-1.0/.github/workflows/pre-commit-updater.yml` & `pokerengine-1.0a0/.github/workflows/pre-commit-updater.yml`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/examples/hand_straight.py` & `pokerengine-1.0a0/examples/hand_straight.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/bits.hpp` & `pokerengine-1.0a0/include/pokerengine/bits.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/constants.hpp` & `pokerengine-1.0a0/include/pokerengine/constants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/engine.hpp` & `pokerengine-1.0a0/include/pokerengine/engine.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -441,19 +441,14 @@
 
 template < typename Engine >
 class actions_manager : public actual::engine_detail< Engine > {
 public:
     using actual::engine_detail< Engine >::engine_detail;
 
     [[nodiscard]] auto get_possible_actions() const -> std::vector< player_action > {
-        if (this->engine.round.get_round() == enums::round::none ||
-            this->engine.round.get_round() == enums::round::showdown) {
-            return std::vector<player_action>{};
-        }
-
         auto player = this->engine.positions.get_player();
         return actual::get_possible_actions(
                         this->engine.round.get_round(),
                         this->engine.positions.get_current(),
                         player.state,
                         player.is_left,
                         this->engine.get_engine_traits().get_bb_bet(),
@@ -532,27 +527,19 @@
     using actual::engine_detail< Engine >::engine_detail;
 
     [[nodiscard]] auto get_current() const noexcept -> enums::position {
         return current_;
     }
 
     [[nodiscard]] auto get_player() const -> player {
-        auto current = static_cast< int >(get_current());
-        auto blank_player = player(true, 0, 0, 0, 0, enums::state::none);
-        return (current && current < this->engine.players.get_players().size()) ?
-                        this->engine.players.get_player(current) :
-                        blank_player;
+        return this->engine.players.get_player(static_cast< int8_t >(get_current()));
     }
 
     [[nodiscard]] auto get_player() -> player & {
-        auto current = static_cast< int >(get_current());
-        auto blank_player = player(true, 0, 0, 0, 0, enums::state::none);
-        return (current && current < this->engine.players.get_players().size()) ?
-                        this->engine.players.get_player(current) :
-                        blank_player;
+        return this->engine.players.get_player(static_cast< int8_t >(get_current()));
     }
 
     [[nodiscard]] auto get_number_alive() const -> int {
         auto iterable = this->engine.players.get_players();
         return std::accumulate(
                         iterable.cbegin(), iterable.cend(), 0, [&](int value, auto const &element) -> int {
                             return element.state != enums::state::out ? value + 1 : value;
@@ -587,25 +574,25 @@
         current_ = position;
     }
 
     auto set_next_current() -> void {
         auto iterable_size = this->engine.players.get_players().size();
         do {
             set_current(static_cast< enums::position >(
-                            (static_cast< int >(get_current()) + 1) % iterable_size));
+                            (static_cast< uint8_t >(get_current()) + 1) % iterable_size));
         } while (get_player().state == enums::state::out || get_player().state == enums::state::allin);
     }
 
     auto set_next_round_player() -> void {
         set_current(enums::position::sb);
 
         auto iterable_size = this->engine.players.get_players().size();
         while (get_player().state == enums::state::out || get_player().state == enums::state::allin) {
             set_current(static_cast< enums::position >(
-                            (static_cast< int >(get_current()) + 1) % iterable_size));
+                            (static_cast< uint8_t >(get_current()) + 1) % iterable_size));
         }
     }
 
 private:
     enums::position current_{ enums::position::none };
 };
 
@@ -613,30 +600,24 @@
     requires(A >= 0 && B > 0 && A < B)
 class pot_manager : public actual::engine_detail< Engine > {
 public:
     using actual::engine_detail< Engine >::engine_detail;
 
     [[nodiscard]] auto get_highest_bet() const -> int32_t {
         auto iterable = this->engine.players.get_players();
-        auto max = std::max_element(
-                        iterable.cbegin(), iterable.cend(), [](const auto &lhs, const auto &rhs) -> bool {
-                            return lhs.front < rhs.front;
-                        });
-
-        return max == iterable.end() ? 0 : max->front;
+        return std::max_element(iterable.cbegin(), iterable.cend(), [](const auto &lhs, const auto &rhs) -> bool {
+                   return lhs.front < rhs.front;
+               })->front;
     }
 
     [[nodiscard]] auto get_round_highest_bet() const -> int32_t {
         auto iterable = this->engine.players.get_players();
-        auto max = std::max_element(
-                        iterable.cbegin(), iterable.cend(), [](const auto &lhs, const auto &rhs) -> bool {
-                            return lhs.round_bet < rhs.round_bet;
-                        });
-
-        return max == iterable.end() ? 0 : max->round_bet;
+        return std::max_element(iterable.cbegin(), iterable.cend(), [](const auto &lhs, const auto &rhs) -> bool {
+                   return lhs.round_bet < rhs.round_bet;
+               })->round_bet;
     }
 
     [[nodiscard]] auto pot() const noexcept -> int32_t {
         auto iterable = this->engine.players.get_players();
         std::vector< int32_t > chips_front;
         for (auto const &player : iterable) {
             chips_front.push_back(player.front);
```

### Comparing `pokerengine-1.0/include/pokerengine/enums.hpp` & `pokerengine-1.0a0/include/pokerengine/enums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/string.hpp` & `pokerengine-1.0a0/include/pokerengine/string.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/vector.hpp` & `pokerengine-1.0a0/include/pokerengine/vector.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/card/card.hpp` & `pokerengine-1.0a0/include/pokerengine/card/card.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/card/cards.hpp` & `pokerengine-1.0a0/include/pokerengine/card/cards.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/card/hand.hpp` & `pokerengine-1.0a0/include/pokerengine/card/hand.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/evaluator/evaluation.hpp` & `pokerengine-1.0a0/include/pokerengine/evaluator/evaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/evaluator/evaluation_result.hpp` & `pokerengine-1.0a0/include/pokerengine/evaluator/evaluation_result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/evaluator/lookup_tables.hpp` & `pokerengine-1.0a0/include/pokerengine/evaluator/lookup_tables.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/evaluator/result.hpp` & `pokerengine-1.0a0/include/pokerengine/evaluator/result.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/python/pycard.hpp` & `pokerengine-1.0a0/include/pokerengine/python/pycard.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/python/pyconstants.hpp` & `pokerengine-1.0a0/include/pokerengine/python/pyconstants.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/python/pyengine.hpp` & `pokerengine-1.0a0/include/pokerengine/python/pyengine.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/python/pyenums.hpp` & `pokerengine-1.0a0/include/pokerengine/python/pyenums.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/include/pokerengine/python/pyevaluation.hpp` & `pokerengine-1.0a0/include/pokerengine/python/pyevaluation.hpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/licenses/MIT` & `pokerengine-1.0a0/licenses/MIT`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/src/pokerengine.cpp` & `pokerengine-1.0a0/src/pokerengine.cpp`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/src/pokerengine/constants.py` & `pokerengine-1.0a0/src/pokerengine/constants.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/src/pokerengine/enums.py` & `pokerengine-1.0a0/src/pokerengine/enums.py`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/src/pokerengine/pokerengine_core/card.pyi` & `pokerengine-1.0a0/src/pokerengine/pokerengine_core/card.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/src/pokerengine/pokerengine_core/constants.pyi` & `pokerengine-1.0a0/src/pokerengine/pokerengine_core/constants.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/src/pokerengine/pokerengine_core/engine.pyi` & `pokerengine-1.0a0/src/pokerengine/pokerengine_core/engine.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -65,57 +65,57 @@
     bb_mult: int
     """Big blind multiplication, used in the formula: stack_to_join=bb_bet*bb_mult"""
     min_raise: int
     """Game minimal raise size."""
 
     def __init__(self, sb_bet: int, bb_bet: int, bb_mult: int) -> None: ...
 
-class EngineDetail: ...
+class _EngineDetail: ...
 
-class Engine:
+class _Engine:
     traits: EngineTraits
     def __init__(self, traits: EngineTraits) -> None: ...
     def load(
         self,
         traits: EngineTraits,
         players: List[Player],
         position: PositionE,
         round: RoundE,
         flop_dealt: bool,
     ) -> None: ...
     @property
-    def actions(self) -> Actions:
+    def actions(self) -> _Actions:
         """
         Use this method to get actions manager.
 
         :return: Actions manager
         """
     @property
-    def players(self) -> Players:
+    def players(self) -> _Players:
         """
         Use this method to get players manager.
 
         :return: Players manager
         """
     @property
-    def positions(self) -> Positions:
+    def positions(self) -> _Positions:
         """
         Use this method to get positions manager.
 
         :return: Positions manager
         """
     @property
-    def pot(self) -> Pot:
+    def pot(self) -> _Pot:
         """
         Use this method to get pot manager.
 
         :return: Pot manager
         """
     @property
-    def round(self) -> Round:
+    def round(self) -> _Round:
         """
         Use this method to get round manager.
 
         :return: Round manager
         """
     def start(self, new_game: bool = False) -> None:
         """
@@ -127,16 +127,16 @@
     def stop(self) -> None:
         """
         Use this method to stop game.
 
         :return: :class:`None`
         """
 
-class Actions(EngineDetail):
-    def __init__(self, engine: Engine) -> None: ...
+class _Actions(_EngineDetail):
+    def __init__(self, engine: _Engine) -> None: ...
     @property
     def actions(self) -> List[PlayerAction]:
         """
         Use this method to get possible actions for current player.
 
         :return: List of possible actions
         """
@@ -144,20 +144,20 @@
         """
         Use this method to execute player action.
 
         :param action: Action to execute
         :return: :class:`None`
         """
 
-class Players(EngineDetail):
+class _Players(_EngineDetail):
     """
     Game players manager.
     """
 
-    def __init__(self, engine: Engine) -> None: ...
+    def __init__(self, engine: _Engine) -> None: ...
     @property
     def players(self) -> List[Player]:
         """
         Use this method to get players.
 
         :return: Players
         """
@@ -186,22 +186,22 @@
         """
         Use this method to add player in the game.
 
         :param index: Player index
         :return: :class:`None`
         """
 
-class Positions(EngineDetail):
+class _Positions(_EngineDetail):
     """
     Game positions manager.
     """
 
     current: PositionE = PositionE.NONE
 
-    def __init__(self, engine: Engine) -> None: ...
+    def __init__(self, engine: _Engine) -> None: ...
     @property
     def number_alive(self) -> int:
         """
         Use this method to get number alive players.
 
         :return: Number alive
         """
@@ -241,20 +241,20 @@
     def set_next_round_player(self) -> None:
         """
         Use this method to set next player to small blind.
 
         :return: :class:`None`
         """
 
-class Pot(EngineDetail):
+class _Pot(_EngineDetail):
     """
     Game pot manager.
     """
 
-    def __init__(self, engine: Engine) -> None: ...
+    def __init__(self, engine: _Engine) -> None: ...
     @property
     def highest_bet(self) -> int:
         """
         Use this method to get the highest bet in the whole game.
 
         :return: Highest bet
         """
@@ -287,36 +287,36 @@
     def pot_rake(self) -> int:
         """
         Use this method to get game pot (rake adjusted).
 
         :return: Pot (rake adjusted)
         """
 
-class Round(EngineDetail):
+class _Round(_EngineDetail):
     """
     Game round manager.
     """
 
     flop_dealt: bool = False
     round: RoundE = RoundE.NONE
 
-    def __init__(self, engine: Engine) -> None: ...
+    def __init__(self, engine: _Engine) -> None: ...
     @property
     def showdown(self) -> bool:
         """
         Use this method to get is game is showdown.
 
         :return: Is game is showdown
         """
     def reset(self) -> None:
         """
         Use this method to reset round.
 
         :return: :class:`None`
         """
 
-class EngineRake01(Engine): ...
-class ActionsRake01(Actions): ...
-class PlayersRake01(Players): ...
-class PositionsRake01(Positions): ...
-class PotRake01(Pot): ...
-class RoundRake01(Round): ...
+class EngineRake01(_Engine): ...
+class ActionsRake01(_Actions): ...
+class PlayersRake01(_Players): ...
+class PositionsRake01(_Positions): ...
+class PotRake01(_Pot): ...
+class RoundRake01(_Round): ...
```

### Comparing `pokerengine-1.0/src/pokerengine/pokerengine_core/evaluation.pyi` & `pokerengine-1.0a0/src/pokerengine/pokerengine_core/evaluation.pyi`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/.gitignore` & `pokerengine-1.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `pokerengine-1.0/pyproject.toml` & `pokerengine-1.0a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["scikit-build-core", "pybind11"]
+requires = ["scikit-build-core>=0.6.1", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "pokerengine"
-version = "1.0"
+version = "1.0a"
 description = "Poker Library"
 readme = "README.md"
 authors = [
     {name = "raindinners"}
 ]
 requires-python = ">=3.8"
 keywords = [
@@ -37,22 +37,14 @@
 dev = [
     "black~=23.10.0",
     "isort~=5.12.0",
     "ruff~=0.1.1",
     "pre-commit~=3.5.0",
 ]
 
-build = [
-    "build~=1.2.1",
-    "twine~=5.0.0",
-]
-
-[tool.scikit-build]
-wheel.build-tag = "manylinux"
-
 [tool.ruff]
 line-length = 99
 select = [
     "C4",
     "E",
     "F",
     "T10",
```

### Comparing `pokerengine-1.0/PKG-INFO` & `pokerengine-1.0a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: pokerengine
-Version: 1.0
+Version: 1.0a0
 Summary: Poker Library
+Keywords: raindinners engine poker texas holdem texas-holdem texas_holdem pybind11 scikit-build-core fast c++ magic_enum stubs python-stubs python_stubs pythonstubs py-stubs py_stubs pystubs
 Author: raindinners
-Keywords: c++,engine,fast,holdem,magic_enum,poker,py-stubs,py_stubs,pybind11,pystubs,python-stubs,python_stubs,pythonstubs,raindinners,scikit-build-core,stubs,texas,texas-holdem,texas_holdem
 Requires-Python: >=3.8
-Provides-Extra: build
-Requires-Dist: build~=1.2.1; extra == 'build'
-Requires-Dist: twine~=5.0.0; extra == 'build'
 Provides-Extra: dev
-Requires-Dist: black~=23.10.0; extra == 'dev'
-Requires-Dist: isort~=5.12.0; extra == 'dev'
-Requires-Dist: pre-commit~=3.5.0; extra == 'dev'
-Requires-Dist: ruff~=0.1.1; extra == 'dev'
+Requires-Dist: black~=23.10.0; extra == "dev"
+Requires-Dist: isort~=5.12.0; extra == "dev"
+Requires-Dist: ruff~=0.1.1; extra == "dev"
+Requires-Dist: pre-commit~=3.5.0; extra == "dev"
 Description-Content-Type: text/markdown
 
 # pokerengine
 
 The poker engine.
```

