# Comparing `tmp/rwmapeditor_exgcdwu-1.2.8.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.2.8.tar", last modified: Fri Apr 19 16:50:09 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.3.0.tar", last modified: Sun Apr 21 05:32:00 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.2.8.tar` & `rwmapeditor_exgcdwu-1.3.0.tar`

### file list

```diff
@@ -1,290 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.662061 rwmapeditor_exgcdwu-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    45268 2024-04-19 16:50:09.658061 rwmapeditor_exgcdwu-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.610061 rwmapeditor_exgcdwu-1.2.8/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.614061 rwmapeditor_exgcdwu-1.2.8/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_case/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.614061 rwmapeditor_exgcdwu-1.2.8/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.614061 rwmapeditor_exgcdwu-1.2.8/rwmap/_object/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_object/_object_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_object/_object_one.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_object/_object_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_object/_object_pro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.614061 rwmapeditor_exgcdwu-1.2.8/rwmap/_tile/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_tile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_tile/_tile_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.614061 rwmapeditor_exgcdwu-1.2.8/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_util/_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_util/_list_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.614061 rwmapeditor_exgcdwu-1.2.8/rwmap/data/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/data/default_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.618061 rwmapeditor_exgcdwu-1.2.8/rwmap/data/tile_group_grid/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/data/tile_group_grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/data/tile_group_grid/_tile_group_addlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/data/tile_group_grid/_tile_group_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/data/tile_group_grid/tile_group_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.618061 rwmapeditor_exgcdwu-1.2.8/rwmap/data/tobject_group_COP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/data/tobject_group_COP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.618061 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.618061 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.646061 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/bridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/decoration.png
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/deepwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt.png
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt_details.png
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dust.png
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/fauna.png
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/fauna_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/fauna_highland.png
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice.png
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/misc.png
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain.png
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2_old.png
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater.png
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shortgrass.png
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone.png
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2lava.png
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2snow.png
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
--rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/units.png
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/water.png
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/decoration.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/misc.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.658061 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.658061 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Deep Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Dirt.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Dirt_Details.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Dust.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Ice.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Lava.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Long Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Mountain.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Sand.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Shallow Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Short Grass.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Snow.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Stone.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Water.tsx
--rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/units.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:50:09.658061 rwmapeditor_exgcdwu-1.2.8/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45268 2024-04-19 16:50:09.000000 rwmapeditor_exgcdwu-1.2.8/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13076 2024-04-19 16:50:09.000000 rwmapeditor_exgcdwu-1.2.8/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:50:09.000000 rwmapeditor_exgcdwu-1.2.8/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 16:50:09.000000 rwmapeditor_exgcdwu-1.2.8/rwmapeditor_exgcdwu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 16:50:09.000000 rwmapeditor_exgcdwu-1.2.8/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-19 16:50:09.662061 rwmapeditor_exgcdwu-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-19 16:50:00.000000 rwmapeditor_exgcdwu-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46161 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.765223 rwmapeditor_exgcdwu-1.3.0/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_one_and_acti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_object/_object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_otgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_otgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_otgroup/_object_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.769223 rwmapeditor_exgcdwu-1.3.0/rwmap/_tile/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_tile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_tile/_tile_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_add_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_list_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/otgroup_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/otgroup_grid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/_tile_group_addlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/_tile_group_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tile_group_grid/_tile_group_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject/_tobject_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/_city.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/data/tobject_group/_refresh_building.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.773223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.805223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)    66356 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/bridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/decoration.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/deepwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11405 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt_details.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dust.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna_highland.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8192 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7462 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16262 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15956 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16817 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17019 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/misc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9946 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13645 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2road_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2_old.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2ice_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2lava_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10227 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2stone_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6980 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23903 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shortgrass.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_hill.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2lava.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2sand_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7374 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111877 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/units.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/water.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/decoration.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/misc.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.813223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Dirt Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Dirt ShalowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Ice Ice - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Ice ShallowWater - Broken.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Ice ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass ShortGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain LongGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Mountain - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Mountain - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Snow - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Stone - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Nothing Dust - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Nothing Road - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Nothing Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand LandGrass - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Nothing - Flat - 2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Nothing - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Sand - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand ShallowWater - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand ShallowWater - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/ShallowWater Water - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Dirt - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Dirt - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Ice - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Snow - Hill.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Snow Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Sand - Flat.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone ShallowWater - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Snow - ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Water DeepWater - Flat.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Deep Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Dirt.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Dirt_Details.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Dust.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Ice.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Lava.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Long Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Mountain.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Sand.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Shallow Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Short Grass.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Snow.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Stone.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Water.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)    22727 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/units.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46161 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 05:32:00.000000 rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 05:32:00.817223 rwmapeditor_exgcdwu-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-21 05:31:53.000000 rwmapeditor_exgcdwu-1.3.0/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/LICENSE` & `rwmapeditor_exgcdwu-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/PKG-INFO` & `rwmapeditor_exgcdwu-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.2.8
+Version: 1.3.0
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -675,15 +675,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Requires-Python: >=3.5.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.26.4
 
 # rwmapeditor-exgcdwu
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
@@ -735,35 +735,48 @@
 map_name_out = '[p2]example_skirmish_(2p)(1).tmx'#输出地图
 
 mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name)#地图载入
 print(mygraph)#地图输出【部分】
 
 mygraph.addObject(
     "Triggers", 
-    {"name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20", "visible": "0"}, 
+    {"name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1100", "width": "20", "height": "20", "visible": "0"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 #添加宾语：第一项图层名称（Triggers），第二项默认属性，第三项可选属性
 #默认属性可添加id也可不添加，没有id项会自动添加
 
 mygraph.addObject(
     "Triggers", 
     {"name": "刷兵实验", "type": "unitAdd", "x": "1000", "y":"1500", "width": "20", "height": "20"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
-for tobject in mygraph.iterator_object("Triggers", {"y": "1500"}):#返回属性成功匹配正则表达式的宾语
+for tobject in mygraph.iterator_object("Triggers", {"y": "1500"}):#返回属性成功匹配正则表达式的宾语（生成器）
     del tobject#宾语被删除
 
-for tobject in mygraph.iterator_object("Triggers", {"y": "1000"}):
+for tobject in mygraph.iterator_object("Triggers", {"y": "1100"}):
     tobject.assignDefaultProperty("name", "名字改变了")#宾语默认属性被赋值
     tobject.assignOptionalProperty("team", "1")#宾语可选属性被赋值
     print(tobject.returnDefaultProperty("name"))#输出宾语默认属性
     print(tobject.returnOptionalProperty("team"))#输出宾语可选属性
     tobject.deleteDefaultProperty("visible")#删除宾语默认属性
     tobject.deleteOptionalProperty("resetActivationAfter")#删除宾语可选属性
 
+mygraph.addObject_group(rw.data.RefreshBuilding.init_building(rw.Coordinate(1500, 1000), rw.Coordinate(40, 40), 
+                                               "turret", "acti_tu1", 10, 10,
+                                               name_add = "城市添加", name_detect = "城市检测", 
+                                               warmup_add = 10, warmup_detect = 5))
+#建立一个可自动刷新的建筑
+
+mygraph.addObject_group(rw.data.City.init_city(rw.Coordinate(1500, 1500), rw.Coordinate(40, 40), 
+                                               "turret", "acti_tu2", 10, 10, "城市", textColor = "white", 
+                                               textSize = 50, name_add = "城市添加", name_detect = "城市检测", 
+                                               name_maptext = "城市文本", warmup_add = 10, warmup_detect = 5))
+#建立一个自动刷新的城市，有名字
+
+
 mygraph.addTile("Ground", rw.Coordinate(1, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(1, 2))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 #改变地块类型：第一项地块层名称，第二项地块层改变位置，第三项地块集名称（全名），第四项所用地块位置（在地块集中）
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(20, 5), rw.Coordinate(30, 10)), "Long Grass", rw.Coordinate(2, 1))
@@ -793,11 +806,7 @@
 ```
 
 ## 其他
 
 ### 外部文件
 
 本库使用了铁锈战争的默认地块集，存放在rwmap/other_data/maps/
