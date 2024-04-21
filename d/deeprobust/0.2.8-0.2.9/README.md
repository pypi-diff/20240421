# Comparing `tmp/deeprobust-0.2.8.tar.gz` & `tmp/deeprobust-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeprobust-0.2.8.tar", last modified: Fri Mar  3 21:45:15 2023, max compression
+gzip compressed data, was "deeprobust-0.2.9.tar", last modified: Mon Nov 13 23:10:10 2023, max compression
```

## Comparing `deeprobust-0.2.8.tar` & `deeprobust-0.2.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:45:15.690546 deeprobust-0.2.8/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     1101 2023-02-25 05:02:22.000000 deeprobust-0.2.8/LICENSE
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    18236 2023-03-03 21:45:15.689217 deeprobust-0.2.8/PKG-INFO
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    14927 2023-03-03 21:43:30.000000 deeprobust-0.2.8/README.md
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:44:58.472836 deeprobust-0.2.8/deeprobust/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)       95 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/__init__.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:44:58.502993 deeprobust-0.2.8/deeprobust/graph/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)        1 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/graph/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     2776 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/graph/black_box.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:44:58.579291 deeprobust-0.2.8/deeprobust/graph/data/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      609 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/graph/data/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     9603 2023-02-26 03:47:41.000000 deeprobust-0.2.8/deeprobust/graph/data/attacked_data.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    14078 2023-02-25 22:48:29.000000 deeprobust-0.2.8/deeprobust/graph/data/dataset.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    11347 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/graph/data/pyg_dataset.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      101 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/graph/data/utils.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:44:58.755572 deeprobust-0.2.8/deeprobust/graph/defense/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      880 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/graph/defense/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     1509 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/graph/defense/adv_training.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     6924 2023-02-25 05:02:22.000000 deeprobust-0.2.8/deeprobust/graph/defense/chebnet.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     7055 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/gat.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    12355 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/gcn.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    18306 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/gcn_preprocess.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    10381 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/median_gcn.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    19244 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/node_embedding.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     7514 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/pgd.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    11847 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/prognn.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    13502 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/r_gcn.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     6435 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/sgc.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    18044 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/defense/simpgcn.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:44:58.828581 deeprobust-0.2.8/deeprobust/graph/defense_pyg/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      546 2023-02-26 05:24:22.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     6901 2023-02-26 02:06:15.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/airgnn.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     2374 2023-02-26 01:55:59.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/appnp.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     7386 2023-02-26 02:36:02.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/base_model.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3226 2023-03-03 20:14:39.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/gat.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3927 2023-02-26 02:08:59.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/gcn.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4503 2023-03-03 20:49:35.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/gpr.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     8466 2023-03-03 20:16:49.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/mygat_conv.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5341 2023-03-03 21:09:08.000000 deeprobust-0.2.8/deeprobust/graph/defense_pyg/sage.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:44:58.912313 deeprobust-0.2.8/deeprobust/graph/global_attack/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      797 2023-02-26 05:25:41.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3847 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/base_attack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4588 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/dice.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    25562 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/mettack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    10320 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/nipa.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    21117 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/node_embedding_attack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    18216 2023-03-03 21:03:22.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/prbcd.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4803 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/random_attack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    12338 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/global_attack/topology_attack.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:45:07.003905 deeprobust-0.2.8/deeprobust/graph/rl/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)        0 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     9253 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/env.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     2754 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/nipa_config.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     6575 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/nipa_env.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     1978 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/nipa_nstep_replay_mem.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     8821 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/nipa_q_net_node.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5789 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/nstep_replay_mem.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     8535 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/q_net_node.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     2664 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/rl_s2v_config.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     9251 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/rl/rl_s2v_env.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:45:07.088054 deeprobust-0.2.8/deeprobust/graph/targeted_attack/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      275 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/targeted_attack/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3725 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/targeted_attack/base_attack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4774 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/targeted_attack/fga.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     9287 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/targeted_attack/ig_attack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    26522 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/targeted_attack/nettack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     9700 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/targeted_attack/rl_s2v.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5819 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/targeted_attack/rnd.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    14048 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/targeted_attack/sga.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    26246 2023-02-26 05:18:36.000000 deeprobust-0.2.8/deeprobust/graph/utils.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     2826 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/graph/visualization.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:45:07.132451 deeprobust-0.2.8/deeprobust/image/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      308 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/__init__.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:45:07.222173 deeprobust-0.2.8/deeprobust/image/attack/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3177 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/BPDA.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5918 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/Nattack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4134 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/Universal.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4239 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/YOPOpgd.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      458 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     2345 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/base_attack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     9415 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/cw.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4232 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/deepfool.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3224 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/fgsm.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     6741 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/l2_attack.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     6019 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/lbfgs.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5936 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/onepixel.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4559 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/attack/pgd.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     1433 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/config.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:45:07.285369 deeprobust-0.2.8/deeprobust/image/defense/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    10204 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/AWP.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     4829 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/LIDclassifier.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5627 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/TherEncoding.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    13676 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/YOPO.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      285 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     2059 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/base_defense.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5853 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/fast.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     7004 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/fgsmtraining.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     7643 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/pgdtraining.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     9006 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/defense/trades.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     9845 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/evaluation_attack.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:45:15.686456 deeprobust-0.2.8/deeprobust/image/netmodels/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3756 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/CNN.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3714 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/CNN_multilayer.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     2168 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/YOPOCNN.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      257 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/__init__.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5889 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/densenet.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3706 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/preact_resnet.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5785 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/resnet.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     5226 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/train_model.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     1214 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/train_resnet.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3580 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/netmodels/vgg.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    38820 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/optimizer.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     6457 2023-02-25 05:02:30.000000 deeprobust-0.2.8/deeprobust/image/utils.py
-drwxr-x---   0 jinwei2  (1022028) cse       (2010)        0 2023-03-03 21:44:58.478173 deeprobust-0.2.8/deeprobust.egg-info/
--rw-r-----   0 jinwei2  (1022028) cse       (2010)    18236 2023-03-03 21:44:37.000000 deeprobust-0.2.8/deeprobust.egg-info/PKG-INFO
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     3820 2023-03-03 21:44:37.000000 deeprobust-0.2.8/deeprobust.egg-info/SOURCES.txt
--rw-r-----   0 jinwei2  (1022028) cse       (2010)        1 2023-03-03 21:44:37.000000 deeprobust-0.2.8/deeprobust.egg-info/dependency_links.txt
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      220 2023-03-03 21:44:37.000000 deeprobust-0.2.8/deeprobust.egg-info/requires.txt
--rw-r-----   0 jinwei2  (1022028) cse       (2010)       11 2023-03-03 21:44:37.000000 deeprobust-0.2.8/deeprobust.egg-info/top_level.txt
--rw-r-----   0 jinwei2  (1022028) cse       (2010)       38 2023-03-03 21:45:15.691187 deeprobust-0.2.8/setup.cfg
--rw-r-----   0 jinwei2  (1022028) cse       (2010)     1564 2023-03-03 21:43:18.000000 deeprobust-0.2.8/setup.py
--rw-r-----   0 jinwei2  (1022028) cse       (2010)      229 2023-02-25 05:02:36.000000 deeprobust-0.2.8/setup_empty.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.805066 deeprobust-0.2.9/
+-rw-r--r--   0 jinwei     (502) staff       (20)     1101 2023-11-13 23:08:36.000000 deeprobust-0.2.9/LICENSE
+-rw-r--r--   0 jinwei     (502) staff       (20)    16249 2023-11-13 23:10:10.804879 deeprobust-0.2.9/PKG-INFO
+-rw-r--r--   0 jinwei     (502) staff       (20)    15401 2023-11-13 23:09:01.000000 deeprobust-0.2.9/README.md
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.788157 deeprobust-0.2.9/deeprobust/
+-rw-r--r--   0 jinwei     (502) staff       (20)       95 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/__init__.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.790475 deeprobust-0.2.9/deeprobust/graph/
+-rw-r--r--   0 jinwei     (502) staff       (20)        1 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     2776 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/black_box.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.791477 deeprobust-0.2.9/deeprobust/graph/data/
+-rw-r--r--   0 jinwei     (502) staff       (20)      609 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/data/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     9603 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/data/attacked_data.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    14083 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/data/dataset.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    11347 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/data/pyg_dataset.py
+-rw-r--r--   0 jinwei     (502) staff       (20)      101 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/data/utils.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.793913 deeprobust-0.2.9/deeprobust/graph/defense/
+-rw-r--r--   0 jinwei     (502) staff       (20)      880 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     1509 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/adv_training.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     6924 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/chebnet.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     7055 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/gat.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    12355 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/gcn.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    18306 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/gcn_preprocess.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    10381 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/median_gcn.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    19244 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/node_embedding.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     7514 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/pgd.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    11847 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/prognn.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    13502 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/r_gcn.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     6435 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/sgc.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    18044 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense/simpgcn.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.795399 deeprobust-0.2.9/deeprobust/graph/defense_pyg/
+-rw-r--r--   0 jinwei     (502) staff       (20)      546 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     6901 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/airgnn.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     2374 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/appnp.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     7386 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/base_model.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     3226 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/gat.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     3927 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/gcn.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4503 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/gpr.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     8466 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/mygat_conv.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5341 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/defense_pyg/sage.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.796796 deeprobust-0.2.9/deeprobust/graph/global_attack/
+-rw-r--r--   0 jinwei     (502) staff       (20)      797 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     3847 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/base_attack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4588 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/dice.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    25592 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/mettack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    10320 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/nipa.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    21117 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/node_embedding_attack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    18216 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/prbcd.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4803 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/random_attack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    12338 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/global_attack/topology_attack.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.798021 deeprobust-0.2.9/deeprobust/graph/rl/
+-rw-r--r--   0 jinwei     (502) staff       (20)        0 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     9253 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/env.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     2754 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/nipa_config.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     6575 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/nipa_env.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     1978 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/nipa_nstep_replay_mem.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     8821 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/nipa_q_net_node.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5789 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/nstep_replay_mem.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     8535 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/q_net_node.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     2664 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/rl_s2v_config.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     9251 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/rl/rl_s2v_env.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.799299 deeprobust-0.2.9/deeprobust/graph/targeted_attack/
+-rw-r--r--   0 jinwei     (502) staff       (20)      275 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     3725 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/base_attack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4774 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/fga.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     9287 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/ig_attack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    26522 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/nettack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     9700 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/rl_s2v.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5819 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/rnd.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    14048 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/sga.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    37345 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/targeted_attack/ugba.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    26246 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/utils.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     2826 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/graph/visualization.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.800339 deeprobust-0.2.9/deeprobust/image/
+-rw-r--r--   0 jinwei     (502) staff       (20)      308 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/__init__.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.802277 deeprobust-0.2.9/deeprobust/image/attack/
+-rw-r--r--   0 jinwei     (502) staff       (20)     3177 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/BPDA.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5918 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/Nattack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4134 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/Universal.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4239 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/YOPOpgd.py
+-rw-r--r--   0 jinwei     (502) staff       (20)      458 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     2345 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/base_attack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     9415 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/cw.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4232 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/deepfool.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     3224 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/fgsm.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     6741 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/l2_attack.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     6019 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/lbfgs.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5936 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/onepixel.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4559 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/attack/pgd.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     1433 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/config.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.803490 deeprobust-0.2.9/deeprobust/image/defense/
+-rw-r--r--   0 jinwei     (502) staff       (20)    10204 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/AWP.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     4829 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/LIDclassifier.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5627 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/TherEncoding.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    13676 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/YOPO.py
+-rw-r--r--   0 jinwei     (502) staff       (20)      285 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     2059 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/base_defense.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5853 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/fast.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     7004 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/fgsmtraining.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     7643 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/pgdtraining.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     9006 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/defense/trades.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     9845 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/evaluation_attack.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.804696 deeprobust-0.2.9/deeprobust/image/netmodels/
+-rw-r--r--   0 jinwei     (502) staff       (20)     3756 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/CNN.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     3714 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/CNN_multilayer.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     2168 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/YOPOCNN.py
+-rw-r--r--   0 jinwei     (502) staff       (20)      257 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/__init__.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5889 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/densenet.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     3706 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/preact_resnet.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5785 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/resnet.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     5226 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/train_model.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     1214 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/train_resnet.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     3580 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/netmodels/vgg.py
+-rw-r--r--   0 jinwei     (502) staff       (20)    38820 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/optimizer.py
+-rw-r--r--   0 jinwei     (502) staff       (20)     6457 2023-11-13 23:08:36.000000 deeprobust-0.2.9/deeprobust/image/utils.py
+drwxr-xr-x   0 jinwei     (502) staff       (20)        0 2023-11-13 23:10:10.789406 deeprobust-0.2.9/deeprobust.egg-info/
+-rw-r--r--   0 jinwei     (502) staff       (20)    16249 2023-11-13 23:10:10.000000 deeprobust-0.2.9/deeprobust.egg-info/PKG-INFO
+-rw-r--r--   0 jinwei     (502) staff       (20)     3846 2023-11-13 23:10:10.000000 deeprobust-0.2.9/deeprobust.egg-info/SOURCES.txt
+-rw-r--r--   0 jinwei     (502) staff       (20)        1 2023-11-13 23:10:10.000000 deeprobust-0.2.9/deeprobust.egg-info/dependency_links.txt
+-rw-r--r--   0 jinwei     (502) staff       (20)      220 2023-11-13 23:10:10.000000 deeprobust-0.2.9/deeprobust.egg-info/requires.txt
+-rw-r--r--   0 jinwei     (502) staff       (20)       11 2023-11-13 23:10:10.000000 deeprobust-0.2.9/deeprobust.egg-info/top_level.txt
+-rw-r--r--   0 jinwei     (502) staff       (20)       38 2023-11-13 23:10:10.805107 deeprobust-0.2.9/setup.cfg
+-rw-r--r--   0 jinwei     (502) staff       (20)     1564 2023-11-13 23:09:44.000000 deeprobust-0.2.9/setup.py
```

### Comparing `deeprobust-0.2.8/LICENSE` & `deeprobust-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/PKG-INFO` & `deeprobust-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,330 +1,335 @@
 Metadata-Version: 2.1
 Name: deeprobust
