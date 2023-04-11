# Comparing `tmp/open-dread-rando-1.8.0.tar.gz` & `tmp/open-dread-rando-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-dread-rando-1.8.0.tar", last modified: Thu Apr  6 08:59:24 2023, max compression
+gzip compressed data, was "open-dread-rando-1.9.0.tar", last modified: Tue Apr 11 10:22:36 2023, max compression
```

## Comparing `open-dread-rando-1.8.0.tar` & `open-dread-rando-1.9.0.tar`

### file list

```diff
@@ -1,187 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.495356 open-dread-rando-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.471356 open-dread-rando-1.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.471356 open-dread-rando-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/.github/workflows/patch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.471356 open-dread-rando-1.8.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-06 08:59:24.495356 open-dread-rando-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.475356 open-dread-rando-1.8.0/open_dread_rando/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.475356 open-dread-rando-1.8.0/open_dread_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/common_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/cosmetic_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/custom_door_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/door_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/dread_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/elevator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/environmental_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/environmental_damage_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/exefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.479356 open-dread-rando-1.8.0/open_dread_rando/files/
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/custom_scenario.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.479356 open-dread-rando-1.8.0/open_dread_rando/files/dread_depackager/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/dread_depackager/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/dread_depackager/main.npdm
--rw-r--r--   0 runner    (1001) docker     (123)   179102 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/dread_depackager/subsdk9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.479356 open-dread-rando-1.8.0/open_dread_rando/files/exefs_patches/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/exefs_patches/debug_input.s
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.479356 open-dread-rando-1.8.0/open_dread_rando/files/levels/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)    67727 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s010_cave.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    38110 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s020_magma.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    23654 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s030_baselab.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    32324 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s040_aqua.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    25415 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s050_forest.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s060_quarantine.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    30609 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s070_basesanc.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)    16577 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s080_shipyard.lc.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/levels/s090_skybase.lc.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.483357 open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/bit.lua
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/data_structures.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/death_counter.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/guilib.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/input_handling.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/randomizer_powerup.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.459356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.459356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.455356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.455356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube/model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.483357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.455356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.483357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
--rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.455356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.483357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.483357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.455356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.483357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.483357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.459356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.483357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.459356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.459356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.459356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.459356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)   140588 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.487357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat
--rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.467357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.467357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.491356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.491356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.491356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.463356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.467357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.491356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.467357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.467357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.491356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
--rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.467357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/system/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.467357 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/system/minimap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.491356 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/system/minimap/icons/
--rw-r--r--   0 runner    (1001) docker     (123)   414489 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
--rw-r--r--   0 runner    (1001) docker     (123)    24889 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/files/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/game_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/lua_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/map_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/model_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/output_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/patch_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/patcher_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/pickup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13486 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/static_fixes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.495356 open-dread-rando-1.8.0/open_dread_rando/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/boss_powerup_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/custom_core_x.lua
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/custom_init.lua
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/progressive_model_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/randomizer_progressive_template.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/template_doorshield_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/template_powerup_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/templates/template_shieldenergy_bmsad.json
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/text_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/tilegroup_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/open_dread_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 08:59:24.000000 open-dread-rando-1.8.0/open_dread_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.475356 open-dread-rando-1.8.0/open_dread_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-06 08:59:24.000000 open-dread-rando-1.8.0/open_dread_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-06 08:59:24.000000 open-dread-rando-1.8.0/open_dread_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:59:24.000000 open-dread-rando-1.8.0/open_dread_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-06 08:59:24.000000 open-dread-rando-1.8.0/open_dread_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:59:15.000000 open-dread-rando-1.8.0/open_dread_rando.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-06 08:59:24.000000 open-dread-rando-1.8.0/open_dread_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-06 08:59:24.000000 open-dread-rando-1.8.0/open_dread_rando.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-06 08:59:24.495356 open-dread-rando-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.495356 open-dread-rando-1.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:59:24.495356 open-dread-rando-1.8.0/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)   122329 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/tests/test_files/starter_preset_patcher.json
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/tests/test_lua_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-06 08:59:05.000000 open-dread-rando-1.8.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.187322 open-dread-rando-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/.github/workflows/patch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-11 10:22:36.187322 open-dread-rando-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.175322 open-dread-rando-1.9.0/open_dread_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.175322 open-dread-rando-1.9.0/open_dread_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/__pyinstaller/hook-open_dread_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/cosmetic_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/custom_door_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/door_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10528 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/dread_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/elevator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/environmental_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/environmental_damage_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/exefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.175322 open-dread-rando-1.9.0/open_dread_rando/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/custom_scenario.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.179322 open-dread-rando-1.9.0/open_dread_rando/files/dread_depackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/dread_depackager/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/dread_depackager/main.npdm
+-rw-r--r--   0 runner    (1001) docker     (123)   179102 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/dread_depackager/subsdk9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.179322 open-dread-rando-1.9.0/open_dread_rando/files/exefs_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/exefs_patches/debug_input.s
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.179322 open-dread-rando-1.9.0/open_dread_rando/files/levels/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    67785 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s010_cave.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    38168 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s020_magma.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s030_baselab.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    32382 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s040_aqua.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s050_forest.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s060_quarantine.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    30667 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s070_basesanc.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s080_shipyard.lc.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/levels/s090_skybase.lc.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.179322 open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/bit.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/data_structures.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/death_counter.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/guilib.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/input_handling.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/room_names.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/randomizer_powerup.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube/model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.179322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.179322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
+-rw-r--r--   0 runner    (1001) docker     (123)   422936 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.179322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    19348 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mat0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    28948 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_autoilum.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_bola.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)   140588 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat
+-rw-r--r--   0 runner    (1001) docker     (123)    22156 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    28804 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    19894 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    42001 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.167322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    17196 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    34728 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    75887 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.183322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)    71298 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.187322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/
+-rw-r--r--   0 runner    (1001) docker     (123)   155165 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/system/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.171322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/system/minimap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.187322 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/system/minimap/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   414489 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
+-rw-r--r--   0 runner    (1001) docker     (123)    26436 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/files/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/game_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/lua_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/map_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/model_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/output_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/patch_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/patcher_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/static_fixes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.187322 open-dread-rando-1.9.0/open_dread_rando/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/boss_powerup_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/cc_to_room_name.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/custom_core_x.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/custom_init.lua
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/progressive_model_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/randomizer_progressive_template.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/template_doorshield_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/template_powerup_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/templates/template_shieldenergy_bmsad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/text_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/tilegroup_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/open_dread_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-11 10:22:36.000000 open-dread-rando-1.9.0/open_dread_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.175322 open-dread-rando-1.9.0/open_dread_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-11 10:22:36.000000 open-dread-rando-1.9.0/open_dread_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-11 10:22:36.000000 open-dread-rando-1.9.0/open_dread_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:22:36.000000 open-dread-rando-1.9.0/open_dread_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 10:22:36.000000 open-dread-rando-1.9.0/open_dread_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:22:27.000000 open-dread-rando-1.9.0/open_dread_rando.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 10:22:36.000000 open-dread-rando-1.9.0/open_dread_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 10:22:36.000000 open-dread-rando-1.9.0/open_dread_rando.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-11 10:22:36.187322 open-dread-rando-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.187322 open-dread-rando-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:22:36.187322 open-dread-rando-1.9.0/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)   145212 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/tests/test_files/starter_preset_patcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/tests/test_lua_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 10:22:16.000000 open-dread-rando-1.9.0/tests/test_schema.py
```

### Comparing `open-dread-rando-1.8.0/.github/dependabot.yml` & `open-dread-rando-1.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/.github/workflows/patch.yml` & `open-dread-rando-1.9.0/.github/workflows/patch.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/.github/workflows/python.yml` & `open-dread-rando-1.9.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/.gitignore` & `open-dread-rando-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/LICENSE` & `open-dread-rando-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/PKG-INFO` & `open-dread-rando-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 1.8.0
+Version: 1.9.0
 Summary: An open source randomizer patcher for Metroid Dread.
 Home-page: https://github.com/randovania/open-dread-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `open-dread-rando-1.8.0/README.md` & `open-dread-rando-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/cli.py` & `open-dread-rando-1.9.0/open_dread_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/cosmetic_patches.py` & `open-dread-rando-1.9.0/open_dread_rando/cosmetic_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/custom_door_types.py` & `open-dread-rando-1.9.0/open_dread_rando/custom_door_types.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/door_patcher.py` & `open-dread-rando-1.9.0/open_dread_rando/door_patcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from bisect import insort
 from enum import Enum
 from pathlib import Path
 from typing import Sequence
 
 from construct import Container, ListContainer
 
