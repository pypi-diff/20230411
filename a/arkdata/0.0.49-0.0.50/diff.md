# Comparing `tmp/arkdata-0.0.49.tar.gz` & `tmp/arkdata-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdata-0.0.49.tar", last modified: Tue Apr 11 02:21:24 2023, max compression
+gzip compressed data, was "arkdata-0.0.50.tar", last modified: Tue Apr 11 02:30:19 2023, max compression
```

## Comparing `arkdata-0.0.49.tar` & `arkdata-0.0.50.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 02:21:24.620818 arkdata-0.0.49/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-0.0.49/LICENSE
--rw-rw-rw-   0        0        0      804 2023-04-11 02:21:24.621817 arkdata-0.0.49/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-0.0.49/README.md
--rw-rw-rw-   0        0        0      669 2023-04-11 00:23:50.000000 arkdata-0.0.49/pyproject.toml
--rw-rw-rw-   0        0        0     1315 2023-04-11 02:21:24.622814 arkdata-0.0.49/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 02:21:24.548022 arkdata-0.0.49/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 02:21:24.555023 arkdata-0.0.49/src/arkdata/
--rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-0.0.49/src/arkdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:21:24.565022 arkdata-0.0.49/src/arkdata/database/
--rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/database/__init__.py
--rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-0.0.49/src/arkdata/database/configuration.py
--rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-0.0.49/src/arkdata/database/cursor.py
--rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-0.0.49/src/arkdata/database/database.py
--rw-rw-rw-   0        0        0     4856 2023-04-11 02:19:26.000000 arkdata-0.0.49/src/arkdata/database/table.py
--rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-0.0.49/src/arkdata/main.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:21:24.591287 arkdata-0.0.49/src/arkdata/models/
--rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-0.0.49/src/arkdata/models/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-0.0.49/src/arkdata/models/account.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/ammunition.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/armour.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/artifact.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/attachment.py
--rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/cart_item.py
--rw-rw-rw-   0        0        0     1698 2023-04-04 04:45:14.000000 arkdata-0.0.49/src/arkdata/models/command.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/consumable.py
--rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/creature.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/dye.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/egg.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/farm.py
--rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/order_item.py
--rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/product.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/recipe.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/resource.py
--rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/saddle.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/seed.py
--rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/sessions.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/skin.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/structure.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/tool.py
--rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/trophy.py
--rw-rw-rw-   0        0        0     1581 2023-04-11 01:12:51.000000 arkdata-0.0.49/src/arkdata/models/user.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.49/src/arkdata/models/weapon.py
-drwxrwxrwx   0        0        0        0 2023-04-11 02:21:24.620818 arkdata-0.0.49/src/arkdata/seeds/
--rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-0.0.49/src/arkdata/seeds/__init__.py
--rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-0.0.49/src/arkdata/seeds/accounts.json
--rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-0.0.49/src/arkdata/seeds/ammunitions.json
--rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-0.0.49/src/arkdata/seeds/armours.json
--rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-0.0.49/src/arkdata/seeds/artifacts.json
--rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-0.0.49/src/arkdata/seeds/attachments.json
--rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-0.0.49/src/arkdata/seeds/commands.json
--rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-0.0.49/src/arkdata/seeds/consumables.json
--rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-0.0.49/src/arkdata/seeds/creatures.json
--rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-0.0.49/src/arkdata/seeds/dyes.json
--rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-0.0.49/src/arkdata/seeds/eggs.json
--rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-0.0.49/src/arkdata/seeds/farms.json
--rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-0.0.49/src/arkdata/seeds/products.json
--rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-0.0.49/src/arkdata/seeds/recipes.json
--rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-0.0.49/src/arkdata/seeds/resources.json
--rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-0.0.49/src/arkdata/seeds/saddles.json
--rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-0.0.49/src/arkdata/seeds/seeds.json
--rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-0.0.49/src/arkdata/seeds/skins.json
--rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-0.0.49/src/arkdata/seeds/structures.json
--rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-0.0.49/src/arkdata/seeds/tools.json
--rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-0.0.49/src/arkdata/seeds/trophies.json
--rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-0.0.49/src/arkdata/seeds/users.json
--rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-0.0.49/src/arkdata/seeds/weapons.json
-drwxrwxrwx   0        0        0        0 2023-04-11 02:21:24.560022 arkdata-0.0.49/src/arkdata.egg-info/
--rw-rw-rw-   0        0        0      804 2023-04-11 02:21:24.000000 arkdata-0.0.49/src/arkdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2023-04-11 02:21:24.000000 arkdata-0.0.49/src/arkdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 02:21:24.000000 arkdata-0.0.49/src/arkdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-04-11 02:21:24.000000 arkdata-0.0.49/src/arkdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 02:21:24.000000 arkdata-0.0.49/src/arkdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:19.670352 arkdata-0.0.50/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-0.0.50/LICENSE
+-rw-rw-rw-   0        0        0      804 2023-04-11 02:30:19.671353 arkdata-0.0.50/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-0.0.50/README.md
+-rw-rw-rw-   0        0        0      669 2023-04-11 00:23:50.000000 arkdata-0.0.50/pyproject.toml
+-rw-rw-rw-   0        0        0     1315 2023-04-11 02:30:19.672351 arkdata-0.0.50/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:19.606352 arkdata-0.0.50/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:19.612352 arkdata-0.0.50/src/arkdata/
+-rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-0.0.50/src/arkdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:19.622351 arkdata-0.0.50/src/arkdata/database/
+-rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/database/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-0.0.50/src/arkdata/database/configuration.py
+-rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-0.0.50/src/arkdata/database/cursor.py
+-rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-0.0.50/src/arkdata/database/database.py
+-rw-rw-rw-   0        0        0     5190 2023-04-11 02:28:44.000000 arkdata-0.0.50/src/arkdata/database/table.py
+-rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-0.0.50/src/arkdata/main.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:19.646352 arkdata-0.0.50/src/arkdata/models/
+-rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-0.0.50/src/arkdata/models/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-0.0.50/src/arkdata/models/account.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/ammunition.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/armour.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/artifact.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/attachment.py
+-rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/cart_item.py
+-rw-rw-rw-   0        0        0     1698 2023-04-04 04:45:14.000000 arkdata-0.0.50/src/arkdata/models/command.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/consumable.py
+-rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/creature.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/dye.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/egg.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/farm.py
+-rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/order_item.py
+-rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/product.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/recipe.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/resource.py
+-rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/saddle.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/seed.py
+-rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/sessions.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/skin.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/structure.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/tool.py
+-rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/trophy.py
+-rw-rw-rw-   0        0        0     1581 2023-04-11 01:12:51.000000 arkdata-0.0.50/src/arkdata/models/user.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.50/src/arkdata/models/weapon.py
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:19.670352 arkdata-0.0.50/src/arkdata/seeds/
+-rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-0.0.50/src/arkdata/seeds/__init__.py
+-rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-0.0.50/src/arkdata/seeds/accounts.json
+-rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-0.0.50/src/arkdata/seeds/ammunitions.json
+-rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-0.0.50/src/arkdata/seeds/armours.json
+-rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-0.0.50/src/arkdata/seeds/artifacts.json
+-rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-0.0.50/src/arkdata/seeds/attachments.json
+-rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-0.0.50/src/arkdata/seeds/commands.json
+-rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-0.0.50/src/arkdata/seeds/consumables.json
+-rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-0.0.50/src/arkdata/seeds/creatures.json
+-rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-0.0.50/src/arkdata/seeds/dyes.json
+-rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-0.0.50/src/arkdata/seeds/eggs.json
+-rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-0.0.50/src/arkdata/seeds/farms.json
+-rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-0.0.50/src/arkdata/seeds/products.json
+-rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-0.0.50/src/arkdata/seeds/recipes.json
+-rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-0.0.50/src/arkdata/seeds/resources.json
+-rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-0.0.50/src/arkdata/seeds/saddles.json
+-rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-0.0.50/src/arkdata/seeds/seeds.json
+-rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-0.0.50/src/arkdata/seeds/skins.json
+-rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-0.0.50/src/arkdata/seeds/structures.json
+-rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-0.0.50/src/arkdata/seeds/tools.json
+-rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-0.0.50/src/arkdata/seeds/trophies.json
+-rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-0.0.50/src/arkdata/seeds/users.json
+-rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-0.0.50/src/arkdata/seeds/weapons.json
+drwxrwxrwx   0        0        0        0 2023-04-11 02:30:19.618352 arkdata-0.0.50/src/arkdata.egg-info/
+-rw-rw-rw-   0        0        0      804 2023-04-11 02:30:19.000000 arkdata-0.0.50/src/arkdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1948 2023-04-11 02:30:19.000000 arkdata-0.0.50/src/arkdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 02:30:19.000000 arkdata-0.0.50/src/arkdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-04-11 02:30:19.000000 arkdata-0.0.50/src/arkdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 02:30:19.000000 arkdata-0.0.50/src/arkdata.egg-info/top_level.txt
```

### Comparing `arkdata-0.0.49/LICENSE` & `arkdata-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/PKG-INFO` & `arkdata-0.0.50/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 0.0.49
+Version: 0.0.50
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `arkdata-0.0.49/pyproject.toml` & `arkdata-0.0.50/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/setup.cfg` & `arkdata-0.0.50/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6461 7461 0d0a 7665 7273   = arkdata..vers
-00000020: 696f 6e20 3d20 302e 302e 3439 0d0a 6175  ion = 0.0.49..au
+00000020: 696f 6e20 3d20 302e 302e 3530 0d0a 6175  ion = 0.0.50..au
 00000030: 7468 6f72 203d 204d 6175 7269 6369 6f0d  thor = Mauricio.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6465 762e 6d61 7572 6963 696f 2e6c 6f6d  dev.mauricio.lom
 00000060: 656c 6940 676d 6169 6c2e 636f 6d0d 0a64  eli@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2054 6869  escription = Thi
 00000080: 7320 6170 706c 6963 6174 696f 6e20 6163  s application ac
 00000090: 6365 7373 6573 2074 6865 2041 726b 2073  cesses the Ark s
```

