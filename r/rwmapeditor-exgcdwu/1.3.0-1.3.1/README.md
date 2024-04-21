# Comparing `tmp/rwmapeditor_exgcdwu-1.3.0.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.3.0.tar", last modified: Sun Apr 21 05:32:00 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.3.1.tar", last modified: Sun Apr 21 15:02:58 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.3.0.tar` & `rwmapeditor_exgcdwu-1.3.1.tar`

### file list

```diff
@@ -1,303 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46161 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.765223 rwmapeditor_exgcdwu-1.3.0/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_global.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_one_and_acti.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_otgroup/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_otgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_otgroup/_object_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_add_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/otgroup_grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/otgroup_grid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/_tile_group_addlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/_tile_group_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/_tile_group_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject/_tobject_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/_city.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/_refresh_building.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.805223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/bridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/decoration.png
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/deepwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt.png
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt_details.png
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dust.png
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna.png
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna_highland.png
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice.png
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/misc.png
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain.png
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shortgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone.png
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/units.png
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/water.png
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/decoration.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/misc.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.813223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Deep Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Dirt.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Dirt_Details.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Dust.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Ice.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Lava.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Long Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Mountain.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Sand.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Shallow Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Short Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Snow.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Stone.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/units.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46161 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.526059 rwmapeditor_exgcdwu-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41859 2024-04-21 15:02:58.526059 rwmapeditor_exgcdwu-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.478059 rwmapeditor_exgcdwu-1.3.1/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.482059 rwmapeditor_exgcdwu-1.3.1/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.482059 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.482059 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/otgroup_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/otgroup_grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.482059 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tile_group_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tile_group_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tile_group_grid/_tile_group_addlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tile_group_grid/_tile_group_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tile_group_grid/_tile_group_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.482059 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_mapText.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_mapinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_tobject_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_unitAdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_unitDetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_unitRemove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.482059 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject_group/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject_group/_city.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject_group/_refresh_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.486059 rwmapeditor_exgcdwu-1.3.1/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.486059 rwmapeditor_exgcdwu-1.3.1/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_one_and_acti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.486059 rwmapeditor_exgcdwu-1.3.1/rwmap/_otgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_otgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_otgroup/_object_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.486059 rwmapeditor_exgcdwu-1.3.1/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.486059 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_add_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.486059 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.490059 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.514059 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/bridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/decoration.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/deepwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt_details.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dust.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/fauna.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/fauna_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/fauna_highland.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/misc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shortgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/units.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/water.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/decoration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/misc.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.522059 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.526059 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Deep Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Dirt.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Dirt_Details.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Dust.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Ice.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Lava.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Long Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Mountain.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Sand.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Shallow Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Short Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Snow.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Stone.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/units.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 15:02:58.526059 rwmapeditor_exgcdwu-1.3.1/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41859 2024-04-21 15:02:58.000000 rwmapeditor_exgcdwu-1.3.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-04-21 15:02:58.000000 rwmapeditor_exgcdwu-1.3.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 15:02:58.000000 rwmapeditor_exgcdwu-1.3.1/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 15:02:58.000000 rwmapeditor_exgcdwu-1.3.1/rwmapeditor_exgcdwu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 15:02:58.000000 rwmapeditor_exgcdwu-1.3.1/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 15:02:58.526059 rwmapeditor_exgcdwu-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-21 15:02:54.000000 rwmapeditor_exgcdwu-1.3.1/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/LICENSE` & `rwmapeditor_exgcdwu-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/PKG-INFO` & `rwmapeditor_exgcdwu-1.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.3.0
+Version: 1.3.1
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -686,26 +686,30 @@
 
 # rwmapeditor-exgcdwu
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
+[简易使用教程](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/tutorials.md)
+
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
 
 基本框架已完成。
 
 地块组框架已完成。
 
+宾语组框架已完成。
+
 ## 安装
 
 ```console
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
@@ -720,93 +724,12 @@
 
 #### 2.手动载入地块集
 
 #### 3.手动创建所需的地块层和宾语层
 
 #### 4.即可使用python库改变地块和宾语
 