-from open_dread_rando.common_data import ALL_SCENARIOS
+from open_dread_rando.constants import ALL_SCENARIOS
 from open_dread_rando.patcher_editor import PatcherEditor
 
 from mercury_engine_data_structures.formats import Bmscc
 
 # copied from existing entity, so we don't have to make a whole shield
 _EXAMPLE_SHIELD = {"scenario": "s010_cave", "layer": "default", "actor": "Door003_missileShield"}
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/dread_patcher.py` & `open-dread-rando-1.9.0/open_dread_rando/dread_patcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 
 from construct import ListContainer
 from mercury_engine_data_structures.file_tree_editor import OutputFormat
 
 from open_dread_rando import elevator, lua_util, game_patches
 from open_dread_rando.cosmetic_patches import apply_cosmetic_patches
+from open_dread_rando.constants import FadeTimes
 from open_dread_rando.custom_door_types import create_all_shield_assets
 from open_dread_rando.door_patcher import DoorPatcher
 from open_dread_rando.environmental_damage import apply_constant_damage
 from open_dread_rando.exefs import include_depackager, patch_exefs
 from open_dread_rando.logger import LOG
 from open_dread_rando.lua_editor import LuaEditor
 from open_dread_rando.objective import apply_objective_patches
@@ -86,21 +87,30 @@
         "energy_per_part": energy_per_part,
         "immediate_energy_parts": configuration["immediate_energy_parts"],
         "default_x_released": configuration.get("game_patches", {}).get("default_x_released", False),
         "linear_damage_runs": configuration.get("linear_damage_runs"),
         "linear_dps": configuration.get("linear_dps"),
         "configuration_identifier": lua_util.wrap_string(configuration_identifier),
         "required_artifacts": configuration["objective"]["required_artifacts"],
-        "enable_death_counter": cosmetic_options["enable_death_counter"]
+        "enable_death_counter": cosmetic_options["enable_death_counter"],
+        "enable_room_ids": False if cosmetic_options["enable_room_name_display"] == "NEVER" else True,
+        "room_id_fade_time": FadeTimes.NO_FADE.value if (
+            cosmetic_options["enable_room_name_display"] != "WITH_FADE"
+            ) else FadeTimes.ROOM_FADE.value,
     }
 
     replacement.update(configuration.get("game_patches", {}))
 
     return lua_util.replace_lua_template("custom_init.lua", replacement)
 
+def create_collision_camera_table(editor: PatcherEditor, configuration: dict):
+    py_dict: dict = configuration["cosmetic_patches"]["lua"]["camera_names_dict"]
+    
+    file = lua_util.replace_lua_template("cc_to_room_name.lua", { "room_dict" : py_dict}, True).encode("ascii")
+    editor.add_new_asset("system/scripts/cc_to_room_name.lc", file, ["packs/system/system.pkg"])
 
 def patch_pickups(editor: PatcherEditor, lua_scripts: LuaEditor, pickups_config: list[dict], configuration: dict):
     # add to the TOC
     editor.add_new_asset("actors/items/randomizer_powerup/scripts/randomizer_powerup.lc", b'', [])
 
     for i, pickup in enumerate(pickups_config):
         LOG.debug("Writing pickup %d: %s", i, pickup["resources"][0]["item_id"])
@@ -175,14 +185,17 @@
     # Update init.lc
     lua_util.create_script_copy(editor, "system/scripts/init")
     editor.replace_asset(
         "system/scripts/init.lc",
         create_custom_init(editor, configuration).encode("ascii"),
     )
 
