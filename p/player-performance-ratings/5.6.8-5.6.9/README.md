# Comparing `tmp/player-performance-ratings-5.6.8.tar.gz` & `tmp/player-performance-ratings-5.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "player-performance-ratings-5.6.8.tar", last modified: Tue Mar 26 20:47:39 2024, max compression
+gzip compressed data, was "player-performance-ratings-5.6.9.tar", last modified: Tue Mar 26 22:59:56 2024, max compression
```

## Comparing `player-performance-ratings-5.6.8.tar` & `player-performance-ratings-5.6.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.265840 player-performance-ratings-5.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-03-26 20:47:39.265840 player-performance-ratings-5.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.257840 player-performance-ratings-5.6.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.257840 player-performance-ratings-5.6.8/examples/lol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/examples/lol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.257840 player-performance-ratings-5.6.8/examples/lol/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/examples/lol/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/examples/lol/lol_match_predictor_tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.257840 player-performance-ratings-5.6.8/examples/nba/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/examples/nba/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.257840 player-performance-ratings-5.6.8/examples/nba/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/examples/nba/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/examples/nba/data/subsample_nba_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/examples/nba/nba_game_winner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.257840 player-performance-ratings-5.6.8/player_performance_ratings/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.257840 player-performance-ratings-5.6.8/player_performance_ratings/cross_validator/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/cross_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/cross_validator/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/cross_validator/cross_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    22694 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/pipeline_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/pipeline_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.261840 player-performance-ratings-5.6.8/player_performance_ratings/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/predictor/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/predictor/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/predictor/sklearn_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.261840 player-performance-ratings-5.6.8/player_performance_ratings/predictor_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/predictor_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/predictor_transformer/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.261840 player-performance-ratings-5.6.8/player_performance_ratings/ratings/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/league_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/match_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.261840 player-performance-ratings-5.6.8/player_performance_ratings/ratings/performance_generator/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/performance_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/performance_generator/performances_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/performance_generator/performances_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.261840 player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_calculators/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_calculators/match_rating_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_calculators/performance_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_calculators/start_rating_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/time_weight_ratings.py
--rw-r--r--   0 runner    (1001) docker     (127)    28779 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/ratings/update_rating_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.265840 player-performance-ratings-5.6.8/player_performance_ratings/scorer/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/scorer/score.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/transformation_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.265840 player-performance-ratings-5.6.8/player_performance_ratings/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12295 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/transformers/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25067 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/transformers/lag_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/transformers/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.265840 player-performance-ratings-5.6.8/player_performance_ratings/tuner/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/tuner/base_tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/tuner/performances_generator_tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/tuner/pipeline_tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/tuner/predictor_tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14536 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/tuner/rating_generator_tuner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/tuner/start_rating_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/tuner/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/player_performance_ratings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.265840 player-performance-ratings-5.6.8/player_performance_ratings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-03-26 20:47:39.000000 player-performance-ratings-5.6.8/player_performance_ratings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-03-26 20:47:39.000000 player-performance-ratings-5.6.8/player_performance_ratings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 20:47:39.000000 player-performance-ratings-5.6.8/player_performance_ratings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-26 20:47:39.000000 player-performance-ratings-5.6.8/player_performance_ratings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-26 20:47:39.000000 player-performance-ratings-5.6.8/player_performance_ratings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 20:47:39.265840 player-performance-ratings-5.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:47:39.265840 player-performance-ratings-5.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20379 2024-03-26 20:47:31.000000 player-performance-ratings-5.6.8/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.812931 player-performance-ratings-5.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-03-26 22:59:56.812931 player-performance-ratings-5.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.804931 player-performance-ratings-5.6.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.804931 player-performance-ratings-5.6.9/examples/lol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/examples/lol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.804931 player-performance-ratings-5.6.9/examples/lol/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/examples/lol/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/examples/lol/lol_match_predictor_tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.804931 player-performance-ratings-5.6.9/examples/nba/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/examples/nba/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.804931 player-performance-ratings-5.6.9/examples/nba/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/examples/nba/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/examples/nba/data/subsample_nba_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/examples/nba/nba_game_winner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.804931 player-performance-ratings-5.6.9/player_performance_ratings/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.808931 player-performance-ratings-5.6.9/player_performance_ratings/cross_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/cross_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/cross_validator/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/cross_validator/cross_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22694 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/pipeline_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/pipeline_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.808931 player-performance-ratings-5.6.9/player_performance_ratings/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/predictor/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/predictor/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/predictor/sklearn_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.808931 player-performance-ratings-5.6.9/player_performance_ratings/predictor_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/predictor_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/predictor_transformer/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.808931 player-performance-ratings-5.6.9/player_performance_ratings/ratings/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/league_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/match_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.808931 player-performance-ratings-5.6.9/player_performance_ratings/ratings/performance_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/performance_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/performance_generator/performances_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/performance_generator/performances_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.808931 player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_calculators/match_rating_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_calculators/performance_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_calculators/start_rating_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/time_weight_ratings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28779 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/ratings/update_rating_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.808931 player-performance-ratings-5.6.9/player_performance_ratings/scorer/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/scorer/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/transformation_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.812931 player-performance-ratings-5.6.9/player_performance_ratings/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12295 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/transformers/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24960 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/transformers/lag_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8575 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/transformers/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.812931 player-performance-ratings-5.6.9/player_performance_ratings/tuner/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/tuner/base_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/tuner/performances_generator_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12246 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/tuner/pipeline_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/tuner/predictor_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14536 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/tuner/rating_generator_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/tuner/start_rating_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/tuner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/player_performance_ratings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.812931 player-performance-ratings-5.6.9/player_performance_ratings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-03-26 22:59:56.000000 player-performance-ratings-5.6.9/player_performance_ratings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-03-26 22:59:56.000000 player-performance-ratings-5.6.9/player_performance_ratings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:59:56.000000 player-performance-ratings-5.6.9/player_performance_ratings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-26 22:59:56.000000 player-performance-ratings-5.6.9/player_performance_ratings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-26 22:59:56.000000 player-performance-ratings-5.6.9/player_performance_ratings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 22:59:56.812931 player-performance-ratings-5.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:59:56.812931 player-performance-ratings-5.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20379 2024-03-26 22:59:50.000000 player-performance-ratings-5.6.9/tests/test_pipeline.py
```

### Comparing `player-performance-ratings-5.6.8/LICENSE` & `player-performance-ratings-5.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/PKG-INFO` & `player-performance-ratings-5.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: player-performance-ratings
-Version: 5.6.8
+Version: 5.6.9
 Summary: Match Predictions based on Player Ratings
 Home-page: https://github.com/Hiderdk/player-performance-ratings
 Author: Mathias Holmstrøm
 Author-email: mathiasholmstom@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dataclasses_json>=0.6.1