-Version: 0.2.8
+Version: 0.2.9
 Summary: A PyTorch library for adversarial robustness learning for image and graph data.
 Home-page: https://github.com/DSE-MSU/DeepRobust
 Author: MSU-DSE
 Maintainer: MSU-DSE
 License: MIT
-Description: 
-        [contributing-image]: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
-        [contributing-url]: https://github.com/rusty1s/pytorch_geometric/blob/master/CONTRIBUTING.md
-        
-        <p align="center">
-        <img center src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/Deeprobust.png" width = "450" alt="logo">
-        </p>
-        
-        ---------------------
-        <!--
-        <a href="https://github.com/DSE-MSU/DeepRobust/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/DSE-MSU/DeepRobust"></a>  <a href="https://github.com/DSE-MSU/DeepRobust/network/members" ><img alt="GitHub forks" src="https://img.shields.io/github/forks/DSE-MSU/DeepRobust">
-        </a> 
-        -->
-        
-        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/DSE-MSU/DeepRobust"> <a href="https://github.com/DSE-MSU/DeepRobust/issues"> <img alt="GitHub issues" src="https://img.shields.io/github/issues/DSE-MSU/DeepRobust"></a> <img alt="GitHub" src="https://img.shields.io/github/license/DSE-MSU/DeepRobust">
-        [![Contributing][contributing-image]][contributing-url]
-        [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20your%20robust%20machine%20learning%20models%20with%20DeepRobust%20in%2060%20seconds&url=https://github.com/DSE-MSU/DeepRobust&via=dse_msu&hashtags=MachineLearning,DeepLearning,secruity,data,developers)
-        
-        
-        <!-- <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/DSE-MSU/DeepRobust"> -->
-        
-        <!--
-        <div align=center><img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversarial.png" width="500"/></div>
-        <div align=center><img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/graph_attack_example.png" width="00" /></div>
-        -->
-        **[Documentation](https://deeprobust.readthedocs.io/en/latest/)** | **[Paper](https://arxiv.org/abs/2005.06149)** | **[Samples](https://github.com/DSE-MSU/DeepRobust/tree/master/examples)** 
-        
-        [AAAI 2021] DeepRobust is a PyTorch adversarial library for attack and defense methods on images and graphs. 
-        * If you are new to DeepRobust, we highly suggest you read the [documentation page](https://deeprobust.readthedocs.io/en/latest/) or the following content in this README to learn how to use it.  
-        * If you have any questions or suggestions regarding this library, feel free to create an issue [here](https://github.com/DSE-MSU/DeepRobust/issues). We will reply as soon as possible :)
-        
-        <p float="left">
-          <img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/adversarial.png" width="430" />
-          <img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/graph_attack_example.png" width="380" /> 
-        </p>
-        
-        **List of including algorithms can be found in [[Image Package]](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/image) and [[Graph Package]](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph).**
-        
-        [Environment & Installation](#environment)
-        
-        Usage
-        
-        * [Image Attack and Defense](#image-attack-and-defense)
-        
-        * [Graph Attack and Defense](#graph-attack-and-defense)
-        
-        [Acknowledgement](#acknowledgement) 
-        
-        For more details about attacks and defenses, you can read the following papers.
-        * [Adversarial Attacks and Defenses on Graphs: A Review, A Tool and Empirical Studies](https://arxiv.org/abs/2003.00653)
-        * [Adversarial Attacks and Defenses in Images, Graphs and Text: A Review](https://arxiv.org/pdf/1909.08072.pdf)
-        
-        If our work could help your research, please cite:
-        [DeepRobust: A PyTorch Library for Adversarial Attacks and Defenses](https://arxiv.org/abs/2005.06149)
-        ```
-        @article{li2020deeprobust,
-          title={Deeprobust: A pytorch library for adversarial attacks and defenses},
-          author={Li, Yaxin and Jin, Wei and Xu, Han and Tang, Jiliang},
-          journal={arXiv preprint arXiv:2005.06149},
-          year={2020}
-        }
-        ```
-        
-        # Changelog
-        * [02/2023] DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We have added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/2110.14038) to graph package. We can now use PRBCD to attack large-scale graphs such as ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_prbcd.py))! 
-        * [02/2023] Add a robust model [AirGNN, NeurIPS'21](https://proceedings.neurips.cc/paper/2021/file/50abc3e730e36b387ca8e02c26dc0a22-Paper.pdf) to graph package. Try `python examples/graph/test_airgnn.py`! See details in [test_airgnn.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_airgnn.py)
-        * [11/2022] DeepRobust 0.2.6 Released. Please try `pip install deeprobust==0.2.6`! We have more updates coming. Please stay tuned!
-        * [11/2021] A subpackage that includes popular black box attacks in image domain is relased. Find it here. [Link](https://github.com/I-am-Bot/Black-Box-Attacks)
-        * [11/2021] DeepRobust 0.2.4 Released. Please try `pip install deeprobust==0.2.4`!
-        * [10/2021] add scalable attack and MedianGCN. Thank [Jintang](https://github.com/EdisonLeeeee) for his contribution!
-        * [06/2021] [Image Package] Add preprocessing method: APE-GAN.
-        * [05/2021] DeepRobust is published at AAAI 2021. Check [here](https://ojs.aaai.org/index.php/AAAI/article/view/18017)!
-        * [05/2021] DeepRobust 0.2.2 Released. Please try `pip install deeprobust==0.2.2`!
-        * [04/2021] [Image Package] Add support for ImageNet. See details in [test_ImageNet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/image/test_ImageNet.py)
-        * [04/2021] [Graph Package] Add support for OGB datasets.  See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html).
-        * [03/2021] [Graph Package] Added node embedding attack and victim models! See this [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/node_embedding.html).
-        * [02/2021] **[Graph Package] DeepRobust now provides tools for converting the datasets between [Pytorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/) and DeepRobust. See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html)!** DeepRobust now also support GAT, Chebnet and SGC based on pyg; see details in [test_gat.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_gat.py),  [test_chebnet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_chebnet.py) and [test_sgc.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_sgc.py)
-        * [12/2020] DeepRobust now can be installed via pip! Try `pip install deeprobust`!
-        * [12/2020] [Graph Package] Add four more [datasets](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph/#supported-datasets) and one defense algorithm. More details can be found [here](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph/#defense-methods). More datasets and algorithms will be added later. Stay tuned :)
-        * [07/2020] Add [documentation](https://deeprobust.readthedocs.io/en/latest/) page!
-        * [06/2020] Add docstring to both image and graph package
-        
-        # Basic Environment
-        * `python >= 3.6` (python 3.5 should also work)
-        * `pytorch >= 1.2.0`
-        
-        see `setup.py` or `requirements.txt` for more information.
-        
-        # Installation
-        ## Install from pip
-        ```
-        pip install deeprobust 
-        ```
-        ## Install from source
-        ```
-        git clone https://github.com/DSE-MSU/DeepRobust.git
-        cd DeepRobust
-        python setup.py install
-        ```
-        
-        # Test Examples
-        
-        ```
-        python examples/image/test_PGD.py
-        python examples/image/test_pgdtraining.py
-        python examples/graph/test_gcn_jaccard.py --dataset cora
-        python examples/graph/test_mettack.py --dataset cora --ptb_rate 0.05
-        ```
-        
-        # Usage
-        ## Image Attack and Defense
-        1. Train model
-        
-            Example: Train a simple CNN model on MNIST dataset for 20 epoch on gpu.
-            ```python
-            import deeprobust.image.netmodels.train_model as trainmodel
-            trainmodel.train('CNN', 'MNIST', 'cuda', 20)
-            ```
-            Model would be saved in deeprobust/trained_models/.
-        
-        2. Instantiated attack methods and defense methods.
-        
-            Example: Generate adversary example with PGD attack.
-            ```python
-            from deeprobust.image.attack.pgd import PGD
-            from deeprobust.image.config import attack_params
-            from deeprobust.image.utils import download_model
-            import torch
-            import deeprobust.image.netmodels.resnet as resnet
-            from torchvision import transforms,datasets
-            
-            URL = "https://github.com/I-am-Bot/deeprobust_model/raw/master/CIFAR10_ResNet18_epoch_20.pt"
-            download_model(URL, "$MODEL_PATH$")
-        
-            model = resnet.ResNet18().to('cuda')
-            model.load_state_dict(torch.load("$MODEL_PATH$"))
-            model.eval()
-        
-            transform_val = transforms.Compose([transforms.ToTensor()])
-            test_loader  = torch.utils.data.DataLoader(
-                            datasets.CIFAR10('deeprobust/image/data', train = False, download=True,
-                            transform = transform_val),
-                            batch_size = 10, shuffle=True)
-        
-            x, y = next(iter(test_loader))
-            x = x.to('cuda').float()
-            
-            adversary = PGD(model, 'cuda')
-            Adv_img = adversary.generate(x, y, **attack_params['PGD_CIFAR10'])
-            ```
-        
-            Example: Train defense model.
-            ```python
-            from deeprobust.image.defense.pgdtraining import PGDtraining
-            from deeprobust.image.config import defense_params
-            from deeprobust.image.netmodels.CNN import Net
-            import torch
-            from torchvision import datasets, transforms 
-            
-            model = Net()
-            train_loader = torch.utils.data.DataLoader(
-                            datasets.MNIST('deeprobust/image/defense/data', train=True, download=True,
-                                            transform=transforms.Compose([transforms.ToTensor()])),
-                                            batch_size=100,shuffle=True)
-        
-            test_loader = torch.utils.data.DataLoader(
-                          datasets.MNIST('deeprobust/image/defense/data', train=False,
-                                        transform=transforms.Compose([transforms.ToTensor()])),
-                                        batch_size=1000,shuffle=True)
-        
-            defense = PGDtraining(model, 'cuda')
-            defense.generate(train_loader, test_loader, **defense_params["PGDtraining_MNIST"])
-            ```
-        
-            More example code can be found in deeprobust/examples.
-        
-        3. Use our evulation program to test attack algorithm against defense.
-        
-            Example:
-            ```
-            cd DeepRobust
-            python examples/image/test_train.py
-            python deeprobust/image/evaluation_attack.py
-            ```
-        
-        ## Graph Attack and Defense 
-        
-        ### Attacking Graph Neural Networks
-        
-        1. Load dataset
-            ```python
-            import torch
-            import numpy as np
-            from deeprobust.graph.data import Dataset
-            from deeprobust.graph.defense import GCN
-            from deeprobust.graph.global_attack import Metattack
-        
-            data = Dataset(root='/tmp/', name='cora', setting='nettack')
-            adj, features, labels = data.adj, data.features, data.labels
-            idx_train, idx_val, idx_test = data.idx_train, data.idx_val, data.idx_test
-            idx_unlabeled = np.union1d(idx_val, idx_test)
-            ```
-        
-        2. Set up surrogate model
-            ```python
-            device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-            surrogate = GCN(nfeat=features.shape[1], nclass=labels.max().item()+1, nhid=16,
-                            with_relu=False, device=device)
-            surrogate = surrogate.to(device)
-            surrogate.fit(features, adj, labels, idx_train)
-            ```
-        
-        
-        3. Set up attack model and generate perturbations
-            ```python
-            model = Metattack(model=surrogate, nnodes=adj.shape[0], feature_shape=features.shape, device=device)
-            model = model.to(device)
-            perturbations = int(0.05 * (adj.sum() // 2))
-            model.attack(features, adj, labels, idx_train, idx_unlabeled, perturbations, ll_constraint=False)
-            modified_adj = model.modified_adj
-            ```
-            
-        For more details please refer to [mettack.py](https://github.com/I-am-Bot/DeepRobust/blob/master/examples/graph/test_mettack.py) or run 
-            ```
-            python examples/graph/test_mettack.py --dataset cora --ptb_rate 0.05
-            ```
-        
-        ### Defending Against Graph Attacks
-        
-        1. Load dataset
-            ```python
-            import torch
-            from deeprobust.graph.data import Dataset, PtbDataset
-            from deeprobust.graph.defense import GCN, GCNJaccard
-            import numpy as np
-            np.random.seed(15)
-        
-            # load clean graph
-            data = Dataset(root='/tmp/', name='cora', setting='nettack')
-            adj, features, labels = data.adj, data.features, data.labels
-            idx_train, idx_val, idx_test = data.idx_train, data.idx_val, data.idx_test
-        
-            # load pre-attacked graph by mettack
-            perturbed_data = PtbDataset(root='/tmp/', name='cora')
-            perturbed_adj = perturbed_data.adj
-            ```
-        2. Test 
-            ```python
-            # Set up defense model and test performance
-            device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-            model = GCNJaccard(nfeat=features.shape[1], nclass=labels.max()+1, nhid=16, device=device)
-            model = model.to(device)
-            model.fit(features, perturbed_adj, labels, idx_train)
-            model.eval()
-            output = model.test(idx_test)
-        
-            # Test on GCN
-            model = GCN(nfeat=features.shape[1], nclass=labels.max()+1, nhid=16, device=device)
-            model = model.to(device)
-            model.fit(features, perturbed_adj, labels, idx_train)
-            model.eval()
-            output = model.test(idx_test)
-            ```
-            
-        For more details please refer to [test_gcn_jaccard.py](https://github.com/I-am-Bot/DeepRobust/blob/master/examples/graph/test_gcn_jaccard.py) or run
-            ```
-            python examples/graph/test_gcn_jaccard.py --dataset cora
-            ```
-        
-        ## Sample Results
-        adversary examples generated by fgsm:
-        <div align="center">
-        <img height=140 src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/mnist_advexample_fgsm_ori.png"/><img height=140 src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/mnist_advexample_fgsm_adv.png"/>
-        </div>
-        Left:original, classified as 6; Right:adversary, classified as 4.
-        
-        Serveral trained models can be found here: https://drive.google.com/open?id=1uGLiuCyd8zCAQ8tPz9DDUQH6zm-C4tEL
-        
-        ## Acknowledgement
-        Some of the algorithms are referred to paper authors' implementations. References can be found at the top of each file. 
-        
-        Implementation of network structure are referred to weiaicunzai's github. Original code can be found here:
-        [pytorch-cifar100](https://github.com/weiaicunzai/pytorch-cifar100)
-        
-        Thanks to their outstanding works!
-        
-        
-        <!----
-        We would be glad if you find our work useful and cite the paper.
-        
-        '''
-        @misc{jin2020adversarial,
-            title={Adversarial Attacks and Defenses on Graphs: A Review and Empirical Study},
-            author={Wei Jin and Yaxin Li and Han Xu and Yiqi Wang and Jiliang Tang},
-            year={2020},
-            eprint={2003.00653},
-            archivePrefix={arXiv},
-            primaryClass={cs.LG}
-        }
-        '''
-        ```
-        @article{xu2019adversarial,
-          title={Adversarial attacks and defenses in images, graphs and text: A review},
-          author={Xu, Han and Ma, Yao and Liu, Haochen and Deb, Debayan and Liu, Hui and Tang, Jiliang and Jain, Anil},
-          journal={arXiv preprint arXiv:1909.08072},
-          year={2019}
-        }
-        ```
-        ---->
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[contributing-image]: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
+[contributing-url]: https://github.com/rusty1s/pytorch_geometric/blob/master/CONTRIBUTING.md
+
+<p align="center">
+<img center src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/Deeprobust.png" width = "450" alt="logo">
+</p>
+
+---------------------
+<!--
+<a href="https://github.com/DSE-MSU/DeepRobust/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/DSE-MSU/DeepRobust"></a>  <a href="https://github.com/DSE-MSU/DeepRobust/network/members" ><img alt="GitHub forks" src="https://img.shields.io/github/forks/DSE-MSU/DeepRobust">
+</a> 
+-->
+
+<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/DSE-MSU/DeepRobust"> <a href="https://github.com/DSE-MSU/DeepRobust/issues"> <img alt="GitHub issues" src="https://img.shields.io/github/issues/DSE-MSU/DeepRobust"></a> <img alt="GitHub" src="https://img.shields.io/github/license/DSE-MSU/DeepRobust">
+[![Contributing][contributing-image]][contributing-url]
+[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20your%20robust%20machine%20learning%20models%20with%20DeepRobust%20in%2060%20seconds&url=https://github.com/DSE-MSU/DeepRobust&via=dse_msu&hashtags=MachineLearning,DeepLearning,secruity,data,developers)
+
+
+<!-- <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/DSE-MSU/DeepRobust"> -->
+
+<!--
+<div align=center><img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversarial.png" width="500"/></div>
+<div align=center><img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/graph_attack_example.png" width="00" /></div>
+-->
+**[Documentation](https://deeprobust.readthedocs.io/en/latest/)** | **[Paper](https://arxiv.org/abs/2005.06149)** | **[Samples](https://github.com/DSE-MSU/DeepRobust/tree/master/examples)** 
+
+[AAAI 2021] DeepRobust is a PyTorch adversarial library for attack and defense methods on images and graphs. 
+* If you are new to DeepRobust, we highly suggest you read the [documentation page](https://deeprobust.readthedocs.io/en/latest/) or the following content in this README to learn how to use it.  
+* If you have any questions or suggestions regarding this library, feel free to create an issue [here](https://github.com/DSE-MSU/DeepRobust/issues). We will reply as soon as possible :)
+
+<p float="left">
+  <img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/adversarial.png" width="430" />
+  <img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/graph_attack_example.png" width="380" /> 
+</p>
+
+**List of including algorithms can be found in [[Image Package]](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/image) and [[Graph Package]](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph).**
+
+[Environment & Installation](#environment)
+
+Usage
+
+* [Image Attack and Defense](#image-attack-and-defense)
+
+* [Graph Attack and Defense](#graph-attack-and-defense)
+
+[Acknowledgement](#acknowledgement) 
+
+For more details about attacks and defenses, you can read the following papers.
+* [Adversarial Attacks and Defenses on Graphs: A Review, A Tool and Empirical Studies](https://arxiv.org/abs/2003.00653)
+* [Adversarial Attacks and Defenses in Images, Graphs and Text: A Review](https://arxiv.org/pdf/1909.08072.pdf)
+
+If our work could help your research, please cite:
+[DeepRobust: A PyTorch Library for Adversarial Attacks and Defenses](https://arxiv.org/abs/2005.06149)
+```
+@article{li2020deeprobust,
+  title={Deeprobust: A pytorch library for adversarial attacks and defenses},
+  author={Li, Yaxin and Jin, Wei and Xu, Han and Tang, Jiliang},
+  journal={arXiv preprint arXiv:2005.06149},
+  year={2020}
+}
+```
+
+# Changelog
+* [11/2023] DeepRobust 0.2.9 Released. Please try `pip install deeprobust==0.2.9`. We have fixed the OOM issue of metattack on new pytorch versions.
+* [06/2023] We have added a backdoor attack [UGBA, WWW'23](https://arxiv.org/abs/2303.01263) to graph package. We can now use UGBA to conduct unnoticeable backdoor attack on large-scale graphs such as ogb-arxiv (see example in [test_ugba.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_ugba.py))! 
+* [02/2023] DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We have added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/2110.14038) to graph package. We can now use PRBCD to attack large-scale graphs such as ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_prbcd.py))! 
+* [02/2023] Add a robust model [AirGNN, NeurIPS'21](https://proceedings.neurips.cc/paper/2021/file/50abc3e730e36b387ca8e02c26dc0a22-Paper.pdf) to graph package. Try `python examples/graph/test_airgnn.py`! See details in [test_airgnn.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_airgnn.py)
+* [11/2022] DeepRobust 0.2.6 Released. Please try `pip install deeprobust==0.2.6`! We have more updates coming. Please stay tuned!
+* [11/2021] A subpackage that includes popular black box attacks in image domain is released. Find it here. [Link](https://github.com/I-am-Bot/Black-Box-Attacks)
+* [11/2021] DeepRobust 0.2.4 Released. Please try `pip install deeprobust==0.2.4`!
+* [10/2021] add scalable attack and MedianGCN. Thank [Jintang](https://github.com/EdisonLeeeee) for his contribution!
+* [06/2021] [Image Package] Add preprocessing method: APE-GAN.
+* [05/2021] DeepRobust is published at AAAI 2021. Check [here](https://ojs.aaai.org/index.php/AAAI/article/view/18017)!
+* [05/2021] DeepRobust 0.2.2 Released. Please try `pip install deeprobust==0.2.2`!
+* [04/2021] [Image Package] Add support for ImageNet. See details in [test_ImageNet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/image/test_ImageNet.py)
+* [04/2021] [Graph Package] Add support for OGB datasets.  See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html).
+* [03/2021] [Graph Package] Added node embedding attack and victim models! See this [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/node_embedding.html).
+* [02/2021] **[Graph Package] DeepRobust now provides tools for converting the datasets between [Pytorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/) and DeepRobust. See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html)!** DeepRobust now also support GAT, Chebnet and SGC based on pyg; see details in [test_gat.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_gat.py),  [test_chebnet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_chebnet.py) and [test_sgc.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_sgc.py)
+* [12/2020] DeepRobust now can be installed via pip! Try `pip install deeprobust`!
+* [12/2020] [Graph Package] Add four more [datasets](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph/#supported-datasets) and one defense algorithm. More details can be found [here](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph/#defense-methods). More datasets and algorithms will be added later. Stay tuned :)
+* [07/2020] Add [documentation](https://deeprobust.readthedocs.io/en/latest/) page!
+* [06/2020] Add docstring to both image and graph package
+
+# Basic Environment
+* `python >= 3.6` (python 3.5 should also work)
+* `pytorch >= 1.2.0`
+
+see `setup.py` or `requirements.txt` for more information.
+
+# Installation
+## Install from pip
+```
+pip install deeprobust 
+```
+## Install from source
+```
+git clone https://github.com/DSE-MSU/DeepRobust.git
+cd DeepRobust
+python setup.py install
+```
+
+# Test Examples
+
+```
+python examples/image/test_PGD.py
+python examples/image/test_pgdtraining.py
+python examples/graph/test_gcn_jaccard.py --dataset cora
+python examples/graph/test_mettack.py --dataset cora --ptb_rate 0.05
+```
+
+# Usage
+## Image Attack and Defense
+1. Train model
+
+    Example: Train a simple CNN model on MNIST dataset for 20 epoch on gpu.
+    ```python
+    import deeprobust.image.netmodels.train_model as trainmodel
+    trainmodel.train('CNN', 'MNIST', 'cuda', 20)
+    ```
+    Model would be saved in deeprobust/trained_models/.
+
+2. Instantiated attack methods and defense methods.
+
+    Example: Generate adversary example with PGD attack.
+    ```python
+    from deeprobust.image.attack.pgd import PGD
+    from deeprobust.image.config import attack_params
+    from deeprobust.image.utils import download_model
+    import torch
+    import deeprobust.image.netmodels.resnet as resnet
+    from torchvision import transforms,datasets
+    
+    URL = "https://github.com/I-am-Bot/deeprobust_model/raw/master/CIFAR10_ResNet18_epoch_20.pt"
+    download_model(URL, "$MODEL_PATH$")
+
+    model = resnet.ResNet18().to('cuda')
+    model.load_state_dict(torch.load("$MODEL_PATH$"))
+    model.eval()
+
+    transform_val = transforms.Compose([transforms.ToTensor()])
+    test_loader  = torch.utils.data.DataLoader(
+                    datasets.CIFAR10('deeprobust/image/data', train = False, download=True,
+                    transform = transform_val),
+                    batch_size = 10, shuffle=True)
+
+    x, y = next(iter(test_loader))
+    x = x.to('cuda').float()
+    
+    adversary = PGD(model, 'cuda')
+    Adv_img = adversary.generate(x, y, **attack_params['PGD_CIFAR10'])
+    ```
+
+    Example: Train defense model.
+    ```python
+    from deeprobust.image.defense.pgdtraining import PGDtraining
+    from deeprobust.image.config import defense_params
+    from deeprobust.image.netmodels.CNN import Net
+    import torch
+    from torchvision import datasets, transforms 
+    
+    model = Net()
+    train_loader = torch.utils.data.DataLoader(
+                    datasets.MNIST('deeprobust/image/defense/data', train=True, download=True,
+                                    transform=transforms.Compose([transforms.ToTensor()])),
+                                    batch_size=100,shuffle=True)
+
+    test_loader = torch.utils.data.DataLoader(
+                  datasets.MNIST('deeprobust/image/defense/data', train=False,
+                                transform=transforms.Compose([transforms.ToTensor()])),
+                                batch_size=1000,shuffle=True)
+
+    defense = PGDtraining(model, 'cuda')
+    defense.generate(train_loader, test_loader, **defense_params["PGDtraining_MNIST"])
+    ```
+
+    More example code can be found in deeprobust/examples.
+
+3. Use our evulation program to test attack algorithm against defense.
+
+    Example:
+    ```
+    cd DeepRobust
+    python examples/image/test_train.py
+    python deeprobust/image/evaluation_attack.py
+    ```
+
+## Graph Attack and Defense 
+
+### Attacking Graph Neural Networks
+
+1. Load dataset
+    ```python
+    import torch
+    import numpy as np
+    from deeprobust.graph.data import Dataset
+    from deeprobust.graph.defense import GCN
+    from deeprobust.graph.global_attack import Metattack
+
+    data = Dataset(root='/tmp/', name='cora', setting='nettack')
+    adj, features, labels = data.adj, data.features, data.labels
+    idx_train, idx_val, idx_test = data.idx_train, data.idx_val, data.idx_test
+    idx_unlabeled = np.union1d(idx_val, idx_test)
+    ```
+
+2. Set up surrogate model
+    ```python
+    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+    surrogate = GCN(nfeat=features.shape[1], nclass=labels.max().item()+1, nhid=16,
+                    with_relu=False, device=device)
+    surrogate = surrogate.to(device)
+    surrogate.fit(features, adj, labels, idx_train)
+    ```
+
+
+3. Set up attack model and generate perturbations
+    ```python
+    model = Metattack(model=surrogate, nnodes=adj.shape[0], feature_shape=features.shape, device=device)
+    model = model.to(device)
+    perturbations = int(0.05 * (adj.sum() // 2))
+    model.attack(features, adj, labels, idx_train, idx_unlabeled, perturbations, ll_constraint=False)
+    modified_adj = model.modified_adj
+    ```
+    
+For more details please refer to [mettack.py](https://github.com/I-am-Bot/DeepRobust/blob/master/examples/graph/test_mettack.py) or run 
+    ```
+    python examples/graph/test_mettack.py --dataset cora --ptb_rate 0.05
+    ```
+
+### Defending Against Graph Attacks
+
+1. Load dataset
+    ```python
+    import torch
+    from deeprobust.graph.data import Dataset, PtbDataset
+    from deeprobust.graph.defense import GCN, GCNJaccard
+    import numpy as np
+    np.random.seed(15)
+
+    # load clean graph
+    data = Dataset(root='/tmp/', name='cora', setting='nettack')
+    adj, features, labels = data.adj, data.features, data.labels
+    idx_train, idx_val, idx_test = data.idx_train, data.idx_val, data.idx_test
+
+    # load pre-attacked graph by mettack
+    perturbed_data = PtbDataset(root='/tmp/', name='cora')
+    perturbed_adj = perturbed_data.adj
+    ```
+2. Test 
+    ```python
+    # Set up defense model and test performance
+    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+    model = GCNJaccard(nfeat=features.shape[1], nclass=labels.max()+1, nhid=16, device=device)
+    model = model.to(device)
+    model.fit(features, perturbed_adj, labels, idx_train)
+    model.eval()
+    output = model.test(idx_test)
+
+    # Test on GCN
+    model = GCN(nfeat=features.shape[1], nclass=labels.max()+1, nhid=16, device=device)
+    model = model.to(device)
+    model.fit(features, perturbed_adj, labels, idx_train)
+    model.eval()
+    output = model.test(idx_test)
+    ```
+    
+For more details please refer to [test_gcn_jaccard.py](https://github.com/I-am-Bot/DeepRobust/blob/master/examples/graph/test_gcn_jaccard.py) or run
+    ```
+    python examples/graph/test_gcn_jaccard.py --dataset cora
+    ```
+
+## Sample Results
+adversary examples generated by fgsm:
+<div align="center">
+<img height=140 src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/mnist_advexample_fgsm_ori.png"/><img height=140 src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/mnist_advexample_fgsm_adv.png"/>
+</div>
+Left:original, classified as 6; Right:adversary, classified as 4.
+
+Serveral trained models can be found here: https://drive.google.com/open?id=1uGLiuCyd8zCAQ8tPz9DDUQH6zm-C4tEL
+
+## Acknowledgement
+Some of the algorithms are referred to paper authors' implementations. References can be found at the top of each file. 
+
+Implementation of network structure are referred to weiaicunzai's github. Original code can be found here:
+[pytorch-cifar100](https://github.com/weiaicunzai/pytorch-cifar100)
+
+Thanks to their outstanding works!
+
+
+<!----
+We would be glad if you find our work useful and cite the paper.
+
+'''
+@misc{jin2020adversarial,
+    title={Adversarial Attacks and Defenses on Graphs: A Review and Empirical Study},
+    author={Wei Jin and Yaxin Li and Han Xu and Yiqi Wang and Jiliang Tang},
+    year={2020},
+    eprint={2003.00653},
+    archivePrefix={arXiv},
+    primaryClass={cs.LG}
+}
+'''
+```
+@article{xu2019adversarial,
+  title={Adversarial attacks and defenses in images, graphs and text: A review},
+  author={Xu, Han and Ma, Yao and Liu, Haochen and Deb, Debayan and Liu, Hui and Tang, Jiliang and Jain, Anil},
+  journal={arXiv preprint arXiv:1909.08072},
+  year={2019}
+}
+```
+---->
+
+
```

#### html2text {}

```diff
@@ -1,13 +1,21 @@
-Metadata-Version: 2.1 Name: deeprobust Version: 0.2.8 Summary: A PyTorch
+Metadata-Version: 2.1 Name: deeprobust Version: 0.2.9 Summary: A PyTorch
 library for adversarial robustness learning for image and graph data. Home-
 page: https://github.com/DSE-MSU/DeepRobust Author: MSU-DSE Maintainer: MSU-DSE
-License: MIT Description: [contributing-image]: https://img.shields.io/badge/
-contributions-welcome-brightgreen.svg?style=flat [contributing-url]: https://
-github.com/rusty1s/pytorch_geometric/blob/master/CONTRIBUTING.md
+License: MIT Platform: UNKNOWN Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Science/Research Classifier: Programming Language :: Python :: 3.5 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Topic :: Scientific/Engineering :: Mathematics Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Software
+Development :: Libraries Description-Content-Type: text/markdown License-File:
+LICENSE [contributing-image]: https://img.shields.io/badge/contributions-
+welcome-brightgreen.svg?style=flat [contributing-url]: https://github.com/
+rusty1s/pytorch_geometric/blob/master/CONTRIBUTING.md
                                     [logo]
 --------------------- [GitHub last commit]_[_G_i_t_H_u_b_ _i_s_s_u_e_s_][GitHub][!
 [Contributing][contributing-image]][contributing-url] [![Tweet](https://
 img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://
 twitter.com/intent/
 tweet?text=Build%20your%20robust%20machine%20learning%20models%20with%20DeepRobust%20in%2060%20seconds&url=https:
 //github.com/DSE-MSU/
@@ -34,27 +42,33 @@
 Defenses on Graphs: A Review, A Tool and Empirical Studies](https://arxiv.org/
 abs/2003.00653) * [Adversarial Attacks and Defenses in Images, Graphs and Text:
 A Review](https://arxiv.org/pdf/1909.08072.pdf) If our work could help your
 research, please cite: [DeepRobust: A PyTorch Library for Adversarial Attacks
 and Defenses](https://arxiv.org/abs/2005.06149) ``` @article{li2020deeprobust,
 title={Deeprobust: A pytorch library for adversarial attacks and defenses},
 author={Li, Yaxin and Jin, Wei and Xu, Han and Tang, Jiliang}, journal={arXiv
-preprint arXiv:2005.06149}, year={2020} } ``` # Changelog * [02/2023]
-DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We have
-added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/2110.14038)
-to graph package. We can now use PRBCD to attack large-scale graphs such as
-ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/
+preprint arXiv:2005.06149}, year={2020} } ``` # Changelog * [11/2023]
+DeepRobust 0.2.9 Released. Please try `pip install deeprobust==0.2.9`. We have
+fixed the OOM issue of metattack on new pytorch versions. * [06/2023] We have
+added a backdoor attack [UGBA, WWW'23](https://arxiv.org/abs/2303.01263) to
+graph package. We can now use UGBA to conduct unnoticeable backdoor attack on
+large-scale graphs such as ogb-arxiv (see example in [test_ugba.py](https://
+github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_ugba.py))! * [02/
+2023] DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We
+have added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/
+2110.14038) to graph package. We can now use PRBCD to attack large-scale graphs
+such as ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/
 DeepRobust/blob/master/examples/graph/test_prbcd.py))! * [02/2023] Add a robust
 model [AirGNN, NeurIPS'21](https://proceedings.neurips.cc/paper/2021/file/
 50abc3e730e36b387ca8e02c26dc0a22-Paper.pdf) to graph package. Try `python
 examples/graph/test_airgnn.py`! See details in [test_airgnn.py](https://
 github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_airgnn.py) * [11/
 2022] DeepRobust 0.2.6 Released. Please try `pip install deeprobust==0.2.6`! We
 have more updates coming. Please stay tuned! * [11/2021] A subpackage that
-includes popular black box attacks in image domain is relased. Find it here.
+includes popular black box attacks in image domain is released. Find it here.
 [Link](https://github.com/I-am-Bot/Black-Box-Attacks) * [11/2021] DeepRobust
 0.2.4 Released. Please try `pip install deeprobust==0.2.4`! * [10/2021] add
 scalable attack and MedianGCN. Thank [Jintang](https://github.com/EdisonLeeeee)
 for his contribution! * [06/2021] [Image Package] Add preprocessing method:
 APE-GAN. * [05/2021] DeepRobust is published at AAAI 2021. Check [here](https:/
 /ojs.aaai.org/index.php/AAAI/article/view/18017)! * [05/2021] DeepRobust 0.2.2
 Released. Please try `pip install deeprobust==0.2.2`! * [04/2021] [Image
@@ -163,15 +177,8 @@
 Left:original, classified as 6; Right:adversary, classified as 4. Serveral
 trained models can be found here: https://drive.google.com/
 open?id=1uGLiuCyd8zCAQ8tPz9DDUQH6zm-C4tEL ## Acknowledgement Some of the
 algorithms are referred to paper authors' implementations. References can be
 found at the top of each file. Implementation of network structure are referred
 to weiaicunzai's github. Original code can be found here: [pytorch-cifar100]
 (https://github.com/weiaicunzai/pytorch-cifar100) Thanks to their outstanding
-works! Platform: UNKNOWN Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education Classifier: Intended Audience ::
-Science/Research Classifier: Programming Language :: Python :: 3.5 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Topic :: Scientific/Engineering :: Mathematics Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Software
-Development :: Libraries Description-Content-Type: text/markdown
+works!
```

### Comparing `deeprobust-0.2.8/README.md` & `deeprobust-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,20 @@
   author={Li, Yaxin and Jin, Wei and Xu, Han and Tang, Jiliang},
   journal={arXiv preprint arXiv:2005.06149},
   year={2020}
 }
 ```
 
 # Changelog
+* [11/2023] DeepRobust 0.2.9 Released. Please try `pip install deeprobust==0.2.9`. We have fixed the OOM issue of metattack on new pytorch versions.
+* [06/2023] We have added a backdoor attack [UGBA, WWW'23](https://arxiv.org/abs/2303.01263) to graph package. We can now use UGBA to conduct unnoticeable backdoor attack on large-scale graphs such as ogb-arxiv (see example in [test_ugba.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_ugba.py))! 
 * [02/2023] DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We have added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/2110.14038) to graph package. We can now use PRBCD to attack large-scale graphs such as ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_prbcd.py))! 
 * [02/2023] Add a robust model [AirGNN, NeurIPS'21](https://proceedings.neurips.cc/paper/2021/file/50abc3e730e36b387ca8e02c26dc0a22-Paper.pdf) to graph package. Try `python examples/graph/test_airgnn.py`! See details in [test_airgnn.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_airgnn.py)
 * [11/2022] DeepRobust 0.2.6 Released. Please try `pip install deeprobust==0.2.6`! We have more updates coming. Please stay tuned!
-* [11/2021] A subpackage that includes popular black box attacks in image domain is relased. Find it here. [Link](https://github.com/I-am-Bot/Black-Box-Attacks)
+* [11/2021] A subpackage that includes popular black box attacks in image domain is released. Find it here. [Link](https://github.com/I-am-Bot/Black-Box-Attacks)
 * [11/2021] DeepRobust 0.2.4 Released. Please try `pip install deeprobust==0.2.4`!
 * [10/2021] add scalable attack and MedianGCN. Thank [Jintang](https://github.com/EdisonLeeeee) for his contribution!
 * [06/2021] [Image Package] Add preprocessing method: APE-GAN.
 * [05/2021] DeepRobust is published at AAAI 2021. Check [here](https://ojs.aaai.org/index.php/AAAI/article/view/18017)!
 * [05/2021] DeepRobust 0.2.2 Released. Please try `pip install deeprobust==0.2.2`!
 * [04/2021] [Image Package] Add support for ImageNet. See details in [test_ImageNet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/image/test_ImageNet.py)
 * [04/2021] [Graph Package] Add support for OGB datasets.  See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html).
```

#### html2text {}

```diff
@@ -31,27 +31,33 @@
 Defenses on Graphs: A Review, A Tool and Empirical Studies](https://arxiv.org/
 abs/2003.00653) * [Adversarial Attacks and Defenses in Images, Graphs and Text:
 A Review](https://arxiv.org/pdf/1909.08072.pdf) If our work could help your
 research, please cite: [DeepRobust: A PyTorch Library for Adversarial Attacks
 and Defenses](https://arxiv.org/abs/2005.06149) ``` @article{li2020deeprobust,
 title={Deeprobust: A pytorch library for adversarial attacks and defenses},
 author={Li, Yaxin and Jin, Wei and Xu, Han and Tang, Jiliang}, journal={arXiv
-preprint arXiv:2005.06149}, year={2020} } ``` # Changelog * [02/2023]
-DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We have
-added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/2110.14038)
-to graph package. We can now use PRBCD to attack large-scale graphs such as
-ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/
+preprint arXiv:2005.06149}, year={2020} } ``` # Changelog * [11/2023]
+DeepRobust 0.2.9 Released. Please try `pip install deeprobust==0.2.9`. We have
+fixed the OOM issue of metattack on new pytorch versions. * [06/2023] We have
+added a backdoor attack [UGBA, WWW'23](https://arxiv.org/abs/2303.01263) to
+graph package. We can now use UGBA to conduct unnoticeable backdoor attack on
+large-scale graphs such as ogb-arxiv (see example in [test_ugba.py](https://
+github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_ugba.py))! * [02/
+2023] DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We
+have added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/
+2110.14038) to graph package. We can now use PRBCD to attack large-scale graphs
+such as ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/
 DeepRobust/blob/master/examples/graph/test_prbcd.py))! * [02/2023] Add a robust
 model [AirGNN, NeurIPS'21](https://proceedings.neurips.cc/paper/2021/file/
 50abc3e730e36b387ca8e02c26dc0a22-Paper.pdf) to graph package. Try `python
 examples/graph/test_airgnn.py`! See details in [test_airgnn.py](https://
 github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_airgnn.py) * [11/
 2022] DeepRobust 0.2.6 Released. Please try `pip install deeprobust==0.2.6`! We
 have more updates coming. Please stay tuned! * [11/2021] A subpackage that
-includes popular black box attacks in image domain is relased. Find it here.
+includes popular black box attacks in image domain is released. Find it here.
 [Link](https://github.com/I-am-Bot/Black-Box-Attacks) * [11/2021] DeepRobust
 0.2.4 Released. Please try `pip install deeprobust==0.2.4`! * [10/2021] add
 scalable attack and MedianGCN. Thank [Jintang](https://github.com/EdisonLeeeee)
 for his contribution! * [06/2021] [Image Package] Add preprocessing method:
 APE-GAN. * [05/2021] DeepRobust is published at AAAI 2021. Check [here](https:/
 /ojs.aaai.org/index.php/AAAI/article/view/18017)! * [05/2021] DeepRobust 0.2.2
 Released. Please try `pip install deeprobust==0.2.2`! * [04/2021] [Image
```

### Comparing `deeprobust-0.2.8/deeprobust/graph/black_box.py` & `deeprobust-0.2.9/deeprobust/graph/black_box.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/data/__init__.py` & `deeprobust-0.2.9/deeprobust/graph/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/data/attacked_data.py` & `deeprobust-0.2.9/deeprobust/graph/data/attacked_data.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/data/dataset.py` & `deeprobust-0.2.9/deeprobust/graph/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                         " choosen from ['gcn', 'nettack', 'prognn']"
 
         self.seed = seed
         # self.url =  'https://raw.githubusercontent.com/danielzuegner/nettack/master/data/%s.npz' % self.name
         self.url =  'https://raw.githubusercontent.com/danielzuegner/gnn-meta-attack/master/data/%s.npz' % self.name
 
         if platform.system() == 'Windows':
-            root = root
+            self.root = root
         else:
         	self.root = osp.expanduser(osp.normpath(root))
 
         self.data_folder = osp.join(root, self.name)
         self.data_filename = self.data_folder + '.npz'
         self.require_mask = require_mask
```

### Comparing `deeprobust-0.2.8/deeprobust/graph/data/pyg_dataset.py` & `deeprobust-0.2.9/deeprobust/graph/data/pyg_dataset.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/__init__.py` & `deeprobust-0.2.9/deeprobust/graph/defense/__init__.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/adv_training.py` & `deeprobust-0.2.9/deeprobust/graph/defense/adv_training.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/chebnet.py` & `deeprobust-0.2.9/deeprobust/graph/defense/chebnet.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/gat.py` & `deeprobust-0.2.9/deeprobust/graph/defense/gat.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/gcn.py` & `deeprobust-0.2.9/deeprobust/graph/defense/gcn.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/gcn_preprocess.py` & `deeprobust-0.2.9/deeprobust/graph/defense/gcn_preprocess.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/median_gcn.py` & `deeprobust-0.2.9/deeprobust/graph/defense/median_gcn.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/node_embedding.py` & `deeprobust-0.2.9/deeprobust/graph/defense/node_embedding.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/pgd.py` & `deeprobust-0.2.9/deeprobust/graph/defense/pgd.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/prognn.py` & `deeprobust-0.2.9/deeprobust/graph/defense/prognn.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/r_gcn.py` & `deeprobust-0.2.9/deeprobust/graph/defense/r_gcn.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/sgc.py` & `deeprobust-0.2.9/deeprobust/graph/defense/sgc.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense/simpgcn.py` & `deeprobust-0.2.9/deeprobust/graph/defense/simpgcn.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/__init__.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/__init__.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/airgnn.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/airgnn.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/appnp.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/appnp.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/base_model.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/base_model.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/gat.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/gat.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/gcn.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/gcn.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/gpr.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/gpr.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/mygat_conv.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/mygat_conv.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/defense_pyg/sage.py` & `deeprobust-0.2.9/deeprobust/graph/defense_pyg/sage.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/__init__.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/__init__.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/base_attack.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/base_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/dice.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/dice.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/mettack.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/mettack.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,17 +121,17 @@
                                                                     ori_adj, t_d_min,
                                                                     ll_cutoff, undirected=self.undirected)
         return allowed_mask, current_ratio
 
     def get_adj_score(self, adj_grad, modified_adj, ori_adj, ll_constraint, ll_cutoff):
         adj_meta_grad = adj_grad * (-2 * modified_adj + 1)
         # Make sure that the minimum entry is 0.
-        adj_meta_grad -= adj_meta_grad.min()
+        adj_meta_grad = adj_meta_grad - adj_meta_grad.min()
         # Filter self-loops
-        adj_meta_grad -= torch.diag(torch.diag(adj_meta_grad, 0))
+        adj_meta_grad = adj_meta_grad - torch.diag(torch.diag(adj_meta_grad, 0))
         # # Set entries to 0 that could lead to singleton nodes.
         singleton_mask = self.filter_potential_singletons(modified_adj)
         adj_meta_grad = adj_meta_grad *  singleton_mask
 
         if ll_constraint:
             allowed_mask, self.ll_ratio = self.log_likelihood_constraint(modified_adj, ori_adj, ll_cutoff)
             allowed_mask = allowed_mask.to(self.device)
```

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/nipa.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/nipa.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/node_embedding_attack.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/node_embedding_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/prbcd.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/prbcd.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/random_attack.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/random_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/global_attack/topology_attack.py` & `deeprobust-0.2.9/deeprobust/graph/global_attack/topology_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/env.py` & `deeprobust-0.2.9/deeprobust/graph/rl/env.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/nipa_config.py` & `deeprobust-0.2.9/deeprobust/graph/rl/nipa_config.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/nipa_env.py` & `deeprobust-0.2.9/deeprobust/graph/rl/nipa_env.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/nipa_nstep_replay_mem.py` & `deeprobust-0.2.9/deeprobust/graph/rl/nipa_nstep_replay_mem.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/nipa_q_net_node.py` & `deeprobust-0.2.9/deeprobust/graph/rl/nipa_q_net_node.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/nstep_replay_mem.py` & `deeprobust-0.2.9/deeprobust/graph/rl/nstep_replay_mem.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/q_net_node.py` & `deeprobust-0.2.9/deeprobust/graph/rl/q_net_node.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/rl_s2v_config.py` & `deeprobust-0.2.9/deeprobust/graph/rl/rl_s2v_config.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/rl/rl_s2v_env.py` & `deeprobust-0.2.9/deeprobust/graph/rl/rl_s2v_env.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/targeted_attack/base_attack.py` & `deeprobust-0.2.9/deeprobust/graph/targeted_attack/base_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/targeted_attack/fga.py` & `deeprobust-0.2.9/deeprobust/graph/targeted_attack/fga.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/targeted_attack/ig_attack.py` & `deeprobust-0.2.9/deeprobust/graph/targeted_attack/ig_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/targeted_attack/nettack.py` & `deeprobust-0.2.9/deeprobust/graph/targeted_attack/nettack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/targeted_attack/rl_s2v.py` & `deeprobust-0.2.9/deeprobust/graph/targeted_attack/rl_s2v.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/targeted_attack/rnd.py` & `deeprobust-0.2.9/deeprobust/graph/targeted_attack/rnd.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/targeted_attack/sga.py` & `deeprobust-0.2.9/deeprobust/graph/targeted_attack/sga.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/utils.py` & `deeprobust-0.2.9/deeprobust/graph/utils.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/graph/visualization.py` & `deeprobust-0.2.9/deeprobust/graph/visualization.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/BPDA.py` & `deeprobust-0.2.9/deeprobust/image/attack/BPDA.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/Nattack.py` & `deeprobust-0.2.9/deeprobust/image/attack/Nattack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/Universal.py` & `deeprobust-0.2.9/deeprobust/image/attack/Universal.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/YOPOpgd.py` & `deeprobust-0.2.9/deeprobust/image/attack/YOPOpgd.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/base_attack.py` & `deeprobust-0.2.9/deeprobust/image/attack/base_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/cw.py` & `deeprobust-0.2.9/deeprobust/image/attack/cw.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/deepfool.py` & `deeprobust-0.2.9/deeprobust/image/attack/deepfool.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/fgsm.py` & `deeprobust-0.2.9/deeprobust/image/attack/fgsm.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/l2_attack.py` & `deeprobust-0.2.9/deeprobust/image/attack/l2_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/lbfgs.py` & `deeprobust-0.2.9/deeprobust/image/attack/lbfgs.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/onepixel.py` & `deeprobust-0.2.9/deeprobust/image/attack/onepixel.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/attack/pgd.py` & `deeprobust-0.2.9/deeprobust/image/attack/pgd.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/config.py` & `deeprobust-0.2.9/deeprobust/image/config.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/AWP.py` & `deeprobust-0.2.9/deeprobust/image/defense/AWP.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/LIDclassifier.py` & `deeprobust-0.2.9/deeprobust/image/defense/LIDclassifier.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/TherEncoding.py` & `deeprobust-0.2.9/deeprobust/image/defense/TherEncoding.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/YOPO.py` & `deeprobust-0.2.9/deeprobust/image/defense/YOPO.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/base_defense.py` & `deeprobust-0.2.9/deeprobust/image/defense/base_defense.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/fast.py` & `deeprobust-0.2.9/deeprobust/image/defense/fast.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/fgsmtraining.py` & `deeprobust-0.2.9/deeprobust/image/defense/fgsmtraining.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/pgdtraining.py` & `deeprobust-0.2.9/deeprobust/image/defense/pgdtraining.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/defense/trades.py` & `deeprobust-0.2.9/deeprobust/image/defense/trades.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/evaluation_attack.py` & `deeprobust-0.2.9/deeprobust/image/evaluation_attack.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/CNN.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/CNN.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/CNN_multilayer.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/CNN_multilayer.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/YOPOCNN.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/YOPOCNN.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/densenet.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/densenet.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/preact_resnet.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/preact_resnet.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/resnet.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/resnet.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/train_model.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/train_model.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/train_resnet.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/train_resnet.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/netmodels/vgg.py` & `deeprobust-0.2.9/deeprobust/image/netmodels/vgg.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/optimizer.py` & `deeprobust-0.2.9/deeprobust/image/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust/image/utils.py` & `deeprobust-0.2.9/deeprobust/image/utils.py`

 * *Files identical despite different names*

### Comparing `deeprobust-0.2.8/deeprobust.egg-info/PKG-INFO` & `deeprobust-0.2.9/deeprobust.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,330 +1,335 @@
 Metadata-Version: 2.1
 Name: deeprobust
-Version: 0.2.8
+Version: 0.2.9
 Summary: A PyTorch library for adversarial robustness learning for image and graph data.
 Home-page: https://github.com/DSE-MSU/DeepRobust
 Author: MSU-DSE
 Maintainer: MSU-DSE
 License: MIT
-Description: 
-        [contributing-image]: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
-        [contributing-url]: https://github.com/rusty1s/pytorch_geometric/blob/master/CONTRIBUTING.md
-        
-        <p align="center">
-        <img center src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/Deeprobust.png" width = "450" alt="logo">
-        </p>
-        
-        ---------------------
-        <!--
-        <a href="https://github.com/DSE-MSU/DeepRobust/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/DSE-MSU/DeepRobust"></a>  <a href="https://github.com/DSE-MSU/DeepRobust/network/members" ><img alt="GitHub forks" src="https://img.shields.io/github/forks/DSE-MSU/DeepRobust">
-        </a> 
-        -->
-        
-        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/DSE-MSU/DeepRobust"> <a href="https://github.com/DSE-MSU/DeepRobust/issues"> <img alt="GitHub issues" src="https://img.shields.io/github/issues/DSE-MSU/DeepRobust"></a> <img alt="GitHub" src="https://img.shields.io/github/license/DSE-MSU/DeepRobust">
-        [![Contributing][contributing-image]][contributing-url]
-        [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20your%20robust%20machine%20learning%20models%20with%20DeepRobust%20in%2060%20seconds&url=https://github.com/DSE-MSU/DeepRobust&via=dse_msu&hashtags=MachineLearning,DeepLearning,secruity,data,developers)
-        
-        
-        <!-- <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/DSE-MSU/DeepRobust"> -->
-        
-        <!--
-        <div align=center><img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversarial.png" width="500"/></div>
-        <div align=center><img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/graph_attack_example.png" width="00" /></div>
-        -->
-        **[Documentation](https://deeprobust.readthedocs.io/en/latest/)** | **[Paper](https://arxiv.org/abs/2005.06149)** | **[Samples](https://github.com/DSE-MSU/DeepRobust/tree/master/examples)** 
-        
-        [AAAI 2021] DeepRobust is a PyTorch adversarial library for attack and defense methods on images and graphs. 
-        * If you are new to DeepRobust, we highly suggest you read the [documentation page](https://deeprobust.readthedocs.io/en/latest/) or the following content in this README to learn how to use it.  
-        * If you have any questions or suggestions regarding this library, feel free to create an issue [here](https://github.com/DSE-MSU/DeepRobust/issues). We will reply as soon as possible :)
-        
-        <p float="left">
-          <img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/adversarial.png" width="430" />
-          <img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/graph_attack_example.png" width="380" /> 
-        </p>
-        
-        **List of including algorithms can be found in [[Image Package]](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/image) and [[Graph Package]](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph).**
-        
-        [Environment & Installation](#environment)
-        
-        Usage
-        
-        * [Image Attack and Defense](#image-attack-and-defense)
-        
-        * [Graph Attack and Defense](#graph-attack-and-defense)
-        
-        [Acknowledgement](#acknowledgement) 
-        
-        For more details about attacks and defenses, you can read the following papers.
-        * [Adversarial Attacks and Defenses on Graphs: A Review, A Tool and Empirical Studies](https://arxiv.org/abs/2003.00653)
-        * [Adversarial Attacks and Defenses in Images, Graphs and Text: A Review](https://arxiv.org/pdf/1909.08072.pdf)
-        
-        If our work could help your research, please cite:
-        [DeepRobust: A PyTorch Library for Adversarial Attacks and Defenses](https://arxiv.org/abs/2005.06149)
-        ```
-        @article{li2020deeprobust,
-          title={Deeprobust: A pytorch library for adversarial attacks and defenses},
-          author={Li, Yaxin and Jin, Wei and Xu, Han and Tang, Jiliang},
-          journal={arXiv preprint arXiv:2005.06149},
-          year={2020}
-        }
-        ```
-        
-        # Changelog
-        * [02/2023] DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We have added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/2110.14038) to graph package. We can now use PRBCD to attack large-scale graphs such as ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_prbcd.py))! 
-        * [02/2023] Add a robust model [AirGNN, NeurIPS'21](https://proceedings.neurips.cc/paper/2021/file/50abc3e730e36b387ca8e02c26dc0a22-Paper.pdf) to graph package. Try `python examples/graph/test_airgnn.py`! See details in [test_airgnn.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_airgnn.py)
-        * [11/2022] DeepRobust 0.2.6 Released. Please try `pip install deeprobust==0.2.6`! We have more updates coming. Please stay tuned!
-        * [11/2021] A subpackage that includes popular black box attacks in image domain is relased. Find it here. [Link](https://github.com/I-am-Bot/Black-Box-Attacks)
-        * [11/2021] DeepRobust 0.2.4 Released. Please try `pip install deeprobust==0.2.4`!
-        * [10/2021] add scalable attack and MedianGCN. Thank [Jintang](https://github.com/EdisonLeeeee) for his contribution!
-        * [06/2021] [Image Package] Add preprocessing method: APE-GAN.
-        * [05/2021] DeepRobust is published at AAAI 2021. Check [here](https://ojs.aaai.org/index.php/AAAI/article/view/18017)!
-        * [05/2021] DeepRobust 0.2.2 Released. Please try `pip install deeprobust==0.2.2`!
-        * [04/2021] [Image Package] Add support for ImageNet. See details in [test_ImageNet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/image/test_ImageNet.py)
-        * [04/2021] [Graph Package] Add support for OGB datasets.  See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html).
-        * [03/2021] [Graph Package] Added node embedding attack and victim models! See this [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/node_embedding.html).
-        * [02/2021] **[Graph Package] DeepRobust now provides tools for converting the datasets between [Pytorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/) and DeepRobust. See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html)!** DeepRobust now also support GAT, Chebnet and SGC based on pyg; see details in [test_gat.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_gat.py),  [test_chebnet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_chebnet.py) and [test_sgc.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_sgc.py)
-        * [12/2020] DeepRobust now can be installed via pip! Try `pip install deeprobust`!
-        * [12/2020] [Graph Package] Add four more [datasets](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph/#supported-datasets) and one defense algorithm. More details can be found [here](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph/#defense-methods). More datasets and algorithms will be added later. Stay tuned :)
-        * [07/2020] Add [documentation](https://deeprobust.readthedocs.io/en/latest/) page!
-        * [06/2020] Add docstring to both image and graph package
-        
-        # Basic Environment
-        * `python >= 3.6` (python 3.5 should also work)
-        * `pytorch >= 1.2.0`
-        
-        see `setup.py` or `requirements.txt` for more information.
-        
-        # Installation
-        ## Install from pip
-        ```
-        pip install deeprobust 
-        ```
-        ## Install from source
-        ```
-        git clone https://github.com/DSE-MSU/DeepRobust.git
-        cd DeepRobust
-        python setup.py install
-        ```
-        
-        # Test Examples
-        
-        ```
-        python examples/image/test_PGD.py
-        python examples/image/test_pgdtraining.py
-        python examples/graph/test_gcn_jaccard.py --dataset cora
-        python examples/graph/test_mettack.py --dataset cora --ptb_rate 0.05
-        ```
-        
-        # Usage
-        ## Image Attack and Defense
-        1. Train model
-        
-            Example: Train a simple CNN model on MNIST dataset for 20 epoch on gpu.
-            ```python
-            import deeprobust.image.netmodels.train_model as trainmodel
-            trainmodel.train('CNN', 'MNIST', 'cuda', 20)
-            ```
-            Model would be saved in deeprobust/trained_models/.
-        
-        2. Instantiated attack methods and defense methods.
-        
-            Example: Generate adversary example with PGD attack.
-            ```python
-            from deeprobust.image.attack.pgd import PGD
-            from deeprobust.image.config import attack_params
-            from deeprobust.image.utils import download_model
-            import torch
-            import deeprobust.image.netmodels.resnet as resnet
-            from torchvision import transforms,datasets
-            
-            URL = "https://github.com/I-am-Bot/deeprobust_model/raw/master/CIFAR10_ResNet18_epoch_20.pt"
-            download_model(URL, "$MODEL_PATH$")
-        
-            model = resnet.ResNet18().to('cuda')
-            model.load_state_dict(torch.load("$MODEL_PATH$"))
-            model.eval()
-        
-            transform_val = transforms.Compose([transforms.ToTensor()])
-            test_loader  = torch.utils.data.DataLoader(
-                            datasets.CIFAR10('deeprobust/image/data', train = False, download=True,
-                            transform = transform_val),
-                            batch_size = 10, shuffle=True)
-        
-            x, y = next(iter(test_loader))
-            x = x.to('cuda').float()
-            
-            adversary = PGD(model, 'cuda')
-            Adv_img = adversary.generate(x, y, **attack_params['PGD_CIFAR10'])
-            ```
-        
-            Example: Train defense model.
-            ```python
-            from deeprobust.image.defense.pgdtraining import PGDtraining
-            from deeprobust.image.config import defense_params
-            from deeprobust.image.netmodels.CNN import Net
-            import torch
-            from torchvision import datasets, transforms 
-            
-            model = Net()
-            train_loader = torch.utils.data.DataLoader(
-                            datasets.MNIST('deeprobust/image/defense/data', train=True, download=True,
-                                            transform=transforms.Compose([transforms.ToTensor()])),
-                                            batch_size=100,shuffle=True)
-        
-            test_loader = torch.utils.data.DataLoader(
-                          datasets.MNIST('deeprobust/image/defense/data', train=False,
-                                        transform=transforms.Compose([transforms.ToTensor()])),
-                                        batch_size=1000,shuffle=True)
-        
-            defense = PGDtraining(model, 'cuda')
-            defense.generate(train_loader, test_loader, **defense_params["PGDtraining_MNIST"])
-            ```
-        
-            More example code can be found in deeprobust/examples.
-        
-        3. Use our evulation program to test attack algorithm against defense.
-        
-            Example:
-            ```
-            cd DeepRobust
-            python examples/image/test_train.py
-            python deeprobust/image/evaluation_attack.py
-            ```
-        
-        ## Graph Attack and Defense 
-        
-        ### Attacking Graph Neural Networks
-        
-        1. Load dataset
-            ```python
-            import torch
-            import numpy as np
-            from deeprobust.graph.data import Dataset
-            from deeprobust.graph.defense import GCN
-            from deeprobust.graph.global_attack import Metattack
-        
-            data = Dataset(root='/tmp/', name='cora', setting='nettack')
-            adj, features, labels = data.adj, data.features, data.labels
-            idx_train, idx_val, idx_test = data.idx_train, data.idx_val, data.idx_test
-            idx_unlabeled = np.union1d(idx_val, idx_test)
-            ```
-        
-        2. Set up surrogate model
-            ```python
-            device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-            surrogate = GCN(nfeat=features.shape[1], nclass=labels.max().item()+1, nhid=16,
-                            with_relu=False, device=device)
-            surrogate = surrogate.to(device)
-            surrogate.fit(features, adj, labels, idx_train)
-            ```
-        
-        
-        3. Set up attack model and generate perturbations
-            ```python
-            model = Metattack(model=surrogate, nnodes=adj.shape[0], feature_shape=features.shape, device=device)
-            model = model.to(device)
-            perturbations = int(0.05 * (adj.sum() // 2))
-            model.attack(features, adj, labels, idx_train, idx_unlabeled, perturbations, ll_constraint=False)
-            modified_adj = model.modified_adj
-            ```
-            
-        For more details please refer to [mettack.py](https://github.com/I-am-Bot/DeepRobust/blob/master/examples/graph/test_mettack.py) or run 
-            ```
-            python examples/graph/test_mettack.py --dataset cora --ptb_rate 0.05
-            ```
-        
-        ### Defending Against Graph Attacks
-        
-        1. Load dataset
-            ```python
-            import torch
-            from deeprobust.graph.data import Dataset, PtbDataset
-            from deeprobust.graph.defense import GCN, GCNJaccard
-            import numpy as np
-            np.random.seed(15)
-        
-            # load clean graph
-            data = Dataset(root='/tmp/', name='cora', setting='nettack')
-            adj, features, labels = data.adj, data.features, data.labels
-            idx_train, idx_val, idx_test = data.idx_train, data.idx_val, data.idx_test
-        
-            # load pre-attacked graph by mettack
-            perturbed_data = PtbDataset(root='/tmp/', name='cora')
-            perturbed_adj = perturbed_data.adj
-            ```
-        2. Test 
-            ```python
-            # Set up defense model and test performance
-            device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-            model = GCNJaccard(nfeat=features.shape[1], nclass=labels.max()+1, nhid=16, device=device)
-            model = model.to(device)
-            model.fit(features, perturbed_adj, labels, idx_train)
-            model.eval()
-            output = model.test(idx_test)
-        
-            # Test on GCN
-            model = GCN(nfeat=features.shape[1], nclass=labels.max()+1, nhid=16, device=device)
-            model = model.to(device)
-            model.fit(features, perturbed_adj, labels, idx_train)
-            model.eval()
-            output = model.test(idx_test)
-            ```
-            
-        For more details please refer to [test_gcn_jaccard.py](https://github.com/I-am-Bot/DeepRobust/blob/master/examples/graph/test_gcn_jaccard.py) or run
-            ```
-            python examples/graph/test_gcn_jaccard.py --dataset cora
-            ```
-        
-        ## Sample Results
-        adversary examples generated by fgsm:
-        <div align="center">
-        <img height=140 src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/mnist_advexample_fgsm_ori.png"/><img height=140 src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/mnist_advexample_fgsm_adv.png"/>
-        </div>
-        Left:original, classified as 6; Right:adversary, classified as 4.
-        
-        Serveral trained models can be found here: https://drive.google.com/open?id=1uGLiuCyd8zCAQ8tPz9DDUQH6zm-C4tEL
-        
-        ## Acknowledgement
-        Some of the algorithms are referred to paper authors' implementations. References can be found at the top of each file. 
-        
-        Implementation of network structure are referred to weiaicunzai's github. Original code can be found here:
-        [pytorch-cifar100](https://github.com/weiaicunzai/pytorch-cifar100)
-        
-        Thanks to their outstanding works!
-        
-        
-        <!----
-        We would be glad if you find our work useful and cite the paper.
-        
-        '''
-        @misc{jin2020adversarial,
-            title={Adversarial Attacks and Defenses on Graphs: A Review and Empirical Study},
-            author={Wei Jin and Yaxin Li and Han Xu and Yiqi Wang and Jiliang Tang},
-            year={2020},
-            eprint={2003.00653},
-            archivePrefix={arXiv},
-            primaryClass={cs.LG}
-        }
-        '''
-        ```
-        @article{xu2019adversarial,
-          title={Adversarial attacks and defenses in images, graphs and text: A review},
-          author={Xu, Han and Ma, Yao and Liu, Haochen and Deb, Debayan and Liu, Hui and Tang, Jiliang and Jain, Anil},
-          journal={arXiv preprint arXiv:1909.08072},
-          year={2019}
-        }
-        ```
-        ---->
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[contributing-image]: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
+[contributing-url]: https://github.com/rusty1s/pytorch_geometric/blob/master/CONTRIBUTING.md
+
+<p align="center">
+<img center src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/Deeprobust.png" width = "450" alt="logo">
+</p>
+
+---------------------
+<!--
+<a href="https://github.com/DSE-MSU/DeepRobust/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/DSE-MSU/DeepRobust"></a>  <a href="https://github.com/DSE-MSU/DeepRobust/network/members" ><img alt="GitHub forks" src="https://img.shields.io/github/forks/DSE-MSU/DeepRobust">
+</a> 
+-->
+
+<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/DSE-MSU/DeepRobust"> <a href="https://github.com/DSE-MSU/DeepRobust/issues"> <img alt="GitHub issues" src="https://img.shields.io/github/issues/DSE-MSU/DeepRobust"></a> <img alt="GitHub" src="https://img.shields.io/github/license/DSE-MSU/DeepRobust">
+[![Contributing][contributing-image]][contributing-url]
+[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Build%20your%20robust%20machine%20learning%20models%20with%20DeepRobust%20in%2060%20seconds&url=https://github.com/DSE-MSU/DeepRobust&via=dse_msu&hashtags=MachineLearning,DeepLearning,secruity,data,developers)
+
+
+<!-- <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/DSE-MSU/DeepRobust"> -->
+
+<!--
+<div align=center><img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversarial.png" width="500"/></div>
+<div align=center><img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/graph_attack_example.png" width="00" /></div>
+-->
+**[Documentation](https://deeprobust.readthedocs.io/en/latest/)** | **[Paper](https://arxiv.org/abs/2005.06149)** | **[Samples](https://github.com/DSE-MSU/DeepRobust/tree/master/examples)** 
+
+[AAAI 2021] DeepRobust is a PyTorch adversarial library for attack and defense methods on images and graphs. 
+* If you are new to DeepRobust, we highly suggest you read the [documentation page](https://deeprobust.readthedocs.io/en/latest/) or the following content in this README to learn how to use it.  
+* If you have any questions or suggestions regarding this library, feel free to create an issue [here](https://github.com/DSE-MSU/DeepRobust/issues). We will reply as soon as possible :)
+
+<p float="left">
+  <img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/adversarial.png" width="430" />
+  <img src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/graph_attack_example.png" width="380" /> 
+</p>
+
+**List of including algorithms can be found in [[Image Package]](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/image) and [[Graph Package]](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph).**
+
+[Environment & Installation](#environment)
+
+Usage
+
+* [Image Attack and Defense](#image-attack-and-defense)
+
+* [Graph Attack and Defense](#graph-attack-and-defense)
+
+[Acknowledgement](#acknowledgement) 
+
+For more details about attacks and defenses, you can read the following papers.
+* [Adversarial Attacks and Defenses on Graphs: A Review, A Tool and Empirical Studies](https://arxiv.org/abs/2003.00653)
+* [Adversarial Attacks and Defenses in Images, Graphs and Text: A Review](https://arxiv.org/pdf/1909.08072.pdf)
+
+If our work could help your research, please cite:
+[DeepRobust: A PyTorch Library for Adversarial Attacks and Defenses](https://arxiv.org/abs/2005.06149)
+```
+@article{li2020deeprobust,
+  title={Deeprobust: A pytorch library for adversarial attacks and defenses},
+  author={Li, Yaxin and Jin, Wei and Xu, Han and Tang, Jiliang},
+  journal={arXiv preprint arXiv:2005.06149},
+  year={2020}
+}
+```
+
+# Changelog
+* [11/2023] DeepRobust 0.2.9 Released. Please try `pip install deeprobust==0.2.9`. We have fixed the OOM issue of metattack on new pytorch versions.
+* [06/2023] We have added a backdoor attack [UGBA, WWW'23](https://arxiv.org/abs/2303.01263) to graph package. We can now use UGBA to conduct unnoticeable backdoor attack on large-scale graphs such as ogb-arxiv (see example in [test_ugba.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_ugba.py))! 
+* [02/2023] DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We have added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/2110.14038) to graph package. We can now use PRBCD to attack large-scale graphs such as ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_prbcd.py))! 
+* [02/2023] Add a robust model [AirGNN, NeurIPS'21](https://proceedings.neurips.cc/paper/2021/file/50abc3e730e36b387ca8e02c26dc0a22-Paper.pdf) to graph package. Try `python examples/graph/test_airgnn.py`! See details in [test_airgnn.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_airgnn.py)
+* [11/2022] DeepRobust 0.2.6 Released. Please try `pip install deeprobust==0.2.6`! We have more updates coming. Please stay tuned!
+* [11/2021] A subpackage that includes popular black box attacks in image domain is released. Find it here. [Link](https://github.com/I-am-Bot/Black-Box-Attacks)
+* [11/2021] DeepRobust 0.2.4 Released. Please try `pip install deeprobust==0.2.4`!
+* [10/2021] add scalable attack and MedianGCN. Thank [Jintang](https://github.com/EdisonLeeeee) for his contribution!
+* [06/2021] [Image Package] Add preprocessing method: APE-GAN.
+* [05/2021] DeepRobust is published at AAAI 2021. Check [here](https://ojs.aaai.org/index.php/AAAI/article/view/18017)!
+* [05/2021] DeepRobust 0.2.2 Released. Please try `pip install deeprobust==0.2.2`!
+* [04/2021] [Image Package] Add support for ImageNet. See details in [test_ImageNet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/image/test_ImageNet.py)
+* [04/2021] [Graph Package] Add support for OGB datasets.  See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html).
+* [03/2021] [Graph Package] Added node embedding attack and victim models! See this [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/node_embedding.html).
+* [02/2021] **[Graph Package] DeepRobust now provides tools for converting the datasets between [Pytorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/) and DeepRobust. See more details in the [tutorial page](https://deeprobust.readthedocs.io/en/latest/graph/pyg.html)!** DeepRobust now also support GAT, Chebnet and SGC based on pyg; see details in [test_gat.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_gat.py),  [test_chebnet.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_chebnet.py) and [test_sgc.py](https://github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_sgc.py)
+* [12/2020] DeepRobust now can be installed via pip! Try `pip install deeprobust`!
+* [12/2020] [Graph Package] Add four more [datasets](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph/#supported-datasets) and one defense algorithm. More details can be found [here](https://github.com/DSE-MSU/DeepRobust/tree/master/deeprobust/graph/#defense-methods). More datasets and algorithms will be added later. Stay tuned :)
+* [07/2020] Add [documentation](https://deeprobust.readthedocs.io/en/latest/) page!
+* [06/2020] Add docstring to both image and graph package
+
+# Basic Environment
+* `python >= 3.6` (python 3.5 should also work)
+* `pytorch >= 1.2.0`
+
+see `setup.py` or `requirements.txt` for more information.
+
+# Installation
+## Install from pip
+```
+pip install deeprobust 
+```
+## Install from source
+```
+git clone https://github.com/DSE-MSU/DeepRobust.git
+cd DeepRobust
+python setup.py install
+```
+
+# Test Examples
+
+```
+python examples/image/test_PGD.py
+python examples/image/test_pgdtraining.py
+python examples/graph/test_gcn_jaccard.py --dataset cora
+python examples/graph/test_mettack.py --dataset cora --ptb_rate 0.05
+```
+
+# Usage
+## Image Attack and Defense
+1. Train model
+
+    Example: Train a simple CNN model on MNIST dataset for 20 epoch on gpu.
+    ```python
+    import deeprobust.image.netmodels.train_model as trainmodel
+    trainmodel.train('CNN', 'MNIST', 'cuda', 20)
+    ```
+    Model would be saved in deeprobust/trained_models/.
+
+2. Instantiated attack methods and defense methods.
+
+    Example: Generate adversary example with PGD attack.
+    ```python
+    from deeprobust.image.attack.pgd import PGD
+    from deeprobust.image.config import attack_params
+    from deeprobust.image.utils import download_model
+    import torch
+    import deeprobust.image.netmodels.resnet as resnet
+    from torchvision import transforms,datasets
+    
+    URL = "https://github.com/I-am-Bot/deeprobust_model/raw/master/CIFAR10_ResNet18_epoch_20.pt"
+    download_model(URL, "$MODEL_PATH$")
+
+    model = resnet.ResNet18().to('cuda')
+    model.load_state_dict(torch.load("$MODEL_PATH$"))
+    model.eval()
+
+    transform_val = transforms.Compose([transforms.ToTensor()])
+    test_loader  = torch.utils.data.DataLoader(
+                    datasets.CIFAR10('deeprobust/image/data', train = False, download=True,
+                    transform = transform_val),
+                    batch_size = 10, shuffle=True)
+
+    x, y = next(iter(test_loader))
+    x = x.to('cuda').float()
+    
+    adversary = PGD(model, 'cuda')
+    Adv_img = adversary.generate(x, y, **attack_params['PGD_CIFAR10'])
+    ```
+
+    Example: Train defense model.
+    ```python
+    from deeprobust.image.defense.pgdtraining import PGDtraining
+    from deeprobust.image.config import defense_params
+    from deeprobust.image.netmodels.CNN import Net
+    import torch
+    from torchvision import datasets, transforms 
+    
+    model = Net()
+    train_loader = torch.utils.data.DataLoader(
+                    datasets.MNIST('deeprobust/image/defense/data', train=True, download=True,
+                                    transform=transforms.Compose([transforms.ToTensor()])),
+                                    batch_size=100,shuffle=True)
+
+    test_loader = torch.utils.data.DataLoader(
+                  datasets.MNIST('deeprobust/image/defense/data', train=False,
+                                transform=transforms.Compose([transforms.ToTensor()])),
+                                batch_size=1000,shuffle=True)
+
+    defense = PGDtraining(model, 'cuda')
+    defense.generate(train_loader, test_loader, **defense_params["PGDtraining_MNIST"])
+    ```
+
+    More example code can be found in deeprobust/examples.
+
+3. Use our evulation program to test attack algorithm against defense.
+
+    Example:
+    ```
+    cd DeepRobust
+    python examples/image/test_train.py
+    python deeprobust/image/evaluation_attack.py
+    ```
+
+## Graph Attack and Defense 
+
+### Attacking Graph Neural Networks
+
+1. Load dataset
+    ```python
+    import torch
+    import numpy as np
+    from deeprobust.graph.data import Dataset
+    from deeprobust.graph.defense import GCN
+    from deeprobust.graph.global_attack import Metattack
+
+    data = Dataset(root='/tmp/', name='cora', setting='nettack')
+    adj, features, labels = data.adj, data.features, data.labels
+    idx_train, idx_val, idx_test = data.idx_train, data.idx_val, data.idx_test
+    idx_unlabeled = np.union1d(idx_val, idx_test)
+    ```
+
+2. Set up surrogate model
+    ```python
+    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+    surrogate = GCN(nfeat=features.shape[1], nclass=labels.max().item()+1, nhid=16,
+                    with_relu=False, device=device)
+    surrogate = surrogate.to(device)
+    surrogate.fit(features, adj, labels, idx_train)
+    ```
+
+
+3. Set up attack model and generate perturbations
+    ```python
+    model = Metattack(model=surrogate, nnodes=adj.shape[0], feature_shape=features.shape, device=device)
+    model = model.to(device)
+    perturbations = int(0.05 * (adj.sum() // 2))
+    model.attack(features, adj, labels, idx_train, idx_unlabeled, perturbations, ll_constraint=False)
+    modified_adj = model.modified_adj
+    ```
+    
+For more details please refer to [mettack.py](https://github.com/I-am-Bot/DeepRobust/blob/master/examples/graph/test_mettack.py) or run 
+    ```
+    python examples/graph/test_mettack.py --dataset cora --ptb_rate 0.05
+    ```
+
+### Defending Against Graph Attacks
+
+1. Load dataset
+    ```python
+    import torch
+    from deeprobust.graph.data import Dataset, PtbDataset
+    from deeprobust.graph.defense import GCN, GCNJaccard
+    import numpy as np
+    np.random.seed(15)
+
+    # load clean graph
+    data = Dataset(root='/tmp/', name='cora', setting='nettack')
+    adj, features, labels = data.adj, data.features, data.labels
+    idx_train, idx_val, idx_test = data.idx_train, data.idx_val, data.idx_test
+
+    # load pre-attacked graph by mettack
+    perturbed_data = PtbDataset(root='/tmp/', name='cora')
+    perturbed_adj = perturbed_data.adj
+    ```
+2. Test 
+    ```python
+    # Set up defense model and test performance
+    device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+    model = GCNJaccard(nfeat=features.shape[1], nclass=labels.max()+1, nhid=16, device=device)
+    model = model.to(device)
+    model.fit(features, perturbed_adj, labels, idx_train)
+    model.eval()
+    output = model.test(idx_test)
+
+    # Test on GCN
+    model = GCN(nfeat=features.shape[1], nclass=labels.max()+1, nhid=16, device=device)
+    model = model.to(device)
+    model.fit(features, perturbed_adj, labels, idx_train)
+    model.eval()
+    output = model.test(idx_test)
+    ```
+    
+For more details please refer to [test_gcn_jaccard.py](https://github.com/I-am-Bot/DeepRobust/blob/master/examples/graph/test_gcn_jaccard.py) or run
+    ```
+    python examples/graph/test_gcn_jaccard.py --dataset cora
+    ```
+
+## Sample Results
+adversary examples generated by fgsm:
+<div align="center">
+<img height=140 src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/mnist_advexample_fgsm_ori.png"/><img height=140 src="https://github.com/DSE-MSU/DeepRobust/blob/master/adversary_examples/mnist_advexample_fgsm_adv.png"/>
+</div>
+Left:original, classified as 6; Right:adversary, classified as 4.
+
+Serveral trained models can be found here: https://drive.google.com/open?id=1uGLiuCyd8zCAQ8tPz9DDUQH6zm-C4tEL
+
+## Acknowledgement
+Some of the algorithms are referred to paper authors' implementations. References can be found at the top of each file. 
+
+Implementation of network structure are referred to weiaicunzai's github. Original code can be found here:
+[pytorch-cifar100](https://github.com/weiaicunzai/pytorch-cifar100)
+
+Thanks to their outstanding works!
+
+
+<!----
+We would be glad if you find our work useful and cite the paper.
+
+'''
+@misc{jin2020adversarial,
+    title={Adversarial Attacks and Defenses on Graphs: A Review and Empirical Study},
+    author={Wei Jin and Yaxin Li and Han Xu and Yiqi Wang and Jiliang Tang},
+    year={2020},
+    eprint={2003.00653},
+    archivePrefix={arXiv},
+    primaryClass={cs.LG}
+}
+'''
+```
+@article{xu2019adversarial,
+  title={Adversarial attacks and defenses in images, graphs and text: A review},
+  author={Xu, Han and Ma, Yao and Liu, Haochen and Deb, Debayan and Liu, Hui and Tang, Jiliang and Jain, Anil},
+  journal={arXiv preprint arXiv:1909.08072},
+  year={2019}
+}
+```
+---->
+
+
```

#### html2text {}

```diff
@@ -1,13 +1,21 @@
-Metadata-Version: 2.1 Name: deeprobust Version: 0.2.8 Summary: A PyTorch
+Metadata-Version: 2.1 Name: deeprobust Version: 0.2.9 Summary: A PyTorch
 library for adversarial robustness learning for image and graph data. Home-
 page: https://github.com/DSE-MSU/DeepRobust Author: MSU-DSE Maintainer: MSU-DSE
-License: MIT Description: [contributing-image]: https://img.shields.io/badge/
-contributions-welcome-brightgreen.svg?style=flat [contributing-url]: https://
-github.com/rusty1s/pytorch_geometric/blob/master/CONTRIBUTING.md
+License: MIT Platform: UNKNOWN Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education Classifier: Intended Audience ::
+Science/Research Classifier: Programming Language :: Python :: 3.5 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Topic :: Scientific/Engineering :: Mathematics Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Software
+Development :: Libraries Description-Content-Type: text/markdown License-File:
+LICENSE [contributing-image]: https://img.shields.io/badge/contributions-
+welcome-brightgreen.svg?style=flat [contributing-url]: https://github.com/
+rusty1s/pytorch_geometric/blob/master/CONTRIBUTING.md
                                     [logo]
 --------------------- [GitHub last commit]_[_G_i_t_H_u_b_ _i_s_s_u_e_s_][GitHub][!
 [Contributing][contributing-image]][contributing-url] [![Tweet](https://
 img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://
 twitter.com/intent/
 tweet?text=Build%20your%20robust%20machine%20learning%20models%20with%20DeepRobust%20in%2060%20seconds&url=https:
 //github.com/DSE-MSU/
@@ -34,27 +42,33 @@
 Defenses on Graphs: A Review, A Tool and Empirical Studies](https://arxiv.org/
 abs/2003.00653) * [Adversarial Attacks and Defenses in Images, Graphs and Text:
 A Review](https://arxiv.org/pdf/1909.08072.pdf) If our work could help your
 research, please cite: [DeepRobust: A PyTorch Library for Adversarial Attacks
 and Defenses](https://arxiv.org/abs/2005.06149) ``` @article{li2020deeprobust,
 title={Deeprobust: A pytorch library for adversarial attacks and defenses},
 author={Li, Yaxin and Jin, Wei and Xu, Han and Tang, Jiliang}, journal={arXiv
-preprint arXiv:2005.06149}, year={2020} } ``` # Changelog * [02/2023]
-DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We have
-added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/2110.14038)
-to graph package. We can now use PRBCD to attack large-scale graphs such as
-ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/
+preprint arXiv:2005.06149}, year={2020} } ``` # Changelog * [11/2023]
+DeepRobust 0.2.9 Released. Please try `pip install deeprobust==0.2.9`. We have
+fixed the OOM issue of metattack on new pytorch versions. * [06/2023] We have
+added a backdoor attack [UGBA, WWW'23](https://arxiv.org/abs/2303.01263) to
+graph package. We can now use UGBA to conduct unnoticeable backdoor attack on
+large-scale graphs such as ogb-arxiv (see example in [test_ugba.py](https://
+github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_ugba.py))! * [02/
+2023] DeepRobust 0.2.8 Released. Please try `pip install deeprobust==0.2.8`! We
+have added a scalable attack [PRBCD, NeurIPS'21](https://arxiv.org/abs/
+2110.14038) to graph package. We can now use PRBCD to attack large-scale graphs
+such as ogb-arxiv (see example in [test_prbcd.py](https://github.com/DSE-MSU/
 DeepRobust/blob/master/examples/graph/test_prbcd.py))! * [02/2023] Add a robust
 model [AirGNN, NeurIPS'21](https://proceedings.neurips.cc/paper/2021/file/
 50abc3e730e36b387ca8e02c26dc0a22-Paper.pdf) to graph package. Try `python
 examples/graph/test_airgnn.py`! See details in [test_airgnn.py](https://
 github.com/DSE-MSU/DeepRobust/blob/master/examples/graph/test_airgnn.py) * [11/
 2022] DeepRobust 0.2.6 Released. Please try `pip install deeprobust==0.2.6`! We
 have more updates coming. Please stay tuned! * [11/2021] A subpackage that
-includes popular black box attacks in image domain is relased. Find it here.
+includes popular black box attacks in image domain is released. Find it here.
 [Link](https://github.com/I-am-Bot/Black-Box-Attacks) * [11/2021] DeepRobust
 0.2.4 Released. Please try `pip install deeprobust==0.2.4`! * [10/2021] add
 scalable attack and MedianGCN. Thank [Jintang](https://github.com/EdisonLeeeee)
 for his contribution! * [06/2021] [Image Package] Add preprocessing method:
 APE-GAN. * [05/2021] DeepRobust is published at AAAI 2021. Check [here](https:/
 /ojs.aaai.org/index.php/AAAI/article/view/18017)! * [05/2021] DeepRobust 0.2.2
 Released. Please try `pip install deeprobust==0.2.2`! * [04/2021] [Image
@@ -163,15 +177,8 @@
 Left:original, classified as 6; Right:adversary, classified as 4. Serveral
 trained models can be found here: https://drive.google.com/
 open?id=1uGLiuCyd8zCAQ8tPz9DDUQH6zm-C4tEL ## Acknowledgement Some of the
 algorithms are referred to paper authors' implementations. References can be
 found at the top of each file. Implementation of network structure are referred
 to weiaicunzai's github. Original code can be found here: [pytorch-cifar100]
 (https://github.com/weiaicunzai/pytorch-cifar100) Thanks to their outstanding
-works! Platform: UNKNOWN Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education Classifier: Intended Audience ::
-Science/Research Classifier: Programming Language :: Python :: 3.5 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Topic :: Scientific/Engineering :: Mathematics Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Software
-Development :: Libraries Description-Content-Type: text/markdown
+works!
```

### Comparing `deeprobust-0.2.8/deeprobust.egg-info/SOURCES.txt` & `deeprobust-0.2.9/deeprobust.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 setup.py
-setup_empty.py
 deeprobust/__init__.py
 deeprobust.egg-info/PKG-INFO
 deeprobust.egg-info/SOURCES.txt
 deeprobust.egg-info/dependency_links.txt
 deeprobust.egg-info/requires.txt
 deeprobust.egg-info/top_level.txt
 deeprobust/graph/__init__.py
@@ -62,14 +61,15 @@
 deeprobust/graph/targeted_attack/base_attack.py
 deeprobust/graph/targeted_attack/fga.py
 deeprobust/graph/targeted_attack/ig_attack.py
 deeprobust/graph/targeted_attack/nettack.py
 deeprobust/graph/targeted_attack/rl_s2v.py
 deeprobust/graph/targeted_attack/rnd.py
 deeprobust/graph/targeted_attack/sga.py
+deeprobust/graph/targeted_attack/ugba.py
 deeprobust/image/__init__.py
 deeprobust/image/config.py
 deeprobust/image/evaluation_attack.py
 deeprobust/image/optimizer.py
 deeprobust/image/utils.py
 deeprobust/image/attack/BPDA.py
 deeprobust/image/attack/Nattack.py
```

### Comparing `deeprobust-0.2.8/setup.py` & `deeprobust-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 
 with open("README.md", 'r') as fh:
     long_description = fh.read()
 
 setup(name = "deeprobust",
-      version = "0.2.8",
+      version = "0.2.9",
       author='MSU-DSE',
       maintainer='MSU-DSE',
       description = "A PyTorch library for adversarial robustness learning for image and graph data.",
       long_description=long_description,
       long_description_content_type = "text/markdown",
       packages = find_packages(),
       url='https://github.com/DSE-MSU/DeepRobust',
```

