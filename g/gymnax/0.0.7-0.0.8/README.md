# Comparing `tmp/gymnax-0.0.7.tar.gz` & `tmp/gymnax-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymnax-0.0.7.tar", last modified: Thu Apr  4 15:40:55 2024, max compression
+gzip compressed data, was "gymnax-0.0.8.tar", last modified: Sun Apr 21 10:54:06 2024, max compression
```

## Comparing `gymnax-0.0.7.tar` & `gymnax-0.0.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.336283 gymnax-0.0.7/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10238 2024-04-04 15:40:47.000000 gymnax-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19372 2024-04-04 15:40:55.332283 gymnax-0.0.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    18596 2024-04-04 15:40:47.000000 gymnax-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.324283 gymnax-0.0.7/gymnax/
--rwxr-xr-x   0 runner    (1001) docker     (127)      342 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.324283 gymnax-0.0.7/gymnax/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.328283 gymnax-0.0.7/gymnax/environments/bsuite/
--rwxr-xr-x   0 runner    (1001) docker     (127)      776 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/bsuite/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3798 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/bsuite/bandit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6229 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/bsuite/catch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7851 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/bsuite/deep_sea.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4444 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/bsuite/discounting_chain.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5310 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/bsuite/memory_chain.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3956 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/bsuite/mnist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5175 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/bsuite/umbrella_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.328283 gymnax-0.0.7/gymnax/environments/classic_control/
--rwxr-xr-x   0 runner    (1001) docker     (127)      646 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/classic_control/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8712 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/classic_control/acrobot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6144 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/classic_control/cartpole.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5306 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/classic_control/continuous_mountain_car.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4740 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/classic_control/mountain_car.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5497 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/classic_control/pendulum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4405 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.328283 gymnax-0.0.7/gymnax/environments/minatar/
--rwxr-xr-x   0 runner    (1001) docker     (127)      586 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/minatar/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14187 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/minatar/asterix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10176 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/minatar/breakout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10901 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/minatar/freeway.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18195 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/minatar/seaquest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13461 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/minatar/space_invaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.328283 gymnax-0.0.7/gymnax/environments/misc/
--rwxr-xr-x   0 runner    (1001) docker     (127)      831 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/bernoulli_bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/gaussian_bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/meta_maze.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/point_robot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12694 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/pong.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/reacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/rooms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/misc/swimmer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5050 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/environments/spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.332283 gymnax-0.0.7/gymnax/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/experimental/rollout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5013 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.332283 gymnax-0.0.7/gymnax/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)      462 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/utils/load_mnist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10856 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/utils/state_translate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2706 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/utils/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.332283 gymnax-0.0.7/gymnax/visualize/
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/visualize/vis_catch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/visualize/vis_circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/visualize/vis_gym.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/visualize/vis_maze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/visualize/vis_minatar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.332283 gymnax-0.0.7/gymnax/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/wrappers/brax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/wrappers/dm_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/wrappers/evojax.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/wrappers/gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-04 15:40:47.000000 gymnax-0.0.7/gymnax/wrappers/purerl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.332283 gymnax-0.0.7/gymnax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19372 2024-04-04 15:40:55.000000 gymnax-0.0.7/gymnax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-04 15:40:55.000000 gymnax-0.0.7/gymnax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:40:55.000000 gymnax-0.0.7/gymnax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:40:55.000000 gymnax-0.0.7/gymnax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 15:40:55.000000 gymnax-0.0.7/gymnax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 15:40:55.000000 gymnax-0.0.7/gymnax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:40:55.336283 gymnax-0.0.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1843 2024-04-04 15:40:47.000000 gymnax-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:40:55.332283 gymnax-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-04 15:40:47.000000 gymnax-0.0.7/tests/test_visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.045250 gymnax-0.0.8/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10238 2024-04-21 10:53:58.000000 gymnax-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-04-21 10:54:06.045250 gymnax-0.0.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18596 2024-04-21 10:53:58.000000 gymnax-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.033250 gymnax-0.0.8/gymnax/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      342 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.033250 gymnax-0.0.8/gymnax/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.037250 gymnax-0.0.8/gymnax/environments/bsuite/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      776 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/bsuite/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3798 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/bsuite/bandit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6229 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/bsuite/catch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7851 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/bsuite/deep_sea.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4444 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/bsuite/discounting_chain.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5310 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/bsuite/memory_chain.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3956 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/bsuite/mnist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5175 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/bsuite/umbrella_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.037250 gymnax-0.0.8/gymnax/environments/classic_control/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      646 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/classic_control/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8712 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/classic_control/acrobot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6144 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/classic_control/cartpole.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5306 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/classic_control/continuous_mountain_car.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4740 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/classic_control/mountain_car.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5497 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/classic_control/pendulum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4405 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.037250 gymnax-0.0.8/gymnax/environments/minatar/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      586 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/minatar/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14187 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/minatar/asterix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10176 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/minatar/breakout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10901 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/minatar/freeway.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18195 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/minatar/seaquest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13461 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/minatar/space_invaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.041250 gymnax-0.0.8/gymnax/environments/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      831 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5332 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/bernoulli_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/gaussian_bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/meta_maze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/point_robot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12694 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/pong.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/reacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/rooms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/misc/swimmer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5050 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/environments/spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.041250 gymnax-0.0.8/gymnax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/experimental/rollout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5013 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.041250 gymnax-0.0.8/gymnax/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      462 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/utils/load_mnist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10856 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/utils/state_translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2706 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/utils/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.041250 gymnax-0.0.8/gymnax/visualize/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/visualize/vis_catch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/visualize/vis_circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/visualize/vis_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/visualize/vis_maze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/visualize/vis_minatar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.041250 gymnax-0.0.8/gymnax/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/wrappers/brax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/wrappers/dm_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/wrappers/evojax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/wrappers/gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-21 10:53:58.000000 gymnax-0.0.8/gymnax/wrappers/purerl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.041250 gymnax-0.0.8/gymnax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-04-21 10:54:05.000000 gymnax-0.0.8/gymnax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-21 10:54:06.000000 gymnax-0.0.8/gymnax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:54:05.000000 gymnax-0.0.8/gymnax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:54:05.000000 gymnax-0.0.8/gymnax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-21 10:54:05.000000 gymnax-0.0.8/gymnax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 10:54:05.000000 gymnax-0.0.8/gymnax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:54:06.045250 gymnax-0.0.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1907 2024-04-21 10:53:58.000000 gymnax-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:54:06.041250 gymnax-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-21 10:53:58.000000 gymnax-0.0.8/tests/test_visualizer.py
```

### Comparing `gymnax-0.0.7/LICENSE` & `gymnax-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/PKG-INFO` & `gymnax-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gymnax
-Version: 0.0.7
+Version: 0.0.8
 Summary: JAX-compatible version of Open AI's gym environments
 Home-page: https://github.com/RobertTLange/gymnax
