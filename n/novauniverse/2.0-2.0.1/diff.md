# Comparing `tmp/novauniverse-2.0.tar.gz` & `tmp/novauniverse-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novauniverse-2.0.tar", last modified: Wed Mar 22 18:21:12 2023, max compression
+gzip compressed data, was "novauniverse-2.0.1.tar", last modified: Tue Apr 11 06:16:47 2023, max compression
```

## Comparing `novauniverse-2.0.tar` & `novauniverse-2.0.1.tar`

### file list

```diff
@@ -1,88 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.127647 novauniverse-2.0/
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:11.955572 novauniverse-2.0/.github/
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:11.985420 novauniverse-2.0/.github/workflows/
--rw-rw-rw-   0        0        0      695 2023-03-21 20:38:29.000000 novauniverse-2.0/.github/workflows/documentation.yaml
--rw-rw-rw-   0        0        0       50 2023-03-21 20:18:52.000000 novauniverse-2.0/.gitignore
--rw-rw-rw-   0        0        0     1228 2023-03-22 18:04:31.000000 novauniverse-2.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0      161 2023-03-22 18:20:14.000000 novauniverse-2.0/Makefile
--rw-rw-rw-   0        0        0     3101 2023-03-22 18:21:12.126648 novauniverse-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2064 2023-03-22 17:35:04.000000 novauniverse-2.0/README.md
--rw-rw-rw-   0        0        0       82 2023-03-21 20:18:52.000000 novauniverse-2.0/demo.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.012119 novauniverse-2.0/docs/
--rw-rw-rw-   0        0        0      654 2023-03-21 20:18:52.000000 novauniverse-2.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.014117 novauniverse-2.0/docs/_static/
--rw-rw-rw-   0        0        0  1821311 2023-03-21 20:18:52.000000 novauniverse-2.0/docs/_static/logo.png
--rw-rw-rw-   0        0        0      728 2023-03-22 17:20:14.000000 novauniverse-2.0/docs/api.rst
--rw-rw-rw-   0        0        0     2539 2023-03-22 17:20:14.000000 novauniverse-2.0/docs/conf.py
--rw-rw-rw-   0        0        0     1189 2023-03-22 17:55:36.000000 novauniverse-2.0/docs/events.rst
--rw-rw-rw-   0        0        0     3347 2023-03-22 17:55:20.000000 novauniverse-2.0/docs/index.rst
--rw-rw-rw-   0        0        0     3548 2023-03-22 17:20:14.000000 novauniverse-2.0/docs/interfaces.rst
--rw-rw-rw-   0        0        0      398 2023-03-21 20:18:52.000000 novauniverse-2.0/docs/interfaces.stats.discord.rst
--rw-rw-rw-   0        0        0     1449 2023-03-21 20:18:52.000000 novauniverse-2.0/docs/interfaces.stats.server.rst
--rwxrwxrwx   0        0        0      800 2023-03-21 20:18:52.000000 novauniverse-2.0/docs/make.bat
--rw-rw-rw-   0        0        0      787 2023-03-22 17:20:14.000000 novauniverse-2.0/docs/objects.rst
--rw-rw-rw-   0        0        0      484 2023-03-21 20:18:52.000000 novauniverse-2.0/docs/objects.tournaments.rst
--rw-rw-rw-   0        0        0      247 2023-03-22 17:20:14.000000 novauniverse-2.0/docs/utils.rst
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.027116 novauniverse-2.0/novauniverse/
--rw-rw-rw-   0        0        0     1784 2023-03-22 17:55:03.000000 novauniverse-2.0/novauniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.062116 novauniverse-2.0/novauniverse/api/
--rw-rw-rw-   0        0        0     2799 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/api/__init__.py
--rw-rw-rw-   0        0        0     1874 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/api/cdn.py
--rw-rw-rw-   0        0        0     1822 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/api/endpoints.py
--rw-rw-rw-   0        0        0     1135 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/api/errors.py
--rw-rw-rw-   0        0        0      554 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/configuration.py
--rw-rw-rw-   0        0        0      417 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/errors.py
--rw-rw-rw-   0        0        0     4104 2023-03-22 17:20:14.000000 novauniverse-2.0/novauniverse/event_client.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.069648 novauniverse-2.0/novauniverse/events/
--rw-rw-rw-   0        0        0     3877 2023-03-22 17:20:14.000000 novauniverse-2.0/novauniverse/events/__init__.py
--rw-rw-rw-   0        0        0      494 2023-03-22 17:20:14.000000 novauniverse-2.0/novauniverse/events/client_ready.py
--rw-rw-rw-   0        0        0     1162 2023-03-22 17:20:14.000000 novauniverse-2.0/novauniverse/events/player_join.py
--rw-rw-rw-   0        0        0     1045 2023-03-22 17:20:14.000000 novauniverse-2.0/novauniverse/events/player_leave.py
--rw-rw-rw-   0        0        0      352 2023-03-22 18:18:29.000000 novauniverse-2.0/novauniverse/info.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.071649 novauniverse-2.0/novauniverse/interfaces/
--rw-rw-rw-   0        0        0     1945 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.075649 novauniverse-2.0/novauniverse/interfaces/mcf/
--rw-rw-rw-   0        0        0     2811 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/mcf/__init__.py
--rw-rw-rw-   0        0        0      194 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/mcf/mcf_tournament.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.077646 novauniverse-2.0/novauniverse/interfaces/stats/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.081649 novauniverse-2.0/novauniverse/interfaces/stats/discord/
--rw-rw-rw-   0        0        0      541 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/discord/__init__.py
--rw-rw-rw-   0        0        0      781 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/discord/discord_stats.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.096648 novauniverse-2.0/novauniverse/interfaces/stats/server/
--rw-rw-rw-   0        0        0     1024 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/server/__init__.py
--rw-rw-rw-   0        0        0      551 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/server/global_.py
--rw-rw-rw-   0        0        0     1001 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/server/nova_online_player.py
--rw-rw-rw-   0        0        0     1022 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/server/nova_server.py
--rw-rw-rw-   0        0        0      666 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/server/player_preview.py
--rw-rw-rw-   0        0        0     1926 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/server/server_info.py
--rw-rw-rw-   0        0        0      344 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/interfaces/stats/server/system.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.105648 novauniverse-2.0/novauniverse/objects/
--rw-rw-rw-   0        0        0      337 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/objects/__init__.py
--rw-rw-rw-   0        0        0     1018 2023-03-22 14:57:55.000000 novauniverse-2.0/novauniverse/objects/nova_dataclass.py
--rw-rw-rw-   0        0        0      653 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/objects/nova_player.py
--rw-rw-rw-   0        0        0      355 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/objects/order_by.py
--rw-rw-rw-   0        0        0      798 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/objects/timestamp.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.111648 novauniverse-2.0/novauniverse/objects/tournaments/
--rw-rw-rw-   0        0        0     1697 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/objects/tournaments/__init__.py
--rw-rw-rw-   0        0        0      975 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/objects/tournaments/tournament_player.py
--rw-rw-rw-   0        0        0      906 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/objects/tournaments/tournament_team.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.115649 novauniverse-2.0/novauniverse/utils/
--rw-rw-rw-   0        0        0       36 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/utils/__init__.py
--rw-rw-rw-   0        0        0     1657 2023-03-21 20:18:52.000000 novauniverse-2.0/novauniverse/utils/search.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.054118 novauniverse-2.0/novauniverse.egg-info/
--rw-rw-rw-   0        0        0     3101 2023-03-22 18:21:11.000000 novauniverse-2.0/novauniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2090 2023-03-22 18:21:11.000000 novauniverse-2.0/novauniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 18:21:11.000000 novauniverse-2.0/novauniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2023-03-22 18:21:11.000000 novauniverse-2.0/novauniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-22 18:21:11.000000 novauniverse-2.0/novauniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1589 2023-03-22 18:15:20.000000 novauniverse-2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-22 18:21:12.127647 novauniverse-2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.117646 novauniverse-2.0/tests/
--rw-rw-rw-   0        0        0       66 2023-03-21 20:18:52.000000 novauniverse-2.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.119645 novauniverse-2.0/tests/interfaces/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0/tests/interfaces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 18:21:12.124648 novauniverse-2.0/tests/interfaces/stats/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0/tests/interfaces/stats/__init__.py
--rw-rw-rw-   0        0        0      275 2023-03-21 20:18:52.000000 novauniverse-2.0/tests/interfaces/stats/test_discord.py
--rw-rw-rw-   0        0        0      846 2023-03-21 20:18:52.000000 novauniverse-2.0/tests/interfaces/stats/test_server.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.569648 novauniverse-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.366649 novauniverse-2.0.1/.github/
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.393644 novauniverse-2.0.1/.github/workflows/
+-rw-rw-rw-   0        0        0      830 2023-03-22 19:01:49.000000 novauniverse-2.0.1/.github/workflows/documentation.yaml
+-rw-rw-rw-   0        0        0       68 2023-03-22 18:30:58.000000 novauniverse-2.0.1/.gitignore
+-rw-rw-rw-   0        0        0     1228 2023-03-22 18:04:31.000000 novauniverse-2.0.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0      161 2023-03-22 18:20:14.000000 novauniverse-2.0.1/Makefile
+-rw-rw-rw-   0        0        0     3136 2023-04-11 06:16:47.568642 novauniverse-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2091 2023-03-24 17:08:14.000000 novauniverse-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.451644 novauniverse-2.0.1/docs/
+-rw-rw-rw-   0        0        0      654 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.453645 novauniverse-2.0.1/docs/_static/
+-rw-rw-rw-   0        0        0  1821311 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/_static/logo.png
+-rw-rw-rw-   0        0        0      728 2023-03-22 17:20:14.000000 novauniverse-2.0.1/docs/api.rst
+-rw-rw-rw-   0        0        0     1545 2023-03-22 19:18:54.000000 novauniverse-2.0.1/docs/conf.py
+-rw-rw-rw-   0        0        0     1189 2023-03-22 17:55:36.000000 novauniverse-2.0.1/docs/events.rst
+-rw-rw-rw-   0        0        0     3301 2023-03-22 19:02:01.000000 novauniverse-2.0.1/docs/index.rst
+-rw-rw-rw-   0        0        0     3548 2023-03-22 17:20:14.000000 novauniverse-2.0.1/docs/interfaces.rst
+-rw-rw-rw-   0        0        0      398 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/interfaces.stats.discord.rst
+-rw-rw-rw-   0        0        0     1449 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/interfaces.stats.server.rst
+-rwxrwxrwx   0        0        0      800 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/make.bat
+-rw-rw-rw-   0        0        0      787 2023-03-22 17:20:14.000000 novauniverse-2.0.1/docs/objects.rst
+-rw-rw-rw-   0        0        0      484 2023-03-21 20:18:52.000000 novauniverse-2.0.1/docs/objects.tournaments.rst
+-rw-rw-rw-   0        0        0      247 2023-03-22 17:20:14.000000 novauniverse-2.0.1/docs/utils.rst
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.466642 novauniverse-2.0.1/novauniverse/
+-rw-rw-rw-   0        0        0     1803 2023-04-11 06:12:05.000000 novauniverse-2.0.1/novauniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.503644 novauniverse-2.0.1/novauniverse/api/
+-rw-rw-rw-   0        0        0     2799 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/api/__init__.py
+-rw-rw-rw-   0        0        0     1874 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/api/cdn.py
+-rw-rw-rw-   0        0        0     1822 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/api/endpoints.py
+-rw-rw-rw-   0        0        0     1135 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/api/errors.py
+-rw-rw-rw-   0        0        0      554 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/configuration.py
+-rw-rw-rw-   0        0        0      417 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/errors.py
+-rw-rw-rw-   0        0        0     4104 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/event_client.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.511641 novauniverse-2.0.1/novauniverse/events/
+-rw-rw-rw-   0        0        0     3877 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/events/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/events/client_ready.py
+-rw-rw-rw-   0        0        0     1162 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/events/player_join.py
+-rw-rw-rw-   0        0        0     1045 2023-03-22 17:20:14.000000 novauniverse-2.0.1/novauniverse/events/player_leave.py
+-rw-rw-rw-   0        0        0      356 2023-04-11 06:16:05.000000 novauniverse-2.0.1/novauniverse/info.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.513643 novauniverse-2.0.1/novauniverse/interfaces/
+-rw-rw-rw-   0        0        0     1945 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.516643 novauniverse-2.0.1/novauniverse/interfaces/mcf/
+-rw-rw-rw-   0        0        0     2811 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/mcf/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/mcf/mcf_tournament.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.518642 novauniverse-2.0.1/novauniverse/interfaces/stats/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.523643 novauniverse-2.0.1/novauniverse/interfaces/stats/discord/
+-rw-rw-rw-   0        0        0      541 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/discord/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/discord/discord_stats.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.537644 novauniverse-2.0.1/novauniverse/interfaces/stats/server/
+-rw-rw-rw-   0        0        0     1024 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/__init__.py
+-rw-rw-rw-   0        0        0      551 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/global_.py
+-rw-rw-rw-   0        0        0     1001 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/nova_online_player.py
+-rw-rw-rw-   0        0        0     1022 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/nova_server.py
+-rw-rw-rw-   0        0        0      666 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/player_preview.py
+-rw-rw-rw-   0        0        0     1926 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/server_info.py
+-rw-rw-rw-   0        0        0      344 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/interfaces/stats/server/system.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.547646 novauniverse-2.0.1/novauniverse/objects/
+-rw-rw-rw-   0        0        0      337 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/__init__.py
+-rw-rw-rw-   0        0        0     1018 2023-03-22 14:57:55.000000 novauniverse-2.0.1/novauniverse/objects/nova_dataclass.py
+-rw-rw-rw-   0        0        0      653 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/nova_player.py
+-rw-rw-rw-   0        0        0      355 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/order_by.py
+-rw-rw-rw-   0        0        0      798 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/timestamp.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.553646 novauniverse-2.0.1/novauniverse/objects/tournaments/
+-rw-rw-rw-   0        0        0     1697 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/tournaments/__init__.py
+-rw-rw-rw-   0        0        0      975 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/tournaments/tournament_player.py
+-rw-rw-rw-   0        0        0      906 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/objects/tournaments/tournament_team.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.557644 novauniverse-2.0.1/novauniverse/utils/
+-rw-rw-rw-   0        0        0       36 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1657 2023-03-21 20:18:52.000000 novauniverse-2.0.1/novauniverse/utils/search.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.495655 novauniverse-2.0.1/novauniverse.egg-info/
+-rw-rw-rw-   0        0        0     3136 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 06:16:47.000000 novauniverse-2.0.1/novauniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1597 2023-04-11 06:07:36.000000 novauniverse-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 06:16:47.569648 novauniverse-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.559646 novauniverse-2.0.1/tests/
+-rw-rw-rw-   0        0        0       66 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.561643 novauniverse-2.0.1/tests/interfaces/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/interfaces/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 06:16:47.566641 novauniverse-2.0.1/tests/interfaces/stats/
+-rw-rw-rw-   0        0        0        0 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/interfaces/stats/__init__.py
+-rw-rw-rw-   0        0        0      275 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/interfaces/stats/test_discord.py
+-rw-rw-rw-   0        0        0      846 2023-03-21 20:18:52.000000 novauniverse-2.0.1/tests/interfaces/stats/test_server.py
```

### Comparing `novauniverse-2.0/.github/workflows/documentation.yaml` & `novauniverse-2.0.1/.github/workflows/documentation.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -6,18 +6,22 @@
   docs:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v3
       - name: Install dependencies
         run: |