```

### Comparing `player-performance-ratings-5.6.8/README.md` & `player-performance-ratings-5.6.9/README.md`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/examples/lol/lol_match_predictor_tuner.py` & `player-performance-ratings-5.6.9/examples/lol/lol_match_predictor_tuner.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/examples/nba/data/subsample_nba_data.py` & `player-performance-ratings-5.6.9/examples/nba/data/subsample_nba_data.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/examples/nba/nba_game_winner.py` & `player-performance-ratings-5.6.9/examples/nba/nba_game_winner.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/cross_validator/_base.py` & `player-performance-ratings-5.6.9/player_performance_ratings/cross_validator/_base.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/cross_validator/cross_validator.py` & `player-performance-ratings-5.6.9/player_performance_ratings/cross_validator/cross_validator.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/data_structures.py` & `player-performance-ratings-5.6.9/player_performance_ratings/data_structures.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/pipeline.py` & `player-performance-ratings-5.6.9/player_performance_ratings/pipeline.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/pipeline_factory.py` & `player-performance-ratings-5.6.9/player_performance_ratings/pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/predictor/_base.py` & `player-performance-ratings-5.6.9/player_performance_ratings/predictor/_base.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/predictor/predictor.py` & `player-performance-ratings-5.6.9/player_performance_ratings/predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/predictor/sklearn_estimator.py` & `player-performance-ratings-5.6.9/player_performance_ratings/predictor/sklearn_estimator.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/predictor_transformer/transformer.py` & `player-performance-ratings-5.6.9/player_performance_ratings/predictor_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/__init__.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/__init__.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/enums.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/enums.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/league_identifier.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/league_identifier.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/match_generator.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/match_generator.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/performance_generator/performances_generator.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/performance_generator/performances_generator.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/performance_generator/performances_transformers.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/performance_generator/performances_transformers.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_calculators/match_rating_generator.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_calculators/match_rating_generator.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_calculators/performance_predictor.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_calculators/performance_predictor.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_calculators/start_rating_generator.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_calculators/start_rating_generator.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/rating_generator.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/rating_generator.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/time_weight_ratings.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/time_weight_ratings.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/ratings/update_rating_generator.py` & `player-performance-ratings-5.6.9/player_performance_ratings/ratings/update_rating_generator.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/scorer/score.py` & `player-performance-ratings-5.6.9/player_performance_ratings/scorer/score.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/transformers/base_transformer.py` & `player-performance-ratings-5.6.9/player_performance_ratings/transformers/base_transformer.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/transformers/lag_generators.py` & `player-performance-ratings-5.6.9/player_performance_ratings/transformers/lag_generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,14 @@
         data = data.groupby(granularity + [game_id])[feature_name].sum().reset_index()
 
     else:
         data = data.groupby(granularity + [game_id])[feature_name].mean().reset_index()
     return data
 
 
-
-
-
 class LagTransformer(BaseLagGenerator):
 
     def __init__(self,
                  features: list[str],
                  lag_length: int,
                  granularity: Optional[list[str]] = None,
                  days_between_lags: Optional[list[int]] = None,
@@ -171,15 +168,15 @@
 
     def __init__(self,
                  features: list[str],
                  window: int,
                  granularity: Union[list[str], str] = None,
                  add_opponent: bool = False,
                  min_periods: int = 1,
-                 are_estimator_features=False,
+                 are_estimator_features=True,
                  prefix: str = 'rolling_mean_'):
         """
 
         :param features:
             Features to create rolling mean for
 
         :param granularity:
@@ -405,15 +402,14 @@
         self._fitted_game_ids = []
 
     @property
     def features_out(self) -> list[str]:
         return self._features_out
 
 
-
 class BinaryOutcomeRollingMeanTransformer(BaseLagGenerator):
 
     def __init__(self,
                  features: list[str],
                  window: int,
                  binary_column: str,
                  granularity: list[str] = None,
@@ -439,18 +435,16 @@
                 self._features_out.append(f'{self.prefix}{self.window}_{feature_name}_1_opponent')
                 self._features_out.append(f'{self.prefix}{self.window}_{feature_name}_0_opponent')
 
         if self.prob_column:
             for feature_name in self.features:
                 prob_feature = f'{self.prefix}{self.window}_{self.prob_column}_{feature_name}'
                 self._features_out.append(prob_feature)
-            #  self._entity_features.append(prob_feature)
 
-            #  if self.add_opponent:
-            #    self._features_out.append(f'{prob_feature}_opponent')
+        self._estimator_features_out = self._features_out.copy()
 
     def generate_historical(self, df: pd.DataFrame, column_names: ColumnNames) -> pd.DataFrame:
         self.column_names = column_names
         self.granularity = self.granularity or [self.column_names.player_id]
         validate_sorting(df=df, column_names=self.column_names)
         additional_cols_to_use = [self.binary_column] + ([self.prob_column] if self.prob_column else [])
         self._store_df(df, additional_cols_to_use=additional_cols_to_use)
@@ -492,15 +486,14 @@
                                                                   1 -
                                                                   transformed_df[
                                                                       self.prob_column])
         return transformed_df
 
     def _generate_concat_df_with_feats(self, df: pd.DataFrame) -> pd.DataFrame:
 
-
         additional_cols_to_use = [self.binary_column] + ([self.prob_column] if self.prob_column else [])
         concat_df = self._concat_df(df, additional_cols_to_use=additional_cols_to_use)
 
         for feature in self.features:
             mask_result_1 = concat_df[self.binary_column] == 1
             mask_result_0 = concat_df[self.binary_column] == 0
```

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/transformers/transformers.py` & `player-performance-ratings-5.6.9/player_performance_ratings/transformers/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,37 +40,40 @@
         if self._are_estimator_features:
             self._estimator_features_out.append(self.predictor.pred_column)
             self.features_out.append(self.predictor.pred_column)
         if self.prefix is "":
             raise ValueError("Prefix must not be empty")
 
     def fit_transform(self, df: pd.DataFrame, column_names: Optional[ColumnNames] = None) -> pd.DataFrame:
+        ori_cols = df.columns.tolist()
         self.column_names = column_names
         self.predictor.train(df, estimator_features=self.features)
-        if self.lag_generators:
-            df = self.predictor.add_prediction(df)
+        df = self.predictor.add_prediction(df)
+        new_feature_name = self.prefix + self.predictor.pred_column
+        if self.predictor.target not in df.columns:
+            df = df.assign(**{new_feature_name: np.nan})
+        else:
+            df = df.assign(**{new_feature_name: df[self.predictor.target] - df[self.predictor.pred_column]})
         for lag_generator in self.lag_generators:
             df = lag_generator.generate_historical(df, column_names=self.column_names)
-        return self.transform(df)
+        return df[list(set(ori_cols + self.features_out))]
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        ori_cols = df.columns.tolist()
         df = self.predictor.add_prediction(df)
         new_feature_name = self.prefix + self.predictor.pred_column
         if self.predictor.target not in df.columns:
             df = df.assign(**{new_feature_name: np.nan})
         else:
             df = df.assign(**{new_feature_name: df[self.predictor.target] - df[self.predictor.pred_column]})
 
         for lag_generator in self.lag_generators:
-            fitted_game_ids = lag_generator._df[self.column_names.match_id].unique()
-            if df[self.column_names.match_id].nunique() != len(
-                    fitted_game_ids) + df[self.column_names.match_id].nunique():
-                df = copy.deepcopy(lag_generator).generate_historical(df, column_names=self.column_names)
+            df = lag_generator.generate_future(df)
 