+    # Update cc_to_room_name.lua
+    create_collision_camera_table(editor, configuration)
+
     # Update scenario.lc
     lua_util.replace_script(editor, "system/scripts/scenario", "custom_scenario.lua")
 
     # Elevators
     if "elevators" in configuration:
         elevator.patch_elevators(editor, configuration["elevators"])
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/elevator.py` & `open-dread-rando-1.9.0/open_dread_rando/elevator.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/environmental_damage.py` & `open-dread-rando-1.9.0/open_dread_rando/environmental_damage.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/environmental_damage_sources.py` & `open-dread-rando-1.9.0/open_dread_rando/environmental_damage_sources.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/exefs.py` & `open-dread-rando-1.9.0/open_dread_rando/exefs.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/custom_scenario.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/custom_scenario.lua`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Game.ImportLibrary("system/scripts/scenario_original.lua")
 
 Game.DoFile("system/scripts/input_handling.lua")
 Game.DoFile("system/scripts/data_structures.lua")
 Game.DoFile("system/scripts/guilib.lua")
 Game.DoFile("system/scripts/death_counter.lua")
+Game.DoFile("system/scripts/room_names.lua")
 
 Scenario.tRandoHintPropIDs = {
     CAVE_1 = Blackboard.RegisterLUAProp("HINT_CAVE_1", "bool"),
     CAVE_2 = Blackboard.RegisterLUAProp("HINT_CAVE_2", "bool"),
     MAGMA_1 = Blackboard.RegisterLUAProp("HINT_MAGMA_1", "bool"),
     MAGMA_2 = Blackboard.RegisterLUAProp("HINT_MAGMA_2", "bool"),
     LAB_1 = Blackboard.RegisterLUAProp("HINT_LAB_1", "bool"),
@@ -358,14 +359,19 @@
 
 
 function Scenario.OnTeleportFinished()
     Scenario.EnableInput()
     Game.ReinitPlayerFromBlackboard()
 end
 
+function Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
+    Scenario.UpdateProgressiveItemModels()
+    Scenario.UpdateRoomName(new_subarea)
+end
+
 Scenario.NumUIs = 0
 function Scenario.InitGui()
     Game.LogWarn(0, "Creating GUI")
     Scenario.NumUIs = Scenario.NumUIs +1
     local ui = GUILib("RandoUI"..Scenario.NumUIs)
     ui:AddContainer("Content")
     ui:Get("Content"):AddLabel("Popup", "", {
@@ -380,14 +386,18 @@
     })
     ui:Show()
     Scenario.RandoUI = ui
 
     if Init.bEnableDeathCounter then
         DeathCounter.Init()
     end
+
+    if Init.bEnableRoomIds then
+        RoomNameGui.Init()
+    end
 end
 
 Scenario.QueuedPopups = Scenario.QueuedPopups or Queue()
 Scenario.ShowingPopup = false
 
 function Scenario.QueueAsyncPopup(text, time)
     Scenario.QueuedPopups:push({Text = text, Time = time or 5.0})
@@ -421,7 +431,11 @@
     if not Scenario.QueuedPopups:empty() then
         Scenario.QueuedPopups:pop()
     end
     Scenario.RandoUI:Get("Content"):Get("Popup"):SetProperties({Visible = false})
     Game.AddGUISF(0.5, "Scenario.ShowNextAsyncPopup", "")
     pop_debug_print_override()
 end
+
+function Scenario.UpdateRoomName(new_subarea)
+    RoomNameGui.Update(new_subarea)
+end
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/dread_depackager/main.npdm` & `open-dread-rando-1.9.0/open_dread_rando/files/dread_depackager/main.npdm`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/dread_depackager/subsdk9` & `open-dread-rando-1.9.0/open_dread_rando/files/dread_depackager/subsdk9`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/exefs_patches/debug_input.s` & `open-dread-rando-1.9.0/open_dread_rando/files/exefs_patches/debug_input.s`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s010_cave.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s010_cave.lc.lua`

 * *Files 1% similar despite different names*

```diff
@@ -1211,15 +1211,15 @@
     -- lock CU door except when entering from the CU room if emmi is alive
     local cu_door = Game.GetActor("Door017 (CU)_000")
     if cu_door ~= nil then
       cu_door.LIFE:LockDoor()
     end
   end
 
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
 
 
 s010_cave.tTriggersToEnable = {
   "TG_ChainReaction_Camera_001",
   "TG_ChainReaction_SteamJet_016",
   "TG_ChainReaction_SteamJet_017"
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s020_magma.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s020_magma.lc.lua`

 * *Files 0% similar despite different names*

```diff
@@ -831,15 +831,15 @@
   elseif old_subarea == "collision_camera_063" and new_subarea == "collision_camera_044" then
     Game.PlayCurrentEnvironmentMusic()
   elseif old_subarea == "collision_camera_022" and new_subarea == "collision_camera_030" then
     Game.StopMusic(true)
     Game.PlayCurrentEnvironmentMusic()
   end
 
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
 
 function s020_magma.Kraid_InitCutscene()
   Game.PushSetup("Kraid_Stage_01", true, true)
   local oActor1 = Game.GetActor("cutsceneplayer_59") 
   if oActor1 ~= nil then
     oActor1.CUTSCENE:TryLaunchCutscene()
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s030_baselab.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s030_baselab.lc.lua`

 * *Files 1% similar despite different names*

```diff
@@ -691,15 +691,15 @@
   if wide_door_left ~= nil then
     wide_door_left.LIFE:SetInvulnerable(disable_wide)
   end
   if wide_door_right ~= nil then
     wide_door_right.LIFE:SetInvulnerable(disable_wide)
   end
 
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s040_aqua.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s040_aqua.lc.lua`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 function s040_aqua.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
   if old_subarea == "collision_camera_010" and new_subarea == "collision_camera_014" then
     --s040_aqua.LaunchCutscene_32()
   elseif old_subarea ~= "collision_camera_029" or new_subarea == "collision_camera_028" then     
       
   end
 
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
 
 function s040_aqua.LaunchCutscene_32()
   local oActor = Game.GetActor("cutsceneplayer_32")
   if oActor ~= nil then
     oActor.CUTSCENE:TryLaunchCutscene()
   end
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s050_forest.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s050_forest.lc.lua`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
       if L5_2.SPAWNGROUP.iNumDeaths > 0 then
         Game.PopSetup("ChozoWarriorX", true, true)
         Game.PushSetup("PostChozoWarriorX", false, true)
       end
     end
   end
 
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
 
 function s050_forest.LaunchCutscene_33()
   local oActor = Game.GetActor("cutsceneplayer_33") 
   if oActor ~= nil then
     oActor.CUTSCENE:TryLaunchCutscene()
   end
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s060_quarantine.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s060_quarantine.lc.lua`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
       Game.PushSetup("PostChozoWarriorX", true, true)
       if L5_2 ~= nil then
         L5_2.bEnabled = true
       end
     end
   end
 
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
 
 
 
 
 
 function s060_quarantine.LaunchCutscene_67()
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s070_basesanc.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s070_basesanc.lc.lua`

 * *Files 1% similar despite different names*

```diff
@@ -978,15 +978,15 @@
 
     if L5_2.SPAWNGROUP.iNumDeaths > 1 then
       Game.PopSetup("2ChozoRobots", true, true)
       Game.PushSetup("Post2ChozoRobots", false, true)
     end
   end
 
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s080_shipyard.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s080_shipyard.lc.lua`

 * *Files 1% similar despite different names*

```diff
@@ -468,15 +468,15 @@
     s080_shipyard.OnBegin_Cutscene_12()
   elseif old_subarea == "collision_camera_006" and new_subarea == "collision_camera_005" and SHIP_CWXELITE_PRESENTATION == false then
     s080_shipyard.OnBegin_Cutscene_71()
   elseif old_subarea == "collision_camera_000" and new_subarea == "collision_camera_016" then
     Game.StopMusic(true)
   end
 
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
 
 function s080_shipyard.ClosePowerBombDoor()
   
   local L0_2 = Game.GetActor("doorpowerclosed_001")
   if L0_2 ~= nil and L0_2.LIFE:CanBeClosedSafely() then
     Game.GetActor("doorpowerclosed_001").LIFE:CloseDoor(false, true, false)
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/levels/s090_skybase.lc.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/levels/s090_skybase.lc.lua`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 function s090_skybase.SubAreaChangeRequest(_ARG_0_, _ARG_1_, _ARG_2_, _ARG_3_)
   Scenario.SubAreaChangeRequest(_ARG_0_, _ARG_1_, _ARG_2_, _ARG_3_)
 end
 
 
 function s090_skybase.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
-  Scenario.UpdateProgressiveItemModels()
+  Scenario.OnSubAreaChange(old_subarea, old_actorgroup, new_subarea, new_actorgroup, disable_fade)
 end
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/bit.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/bit.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/data_structures.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/data_structures.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/lua_libraries/input_handling.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/lua_libraries/input_handling.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/randomizer_powerup.lua` & `open-dread-rando-1.9.0/open_dread_rando/files/randomizer_powerup.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphhologram.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/imats/powerup_morphmaterial.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_magnet01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/imats/powerup_doublejump_mp_white__01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_doublejump/models/powerup_magnet.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/imats/powerup_powerbomb_mp_fxhologram_0001.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_powerbomb/models/powerup_powerbomb.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/imats/powerup_ice__missile_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_supermissile/models/powerup_ice__missile.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/imats/powerup_wavebeam_cangrejo.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/items/powerup_widebeam/models/powerup_wavebeam.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_matfx.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/imats/shield_diffusion_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield___diffusion/models/shield_diffusion.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/imats/shield_icemissile_mp_opaque_01.bsmat`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/actors/props/shield_icemissile/models/shield_icemissile.bcmdl`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_at.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/itemsphere/models/textures/speedboost_nm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphat.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex` & `open-dread-rando-1.9.0/open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/files/schema.json` & `open-dread-rando-1.9.0/open_dread_rando/files/schema.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999994375508088%*

 * *Differences: {"'properties'": "{'cosmetic_patches': {'properties': {'lua': {'properties': {'custom_init': "*

 * *                 "{'properties': {'enable_room_name_display': OrderedDict([('type', 'string'), "*

 * *                 "('enum', ['NEVER', 'ALWAYS', 'WITH_FADE']), ('default', 'NEVER'), "*

 * *                 "('description', 'Configures how the room name is displayed on the HUD. Defaults "*

 * *                 "to disabled.')])}}, 'camera_names_dict': OrderedDict([('type', 'object'), "*

 * *                 "('description', 'A dic […]*

```diff
@@ -202,21 +202,48 @@
             "properties": {
                 "config": {
                     "type": "object"
                 },
                 "lua": {
                     "additionalProperties": false,
                     "properties": {
+                        "camera_names_dict": {
+                            "additionalProperties": false,
+                            "default": {},
+                            "description": "A dictionary of dictionaries mapping scenario and collision camera to room name in the database",
+                            "patternProperties": {
+                                ".*": {
+                                    "additionalProperties": false,
+                                    "patternProperties": {
+                                        ".*": {
+                                            "type": "string"
+                                        }
+                                    },
+                                    "type": "object"
+                                }
+                            },
+                            "type": "object"
+                        },
                         "custom_init": {
                             "additionalProperties": false,
                             "properties": {
                                 "enable_death_counter": {
                                     "default": false,
                                     "description": "Enables an in-game death counter shown in the player's HUD",
                                     "type": "boolean"
+                                },
+                                "enable_room_name_display": {
+                                    "default": "NEVER",
+                                    "description": "Configures how the room name is displayed on the HUD. Defaults to disabled.",
+                                    "enum": [
+                                        "NEVER",
+                                        "ALWAYS",
+                                        "WITH_FADE"
+                                    ],
+                                    "type": "string"
                                 }
                             },
                             "type": "object"
                         }
                     },
                     "type": "object"
                 }
@@ -248,15 +275,17 @@
                             "charge_beam",
                             "diffusion_beam",
                             "wide_beam",
                             "plasma_beam",
                             "wave_beam",
                             "missile",
                             "super_missile",
-                            "ice_missile"
+                            "ice_missile",
+                            "grapple_beam",
+                            "sensor_door"
                         ],
                         "type": "string"
                     }
                 },
                 "required": [
                     "actor",
                     "door_type"
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/game_patches.py` & `open-dread-rando-1.9.0/open_dread_rando/game_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/lua_editor.py` & `open-dread-rando-1.9.0/open_dread_rando/lua_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 from pathlib import Path
 
 from open_dread_rando import lua_util
-from open_dread_rando.common_data import ALL_SCENARIOS
+from open_dread_rando.constants import ALL_SCENARIOS
 from open_dread_rando.patcher_editor import PatcherEditor, path_for_level
 
 
 def _read_powerup_lua() -> bytes:
     return Path(__file__).parent.joinpath("files", "randomizer_powerup.lua").read_bytes()
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/map_icons.py` & `open-dread-rando-1.9.0/open_dread_rando/map_icons.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 from typing import Tuple, Union, TYPE_CHECKING
 
 from mercury_engine_data_structures.formats import Bmmdef
 
-from open_dread_rando.common_data import ALL_SCENARIOS
+from open_dread_rando.constants import ALL_SCENARIOS
 from open_dread_rando.text_patches import patch_text
 if TYPE_CHECKING:
     from open_dread_rando.patcher_editor import PatcherEditor
 
 
 @dataclasses.dataclass(frozen=True)
 class MapIcon:
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/model_data.py` & `open-dread-rando-1.9.0/open_dread_rando/model_data.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/objective.py` & `open-dread-rando-1.9.0/open_dread_rando/objective.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/output_config.py` & `open-dread-rando-1.9.0/open_dread_rando/output_config.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/patch_util.py` & `open-dread-rando-1.9.0/open_dread_rando/patch_util.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/patcher_editor.py` & `open-dread-rando-1.9.0/open_dread_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/pickup.py` & `open-dread-rando-1.9.0/open_dread_rando/pickup.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/static_fixes.py` & `open-dread-rando-1.9.0/open_dread_rando/static_fixes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 from typing import Optional
 
 import construct
 from mercury_engine_data_structures.formats.gui_files import Bmscp
 
 from open_dread_rando import door_patcher
-from open_dread_rando.common_data import ALL_SCENARIOS
+from open_dread_rando.constants import ALL_SCENARIOS
 from open_dread_rando.logger import LOG
 from open_dread_rando.map_icons import MapIconEditor
 from open_dread_rando.patcher_editor import PatcherEditor
 
 
 def flip_icon_id(icon_id: str) -> str:
     if icon_id.endswith("R"):
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/templates/custom_core_x.lua` & `open-dread-rando-1.9.0/open_dread_rando/templates/custom_core_x.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua` & `open-dread-rando-1.9.0/open_dread_rando/templates/custom_core_x_superquetzoa.lua`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/templates/custom_init.lua` & `open-dread-rando-1.9.0/open_dread_rando/templates/custom_init.lua`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 Init.fEnergyPerPart = TEMPLATE("energy_per_part")
 Init.bImmediateEnergyParts = TEMPLATE("immediate_energy_parts")
 Init.bDefaultXRelease = TEMPLATE("default_x_released")
 Init.bEnableExperimentBoss = TEMPLATE("enable_experiment_boss")
 Init.iNumRequiredArtifacts = TEMPLATE("required_artifacts")
 Init.bWarpToStart = TEMPLATE("warp_to_start")
 Init.bEnableDeathCounter = TEMPLATE("enable_death_counter")
+Init.bEnableRoomIds = TEMPLATE("enable_room_ids")
+Init.bRoomIdFadeTime = TEMPLATE("room_id_fade_time")
 
 Game.LogWarn(0, "Inventory:")
 for k, v in pairs(Init.tNewGameInventory) do
     Game.LogWarn(0, tostring(k) .. " = " .. tostring(v))
 end
 
 local buff = {}
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando/templates/template_doorshield_bmsad.json` & `open-dread-rando-1.9.0/open_dread_rando/templates/template_doorshield_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/templates/template_powerup_bmsad.json` & `open-dread-rando-1.9.0/open_dread_rando/templates/template_powerup_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/templates/template_shieldenergy_bmsad.json` & `open-dread-rando-1.9.0/open_dread_rando/templates/template_shieldenergy_bmsad.json`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/text_patches.py` & `open-dread-rando-1.9.0/open_dread_rando/text_patches.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/tilegroup_patcher.py` & `open-dread-rando-1.9.0/open_dread_rando/tilegroup_patcher.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando/validator_with_default.py` & `open-dread-rando-1.9.0/open_dread_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/open_dread_rando.egg-info/PKG-INFO` & `open-dread-rando-1.9.0/open_dread_rando.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-dread-rando
-Version: 1.8.0
+Version: 1.9.0
 Summary: An open source randomizer patcher for Metroid Dread.
 Home-page: https://github.com/randovania/open-dread-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `open-dread-rando-1.8.0/open_dread_rando.egg-info/SOURCES.txt` & `open-dread-rando-1.9.0/open_dread_rando.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 .github/dependabot.yml
 .github/workflows/patch.yml
 .github/workflows/python.yml
 .vscode/settings.json
 open_dread_rando/__init__.py
 open_dread_rando/__main__.py
 open_dread_rando/cli.py
-open_dread_rando/common_data.py
+open_dread_rando/constants.py
 open_dread_rando/cosmetic_patches.py
 open_dread_rando/custom_door_types.py
 open_dread_rando/door_patcher.py
 open_dread_rando/dread_patcher.py
 open_dread_rando/elevator.py
 open_dread_rando/environmental_damage.py
 open_dread_rando/environmental_damage_sources.py
@@ -63,14 +63,15 @@
 open_dread_rando/files/levels/s080_shipyard.lc.lua
 open_dread_rando/files/levels/s090_skybase.lc.lua
 open_dread_rando/files/lua_libraries/bit.lua
 open_dread_rando/files/lua_libraries/data_structures.lua
 open_dread_rando/files/lua_libraries/death_counter.lua
 open_dread_rando/files/lua_libraries/guilib.lua
 open_dread_rando/files/lua_libraries/input_handling.lua
+open_dread_rando/files/lua_libraries/room_names.lua
 open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_camo.bsmat
 open_dread_rando/files/romfs/actors/items/item_cube/model/imats/itemcube_sonr.bsmat
 open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_camo.bcmdl
 open_dread_rando/files/romfs/actors/items/item_cube_broken/model/itemcube_sonr.bcmdl
 open_dread_rando/files/romfs/actors/items/itemsphere/models/speed_booster.bcmdl
 open_dread_rando/files/romfs/actors/items/itemsphere/models/imats/speedboost_mp_opaque_01.bsmat
 open_dread_rando/files/romfs/actors/items/powerup_bomb/models/powerup_morph.bcmdl
@@ -100,14 +101,15 @@
 open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphbc.bctex
 open_dread_rando/files/romfs/textures/actors/items/powerup_bomb/models/textures/powerup_morphnm.bctex
 open_dread_rando/files/romfs/textures/actors/items/powerup_doublejump/models/textures/powerup_spi_magnet_bc.bctex
 open_dread_rando/files/romfs/textures/actors/items/powerup_supermissile/models/textures/powerup_ice__missile_bc.bctex
 open_dread_rando/files/romfs/textures/actors/items/powerup_widebeam/models/textures/pup_wavebeam_bc.bctex
 open_dread_rando/files/romfs/textures/system/minimap/icons/icons.bctex
 open_dread_rando/templates/boss_powerup_template.lua
+open_dread_rando/templates/cc_to_room_name.lua
 open_dread_rando/templates/custom_core_x.lua
 open_dread_rando/templates/custom_core_x_superquetzoa.lua
 open_dread_rando/templates/custom_init.lua
 open_dread_rando/templates/progressive_model_template.lua
 open_dread_rando/templates/randomizer_progressive_template.lua
 open_dread_rando/templates/template_doorshield_bmsad.json
 open_dread_rando/templates/template_powerup_bmsad.json
```

### Comparing `open-dread-rando-1.8.0/setup.cfg` & `open-dread-rando-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `open-dread-rando-1.8.0/tests/test_files/starter_preset_patcher.json` & `open-dread-rando-1.9.0/tests/test_files/starter_preset_patcher.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99609375%*

 * *Differences: {"'cosmetic_patches'": "{'lua': {'custom_init': {'enable_room_name_display': 'NEVER'}, "*

 * *                       "'camera_names_dict': OrderedDict([('s010_cave', "*

 * *                       "OrderedDict([('collision_camera_000', 'First Tutorial'), "*

 * *                       "('collision_camera_000_Init', 'Intro Room'), ('collision_camera_001', "*

 * *                       "'Charge Tutorial'), ('collision_camera_002', 'Melee Tutorial West'), "*

 * *                       "('collision_camera_003', 'Melee Tutorial Room'), (' […]*

```diff
@@ -11,16 +11,367 @@
                 "bShowBossLifebar": true,
                 "bShowEnemyDamage": false,
                 "bShowEnemyLife": false,
                 "bShowPlayerDamage": true
             }
         },
         "lua": {
+            "camera_names_dict": {
+                "s010_cave": {
+                    "collision_camera_000": "First Tutorial",
+                    "collision_camera_000_Init": "Intro Room",
+                    "collision_camera_001": "Charge Tutorial",
+                    "collision_camera_002": "Melee Tutorial West",
+                    "collision_camera_003": "Melee Tutorial Room",
+                    "collision_camera_004": "Early Cloak Room",
+                    "collision_camera_005": "EMMI Zone First Entrance",
+                    "collision_camera_006": "White EMMI Introduction",
+                    "collision_camera_008": "Teleport to Dairon",
+                    "collision_camera_009": "EMMI Zone Exit North",
+                    "collision_camera_010": "EMMI Zone Hub",
+                    "collision_camera_011": "Teleport to Cataris",
+                    "collision_camera_012": "Save Station West",
+                    "collision_camera_013": "Charge Beam Access",
+                    "collision_camera_014": "Charge Beam Room",
+                    "collision_camera_015": "EMMI Zone Spinner",
+                    "collision_camera_016": "Proto EMMI Introduction",
+                    "collision_camera_017": "White EMMI Arena",
+                    "collision_camera_018": "EMMI Zone Entrance Hallway",
+                    "collision_camera_020": "Corpius Arena",
+                    "collision_camera_021": "David Jaffe Room",
+                    "collision_camera_022": "Thermal Door Tutorial",
+                    "collision_camera_023": "Magma Flow Vista",
+                    "collision_camera_023_B": "East Lava Missile Room",
+                    "collision_camera_024": "Hot Room Hub",
+                    "collision_camera_025": "Save Station East",
+                    "collision_camera_026": "Chain Reaction Room",
+                    "collision_camera_028": "Varia Suit Tutorial South",
+                    "collision_camera_029": "Varia Suit Tutorial North",
+                    "collision_camera_030": "Shutter Platform Puzzle",
+                    "collision_camera_031": "Varia Suit Room",
+                    "collision_camera_032": "Spider Beam Tower",
+                    "collision_camera_033": "Grapple Beam Room",
+                    "collision_camera_034": "Transport to Dairon",
+                    "collision_camera_045": "First Tutorial Access",
+                    "collision_camera_048": "EMMI Zone Dome",
+                    "collision_camera_049": "Central Unit Access",
+                    "collision_camera_050": "Invisible Corpius Room",
+                    "collision_camera_051": "EMMI Zone Exit Northwest",
+                    "collision_camera_053": "EMMI Zone Ballspark Hallway",
+                    "collision_camera_054": "Energy Recharge Station South",
+                    "collision_camera_055": "Chain Reaction Access",
+                    "collision_camera_056": "Waterfall",
+                    "collision_camera_057": "Water Tunnel under Map",
+                    "collision_camera_058": "Map Station",
+                    "collision_camera_059": "Behind Waterfall",
+                    "collision_camera_060": "Water Reservoir",
+                    "collision_camera_061": "EMMI Zone Exit South",
+                    "collision_camera_062": "Cold Introduction",
+                    "collision_camera_063": "Save Station South",
+                    "collision_camera_064": "Proto EMMI Battle",
+                    "collision_camera_065": "Navigation Station North",
+                    "collision_camera_066": "Path to Thermal Device",
+                    "collision_camera_067": "Thermal Device",
+                    "collision_camera_068": "Navigation Station South",
+                    "collision_camera_069": "Wide Beam Block Room",
+                    "collision_camera_070": "Arbitrary Enky Room",
+                    "collision_camera_071": "EMMI First Chase End",
+                    "collision_camera_072": "Path to Corpius",
+                    "collision_camera_073": "Phantom Cloak Tutorial",
+                    "collision_camera_074": "Proto EMMI CU",
+                    "collision_camera_075": "EMMI Zone Exit Southwest",
+                    "collision_camera_076": "Save Station North",
+                    "collision_camera_077": "Transport to Cataris",
+                    "collision_camera_078": "Hot Cataris Shortcut",
+                    "collision_camera_079": "Lower Path to Cataris",
+                    "collision_camera_080": "Transport to Burenia",
+                    "collision_camera_081": "Screw Attack Room",
+                    "collision_camera_082": "Freezer",
+                    "collision_camera_083": "Speed Booster Bonus Room",
+                    "collision_camera_085": "Shortcut to Screw Attack",
+                    "collision_camera_086": "Speed Hallway",
+                    "collision_camera_088": "Shinespark Tower to Grapple",
+                    "collision_camera_089": "Grapple Beam Tutorial",
+                    "collision_camera_090": "Central Unit",
+                    "collision_camera_091": "Red Chozo Arena"
+                },
+                "s020_magma": {
+                    "collision_camera_000": "Transport to Artaria",
+                    "collision_camera_001": "Dropdown Pit",
+                    "collision_camera_002": "Navigation Station Southeast",
+                    "collision_camera_004": "Thermal Device Room South",
+                    "collision_camera_006": "Artaria Transport Access",
+                    "collision_camera_007": "Total Recharge Station South",
+                    "collision_camera_009": "Above Z-57 Fight",
+                    "collision_camera_010": "EMMI Zone Exit East",
+                    "collision_camera_012": "Lava Button East",
+                    "collision_camera_013": "Tall Magnet Walls Access",
+                    "collision_camera_014": "Moving Magnet Walls (Tall)",
+                    "collision_camera_015": "Teleport to Artaria (Blue)",
+                    "collision_camera_016": "Total Recharge Station North",
+                    "collision_camera_018": "Energy Recharge Station",
+                    "collision_camera_019": "Z-57 Heat Room West (Left)",
+                    "collision_camera_020": "Green EMMI Introduction",
+                    "collision_camera_021": "Z-57 Heat Room West (Right)",
+                    "collision_camera_022": "EMMI Zone Exit to Map Station",
+                    "collision_camera_023": "Long Mouth Statue Room",
+                    "collision_camera_024": "Above Kraid",
+                    "collision_camera_025": "Teleport to Artaria (Red)",
+                    "collision_camera_026": "Teleport to Ghavoran",
+                    "collision_camera_027": "Ghavoran Teleport Access",
+                    "collision_camera_028": "EMMI Zone Exits West",
+                    "collision_camera_029": "EMMI Zone Item Tunnel",
+                    "collision_camera_030": "Map Station",
+                    "collision_camera_031": "Moving Magnet Walls (Small)",
+                    "collision_camera_032": "EMMI Zone Tower East",
+                    "collision_camera_033": "Save Station East",
+                    "collision_camera_034": "Hall Thermal Device Room",
+                    "collision_camera_035": "EMMI Zone Tower West",
+                    "collision_camera_036": "Central Unit Access",
+                    "collision_camera_037": "Central Unit",
+                    "collision_camera_038": "Lava Button West",
+                    "collision_camera_040": "Dairon Transport Access",
+                    "collision_camera_041": "Transport to Dairon",
+                    "collision_camera_042": "Thermal Device Room North",
+                    "collision_camera_043": "Path to Kraid Entryway",
+                    "collision_camera_044": "Diffusion Beam Room",
+                    "collision_camera_045": "Lava Button East Access",
+                    "collision_camera_046": "EMMI Zone East Tower Access",
+                    "collision_camera_048": "Double Obsydomithon Room",
+                    "collision_camera_049": "Z-57 Heat Room East",
+                    "collision_camera_051": "Teleport to Dairon",
+                    "collision_camera_052": "Green EMMI Introduction Access",
+                    "collision_camera_053": "Underlava Puzzle Room 2",
+                    "collision_camera_054": "Underlava Puzzle Room 1",
+                    "collision_camera_055": "EMMI Zone Hidden Missile Room",
+                    "collision_camera_058": "Navigation Station Northwest",
+                    "collision_camera_059": "EMMI Zone West Exit Path",
+                    "collision_camera_060": "Heated U-Turn",
+                    "collision_camera_061": "Kraid Eyedoor Room",
+                    "collision_camera_062": "Save Station West",
+                    "collision_camera_063": "Kraid Arena",
+                    "collision_camera_064": "West Teleport Access",
+                    "collision_camera_CooldownX": "Experiment Z-57 Fight?"
+                },
+                "s030_baselab": {
+                    "collision_camera_000": "Save Station East",
+                    "collision_camera_001": "Teleport to Artaria",
+                    "collision_camera_002": "Hub Access",
+                    "collision_camera_003": "East Transport to Ferenia",
+                    "collision_camera_004": "Big Hub",
+                    "collision_camera_005": "EMMI Zone Exit East",
+                    "collision_camera_006": "Wide Beam Room",
+                    "collision_camera_007": "Power Switch 1",
+                    "collision_camera_008": "Teleport to Cataris",
+                    "collision_camera_009": "Total Recharge Station East",
+                    "collision_camera_010": "Early Grapple Access",
+                    "collision_camera_011": "Transport to Artaria",
+                    "collision_camera_012": "Early Grapple Room",
+                    "collision_camera_013": "Heated Room West",
+                    "collision_camera_014": "Navigation Station South",
+                    "collision_camera_015": "Energy Recharge Station Middle",
+                    "collision_camera_016": "Shinespark Tutorial",
+                    "collision_camera_017": "EMMI Zone Exit North",
+                    "collision_camera_018": "Yellow EMMI Introduction",
+                    "collision_camera_019": "West Transport to Ferenia",
+                    "collision_camera_020": "Cross Bomb Puzzle Room",
+                    "collision_camera_021": "Bomb Room",
+                    "collision_camera_022": "Total Recharge Station West",
+                    "collision_camera_023": "Map Station",
+                    "collision_camera_024": "Power Switch 2",
+                    "collision_camera_025": "Freezer",
+                    "collision_camera_026": "Test Chamber Access",
+                    "collision_camera_027": "EMMI Zone Exit Northwest",
+                    "collision_camera_028": "Experiment Z-57 Test Chamber",
+                    "collision_camera_029": "EMMI Zone Exit West",
+                    "collision_camera_030": "Hidden Grapple Shortcut Room",
+                    "collision_camera_031": "Save Station West Tunnels",
+                    "collision_camera_032": "Save Station West",
+                    "collision_camera_033": "Storm Missile Gate Room",
+                    "collision_camera_034": "Ammo Recharge Station",
+                    "collision_camera_035": "Lake Puzzle Room",
+                    "collision_camera_036": "EMMI Zone Exit Southwest",
+                    "collision_camera_037": "EMMI Zone Exit South",
+                    "collision_camera_038": "Central Unit",
+                    "collision_camera_039": "Burenia Upper Transport Access",
+                    "collision_camera_040": "Central Unit Access",
+                    "collision_camera_041": "Burenia Lower Transport Access",
+                    "collision_camera_042": "Energy Recharge Station West",
+                    "collision_camera_043": "Transport to Cataris",
+                    "collision_camera_044": "Navigation Station North",
+                    "collision_camera_045": "Lower Transport to Burenia",
+                    "collision_camera_046": "Upper Transport to Burenia",
+                    "collision_camera_047": "Transport to Ghavoran"
+                },
+                "s040_aqua": {
+                    "collision_camera_000": "Map Station",
+                    "collision_camera_001": "Upper Burenia Hub",
+                    "collision_camera_002": "Burenia Hub to Dairon",
+                    "collision_camera_003": "Upper Transport to Dairon",
+                    "collision_camera_004": "Lower Transport to Dairon",
+                    "collision_camera_005": "Drogyga Eyedoor",
+                    "collision_camera_006": "Transport to Ghavoran",
+                    "collision_camera_007": "Underneath Drogyga",
+                    "collision_camera_008": "Teleport to Ferenia",
+                    "collision_camera_009": "Navigation Station North",
+                    "collision_camera_010": "Burenia Main Hub",
+                    "collision_camera_011": "Save Station Middle",
+                    "collision_camera_012": "Underwater Horseshoe",
+                    "collision_camera_013": "Energy Recharge South",
+                    "collision_camera_014": "Flash Shift Room",
+                    "collision_camera_015": "Teleport to Ghavoran",
+                    "collision_camera_016": "Navigation Station South",
+                    "collision_camera_017": "Transport to Artaria",
+                    "collision_camera_018": "Early Gravity Speedboost Room 1",
+                    "collision_camera_019": "Early Gravity Speedboost Room 2",
+                    "collision_camera_021": "Gravity Suit Tower",
+                    "collision_camera_022": "Ammo Recharge South",
+                    "collision_camera_023_B": "Gravity Suit Room",
+                    "collision_camera_024": "Gravity Suit Room Access",
+                    "collision_camera_025": "Storm Missile Gate Room",
+                    "collision_camera_026": "Save Station South Access",
+                    "collision_camera_027": "Save Station South",
+                    "collision_camera_028": "Drogyga Arena",
+                    "collision_camera_029": "Drogyga Access",
+                    "collision_camera_030": "Save Station North"
+                },
+                "s050_forest": {
+                    "collision_camera_000": "Transport to Burenia",
+                    "collision_camera_001": "Right Entrance",
+                    "collision_camera_002": "Robot Fight Arena",
+                    "collision_camera_003": "Left Entrance",
+                    "collision_camera_004": "Blue EMMI Introduction",
+                    "collision_camera_005": "Navigation Station Access",
+                    "collision_camera_006": "Navigation Station",
+                    "collision_camera_007": "Flipper Room",
+                    "collision_camera_008": "Dairon Transport Access",
+                    "collision_camera_009": "Super Missile Room Access",
+                    "collision_camera_010": "Super Missile Room",
+                    "collision_camera_011": "EMMI Zone Exit Southeast",
+                    "collision_camera_012": "Map Station Access",
+                    "collision_camera_013": "Map Station",
+                    "collision_camera_014": "EMMI Zone Exit West",
+                    "collision_camera_015": "Early Ice Room",
+                    "collision_camera_016": "EMMI Zone Exit Northwest",
+                    "collision_camera_017": "Central Unit",
+                    "collision_camera_018": "EMMI Zone Middle Path",
+                    "collision_camera_019": "Central Unit Access",
+                    "collision_camera_020": "EMMI Zone Exit Northeast",
+                    "collision_camera_021": "Spin Boost Tower",
+                    "collision_camera_022": "Save Station Center",
+                    "collision_camera_023": "Chozo Warrior Arena",
+                    "collision_camera_024": "Golzuna Tower",
+                    "collision_camera_025_B": "Total Recharge Station North",
+                    "collision_camera_026": "Golzuna Arena",
+                    "collision_camera_027": "Transport to Ferenia",
+                    "collision_camera_028": "Map Station Access Secret",
+                    "collision_camera_029": "Elun Transport Access",
+                    "collision_camera_030": "Spin Boost Room",
+                    "collision_camera_031": "Energy Recharge Station",
+                    "collision_camera_032": "Pulse Radar Room",
+                    "collision_camera_033": "Cross Bomb Tutorial",
+                    "collision_camera_034": "Transport to Hanubia",
+                    "collision_camera_035": "Spider Magnet Elevator",
+                    "collision_camera_036": "Above Golzuna",
+                    "collision_camera_037": "Transport to Elun",
+                    "collision_camera_038": "Transport to Dairon",
+                    "collision_camera_039": "Above Pulse Radar",
+                    "collision_camera_040": "Save Station East"
+                },
+                "s060_quarantine": {
+                    "collision_camera_000": "Bridge Gate",
+                    "collision_camera_001": "Transport to Ghavoran",
+                    "collision_camera_002": "Purple Drapes",
+                    "collision_camera_003": "Ammo Recharge Station",
+                    "collision_camera_004": "Chozo Soldier Arena",
+                    "collision_camera_005": "Gyroscope Room",
+                    "collision_camera_006": "Plasma Beam Room",
+                    "collision_camera_007": "Spider Magnet Room",
+                    "collision_camera_008": "Fan Room",
+                    "collision_camera_009": "Vertical Bomb Maze",
+                    "collision_camera_010": "Horizontal Bomb Maze",
+                    "collision_camera_011": "Exterior Bridge",
+                    "collision_camera_012": "Save Station",
+                    "collision_camera_MBL_B": "Bottom Morph Launcher"
+                },
+                "s070_basesanc": {
+                    "collision_camera_000": "East Transport to Darion",
+                    "collision_camera_001": "Purple EMMI Introduction Access",
+                    "collision_camera_002": "Total Recharge Station",
+                    "collision_camera_003": "EMMI Zone Exit West",
+                    "collision_camera_004": "Fan Room Access",
+                    "collision_camera_005": "Quiet Robe Room",
+                    "collision_camera_006": "Fan Room",
+                    "collision_camera_007": "Teleport to Burenia (Cyan)",
+                    "collision_camera_008": "Transport to Dairon",
+                    "collision_camera_009": "Speedboost Slopes Maze",
+                    "collision_camera_010": "Cold Room (Small)",
+                    "collision_camera_011": "Separate Tunnels Room",
+                    "collision_camera_012": "Space Jump Room",
+                    "collision_camera_013": "Pitfall Puzzle Room",
+                    "collision_camera_014": "Transport to Ghavoran",
+                    "collision_camera_015": "Space Jump Room Access",
+                    "collision_camera_016": "Navigation Station",
+                    "collision_camera_017": "Twin Robot Arena",
+                    "collision_camera_018": "Cold Room (Energy Recharge Station)",
+                    "collision_camera_019": "Energy Recharge Station (Gate)",
+                    "collision_camera_020": "Energy Recharge Station Secret",
+                    "collision_camera_021": "EMMI Zone Exit Middle",
+                    "collision_camera_022": "Map Station Access",
+                    "collision_camera_023": "Map Station",
+                    "collision_camera_024": "Storm Missile Tutorial",
+                    "collision_camera_025": "Path to Escue",
+                    "collision_camera_026": "Escue Eyedoor Room",
+                    "collision_camera_027": "Escue Arena",
+                    "collision_camera_028": "Transport to Hanubia",
+                    "collision_camera_029": "Save Station North",
+                    "collision_camera_030": "Cold Room (Storm Missile Gate)",
+                    "collision_camera_031": "Wave Beam Tutorial",
+                    "collision_camera_032": "EMMI Zone Exit East",
+                    "collision_camera_033": "EMMI Zone Exit East Access",
+                    "collision_camera_034": "Purple EMMI Arena",
+                    "collision_camera_035": "Central Unit",
+                    "collision_camera_038_A": "Central Unit Access",
+                    "collision_camera_040": "Purple EMMI Introduction",
+                    "collision_camera_041": "Save Station Southeast"
+                },
+                "s080_shipyard": {
+                    "collision_camera_000": "Transport to Ferenia",
+                    "collision_camera_001": "Transport to Ghavoran",
+                    "collision_camera_002": "Ferenia Shortcut",
+                    "collision_camera_003": "Navigation Station",
+                    "collision_camera_004": "Entrance Tall Room",
+                    "collision_camera_005": "Gold Chozo Warrior Arena",
+                    "collision_camera_006": "Total Recharge Station North",
+                    "collision_camera_007": "Transport to Itorash",
+                    "collision_camera_008": "Ship Room",
+                    "collision_camera_009": "Speedboost Puzzle Room",
+                    "collision_camera_010": "Tank Room",
+                    "collision_camera_011": "EMMI Zone Exit West",
+                    "collision_camera_012": "Central Unit",
+                    "collision_camera_013": "EMMI Zone Exit East",
+                    "collision_camera_014": "Orange EMMI Introduction",
+                    "collision_camera_015": "Total Recharge Station East",
+                    "collision_camera_016": "Escape Room 3",
+                    "collision_camera_018": "Escape Room 2",
+                    "collision_camera_019": "Escape Room 1",
+                    "collision_camera_020": "Raven Beak X Arena",
+                    "collision_camera_1000": "collision_camera_1000 (H)"
+                },
+                "s090_skybase": {
+                    "collision_camera_000": "Save Station",
+                    "collision_camera_001": "Transport to Hanubia",
+                    "collision_camera_002": "Elevator to Raven Beak",
+                    "collision_camera_003": "Elevator Cutscene",
+                    "collision_camera_004": "Raven Beak Arena"
+                }
+            },
             "custom_init": {
-                "enable_death_counter": true
+                "enable_death_counter": true,
+                "enable_room_name_display": "NEVER"
             }
         }
     },
     "door_patches": [
         {
             "actor": {
                 "actor": "doorpowerpower_005",
```