-
-### 第三方库依赖
-
-numpy
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/README.md` & `rwmapeditor_exgcdwu-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -49,35 +49,48 @@
 map_name_out = '[p2]example_skirmish_(2p)(1).tmx'#输出地图
 
 mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name)#地图载入
 print(mygraph)#地图输出【部分】
 
 mygraph.addObject(
     "Triggers", 
-    {"name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20", "visible": "0"}, 
+    {"name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1100", "width": "20", "height": "20", "visible": "0"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 #添加宾语：第一项图层名称（Triggers），第二项默认属性，第三项可选属性
 #默认属性可添加id也可不添加，没有id项会自动添加
 
 mygraph.addObject(
     "Triggers", 
     {"name": "刷兵实验", "type": "unitAdd", "x": "1000", "y":"1500", "width": "20", "height": "20"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
-for tobject in mygraph.iterator_object("Triggers", {"y": "1500"}):#返回属性成功匹配正则表达式的宾语
+for tobject in mygraph.iterator_object("Triggers", {"y": "1500"}):#返回属性成功匹配正则表达式的宾语（生成器）
     del tobject#宾语被删除
 
-for tobject in mygraph.iterator_object("Triggers", {"y": "1000"}):
+for tobject in mygraph.iterator_object("Triggers", {"y": "1100"}):
     tobject.assignDefaultProperty("name", "名字改变了")#宾语默认属性被赋值
     tobject.assignOptionalProperty("team", "1")#宾语可选属性被赋值
     print(tobject.returnDefaultProperty("name"))#输出宾语默认属性
     print(tobject.returnOptionalProperty("team"))#输出宾语可选属性
     tobject.deleteDefaultProperty("visible")#删除宾语默认属性
     tobject.deleteOptionalProperty("resetActivationAfter")#删除宾语可选属性
 
+mygraph.addObject_group(rw.data.RefreshBuilding.init_building(rw.Coordinate(1500, 1000), rw.Coordinate(40, 40), 
+                                               "turret", "acti_tu1", 10, 10,
+                                               name_add = "城市添加", name_detect = "城市检测", 
+                                               warmup_add = 10, warmup_detect = 5))
+#建立一个可自动刷新的建筑
+
+mygraph.addObject_group(rw.data.City.init_city(rw.Coordinate(1500, 1500), rw.Coordinate(40, 40), 
+                                               "turret", "acti_tu2", 10, 10, "城市", textColor = "white", 
+                                               textSize = 50, name_add = "城市添加", name_detect = "城市检测", 
+                                               name_maptext = "城市文本", warmup_add = 10, warmup_detect = 5))
+#建立一个自动刷新的城市，有名字
+
+
 mygraph.addTile("Ground", rw.Coordinate(1, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(1, 2))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 #改变地块类型：第一项地块层名称，第二项地块层改变位置，第三项地块集名称（全名），第四项所用地块位置（在地块集中）
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(20, 5), rw.Coordinate(30, 10)), "Long Grass", rw.Coordinate(2, 1))
@@ -107,11 +120,7 @@
 ```
 
 ## 其他
 
 ### 外部文件
 
 本库使用了铁锈战争的默认地块集，存放在rwmap/other_data/maps/
-
-### 第三方库依赖
-
-numpy
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_layer.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
     def output_etElement(self)->et.Element:
         root = et.Element("layer")
         self._properties.output_etElement(root)
         root.append(utility.get_etElement_from_text_packed(self._tilematrix, self._encoding, self._compression))
         return root
     
+    def __repr__(self)->str:
+        return self.output_str()
+
     def id(self)->int:
         return int(self._properties.default_properties["id"])
     
     def tileid(self, place_grid:frame.Coordinate)->int:
         return int(self._tilematrix[place_grid.x()][place_grid.y()])
     
     def assigntileid(self, place_grid:frame.Coordinate, tileid:int):
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_case/_object.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_object.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,8 +25,11 @@
         
     def output_str(self)->str:
         str_ans = super().output_str()
         str_add = "other_properties:" + str(self._other_properties) + "\n"
         str_add = utility.indentstr_Tab(str_ans)
         str_ans = str_ans + str_add
         return str_ans
+    
+    def __repr__(self)->str:
+        return self.output_str()
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_objectgroup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     
     def output_str(self, objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "".join([self._object_list[i].output_str() + "\n" for i in range(0, -1)]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
+    
+    def __repr__(self)->str:
+        return self.output_str()
 
     def output_etElement(self)->et.Element:
         root = et.Element("objectgroup")
         self._properties.output_etElement(root)
         for tobject in self._object_list:
             tobject_element = et.Element("object")
             tobject.output_etElement(tobject_element)
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_case/_tileset.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
         if self._png_text != None:
             _png_text_now = self._png_text[:pngtextnum] if pngtextnum != -1 else ""
             str_ans = str_ans + _png_text_now + "\n"
         if self._tilelist_properties != None:
             str_ans = str_ans + "".join([self._tilelist_properties[i].output_str() + "\n" for i in range(0, tilenum)]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
         return str_ans
+    
+    def __repr__(self)->str:
+        return self.output_str()
 
     def output_etElement(self)->et.Element:
         root = et.Element("tileset")
         self._properties.output_etElement(root)
         if self._image_properties != None:
             image_element = et.Element("image")
             self._image_properties.output_etElement(image_element)
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from typing import Generator
 
 import rwmap._exceptions as rwexceptions
 import rwmap._util as utility
 import rwmap._case as case
 import rwmap._frame as frame
 import rwmap._tile as tile
+import rwmap._object as object
+import rwmap._otgroup as otgroup
 
 
 RWMAP_DIR = os.path.dirname(__file__)
 RWMAP_MAPS = RWMAP_DIR + "/other_data/maps/"
 
 class RWmap(frame.ElementOri):
     def __init__(self, properties:frame.ElementProperties, tileset_list:list[case.TileSet],
@@ -37,14 +39,22 @@
         
         tileset_list = None if tileset_list == [] else tileset_list
         layer_list = None if layer_list == [] else layer_list
         objectGroup_list = None if objectGroup_list == [] else objectGroup_list
         
         return cls(properties, tileset_list, layer_list, objectGroup_list)
 
+    def size(self)->frame.Coordinate:
+        return frame.Coordinate(int(self._properties.returnDefaultProperty("width")), 
+                                int(self._properties.returnDefaultProperty("height")))
+    
+    def tile_size(self)->frame.Coordinate:
+        return frame.Coordinate(int(self._properties.returnDefaultProperty("tilewidth")), 
+                                int(self._properties.returnDefaultProperty("tileheight")))
+
     def output_str(self, pngtextnum:int = -1, tilenum:int = -1, output_rectangle:frame.Rectangle = frame.Rectangle(frame.Coordinate(), frame.Coordinate(-1, -1)), objectnum:int = -1)->str:
         str_ans = ""
         str_ans = str_ans + self._properties.output_str() + "\n"
         str_ans = str_ans + "\n".join([tileset.output_str(pngtextnum, tilenum) for tileset in self._tileset_list if tileset.isexist()]) + "\n"
         str_ans = str_ans + "\n".join([layer.output_str(output_rectangle) for layer in self._layer_list]) + "\n"
         str_ans = str_ans + "\n".join([tobject.output_str(objectnum) for tobject in self._objectGroup_list]) + "\n"
         str_ans = utility.indentstr_Tab(str_ans)
@@ -76,14 +86,22 @@
         if objectGroup_now == None:
             raise KeyError("objectGroup name:" + objectGroup_name + " not found")
         objectGroup_now.addObject(default_properties, optional_properties, other_properties)
         if default_properties.get("id") == None:
             default_properties["id"] = self._properties.returnDefaultProperty("nextobjectid")
         str_nextobjectid = str(max(int(self._properties.returnDefaultProperty("nextobjectid")), int(default_properties["id"]) + 1))
         self._properties.assignDefaultProperty("nextobjectid", str_nextobjectid)
+    
+    def addObject_one(self, tobject:object.TObject_One, offset:frame.Coordinate = frame.Coordinate()):
+        ntobject = tobject.offset(offset)
+        self.addObject("Triggers", ntobject.default_properties(), ntobject.optional_properties(), ntobject.other_properties())
+
+    def addObject_group(self, tobject_group:object.TObject_Group, offset:frame.Coordinate = frame.Coordinate()):
+        for tobject in tobject_group._TObject_One_list:
+            self.addObject_one(tobject, offset)
 
     def iterator_object(self, objectGroup_name:str, default_re:dict[str, str] = {}, optional_re:dict[str, str] = {})->Generator[case.TObject, None, None]:
         objectGroup_now:case.ObjectGroup = utility.get_ElementOri_from_list_by_name(self._objectGroup_list, objectGroup_name)
         if objectGroup_now == None:
             raise KeyError("objectGroup name:" + objectGroup_name + " not found")
         for tobject in objectGroup_now._object_list:
             tobject_sas:bool = True
@@ -99,30 +117,14 @@
                     if tobject.returnOptionalProperty(dname) == None or re.match(dvalue, tobject.returnOptionalProperty(dname)) == None:
                         tobject_sas = False
                         break
             if tobject_sas == False:
                 continue
             yield tobject
 
-    def changeObject_defaultProperty(self, objectGroup_name:str, ID:int, name:str, value:str):
-        objectGroup_now:case.ObjectGroup = utility.get_ElementOri_from_list_by_name(self._objectGroup_list, objectGroup_name)
-        if objectGroup_now == None:
-            raise KeyError("objectGroup name:" + objectGroup_name + " not found")
-        for tobject in objectGroup_now._object_list:
-            if tobject.returnDefaultProperty("id") == str(ID):
-                tobject.assignDefaultProperty(name, value)
-
-    def changeObject_optionalProperty(self, objectGroup_name:str, ID:int, name:str, value:str):
-        objectGroup_now:case.ObjectGroup = utility.get_ElementOri_from_list_by_name(self._objectGroup_list, objectGroup_name)
-        if objectGroup_now == None:
-            raise KeyError("objectGroup name:" + objectGroup_name + " not found")
-        for tobject in objectGroup_now._object_list:
-            if tobject.returnDefaultProperty("id") == str(ID):
-                tobject.assignOptionalProperty(name, value)
-
     def addTile_place(self, layerplace:frame.TagCoordinate, tileplace:frame.TagCoordinate):
         layer:case.Layer = utility.get_ElementOri_from_list_by_name(self._layer_list, layerplace.tag())
         if layer == None:
             raise KeyError("layer name:" + layerplace.tag() + " not found")
         for tileset_now in self._tileset_list:
             if tileset_now.output_name() == tileplace.tag():
                 tileset = tileset_now
@@ -147,14 +149,17 @@
         for tilegroup in tilegroup_list:
             self.addTile_group(original_grid, tilegroup)
 
     def addTile_square(self, layer_name:str, place_rectangle:frame.Rectangle, tileset_name:str, tile_grid:frame.Coordinate)->None:
         for place_grid in place_rectangle:
             self.addTile(layer_name, place_grid, tileset_name, tile_grid)
 
+    def add_OTGroup(self, otgroup:otgroup.OTGroup, offset_grid:frame.Coordinate = frame.Coordinate(), ):
+        self.addTile_group_list(offset_grid, otgroup._tilegroup_list)
+        self.addObject_group(otgroup._tobject_group, offset_grid * self.tile_size())
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_coordinate.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,27 @@
             new_content = other._content * self._content
         elif isinstance(other, np.matrix) or (isinstance(other, np.ndarray) and other.ndim == 2):
             new_content = other @ self._content
         else:
             new_content = other * self._content
         ans._content = new_content
         return ans
-
+    
+    def __truediv__(self, other):
+        ans = Coordinate(0, 0)
+        if isinstance(other, Coordinate):
+            new_content = self._content / other._content
+        else:
+            new_content = self._content / other
+        ans._content = new_content
+        return ans
+    
+    def __floordiv__(self, other):
+        return self.__truediv__(other)
+    
     def __sub__(self, other):
         if isinstance(other, Coordinate):
             return Coordinate(self.x() - other.x(), self.y() - other.y())
         else:
             return Coordinate(self.x() - other, self.y() - other)
 
     def __neg__(self):
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_frame/_element_property.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_tile/_tile_group.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_tile/_tile_group.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_util/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 
 from rwmap._util._dict_util import dict_isconflict
 
 from rwmap._util._class_rel import get_ElementOri_from_list_by_name
 
 from rwmap._util._png_rel import image_width, image_height
 
-from rwmap._util._list_util import fill_list_of_list
+from rwmap._util._list_util import fill_list_of_list
+
+from rwmap._util._add_dict import add_str_pro, add_time_pro, add_acti_pro
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.3.0/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/bridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/bridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/decoration.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/decoration.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/deepwater.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/deepwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2dirt_ridge_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dirt_details.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dirt_details.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/dust.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/dust.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/fauna.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/fauna_dark.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/fauna_highland.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/fauna_highland.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2ice_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_broken.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/ice2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/lava2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/lava2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2shortgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longgrass2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/longrass2darkgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/misc.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/misc.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2highland_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2nothing_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/mountain2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2dust_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/nothing2road_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2road_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/nothing2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2_old.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2_old.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2darksand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2darksand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2ice_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2ice_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2lava_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2lava_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2mountain_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2nothing_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2sand_hill.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2stone_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2stone_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sand_dark.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sand_dark.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shallowwater2water_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/shortgrass.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/shortgrass.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2snow_hill.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_hill.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/snow2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/sone2sand_flat_2.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2dirt_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2dirt_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2ice_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2lava.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2lava.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2lava_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2longgrass_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2longgrass_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2mountain_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2sand_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2sand_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2sand_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2shallowwater_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2snow.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2snow_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2snow_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/stone2stone_ridge.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/units.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/units.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/water.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/water.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/bitmaps/water2deepwater_flat.png`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/misc.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/misc.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass LongGrass - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/LongGrass ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Nothing - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain ShallowWater - Flat.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Mountain Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Sand Sand - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Lava - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Lava - ridge2.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/ridges/Stone Stone - Ridge.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/terrain/Lava.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/terrain/Lava.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmap/other_data/maps/units.tsx` & `rwmapeditor_exgcdwu-1.3.0/rwmap/other_data/maps/units.tsx`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.2.8
+Version: 1.3.0
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -675,15 +675,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Requires-Python: >=3.5.0
+Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.26.4
 
 # rwmapeditor-exgcdwu
 
 ___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
@@ -735,35 +735,48 @@
 map_name_out = '[p2]example_skirmish_(2p)(1).tmx'#输出地图
 
 mygraph:rw.RWmap = rw.RWmap.init_mapfile(map_dir + map_name)#地图载入
 print(mygraph)#地图输出【部分】
 
 mygraph.addObject(
     "Triggers", 
-    {"name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1000", "width": "20", "height": "20", "visible": "0"}, 
+    {"name": "刷兵实验", "type": "unitAdd", "x": "1500", "y":"1100", "width": "20", "height": "20", "visible": "0"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 #添加宾语：第一项图层名称（Triggers），第二项默认属性，第三项可选属性
 #默认属性可添加id也可不添加，没有id项会自动添加
 
 mygraph.addObject(
     "Triggers", 
     {"name": "刷兵实验", "type": "unitAdd", "x": "1000", "y":"1500", "width": "20", "height": "20"}, 
     {"resetActivationAfter":"5s", "spawnUnits": "heavyTank*10", "team" :"0", "warmup":"5s"})
 
-for tobject in mygraph.iterator_object("Triggers", {"y": "1500"}):#返回属性成功匹配正则表达式的宾语
+for tobject in mygraph.iterator_object("Triggers", {"y": "1500"}):#返回属性成功匹配正则表达式的宾语（生成器）
     del tobject#宾语被删除
 
-for tobject in mygraph.iterator_object("Triggers", {"y": "1000"}):
+for tobject in mygraph.iterator_object("Triggers", {"y": "1100"}):
     tobject.assignDefaultProperty("name", "名字改变了")#宾语默认属性被赋值
     tobject.assignOptionalProperty("team", "1")#宾语可选属性被赋值
     print(tobject.returnDefaultProperty("name"))#输出宾语默认属性
     print(tobject.returnOptionalProperty("team"))#输出宾语可选属性
     tobject.deleteDefaultProperty("visible")#删除宾语默认属性
     tobject.deleteOptionalProperty("resetActivationAfter")#删除宾语可选属性
 
+mygraph.addObject_group(rw.data.RefreshBuilding.init_building(rw.Coordinate(1500, 1000), rw.Coordinate(40, 40), 
+                                               "turret", "acti_tu1", 10, 10,
+                                               name_add = "城市添加", name_detect = "城市检测", 
+                                               warmup_add = 10, warmup_detect = 5))
+#建立一个可自动刷新的建筑
+
+mygraph.addObject_group(rw.data.City.init_city(rw.Coordinate(1500, 1500), rw.Coordinate(40, 40), 
+                                               "turret", "acti_tu2", 10, 10, "城市", textColor = "white", 
+                                               textSize = 50, name_add = "城市添加", name_detect = "城市检测", 
+                                               name_maptext = "城市文本", warmup_add = 10, warmup_detect = 5))
+#建立一个自动刷新的城市，有名字
+
+
 mygraph.addTile("Ground", rw.Coordinate(1, 0), "Long Grass", rw.Coordinate(0, 0))
 mygraph.addTile("Ground", rw.Coordinate(2, 0), "Long Grass", rw.Coordinate(1, 2))
 mygraph.addTile("Ground", rw.Coordinate(0, 1), "Long Grass", rw.Coordinate(0, 0))
 #改变地块类型：第一项地块层名称，第二项地块层改变位置，第三项地块集名称（全名），第四项所用地块位置（在地块集中）
 
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(5, 5), rw.Coordinate(10, 10)), "Deep Water", rw.Coordinate(0, 0))
 mygraph.addTile_square("Ground", rw.Rectangle(rw.Coordinate(20, 5), rw.Coordinate(30, 10)), "Long Grass", rw.Coordinate(2, 1))
@@ -793,11 +806,7 @@
 ```
 
 ## 其他
 
 ### 外部文件
 
 本库使用了铁锈战争的默认地块集，存放在rwmap/other_data/maps/
-
-### 第三方库依赖
-
-numpy
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.3.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,34 +11,44 @@
 rwmap/_case/_objectgroup.py
 rwmap/_case/_tileset.py
 rwmap/_frame/__init__.py
 rwmap/_frame/_coordinate.py
 rwmap/_frame/_element_ori.py
 rwmap/_frame/_element_property.py
 rwmap/_object/__init__.py
+rwmap/_object/_object_global.py
 rwmap/_object/_object_group.py
-rwmap/_object/_object_one.py
+rwmap/_object/_object_one_and_acti.py
 rwmap/_object/_object_pos.py
-rwmap/_object/_object_pro.py
+rwmap/_object/_object_time.py
+rwmap/_object/_object_type.py
+rwmap/_otgroup/__init__.py
+rwmap/_otgroup/_object_tile_group.py
 rwmap/_tile/__init__.py
 rwmap/_tile/_tile_group.py
 rwmap/_util/__init__.py
+rwmap/_util/_add_dict.py
 rwmap/_util/_class_rel.py
 rwmap/_util/_dict_util.py
 rwmap/_util/_etElement_process.py
 rwmap/_util/_list_util.py
 rwmap/_util/_png_rel.py
 rwmap/_util/_str_util.py
 rwmap/data/__init__.py
-rwmap/data/default_data.py
+rwmap/data/const.py
+rwmap/data/otgroup_grid/__init__.py
 rwmap/data/tile_group_grid/__init__.py
 rwmap/data/tile_group_grid/_tile_group_addlayer.py
 rwmap/data/tile_group_grid/_tile_group_matrix.py
-rwmap/data/tile_group_grid/tile_group_one.py
-rwmap/data/tobject_group_COP/__init__.py
+rwmap/data/tile_group_grid/_tile_group_one.py
+rwmap/data/tobject/__init__.py
+rwmap/data/tobject/_tobject_one.py
+rwmap/data/tobject_group/__init__.py
+rwmap/data/tobject_group/_city.py
+rwmap/data/tobject_group/_refresh_building.py
 rwmap/other_data/requirements.txt
 rwmap/other_data/maps/decoration.tsx
 rwmap/other_data/maps/misc.tsx
 rwmap/other_data/maps/units.tsx
 rwmap/other_data/maps/bitmaps/bridge.png
 rwmap/other_data/maps/bitmaps/decoration.png
 rwmap/other_data/maps/bitmaps/deepwater.png
```

### Comparing `rwmapeditor_exgcdwu-1.2.8/setup.py` & `rwmapeditor_exgcdwu-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 import os
 from setuptools import setup, find_packages
 
-__version__ = '1.2.8'
+__version__ = '1.3.0'
 
 def read_file(file:str):
     with open(file) as file:
         return file.read()
 
 def readline_file(file:str):
     with open(file) as file:
@@ -23,10 +23,10 @@
     license = read_file('LICENSE'),
     url = "https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-",
     long_description = read_file('README.md'),
     long_description_content_type = "text/markdown",
     packages = find_packages(exclude=["tests"]),
     package_data={'rwmap': ['other_data/*.txt', DATA_PREFIX_MAPS + '*.tsx', DATA_PREFIX_MAPS + 'bitmaps/*.png',
                              DATA_PREFIX_MAPS + 'ridges/*.tsx', DATA_PREFIX_MAPS + 'terrain/*.tsx']},
-    python_requires = '>=3.5.0',
+    python_requires = '>=3.6.0',
     install_requires = readline_file("./rwmap/other_data/requirements.txt")
 )
```