-          pip install .
+          pip install .[dev]
       - name: Sphinx build
         run: |
           sphinx-build docs _build
+      - name: Download CNAME file from API.
+        run: |
+          cd _build && wget "https://api.devgoldy.me/stash/CNAME"
+
       - name: Deploy
         uses: peaceiris/actions-gh-pages@v3
         if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
         with:
           publish_branch: gh-pages
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: _build/
```

### Comparing `novauniverse-2.0/CHANGELOG.rst` & `novauniverse-2.0.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/PKG-INFO` & `novauniverse-2.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 Metadata-Version: 2.1
 Name: novauniverse
-Version: 2.0
+Version: 2.0.1
 Summary: A modern & maintained wrapper for the Nova Universe API written in 🐍 Python.
 Author-email: Goldy <goldy@devgoldy.me>
 Project-URL: GitHub, https://github.com/NovaUniverse/NovaUniverse.py
 Project-URL: BugTracker, https://github.com/NovaUniverse/NovaUniverse.py/issues
-Project-URL: ChangeLog, https://github.com/NovaUniverse/NovaUniverse.py/v2/CHANGELOG.md
+Project-URL: ChangeLog, https://github.com/NovaUniverse/NovaUniverse.py/blob/main/CHANGELOG.rst
 Keywords: novauniverse,minecraft novauniverse,nova universe,mc novauniverse
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-[![Discord Shield](https://discordapp.com/api/guilds/692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7)
-[![PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/project/novauniverse/)
-[![Python Badge](https://img.shields.io/pypi/pyversions/novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported python versions.")
-[![Docs Badge](https://img.shields.io/static/v1?label=docs&message=Available&color=light-green)](https://nupy.devgoldy.me/)
+<div align="center">
 
-<p align="center">
- <img src="https://user-images.githubusercontent.com/66202304/147414615-4a410681-0e02-41e3-88cd-3d28d4bf6898.png" width="500" />
-</p>
-
-### 🐍[``novauniverse.py``](https://pypi.org/project/novauniverse/) - A modern & maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/) written in Python.
+  # 🐍[``novauniverse.py``](https://pypi.org/project/novauniverse/)
+  
+  <sub>A modern & maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/) written in Python.</sub>
+  
+  [![Discord Shield](https://discordapp.com/api/guilds/692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7)
+  [![PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/project/novauniverse/)
+  [![Python Badge](https://img.shields.io/pypi/pyversions/novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported python versions.")
+  [![Docs Badge](https://img.shields.io/github/actions/workflow/status/NovaUniverse/NovaUniverse.py/documentation.yaml?label=docs)](https://nupy.devgoldy.me/)
+  
+</div>
 
-#### ℹ Notice: 2.0 is currently in development so not all api endpoints are implemented.
+> #### ℹ Notice: 2.0 is currently in development so not all api endpoints are implemented.
 
 <p align="right">
  <img align="left" src="https://raw.githubusercontent.com/NovaUniverse/NovaUniverse.py/main/docs/_static/logo.png" width="180" />
  
  <h2>What is Nova Universe.py?</h2>
- NovaUniverse.py is a API wrapper for the minecraft server <a href="https://novauniverse.net/">Nova Universe</a> that allows you to access the Nova Universe <a href="https://novauniverse.net/api">API</a> in a fast object oriented way in Python. One of the bonuses is that it was developed by one of the devs at NovaUniverse.
+ NovaUniverse.py is an API wrapper for “<a href="https://novauniverse.net/">Nova Universe</a>” (a minecraft event hosting group) that allows you to interface with the <a href="https://novauniverse.net/api">Nova Universe API</a> in a fast object oriented way natively within Python. One of the bonuses is that it was developed by <a href="https://github.com/THEGOLDENPRO">ME</a>, an admin at NovaUniverse.
 </p>
 
 <br>
 
 ## *Install/Set Up*
 1. **Install package from pypi.**
 ```sh
 #Windows/Linux
 
 pip install novauniverse
 ```
 2. **That's It!** - *Brief Example Below*
 ```python
-from novauniverse import NovaClient, Events, NovaOnlinePlayer 
+from novauniverse import EventClient, Events, NovaOnlinePlayer 
 
-client = NovaClient()
+client = EventClient()
 
 @client.on_event(Events.CLIENT_READY)
 def client_is_ready():
     print("Client is ready!")
 
 @client.on_event(Events.PLAYER_JOIN)
 def on_player_join(player:NovaOnlinePlayer):
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: novauniverse Version: 2.0 Summary: A modern &
+Metadata-Version: 2.1 Name: novauniverse Version: 2.0.1 Summary: A modern &
 maintained wrapper for the Nova Universe API written in ð Python. Author-
 email: Goldy
 devgoldy.me> Project-URL: GitHub, https://github.com/NovaUniverse/
 NovaUniverse.py Project-URL: BugTracker, https://github.com/NovaUniverse/
 NovaUniverse.py/issues Project-URL: ChangeLog, https://github.com/NovaUniverse/
-NovaUniverse.py/v2/CHANGELOG.md Keywords: novauniverse,minecraft
+NovaUniverse.py/blob/main/CHANGELOG.rst Keywords: novauniverse,minecraft
 novauniverse,nova universe,mc novauniverse Classifier: Operating System ::
 Microsoft :: Windows :: Windows 11 Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev [![Discord Shield](https://discordapp.com/
-api/guilds/692764975902752871/widget.png?style=shield)](https://discord.gg/
-4gZSVJ7) [![PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://
-pypi.org/project/novauniverse/) [![Python Badge](https://img.shields.io/pypi/
-pyversions/novauniverse?style=flat)](https://pypi.org/project/novauniverse/
-"Supported python versions.") [![Docs Badge](https://img.shields.io/static/
-v1?label=docs&message=Available&color=light-green)](https://nupy.devgoldy.me/)
- [https://user-images.githubusercontent.com/66202304/147414615-4a410681-0e02-
-                          41e3-88cd-3d28d4bf6898.png]
-### ð[``novauniverse.py``](https://pypi.org/project/novauniverse/) - A
-modern & maintained wrapper for the [Nova Universe API](https://
-novauniverse.net/api/) written in Python. #### â¹ Notice: 2.0 is currently in
-development so not all api endpoints are implemented.
+text/markdown Provides-Extra: dev
+# ð[``novauniverse.py``](https://pypi.org/project/novauniverse/) A modern &
+ maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/
+  ) written in Python. [![Discord Shield](https://discordapp.com/api/guilds/
+  692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7) [!
+ [PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/
+project/novauniverse/) [![Python Badge](https://img.shields.io/pypi/pyversions/
+  novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported
+   python versions.") [![Docs Badge](https://img.shields.io/github/actions/
+ workflow/status/NovaUniverse/NovaUniverse.py/documentation.yaml?label=docs)]
+                          (https://nupy.devgoldy.me/)
+> #### â¹ Notice: 2.0 is currently in development so not all api endpoints are
+implemented.
      [https://raw.githubusercontent.com/NovaUniverse/NovaUniverse.py/main/docs/
                                                               _static/logo.png]
 ***** What is Nova Universe.py? *****
-NovaUniverse.py is a API wrapper for the minecraft server Nova_Universe that
-allows you to access the Nova Universe API in a fast object oriented way in
-Python. One of the bonuses is that it was developed by one of the devs at
-NovaUniverse.
+NovaUniverse.py is an API wrapper for âNova_Universeâ (a minecraft event
+hosting group) that allows you to interface with the Nova_Universe_API in a
+fast object oriented way natively within Python. One of the bonuses is that it
+was developed by ME, an admin at NovaUniverse.
 
 ## *Install/Set Up* 1. **Install package from pypi.** ```sh #Windows/Linux pip
 install novauniverse ``` 2. **That's It!** - *Brief Example Below* ```python
-from novauniverse import NovaClient, Events, NovaOnlinePlayer client =
-NovaClient() @client.on_event(Events.CLIENT_READY) def client_is_ready(): print
-("Client is ready!") @client.on_event(Events.PLAYER_JOIN) def on_player_join
-(player:NovaOnlinePlayer): print(f"{player.username} joined
+from novauniverse import EventClient, Events, NovaOnlinePlayer client =
+EventClient() @client.on_event(Events.CLIENT_READY) def client_is_ready():
+print("Client is ready!") @client.on_event(Events.PLAYER_JOIN) def
+on_player_join(player:NovaOnlinePlayer): print(f"{player.username} joined
 {player.server_name}!") client.start() ```
 > ### More Examples and Info at https://nupy.devgoldy.me/
```

### Comparing `novauniverse-2.0/README.md` & `novauniverse-2.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-[![Discord Shield](https://discordapp.com/api/guilds/692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7)
-[![PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/project/novauniverse/)
-[![Python Badge](https://img.shields.io/pypi/pyversions/novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported python versions.")
-[![Docs Badge](https://img.shields.io/static/v1?label=docs&message=Available&color=light-green)](https://nupy.devgoldy.me/)
+<div align="center">
 
-<p align="center">
- <img src="https://user-images.githubusercontent.com/66202304/147414615-4a410681-0e02-41e3-88cd-3d28d4bf6898.png" width="500" />
-</p>
-
-### 🐍[``novauniverse.py``](https://pypi.org/project/novauniverse/) - A modern & maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/) written in Python.
+  # 🐍[``novauniverse.py``](https://pypi.org/project/novauniverse/)
+  
+  <sub>A modern & maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/) written in Python.</sub>
+  
+  [![Discord Shield](https://discordapp.com/api/guilds/692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7)
+  [![PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/project/novauniverse/)
+  [![Python Badge](https://img.shields.io/pypi/pyversions/novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported python versions.")
+  [![Docs Badge](https://img.shields.io/github/actions/workflow/status/NovaUniverse/NovaUniverse.py/documentation.yaml?label=docs)](https://nupy.devgoldy.me/)
+  
+</div>
 
-#### ℹ Notice: 2.0 is currently in development so not all api endpoints are implemented.
+> #### ℹ Notice: 2.0 is currently in development so not all api endpoints are implemented.
 
 <p align="right">
  <img align="left" src="https://raw.githubusercontent.com/NovaUniverse/NovaUniverse.py/main/docs/_static/logo.png" width="180" />
  
  <h2>What is Nova Universe.py?</h2>
- NovaUniverse.py is a API wrapper for the minecraft server <a href="https://novauniverse.net/">Nova Universe</a> that allows you to access the Nova Universe <a href="https://novauniverse.net/api">API</a> in a fast object oriented way in Python. One of the bonuses is that it was developed by one of the devs at NovaUniverse.
+ NovaUniverse.py is an API wrapper for “<a href="https://novauniverse.net/">Nova Universe</a>” (a minecraft event hosting group) that allows you to interface with the <a href="https://novauniverse.net/api">Nova Universe API</a> in a fast object oriented way natively within Python. One of the bonuses is that it was developed by <a href="https://github.com/THEGOLDENPRO">ME</a>, an admin at NovaUniverse.
 </p>
 
 <br>
 
 ## *Install/Set Up*
 1. **Install package from pypi.**
 ```sh
 #Windows/Linux
 
 pip install novauniverse
 ```
 2. **That's It!** - *Brief Example Below*
 ```python
-from novauniverse import NovaClient, Events, NovaOnlinePlayer 
+from novauniverse import EventClient, Events, NovaOnlinePlayer 
 
-client = NovaClient()
+client = EventClient()
 
 @client.on_event(Events.CLIENT_READY)
 def client_is_ready():
     print("Client is ready!")
 
 @client.on_event(Events.PLAYER_JOIN)
 def on_player_join(player:NovaOnlinePlayer):
     print(f"{player.username} joined {player.server_name}!")
 
 client.start()
 ```
 
 <br>
 
-> ### More Examples and Info at https://nupy.devgoldy.me/
+> ### More Examples and Info at https://nupy.devgoldy.me/
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-[![Discord Shield](https://discordapp.com/api/guilds/692764975902752871/
-widget.png?style=shield)](https://discord.gg/4gZSVJ7) [![PyPI version](https://
-badge.fury.io/py/novauniverse.svg)](https://pypi.org/project/novauniverse/) [!
-[Python Badge](https://img.shields.io/pypi/pyversions/novauniverse?style=flat)]
-(https://pypi.org/project/novauniverse/ "Supported python versions.") [![Docs
-Badge](https://img.shields.io/static/
-v1?label=docs&message=Available&color=light-green)](https://nupy.devgoldy.me/)
- [https://user-images.githubusercontent.com/66202304/147414615-4a410681-0e02-
-                          41e3-88cd-3d28d4bf6898.png]
-### ð[``novauniverse.py``](https://pypi.org/project/novauniverse/) - A
-modern & maintained wrapper for the [Nova Universe API](https://
-novauniverse.net/api/) written in Python. #### â¹ Notice: 2.0 is currently in
-development so not all api endpoints are implemented.
+# ð[``novauniverse.py``](https://pypi.org/project/novauniverse/) A modern &
+ maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/
+  ) written in Python. [![Discord Shield](https://discordapp.com/api/guilds/
+  692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7) [!
+ [PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/
+project/novauniverse/) [![Python Badge](https://img.shields.io/pypi/pyversions/
+  novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported
+   python versions.") [![Docs Badge](https://img.shields.io/github/actions/
+ workflow/status/NovaUniverse/NovaUniverse.py/documentation.yaml?label=docs)]
+                          (https://nupy.devgoldy.me/)
+> #### â¹ Notice: 2.0 is currently in development so not all api endpoints are
+implemented.
      [https://raw.githubusercontent.com/NovaUniverse/NovaUniverse.py/main/docs/
                                                               _static/logo.png]
 ***** What is Nova Universe.py? *****
-NovaUniverse.py is a API wrapper for the minecraft server Nova_Universe that
-allows you to access the Nova Universe API in a fast object oriented way in
-Python. One of the bonuses is that it was developed by one of the devs at
-NovaUniverse.
+NovaUniverse.py is an API wrapper for âNova_Universeâ (a minecraft event
+hosting group) that allows you to interface with the Nova_Universe_API in a
+fast object oriented way natively within Python. One of the bonuses is that it
+was developed by ME, an admin at NovaUniverse.
 
 ## *Install/Set Up* 1. **Install package from pypi.** ```sh #Windows/Linux pip
 install novauniverse ``` 2. **That's It!** - *Brief Example Below* ```python
-from novauniverse import NovaClient, Events, NovaOnlinePlayer client =
-NovaClient() @client.on_event(Events.CLIENT_READY) def client_is_ready(): print
-("Client is ready!") @client.on_event(Events.PLAYER_JOIN) def on_player_join
-(player:NovaOnlinePlayer): print(f"{player.username} joined
+from novauniverse import EventClient, Events, NovaOnlinePlayer client =
+EventClient() @client.on_event(Events.CLIENT_READY) def client_is_ready():
+print("Client is ready!") @client.on_event(Events.PLAYER_JOIN) def
+on_player_join(player:NovaOnlinePlayer): print(f"{player.username} joined
 {player.server_name}!") client.start() ```
 > ### More Examples and Info at https://nupy.devgoldy.me/
```

### Comparing `novauniverse-2.0/docs/Makefile` & `novauniverse-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/docs/_static/logo.png` & `novauniverse-2.0.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/docs/api.rst` & `novauniverse-2.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/docs/events.rst` & `novauniverse-2.0.1/docs/events.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/docs/index.rst` & `novauniverse-2.0.1/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ⚙ *Install/Set Up:*
 -------------------
 1. **Install package from pypi.** (In development so no PyPi package yet, install via GitHub instead.)::
 
       #Windows/Linux
 
-      pip install git+https://github.com/NovaUniverse/NovaUniverse.py.git@v2
+      pip install novauniverse
 
 2. **That's It!** - *Brief Example Below*::
 
       from novauniverse import EventClient, Events, NovaOnlinePlayer 
 
       client = EventClient()
```

### Comparing `novauniverse-2.0/docs/interfaces.rst` & `novauniverse-2.0.1/docs/interfaces.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/docs/interfaces.stats.server.rst` & `novauniverse-2.0.1/docs/interfaces.stats.server.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/docs/make.bat` & `novauniverse-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/docs/objects.rst` & `novauniverse-2.0.1/docs/objects.rst`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/__init__.py` & `novauniverse-2.0.1/novauniverse/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 # Logging stuff
 # ---------------
 from .info import LOGGER_NAME
 from devgoldyutils.logging import add_custom_handler, log
 
-nova_logger = add_custom_handler(log.getLogger(LOGGER_NAME))
+nova_logger = add_custom_handler(log.getLogger(LOGGER_NAME), level=log.WARNING)
 """
 The python ``logging.Logger()`` class for NovaUniverse.py.
 
 ---------------
 ### ``Example:``
 
 You can disable and also adjust the level of logging from the api wrapper like this:
```

### Comparing `novauniverse-2.0/novauniverse/api/__init__.py` & `novauniverse-2.0.1/novauniverse/api/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/api/cdn.py` & `novauniverse-2.0.1/novauniverse/api/cdn.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/api/endpoints.py` & `novauniverse-2.0.1/novauniverse/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/api/errors.py` & `novauniverse-2.0.1/novauniverse/api/errors.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/configuration.py` & `novauniverse-2.0.1/novauniverse/configuration.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/event_client.py` & `novauniverse-2.0.1/novauniverse/event_client.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/events/__init__.py` & `novauniverse-2.0.1/novauniverse/events/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/events/player_join.py` & `novauniverse-2.0.1/novauniverse/events/player_join.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/events/player_leave.py` & `novauniverse-2.0.1/novauniverse/events/player_leave.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/__init__.py` & `novauniverse-2.0.1/novauniverse/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/mcf/__init__.py` & `novauniverse-2.0.1/novauniverse/interfaces/mcf/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/stats/discord/__init__.py` & `novauniverse-2.0.1/novauniverse/interfaces/stats/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/stats/discord/discord_stats.py` & `novauniverse-2.0.1/novauniverse/interfaces/stats/discord/discord_stats.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/stats/server/__init__.py` & `novauniverse-2.0.1/novauniverse/interfaces/stats/server/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/stats/server/global_.py` & `novauniverse-2.0.1/novauniverse/interfaces/stats/server/global_.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/stats/server/nova_online_player.py` & `novauniverse-2.0.1/novauniverse/interfaces/stats/server/nova_online_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/stats/server/nova_server.py` & `novauniverse-2.0.1/novauniverse/interfaces/stats/server/nova_server.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/stats/server/player_preview.py` & `novauniverse-2.0.1/novauniverse/interfaces/stats/server/player_preview.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/interfaces/stats/server/server_info.py` & `novauniverse-2.0.1/novauniverse/interfaces/stats/server/server_info.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/objects/nova_dataclass.py` & `novauniverse-2.0.1/novauniverse/objects/nova_dataclass.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/objects/nova_player.py` & `novauniverse-2.0.1/novauniverse/objects/nova_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/objects/timestamp.py` & `novauniverse-2.0.1/novauniverse/objects/timestamp.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/objects/tournaments/__init__.py` & `novauniverse-2.0.1/novauniverse/objects/tournaments/__init__.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/objects/tournaments/tournament_player.py` & `novauniverse-2.0.1/novauniverse/objects/tournaments/tournament_player.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/objects/tournaments/tournament_team.py` & `novauniverse-2.0.1/novauniverse/objects/tournaments/tournament_team.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse/utils/search.py` & `novauniverse-2.0.1/novauniverse/utils/search.py`

 * *Files identical despite different names*

### Comparing `novauniverse-2.0/novauniverse.egg-info/PKG-INFO` & `novauniverse-2.0.1/novauniverse.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 Metadata-Version: 2.1
 Name: novauniverse
-Version: 2.0
+Version: 2.0.1
 Summary: A modern & maintained wrapper for the Nova Universe API written in 🐍 Python.
 Author-email: Goldy <goldy@devgoldy.me>
 Project-URL: GitHub, https://github.com/NovaUniverse/NovaUniverse.py
 Project-URL: BugTracker, https://github.com/NovaUniverse/NovaUniverse.py/issues
-Project-URL: ChangeLog, https://github.com/NovaUniverse/NovaUniverse.py/v2/CHANGELOG.md
+Project-URL: ChangeLog, https://github.com/NovaUniverse/NovaUniverse.py/blob/main/CHANGELOG.rst
 Keywords: novauniverse,minecraft novauniverse,nova universe,mc novauniverse
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-[![Discord Shield](https://discordapp.com/api/guilds/692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7)
-[![PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/project/novauniverse/)
-[![Python Badge](https://img.shields.io/pypi/pyversions/novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported python versions.")
-[![Docs Badge](https://img.shields.io/static/v1?label=docs&message=Available&color=light-green)](https://nupy.devgoldy.me/)
+<div align="center">
 
-<p align="center">
- <img src="https://user-images.githubusercontent.com/66202304/147414615-4a410681-0e02-41e3-88cd-3d28d4bf6898.png" width="500" />
-</p>
-
-### 🐍[``novauniverse.py``](https://pypi.org/project/novauniverse/) - A modern & maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/) written in Python.
+  # 🐍[``novauniverse.py``](https://pypi.org/project/novauniverse/)
+  
+  <sub>A modern & maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/) written in Python.</sub>
+  
+  [![Discord Shield](https://discordapp.com/api/guilds/692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7)
+  [![PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/project/novauniverse/)
+  [![Python Badge](https://img.shields.io/pypi/pyversions/novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported python versions.")
+  [![Docs Badge](https://img.shields.io/github/actions/workflow/status/NovaUniverse/NovaUniverse.py/documentation.yaml?label=docs)](https://nupy.devgoldy.me/)
+  
+</div>
 
-#### ℹ Notice: 2.0 is currently in development so not all api endpoints are implemented.
+> #### ℹ Notice: 2.0 is currently in development so not all api endpoints are implemented.
 
 <p align="right">
  <img align="left" src="https://raw.githubusercontent.com/NovaUniverse/NovaUniverse.py/main/docs/_static/logo.png" width="180" />
  
  <h2>What is Nova Universe.py?</h2>
- NovaUniverse.py is a API wrapper for the minecraft server <a href="https://novauniverse.net/">Nova Universe</a> that allows you to access the Nova Universe <a href="https://novauniverse.net/api">API</a> in a fast object oriented way in Python. One of the bonuses is that it was developed by one of the devs at NovaUniverse.
+ NovaUniverse.py is an API wrapper for “<a href="https://novauniverse.net/">Nova Universe</a>” (a minecraft event hosting group) that allows you to interface with the <a href="https://novauniverse.net/api">Nova Universe API</a> in a fast object oriented way natively within Python. One of the bonuses is that it was developed by <a href="https://github.com/THEGOLDENPRO">ME</a>, an admin at NovaUniverse.
 </p>
 
 <br>
 
 ## *Install/Set Up*
 1. **Install package from pypi.**
 ```sh
 #Windows/Linux
 
 pip install novauniverse
 ```
 2. **That's It!** - *Brief Example Below*
 ```python
-from novauniverse import NovaClient, Events, NovaOnlinePlayer 
+from novauniverse import EventClient, Events, NovaOnlinePlayer 
 
-client = NovaClient()
+client = EventClient()
 
 @client.on_event(Events.CLIENT_READY)
 def client_is_ready():
     print("Client is ready!")
 
 @client.on_event(Events.PLAYER_JOIN)
 def on_player_join(player:NovaOnlinePlayer):
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: novauniverse Version: 2.0 Summary: A modern &
+Metadata-Version: 2.1 Name: novauniverse Version: 2.0.1 Summary: A modern &
 maintained wrapper for the Nova Universe API written in ð Python. Author-
 email: Goldy
 devgoldy.me> Project-URL: GitHub, https://github.com/NovaUniverse/
 NovaUniverse.py Project-URL: BugTracker, https://github.com/NovaUniverse/
 NovaUniverse.py/issues Project-URL: ChangeLog, https://github.com/NovaUniverse/
-NovaUniverse.py/v2/CHANGELOG.md Keywords: novauniverse,minecraft
+NovaUniverse.py/blob/main/CHANGELOG.rst Keywords: novauniverse,minecraft
 novauniverse,nova universe,mc novauniverse Classifier: Operating System ::
 Microsoft :: Windows :: Windows 11 Classifier: Operating System :: Microsoft ::
 Windows :: Windows 10 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev [![Discord Shield](https://discordapp.com/
-api/guilds/692764975902752871/widget.png?style=shield)](https://discord.gg/
-4gZSVJ7) [![PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://
-pypi.org/project/novauniverse/) [![Python Badge](https://img.shields.io/pypi/
-pyversions/novauniverse?style=flat)](https://pypi.org/project/novauniverse/
-"Supported python versions.") [![Docs Badge](https://img.shields.io/static/
-v1?label=docs&message=Available&color=light-green)](https://nupy.devgoldy.me/)
- [https://user-images.githubusercontent.com/66202304/147414615-4a410681-0e02-
-                          41e3-88cd-3d28d4bf6898.png]
-### ð[``novauniverse.py``](https://pypi.org/project/novauniverse/) - A
-modern & maintained wrapper for the [Nova Universe API](https://
-novauniverse.net/api/) written in Python. #### â¹ Notice: 2.0 is currently in
-development so not all api endpoints are implemented.
+text/markdown Provides-Extra: dev
+# ð[``novauniverse.py``](https://pypi.org/project/novauniverse/) A modern &
+ maintained wrapper for the [Nova Universe API](https://novauniverse.net/api/
+  ) written in Python. [![Discord Shield](https://discordapp.com/api/guilds/
+  692764975902752871/widget.png?style=shield)](https://discord.gg/4gZSVJ7) [!
+ [PyPI version](https://badge.fury.io/py/novauniverse.svg)](https://pypi.org/
+project/novauniverse/) [![Python Badge](https://img.shields.io/pypi/pyversions/
+  novauniverse?style=flat)](https://pypi.org/project/novauniverse/ "Supported
+   python versions.") [![Docs Badge](https://img.shields.io/github/actions/
+ workflow/status/NovaUniverse/NovaUniverse.py/documentation.yaml?label=docs)]
+                          (https://nupy.devgoldy.me/)
+> #### â¹ Notice: 2.0 is currently in development so not all api endpoints are
+implemented.
      [https://raw.githubusercontent.com/NovaUniverse/NovaUniverse.py/main/docs/
                                                               _static/logo.png]
 ***** What is Nova Universe.py? *****
-NovaUniverse.py is a API wrapper for the minecraft server Nova_Universe that
-allows you to access the Nova Universe API in a fast object oriented way in
-Python. One of the bonuses is that it was developed by one of the devs at
-NovaUniverse.
+NovaUniverse.py is an API wrapper for âNova_Universeâ (a minecraft event
+hosting group) that allows you to interface with the Nova_Universe_API in a
+fast object oriented way natively within Python. One of the bonuses is that it
+was developed by ME, an admin at NovaUniverse.
 
 ## *Install/Set Up* 1. **Install package from pypi.** ```sh #Windows/Linux pip
 install novauniverse ``` 2. **That's It!** - *Brief Example Below* ```python
-from novauniverse import NovaClient, Events, NovaOnlinePlayer client =
-NovaClient() @client.on_event(Events.CLIENT_READY) def client_is_ready(): print
-("Client is ready!") @client.on_event(Events.PLAYER_JOIN) def on_player_join
-(player:NovaOnlinePlayer): print(f"{player.username} joined
+from novauniverse import EventClient, Events, NovaOnlinePlayer client =
+EventClient() @client.on_event(Events.CLIENT_READY) def client_is_ready():
+print("Client is ready!") @client.on_event(Events.PLAYER_JOIN) def
+on_player_join(player:NovaOnlinePlayer): print(f"{player.username} joined
 {player.server_name}!") client.start() ```
 > ### More Examples and Info at https://nupy.devgoldy.me/
```

### Comparing `novauniverse-2.0/novauniverse.egg-info/SOURCES.txt` & `novauniverse-2.0.1/novauniverse.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .gitignore
 CHANGELOG.rst
 Makefile
 README.md
-demo.py
 pyproject.toml
 .github/workflows/documentation.yaml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/events.rst
 docs/index.rst
```

### Comparing `novauniverse-2.0/pyproject.toml` & `novauniverse-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
     "requests",
     "importlib-metadata; python_version<'3.8'",
-    "devgoldyutils>=2.3.7",
+    "devgoldyutils>=2.4.3",
     "prettyprinter",
     "python-decouple>=3.7"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
@@ -37,15 +37,15 @@
   "pytest",
   "pytest-cov",
 ]
 
 [project.urls]
 GitHub = "https://github.com/NovaUniverse/NovaUniverse.py"
 BugTracker = "https://github.com/NovaUniverse/NovaUniverse.py/issues"
-ChangeLog = "https://github.com/NovaUniverse/NovaUniverse.py/v2/CHANGELOG.md"
+ChangeLog = "https://github.com/NovaUniverse/NovaUniverse.py/blob/main/CHANGELOG.rst"
 
 [tool.setuptools.dynamic]
 version = { attr = "novauniverse.info.VERSION" }
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `novauniverse-2.0/tests/interfaces/stats/test_server.py` & `novauniverse-2.0.1/tests/interfaces/stats/test_server.py`

 * *Files identical despite different names*