### Comparing `arkdata-0.0.49/src/arkdata/database/configuration.py` & `arkdata-0.0.50/src/arkdata/database/configuration.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/database/cursor.py` & `arkdata-0.0.50/src/arkdata/database/cursor.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/database/database.py` & `arkdata-0.0.50/src/arkdata/database/database.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/database/table.py` & `arkdata-0.0.50/src/arkdata/database/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,23 @@
     @classmethod
     def length(cls):
         with sqlalchemy.app_context():
             return sqlalchemy.db.session.query(cls).count()
 
     @classmethod
     def bulk_insert(cls, values: list):
-        return [cls(**kwargs).create() for kwargs in values]
+        with sqlalchemy.app_context():
+            items = []
+            for kwargs in values:
+                record = cls(**kwargs)
+                sqlalchemy.db.session.add(record)
+                items.append(record)
+            sqlalchemy.db.session.commit()
+            ids = [r.id for r in items]
+            return sqlalchemy.db.session.query(cls).filter(cls.id.in_(ids)).all()
 
     @classmethod
     def bulk_delete(cls, items: list):
         with sqlalchemy.app_context():
             for item in items:
                 sqlalchemy.db.session.delete(item)
             sqlalchemy.db.session.commit()
```

### Comparing `arkdata-0.0.49/src/arkdata/models/__init__.py` & `arkdata-0.0.50/src/arkdata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/account.py` & `arkdata-0.0.50/src/arkdata/models/account.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/ammunition.py` & `arkdata-0.0.50/src/arkdata/models/ammunition.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/armour.py` & `arkdata-0.0.50/src/arkdata/models/armour.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/artifact.py` & `arkdata-0.0.50/src/arkdata/models/artifact.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/attachment.py` & `arkdata-0.0.50/src/arkdata/models/attachment.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/cart_item.py` & `arkdata-0.0.50/src/arkdata/models/cart_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/command.py` & `arkdata-0.0.50/src/arkdata/models/command.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/consumable.py` & `arkdata-0.0.50/src/arkdata/models/consumable.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/creature.py` & `arkdata-0.0.50/src/arkdata/models/creature.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/dye.py` & `arkdata-0.0.50/src/arkdata/models/dye.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/egg.py` & `arkdata-0.0.50/src/arkdata/models/egg.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/farm.py` & `arkdata-0.0.50/src/arkdata/models/farm.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/order_item.py` & `arkdata-0.0.50/src/arkdata/models/order_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/product.py` & `arkdata-0.0.50/src/arkdata/models/product.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/recipe.py` & `arkdata-0.0.50/src/arkdata/models/recipe.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/resource.py` & `arkdata-0.0.50/src/arkdata/models/resource.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/saddle.py` & `arkdata-0.0.50/src/arkdata/models/saddle.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/seed.py` & `arkdata-0.0.50/src/arkdata/models/seed.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/server.py` & `arkdata-0.0.50/src/arkdata/models/server.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/sessions.py` & `arkdata-0.0.50/src/arkdata/models/sessions.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/skin.py` & `arkdata-0.0.50/src/arkdata/models/skin.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/structure.py` & `arkdata-0.0.50/src/arkdata/models/structure.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/tool.py` & `arkdata-0.0.50/src/arkdata/models/tool.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/trophy.py` & `arkdata-0.0.50/src/arkdata/models/trophy.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/user.py` & `arkdata-0.0.50/src/arkdata/models/user.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/models/weapon.py` & `arkdata-0.0.50/src/arkdata/models/weapon.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/accounts.json` & `arkdata-0.0.50/src/arkdata/seeds/accounts.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/ammunitions.json` & `arkdata-0.0.50/src/arkdata/seeds/ammunitions.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/armours.json` & `arkdata-0.0.50/src/arkdata/seeds/armours.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/artifacts.json` & `arkdata-0.0.50/src/arkdata/seeds/artifacts.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/attachments.json` & `arkdata-0.0.50/src/arkdata/seeds/attachments.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/commands.json` & `arkdata-0.0.50/src/arkdata/seeds/commands.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/consumables.json` & `arkdata-0.0.50/src/arkdata/seeds/consumables.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/creatures.json` & `arkdata-0.0.50/src/arkdata/seeds/creatures.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/dyes.json` & `arkdata-0.0.50/src/arkdata/seeds/dyes.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/eggs.json` & `arkdata-0.0.50/src/arkdata/seeds/eggs.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/farms.json` & `arkdata-0.0.50/src/arkdata/seeds/farms.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/products.json` & `arkdata-0.0.50/src/arkdata/seeds/products.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/recipes.json` & `arkdata-0.0.50/src/arkdata/seeds/recipes.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/resources.json` & `arkdata-0.0.50/src/arkdata/seeds/resources.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/saddles.json` & `arkdata-0.0.50/src/arkdata/seeds/saddles.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/seeds.json` & `arkdata-0.0.50/src/arkdata/seeds/seeds.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/skins.json` & `arkdata-0.0.50/src/arkdata/seeds/skins.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/structures.json` & `arkdata-0.0.50/src/arkdata/seeds/structures.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/tools.json` & `arkdata-0.0.50/src/arkdata/seeds/tools.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/trophies.json` & `arkdata-0.0.50/src/arkdata/seeds/trophies.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/users.json` & `arkdata-0.0.50/src/arkdata/seeds/users.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata/seeds/weapons.json` & `arkdata-0.0.50/src/arkdata/seeds/weapons.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.49/src/arkdata.egg-info/PKG-INFO` & `arkdata-0.0.50/src/arkdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 0.0.49
+Version: 0.0.50
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `arkdata-0.0.49/src/arkdata.egg-info/SOURCES.txt` & `arkdata-0.0.50/src/arkdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

