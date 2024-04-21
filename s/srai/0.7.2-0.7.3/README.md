# Comparing `tmp/srai-0.7.2.tar.gz` & `tmp/srai-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-0.7.2.tar", last modified: Sat Apr 20 14:01:27 2024, max compression
+gzip compressed data, was "srai-0.7.3.tar", last modified: Sun Apr 21 17:32:43 2024, max compression
```

## Comparing `srai-0.7.2.tar` & `srai-0.7.3.tar`

### file list

```diff
@@ -1,168 +1,168 @@
--rw-r--r--   0        0        0    10760 2024-04-20 14:01:08.055309 srai-0.7.2/LICENSE.md
--rw-r--r--   0        0        0    18089 2024-04-20 14:01:08.055309 srai-0.7.2/README.md
--rw-r--r--   0        0        0     5261 2024-04-20 14:01:27.459538 srai-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      428 2024-04-20 14:01:08.067309 srai-0.7.2/srai/__init__.py
--rw-r--r--   0        0        0     2904 2024-04-20 14:01:08.067309 srai-0.7.2/srai/_optional.py
--rw-r--r--   0        0        0      717 2024-04-20 14:01:08.067309 srai-0.7.2/srai/_typing.py
--rw-r--r--   0        0        0      155 2024-04-20 14:01:08.067309 srai-0.7.2/srai/constants.py
--rw-r--r--   0        0        0      854 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/__init__.py
--rw-r--r--   0        0        0     4846 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/_base.py
--rw-r--r--   0        0        0      482 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/_pytorch_stubs.py
--rw-r--r--   0        0        0     9181 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/contextual_count_embedder.py
--rw-r--r--   0        0        0     8180 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/count_embedder.py
--rw-r--r--   0        0        0      186 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/geovex/__init__.py
--rw-r--r--   0        0        0     6882 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/geovex/dataset.py
--rw-r--r--   0        0        0     9809 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/geovex/embedder.py
--rw-r--r--   0        0        0    18081 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/geovex/model.py
--rw-r--r--   0        0        0      136 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/gtfs2vec/__init__.py
--rw-r--r--   0        0        0    11336 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/gtfs2vec/embedder.py
--rw-r--r--   0        0        0     2278 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/gtfs2vec/model.py
--rw-r--r--   0        0        0      247 2024-04-20 14:01:08.067309 srai-0.7.2/srai/embedders/hex2vec/__init__.py
--rw-r--r--   0        0        0    10941 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/hex2vec/embedder.py
--rw-r--r--   0        0        0     6804 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/hex2vec/model.py
--rw-r--r--   0        0        0     6301 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/hex2vec/neighbour_dataset.py
--rw-r--r--   0        0        0      153 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/highway2vec/__init__.py
--rw-r--r--   0        0        0     7919 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/highway2vec/embedder.py
--rw-r--r--   0        0        0     2855 2024-04-20 14:01:08.071309 srai-0.7.2/srai/embedders/highway2vec/model.py
--rw-r--r--   0        0        0      580 2024-04-20 14:01:08.071309 srai-0.7.2/srai/exceptions.py
--rw-r--r--   0        0        0     4247 2024-04-20 14:01:08.071309 srai-0.7.2/srai/geometry.py
--rw-r--r--   0        0        0     9060 2024-04-20 14:01:08.071309 srai-0.7.2/srai/h3.py
--rw-r--r--   0        0        0      531 2024-04-20 14:01:08.071309 srai-0.7.2/srai/joiners/__init__.py
--rw-r--r--   0        0        0      731 2024-04-20 14:01:08.071309 srai-0.7.2/srai/joiners/_base.py
--rw-r--r--   0        0        0     3836 2024-04-20 14:01:08.071309 srai-0.7.2/srai/joiners/intersection_joiner.py
--rw-r--r--   0        0        0      820 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/__init__.py
--rw-r--r--   0        0        0      591 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/_base.py
--rw-r--r--   0        0        0     1343 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/download.py
--rw-r--r--   0        0        0     2189 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/geoparquet_loader.py
--rw-r--r--   0        0        0     5391 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/gtfs_loader.py
--rw-r--r--   0        0        0      257 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/__init__.py
--rw-r--r--   0        0        0     7765 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/_base.py
--rw-r--r--   0        0        0      472 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/__init__.py
--rw-r--r--   0        0        0     4402 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/_typing.py
--rw-r--r--   0        0        0     5315 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/base_osm_groups.py
--rw-r--r--   0        0        0    10696 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/geofabrik.py
--rw-r--r--   0        0        0    15751 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/hex2vec.py
--rw-r--r--   0        0        0     2447 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/filters/popular.py
--rw-r--r--   0        0        0     5996 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/osm_online_loader.py
--rw-r--r--   0        0        0     9280 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/osm_pbf_loader.py
--rw-r--r--   0        0        0     2778 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/osm_tile_data_collector.py
--rw-r--r--   0        0        0     5033 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_loaders/osm_tile_loader.py
--rw-r--r--   0        0        0      124 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_way_loader/__init__.py
--rw-r--r--   0        0        0     7556 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_way_loader/constants.py
--rw-r--r--   0        0        0    14142 2024-04-20 14:01:08.071309 srai-0.7.2/srai/loaders/osm_way_loader/osm_way_loader.py
--rw-r--r--   0        0        0      468 2024-04-20 14:01:08.071309 srai-0.7.2/srai/neighbourhoods/__init__.py
--rw-r--r--   0        0        0     6176 2024-04-20 14:01:08.071309 srai-0.7.2/srai/neighbourhoods/_base.py
--rw-r--r--   0        0        0     3609 2024-04-20 14:01:08.071309 srai-0.7.2/srai/neighbourhoods/adjacency_neighbourhood.py
--rw-r--r--   0        0        0     4632 2024-04-20 14:01:08.071309 srai-0.7.2/srai/neighbourhoods/h3_neighbourhood.py
--rw-r--r--   0        0        0      497 2024-04-20 14:01:08.071309 srai-0.7.2/srai/plotting/__init__.py
--rw-r--r--   0        0        0    11418 2024-04-20 14:01:08.071309 srai-0.7.2/srai/plotting/folium_wrapper.py
--rw-r--r--   0        0        0    14129 2024-04-20 14:01:08.071309 srai-0.7.2/srai/plotting/plotly_wrapper.py
--rw-r--r--   0        0        0       55 2024-04-20 14:01:08.071309 srai-0.7.2/srai/py.typed
--rw-r--r--   0        0        0     1006 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/__init__.py
--rw-r--r--   0        0        0      957 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/_base.py
--rw-r--r--   0        0        0    27555 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/_spherical_voronoi.py
--rw-r--r--   0        0        0    15629 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2477 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/geocode.py
--rw-r--r--   0        0        0     2610 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/h3_regionalizer.py
--rw-r--r--   0        0        0     3136 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/s2_regionalizer.py
--rw-r--r--   0        0        0     4184 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/slippy_map_regionalizer.py
--rw-r--r--   0        0        0     6001 2024-04-20 14:01:08.071309 srai-0.7.2/srai/regionalizers/voronoi_regionalizer.py
--rw-r--r--   0        0        0       29 2024-04-20 14:01:08.071309 srai-0.7.2/tests/__init__.py
--rw-r--r--   0        0        0     7806 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/conftest.py
--rw-r--r--   0        0        0     1015 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/geovex/constants.py
--rw-r--r--   0        0        0     6245 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/geovex/generation.py
--rw-r--r--   0        0        0     4211 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/geovex/test_dataset.py
--rw-r--r--   0        0        0     4049 2024-04-20 14:01:08.071309 srai-0.7.2/tests/embedders/geovex/test_embedder.py
--rw-r--r--   0        0        0   484605 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_0.pt
--rw-r--r--   0        0        0   484605 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_1.pt
--rw-r--r--   0        0        0   484605 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_2.pt
--rw-r--r--   0        0        0   339453 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_3.pt
--rw-r--r--   0        0        0     2139 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt
--rw-r--r--   0        0        0     2139 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt
--rw-r--r--   0        0        0     2139 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt
--rw-r--r--   0        0        0     1755 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt
--rw-r--r--   0        0        0    75958 2024-04-20 14:01:08.075309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_features.parquet
--rw-r--r--   0        0        0   968711 2024-04-20 14:01:08.079309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_0.pt
--rw-r--r--   0        0        0   968711 2024-04-20 14:01:08.079309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_1.pt
--rw-r--r--   0        0        0   968711 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_2.pt
--rw-r--r--   0        0        0   678407 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_3.pt
--rw-r--r--   0        0        0     7011 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_joint.parquet
--rw-r--r--   0        0        0      762 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_0.pt
--rw-r--r--   0        0        0      762 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_1.pt
--rw-r--r--   0        0        0      762 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_2.pt
--rw-r--r--   0        0        0      762 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_3.pt
--rw-r--r--   0        0        0    13915 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_regions.parquet
--rw-r--r--   0        0        0    24970 2024-04-20 14:01:08.083309 srai-0.7.2/tests/embedders/geovex/test_files/AL_10_result.parquet
--rw-r--r--   0        0        0   272893 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_batch_0.pt
--rw-r--r--   0        0        0   245693 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_batch_1.pt
--rw-r--r--   0        0        0     2139 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt
--rw-r--r--   0        0        0     2011 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt
--rw-r--r--   0        0        0   803774 2024-04-20 14:01:08.087309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0   545287 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_forward_0.pt
--rw-r--r--   0        0        0   490887 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_forward_1.pt
--rw-r--r--   0        0        0    76452 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0      762 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_loss_0.pt
--rw-r--r--   0        0        0      762 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_loss_1.pt
--rw-r--r--   0        0        0    10162 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    21999 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     4538 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/geovex/test_model.py
--rw-r--r--   0        0        0      579 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/constants.py
--rw-r--r--   0        0        0     2782 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/generation.py
--rw-r--r--   0        0        0     3013 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/test_embedder.py
--rw-r--r--   0        0        0    97383 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_features.parquet
--rw-r--r--   0        0        0   111218 2024-04-20 14:01:08.091309 srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
--rw-r--r--   0        0        0    14226 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
--rw-r--r--   0        0        0    14498 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_result.parquet
--rw-r--r--   0        0        0    89227 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_features.parquet
--rw-r--r--   0        0        0    86944 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
--rw-r--r--   0        0        0    16794 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
--rw-r--r--   0        0        0    15781 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_result.parquet
--rw-r--r--   0        0        0     1056 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_model.py
--rw-r--r--   0        0        0     3058 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/hex2vec/test_neighbour_dataset.py
--rw-r--r--   0        0        0    27244 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/test_contextual_count_embedder.py
--rw-r--r--   0        0        0    12298 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/test_count_embedder.py
--rw-r--r--   0        0        0     7091 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/test_gtfs2vec_embedder.py
--rw-r--r--   0        0        0     3631 2024-04-20 14:01:08.095309 srai-0.7.2/tests/embedders/test_highway2vec_embedder.py
--rw-r--r--   0        0        0     2838 2024-04-20 14:01:08.095309 srai-0.7.2/tests/h3/conftest.py
--rw-r--r--   0        0        0     3035 2024-04-20 14:01:08.095309 srai-0.7.2/tests/h3/test_ij_coordinates.py
--rw-r--r--   0        0        0     3083 2024-04-20 14:01:08.095309 srai-0.7.2/tests/h3/test_shapely_conversion.py
--rw-r--r--   0        0        0     1765 2024-04-20 14:01:08.095309 srai-0.7.2/tests/joiners/conftest.py
--rw-r--r--   0        0        0     2530 2024-04-20 14:01:08.095309 srai-0.7.2/tests/joiners/test_intersection_joiner.py
--rw-r--r--   0        0        0     3001 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/conftest.py
--rw-r--r--   0        0        0     4285 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/conftest.py
--rw-r--r--   0        0        0     4824 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/filters/popular_filter_example.json
--rw-r--r--   0        0        0     4094 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
--rw-r--r--   0        0        0     3283 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
--rw-r--r--   0        0        0      342 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-04-20 14:01:08.095309 srai-0.7.2/tests/loaders/osm_loaders/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0   111539 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_files/poland.geojson
--rw-r--r--   0        0        0   252620 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
--rw-r--r--   0        0        0     3026 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_osm_online_loader.py
--rw-r--r--   0        0        0     4921 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_osm_pbf_loader.py
--rw-r--r--   0        0        0     3159 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
--rw-r--r--   0        0        0     3142 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_loaders/test_osm_tile_loader.py
--rw-r--r--   0        0        0     3803 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_1.pkl
--rw-r--r--   0        0        0     3334 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_2.pkl
--rw-r--r--   0        0        0     5099 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_3.pkl
--rw-r--r--   0        0        0     3803 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_4.pkl
--rw-r--r--   0        0        0    11234 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/osm_way_loader/test_osm_way_loader.py
--rw-r--r--   0        0        0    27801 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/test_files/example.parquet
--rw-r--r--   0        0        0     2182 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/test_geoparquet_loader.py
--rw-r--r--   0        0        0     3177 2024-04-20 14:01:08.099310 srai-0.7.2/tests/loaders/test_gtfs_loader.py
--rw-r--r--   0        0        0     4878 2024-04-20 14:01:08.099310 srai-0.7.2/tests/miscellaneous/test_optional_dependencies.py
--rw-r--r--   0        0        0     8340 2024-04-20 14:01:08.099310 srai-0.7.2/tests/neighbourhoods/h3/test_no_regions.py
--rw-r--r--   0        0        0     9166 2024-04-20 14:01:08.099310 srai-0.7.2/tests/neighbourhoods/h3/test_with_regions.py
--rw-r--r--   0        0        0    11395 2024-04-20 14:01:08.099310 srai-0.7.2/tests/neighbourhoods/test_adjacency_neighbourhood.py
--rw-r--r--   0        0        0    11019 2024-04-20 14:01:08.099310 srai-0.7.2/tests/neighbourhoods/test_neighbourhood.py
--rw-r--r--   0        0        0      765 2024-04-20 14:01:08.099310 srai-0.7.2/tests/plotting/test_folium_wrapper.py
--rw-r--r--   0        0        0     3729 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/conftest.py
--rw-r--r--   0        0        0     6509 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_administrative_boundary_regionalizer.py
--rw-r--r--   0        0        0     2616 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_h3_regionalizer.py
--rw-r--r--   0        0        0     1856 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_s2_regionalizer.py
--rw-r--r--   0        0        0     2690 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_slippy_map_regionalizer.py
--rw-r--r--   0        0        0     9215 2024-04-20 14:01:08.099310 srai-0.7.2/tests/regionalizers/test_voronoi_regionalizer.py
--rw-r--r--   0        0        0    20378 1970-01-01 00:00:00.000000 srai-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    10760 2024-04-21 17:32:24.518289 srai-0.7.3/LICENSE.md
+-rw-r--r--   0        0        0    18091 2024-04-21 17:32:24.518289 srai-0.7.3/README.md
+-rw-r--r--   0        0        0     5261 2024-04-21 17:32:43.102470 srai-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      428 2024-04-21 17:32:24.530290 srai-0.7.3/srai/__init__.py
+-rw-r--r--   0        0        0     2904 2024-04-21 17:32:24.530290 srai-0.7.3/srai/_optional.py
+-rw-r--r--   0        0        0      717 2024-04-21 17:32:24.530290 srai-0.7.3/srai/_typing.py
+-rw-r--r--   0        0        0      155 2024-04-21 17:32:24.530290 srai-0.7.3/srai/constants.py
+-rw-r--r--   0        0        0      854 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/__init__.py
+-rw-r--r--   0        0        0     4846 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/_base.py
+-rw-r--r--   0        0        0      482 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/_pytorch_stubs.py
+-rw-r--r--   0        0        0     9181 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/contextual_count_embedder.py
+-rw-r--r--   0        0        0     8180 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/count_embedder.py
+-rw-r--r--   0        0        0      186 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/geovex/__init__.py
+-rw-r--r--   0        0        0     6882 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/geovex/dataset.py
+-rw-r--r--   0        0        0     9809 2024-04-21 17:32:24.530290 srai-0.7.3/srai/embedders/geovex/embedder.py
+-rw-r--r--   0        0        0    18081 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/geovex/model.py
+-rw-r--r--   0        0        0      136 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/gtfs2vec/__init__.py
+-rw-r--r--   0        0        0    11336 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/gtfs2vec/embedder.py
+-rw-r--r--   0        0        0     2278 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/gtfs2vec/model.py
+-rw-r--r--   0        0        0      247 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/hex2vec/__init__.py
+-rw-r--r--   0        0        0    10941 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/hex2vec/embedder.py
+-rw-r--r--   0        0        0     6804 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/hex2vec/model.py
+-rw-r--r--   0        0        0     6301 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/hex2vec/neighbour_dataset.py
+-rw-r--r--   0        0        0      153 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/highway2vec/__init__.py
+-rw-r--r--   0        0        0     7919 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/highway2vec/embedder.py
+-rw-r--r--   0        0        0     2855 2024-04-21 17:32:24.534290 srai-0.7.3/srai/embedders/highway2vec/model.py
+-rw-r--r--   0        0        0      580 2024-04-21 17:32:24.534290 srai-0.7.3/srai/exceptions.py
+-rw-r--r--   0        0        0     4247 2024-04-21 17:32:24.534290 srai-0.7.3/srai/geometry.py
+-rw-r--r--   0        0        0     9060 2024-04-21 17:32:24.534290 srai-0.7.3/srai/h3.py
+-rw-r--r--   0        0        0      531 2024-04-21 17:32:24.534290 srai-0.7.3/srai/joiners/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-21 17:32:24.534290 srai-0.7.3/srai/joiners/_base.py
+-rw-r--r--   0        0        0     3836 2024-04-21 17:32:24.534290 srai-0.7.3/srai/joiners/intersection_joiner.py
+-rw-r--r--   0        0        0      820 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/__init__.py
+-rw-r--r--   0        0        0      591 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/_base.py
+-rw-r--r--   0        0        0     1343 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/download.py
+-rw-r--r--   0        0        0     2189 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/geoparquet_loader.py
+-rw-r--r--   0        0        0     5391 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/gtfs_loader.py
+-rw-r--r--   0        0        0      257 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/__init__.py
+-rw-r--r--   0        0        0     7765 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/_base.py
+-rw-r--r--   0        0        0      472 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/__init__.py
+-rw-r--r--   0        0        0     4402 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/_typing.py
+-rw-r--r--   0        0        0     5315 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/base_osm_groups.py
+-rw-r--r--   0        0        0    10696 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/geofabrik.py
+-rw-r--r--   0        0        0    15751 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/hex2vec.py
+-rw-r--r--   0        0        0     2447 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/filters/popular.py
+-rw-r--r--   0        0        0     5996 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/osm_online_loader.py
+-rw-r--r--   0        0        0     9286 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/osm_pbf_loader.py
+-rw-r--r--   0        0        0     2778 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/osm_tile_data_collector.py
+-rw-r--r--   0        0        0     5033 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_loaders/osm_tile_loader.py
+-rw-r--r--   0        0        0      124 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_way_loader/__init__.py
+-rw-r--r--   0        0        0     7556 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_way_loader/constants.py
+-rw-r--r--   0        0        0    14142 2024-04-21 17:32:24.534290 srai-0.7.3/srai/loaders/osm_way_loader/osm_way_loader.py
+-rw-r--r--   0        0        0      468 2024-04-21 17:32:24.534290 srai-0.7.3/srai/neighbourhoods/__init__.py
+-rw-r--r--   0        0        0     6176 2024-04-21 17:32:24.534290 srai-0.7.3/srai/neighbourhoods/_base.py
+-rw-r--r--   0        0        0     3609 2024-04-21 17:32:24.534290 srai-0.7.3/srai/neighbourhoods/adjacency_neighbourhood.py
+-rw-r--r--   0        0        0     4632 2024-04-21 17:32:24.534290 srai-0.7.3/srai/neighbourhoods/h3_neighbourhood.py
+-rw-r--r--   0        0        0      497 2024-04-21 17:32:24.534290 srai-0.7.3/srai/plotting/__init__.py
+-rw-r--r--   0        0        0    11418 2024-04-21 17:32:24.534290 srai-0.7.3/srai/plotting/folium_wrapper.py
+-rw-r--r--   0        0        0    14129 2024-04-21 17:32:24.534290 srai-0.7.3/srai/plotting/plotly_wrapper.py
+-rw-r--r--   0        0        0       55 2024-04-21 17:32:24.534290 srai-0.7.3/srai/py.typed
+-rw-r--r--   0        0        0     1006 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/__init__.py
+-rw-r--r--   0        0        0      957 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/_base.py
+-rw-r--r--   0        0        0    27555 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/_spherical_voronoi.py
+-rw-r--r--   0        0        0    15629 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2477 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/geocode.py
+-rw-r--r--   0        0        0     2610 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/h3_regionalizer.py
+-rw-r--r--   0        0        0     3136 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/s2_regionalizer.py
+-rw-r--r--   0        0        0     4184 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     6001 2024-04-21 17:32:24.534290 srai-0.7.3/srai/regionalizers/voronoi_regionalizer.py
+-rw-r--r--   0        0        0       29 2024-04-21 17:32:24.534290 srai-0.7.3/tests/__init__.py
+-rw-r--r--   0        0        0     7806 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/conftest.py
+-rw-r--r--   0        0        0     1015 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/geovex/constants.py
+-rw-r--r--   0        0        0     6245 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/geovex/generation.py
+-rw-r--r--   0        0        0     4211 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/geovex/test_dataset.py
+-rw-r--r--   0        0        0     4049 2024-04-21 17:32:24.534290 srai-0.7.3/tests/embedders/geovex/test_embedder.py
+-rw-r--r--   0        0        0   484605 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_0.pt
+-rw-r--r--   0        0        0   484605 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_1.pt
+-rw-r--r--   0        0        0   484605 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_2.pt
+-rw-r--r--   0        0        0   339453 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_3.pt
+-rw-r--r--   0        0        0     2139 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt
+-rw-r--r--   0        0        0     2139 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt
+-rw-r--r--   0        0        0     2139 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt
+-rw-r--r--   0        0        0     1755 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt
+-rw-r--r--   0        0        0    75958 2024-04-21 17:32:24.538290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_features.parquet
+-rw-r--r--   0        0        0   968711 2024-04-21 17:32:24.542290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_0.pt
+-rw-r--r--   0        0        0   968711 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_1.pt
+-rw-r--r--   0        0        0   968711 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_2.pt
+-rw-r--r--   0        0        0   678407 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_3.pt
+-rw-r--r--   0        0        0     7011 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_joint.parquet
+-rw-r--r--   0        0        0      762 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_0.pt
+-rw-r--r--   0        0        0      762 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_1.pt
+-rw-r--r--   0        0        0      762 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_2.pt
+-rw-r--r--   0        0        0      762 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_3.pt
+-rw-r--r--   0        0        0    13915 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_regions.parquet
+-rw-r--r--   0        0        0    24970 2024-04-21 17:32:24.546290 srai-0.7.3/tests/embedders/geovex/test_files/AL_10_result.parquet
+-rw-r--r--   0        0        0   272893 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_batch_0.pt
+-rw-r--r--   0        0        0   245693 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_batch_1.pt
+-rw-r--r--   0        0        0     2139 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt
+-rw-r--r--   0        0        0     2011 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt
+-rw-r--r--   0        0        0   803774 2024-04-21 17:32:24.550290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0   545287 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_forward_0.pt
+-rw-r--r--   0        0        0   490887 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_forward_1.pt
+-rw-r--r--   0        0        0    76452 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0      762 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_loss_0.pt
+-rw-r--r--   0        0        0      762 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_loss_1.pt
+-rw-r--r--   0        0        0    10162 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    21999 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     4538 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/geovex/test_model.py
+-rw-r--r--   0        0        0      579 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/hex2vec/constants.py
+-rw-r--r--   0        0        0     2782 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/hex2vec/generation.py
+-rw-r--r--   0        0        0     3013 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/hex2vec/test_embedder.py
+-rw-r--r--   0        0        0    97383 2024-04-21 17:32:24.554290 srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_features.parquet
+-rw-r--r--   0        0        0   111218 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_joint.parquet
+-rw-r--r--   0        0        0    14226 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_regions.parquet
+-rw-r--r--   0        0        0    14498 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_result.parquet
+-rw-r--r--   0        0        0    89227 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_features.parquet
+-rw-r--r--   0        0        0    86944 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_joint.parquet
+-rw-r--r--   0        0        0    16794 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_regions.parquet
+-rw-r--r--   0        0        0    15781 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_result.parquet
+-rw-r--r--   0        0        0     1056 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_model.py
+-rw-r--r--   0        0        0     3058 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/hex2vec/test_neighbour_dataset.py
+-rw-r--r--   0        0        0    27244 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/test_contextual_count_embedder.py
+-rw-r--r--   0        0        0    12298 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/test_count_embedder.py
+-rw-r--r--   0        0        0     7091 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/test_gtfs2vec_embedder.py
+-rw-r--r--   0        0        0     3631 2024-04-21 17:32:24.558290 srai-0.7.3/tests/embedders/test_highway2vec_embedder.py
+-rw-r--r--   0        0        0     2838 2024-04-21 17:32:24.558290 srai-0.7.3/tests/h3/conftest.py
+-rw-r--r--   0        0        0     3035 2024-04-21 17:32:24.558290 srai-0.7.3/tests/h3/test_ij_coordinates.py
+-rw-r--r--   0        0        0     3083 2024-04-21 17:32:24.558290 srai-0.7.3/tests/h3/test_shapely_conversion.py
+-rw-r--r--   0        0        0     1765 2024-04-21 17:32:24.558290 srai-0.7.3/tests/joiners/conftest.py
+-rw-r--r--   0        0        0     2530 2024-04-21 17:32:24.558290 srai-0.7.3/tests/joiners/test_intersection_joiner.py
+-rw-r--r--   0        0        0     3001 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/conftest.py
+-rw-r--r--   0        0        0     4285 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/conftest.py
+-rw-r--r--   0        0        0     4824 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/filters/popular_filter_example.json
+-rw-r--r--   0        0        0     4094 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/filters/test_merge_filter_types.py
+-rw-r--r--   0        0        0     3283 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py
+-rw-r--r--   0        0        0      342 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-04-21 17:32:24.558290 srai-0.7.3/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0   111539 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_files/poland.geojson
+-rw-r--r--   0        0        0   252620 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson
+-rw-r--r--   0        0        0     3026 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_osm_online_loader.py
+-rw-r--r--   0        0        0     4921 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_osm_pbf_loader.py
+-rw-r--r--   0        0        0     3159 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_osm_tile_data_collector.py
+-rw-r--r--   0        0        0     3142 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_loaders/test_osm_tile_loader.py
+-rw-r--r--   0        0        0     3803 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_1.pkl
+-rw-r--r--   0        0        0     3334 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_2.pkl
+-rw-r--r--   0        0        0     5099 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_3.pkl
+-rw-r--r--   0        0        0     3803 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_4.pkl
+-rw-r--r--   0        0        0    11234 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/osm_way_loader/test_osm_way_loader.py
+-rw-r--r--   0        0        0    27801 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/test_files/example.parquet
+-rw-r--r--   0        0        0     2182 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/test_geoparquet_loader.py
+-rw-r--r--   0        0        0     3177 2024-04-21 17:32:24.562290 srai-0.7.3/tests/loaders/test_gtfs_loader.py
+-rw-r--r--   0        0        0     4878 2024-04-21 17:32:24.562290 srai-0.7.3/tests/miscellaneous/test_optional_dependencies.py
+-rw-r--r--   0        0        0     8340 2024-04-21 17:32:24.562290 srai-0.7.3/tests/neighbourhoods/h3/test_no_regions.py
+-rw-r--r--   0        0        0     9166 2024-04-21 17:32:24.562290 srai-0.7.3/tests/neighbourhoods/h3/test_with_regions.py
+-rw-r--r--   0        0        0    11395 2024-04-21 17:32:24.562290 srai-0.7.3/tests/neighbourhoods/test_adjacency_neighbourhood.py
+-rw-r--r--   0        0        0    11019 2024-04-21 17:32:24.562290 srai-0.7.3/tests/neighbourhoods/test_neighbourhood.py
+-rw-r--r--   0        0        0      765 2024-04-21 17:32:24.562290 srai-0.7.3/tests/plotting/test_folium_wrapper.py
+-rw-r--r--   0        0        0     3729 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/conftest.py
+-rw-r--r--   0        0        0     6509 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_administrative_boundary_regionalizer.py
+-rw-r--r--   0        0        0     2616 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_h3_regionalizer.py
+-rw-r--r--   0        0        0     1856 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_s2_regionalizer.py
+-rw-r--r--   0        0        0     2690 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_slippy_map_regionalizer.py
+-rw-r--r--   0        0        0     9215 2024-04-21 17:32:24.562290 srai-0.7.3/tests/regionalizers/test_voronoi_regionalizer.py
+-rw-r--r--   0        0        0    20380 1970-01-01 00:00:00.000000 srai-0.7.3/PKG-INFO
```

### Comparing `srai-0.7.2/LICENSE.md` & `srai-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/README.md` & `srai-0.7.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 * **Pre-computed embeddings** - pre-computed embeddings for different regions and different embedding algorithms
 * **Full pipelines** - full pipelines for different embedding approaches, pre-configured from `srai` components
 * **Image data download and processing** - downloading and processing image data (eg. OSM tiles, etc.)
 
 ### End-to-end examples
 