-Download-URL: https://github.com/RobertTLange/gymnax/archive/v0.0.7.tar.gz
+Download-URL: https://github.com/RobertTLange/gymnax/archive/v0.0.8.tar.gz
 Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -17,14 +17,16 @@
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: chex
 Requires-Dist: flax
 Requires-Dist: pyyaml
 Requires-Dist: gym>=0.26
 Requires-Dist: gymnasium
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
 
 <h1 align="center">
   <a href="https://github.com/RobertTLange/gymnax/blob/main/docs/logo.png">
     <img src="https://github.com/RobertTLange/gymnax/blob/main/docs/logo.png?raw=true" width="215" /></a><br>
   <b>Reinforcement Learning Environments in JAX 🌍</b><br>
 </h1>
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: gymnax Version: 0.0.7 Summary: JAX-compatible
+Metadata-Version: 2.1 Name: gymnax Version: 0.0.8 Summary: JAX-compatible
 version of Open AI's gym environments Home-page: https://github.com/
 RobertTLange/gymnax Download-URL: https://github.com/RobertTLange/gymnax/
-archive/v0.0.7.tar.gz Author: Robert Tjarko Lange Author-email:
+archive/v0.0.8.tar.gz Author: Robert Tjarko Lange Author-email:
 robertlange0@gmail.com Platform: any Classifier: Programming Language :: Python
 :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
 :: Artificial Intelligence Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: jax Requires-Dist: jaxlib
 Requires-Dist: chex Requires-Dist: flax Requires-Dist: pyyaml Requires-Dist:
-gym>=0.26 Requires-Dist: gymnasium
+gym>=0.26 Requires-Dist: gymnasium Requires-Dist: matplotlib Requires-Dist:
+seaborn
         ************ _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_RR_oo_bb_ee_rr_tt_TT_LL_aa_nn_gg_ee_//_gg_yy_mm_nn_aa_xx_//_bb_ll_oo_bb_//_mm_aa_ii_nn_//_dd_oo_cc_ss_//
                               _ll_oo_gg_oo_.._pp_nn_gg_??_rr_aa_ww_==_tt_rr_uu_ee_]]
                 RReeiinnffoorrcceemmeenntt LLeeaarrnniinngg EEnnvviirroonnmmeennttss iinn JJAAXX ?ð???
                                      ************
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_g_y_m_n_a_x_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/
  _b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_g_y_m_n_a_x_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_A_p_a_c_h_e_2_._0_-
     _b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_R_o_b_e_r_t_T_L_a_n_g_e_/_g_y_m_n_a_x_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