-        return df.drop(columns=[self.predictor.pred_column])
+        return df[list(set(ori_cols + self.features_out))]
 
     @property
     def features_out(self) -> list[str]:
         return self._features_out
 
     def reset(self) -> "BaseTransformer":
         for lag_generator in self.lag_generators:
@@ -163,15 +166,15 @@
         ori_cols = df.columns.tolist()
         self.column_names = column_names
         self.predictor.train(df=df, estimator_features=self.features)
         transformed_df = self.transform(df)
         for lag_generator in self.lag_generators:
             transformed_df = lag_generator.generate_historical(transformed_df, column_names=self.column_names)
 
-        return df[list(set(ori_cols + self.features_out))]
+        return transformed_df[list(set(ori_cols + self.features_out))]
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         df = self.predictor.add_prediction(df=df)
 
         df[self.predictor.pred_column + "_sum"] = df.groupby([self.column_names.match_id, self.column_names.team_id])[
             self.predictor.pred_column].transform('sum')
         df[self._features_out[0]] = df[self.predictor.pred_column] / df[self.predictor.pred_column + "_sum"]
```

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/tuner/performances_generator_tuner.py` & `player-performance-ratings-5.6.9/player_performance_ratings/tuner/performances_generator_tuner.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/tuner/pipeline_tuner.py` & `player-performance-ratings-5.6.9/player_performance_ratings/tuner/pipeline_tuner.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/tuner/predictor_tuner.py` & `player-performance-ratings-5.6.9/player_performance_ratings/tuner/predictor_tuner.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/tuner/rating_generator_tuner.py` & `player-performance-ratings-5.6.9/player_performance_ratings/tuner/rating_generator_tuner.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/tuner/start_rating_optimizer.py` & `player-performance-ratings-5.6.9/player_performance_ratings/tuner/start_rating_optimizer.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/tuner/utils.py` & `player-performance-ratings-5.6.9/player_performance_ratings/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings/utils.py` & `player-performance-ratings-5.6.9/player_performance_ratings/utils.py`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings.egg-info/PKG-INFO` & `player-performance-ratings-5.6.9/player_performance_ratings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: player-performance-ratings
-Version: 5.6.8
+Version: 5.6.9
 Summary: Match Predictions based on Player Ratings
 Home-page: https://github.com/Hiderdk/player-performance-ratings
 Author: Mathias Holmstrøm
 Author-email: mathiasholmstom@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dataclasses_json>=0.6.1
```

### Comparing `player-performance-ratings-5.6.8/player_performance_ratings.egg-info/SOURCES.txt` & `player-performance-ratings-5.6.9/player_performance_ratings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `player-performance-ratings-5.6.8/setup.py` & `player-performance-ratings-5.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="player-performance-ratings",
-    version="5.6.8",
+    version="5.6.9",
     packages=find_packages(),
     install_requires=required,
     author="Mathias Holmstrøm",
     author_email="mathiasholmstom@gmail.com",
     description="Match Predictions based on Player Ratings",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

### Comparing `player-performance-ratings-5.6.8/tests/test_pipeline.py` & `player-performance-ratings-5.6.9/tests/test_pipeline.py`

 * *Files identical despite different names*