-## 简易使用例子
-
-```python
-# coding: utf-8
-import rwmap as rw
-
-map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'#此为地图所在文件夹
-map_name = '[p2]example_skirmish_(2p).tmx'#输入地图
-map_name_out = '[p2]example_skirmish_(2p)(1).tmx'#输出地图
-
-mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name)#地图载入
-print(mygraph)#地图输出【部分】
-
-mygraph.addObject(
-    "Triggers", 
-    {"name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1100", "width": "20", "height": "20", "visible": "0"}, 
-    {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
-#添加宾语：第一项图层名称（Triggers），第二项默认属性，第三项可选属性
-#默认属性可添加id也可不添加，没有id项会自动添加
-
-mygraph.addObject(
-    "Triggers", 
-    {"name": "刷兵实验", "type": "unitAdd", "x": "1000", "y":"1500", "width": "20", "height": "20"}, 
-    {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
-
-for tobject in mygraph.iterator_object("Triggers", {"y": "1500"}):#返回属性成功匹配正则表达式的宾语（生成器）
-    del tobject#宾语被删除
-
-for tobject in mygraph.iterator_object("Triggers", {"y": "1100"}):
-    tobject.assignDefaultProperty("name", "名字改变了")#宾语默认属性被赋值
-    tobject.assignOptionalProperty("team", "1")#宾语可选属性被赋值
-    print(tobject.returnDefaultProperty("name"))#输出宾语默认属性
-    print(tobject.returnOptionalProperty("team"))#输出宾语可选属性
-    tobject.deleteDefaultProperty("visible")#删除宾语默认属性
-    tobject.deleteOptionalProperty("resetActivationAfter")#删除宾语可选属性
-
-mygraph.addObject_group(rw.data.RefreshBuilding.init_building(rw.Coordinate(1500, 1000), rw.Coordinate(40, 40), 
-                                               "turret", "acti_tu1", 10, 10,
-                                               name_add = "城市添加", name_detect = "城市检测", 
-                                               warmup_add = 10, warmup_detect = 5))
-#建立一个可自动刷新的建筑
-
-mygraph.addObject_group(rw.data.City.init_city(rw.Coordinate(1500, 1500), rw.Coordinate(40, 40), 
-                                               "turret", "acti_tu2", 10, 10, "城市", textColor = "white", 
-                                               textSize = 50, name_add = "城市添加", name_detect = "城市检测", 
-                                               name_maptext = "城市文本", warmup_add = 10, warmup_detect = 5))
-#建立一个自动刷新的城市，有名字
-
-
-mygraph.addTile("Ground", rw.Coordinate(1, 0), "Long Grass", rw.Coordinate(0, 0))
-mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(1, 2))
-mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
-#改变地块类型：第一项地块层名称，第二项地块层改变位置，第三项地块集名称（全名），第四项所用地块位置（在地块集中）
-
-mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
-mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(20, 5), rw.Coordinate(30, 10)), "Long Grass", rw.Coordinate(2, 1))
-#改变地块类型（矩形）：第一项地块层名称，第二项地块层改变位置（前者为起始位置，后者为增量），第三项地块集名称（全名），第四项所用地块位置（在地块集中）
-
-mygraph.addTile_group(rw.Coordinate(5, 20), rw.data.tile_group_grid.fill_tile_group_one_ground_water_28_24)
-#改变地块类型（地块组）：第一项位置，第二项地块组（使用默认）
-
-tilegroup_matrix = rw.tile.TileGroup_Matrix([['a'] * 6  if i % 2 == 0 else ['b'] * 6 for i in range(10)])
-#创建匿名地块组
-tilegroup_addlayer = rw.tile.TileGroup_AddLayer.init_tilegroup_matrix("Ground", tilegroup_matrix)
-#匿名地块组确定地块层
-tile_dict = {
-    "a": rw.TagCoordinate("Long Grass", rw.Coordinate(0, 0)), 
-    "b": rw.TagCoordinate("Dirt", rw.Coordinate(0, 0))
-}
-tilegroup_one = rw.tile.TileGroup_One.init_tilegroup_addlayer(
-    tile_dict, tilegroup_addlayer)
-#匿名地块组确定地块类型
-
-mygraph.addTile_group(rw.Coordinate(20, 20), tilegroup_one)
-#添加地块组
-
-mygraph.write_file(map_dir + map_name_out)
-#输出到新地图文件
-
-```
-
 ## 其他
 
 ### 外部文件
 
 本库使用了铁锈战争的默认地块集，存放在rwmap/other_data/maps/
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_case/_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 
 """
 import xml.etree.ElementTree as et
 import numpy as np
 
 import rwmap._util as utility
 import rwmap._frame as frame
+from rwmap._frame._element_ori import ElementOri
+from rwmap._frame._element_property import ElementProperties
 
-class Layer(frame.ElementOri):
-    def __init__(self, properties:frame.ElementProperties, tilematrix:np.ndarray, encoding:str, compression:str)->None:
+class Layer(ElementOri):
+    def __init__(self, properties:ElementProperties, tilematrix:np.ndarray, encoding:str, compression:str)->None:
         super().__init__(properties)
         self._tilematrix = tilematrix
         self._encoding = encoding
         self._compression = compression
     @classmethod
     def init_etElement(cls, root:et.Element)->None:
-        properties = frame.ElementProperties.init_etElement(root)
+        properties = ElementProperties.init_etElement(root)
         data = utility.get_etElement_callable_from_tag(root, "data")
         _tilematrix = utility.get_etElement_ndarray_from_text_packed(data, frame.Coordinate(root.attrib['width'], root.attrib['height']))
         return cls(properties, _tilematrix, data.attrib["encoding"], data.attrib["compression"])
 
     def output_str(self, output_rectangle:frame.Rectangle = frame.Rectangle(frame.Coordinate(), frame.Coordinate(-1, -1)))->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_case/_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import xml.etree.ElementTree as et
 
 import rwmap._frame as frame
 import rwmap._util as utility
-class TObject(frame.ElementProperties):
+from rwmap._frame._element_property import ElementProperties
+
+class TObject(ElementProperties):
     def __init__(self, tag:str, default_properties:dict[str, str] = {}, optional_properties:dict[str, str] = {}, other_properties:list[et.Element] = [])->None:
         super().__init__(tag, default_properties, optional_properties)
         self._other_properties = other_properties
         
     @classmethod
     def init_etElement(cls, root:et.Element):
         if root == None:
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_case/_objectgroup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 """
 
 import xml.etree.ElementTree as et
 
 import rwmap._util as utility
 import rwmap._frame as frame
 from rwmap._case._object import TObject
