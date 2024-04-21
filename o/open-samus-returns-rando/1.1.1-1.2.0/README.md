# Comparing `tmp/open_samus_returns_rando-1.1.1.tar.gz` & `tmp/open_samus_returns_rando-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_samus_returns_rando-1.1.1.tar", last modified: Tue Apr 16 15:21:38 2024, max compression
+gzip compressed data, was "open_samus_returns_rando-1.2.0.tar", last modified: Sun Apr 21 14:15:38 2024, max compression
```

## Comparing `open_samus_returns_rando-1.1.1.tar` & `open_samus_returns_rando-1.2.0.tar`

### file list

```diff
@@ -1,134 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.944699 open_samus_returns_rando-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.928698 open_samus_returns_rando-1.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.928698 open_samus_returns_rando-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-16 15:21:38.944699 open_samus_returns_rando-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:21:38.944699 open_samus_returns_rando-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.924698 open_samus_returns_rando-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.928698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.928698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.932699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.932699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/doors.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/heatzone.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/room_names.lua
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/savestation.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/scenario.lua
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/ship.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.936699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s000_surface.lua
--rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s010_area1.lua
--rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s020_area2.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s025_area2b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s028_area2c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s030_area3.lua
--rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s033_area3b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s036_area3c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s040_area4.lua
--rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s050_area5.lua
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s060_area6.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s065_area6b.lua
--rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s067_area6c.lua
--rw-r--r--   0 runner    (1001) docker     (127)    41935 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s070_area7.lua
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s090_area9.lua
--rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s100_area10.lua
--rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.936699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.924698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.924698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.924698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.924698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.936699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.936699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.924698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.924698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.924698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.936699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
--rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
--rw-r--r--   0 runner    (1001) docker     (127)    22095 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.940698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/cosmetics.lua
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/metroid_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/lua_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.940698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/credits.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/exefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/spawn_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.940698 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/pickups/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/pickups/custom_pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/pickups/model_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/pickups/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/samus_returns_patcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.944699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/door_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/hint_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/metroid_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/static_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/tunable_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 15:21:38.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.944699 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-16 15:21:38.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-16 15:21:38.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:21:38.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 15:21:38.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 15:21:38.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 15:21:38.000000 open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.944699 open_samus_returns_rando-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:21:38.944699 open_samus_returns_rando-1.1.1/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/tests/test_files/item_models_test.json
--rw-r--r--   0 runner    (1001) docker     (127)   146805 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-16 15:21:29.000000 open_samus_returns_rando-1.1.1/tests/test_lua_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.515809 open_samus_returns_rando-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.515809 open_samus_returns_rando-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.519809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.519809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/__pyinstaller/hook-open_samus_returns_rando.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.519809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.519809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/doors.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/heatzone.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/savestation.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/scenario.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/ship.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/sprites_splashes.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.523809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (127)    26259 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s000_surface.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    31259 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s010_area1.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    29548 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s020_area2.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s025_area2b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s028_area2c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    27509 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s030_area3.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    40894 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s033_area3b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23245 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s036_area3c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    30051 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s040_area4.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    34925 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s050_area5.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s060_area6.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s065_area6b.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s067_area6c.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    41935 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s070_area7.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s090_area9.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    39148 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s100_area10.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    26016 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerbabyhatchling.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerenergyshield.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerenergywave.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerphasedisplacement.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetankm.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerscanningpulse.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersuit.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.511809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)    43927 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.515809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.527809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/gui/textures/
+-rw-r--r--   0 runner    (1001) docker     (127)   524553 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex
+-rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.531809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/chozoseal_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/cosmetics.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/elevators.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/metroid_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15823 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/lua_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.531809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/collision_camera_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/elevators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/exefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/spawn_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.531809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/custom_pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/samus_returns_patcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.531809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20266 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/door_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9260 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/heat_room_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/hint_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12026 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/metroid_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/static_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/tunable_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-21 14:15:38.000000 open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:15:38.535809 open_samus_returns_rando-1.2.0/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/tests/test_files/item_models_test.json
+-rw-r--r--   0 runner    (1001) docker     (127)   147194 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-21 14:15:28.000000 open_samus_returns_rando-1.2.0/tests/test_lua_util.py
```

### Comparing `open_samus_returns_rando-1.1.1/.github/dependabot.yml` & `open_samus_returns_rando-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/.github/workflows/python.yml` & `open_samus_returns_rando-1.2.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/.gitignore` & `open_samus_returns_rando-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/LICENSE` & `open_samus_returns_rando-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/PKG-INFO` & `open_samus_returns_rando-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.1.1
+Version: 1.2.0
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `open_samus_returns_rando-1.1.1/README.md` & `open_samus_returns_rando-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/pyproject.toml` & `open_samus_returns_rando-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/cli.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/constants.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/constants.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/debug.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/debug.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/doors.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/doors.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/guilib.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/guilib.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/heatzone.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/heatzone.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/room_names.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/room_names.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/savestation.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/savestation.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/scenario.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/scenario.lua`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Game.ImportLibrary("system/scripts/scenario_original.lua")
 Game.ImportLibrary("system/scripts/guilib.lua", false)
 Game.ImportLibrary("system/scripts/cosmetics.lua", false)
 
 Game.DoFile("system/scripts/room_names.lua")