```

### Comparing `gymnax-0.0.7/README.md` & `gymnax-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/__init__.py` & `gymnax-0.0.8/gymnax/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/bsuite/__init__.py` & `gymnax-0.0.8/gymnax/environments/bsuite/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/bsuite/bandit.py` & `gymnax-0.0.8/gymnax/environments/bsuite/bandit.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/bsuite/catch.py` & `gymnax-0.0.8/gymnax/environments/bsuite/catch.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/bsuite/deep_sea.py` & `gymnax-0.0.8/gymnax/environments/bsuite/deep_sea.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/bsuite/discounting_chain.py` & `gymnax-0.0.8/gymnax/environments/bsuite/discounting_chain.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/bsuite/memory_chain.py` & `gymnax-0.0.8/gymnax/environments/bsuite/memory_chain.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/bsuite/mnist.py` & `gymnax-0.0.8/gymnax/environments/bsuite/mnist.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/bsuite/umbrella_chain.py` & `gymnax-0.0.8/gymnax/environments/bsuite/umbrella_chain.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/classic_control/__init__.py` & `gymnax-0.0.8/gymnax/environments/classic_control/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/classic_control/acrobot.py` & `gymnax-0.0.8/gymnax/environments/classic_control/acrobot.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/classic_control/cartpole.py` & `gymnax-0.0.8/gymnax/environments/classic_control/cartpole.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/classic_control/continuous_mountain_car.py` & `gymnax-0.0.8/gymnax/environments/classic_control/continuous_mountain_car.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/classic_control/mountain_car.py` & `gymnax-0.0.8/gymnax/environments/classic_control/mountain_car.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/classic_control/pendulum.py` & `gymnax-0.0.8/gymnax/environments/classic_control/pendulum.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/environment.py` & `gymnax-0.0.8/gymnax/environments/environment.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/minatar/__init__.py` & `gymnax-0.0.8/gymnax/environments/minatar/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/minatar/asterix.py` & `gymnax-0.0.8/gymnax/environments/minatar/asterix.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/minatar/breakout.py` & `gymnax-0.0.8/gymnax/environments/minatar/breakout.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/minatar/freeway.py` & `gymnax-0.0.8/gymnax/environments/minatar/freeway.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/minatar/seaquest.py` & `gymnax-0.0.8/gymnax/environments/minatar/seaquest.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/minatar/space_invaders.py` & `gymnax-0.0.8/gymnax/environments/minatar/space_invaders.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/__init__.py` & `gymnax-0.0.8/gymnax/environments/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/bernoulli_bandit.py` & `gymnax-0.0.8/gymnax/environments/misc/bernoulli_bandit.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/gaussian_bandit.py` & `gymnax-0.0.8/gymnax/environments/misc/gaussian_bandit.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/meta_maze.py` & `gymnax-0.0.8/gymnax/environments/misc/meta_maze.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/point_robot.py` & `gymnax-0.0.8/gymnax/environments/misc/point_robot.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/pong.py` & `gymnax-0.0.8/gymnax/environments/misc/pong.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/reacher.py` & `gymnax-0.0.8/gymnax/environments/misc/reacher.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/rooms.py` & `gymnax-0.0.8/gymnax/environments/misc/rooms.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/misc/swimmer.py` & `gymnax-0.0.8/gymnax/environments/misc/swimmer.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/environments/spaces.py` & `gymnax-0.0.8/gymnax/environments/spaces.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/experimental/rollout.py` & `gymnax-0.0.8/gymnax/experimental/rollout.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/registration.py` & `gymnax-0.0.8/gymnax/registration.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/utils/load_mnist.py` & `gymnax-0.0.8/gymnax/utils/load_mnist.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/utils/state_translate.py` & `gymnax-0.0.8/gymnax/utils/state_translate.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/utils/test_helpers.py` & `gymnax-0.0.8/gymnax/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/visualize/vis_catch.py` & `gymnax-0.0.8/gymnax/visualize/vis_catch.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/visualize/vis_circle.py` & `gymnax-0.0.8/gymnax/visualize/vis_circle.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/visualize/vis_gym.py` & `gymnax-0.0.8/gymnax/visualize/vis_gym.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/visualize/vis_maze.py` & `gymnax-0.0.8/gymnax/visualize/vis_maze.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/visualize/vis_minatar.py` & `gymnax-0.0.8/gymnax/visualize/vis_minatar.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/visualize/visualizer.py` & `gymnax-0.0.8/gymnax/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/wrappers/__init__.py` & `gymnax-0.0.8/gymnax/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/wrappers/brax.py` & `gymnax-0.0.8/gymnax/wrappers/brax.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/wrappers/dm_env.py` & `gymnax-0.0.8/gymnax/wrappers/dm_env.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/wrappers/evojax.py` & `gymnax-0.0.8/gymnax/wrappers/evojax.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/wrappers/gym.py` & `gymnax-0.0.8/gymnax/wrappers/gym.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax/wrappers/purerl.py` & `gymnax-0.0.8/gymnax/wrappers/purerl.py`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/gymnax.egg-info/PKG-INFO` & `gymnax-0.0.8/gymnax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gymnax
-Version: 0.0.7
+Version: 0.0.8
 Summary: JAX-compatible version of Open AI's gym environments
 Home-page: https://github.com/RobertTLange/gymnax
-Download-URL: https://github.com/RobertTLange/gymnax/archive/v0.0.7.tar.gz
+Download-URL: https://github.com/RobertTLange/gymnax/archive/v0.0.8.tar.gz
 Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -17,14 +17,16 @@
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: chex
 Requires-Dist: flax
 Requires-Dist: pyyaml
 Requires-Dist: gym>=0.26
 Requires-Dist: gymnasium
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
 
 <h1 align="center">
   <a href="https://github.com/RobertTLange/gymnax/blob/main/docs/logo.png">
     <img src="https://github.com/RobertTLange/gymnax/blob/main/docs/logo.png?raw=true" width="215" /></a><br>
   <b>Reinforcement Learning Environments in JAX 🌍</b><br>
 </h1>
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: gymnax Version: 0.0.7 Summary: JAX-compatible
+Metadata-Version: 2.1 Name: gymnax Version: 0.0.8 Summary: JAX-compatible
 version of Open AI's gym environments Home-page: https://github.com/
 RobertTLange/gymnax Download-URL: https://github.com/RobertTLange/gymnax/
-archive/v0.0.7.tar.gz Author: Robert Tjarko Lange Author-email:
+archive/v0.0.8.tar.gz Author: Robert Tjarko Lange Author-email:
 robertlange0@gmail.com Platform: any Classifier: Programming Language :: Python
 :: 3.10 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
 :: Artificial Intelligence Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: jax Requires-Dist: jaxlib
 Requires-Dist: chex Requires-Dist: flax Requires-Dist: pyyaml Requires-Dist:
-gym>=0.26 Requires-Dist: gymnasium
+gym>=0.26 Requires-Dist: gymnasium Requires-Dist: matplotlib Requires-Dist:
+seaborn
         ************ _[[_hh_tt_tt_pp_ss_::_//_//_gg_ii_tt_hh_uu_bb_.._cc_oo_mm_//_RR_oo_bb_ee_rr_tt_TT_LL_aa_nn_gg_ee_//_gg_yy_mm_nn_aa_xx_//_bb_ll_oo_bb_//_mm_aa_ii_nn_//_dd_oo_cc_ss_//
                               _ll_oo_gg_oo_.._pp_nn_gg_??_rr_aa_ww_==_tt_rr_uu_ee_]]
                 RReeiinnffoorrcceemmeenntt LLeeaarrnniinngg EEnnvviirroonnmmeennttss iinn JJAAXX ?ð???
                                      ************
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_g_y_m_n_a_x_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/
  _b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_g_y_m_n_a_x_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_l_i_c_e_n_s_e_-_A_p_a_c_h_e_2_._0_-
     _b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_R_o_b_e_r_t_T_L_a_n_g_e_/_g_y_m_n_a_x_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/
```

### Comparing `gymnax-0.0.7/gymnax.egg-info/SOURCES.txt` & `gymnax-0.0.8/gymnax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gymnax-0.0.7/setup.py` & `gymnax-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,25 @@
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
     verstr = mo.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 git_tar = f"https://github.com/RobertTLange/gymnax/archive/v{verstr}.tar.gz"
 
-requires = ["jax", "jaxlib", "chex", "flax", "pyyaml", "gym>=0.26", "gymnasium"]
+requires = [
+    "jax",
+    "jaxlib",
+    "chex",
+    "flax",
+    "pyyaml",
+    "gym>=0.26",
+    "gymnasium",
+    "matplotlib",
+    "seaborn",
+]
 test_requires = ["bsuite", "minatar", "brax"]
 
 setup(
     name="gymnax",
     version=verstr,
     author="Robert Tjarko Lange",
     author_email="robertlange0@gmail.com",
```

### Comparing `gymnax-0.0.7/tests/test_visualizer.py` & `gymnax-0.0.8/tests/test_visualizer.py`

 * *Files identical despite different names*

