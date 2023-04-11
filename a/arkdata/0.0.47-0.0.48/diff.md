# Comparing `tmp/arkdata-0.0.47.tar.gz` & `tmp/arkdata-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdata-0.0.47.tar", last modified: Tue Apr 11 00:09:54 2023, max compression
+gzip compressed data, was "arkdata-0.0.48.tar", last modified: Tue Apr 11 00:24:14 2023, max compression
```

## Comparing `arkdata-0.0.47.tar` & `arkdata-0.0.48.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 00:09:54.623171 arkdata-0.0.47/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-0.0.47/LICENSE
--rw-rw-rw-   0        0        0      804 2023-04-11 00:09:54.623171 arkdata-0.0.47/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-0.0.47/README.md
--rw-rw-rw-   0        0        0      632 2023-04-11 00:09:21.000000 arkdata-0.0.47/pyproject.toml
--rw-rw-rw-   0        0        0     1270 2023-04-11 00:09:54.629674 arkdata-0.0.47/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 00:09:54.545146 arkdata-0.0.47/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 00:09:54.552665 arkdata-0.0.47/src/arkdata/
--rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-0.0.47/src/arkdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:09:54.571705 arkdata-0.0.47/src/arkdata/database/
--rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/database/__init__.py
--rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-0.0.47/src/arkdata/database/configuration.py
--rw-rw-rw-   0        0        0     3858 2023-04-07 21:33:59.000000 arkdata-0.0.47/src/arkdata/database/cursor.py
--rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-0.0.47/src/arkdata/database/database.py
--rw-rw-rw-   0        0        0     4727 2023-04-07 22:03:59.000000 arkdata-0.0.47/src/arkdata/database/table.py
--rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-0.0.47/src/arkdata/main.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:09:54.596169 arkdata-0.0.47/src/arkdata/models/
--rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-0.0.47/src/arkdata/models/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-0.0.47/src/arkdata/models/account.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/ammunition.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/armour.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/artifact.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/attachment.py
--rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/cart_item.py
--rw-rw-rw-   0        0        0     1698 2023-04-04 04:45:14.000000 arkdata-0.0.47/src/arkdata/models/command.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/consumable.py
--rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/creature.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/dye.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/egg.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/farm.py
--rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/order_item.py
--rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/product.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/recipe.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/resource.py
--rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/saddle.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/seed.py
--rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/sessions.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/skin.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/structure.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/tool.py
--rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/trophy.py
--rw-rw-rw-   0        0        0     1611 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/user.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.47/src/arkdata/models/weapon.py
-drwxrwxrwx   0        0        0        0 2023-04-11 00:09:54.622171 arkdata-0.0.47/src/arkdata/seeds/
--rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-0.0.47/src/arkdata/seeds/__init__.py
--rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-0.0.47/src/arkdata/seeds/accounts.json
--rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-0.0.47/src/arkdata/seeds/ammunitions.json
--rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-0.0.47/src/arkdata/seeds/armours.json
--rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-0.0.47/src/arkdata/seeds/artifacts.json
--rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-0.0.47/src/arkdata/seeds/attachments.json
--rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-0.0.47/src/arkdata/seeds/commands.json
--rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-0.0.47/src/arkdata/seeds/consumables.json
--rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-0.0.47/src/arkdata/seeds/creatures.json
--rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-0.0.47/src/arkdata/seeds/dyes.json
--rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-0.0.47/src/arkdata/seeds/eggs.json
--rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-0.0.47/src/arkdata/seeds/farms.json
--rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-0.0.47/src/arkdata/seeds/products.json
--rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-0.0.47/src/arkdata/seeds/recipes.json
--rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-0.0.47/src/arkdata/seeds/resources.json
--rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-0.0.47/src/arkdata/seeds/saddles.json
--rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-0.0.47/src/arkdata/seeds/seeds.json
--rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-0.0.47/src/arkdata/seeds/skins.json
--rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-0.0.47/src/arkdata/seeds/structures.json
--rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-0.0.47/src/arkdata/seeds/tools.json
--rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-0.0.47/src/arkdata/seeds/trophies.json
--rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-0.0.47/src/arkdata/seeds/users.json
--rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-0.0.47/src/arkdata/seeds/weapons.json
-drwxrwxrwx   0        0        0        0 2023-04-11 00:09:54.567181 arkdata-0.0.47/src/arkdata.egg-info/
--rw-rw-rw-   0        0        0      804 2023-04-11 00:09:54.000000 arkdata-0.0.47/src/arkdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2023-04-11 00:09:54.000000 arkdata-0.0.47/src/arkdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 00:09:54.000000 arkdata-0.0.47/src/arkdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-04-11 00:09:54.000000 arkdata-0.0.47/src/arkdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 00:09:54.000000 arkdata-0.0.47/src/arkdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 00:24:14.818508 arkdata-0.0.48/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-0.0.48/LICENSE
+-rw-rw-rw-   0        0        0      804 2023-04-11 00:24:14.818508 arkdata-0.0.48/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-0.0.48/README.md
+-rw-rw-rw-   0        0        0      669 2023-04-11 00:23:50.000000 arkdata-0.0.48/pyproject.toml
+-rw-rw-rw-   0        0        0     1315 2023-04-11 00:24:14.826027 arkdata-0.0.48/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 00:24:14.736146 arkdata-0.0.48/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 00:24:14.743199 arkdata-0.0.48/src/arkdata/
+-rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-0.0.48/src/arkdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:24:14.763109 arkdata-0.0.48/src/arkdata/database/
+-rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/database/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-0.0.48/src/arkdata/database/configuration.py
+-rw-rw-rw-   0        0        0     3858 2023-04-07 21:33:59.000000 arkdata-0.0.48/src/arkdata/database/cursor.py
+-rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-0.0.48/src/arkdata/database/database.py
+-rw-rw-rw-   0        0        0     4727 2023-04-07 22:03:59.000000 arkdata-0.0.48/src/arkdata/database/table.py
+-rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-0.0.48/src/arkdata/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:24:14.790943 arkdata-0.0.48/src/arkdata/models/
+-rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-0.0.48/src/arkdata/models/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-0.0.48/src/arkdata/models/account.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/ammunition.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/armour.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/artifact.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/attachment.py
+-rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/cart_item.py
+-rw-rw-rw-   0        0        0     1698 2023-04-04 04:45:14.000000 arkdata-0.0.48/src/arkdata/models/command.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/consumable.py
+-rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/creature.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/dye.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/egg.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/farm.py
+-rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/order_item.py
+-rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/product.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/recipe.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/resource.py
+-rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/saddle.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/seed.py
+-rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/sessions.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/skin.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/structure.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/tool.py
+-rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/trophy.py
+-rw-rw-rw-   0        0        0     1611 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/user.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.48/src/arkdata/models/weapon.py
+drwxrwxrwx   0        0        0        0 2023-04-11 00:24:14.816506 arkdata-0.0.48/src/arkdata/seeds/
+-rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-0.0.48/src/arkdata/seeds/__init__.py
+-rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-0.0.48/src/arkdata/seeds/accounts.json
+-rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-0.0.48/src/arkdata/seeds/ammunitions.json
+-rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-0.0.48/src/arkdata/seeds/armours.json
+-rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-0.0.48/src/arkdata/seeds/artifacts.json
+-rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-0.0.48/src/arkdata/seeds/attachments.json
+-rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-0.0.48/src/arkdata/seeds/commands.json
+-rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-0.0.48/src/arkdata/seeds/consumables.json
+-rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-0.0.48/src/arkdata/seeds/creatures.json
+-rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-0.0.48/src/arkdata/seeds/dyes.json
+-rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-0.0.48/src/arkdata/seeds/eggs.json
+-rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-0.0.48/src/arkdata/seeds/farms.json
+-rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-0.0.48/src/arkdata/seeds/products.json
+-rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-0.0.48/src/arkdata/seeds/recipes.json
+-rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-0.0.48/src/arkdata/seeds/resources.json
+-rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-0.0.48/src/arkdata/seeds/saddles.json
+-rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-0.0.48/src/arkdata/seeds/seeds.json
+-rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-0.0.48/src/arkdata/seeds/skins.json
+-rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-0.0.48/src/arkdata/seeds/structures.json
+-rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-0.0.48/src/arkdata/seeds/tools.json
+-rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-0.0.48/src/arkdata/seeds/trophies.json
+-rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-0.0.48/src/arkdata/seeds/users.json
+-rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-0.0.48/src/arkdata/seeds/weapons.json
+drwxrwxrwx   0        0        0        0 2023-04-11 00:24:14.758714 arkdata-0.0.48/src/arkdata.egg-info/
+-rw-rw-rw-   0        0        0      804 2023-04-11 00:24:14.000000 arkdata-0.0.48/src/arkdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1948 2023-04-11 00:24:14.000000 arkdata-0.0.48/src/arkdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 00:24:14.000000 arkdata-0.0.48/src/arkdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-04-11 00:24:14.000000 arkdata-0.0.48/src/arkdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 00:24:14.000000 arkdata-0.0.48/src/arkdata.egg-info/top_level.txt
```

### Comparing `arkdata-0.0.47/LICENSE` & `arkdata-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/PKG-INFO` & `arkdata-0.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 0.0.47
+Version: 0.0.48
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `arkdata-0.0.47/pyproject.toml` & `arkdata-0.0.48/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
-    "arklibrary",
-    "python-dotenv",
-    "SQLAlchemy",
-    "sqlalchemy_utils",
-    "flask"
+    "arklibrary>=0.0.62",
+    "python-dotenv>=1.0.0",
+    "SQLAlchemy>=2.0.9",
+    "sqlalchemy_utils>=0.40.0",
+    "flask>=2.2.3"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [too.pytest.ini_options]
 addopts = "--cov=arkdata"
 testpaths = [
```