-Right now, `srai` provides a toolset for data download and processing sufficient to solve downstream tasks. Please see [this project](https://pwr-inf.github.io/Transfer-learning-approach-to-bicycle-sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ](https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations' locations for a wide range of cities worldwide.
+Right now, `srai` provides a toolset for data download and processing sufficient to solve downstream tasks. Please see [this project](https://kraina-ai.github.io/Transfer-learning-approach-to-bicycle-sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ](https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations' locations for a wide range of cities worldwide.
 
 For `srai` integration into full [kedro](https://kedro.org/) pipeline, see [this project](https://github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://github.com/Calychas).
 
 ## Installation
 
 To install `srai` simply run:
```

#### html2text {}

```diff
@@ -27,24 +27,24 @@
 future releases, we plan to add more functionalities, such as: * **Pre-computed
 embeddings** - pre-computed embeddings for different regions and different
 embedding algorithms * **Full pipelines** - full pipelines for different
 embedding approaches, pre-configured from `srai` components * **Image data
 download and processing** - downloading and processing image data (eg. OSM
 tiles, etc.) ### End-to-end examples Right now, `srai` provides a toolset for
 data download and processing sufficient to solve downstream tasks. Please see
-[this project](https://pwr-inf.github.io/Transfer-learning-approach-to-bicycle-
-sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ]
-(https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations'
-locations for a wide range of cities worldwide. For `srai` integration into
-full [kedro](https://kedro.org/) pipeline, see [this project](https://
-github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://github.com/
-Calychas). ## Installation To install `srai` simply run: ```bash pip install
-srai ``` This will install the `srai` package and dependencies required by most
-of the use cases. There are several optional dependencies that can be installed
-to enable additional functionality. These are listed in the [optional
+[this project](https://kraina-ai.github.io/Transfer-learning-approach-to-
+bicycle-sharing-systems-station-location-planning-using-OpenStreetMap/) by
+[@RaczeQ](https://github.com/RaczeQ), which predicts Bike Sharing System (BSS)
+stations' locations for a wide range of cities worldwide. For `srai`
+integration into full [kedro](https://kedro.org/) pipeline, see [this project]
+(https://github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://
+github.com/Calychas). ## Installation To install `srai` simply run: ```bash pip
+install srai ``` This will install the `srai` package and dependencies required
+by most of the use cases. There are several optional dependencies that can be
+installed to enable additional functionality. These are listed in the [optional
 dependencies](#optional-dependencies) section. ### Optional dependencies The
 following optional dependencies can be installed to enable additional
 functionality: * `srai[all]` - all optional dependencies * `srai[osm]` -
 dependencies required to download OpenStreetMap data * `srai[voronoi]` -
 dependencies to use Voronoi-based regionalization method * `srai[gtfs]` -
 dependencies to process GTFS data * `srai[plotting]` - dependencies to plot
 graphs and maps * `srai[torch]` - dependencies to use torch-based embedders ##
```

### Comparing `srai-0.7.2/pyproject.toml` & `srai-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "srai"
-version = "0.7.2"
+version = "0.7.3"
 description = "A set of python modules for geospatial machine learning and data mining"
 authors = [
     { name = "Piotr Gramacki", email = "pgramacki@kraina.ai" },
     { name = "Kacper Leśniara", email = "klesniara@kraina.ai" },
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
     { name = "Szymon Woźniak", email = "swozniak@kraina.ai" },
 ]
@@ -198,15 +198,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.7.2"
+current_version = "0.7.3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `srai-0.7.2/srai/_optional.py` & `srai-0.7.3/srai/_optional.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/_typing.py` & `srai-0.7.3/srai/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/__init__.py` & `srai-0.7.3/srai/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/_base.py` & `srai-0.7.3/srai/embedders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/contextual_count_embedder.py` & `srai-0.7.3/srai/embedders/contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/count_embedder.py` & `srai-0.7.3/srai/embedders/count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/geovex/dataset.py` & `srai-0.7.3/srai/embedders/geovex/dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/geovex/embedder.py` & `srai-0.7.3/srai/embedders/geovex/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/geovex/model.py` & `srai-0.7.3/srai/embedders/geovex/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/gtfs2vec/embedder.py` & `srai-0.7.3/srai/embedders/gtfs2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/gtfs2vec/model.py` & `srai-0.7.3/srai/embedders/gtfs2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/hex2vec/embedder.py` & `srai-0.7.3/srai/embedders/hex2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/hex2vec/model.py` & `srai-0.7.3/srai/embedders/hex2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/hex2vec/neighbour_dataset.py` & `srai-0.7.3/srai/embedders/hex2vec/neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/highway2vec/embedder.py` & `srai-0.7.3/srai/embedders/highway2vec/embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/embedders/highway2vec/model.py` & `srai-0.7.3/srai/embedders/highway2vec/model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/exceptions.py` & `srai-0.7.3/srai/exceptions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/geometry.py` & `srai-0.7.3/srai/geometry.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/h3.py` & `srai-0.7.3/srai/h3.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/joiners/__init__.py` & `srai-0.7.3/srai/joiners/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/joiners/_base.py` & `srai-0.7.3/srai/joiners/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/joiners/intersection_joiner.py` & `srai-0.7.3/srai/joiners/intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/__init__.py` & `srai-0.7.3/srai/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/_base.py` & `srai-0.7.3/srai/loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/download.py` & `srai-0.7.3/srai/loaders/download.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/geoparquet_loader.py` & `srai-0.7.3/srai/loaders/geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/gtfs_loader.py` & `srai-0.7.3/srai/loaders/gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/_base.py` & `srai-0.7.3/srai/loaders/osm_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/filters/_typing.py` & `srai-0.7.3/srai/loaders/osm_loaders/filters/_typing.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/filters/base_osm_groups.py` & `srai-0.7.3/srai/loaders/osm_loaders/filters/base_osm_groups.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/filters/geofabrik.py` & `srai-0.7.3/srai/loaders/osm_loaders/filters/geofabrik.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/filters/hex2vec.py` & `srai-0.7.3/srai/loaders/osm_loaders/filters/hex2vec.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/filters/popular.py` & `srai-0.7.3/srai/loaders/osm_loaders/filters/popular.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/osm_online_loader.py` & `srai-0.7.3/srai/loaders/osm_loaders/osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/osm_pbf_loader.py` & `srai-0.7.3/srai/loaders/osm_loaders/osm_pbf_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         4. https://duckdb.org/
         5. https://github.com/duckdb/duckdb_spatial
     """
 
     def __init__(
         self,
         pbf_file: Optional[Union[str, Path]] = None,
-        download_source: "OsmExtractSource" = "any",
+        download_source: "OsmExtractSource" = "geofabrik",
         download_directory: Union[str, Path] = "files",
     ) -> None:
         """
         Initialize OSMPbfLoader.
 
         Args:
             pbf_file (Union[str, Path], optional): Downloaded `*.osm.pbf` file to be used by
```

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/osm_tile_data_collector.py` & `srai-0.7.3/srai/loaders/osm_loaders/osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_loaders/osm_tile_loader.py` & `srai-0.7.3/srai/loaders/osm_loaders/osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_way_loader/constants.py` & `srai-0.7.3/srai/loaders/osm_way_loader/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/loaders/osm_way_loader/osm_way_loader.py` & `srai-0.7.3/srai/loaders/osm_way_loader/osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/neighbourhoods/_base.py` & `srai-0.7.3/srai/neighbourhoods/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/neighbourhoods/adjacency_neighbourhood.py` & `srai-0.7.3/srai/neighbourhoods/adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/neighbourhoods/h3_neighbourhood.py` & `srai-0.7.3/srai/neighbourhoods/h3_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/plotting/folium_wrapper.py` & `srai-0.7.3/srai/plotting/folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/plotting/plotly_wrapper.py` & `srai-0.7.3/srai/plotting/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/__init__.py` & `srai-0.7.3/srai/regionalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/_base.py` & `srai-0.7.3/srai/regionalizers/_base.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/_spherical_voronoi.py` & `srai-0.7.3/srai/regionalizers/_spherical_voronoi.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/administrative_boundary_regionalizer.py` & `srai-0.7.3/srai/regionalizers/administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/geocode.py` & `srai-0.7.3/srai/regionalizers/geocode.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/h3_regionalizer.py` & `srai-0.7.3/srai/regionalizers/h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/s2_regionalizer.py` & `srai-0.7.3/srai/regionalizers/s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/slippy_map_regionalizer.py` & `srai-0.7.3/srai/regionalizers/slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/srai/regionalizers/voronoi_regionalizer.py` & `srai-0.7.3/srai/regionalizers/voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/conftest.py` & `srai-0.7.3/tests/embedders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/constants.py` & `srai-0.7.3/tests/embedders/geovex/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/generation.py` & `srai-0.7.3/tests/embedders/geovex/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_dataset.py` & `srai-0.7.3/tests/embedders/geovex/test_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_embedder.py` & `srai-0.7.3/tests/embedders/geovex/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_0.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_1.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_2.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_batch_3.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_batch_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_encoder_forward_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_features.parquet` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_0.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_1.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_2.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_forward_3.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_forward_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_joint.parquet` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_0.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_1.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_2.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_2.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_loss_3.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_loss_3.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_regions.parquet` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/AL_10_result.parquet` & `srai-0.7.3/tests/embedders/geovex/test_files/AL_10_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_batch_0.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_batch_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_batch_1.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_batch_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_encoder_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_encoder_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_features.parquet` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_forward_0.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_forward_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_forward_1.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_forward_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_joint.parquet` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_loss_0.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_loss_0.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_loss_1.pt` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_loss_1.pt`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_regions.parquet` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_files/wro_9_result.parquet` & `srai-0.7.3/tests/embedders/geovex/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/geovex/test_model.py` & `srai-0.7.3/tests/embedders/geovex/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/constants.py` & `srai-0.7.3/tests/embedders/hex2vec/constants.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/generation.py` & `srai-0.7.3/tests/embedders/hex2vec/generation.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_embedder.py` & `srai-0.7.3/tests/embedders/hex2vec/test_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_features.parquet` & `srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_joint.parquet` & `srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_regions.parquet` & `srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_files/poz_8_result.parquet` & `srai-0.7.3/tests/embedders/hex2vec/test_files/poz_8_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_features.parquet` & `srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_features.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_joint.parquet` & `srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_joint.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_regions.parquet` & `srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_regions.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_files/wro_9_result.parquet` & `srai-0.7.3/tests/embedders/hex2vec/test_files/wro_9_result.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_model.py` & `srai-0.7.3/tests/embedders/hex2vec/test_model.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/hex2vec/test_neighbour_dataset.py` & `srai-0.7.3/tests/embedders/hex2vec/test_neighbour_dataset.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/test_contextual_count_embedder.py` & `srai-0.7.3/tests/embedders/test_contextual_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/test_count_embedder.py` & `srai-0.7.3/tests/embedders/test_count_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/test_gtfs2vec_embedder.py` & `srai-0.7.3/tests/embedders/test_gtfs2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/embedders/test_highway2vec_embedder.py` & `srai-0.7.3/tests/embedders/test_highway2vec_embedder.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/h3/conftest.py` & `srai-0.7.3/tests/h3/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/h3/test_ij_coordinates.py` & `srai-0.7.3/tests/h3/test_ij_coordinates.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/h3/test_shapely_conversion.py` & `srai-0.7.3/tests/h3/test_shapely_conversion.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/joiners/conftest.py` & `srai-0.7.3/tests/joiners/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/joiners/test_intersection_joiner.py` & `srai-0.7.3/tests/joiners/test_intersection_joiner.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/conftest.py` & `srai-0.7.3/tests/loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/conftest.py` & `srai-0.7.3/tests/loaders/osm_loaders/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/filters/popular_filter_example.json` & `srai-0.7.3/tests/loaders/osm_loaders/filters/popular_filter_example.json`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/filters/test_merge_filter_types.py` & `srai-0.7.3/tests/loaders/osm_loaders/filters/test_merge_filter_types.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py` & `srai-0.7.3/tests/loaders/osm_loaders/filters/test_popular_tag_downloader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `srai-0.7.3/tests/loaders/osm_loaders/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `srai-0.7.3/tests/loaders/osm_loaders/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `srai-0.7.3/tests/loaders/osm_loaders/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_files/monaco.osm.pbf` & `srai-0.7.3/tests/loaders/osm_loaders/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_files/poland.geojson` & `srai-0.7.3/tests/loaders/osm_loaders/test_files/poland.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson` & `srai-0.7.3/tests/loaders/osm_loaders/test_files/south_africa_without_islands.geojson`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_osm_online_loader.py` & `srai-0.7.3/tests/loaders/osm_loaders/test_osm_online_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_osm_pbf_loader.py` & `srai-0.7.3/tests/loaders/osm_loaders/test_osm_pbf_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_osm_tile_data_collector.py` & `srai-0.7.3/tests/loaders/osm_loaders/test_osm_tile_data_collector.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_loaders/test_osm_tile_loader.py` & `srai-0.7.3/tests/loaders/osm_loaders/test_osm_tile_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_1.pkl` & `srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_1.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_2.pkl` & `srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_2.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_3.pkl` & `srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_3.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_way_loader/test_files/graph_4.pkl` & `srai-0.7.3/tests/loaders/osm_way_loader/test_files/graph_4.pkl`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/osm_way_loader/test_osm_way_loader.py` & `srai-0.7.3/tests/loaders/osm_way_loader/test_osm_way_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/test_files/example.parquet` & `srai-0.7.3/tests/loaders/test_files/example.parquet`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/test_geoparquet_loader.py` & `srai-0.7.3/tests/loaders/test_geoparquet_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/loaders/test_gtfs_loader.py` & `srai-0.7.3/tests/loaders/test_gtfs_loader.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/miscellaneous/test_optional_dependencies.py` & `srai-0.7.3/tests/miscellaneous/test_optional_dependencies.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/neighbourhoods/h3/test_no_regions.py` & `srai-0.7.3/tests/neighbourhoods/h3/test_no_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/neighbourhoods/h3/test_with_regions.py` & `srai-0.7.3/tests/neighbourhoods/h3/test_with_regions.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/neighbourhoods/test_adjacency_neighbourhood.py` & `srai-0.7.3/tests/neighbourhoods/test_adjacency_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/neighbourhoods/test_neighbourhood.py` & `srai-0.7.3/tests/neighbourhoods/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/plotting/test_folium_wrapper.py` & `srai-0.7.3/tests/plotting/test_folium_wrapper.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/regionalizers/conftest.py` & `srai-0.7.3/tests/regionalizers/conftest.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/regionalizers/test_administrative_boundary_regionalizer.py` & `srai-0.7.3/tests/regionalizers/test_administrative_boundary_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/regionalizers/test_h3_regionalizer.py` & `srai-0.7.3/tests/regionalizers/test_h3_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/regionalizers/test_s2_regionalizer.py` & `srai-0.7.3/tests/regionalizers/test_s2_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/regionalizers/test_slippy_map_regionalizer.py` & `srai-0.7.3/tests/regionalizers/test_slippy_map_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/tests/regionalizers/test_voronoi_regionalizer.py` & `srai-0.7.3/tests/regionalizers/test_voronoi_regionalizer.py`

 * *Files identical despite different names*

### Comparing `srai-0.7.2/PKG-INFO` & `srai-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srai
-Version: 0.7.2
+Version: 0.7.3
 Summary: A set of python modules for geospatial machine learning and data mining
 Author-Email: Piotr Gramacki <pgramacki@kraina.ai>, =?utf-8?q?Kacper_Le=C5=9Bniara?= <klesniara@kraina.ai>, Kamil Raczycki <kraczycki@kraina.ai>, =?utf-8?q?Szymon_Wo=C5=BAniak?= <swozniak@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -118,15 +118,15 @@
 
 * **Pre-computed embeddings** - pre-computed embeddings for different regions and different embedding algorithms
 * **Full pipelines** - full pipelines for different embedding approaches, pre-configured from `srai` components
 * **Image data download and processing** - downloading and processing image data (eg. OSM tiles, etc.)
 
 ### End-to-end examples
 
-Right now, `srai` provides a toolset for data download and processing sufficient to solve downstream tasks. Please see [this project](https://pwr-inf.github.io/Transfer-learning-approach-to-bicycle-sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ](https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations' locations for a wide range of cities worldwide.
+Right now, `srai` provides a toolset for data download and processing sufficient to solve downstream tasks. Please see [this project](https://kraina-ai.github.io/Transfer-learning-approach-to-bicycle-sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ](https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations' locations for a wide range of cities worldwide.
 
 For `srai` integration into full [kedro](https://kedro.org/) pipeline, see [this project](https://github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://github.com/Calychas).
 
 ## Installation
 
 To install `srai` simply run:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: srai Version: 0.7.2 Summary: A set of python
+Metadata-Version: 2.1 Name: srai Version: 0.7.3 Summary: A set of python
 modules for geospatial machine learning and data mining Author-Email: Piotr
 Gramacki
 kraina.ai>, =?utf-8?q?Kacper_Le=C5=9Bniara?=
 kraina.ai>, Kamil Raczycki
 kraina.ai>, =?utf-8?q?Szymon_Wo=C5=BAniak?=
 kraina.ai> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
@@ -64,24 +64,24 @@
 future releases, we plan to add more functionalities, such as: * **Pre-computed
 embeddings** - pre-computed embeddings for different regions and different
 embedding algorithms * **Full pipelines** - full pipelines for different
 embedding approaches, pre-configured from `srai` components * **Image data
 download and processing** - downloading and processing image data (eg. OSM
 tiles, etc.) ### End-to-end examples Right now, `srai` provides a toolset for
 data download and processing sufficient to solve downstream tasks. Please see
-[this project](https://pwr-inf.github.io/Transfer-learning-approach-to-bicycle-
-sharing-systems-station-location-planning-using-OpenStreetMap/) by [@RaczeQ]
-(https://github.com/RaczeQ), which predicts Bike Sharing System (BSS) stations'
-locations for a wide range of cities worldwide. For `srai` integration into
-full [kedro](https://kedro.org/) pipeline, see [this project](https://
-github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://github.com/
-Calychas). ## Installation To install `srai` simply run: ```bash pip install
-srai ``` This will install the `srai` package and dependencies required by most
-of the use cases. There are several optional dependencies that can be installed
-to enable additional functionality. These are listed in the [optional
+[this project](https://kraina-ai.github.io/Transfer-learning-approach-to-
+bicycle-sharing-systems-station-location-planning-using-OpenStreetMap/) by
+[@RaczeQ](https://github.com/RaczeQ), which predicts Bike Sharing System (BSS)
+stations' locations for a wide range of cities worldwide. For `srai`
+integration into full [kedro](https://kedro.org/) pipeline, see [this project]
+(https://github.com/Calychas/highway2vec_remaster/) by [@Calychas](https://
+github.com/Calychas). ## Installation To install `srai` simply run: ```bash pip
+install srai ``` This will install the `srai` package and dependencies required
+by most of the use cases. There are several optional dependencies that can be
+installed to enable additional functionality. These are listed in the [optional
 dependencies](#optional-dependencies) section. ### Optional dependencies The
 following optional dependencies can be installed to enable additional
 functionality: * `srai[all]` - all optional dependencies * `srai[osm]` -
 dependencies required to download OpenStreetMap data * `srai[voronoi]` -
 dependencies to use Voronoi-based regionalization method * `srai[gtfs]` -
 dependencies to process GTFS data * `srai[plotting]` - dependencies to plot
 graphs and maps * `srai[torch]` - dependencies to use torch-based embedders ##
```