+from rwmap._frame._element_ori import ElementOri
+from rwmap._frame._element_property import ElementProperties
 
-class ObjectGroup(frame.ElementOri):
-    def __init__(self, properties:frame.ElementProperties, object_list:list[TObject])->None:
+class ObjectGroup(ElementOri):
+    def __init__(self, properties:ElementProperties, object_list:list[TObject])->None:
         super().__init__(properties)
         self._object_list = object_list
 
     def __iter__(self):
         return self._object_list
 
     @classmethod
     def init_etElement(cls, root:et.Element)->None:
-        properties = frame.ElementProperties.init_etElement(root)
+        properties = ElementProperties.init_etElement(root)
         object_list = [TObject.init_etElement(tobject) for tobject in root if tobject.tag == "object"]
         return cls(properties, object_list)
     
     def output_str(self, objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "".join([self._object_list[i].output_str() + "\n" for i in range(0, -1)]) + "\n"
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_case/_tileset.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 """
 import xml.etree.ElementTree as et
 
 import rwmap._util as utility
 import rwmap._frame as frame
 import rwmap._exceptions as exception
+from rwmap._frame._element_ori import ElementOri
+from rwmap._frame._element_property import ElementProperties
 
-class TileSet(frame.ElementOri):
-    def __init__(self, properties:frame.ElementProperties, size:frame.Coordinate, image_properties:frame.ElementProperties = None,
-                  png_text:str = None, tilelist_properties:list[frame.ElementProperties] = None)->None:
+class TileSet(ElementOri):
+    def __init__(self, properties:ElementProperties, size:frame.Coordinate, image_properties:ElementProperties = None,
+                  png_text:str = None, tilelist_properties:list[ElementProperties] = None)->None:
         super().__init__(properties)
         self._size = size
         self._image_properties = image_properties
         self._png_text = png_text
         self._tilelist_properties = tilelist_properties
     @classmethod
     def init_etElement(cls, root:et.Element, rwmaps_dir:str)->None:
         png_text_pro = utility.get_etElement_callable_from_tag(root, "properties")
         png_text = utility.get_etElement_name_to_text_rm(png_text_pro, "embedded_png")
-        properties = frame.ElementProperties.init_etElement(root)
-        image_properties = frame.ElementProperties.init_etElement(utility.get_etElement_callable_from_tag(root, "image"))
-        tilelist_properties = [frame.ElementProperties.init_etElement(tile) for tile in root if tile.tag == "tile"]
+        properties = ElementProperties.init_etElement(root)
+        image_properties = ElementProperties.init_etElement(utility.get_etElement_callable_from_tag(root, "image"))
+        tilelist_properties = [ElementProperties.init_etElement(tile) for tile in root if tile.tag == "tile"]
         tilelist_properties = None if tilelist_properties == [] else tilelist_properties
         
         if properties.returnDefaultProperty("columns") == None:
             source_file = properties.returnDefaultProperty("source")
 
             source = rwmaps_dir + source_file
             root = et.ElementTree(file = source).getroot()
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,36 +7,38 @@
 import os
 from typing import Generator
 
 import rwmap._exceptions as rwexceptions
 import rwmap._util as utility
 import rwmap._case as case
 import rwmap._frame as frame
+from rwmap._frame._element_ori import ElementOri
+from rwmap._frame._element_property import ElementProperties
 import rwmap._tile as tile
 import rwmap._object as object
 import rwmap._otgroup as otgroup
 
 
 RWMAP_DIR = os.path.dirname(__file__)
 RWMAP_MAPS = RWMAP_DIR + "/other_data/maps/"
 
-class RWmap(frame.ElementOri):
-    def __init__(self, properties:frame.ElementProperties, tileset_list:list[case.TileSet],
+class RWmap(ElementOri):
+    def __init__(self, properties:ElementProperties, tileset_list:list[case.TileSet],
                   layer_list:list[case.Layer], objectGroup_list:list[case.ObjectGroup])->None:
         super().__init__(properties)
         self._tileset_list = tileset_list
         self._layer_list = layer_list
         self._objectGroup_list = objectGroup_list
     @classmethod
     def init_mapfile(cls, map_file:str, rwmaps_dir = RWMAP_MAPS)->None:
         xmlTree:et.ElementTree = et.ElementTree(file=map_file)
         root:et.Element = xmlTree.getroot()
-        properties = frame.ElementProperties.init_etElement(root)
+        properties = ElementProperties.init_etElement(root)
 
-        tileset_list = [case.TileSet(frame.ElementProperties("tileset", {"firstgid": "0", "name": "empty"}), frame.Coordinate(1, 1))]
+        tileset_list = [case.TileSet(ElementProperties("tileset", {"firstgid": "0", "name": "empty"}), frame.Coordinate(1, 1))]
         tileset_list = tileset_list + [case.TileSet.init_etElement(tileset, rwmaps_dir) for tileset in root if tileset.tag == "tileset"]
         layer_list = [case.Layer.init_etElement(layer) for layer in root if layer.tag == "layer"]
         objectGroup_list = [case.ObjectGroup.init_etElement(objectGroup) for objectGroup in root if objectGroup.tag == "objectgroup"]  
         
         tileset_list = None if tileset_list == [] else tileset_list
         layer_list = None if layer_list == [] else layer_list
         objectGroup_list = None if objectGroup_list == [] else objectGroup_list
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_frame/_coordinate.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_frame/_element_property.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_global.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_global.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_group.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_one_and_acti.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_one_and_acti.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_pos.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_pos.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_time.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_time.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_type.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_object/_object_type.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_tile/_tile_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_add_dict.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_add_dict.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/data/const.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_data/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import rwmap._frame as frame
+
 
 class KEY:
     empty_tile = "0"
 
 class NAME:
     Ground = "Ground"
     Triggers = "Triggers"
@@ -22,10 +24,13 @@
     NONE = "NONE"
     mainBuildings = "mainBuildings"
     allUnitsAndBuildings = "allUnitsAndBuildings"
     allBuildings = "allBuildings"
     commandCenter = "commandCenter"
     requiredObjectives = "requiredObjectives"
 
+class COO:
+    SIZE_STANDARD = frame.Coordinate(20, 20)
+
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject/_tobject_one.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject/_tobject_one.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/_city.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject_group/_city.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Union
 
 import rwmap._object as object
 import rwmap._frame as frame
-import rwmap.data.tobject._tobject_one as tobject_one
+import rwmap._data.tobject as tobject
 
 class City(object.TObject_Group):
     @classmethod
     def init_city(cls, pos: frame.Coordinate, size: frame.Coordinate, spawnUnits:str, id_detect:str, 
                   reset_add:int, reset_detect:int, text:str, textColor:str = None, textSize:int = -1, 
                   name_add:str = None, name_detect:str = None, name_maptext:str = None, 
                   warmup_add:int = -1, warmup_detect:int = -1, techLevel:int = -1):
-        uadd = tobject_one.unitAdd(pos, -1, spawnUnits, name = name_add, warmup = warmup_add, 
+        uadd = tobject.UnitAdd(pos, -1, spawnUnits, name = name_add, warmup = warmup_add, 
                                    reset = reset_add, techLevel = techLevel)
-        udetect = tobject_one.unitDetect(pos, size, name = name_detect, maxUnits = 0, 
+        udetect = tobject.UnitDetect(pos, size, name = name_detect, maxUnits = 0, 
                                          unitType = spawnUnits, warmup = warmup_detect, reset = reset_detect, 
                                          id = id_detect)
-        maptext = tobject_one.mapText(pos, text = text, textColor = textColor, textSize = textSize, 
+        maptext = tobject.MapText(pos, text = text, textColor = textColor, textSize = textSize, 
                                       name = name_maptext)
         tobn = udetect.return_idTObject()
         uadd.add_actiBy([tobn])
         return cls([uadd, udetect, maptext])
     
     def return_idTObject(self)->Union[object.TObject_One, None]:
         return self._TObject_One_list[1].return_idTObject()
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/_refresh_building.py` & `rwmapeditor_exgcdwu-1.3.1/rwmap/_data/tobject_group/_refresh_building.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from typing import Union
 
 import rwmap._object as object
 import rwmap._frame as frame
-import rwmap.data.tobject._tobject_one as tobject_one
-
-
+import rwmap.data.tobject as tobject
 
 class RefreshBuilding(object.TObject_Group):
     @classmethod
     def init_building(cls, pos: frame.Coordinate, size: frame.Coordinate, spawnUnits:str, id_detect:str, 
                   reset_add:int, reset_detect:int, name_add:str = None, name_detect:str = None, 
                   warmup_add:int = -1, warmup_detect:int = -1, techLevel:int = -1):
-        uadd = tobject_one.unitAdd(pos, -1, spawnUnits, name = name_add, warmup = warmup_add, 
+        uadd = tobject.UnitAdd(pos, -1, spawnUnits, name = name_add, warmup = warmup_add, 
                                    reset = reset_add, techLevel = techLevel)
-        udetect = tobject_one.unitDetect(pos, size, name = name_detect, maxUnits = 0, 
+        udetect = tobject.UnitDetect(pos, size, name = name_detect, maxUnits = 0, 
                                          unitType = spawnUnits, warmup = warmup_detect, reset = reset_detect, 
                                          id = id_detect)
         tobn = udetect.return_idTObject()
         uadd.add_actiBy([tobn])
         return cls([uadd, udetect])
     
     def return_idTObject(self)->Union[object.TObject_One, None]:
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/bridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/bridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/decoration.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/decoration.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/deepwater.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/deepwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt_details.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dirt_details.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dust.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/dust.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/fauna.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna_dark.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/fauna_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna_highland.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/fauna_highland.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2ice_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/lava2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/misc.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/misc.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2road_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/nothing2road_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2_old.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2ice_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2lava_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_hill.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2sand_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2stone_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand_dark.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sand_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shortgrass.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/shortgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_hill.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2snow_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2lava.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/units.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/units.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/water.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/water.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/misc.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/misc.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Lava.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/terrain/Lava.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/units.tsx` & `rwmapeditor_exgcdwu-1.3.1/rwmap/other_data/maps/units.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.3.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.3.0
+Version: 1.3.1
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -686,26 +686,30 @@
 
 # rwmapeditor-exgcdwu
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
 ![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
+[简易使用教程](https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-/tutorials.md)
+
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
 
 基本框架已完成。
 
 地块组框架已完成。
 
+宾语组框架已完成。
+
 ## 安装
 
 ```console
 pip install rwmapeditor-exgcdwu
 ```
 
 ## 使用之前
@@ -720,93 +724,12 @@
 
 #### 2.手动载入地块集
 
 #### 3.手动创建所需的地块层和宾语层
 
 #### 4.即可使用python库改变地块和宾语
 
-## 简易使用例子
-
-```python
-# coding: utf-8
-import rwmap as rw
-
-map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'#此为地图所在文件夹
-map_name = '[p2]example_skirmish_(2p).tmx'#输入地图
-map_name_out = '[p2]example_skirmish_(2p)(1).tmx'#输出地图
-
-mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name)#地图载入
-print(mygraph)#地图输出【部分】
-
-mygraph.addObject(
-    "Triggers", 
-    {"name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1100", "width": "20", "height": "20", "visible": "0"}, 
-    {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
-#添加宾语：第一项图层名称（Triggers），第二项默认属性，第三项可选属性
-#默认属性可添加id也可不添加，没有id项会自动添加
-
-mygraph.addObject(
-    "Triggers", 
-    {"name": "刷兵实验", "type": "unitAdd", "x": "1000", "y":"1500", "width": "20", "height": "20"}, 
-    {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
-
-for tobject in mygraph.iterator_object("Triggers", {"y": "1500"}):#返回属性成功匹配正则表达式的宾语（生成器）
-    del tobject#宾语被删除
-
-for tobject in mygraph.iterator_object("Triggers", {"y": "1100"}):
-    tobject.assignDefaultProperty("name", "名字改变了")#宾语默认属性被赋值
-    tobject.assignOptionalProperty("team", "1")#宾语可选属性被赋值
-    print(tobject.returnDefaultProperty("name"))#输出宾语默认属性
-    print(tobject.returnOptionalProperty("team"))#输出宾语可选属性
-    tobject.deleteDefaultProperty("visible")#删除宾语默认属性
-    tobject.deleteOptionalProperty("resetActivationAfter")#删除宾语可选属性
-
-mygraph.addObject_group(rw.data.RefreshBuilding.init_building(rw.Coordinate(1500, 1000), rw.Coordinate(40, 40), 
-                                               "turret", "acti_tu1", 10, 10,
-                                               name_add = "城市添加", name_detect = "城市检测", 
-                                               warmup_add = 10, warmup_detect = 5))
-#建立一个可自动刷新的建筑
-
-mygraph.addObject_group(rw.data.City.init_city(rw.Coordinate(1500, 1500), rw.Coordinate(40, 40), 
-                                               "turret", "acti_tu2", 10, 10, "城市", textColor = "white", 
-                                               textSize = 50, name_add = "城市添加", name_detect = "城市检测", 
-                                               name_maptext = "城市文本", warmup_add = 10, warmup_detect = 5))
-#建立一个自动刷新的城市，有名字
-
-
-mygraph.addTile("Ground", rw.Coordinate(1, 0), "Long Grass", rw.Coordinate(0, 0))
-mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(1, 2))
-mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
-#改变地块类型：第一项地块层名称，第二项地块层改变位置，第三项地块集名称（全名），第四项所用地块位置（在地块集中）
-
-mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
-mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(20, 5), rw.Coordinate(30, 10)), "Long Grass", rw.Coordinate(2, 1))
-#改变地块类型（矩形）：第一项地块层名称，第二项地块层改变位置（前者为起始位置，后者为增量），第三项地块集名称（全名），第四项所用地块位置（在地块集中）
-
-mygraph.addTile_group(rw.Coordinate(5, 20), rw.data.tile_group_grid.fill_tile_group_one_ground_water_28_24)
-#改变地块类型（地块组）：第一项位置，第二项地块组（使用默认）
-
-tilegroup_matrix = rw.tile.TileGroup_Matrix([['a'] * 6  if i % 2 == 0 else ['b'] * 6 for i in range(10)])
-#创建匿名地块组
-tilegroup_addlayer = rw.tile.TileGroup_AddLayer.init_tilegroup_matrix("Ground", tilegroup_matrix)
-#匿名地块组确定地块层
-tile_dict = {
-    "a": rw.TagCoordinate("Long Grass", rw.Coordinate(0, 0)), 
-    "b": rw.TagCoordinate("Dirt", rw.Coordinate(0, 0))
-}
-tilegroup_one = rw.tile.TileGroup_One.init_tilegroup_addlayer(
-    tile_dict, tilegroup_addlayer)
-#匿名地块组确定地块类型
-
-mygraph.addTile_group(rw.Coordinate(20, 20), tilegroup_one)
-#添加地块组
-
-mygraph.write_file(map_dir + map_name_out)
-#输出到新地图文件
-
-```
-
 ## 其他
 
 ### 外部文件
 
 本库使用了铁锈战争的默认地块集，存放在rwmap/other_data/maps/
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.3.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,35 @@
 rwmap/_core.py
 rwmap/_exceptions.py
 rwmap/_case/__init__.py
 rwmap/_case/_layer.py
 rwmap/_case/_object.py
 rwmap/_case/_objectgroup.py
 rwmap/_case/_tileset.py
+rwmap/_data/__init__.py
+rwmap/_data/const.py
+rwmap/_data/otgroup_grid/__init__.py
+rwmap/_data/tile_group_grid/__init__.py
+rwmap/_data/tile_group_grid/_tile_group_addlayer.py
+rwmap/_data/tile_group_grid/_tile_group_matrix.py
+rwmap/_data/tile_group_grid/_tile_group_one.py
+rwmap/_data/tobject/__init__.py
+rwmap/_data/tobject/_camera.py
+rwmap/_data/tobject/_credit.py
+rwmap/_data/tobject/_mapText.py
+rwmap/_data/tobject/_mapinfo.py
+rwmap/_data/tobject/_message.py
+rwmap/_data/tobject/_node.py
+rwmap/_data/tobject/_tobject_one.py
+rwmap/_data/tobject/_unitAdd.py
+rwmap/_data/tobject/_unitDetect.py
+rwmap/_data/tobject/_unitRemove.py
+rwmap/_data/tobject_group/__init__.py
+rwmap/_data/tobject_group/_city.py
+rwmap/_data/tobject_group/_refresh_building.py
 rwmap/_frame/__init__.py
 rwmap/_frame/_coordinate.py
 rwmap/_frame/_element_ori.py
 rwmap/_frame/_element_property.py
 rwmap/_object/__init__.py
 rwmap/_object/_object_global.py
 rwmap/_object/_object_group.py
@@ -29,26 +50,14 @@
 rwmap/_util/_add_dict.py
 rwmap/_util/_class_rel.py
 rwmap/_util/_dict_util.py
 rwmap/_util/_etElement_process.py
 rwmap/_util/_list_util.py
 rwmap/_util/_png_rel.py
 rwmap/_util/_str_util.py
-rwmap/data/__init__.py
-rwmap/data/const.py
-rwmap/data/otgroup_grid/__init__.py
-rwmap/data/tile_group_grid/__init__.py
-rwmap/data/tile_group_grid/_tile_group_addlayer.py
-rwmap/data/tile_group_grid/_tile_group_matrix.py
-rwmap/data/tile_group_grid/_tile_group_one.py
-rwmap/data/tobject/__init__.py
-rwmap/data/tobject/_tobject_one.py
-rwmap/data/tobject_group/__init__.py
-rwmap/data/tobject_group/_city.py
-rwmap/data/tobject_group/_refresh_building.py
 rwmap/other_data/requirements.txt
 rwmap/other_data/maps/decoration.tsx
 rwmap/other_data/maps/misc.tsx
 rwmap/other_data/maps/units.tsx
 rwmap/other_data/maps/bitmaps/bridge.png
 rwmap/other_data/maps/bitmaps/decoration.png
 rwmap/other_data/maps/bitmaps/deepwater.png
```

### Comparing `rwmapeditor_exgcdwu-1.3.0/setup.py` & `rwmapeditor_exgcdwu-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 import os
 from setuptools import setup, find_packages
 
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 
 def read_file(file:str):
     with open(file) as file:
         return file.read()
 
 def readline_file(file:str):
     with open(file) as file:
```