### Comparing `arkdata-0.0.47/setup.cfg` & `arkdata-0.0.48/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6461 7461 0d0a 7665 7273   = arkdata..vers
-00000020: 696f 6e20 3d20 302e 302e 3437 0d0a 6175  ion = 0.0.47..au
+00000020: 696f 6e20 3d20 302e 302e 3438 0d0a 6175  ion = 0.0.48..au
 00000030: 7468 6f72 203d 204d 6175 7269 6369 6f0d  thor = Mauricio.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6465 762e 6d61 7572 6963 696f 2e6c 6f6d  dev.mauricio.lom
 00000060: 656c 6940 676d 6169 6c2e 636f 6d0d 0a64  eli@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2054 6869  escription = Thi
 00000080: 7320 6170 706c 6963 6174 696f 6e20 6163  s application ac
 00000090: 6365 7373 6573 2074 6865 2041 726b 2073  cesses the Ark s
@@ -44,37 +44,40 @@
 000002b0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
 000002c0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
 000002d0: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
 000002e0: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
 000002f0: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
 00000300: 7569 7265 7320 3d20 3e3d 332e 360d 0a69  uires = >=3.6..i
 00000310: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000320: 3d20 0d0a 0972 6571 7565 7374 730d 0a09  = ...requests...
-00000330: 6172 6b6c 6962 7261 7279 0d0a 0970 7974  arklibrary...pyt
-00000340: 686f 6e2d 646f 7465 6e76 0d0a 0953 514c  hon-dotenv...SQL
-00000350: 416c 6368 656d 790d 0a09 7371 6c61 6c63  Alchemy...sqlalc
-00000360: 6865 6d79 5f75 7469 6c73 0d0a 0966 6c61  hemy_utils...fla
-00000370: 736b 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  sk....[options.p
-00000380: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-00000390: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
-000003a0: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
-000003b0: 7175 6972 655d 0d0a 7465 7374 696e 6720  quire]..testing 
-000003c0: 3d20 0d0a 0970 7974 6573 743e 3d36 2e30  = ...pytest>=6.0
-000003d0: 0d0a 0970 7974 6573 742d 636f 763e 3d32  ...pytest-cov>=2
-000003e0: 2e30 0d0a 096d 7970 793e 3d30 2e39 3731  .0...mypy>=0.971
-000003f0: 0d0a 0966 6c61 6b65 383e 3d33 2e39 0d0a  ...flake8>=3.9..
-00000400: 0974 6f78 3e3d 332e 3234 0d0a 0d0a 5b6f  .tox>=3.24....[o
-00000410: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
-00000420: 6174 615d 0d0a 6172 6b64 6174 6120 3d20  ata]..arkdata = 
-00000430: 0d0a 0970 792e 7479 7065 640d 0a09 636f  ...py.typed...co
-00000440: 6e66 6967 2e69 6e69 0d0a 6172 6b64 6174  nfig.ini..arkdat
-00000450: 612e 7365 6564 7320 3d20 0d0a 092a 2e6a  a.seeds = ...*.j
-00000460: 736f 6e0d 0a61 726b 6461 7461 2e73 6565  son..arkdata.see
-00000470: 6473 2e64 6174 6120 3d20 0d0a 092a 2e6a  ds.data = ...*.j
-00000480: 736f 6e0d 0a61 726b 6461 7461 2e73 6565  son..arkdata.see
-00000490: 6473 2e74 6162 6c65 7320 3d20 0d0a 092a  ds.tables = ...*
-000004a0: 2e6a 736f 6e0d 0a0d 0a5b 666c 616b 6538  .json....[flake8
-000004b0: 5d0d 0a6d 6178 2d6c 696e 652d 6c65 6e67  ]..max-line-leng
-000004c0: 7468 203d 2031 3630 0d0a 0d0a 5b65 6767  th = 160....[egg
-000004d0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000004e0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000004f0: 2030 0d0a 0d0a                            0....
+00000320: 3d20 0d0a 0972 6571 7565 7374 733e 3d32  = ...requests>=2
+00000330: 2e32 382e 310d 0a09 6172 6b6c 6962 7261  .28.1...arklibra
+00000340: 7279 3e3d 302e 302e 3632 0d0a 0970 7974  ry>=0.0.62...pyt
+00000350: 686f 6e2d 646f 7465 6e76 3e3d 312e 302e  hon-dotenv>=1.0.
+00000360: 300d 0a09 5351 4c41 6c63 6865 6d79 3e3d  0...SQLAlchemy>=
+00000370: 322e 302e 390d 0a09 7371 6c61 6c63 6865  2.0.9...sqlalche
+00000380: 6d79 5f75 7469 6c73 3e3d 302e 3430 2e30  my_utils>=0.40.0
+00000390: 0d0a 0966 6c61 736b 3e3d 322e 322e 330d  ...flask>=2.2.3.
+000003a0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+000003b0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+000003c0: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
+000003d0: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
+000003e0: 7265 5d0d 0a74 6573 7469 6e67 203d 200d  re]..testing = .
+000003f0: 0a09 7079 7465 7374 3e3d 362e 300d 0a09  ..pytest>=6.0...
+00000400: 7079 7465 7374 2d63 6f76 3e3d 322e 300d  pytest-cov>=2.0.
+00000410: 0a09 6d79 7079 3e3d 302e 3937 310d 0a09  ..mypy>=0.971...
+00000420: 666c 616b 6538 3e3d 332e 390d 0a09 746f  flake8>=3.9...to
+00000430: 783e 3d33 2e32 340d 0a0d 0a5b 6f70 7469  x>=3.24....[opti
+00000440: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+00000450: 5d0d 0a61 726b 6461 7461 203d 200d 0a09  ]..arkdata = ...
+00000460: 7079 2e74 7970 6564 0d0a 0963 6f6e 6669  py.typed...confi
+00000470: 672e 696e 690d 0a61 726b 6461 7461 2e73  g.ini..arkdata.s
+00000480: 6565 6473 203d 200d 0a09 2a2e 6a73 6f6e  eeds = ...*.json
+00000490: 0d0a 6172 6b64 6174 612e 7365 6564 732e  ..arkdata.seeds.
+000004a0: 6461 7461 203d 200d 0a09 2a2e 6a73 6f6e  data = ...*.json
+000004b0: 0d0a 6172 6b64 6174 612e 7365 6564 732e  ..arkdata.seeds.
+000004c0: 7461 626c 6573 203d 200d 0a09 2a2e 6a73  tables = ...*.js
+000004d0: 6f6e 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  on....[flake8]..
+000004e0: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
+000004f0: 3d20 3136 300d 0a0d 0a5b 6567 675f 696e  = 160....[egg_in
+00000500: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000510: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000520: 0a0d 0a                                  ...
```

### Comparing `arkdata-0.0.47/src/arkdata/database/configuration.py` & `arkdata-0.0.48/src/arkdata/database/configuration.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/database/cursor.py` & `arkdata-0.0.48/src/arkdata/database/cursor.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/database/database.py` & `arkdata-0.0.48/src/arkdata/database/database.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/database/table.py` & `arkdata-0.0.48/src/arkdata/database/table.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/__init__.py` & `arkdata-0.0.48/src/arkdata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/account.py` & `arkdata-0.0.48/src/arkdata/models/account.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/ammunition.py` & `arkdata-0.0.48/src/arkdata/models/ammunition.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/armour.py` & `arkdata-0.0.48/src/arkdata/models/armour.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/artifact.py` & `arkdata-0.0.48/src/arkdata/models/artifact.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/attachment.py` & `arkdata-0.0.48/src/arkdata/models/attachment.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/cart_item.py` & `arkdata-0.0.48/src/arkdata/models/cart_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/command.py` & `arkdata-0.0.48/src/arkdata/models/command.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/consumable.py` & `arkdata-0.0.48/src/arkdata/models/consumable.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/creature.py` & `arkdata-0.0.48/src/arkdata/models/creature.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/dye.py` & `arkdata-0.0.48/src/arkdata/models/dye.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/egg.py` & `arkdata-0.0.48/src/arkdata/models/egg.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/farm.py` & `arkdata-0.0.48/src/arkdata/models/farm.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/order_item.py` & `arkdata-0.0.48/src/arkdata/models/order_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/product.py` & `arkdata-0.0.48/src/arkdata/models/product.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/recipe.py` & `arkdata-0.0.48/src/arkdata/models/recipe.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/resource.py` & `arkdata-0.0.48/src/arkdata/models/resource.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/saddle.py` & `arkdata-0.0.48/src/arkdata/models/saddle.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/seed.py` & `arkdata-0.0.48/src/arkdata/models/seed.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/server.py` & `arkdata-0.0.48/src/arkdata/models/server.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/sessions.py` & `arkdata-0.0.48/src/arkdata/models/sessions.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/skin.py` & `arkdata-0.0.48/src/arkdata/models/skin.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/structure.py` & `arkdata-0.0.48/src/arkdata/models/structure.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/tool.py` & `arkdata-0.0.48/src/arkdata/models/tool.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/trophy.py` & `arkdata-0.0.48/src/arkdata/models/trophy.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/user.py` & `arkdata-0.0.48/src/arkdata/models/user.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/models/weapon.py` & `arkdata-0.0.48/src/arkdata/models/weapon.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/accounts.json` & `arkdata-0.0.48/src/arkdata/seeds/accounts.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/ammunitions.json` & `arkdata-0.0.48/src/arkdata/seeds/ammunitions.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/armours.json` & `arkdata-0.0.48/src/arkdata/seeds/armours.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/artifacts.json` & `arkdata-0.0.48/src/arkdata/seeds/artifacts.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/attachments.json` & `arkdata-0.0.48/src/arkdata/seeds/attachments.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/commands.json` & `arkdata-0.0.48/src/arkdata/seeds/commands.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/consumables.json` & `arkdata-0.0.48/src/arkdata/seeds/consumables.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/creatures.json` & `arkdata-0.0.48/src/arkdata/seeds/creatures.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/dyes.json` & `arkdata-0.0.48/src/arkdata/seeds/dyes.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/eggs.json` & `arkdata-0.0.48/src/arkdata/seeds/eggs.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/farms.json` & `arkdata-0.0.48/src/arkdata/seeds/farms.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/products.json` & `arkdata-0.0.48/src/arkdata/seeds/products.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/recipes.json` & `arkdata-0.0.48/src/arkdata/seeds/recipes.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/resources.json` & `arkdata-0.0.48/src/arkdata/seeds/resources.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/saddles.json` & `arkdata-0.0.48/src/arkdata/seeds/saddles.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/seeds.json` & `arkdata-0.0.48/src/arkdata/seeds/seeds.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/skins.json` & `arkdata-0.0.48/src/arkdata/seeds/skins.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/structures.json` & `arkdata-0.0.48/src/arkdata/seeds/structures.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/tools.json` & `arkdata-0.0.48/src/arkdata/seeds/tools.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/trophies.json` & `arkdata-0.0.48/src/arkdata/seeds/trophies.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/users.json` & `arkdata-0.0.48/src/arkdata/seeds/users.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata/seeds/weapons.json` & `arkdata-0.0.48/src/arkdata/seeds/weapons.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.47/src/arkdata.egg-info/PKG-INFO` & `arkdata-0.0.48/src/arkdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 0.0.47
+Version: 0.0.48
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `arkdata-0.0.47/src/arkdata.egg-info/SOURCES.txt` & `arkdata-0.0.48/src/arkdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