+Game.DoFile("system/scripts/elevators.lua")
 
 Scenario = Scenario or {}
 setmetatable(Scenario, {__index = _G})
 
 Scenario.tProgressiveModels = {}
 
 local original_enable =  Scenario.EnableHazarous
@@ -138,8 +139,14 @@
   fatal_messages_seen = 0
   fatal_messages = messageBoxes
   Game.AddSF(0.8, Scenario._ShowNextFatalErrorMessage, "")
 end
 
 function Scenario.UpdateRoomName(new_subarea)
   Game.AddSF(0.0, "RoomNameGui.Update", "s", new_subarea)
+end
+
+function Scenario.RandoOnElevatorUse(from_actor, _ARG_1_, _ARG_2_)
+  local destination = ElevatorDestinations[Scenario.CurrentScenarioID][from_actor.sName]
+  Game.AddGUISF(0.5, GUI.ElevatorStartUseActionStep2InterArea, "")
+  Elevator.Use("c10_samus", destination.scenario, destination.actor, _ARG_2_)
 end
```

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/custom/ship.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/custom/ship.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s000_surface.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s000_surface.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s010_area1.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s010_area1.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s020_area2.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s020_area2.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s025_area2b.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s025_area2b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s028_area2c.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s028_area2c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s030_area3.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s030_area3.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s033_area3b.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s033_area3b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s036_area3c.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s036_area3c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s040_area4.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s040_area4.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s050_area5.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s050_area5.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s060_area6.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s060_area6.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s065_area6b.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s065_area6b.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s067_area6c.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s067_area6c.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s070_area7.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s070_area7.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s090_area9.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s090_area9.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s100_area10.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s100_area10.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/levels/s110_surfaceb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerenergytank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizermissilelauncher.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbomb.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerpowerbombtank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanka.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizerreservetanke.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizersuit.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersuit.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/schema.json` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973529411764706%*

 * *Differences: {"'properties'": "{'elevators': {'type': 'object', 'description': 'A dictionary of dictionaries "*

 * *                 "mapping scenario and elevator actor to a connecting elevator', "*

 * *                 "'patternProperties': OrderedDict([('.*', OrderedDict([('type', 'object'), "*

 * *                 "('additionalProperties', False), ('default', OrderedDict()), "*

 * *                 "('patternProperties', OrderedDict([('.*', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('scenario', Or […]*

```diff
@@ -364,30 +364,41 @@
                     "door_type"
                 ],
                 "type": "object"
             },
             "type": "array"
         },
         "elevators": {
-            "items": {
-                "properties": {
-                    "destination": {
-                        "$ref": "#/$defs/actor_reference"
+            "default": {},
+            "description": "A dictionary of dictionaries mapping scenario and elevator actor to a connecting elevator",
+            "patternProperties": {
+                ".*": {
+                    "additionalProperties": false,
+                    "default": {},
+                    "patternProperties": {
+                        ".*": {
+                            "properties": {
+                                "actor": {
+                                    "type": "string"
+                                },
+                                "scenario": {
+                                    "$ref": "#/$defs/scenario_name"
+                                }
+                            },
+                            "required": [
+                                "scenario",
+                                "actor"
+                            ],
+                            "type": "object"
+                        }
                     },
-                    "teleporter": {
-                        "$ref": "#/$defs/actor_reference_with_layer"
-                    }
-                },
-                "required": [
-                    "teleporter",
-                    "destination"
-                ],
-                "type": "object"
+                    "type": "object"
+                }
             },
-            "type": "array"
+            "type": "object"
         },
         "energy_per_tank": {
             "default": 100.0,
             "description": "How much energy collecting an Energy Tank gives",
             "type": "number"
         },
         "game_patches": {
```

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/chozoseal_template.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/chozoseal_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/cosmetics.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/cosmetics.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/custom_init.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/custom_init.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/metroid_template.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/metroid_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/randomizer_item_template.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/randomizerpowerup.lua`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/lua_editor.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/lua_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,14 +274,15 @@
         scenario_lua_content = files_path().joinpath("custom/scenario.lua").read_text()
         scenario_lua_content += "\n" + self._progressive_models
         lua_util.replace_script_with_content(editor, "system/scripts/scenario", scenario_lua_content)
 
         lua_util.replace_script(editor, "actors/props/samusship/scripts/samusship", "custom/ship.lua")
         lua_util.replace_script(editor, "actors/props/savestation/scripts/savestation", "custom/savestation.lua")
         lua_util.replace_script(editor, "actors/props/heatzone/scripts/heatzone", "custom/heatzone.lua")
+        lua_util.replace_script(editor, "gui/scripts/sprites_splashes", "custom/sprites_splashes.lua")
 
     def save_modifications(self, editor: PatcherEditor, configuration: dict):
         self._add_replacement_files(editor, configuration)
 
         # add new system scripts
         editor.add_new_asset(
             "system/scripts/guilib.lc",
```

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/collision_camera_table.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/collision_camera_table.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/credits.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/credits.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/lua_util.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/lua_util.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/spawn_points.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/spawn_points.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/misc_patches/text_patches.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/misc_patches/text_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/patch_util.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/patcher_editor.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/pickups/custom_pickups.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/custom_pickups.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/pickups/model_data.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/model_data.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/pickups/pickup.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/pickups/pickup.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/samus_returns_patcher.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/samus_returns_patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from open_samus_returns_rando.debug import debug_custom_pickups, debug_spawn_points
 from open_samus_returns_rando.files import files_path
 from open_samus_returns_rando.logger import LOG
 from open_samus_returns_rando.lua_editor import LuaEditor
 from open_samus_returns_rando.misc_patches.collision_camera_table import create_collision_camera_table
 from open_samus_returns_rando.misc_patches.credits import patch_credits
+from open_samus_returns_rando.misc_patches.elevators import patch_elevators
 from open_samus_returns_rando.misc_patches.exefs import DSPatch
 from open_samus_returns_rando.misc_patches.spawn_points import patch_custom_spawn_points
 from open_samus_returns_rando.misc_patches.text_patches import add_spiderboost_status, apply_text_patches
 from open_samus_returns_rando.patcher_editor import PatcherEditor
 from open_samus_returns_rando.pickups.custom_pickups import patch_custom_pickups
 from open_samus_returns_rando.pickups.pickup import patch_pickups
 from open_samus_returns_rando.specific_patches import cosmetic_patches, game_patches, tunable_patches
@@ -112,14 +113,17 @@
         apply_text_patches(editor, configuration["text_patches"])
     patch_credits(editor, configuration["spoiler_log"])
     add_spiderboost_status(editor)
 
      # Update cc_to_room_name.lua
     create_collision_camera_table(editor, configuration)
 
+    # Patch elevator destinations
+    patch_elevators(editor, configuration)
+
     out_romfs = output_path.joinpath("romfs")
     out_exefs = output_path.joinpath("exefs")
     shutil.rmtree(out_romfs, ignore_errors=True)
     shutil.rmtree(out_exefs, ignore_errors=True)
 
     # Create Exefs patches (currently there are none)
     LOG.info("Creating exefs patches")
```

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/chozo_seal_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/door_patches.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/door_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/game_patches.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/game_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/heat_room_patches.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/heat_room_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/map_icons.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/map_icons.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/metroid_patches.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/metroid_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/static_fixes.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/static_fixes.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/specific_patches/tunable_patches.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/specific_patches/tunable_patches.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando/validator_with_default.py` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/PKG-INFO` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open_samus_returns_rando
-Version: 1.1.1
+Version: 1.2.0
 Summary: An open source randomizer patcher for Metroid: Samus Returns.
 Project-URL: Homepage, https://github.com/randovania/open-samus-returns-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `open_samus_returns_rando-1.1.1/src/open_samus_returns_rando.egg-info/SOURCES.txt` & `open_samus_returns_rando-1.2.0/src/open_samus_returns_rando.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/open_samus_returns_rando/files/custom/doors.lua
 src/open_samus_returns_rando/files/custom/guilib.lua
 src/open_samus_returns_rando/files/custom/heatzone.lua
 src/open_samus_returns_rando/files/custom/room_names.lua
 src/open_samus_returns_rando/files/custom/savestation.lua
 src/open_samus_returns_rando/files/custom/scenario.lua
 src/open_samus_returns_rando/files/custom/ship.lua
+src/open_samus_returns_rando/files/custom/sprites_splashes.lua
 src/open_samus_returns_rando/files/levels/s000_surface.lua
 src/open_samus_returns_rando/files/levels/s010_area1.lua
 src/open_samus_returns_rando/files/levels/s020_area2.lua
 src/open_samus_returns_rando/files/levels/s025_area2b.lua
 src/open_samus_returns_rando/files/levels/s028_area2c.lua
 src/open_samus_returns_rando/files/levels/s030_area3.lua
 src/open_samus_returns_rando/files/levels/s033_area3b.lua
@@ -68,25 +69,28 @@
 src/open_samus_returns_rando/files/pickups/randomizersuit.lua
 src/open_samus_returns_rando/files/pickups/randomizersupermissile.lua
 src/open_samus_returns_rando/files/pickups/randomizersupermissiletank.lua
 src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/powerup_missilelauncher.bcmdl
 src/open_samus_returns_rando/files/romfs/actors/items/powerup_missilelauncher/models/textures/missile_e.bctex
 src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/chozodnareceivergold_d.bctex
 src/open_samus_returns_rando/files/romfs/actors/props/chozoseal/models/textures/dna_d.bctex
+src/open_samus_returns_rando/files/romfs/gui/textures/gamelogo.bctex
 src/open_samus_returns_rando/files/templates/cc_to_room_name.lua
 src/open_samus_returns_rando/files/templates/chozoseal_template.lua
 src/open_samus_returns_rando/files/templates/cosmetics.lua
 src/open_samus_returns_rando/files/templates/custom_init.lua
+src/open_samus_returns_rando/files/templates/elevators.lua
 src/open_samus_returns_rando/files/templates/metroid_template.lua
 src/open_samus_returns_rando/files/templates/progressive_model_template.lua
 src/open_samus_returns_rando/files/templates/randomizer_item_template.lua
 src/open_samus_returns_rando/files/templates/randomizerpowerup.lua
 src/open_samus_returns_rando/files/templates/template_powerup_bmsad.json
 src/open_samus_returns_rando/misc_patches/collision_camera_table.py
 src/open_samus_returns_rando/misc_patches/credits.py
+src/open_samus_returns_rando/misc_patches/elevators.py
 src/open_samus_returns_rando/misc_patches/exefs.py
 src/open_samus_returns_rando/misc_patches/lua_util.py
 src/open_samus_returns_rando/misc_patches/spawn_points.py
 src/open_samus_returns_rando/misc_patches/text_patches.py
 src/open_samus_returns_rando/pickups/custom_pickups.py
 src/open_samus_returns_rando/pickups/model_data.py
 src/open_samus_returns_rando/pickups/pickup.py
```

### Comparing `open_samus_returns_rando-1.1.1/tests/test_files/item_models_test.json` & `open_samus_returns_rando-1.2.0/tests/test_files/item_models_test.json`

 * *Files identical despite different names*

### Comparing `open_samus_returns_rando-1.1.1/tests/test_files/starter_preset_patcher.json` & `open_samus_returns_rando-1.2.0/tests/test_files/starter_preset_patcher.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'elevators'": "OrderedDict([('s010_area1', OrderedDict([('LE_Platform_Elevator_FromArea02', "*

 * *                "OrderedDict([('scenario', 's028_area2c'), ('actor', 'ST_FromArea01')]))])), "*

 * *                "('s028_area2c', OrderedDict([('LE_Platform_Elevator_FromArea01', "*

 * *                "OrderedDict([('scenario', 's010_area1'), ('actor', 'ST_FromArea02')]))]))])"}*

```diff
@@ -352,14 +352,28 @@
         ],
         "laser_unlocked_color": [
             1.0,
             0.4980392156862745,
             0.0
         ]
     },
+    "elevators": {
+        "s010_area1": {
+            "LE_Platform_Elevator_FromArea02": {
+                "actor": "ST_FromArea01",
+                "scenario": "s028_area2c"
+            }
+        },
+        "s028_area2c": {
+            "LE_Platform_Elevator_FromArea01": {
+                "actor": "ST_FromArea02",
+                "scenario": "s010_area1"
+            }
+        }
+    },
     "energy_per_tank": 100,
     "game_patches": {
         "beam_burst_buff": true,
         "beam_door_buff": true,
         "charge_door_buff": true,
         "nerf_super_missiles": false,
         "patch_area1_crumbles": true,
```

