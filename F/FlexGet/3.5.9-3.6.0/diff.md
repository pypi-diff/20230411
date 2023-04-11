# Comparing `tmp/FlexGet-3.5.9.tar.gz` & `tmp/FlexGet-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-mtivucuj/FlexGet-3.5.9.tar", last modified: Thu Dec  8 15:14:41 2022, max compression
+gzip compressed data, was "/home/runner/work/Flexget/Flexget/dist/.tmp-p1cbgchw/FlexGet-3.6.0.tar", last modified: Mon Apr 10 15:12:12 2023, max compression
```

## Comparing `FlexGet-3.5.9.tar` & `FlexGet-3.6.0.tar`

### file list

```diff
@@ -1,979 +1,980 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/FlexGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2022-12-08 15:14:40.000000 FlexGet-3.5.9/FlexGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39025 2022-12-08 15:14:40.000000 FlexGet-3.5.9/FlexGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 15:14:40.000000 FlexGet-3.5.9/FlexGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-08 15:14:40.000000 FlexGet-3.5.9/FlexGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2022-12-08 15:14:40.000000 FlexGet-3.5.9/FlexGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-08 15:14:40.000000 FlexGet-3.5.9/FlexGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2022-12-08 15:14:01.000000 FlexGet-3.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-08 15:14:01.000000 FlexGet-3.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2022-12-08 15:14:41.000000 FlexGet-3.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2022-12-08 15:14:01.000000 FlexGet-3.5.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2022-12-08 15:14:01.000000 FlexGet-3.5.9/dev-requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2022-12-08 15:14:01.000000 FlexGet-3.5.9/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-08 15:14:31.000000 FlexGet-3.5.9/flexget/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15592 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20648 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22051 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/templates/api_response.html
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/api/templates/swagger-ui.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/archive/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/archive/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/archive/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/archives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/archives/archives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/archives/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/backlog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/backlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/backlog/backlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/backlog/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/backlog/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/bittorrent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/convert_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/magnet_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/private_torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/torrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/torrent_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/torrent_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/torrent_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/torrent_scrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/torrent_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/bittorrent/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/emby/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/emby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    83323 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/emby/api_emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/emby/emby_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/emby/emby_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/emby/emby_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/emby/emby_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/emby/from_emby.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/estimate_release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/estimate_release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/estimate_release/estimate_release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/estimate_release/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/estimate_release/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/estimate_release/estimators/est_movies_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/estimate_release/estimators/est_released_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/estimate_release/estimators/est_series_tvmaze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/failed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/failed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/failed/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/failed/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/failed/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/failed/retry_failed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/ftp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/ftp/ftp_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/ftp/ftp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/ftp/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    18941 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/ftp/sftp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/history/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/history/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/history/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/history/history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/imdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/from_imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/imdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/imdb_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/imdb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/imdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/irc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/irc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/irc/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/irc/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    43375 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/irc/irc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/managed_lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/list_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/list_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/list_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/list_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/couchpotato_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/entry_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20369 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/imdb_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/movie_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13360 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/pending_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    22661 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/radarr_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/regexp_list/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/regexp_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/regexp_list/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/regexp_list/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/sonarr_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/subtitle_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/thetvdb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/managed_lists/lists/yaml_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/notify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notification_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/cronitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/gotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/ifttt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/microsoftteams.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/notifymyandroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/ntfysh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/prowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/pushalot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/pushbullet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/pushover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/pushsafer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/rapidpush.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/sms_ru.py
--rw-r--r--   0 runner    (1001) docker     (123)    19603 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/toast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notifiers/xmpp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/notify/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/parsing/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/parsing/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/parsing/parsers/parser_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/parsing/parsers/parser_guessit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/parsing/parsers/parser_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/parsing/plugin_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/pending_approval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/pending_approval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/pending_approval/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/pending_approval/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/pending_approval/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/pending_approval/pending_approval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/rejected/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/rejected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/rejected/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/rejected/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/rejected/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/rejected/remember_rejected.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/scheduler/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/seen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/seen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/seen/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/seen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/seen/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/seen/seen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/seen/seen_info_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/seen/seen_movies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/all_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    47214 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/configure_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    57052 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/gen_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/internal_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/metainfo_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/next_series_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/next_series_seasons.py
--rw-r--r--   0 runner    (1001) docker     (123)    53498 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/series_begin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/series_premiere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/series_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/series/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/components/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/components/sites/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/allyoulike.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/alpharatio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/animeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/anirena.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/archetorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/argenteam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/awesomehd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/bakabt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/btn.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/cinemageddon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/cpasbien.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/deadfrog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/descargas2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/ettv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/eztv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/filelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/filelist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/frenchtorrentdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/fuzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/google_cse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/hebits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/hliang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/horriblesubs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/iptorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/koreus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/limetorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)    26174 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/lostfilm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/magnetdl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/morethantv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/ncore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/newtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/newznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/nnmclub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/nyaa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/passthepopcorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/ptn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/rarbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/redirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/rlsbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/rmz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/serienjunkies.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/shortened.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/site_1337x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/site_rutracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/solidtorrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/torrent_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/torrentday.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/torrentleech.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/torrentz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/wordpress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/sites/yts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/urlrewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/urlrewrite_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/urlrewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/sites/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/components/status/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/status/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/status/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/status/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/status/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/components/thetvdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/thetvdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/thetvdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30428 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/thetvdb/api_tvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/thetvdb/thetvdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/components/tmdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/tmdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/tmdb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/tmdb/api_tmdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/tmdb/tmdb_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/components/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17388 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/api_trakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    42383 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/next_trakt_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/trakt_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20862 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/trakt_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/trakt/trakt_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/components/tvmaze/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/tvmaze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/tvmaze/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26637 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/tvmaze/api_tvmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/tvmaze/tvmaze_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/components/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/variables/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/components/variables/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/db_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    43372 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/debug_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/explain_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/inject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/perf_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/try_regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/wiki_qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/cli/win32_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/clients/aria2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31731 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/clients/deluge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/clients/nzbget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9436 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/clients/pyload.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/clients/qbittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25951 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/clients/rtorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    38943 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/clients/transmission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/daemon/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/daemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/daemon/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/filter/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/abort_if_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/accept_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/best_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/content_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/crossmatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/exists_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/exists_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/if_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/limit_new.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/magnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/only_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/proper_movies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/regexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/require_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/thetvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/timeframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/filter/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/generic/cron_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/generic/db_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/generic/db_vacuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/generic/log_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/generic/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/generic/welcome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/input/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/anidb_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/anilist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/apple_trailers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/betaseries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/filmweb_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/from_piratebay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/from_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/from_telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/gazelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/input_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/kitsu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/letterboxd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/medusa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/my_anime_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/myepisodes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/next_sonarr_episodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/npo_watchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/parameterize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18277 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/plex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/pogcal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/regexp_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/rlslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/rottentomatoes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    24946 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/sceper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/sickbeard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11576 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/torznab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/input/twitterfeed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/internal/api_bluray.py
--rw-r--r--   0 runner    (1001) docker     (123)    24459 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/internal/api_rottentomatoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/internal/change_warn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/metainfo/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/assume_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/bluray_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/content_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/media_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/metainfo_movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/nfo_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/nzb_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/rottentomatoes_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/subtitles_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/metainfo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/modify/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/path_by_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/path_by_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/plugin_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/regex_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/reorder_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/set_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/sort_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/modify/sort_by_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/operate/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/abort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/cfscraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/debug_db_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/debug_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/disable_phases.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/domain_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/entry_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/formlogin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/free_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/max_reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/spy_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/verbose_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/verify_ssl_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/operate/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/output/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22426 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/download_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/dump_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    14642 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/memusage.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/mock_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/rtorrent_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/sabnzbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/subtitles_periscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/subtitles_subliminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/output/utorrent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/services/kodi_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/services/myepisodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/plugins/services/pogcal_acquired.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    21065 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/resources/flexget.png
--rw-r--r--   0 runner    (1001) docker     (123)    28413 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/templates/entry/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/templates/entry/default.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/templates/task/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/templates/task/default.template
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/templates/task/html.template
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/templates/task/rss.template
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/tray_icon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/app.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/ui/v1/app/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/app/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/assets/images/header.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   124988 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   391622 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   152796 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90412 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71896 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/ui-grid.eot
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/ui-grid.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/ui-grid.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/fonts/ui-grid.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/app/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)   167898 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/scripts/splash.js
--rw-r--r--   0 runner    (1001) docker     (123)  6142562 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/scripts/vendor.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/app/styles/
--rw-r--r--   0 runner    (1001) docker     (123)   374613 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/styles/splash.css
--rw-r--r--   0 runner    (1001) docker     (123)    86217 2022-12-08 15:14:32.000000 FlexGet-3.5.9/flexget/ui/v1/app/styles/vendor.css
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/bower.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/build.js
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/inject.js
--rw-r--r--   0 runner    (1001) docker     (123)      573 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/lint.js
--rw-r--r--   0 runner    (1001) docker     (123)      717 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/proxy.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/scripts.js
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/server.js
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/styles.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/test.js
--rw-r--r--   0 runner    (1001) docker     (123)      850 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulp/watch.js
--rw-r--r--   0 runner    (1001) docker     (123)      298 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/karma.conf.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/load.failure.html
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)    18741 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/specs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/app.html
--rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/app.loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      857 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/app.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/app.scss
--rw-r--r--   0 runner    (1001) docker     (123)      447 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/app.utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/ui/v1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/assets/images/header.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/_error-dialog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      532 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      702 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      170 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      685 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/exception/exception.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/exception/exception.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/_pagination.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/pagination.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      486 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/pagination.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      741 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/router/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/router/router-helper.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/router/router-helper.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      376 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/url-interceptor/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      750 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/404/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      862 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/_login.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.config.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      215 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      882 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      997 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      967 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/components.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/core/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/core/core.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/core/core.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      993 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/core/core.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/core/core.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      494 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/core/core.route.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/database/_database.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      585 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/home/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/_sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      782 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      461 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/user/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/components/user/user.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/construction.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/directives/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/directives/directives.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/directives/palette-background/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/layout.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-input/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      762 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.filter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      592 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      686 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
--rw-r--r--   0 runner    (1001) docker     (123)      774 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      767 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-list/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      744 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/new-list/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      968 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      671 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      680 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.route.js
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.scss
--rw-r--r--   0 runner    (1001) docker     (123)      994 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.service.js
--rw-r--r--   0 runner    (1001) docker     (123)      897 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      305 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/plugins.module.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      266 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      689 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      791 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      743 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/seen-field/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      749 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:40.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-release/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
--rw-r--r--   0 runner    (1001) docker     (123)      631 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-releases/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-entry/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      367 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episode/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
--rw-r--r--   0 runner    (1001) docker     (123)      636 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
--rw-r--r--   0 runner    (1001) docker     (123)      876 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.component.js
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.component.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      307 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      669 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.route.js
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.route.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.service.js
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.service.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      758 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      846 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/server.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/server.module.js
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/server.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.component.js
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.module.js
--rw-r--r--   0 runner    (1001) docker     (123)      676 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.route.js
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.service.js
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.tmpl.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/scss/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/scss/_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/scss/_loading-bar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      250 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/scss/_variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/scss/flexget.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/src/services/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/src/services/schema.service.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/execute.js
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/history.js
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/movie_list.js
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/registerPlugin.js
--rw-r--r--   0 runner    (1001) docker     (123)      459 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/schedules.js
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/seen.js
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/series.js
--rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/states.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v2/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15872 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
--rw-r--r--   0 runner    (1001) docker     (123)    33576 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22304 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    47404 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  1150672 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)  4396877 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20268 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
--rw-r--r--   0 runner    (1001) docker     (123)   126767 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)   560902 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    15808 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21588 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    70594 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
--rw-r--r--   0 runner    (1001) docker     (123)    91826 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   562036 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
--rw-r--r--   0 runner    (1001) docker     (123)  2069487 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
--rw-r--r--   0 runner    (1001) docker     (123)    41804 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   148218 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
--rw-r--r--   0 runner    (1001) docker     (123)   618494 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    39851 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
--rw-r--r--   0 runner    (1001) docker     (123)    71452 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    57772 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
--rw-r--r--   0 runner    (1001) docker     (123)   225286 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20348 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
--rw-r--r--   0 runner    (1001) docker     (123)    17020 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    46199 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    91316 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    50808 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
--rw-r--r--   0 runner    (1001) docker     (123)   136381 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
--rw-r--r--   0 runner    (1001) docker     (123)    52623 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17008 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
--rw-r--r--   0 runner    (1001) docker     (123)    21952 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
--rw-r--r--   0 runner    (1001) docker     (123)    88547 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   130389 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77360 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
--rw-r--r--   0 runner    (1001) docker     (123)    95799 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
--rw-r--r--   0 runner    (1001) docker     (123)  2285898 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
--rw-r--r--   0 runner    (1001) docker     (123)  9410938 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2022-12-08 15:14:34.000000 FlexGet-3.5.9/flexget/ui/v2/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      411 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/ui/v2/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/bittorrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/cached_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/lazy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:14:41.000000 FlexGet-3.5.9/flexget/utils/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/parsers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/parsers/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28537 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/parsers/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/pathscrub.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/qualities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/simple_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/soup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/sqlalchemy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16984 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2022-12-08 15:14:01.000000 FlexGet-3.5.9/flexget/webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2022-12-08 15:14:01.000000 FlexGet-3.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2022-12-08 15:14:01.000000 FlexGet-3.5.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 15:14:41.000000 FlexGet-3.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/FlexGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-10 15:12:12.000000 FlexGet-3.6.0/FlexGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39082 2023-04-10 15:12:12.000000 FlexGet-3.6.0/FlexGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:12:12.000000 FlexGet-3.6.0/FlexGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-10 15:12:12.000000 FlexGet-3.6.0/FlexGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-10 15:12:12.000000 FlexGet-3.6.0/FlexGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 15:12:12.000000 FlexGet-3.6.0/FlexGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-10 15:11:44.000000 FlexGet-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 15:11:44.000000 FlexGet-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-10 15:12:12.000000 FlexGet-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-10 15:11:44.000000 FlexGet-3.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 15:11:44.000000 FlexGet-3.6.0/dev-requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-10 15:11:44.000000 FlexGet-3.6.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-10 15:12:06.000000 FlexGet-3.6.0/flexget/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15592 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20648 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22051 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/templates/api_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/api/templates/swagger-ui.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/archive/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/archive/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/archive/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/archives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/archives/archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/archives/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/backlog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/backlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/backlog/backlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/backlog/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/backlog/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/bittorrent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/convert_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/magnet_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/private_torrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/torrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/torrent_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/torrent_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/torrent_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/torrent_scrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/torrent_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/bittorrent/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/emby/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/emby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83320 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/emby/api_emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/emby/emby_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/emby/emby_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/emby/emby_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/emby/emby_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/emby/from_emby.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/estimate_release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/estimate_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/estimate_release/estimate_release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/estimate_release/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/estimate_release/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/estimate_release/estimators/est_movies_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/estimate_release/estimators/est_released_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/estimate_release/estimators/est_series_tvmaze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/failed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/failed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/failed/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/failed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/failed/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/failed/retry_failed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/ftp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/ftp/ftp_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/ftp/ftp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/ftp/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23191 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/ftp/sftp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/history/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/history/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/history/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/history/history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/imdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/from_imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/imdb_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/imdb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/imdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/irc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/irc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/irc/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/irc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43492 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/irc/irc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/managed_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/list_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/list_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/list_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/list_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/couchpotato_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/entry_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20369 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/imdb_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/movie_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/pending_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/plex_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22661 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/radarr_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/regexp_list/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/regexp_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/regexp_list/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/regexp_list/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/regexp_list/regexp_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/sonarr_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/subtitle_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/thetvdb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/managed_lists/lists/yaml_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/notify/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notification_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/cronitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/gotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/ifttt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/microsoftteams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/notifymyandroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/ntfysh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/prowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/pushalot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/pushbullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/pushover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/pushsafer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/rapidpush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/sms_ru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19603 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/toast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notifiers/xmpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/notify/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/parsing/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/parsing/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/parsing/parsers/parser_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/parsing/parsers/parser_guessit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/parsing/parsers/parser_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/parsing/plugin_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/pending_approval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/pending_approval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/pending_approval/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/pending_approval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/pending_approval/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/pending_approval/pending_approval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/rejected/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/rejected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/rejected/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/rejected/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/rejected/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/rejected/remember_rejected.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/scheduler/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/seen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/seen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/seen/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/seen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/seen/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/seen/seen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/seen/seen_info_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/seen/seen_movies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/all_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/configure_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57052 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/gen_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/internal_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/metainfo_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/next_series_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/next_series_seasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53498 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/series_begin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/series_premiere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/series_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/series/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/sites/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/allyoulike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/alpharatio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/animeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/anirena.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/archetorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/argenteam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/awesomehd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/bakabt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/btn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/cinemageddon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/cpasbien.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/deadfrog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/descargas2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/ettv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/eztv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/filelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/filelist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/frenchtorrentdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/fuzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/google_cse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/hebits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/hliang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/horriblesubs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/iptorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/koreus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/limetorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26174 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/lostfilm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/magnetdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/morethantv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/ncore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/newtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/newznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/nnmclub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/nyaa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/passthepopcorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/ptn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/rarbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/rlsbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/rmz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/serienjunkies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/shortened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/site_1337x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/site_rutracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/solidtorrents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/torrent_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/torrentday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/torrentleech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/torrentz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/wordpress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/sites/yts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/urlrewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/urlrewrite_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/urlrewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/sites/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/status/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/status/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/status/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/status/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/status/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/thetvdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/thetvdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/thetvdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30428 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/thetvdb/api_tvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/thetvdb/thetvdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/tmdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/tmdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/tmdb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/tmdb/api_tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/tmdb/tmdb_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/api_trakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42383 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/next_trakt_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/trakt_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20862 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/trakt_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/trakt/trakt_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/tvmaze/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/tvmaze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/tvmaze/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26637 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/tvmaze/api_tvmaze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/tvmaze/tvmaze_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/components/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/variables/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/components/variables/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/db_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42927 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23361 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/debug_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/explain_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/perf_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/try_regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/wiki_qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/cli/win32_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/clients/aria2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31731 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/clients/deluge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/clients/nzbget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/clients/pyload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/clients/qbittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25948 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/clients/rtorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40087 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/clients/transmission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/daemon/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/daemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/daemon/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/abort_if_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/accept_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/best_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/content_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/crossmatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/exists_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/exists_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/if_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/limit_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/magnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/only_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/proper_movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/regexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/require_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/thetvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/filter/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/generic/cron_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/generic/db_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/generic/db_vacuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/generic/log_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/generic/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/generic/welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/anidb_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/anilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/apple_trailers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/betaseries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/filmweb_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/from_piratebay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/from_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/from_telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/gazelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/input_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/kitsu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/letterboxd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/medusa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/my_anime_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/myepisodes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/next_sonarr_episodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/npo_watchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18277 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/plex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/pogcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/regexp_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/rlslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/rottentomatoes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24944 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/sceper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/sickbeard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/torznab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/input/twitterfeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/internal/api_bluray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/internal/api_rottentomatoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/internal/change_warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/metainfo/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/assume_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/bluray_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/content_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/media_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/metainfo_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/nfo_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/nzb_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/rottentomatoes_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/subtitles_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/metainfo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/modify/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/path_by_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/path_by_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/plugin_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/regex_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/reorder_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/set_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/modify/sort_by_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/operate/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/abort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/cfscraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/debug_db_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/debug_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/disable_phases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/domain_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/entry_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/formlogin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/free_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/max_reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/spy_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/verbose_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/verify_ssl_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/operate/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22426 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/download_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/dump_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/mock_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/rtorrent_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/sabnzbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/subtitles_periscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/subtitles_subliminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/symlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/output/utorrent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/services/kodi_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/services/myepisodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/plugins/services/pogcal_acquired.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    21065 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/resources/flexget.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28447 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/templates/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/templates/entry/default.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/templates/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/templates/task/default.template
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/templates/task/html.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/templates/task/rss.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/tray_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/app.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/app/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/app/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/assets/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   124988 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   391622 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   152796 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90412 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71896 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/ui-grid.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/ui-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/ui-grid.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/fonts/ui-grid.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/app/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)   167898 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/scripts/splash.js
+-rw-r--r--   0 runner    (1001) docker     (123)  6142562 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/scripts/vendor.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)   374613 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/styles/splash.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86217 2023-04-10 15:12:07.000000 FlexGet-3.6.0/flexget/ui/v1/app/styles/vendor.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/bower.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/build.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/inject.js
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/lint.js
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/scripts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/server.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/styles.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulp/watch.js
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/karma.conf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/load.failure.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18741 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/specs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/app.loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/app.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/app.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/app.utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/assets/icons/ic_movie_black_24px.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/assets/images/header.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/_error-dialog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/exception/exception.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/exception/exception.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/exception/exception.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/_pagination.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/pagination.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/pagination.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/pagination.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/router/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/router/router-helper.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/router/router-helper.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/router/router-helper.provider.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/url-interceptor/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/404/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/_login.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.config.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/components.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/core/core.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/core/core.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/core/core.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/core/core.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/core/core.route.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/database/_database.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/home/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/_sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.semver.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/components/user/user.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/construction.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/directives/directives.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/directives/palette-background/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/layout.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-input/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.filter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-list/
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/new-list/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/plugins.module.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/seen-field/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/seen-field/seen-field.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-release/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-entry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.component.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.route.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.service.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/loading-dialog.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/server.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/server.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/server.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.component.js
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.module.js
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.route.js
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.service.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.tmpl.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/scss/_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/scss/_loading-bar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/scss/_variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/scss/flexget.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/src/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/src/services/schema.service.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/execute.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/history.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/movie_list.js
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/registerPlugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/schedules.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/seen.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/series.js
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/states.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v2/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15872 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33576 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22304 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    47404 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  1150672 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4396877 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    20368 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20268 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   126767 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   560902 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15808 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    70594 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css
+-rw-r--r--   0 runner    (1001) docker     (123)    91826 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   562036 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2069487 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41804 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   148218 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js
+-rw-r--r--   0 runner    (1001) docker     (123)   618494 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    39851 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    71452 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    57772 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   225286 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20348 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17020 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    46199 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91316 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    50808 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js
+-rw-r--r--   0 runner    (1001) docker     (123)   136381 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52623 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17008 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    88547 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   130389 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77360 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css
+-rw-r--r--   0 runner    (1001) docker     (123)    95799 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)  2285898 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js
+-rw-r--r--   0 runner    (1001) docker     (123)  9410938 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-10 15:12:08.000000 FlexGet-3.6.0/flexget/ui/v2/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/ui/v2/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/bittorrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/cached_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/lazy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:12:12.000000 FlexGet-3.6.0/flexget/utils/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/parsers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/parsers/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/parsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28537 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/parsers/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/pathscrub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/qualities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/simple_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/soup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/sqlalchemy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16984 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-10 15:11:44.000000 FlexGet-3.6.0/flexget/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-10 15:11:44.000000 FlexGet-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-10 15:11:44.000000 FlexGet-3.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:12:12.000000 FlexGet-3.6.0/setup.cfg
```

### Comparing `FlexGet-3.5.9/FlexGet.egg-info/PKG-INFO` & `FlexGet-3.6.0/FlexGet.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.5.9
+Version: 3.6.0
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
@@ -65,15 +65,15 @@
 
 Example
 =======
 Flexget uses a `YAML`_ based configuration file.
 The following example will look in the RSS feed in the link, will match any item that match the series names and download it::
 
     tasks:
-      tv_task:
+      tv:
         rss: http://example.com/torrents.xml
         series:
         - some series
         - another series
         download: /tvshows
 
 There are numerous plugins that allow utilizing FlexGet in interesting ways
@@ -108,48 +108,14 @@
 For more detailed instructions see the `installation guide`_.
 
 .. _installation guide: https://flexget.com/Install
 
 How to use GIT checkout
 -----------------------
 
-Check that you have Python 3.7 or newer available with command ``python -V``.
+Refer to `development guide`_.
 
-In some environments newer python might be available under another name like
-'python3.7' or 'python3' in which case you need to use that one instead of
-plain 'python'.
-
-To start using FlexGet from this directory::
-
-    python3 -m venv .
-
-This will initialize python virtualenv. This doesn't need to be directly in
-your checkout directory, but these instructions assume that's where it is.
-
-On some linux distributions (eg. debian, ubuntu) venv module is not included with
-python and this fails. Please install `python3-virtualenv` package and retry
-(or use the separate `virtualenv`_ python package).
-
-.. _virtualenv: https://pypi.python.org/pypi/virtualenv
-
-Upgrading pip and setuptools to latest version is highly advisable if not mandatory
-for working installation and can de done with::
-
-    bin/pip install --upgrade pip setuptools
-
-Next we need to install dependencies and FlexGet itself, this can be done simply::
-
-    bin/pip install -e .
-
-This does an editable (`-e`) development install of the current directory (`.`).
-
-After that FlexGet is usable via ``<checkout directory>/bin/flexget``. Verify
-installation by running::
-
-    bin/flexget -V
-
-You may place the config file in your checkout directory, or in ``~/.flexget``
-(Unix, Mac OS X) or ``C:\Documents and Setting\<username>\flexget`` (Windows).
+.. _development guide: https://flexget.readthedocs.io/en/latest/develop/index.html#how-do-i-get-started
 
 If you don't want to use virtualenv there's ``flexget_vanilla.py`` file which
 can be used to run FlexGet without virtualenv, note that you will need to
 install all required dependencies yourself.
```

### Comparing `FlexGet-3.5.9/FlexGet.egg-info/SOURCES.txt` & `FlexGet-3.6.0/FlexGet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 flexget/components/managed_lists/list_add.py
 flexget/components/managed_lists/list_clear.py
 flexget/components/managed_lists/list_match.py
 flexget/components/managed_lists/list_remove.py
 flexget/components/managed_lists/lists/__init__.py
 flexget/components/managed_lists/lists/couchpotato_list.py
 flexget/components/managed_lists/lists/imdb_list.py
+flexget/components/managed_lists/lists/plex_watchlist.py
 flexget/components/managed_lists/lists/radarr_list.py
 flexget/components/managed_lists/lists/sonarr_list.py
 flexget/components/managed_lists/lists/subtitle_list.py
 flexget/components/managed_lists/lists/thetvdb_list.py
 flexget/components/managed_lists/lists/yaml_list.py
 flexget/components/managed_lists/lists/entry_list/__init__.py
 flexget/components/managed_lists/lists/entry_list/api.py
```

### Comparing `FlexGet-3.5.9/LICENSE` & `FlexGet-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/PKG-INFO` & `FlexGet-3.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlexGet
-Version: 3.5.9
+Version: 3.6.0
 Summary: FlexGet is a program aimed to automate downloading or processing content (torrents, podcasts, etc.) from different sources like RSS-feeds, html-pages, various sites and more.
 Author-email: Marko Koivusalo <marko.koivusalo@gmail.com>, Chase Sterling <chase.sterling@gmail.com>
 License: 
         The MIT License
         
         Copyright (C) 2006, Riku 'Shrike' Lindblad
         Copyright (C) 2007, Marko Koivusalo
@@ -65,15 +65,15 @@
 
 Example
 =======
 Flexget uses a `YAML`_ based configuration file.
 The following example will look in the RSS feed in the link, will match any item that match the series names and download it::
 
     tasks:
-      tv_task:
+      tv:
         rss: http://example.com/torrents.xml
         series:
         - some series
         - another series
         download: /tvshows
 
 There are numerous plugins that allow utilizing FlexGet in interesting ways
@@ -108,48 +108,14 @@
 For more detailed instructions see the `installation guide`_.
 
 .. _installation guide: https://flexget.com/Install
 
 How to use GIT checkout
 -----------------------
 
-Check that you have Python 3.7 or newer available with command ``python -V``.
+Refer to `development guide`_.
 
-In some environments newer python might be available under another name like
-'python3.7' or 'python3' in which case you need to use that one instead of
-plain 'python'.
-
-To start using FlexGet from this directory::
-
-    python3 -m venv .
-
-This will initialize python virtualenv. This doesn't need to be directly in
-your checkout directory, but these instructions assume that's where it is.
-
-On some linux distributions (eg. debian, ubuntu) venv module is not included with
-python and this fails. Please install `python3-virtualenv` package and retry
-(or use the separate `virtualenv`_ python package).
-
-.. _virtualenv: https://pypi.python.org/pypi/virtualenv
-
-Upgrading pip and setuptools to latest version is highly advisable if not mandatory
-for working installation and can de done with::
-
-    bin/pip install --upgrade pip setuptools
-
-Next we need to install dependencies and FlexGet itself, this can be done simply::
-
-    bin/pip install -e .
-
-This does an editable (`-e`) development install of the current directory (`.`).
-
-After that FlexGet is usable via ``<checkout directory>/bin/flexget``. Verify
-installation by running::
-
-    bin/flexget -V
-
-You may place the config file in your checkout directory, or in ``~/.flexget``
-(Unix, Mac OS X) or ``C:\Documents and Setting\<username>\flexget`` (Windows).
+.. _development guide: https://flexget.readthedocs.io/en/latest/develop/index.html#how-do-i-get-started
 
 If you don't want to use virtualenv there's ``flexget_vanilla.py`` file which
 can be used to run FlexGet without virtualenv, note that you will need to
 install all required dependencies yourself.
```

### Comparing `FlexGet-3.5.9/README.rst` & `FlexGet-3.6.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 Example
 =======
 Flexget uses a `YAML`_ based configuration file.
 The following example will look in the RSS feed in the link, will match any item that match the series names and download it::
 
     tasks:
-      tv_task:
+      tv:
         rss: http://example.com/torrents.xml
         series:
         - some series
         - another series
         download: /tvshows
 
 There are numerous plugins that allow utilizing FlexGet in interesting ways
@@ -71,48 +71,14 @@
 For more detailed instructions see the `installation guide`_.
 
 .. _installation guide: https://flexget.com/Install
 
 How to use GIT checkout
 -----------------------
 
-Check that you have Python 3.7 or newer available with command ``python -V``.
+Refer to `development guide`_.
 
-In some environments newer python might be available under another name like
-'python3.7' or 'python3' in which case you need to use that one instead of
-plain 'python'.
-
-To start using FlexGet from this directory::
-
-    python3 -m venv .
-
-This will initialize python virtualenv. This doesn't need to be directly in
-your checkout directory, but these instructions assume that's where it is.
-
-On some linux distributions (eg. debian, ubuntu) venv module is not included with
-python and this fails. Please install `python3-virtualenv` package and retry
-(or use the separate `virtualenv`_ python package).
-
-.. _virtualenv: https://pypi.python.org/pypi/virtualenv
-
-Upgrading pip and setuptools to latest version is highly advisable if not mandatory
-for working installation and can de done with::
-
-    bin/pip install --upgrade pip setuptools
-
-Next we need to install dependencies and FlexGet itself, this can be done simply::
-
-    bin/pip install -e .
-
-This does an editable (`-e`) development install of the current directory (`.`).
-
-After that FlexGet is usable via ``<checkout directory>/bin/flexget``. Verify
-installation by running::
-
-    bin/flexget -V
-
-You may place the config file in your checkout directory, or in ``~/.flexget``
-(Unix, Mac OS X) or ``C:\Documents and Setting\<username>\flexget`` (Windows).
+.. _development guide: https://flexget.readthedocs.io/en/latest/develop/index.html#how-do-i-get-started
 
 If you don't want to use virtualenv there's ``flexget_vanilla.py`` file which
 can be used to run FlexGet without virtualenv, note that you will need to
 install all required dependencies yourself.
```

### Comparing `FlexGet-3.5.9/dev-requirements-extras.txt` & `FlexGet-3.6.0/dev-requirements-extras.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 appdirs==1.4.4 ; python_version >= "3.7" and python_version < "4.0"
 babelfish==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
-boto3==1.26.3 ; python_version >= "3.7" and python_version < "4.0"
-botocore==1.29.3 ; python_version >= "3.7" and python_version < "4.0"
-certifi==2022.9.24 ; python_version >= "3.7" and python_version < "4"
-chardet==5.0.0 ; python_version >= "3.7" and python_version < "4.0"
+boto3==1.26.27 ; python_version >= "3.7" and python_version < "4.0"
+botocore==1.29.27 ; python_version >= "3.7" and python_version < "4.0"
+certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
+chardet==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
 charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows"
 decorator==5.1.1 ; python_version >= "3.7" and python_version < "4.0"
 dogpile-cache==1.1.8 ; python_version >= "3.7" and python_version < "4.0"
 enzyme==0.4.1 ; python_version >= "3.7" and python_version < "4.0"
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4"
-importlib-metadata==5.0.0 ; python_version >= "3.7" and python_version < "3.8"
-importlib-resources==5.10.0 ; python_version >= "3.7" and python_version < "3.9"
+importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.8"
+importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 jmespath==1.0.1 ; python_version >= "3.7" and python_version < "4.0"
 pbr==5.11.0 ; python_version >= "3.7" and python_version < "4.0"
+plexapi==4.13.1 ; python_version >= "3.7" and python_version < "4.0"
 pysrt==1.1.2 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 rarfile==4.0 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
 s3transfer==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
 stevedore==3.5.2 ; python_version >= "3.7" and python_version < "4.0"
 subliminal==2.1.0 ; python_version >= "3.7" and python_version < "4.0"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "3.8"
-urllib3==1.26.12 ; python_version >= "3.7" and python_version < "4"
-zipp==3.10.0 ; python_version >= "3.7" and python_version < "3.9"
+urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
+zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.9"
```

### Comparing `FlexGet-3.5.9/dev-requirements.txt` & `FlexGet-3.6.0/dev-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,92 +1,91 @@
 alabaster==0.7.12 ; python_version >= "3.7" and python_version < "4.0"
 astroid==2.11.7 ; python_version >= "3.7" and python_version < "4.0"
 attrs==22.1.0 ; python_version >= "3.7" and python_version < "4.0"
 babel==2.11.0 ; python_version >= "3.7" and python_version < "4.0"
-black==22.10.0 ; python_version >= "3.7" and python_version < "4.0"
+black==22.12.0 ; python_version >= "3.7" and python_version < "4.0"
 bleach==5.0.1 ; python_version >= "3.7" and python_version < "4.0"
 build==0.9.0 ; python_version >= "3.7" and python_version < "4.0"
-certifi==2022.9.24 ; python_version >= "3.7" and python_version < "4"
+certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
 cffi==1.15.1 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 cfgv==3.3.1 ; python_version >= "3.7" and python_version < "4.0"
 charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 codacy-coverage==1.3.11 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0" and os_name == "nt" or python_version >= "3.7" and python_version < "4.0" and platform_system == "Windows" or python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
 coverage==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
 coverage[toml]==6.5.0 ; python_version >= "3.7" and python_version < "4.0"
-cryptography==38.0.3 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
+cryptography==38.0.4 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 dill==0.3.6 ; python_version >= "3.7" and python_version < "4.0"
 distlib==0.3.6 ; python_version >= "3.7" and python_version < "4.0"
 docutils==0.19 ; python_version >= "3.7" and python_version < "4.0"
-exceptiongroup==1.0.1 ; python_version >= "3.7" and python_version < "3.11"
+exceptiongroup==1.0.4 ; python_version >= "3.7" and python_version < "3.11"
 execnet==1.9.0 ; python_version >= "3.7" and python_version < "4.0"
-filelock==3.8.0 ; python_version >= "3.7" and python_version < "4.0"
-gitdb==4.0.9 ; python_version >= "3.7" and python_version < "4.0"
+filelock==3.8.2 ; python_version >= "3.7" and python_version < "4.0"
+gitdb==4.0.10 ; python_version >= "3.7" and python_version < "4.0"
 gitpython==3.1.29 ; python_version >= "3.7" and python_version < "4.0"
-identify==2.5.8 ; python_version >= "3.7" and python_version < "4.0"
+identify==2.5.9 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4"
 imagesize==1.4.1 ; python_version >= "3.7" and python_version < "4.0"
-importlib-metadata==5.0.0 ; python_version >= "3.7" and python_version < "4.0"
+importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "4.0"
 iniconfig==1.1.1 ; python_version >= "3.7" and python_version < "4.0"
 isort==5.10.1 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
 jeepney==0.8.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 jinja2==3.1.2 ; python_version >= "3.7" and python_version < "4.0"
 keyring==23.11.0 ; python_version >= "3.7" and python_version < "4.0"
 lazy-object-proxy==1.8.0 ; python_version >= "3.7" and python_version < "4.0"
 markupsafe==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 mccabe==0.7.0 ; python_version >= "3.7" and python_version < "4.0"
 more-itertools==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
-multidict==6.0.2 ; python_version >= "3.7" and python_version < "4.0"
+multidict==6.0.3 ; python_version >= "3.7" and python_version < "4.0"
 mypy-extensions==0.4.3 ; python_version >= "3.7" and python_version < "4.0"
-mypy==0.982 ; python_version >= "3.7" and python_version < "4.0"
+mypy==0.991 ; python_version >= "3.7" and python_version < "4.0"
 nodeenv==1.7.0 ; python_version >= "3.7" and python_version < "4.0"
-packaging==21.3 ; python_version >= "3.7" and python_version < "4.0"
-pathspec==0.10.1 ; python_version >= "3.7" and python_version < "4.0"
+packaging==22.0 ; python_version >= "3.7" and python_version < "4.0"
+pathspec==0.10.3 ; python_version >= "3.7" and python_version < "4.0"
 pep517==0.13.0 ; python_version >= "3.7" and python_version < "4.0"
-pkginfo==1.8.3 ; python_version >= "3.7" and python_version < "4.0"
-platformdirs==2.5.3 ; python_version >= "3.7" and python_version < "4.0"
+pkginfo==1.9.2 ; python_version >= "3.7" and python_version < "4.0"
+platformdirs==2.6.0 ; python_version >= "3.7" and python_version < "4.0"
 pluggy==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pre-commit==2.20.0 ; python_version >= "3.7" and python_version < "4.0"
 pycparser==2.21 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
 pylint==2.13.9 ; python_version >= "3.7" and python_version < "4.0"
-pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "4.0"
 pytest-cov==4.0.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest-runner==6.0.0 ; python_version >= "3.7" and python_version < "4.0"
-pytest-xdist==3.0.2 ; python_version >= "3.7" and python_version < "4.0"
+pytest-xdist==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 pytest==7.2.0 ; python_version >= "3.7" and python_version < "4.0"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4.0"
 pywin32-ctypes==0.2.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
 readme-renderer==37.3 ; python_version >= "3.7" and python_version < "4.0"
 requests-toolbelt==0.10.1 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
 rfc3986==2.0.0 ; python_version >= "3.7" and python_version < "4.0"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
 secretstorage==3.3.3 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "linux"
-setuptools==65.5.1 ; python_version >= "3.7" and python_version < "4.0"
+setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4.0"
 smmap==5.0.0 ; python_version >= "3.7" and python_version < "4.0"
 snowballstemmer==2.2.0 ; python_version >= "3.7" and python_version < "4.0"
 sphinx==5.3.0 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-applehelp==1.0.2 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-devhelp==1.0.2 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-htmlhelp==2.0.0 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-jsmath==1.0.1 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-qthelp==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 sphinxcontrib-serializinghtml==1.1.5 ; python_version >= "3.7" and python_version < "4.0"
 sqlalchemy-stubs==0.4 ; python_version >= "3.7" and python_version < "4.0"
 toml==0.10.2 ; python_version >= "3.7" and python_version < "4.0"
 tomli==2.0.1 ; python_version >= "3.7" and python_full_version < "3.11.0a7"
-twine==4.0.1 ; python_version >= "3.7" and python_version < "4.0"
-typed-ast==1.5.4 ; python_version >= "3.7" and python_version < "3.8"
+twine==4.0.2 ; python_version >= "3.7" and python_version < "4.0"
+typed-ast==1.5.4 ; python_version < "3.8" and python_version >= "3.7"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
-urllib3==1.26.12 ; python_version >= "3.7" and python_version < "4"
+urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4.0"
 vcrpy==4.2.1 ; python_version >= "3.7" and python_version < "4.0"
-virtualenv==20.16.6 ; python_version >= "3.7" and python_version < "4.0"
+virtualenv==20.17.1 ; python_version >= "3.7" and python_version < "4.0"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
 wrapt==1.14.1 ; python_version >= "3.7" and python_version < "4.0"
-yarl==1.8.1 ; python_version >= "3.7" and python_version < "4.0"
-zipp==3.10.0 ; python_version >= "3.7" and python_version < "4.0"
+yarl==1.8.2 ; python_version >= "3.7" and python_version < "4.0"
+zipp==3.11.0 ; python_version >= "3.7" and python_version < "4.0"
```

### Comparing `FlexGet-3.5.9/flexget/__init__.py` & `FlexGet-3.6.0/flexget/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,41 @@
 from ._version import __version__  # noqa
 
 # isort: split
 from flexget import log  # noqa
 from flexget.manager import Manager  # noqa
 
 
-def main(args: Sequence = None):
+def main(args: Sequence[str] = None):
     """Main entry point for Command Line Interface"""
 
+    if args is None:
+        args = sys.argv[1:]
     try:
         log.initialize()
 
         try:
             manager = Manager(args)
         except (OSError, ValueError) as e:
+            options = Manager.parse_initial_options(args)
+            log.start(level=options.loglevel, to_file=False)
             if _is_debug():
                 import traceback
 
                 traceback.print_exc()
             else:
                 print('Could not instantiate manager: %s' % e, file=sys.stderr)
             sys.exit(1)
+        else:
+            log.start(
+                manager.log_filename,
+                manager.options.loglevel,
+                to_file=manager.check_ipc_info() is None,
+                to_console=not manager.options.cron,
+            )
 
         try:
             if manager.options.profile:
                 try:
                     import cProfile as profile
                 except ImportError:
                     import profile
```

### Comparing `FlexGet-3.5.9/flexget/api/app.py` & `FlexGet-3.6.0/flexget/api/app.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/authentication.py` & `FlexGet-3.6.0/flexget/api/core/authentication.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/cached.py` & `FlexGet-3.6.0/flexget/api/core/cached.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/database.py` & `FlexGet-3.6.0/flexget/api/core/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/format_checker.py` & `FlexGet-3.6.0/flexget/api/core/format_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/plugins.py` & `FlexGet-3.6.0/flexget/api/core/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/schema.py` & `FlexGet-3.6.0/flexget/api/core/schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/server.py` & `FlexGet-3.6.0/flexget/api/core/server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/tasks.py` & `FlexGet-3.6.0/flexget/api/core/tasks.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/core/user.py` & `FlexGet-3.6.0/flexget/api/core/user.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/templates/api_response.html` & `FlexGet-3.6.0/flexget/api/templates/api_response.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/api/templates/swagger-ui.html` & `FlexGet-3.6.0/flexget/api/templates/swagger-ui.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/archive/archive.py` & `FlexGet-3.6.0/flexget/components/archive/archive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/archive/cli.py` & `FlexGet-3.6.0/flexget/components/archive/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         duplicates = []
 
         for orig in track(
             session.query(flexget.components.archive.db.ArchiveEntry).yield_per(5),
             total=count,
             description='Processing...',
         ):
-
             # item already processed
             if orig.id in duplicates:
                 continue
 
             # item already migrated
             if orig.sources:
                 logger.info(
```

### Comparing `FlexGet-3.5.9/flexget/components/archive/db.py` & `FlexGet-3.6.0/flexget/components/archive/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/archives/archives.py` & `FlexGet-3.6.0/flexget/components/archives/archives.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/archives/decompress.py` & `FlexGet-3.6.0/flexget/components/archives/decompress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/archives/utils.py` & `FlexGet-3.6.0/flexget/components/archives/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/backlog/backlog.py` & `FlexGet-3.6.0/flexget/components/backlog/backlog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/backlog/cli.py` & `FlexGet-3.6.0/flexget/components/backlog/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/backlog/db.py` & `FlexGet-3.6.0/flexget/components/backlog/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/convert_magnet.py` & `FlexGet-3.6.0/flexget/components/bittorrent/convert_magnet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/magnet_info_hash.py` & `FlexGet-3.6.0/flexget/components/bittorrent/magnet_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/private_torrents.py` & `FlexGet-3.6.0/flexget/components/bittorrent/private_torrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/torrent.py` & `FlexGet-3.6.0/flexget/components/bittorrent/torrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/torrent_alive.py` & `FlexGet-3.6.0/flexget/components/bittorrent/torrent_alive.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/torrent_files.py` & `FlexGet-3.6.0/flexget/components/bittorrent/torrent_files.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/torrent_match.py` & `FlexGet-3.6.0/flexget/components/bittorrent/torrent_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/torrent_scrub.py` & `FlexGet-3.6.0/flexget/components/bittorrent/torrent_scrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/torrent_size.py` & `FlexGet-3.6.0/flexget/components/bittorrent/torrent_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/bittorrent/trackers.py` & `FlexGet-3.6.0/flexget/components/bittorrent/trackers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/emby/api_emby.py` & `FlexGet-3.6.0/flexget/components/emby/api_emby.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
         allow_new = kwargs.get('allow_new', False)
 
         my_field_map = field_map.copy()
 
         func_get = dict.get if isinstance(source_item, dict) else getattr
         for field, val in my_field_map.items():
-
             values = val
             if not isinstance(values, list):
                 values = [val]
 
             if values[0] and values[0].find(EmbyApiBase.EMBY_PREF) < 0:
                 values.insert(0, f'{EmbyApiBase.EMBY_PREF}{values[0]}')
 
@@ -193,15 +192,14 @@
 
     def login(self, optional=False):
         """Login user to API"""
 
         userdata = None
 
         if not self._apikey:
-
             if self.is_connect_server():
                 # Make Emby connect login
                 self._login_type = LOGIN_CONNECT
                 userdata = self.check_token_data(persist.get('token_data'), LOGIN_CONNECT)
                 if not userdata:
                     logger.debug(
                         'Login to Emby Connect with username `{}` host `{}`',
@@ -699,15 +697,14 @@
 
     @property
     def immutable(self):
         return self._list.immutable
 
     @staticmethod
     def get_api_list(**kwargs) -> EmbyApiListBase:
-
         if EmbyApiRootList.is_type(**kwargs):
             logger.debug('List is a root list')
             return EmbyApiRootList(**kwargs)
         elif EmbyApiWatchedList.is_type(**kwargs):
             logger.debug('List is a watched list')
             return EmbyApiWatchedList(**kwargs)
         elif EmbyApiFavoriteList.is_type(**kwargs):
```

### Comparing `FlexGet-3.5.9/flexget/components/emby/emby_list.py` & `FlexGet-3.6.0/flexget/components/emby/emby_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/emby/emby_lookup.py` & `FlexGet-3.6.0/flexget/components/emby/emby_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/emby/emby_refresh.py` & `FlexGet-3.6.0/flexget/components/emby/emby_refresh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/emby/emby_util.py` & `FlexGet-3.6.0/flexget/components/emby/emby_util.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/emby/from_emby.py` & `FlexGet-3.6.0/flexget/components/emby/from_emby.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/estimate_release/estimate_release.py` & `FlexGet-3.6.0/flexget/components/estimate_release/estimate_release.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/estimate_release/estimators/est_movies_bluray.py` & `FlexGet-3.6.0/flexget/components/estimate_release/estimators/est_movies_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/estimate_release/estimators/est_released_movies.py` & `FlexGet-3.6.0/flexget/components/estimate_release/estimators/est_released_movies.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 logger = logger.bind(name='est_movies')
 
 
 class EstimatesReleasedMovies:
     @plugin.priority(0)
     def estimate(self, entry):
-
         entity_data = {'data_exists': True, 'entity_date': None}
         if 'tmdb_released' in entry:
             logger.verbose('Querying release estimation for {}', entry['title'])
             entity_data['entity_date'] = entry['tmdb_released']
             return entity_data
         elif 'movie_year' in entry and entry['movie_year'] is not None:
             try:
```

### Comparing `FlexGet-3.5.9/flexget/components/estimate_release/estimators/est_series_tvmaze.py` & `FlexGet-3.6.0/flexget/components/estimate_release/estimators/est_series_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/failed/api.py` & `FlexGet-3.6.0/flexget/components/failed/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/failed/cli.py` & `FlexGet-3.6.0/flexget/components/failed/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/failed/db.py` & `FlexGet-3.6.0/flexget/components/failed/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/failed/retry_failed.py` & `FlexGet-3.6.0/flexget/components/failed/retry_failed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/ftp/ftp_download.py` & `FlexGet-3.6.0/flexget/components/ftp/ftp_download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/ftp/ftp_list.py` & `FlexGet-3.6.0/flexget/components/ftp/ftp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/ftp/sftp.py` & `FlexGet-3.6.0/flexget/components/ftp/sftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import List, Optional
 from urllib.parse import unquote, urlparse
 
 from loguru import logger
 
 from flexget import plugin
-from flexget.components.ftp.sftp_client import SftpClient, SftpError
+from flexget.components.ftp.sftp_client import HOST_KEY_TYPES, HostKey, SftpClient, SftpError
 from flexget.config_schema import one_or_more
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.task import Task
 from flexget.utils.template import RenderError, render_from_entry
 
 logger = logger.bind(name='sftp')
@@ -19,15 +19,16 @@
 # Constants
 DEFAULT_SFTP_PORT: int = 22
 DEFAULT_CONNECT_TRIES: int = 3
 DEFAULT_SOCKET_TIMEOUT_SEC: int = 15
 
 
 SftpConfig = namedtuple(
-    'SftpConfig', ['host', 'port', 'username', 'password', 'private_key', 'private_key_pass']
+    'SftpConfig',
+    ['host', 'port', 'username', 'password', 'private_key', 'private_key_pass', 'host_key'],
 )
 
 
 class SftpList:
     """
     Generate entries from SFTP. This plugin requires the pysftp Python module and its dependencies.
 
@@ -43,14 +44,15 @@
     get_size:             Indicates whetern to calculate the size of the remote file/directory.
                           WARNING: This can be very slow when computing the size of directories!
     files_only:           Indicates wheter to omit diredtories from the results.
     dirs_only:            Indicates whether to omit files from the results.
     dirs:                 List of directories to download.
     socket_timeout_sec:   Socket timeout in seconds (default 15 seconds).
     connection_tries:     Number of times to attempt to connect before failing (default 3).
+    host_key:             Specifies a host key not already in known_hosts
 
     Example:
 
       sftp_list:
           host: example.com
           username: Username
           private_key: /Users/username/.ssh/id_rsa
@@ -74,27 +76,37 @@
             'recursive': {'type': 'boolean', 'default': False},
             'get_size': {'type': 'boolean', 'default': True},
             'private_key': {'type': 'string'},
             'private_key_pass': {'type': 'string'},
             'dirs': one_or_more({'type': 'string'}),
             'socket_timeout_sec': {'type': 'integer', 'default': DEFAULT_SOCKET_TIMEOUT_SEC},
             'connection_tries': {'type': 'integer', 'default': DEFAULT_CONNECT_TRIES},
+            'host_key': {
+                'type': 'object',
+                'properties': {
+                    'key_type': {'type': 'string', 'enum': list(HOST_KEY_TYPES.keys())},
+                    'public_key': {'type': 'string'},
+                },
+                'required': ['key_type', 'public_key'],
+                'additionalProperties': False,
+            },
         },
         'additionProperties': False,
         'required': ['host', 'username'],
     }
 
     @staticmethod
     def prepare_config(config: dict) -> dict:
         """
         Sets defaults for the provided configuration
         """
         config.setdefault('password', None)
         config.setdefault('private_key', None)
         config.setdefault('private_key_pass', None)
+        config.setdefault('host_key', None)
         config.setdefault('dirs', ['.'])
 
         return config
 
     @classmethod
     def on_task_input(cls, task: Task, config: dict) -> List[Entry]:
         """
@@ -234,18 +246,27 @@
         password: str = parsed.password
         port: int = parsed.port or DEFAULT_SFTP_PORT
 
         # get private key info if it exists
         private_key: str = entry.get('private_key')
         private_key_pass: str = entry.get('private_key_pass')
 
+        entry_host_key_config: dict = entry.get('host_key')
+        host_key: Optional[HostKey] = None
+        if entry_host_key_config:
+            host_key = HostKey(
+                entry_host_key_config['key_type'], entry_host_key_config['public_key']
+            )
+
         config: Optional[SftpConfig] = None
 
         if parsed.scheme == 'sftp':
-            config = SftpConfig(host, port, username, password, private_key, private_key_pass)
+            config = SftpConfig(
+                host, port, username, password, private_key, private_key_pass, host_key
+            )
         else:
             logger.warning('Scheme does not match SFTP: {}', entry['url'])
 
         return config
 
 
 class SftpUpload:
@@ -262,14 +283,15 @@
     to:                   Path to upload the file to; supports Jinja2 templating on the input entry. Fields such
                           as series_name must be populated prior to input into this plugin using
                           metainfo_series or similar.
     delete_origin:        Indicates whether to delete the original file after a successful
                           upload.
     socket_timeout_sec:   Socket timeout in seconds
     connection_tries:     Number of times to attempt to connect before failing (default 3).
+    host_key:             Specifies a host key not already in known_hosts
 
     Example:
 
       sftp_list:
           host: example.com
           username: Username
           private_key: /Users/username/.ssh/id_rsa
@@ -284,14 +306,23 @@
             'username': {'type': 'string'},
             'password': {'type': 'string'},
             'port': {'type': 'integer', 'default': DEFAULT_SFTP_PORT},
             'private_key': {'type': 'string'},
             'private_key_pass': {'type': 'string'},
             'to': {'type': 'string'},
             'delete_origin': {'type': 'boolean', 'default': False},
+            'host_key': {
+                'type': 'object',
+                'properties': {
+                    'key_type': {'type': 'string', 'enum': list(HOST_KEY_TYPES.keys())},
+                    'public_key': {'type': 'string'},
+                },
+                'required': ['key_type', 'public_key'],
+                'additionalProperties': False,
+            },
             'socket_timeout_sec': {'type': 'integer', 'default': DEFAULT_SOCKET_TIMEOUT_SEC},
             'connection_tries': {'type': 'integer', 'default': DEFAULT_CONNECT_TRIES},
         },
         'additionProperties': False,
         'required': ['host', 'username'],
     }
 
@@ -305,15 +336,14 @@
         config.setdefault('private_key_pass', None)
         config.setdefault('to', None)
 
         return config
 
     @classmethod
     def handle_entry(cls, entry: Entry, sftp: SftpClient, config: dict):
-
         to: str = config['to']
         location: str = entry['location']
         delete_origin: bool = config['delete_origin']
 
         if to:
             try:
                 to = render_from_entry(to, entry)
@@ -361,27 +391,32 @@
     host: int = config['host']
     port: int = config['port']
     username: str = config['username']
     password: str = config['password']
     private_key: str = config['private_key']
     private_key_pass: str = config['private_key_pass']
 
-    return SftpConfig(host, port, username, password, private_key, private_key_pass)
+    host_key: Optional[HostKey] = None
+    if config.get('host_key') is not None:
+        host_key = HostKey(config['host_key']['key_type'], config['host_key']['public_key'])
+
+    return SftpConfig(host, port, username, password, private_key, private_key_pass, host_key)
 
 
 def sftp_connect(
     sftp_config: SftpConfig, socket_timeout_sec: int, connection_tries: int
 ) -> SftpClient:
     sftp_client: SftpClient = SftpClient(
         host=sftp_config.host,
         username=sftp_config.username,
         private_key=sftp_config.private_key,
         password=sftp_config.password,
         port=sftp_config.port,
         private_key_pass=sftp_config.private_key_pass,
+        host_key=sftp_config.host_key,
         connection_tries=connection_tries,
     )
     sftp_client.set_socket_timeout(socket_timeout_sec)
 
     return sftp_client
```

### Comparing `FlexGet-3.5.9/flexget/components/ftp/sftp_client.py` & `FlexGet-3.6.0/flexget/components/ftp/sftp_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,121 @@
+import importlib
 import logging
+import os
 import time
+from base64 import b64decode
+from dataclasses import dataclass
 from functools import partial
 from pathlib import Path, PurePath, PurePosixPath
+from stat import S_ISLNK
 from typing import Callable, List, Optional
 from urllib.parse import quote, urljoin
 
 from loguru import logger
 
 from flexget import plugin
 from flexget.entry import Entry
+from flexget.task import TaskAbort
 
 # retry configuration constants
 RETRY_INTERVAL_SEC: int = 15
 RETRY_STEP_SEC: int = 5
+HOST_KEY_TYPES: dict = {
+    'ssh-rsa': 'RSAKey',
+    'ssh-ed25519': 'Ed25519Key',
+}
 
 try:
+    import paramiko
     import pysftp
 
     logging.getLogger("paramiko").setLevel(logging.ERROR)
 except ImportError:
     pysftp = None
 
 NodeHandler = Callable[[str], None]
 
 logger = logger.bind(name='sftp_client')
 
 
+def _set_authentication_patch(self, password, private_key, private_key_pass):
+    """
+    Patch pysftp.Connection._set_authentication to support additional
+    key types
+    """
+    if password is None:
+        # Use Private Key.
+        if not private_key:
+            # Try to use default key.
+            if os.path.exists(os.path.expanduser('~/.ssh/id_rsa')):
+                private_key = '~/.ssh/id_rsa'
+            elif os.path.exists(os.path.expanduser('~/.ssh/id_dsa')):
+                private_key = '~/.ssh/id_dsa'
+            else:
+                raise pysftp.exceptions.CredentialException("No password or key specified.")
+
+        if isinstance(private_key, (paramiko.AgentKey, paramiko.RSAKey)):
+            # use the paramiko agent or rsa key
+            self._tconnect['pkey'] = private_key
+        else:
+            # isn't a paramiko AgentKey or RSAKey, try to build a
+            # key from what we assume is a path to a key
+            private_key_file = os.path.expanduser(private_key)
+            for key in [paramiko.RSAKey, paramiko.DSSKey, paramiko.Ed25519Key, paramiko.ECDSAKey]:
+                try:  # try all the keys
+                    self._tconnect['pkey'] = key.from_private_key_file(
+                        private_key_file, private_key_pass
+                    )
+                    return
+                except paramiko.SSHException:  # if it fails, try dss
+                    pass
+            raise paramiko.SSHException(f'Unknown key type: {private_key}')
+
+
+@dataclass
+class HostKey:
+    """
+    Host key used to connect to a SFTP server if not defined in known_hosts.
+    """
+
+    key_type: str
+    public_key: str
+
+
 class SftpClient:
     def __init__(
         self,
         host: str,
         port: int,
         username: str,
         password: Optional[str] = None,
         private_key: Optional[str] = None,
         private_key_pass: Optional[str] = None,
+        host_key: Optional[HostKey] = None,
         connection_tries: int = 3,
     ):
-
         if not pysftp:
             raise plugin.DependencyError(
                 issued_by='sftp_client',
                 missing='pysftp',
                 message='sftp client requires the pysftp Python module.',
             )
 
         self.host: str = host
         self.port: int = port
         self.username: str = username
         self.password: Optional[str] = password
         self.private_key: Optional[str] = private_key
         self.private_key_pass: Optional[str] = private_key_pass
+        self.host_key: Optional[HostKey] = host_key
 
         self.prefix: str = self._get_prefix()
         self._sftp: 'pysftp.Connection' = self._connect(connection_tries)
         self._handler_builder: HandlerBuilder = HandlerBuilder(
-            self._sftp, self.prefix, self.private_key, self.private_key_pass
+            self._sftp, self.prefix, self.private_key, self.private_key_pass, self.host_key
         )
 
     def list_directories(
         self,
         directories: List[str],
         recursive: bool,
         get_size: bool,
@@ -84,64 +140,79 @@
         file_handler: NodeHandler = self._handler_builder.get_file_handler(
             get_size, dirs_only, entries
         )
         unknown_handler: NodeHandler = self._handler_builder.get_unknown_handler()
 
         for directory in directories:
             try:
+                # Always normalize the root path so it's not necessary to normalised
+                # nodes as there are discovered, which means that symlinks will appear
+                # in the entry paths raw rather than been resolved to their target.
                 self._sftp.walktree(
-                    directory, file_handler, dir_handler, unknown_handler, recursive
+                    self._sftp.normalize(directory),
+                    file_handler,
+                    dir_handler,
+                    unknown_handler,
+                    recursive,
                 )
             except OSError as e:
                 logger.warning('Failed to open {} ({})', directory, str(e))
                 continue
 
         return entries
 
     def download(self, source: str, to: str, recursive: bool, delete_origin: bool) -> None:
         """
         Downloads the file specified in "source" to the destination specified in "to"
         :param source: path of the resource to download
         :param to: path of the directory to download to
         :param recursive: indicates whether to download the contents of "source" recursively
-        :param delete_origin: indicates whether to delete the source resource upon download
+        :param delete_origin: indicates whether to delete the source resource upon download, is the source
+                              is a symlink, only the symlink will be removed rather than it's target.
         """
 
         dir_handler: NodeHandler = self._handler_builder.get_null_handler()
         unknown_handler: NodeHandler = self._handler_builder.get_unknown_handler()
 
         parsed_path: PurePosixPath = PurePosixPath(source)
 
         if not self.path_exists(source):
             raise SftpError(f'Remote path does not exist: {source}')
 
+        is_symlink: bool = self.is_link(source)
         if self.is_file(source):
             source_file: str = parsed_path.name
             source_dir: str = parsed_path.parent.as_posix()
             try:
                 self._sftp.cwd(source_dir)
-                self._download_file(to, delete_origin, source_file)
+                self._download_file(to, delete_origin and not is_symlink, source_file)
             except Exception as e:
                 raise SftpError(f'Failed to download file {source} ({str(e)})')
 
-            if delete_origin:
-                self.remove_dir(source_dir)
+            if delete_origin and is_symlink:
+                self.remove_file(source)
+
         elif self.is_dir(source):
             base_path: str = parsed_path.joinpath('..').as_posix()
             dir_name: str = parsed_path.name
-            handle_file: NodeHandler = partial(self._download_file, to, delete_origin)
+            handle_file: NodeHandler = partial(
+                self._download_file, to, delete_origin and not is_symlink
+            )
 
             try:
                 self._sftp.cwd(base_path)
                 self._sftp.walktree(dir_name, handle_file, dir_handler, unknown_handler, recursive)
             except Exception as e:
                 raise SftpError(f'Failed to download directory {source} ({str(e)})')
 
             if delete_origin:
-                self.remove_dir(source)
+                if self.is_link(source):
+                    self.remove_file(source)
+                else:
+                    self.remove_dir(source)
         else:
             logger.warning('Skipping unknown file: {}', source)
 
     def upload(self, source: str, to: str) -> None:
         """
         Upload files or directories to an SFTP server
         :param source: file or directory to upload
@@ -188,14 +259,22 @@
         """
         Check if the node at a given path is a directory
         :param path: path to check
         :return: boolean indicating if the path is a directory
         """
         return self._sftp.isdir(path)
 
+    def is_link(self, path: str) -> bool:
+        """
+        Check if the node at a given path is a directory
+        :param path: path to check
+        :return: boolean indicating if the path is a directory
+        """
+        return S_ISLNK(self._sftp.sftp_client.lstat(path).st_mode)
+
     def path_exists(self, path: str) -> bool:
         """
         Check of a path exists
 
         :param path: Path to check
         :return: boolean indicating if the path exists
         """
@@ -224,49 +303,62 @@
         """
         Sets the SFTP client socket timeout
         :param socket_timeout_sec: Socket timeout in seconds
         """
         self._sftp.timeout = socket_timeout_sec
 
     def _connect(self, connection_tries: int) -> 'pysftp.Connection':
-
         tries: int = connection_tries
         retry_interval: int = RETRY_INTERVAL_SEC
 
         logger.debug('Connecting to {}', self.host)
 
         sftp: Optional['pysftp.Connection'] = None
 
         while not sftp:
             try:
+                pysftp.Connection._set_authentication = _set_authentication_patch
                 sftp = pysftp.Connection(
                     host=self.host,
                     username=self.username,
                     private_key=self.private_key,
                     password=self.password,
                     port=self.port,
                     private_key_pass=self.private_key_pass,
+                    cnopts=self._get_cnopts(),
                 )
                 logger.verbose('Connected to {}', self.host)  # type: ignore
             except Exception as e:
                 tries -= 1
+                logger.debug('Caught exception: {}', e)
                 if not tries:
-                    raise e
+                    raise TaskAbort(f'Failed to connect to {self.host}')
                 else:
                     logger.debug('Caught exception: {}', e)
                     logger.warning(
                         'Failed to connect to {}; waiting {} seconds before retrying.',
                         self.host,
                         retry_interval,
                     )
                     time.sleep(retry_interval)
                     retry_interval += RETRY_STEP_SEC
 
         return sftp
 
+    def _get_cnopts(self) -> Optional['pysftp.CnOpts']:
+        if not self.host_key:
+            return None
+        KeyClass = getattr(
+            importlib.import_module("paramiko"), HOST_KEY_TYPES[self.host_key.key_type]
+        )
+        key = KeyClass(data=b64decode(self.host_key.public_key))
+        cnopts = pysftp.CnOpts()
+        cnopts.hostkeys.add(self.host, self.host_key.key_type, key)
+        return cnopts
+
     def _upload_file(self, source: str, to: str) -> None:
         if not Path(source).exists():
             logger.warning('File no longer exists:', source)
             return
 
         destination = self._get_upload_path(source, to)
         destination_url: str = urljoin(self.prefix, destination)
@@ -285,15 +377,14 @@
             logger.verbose('Successfully uploaded {} to {}', source, destination_url)  # type: ignore
         except OSError:
             raise SftpError(f'Remote directory does not exist: {to}')
         except Exception as e:
             raise SftpError(f'Failed to upload {source} ({str(e)})')
 
     def _download_file(self, destination: str, delete_origin: bool, source: str) -> None:
-
         destination_path: str = self._get_download_path(source, destination)
         destination_dir: str = Path(destination_path).parent.as_posix()
 
         if Path(destination_path).exists():
             logger.verbose(  # type: ignore
                 'Skipping {} because destination file {} already exists.', source, destination_path
             )
@@ -368,19 +459,21 @@
 
     def __init__(
         self,
         sftp: 'pysftp.Connection',
         url_prefix: str,
         private_key: Optional[str],
         private_key_pass: Optional[str],
+        host_key: Optional[HostKey],
     ):
         self._sftp = sftp
         self._prefix = url_prefix
         self._private_key = private_key
         self._private_key_pass = private_key_pass
+        self._host_key = host_key
 
     def get_file_handler(
         self, get_size: bool, dirs_only: bool, entry_accumulator: list
     ) -> NodeHandler:
         """
         Builds a file node handler suitable for use with pysftp.Connection.walktree
 
@@ -392,14 +485,15 @@
             Handlers.handle_file,
             self._sftp,
             self._prefix,
             get_size,
             dirs_only,
             self._private_key,
             self._private_key_pass,
+            self._host_key,
             entry_accumulator,
         )
 
     def get_dir_handler(
         self, get_size: bool, files_only: bool, entry_accumulator: list
     ) -> NodeHandler:
         """
@@ -413,14 +507,15 @@
             Handlers.handle_directory,
             self._sftp,
             self._prefix,
             get_size,
             files_only,
             self._private_key,
             self._private_key_pass,
+            self._host_key,
             entry_accumulator,
         )
 
     def get_unknown_handler(self) -> NodeHandler:
         """
         Builds an unknown node handler suitable for use with pysftp.Connection.walktree
         """
@@ -439,70 +534,74 @@
         cls,
         sftp: 'pysftp.Connection',
         prefix: str,
         get_size: bool,
         dirs_only: bool,
         private_key: Optional[str],
         private_key_pass: Optional[str],
+        host_key: Optional[HostKey],
         entry_accumulator: List[Entry],
         path: str,
     ) -> None:
         """
         File node handler. Adds a file entry to entry_accumulator.
 
         :param sftp: A pysftp.Connection object
         :param logger: a logger object
         :param prefix: SFTP URL prefix
         :param get_size: boolean indicating whether to compute the size of each file
         :param dirs_only: boolean indicating whether to skip files
         :param private_key: private key path
         :param private_key_pass: private key password
+        :param host_key: Host key for the remote server if not in known_hosts
         :param entry_accumulator: a list in which to store entries
         :param path: path to handle
         """
         if dirs_only:
             return
 
         size_handler = partial(cls._file_size, sftp)
         entry = cls._get_entry(
-            sftp, prefix, size_handler, get_size, path, private_key, private_key_pass
+            sftp, prefix, size_handler, get_size, path, private_key, private_key_pass, host_key
         )
         entry_accumulator.append(entry)
 
     @classmethod
     def handle_directory(
         cls,
         sftp: 'pysftp.Connection',
         prefix: str,
         get_size: bool,
         files_only: bool,
         private_key: Optional[str],
         private_key_pass: Optional[str],
+        host_key: Optional[HostKey],
         entry_accumulator: List[Entry],
         path: str,
     ) -> None:
         """
         Directory node handler. Adds a directory entry to entry_accumulator.
 
         :param sftp: A pysftp.Connection object
         :param logger: a logger object
         :param prefix: SFTP URL prefix
         :param get_size: boolean indicating whether to compute the size of each directory
         :param files_only: Boolean indicating whether to skip directories
         :param entry_accumulator: a list in which to store entries
         :param private_key: private key path
         :param private_key_pass: private key password
+        :param host_key: Host key for the remote server if not in known_hosts
         :param path: path to handle
         """
         if files_only:
             return
 
         dir_size: Callable[[str], int] = partial(cls._dir_size, sftp)
         entry: Entry = cls._get_entry(
-            sftp, prefix, dir_size, get_size, path, private_key, private_key_pass
+            sftp, prefix, dir_size, get_size, path, private_key, private_key_pass, host_key
         )
         entry_accumulator.append(entry)
 
     @staticmethod
     def handle_unknown(path: str) -> None:
         """
         Handler for unknown nodes; logs a warning.
@@ -528,31 +627,36 @@
         sftp: 'pysftp.Connection',
         prefix: str,
         size_handler: Callable[[str], int],
         get_size,
         path: str,
         private_key: Optional[str],
         private_key_pass: Optional[str],
+        host_key: Optional[HostKey],
     ) -> Entry:
-
-        url = urljoin(prefix, quote(sftp.normalize(path)))
+        url = urljoin(prefix, quote(path))
         title = PurePosixPath(path).name
 
         entry = Entry(title, url)
 
         if get_size:
             try:
                 size = size_handler(path)
             except Exception as e:
                 logger.warning('Failed to get size for {} ({})', path, e)
                 size = -1
             entry['content_size'] = size
 
         entry['private_key'] = private_key
         entry['private_key_pass'] = private_key_pass
+        if host_key:
+            entry['host_key'] = {
+                'key_type': host_key.key_type,
+                'public_key': host_key.public_key,
+            }
 
         return entry
 
     @classmethod
     def _dir_size(cls, sftp: 'pysftp.Connection', path: str) -> int:
         sizes: List[int] = []
```

### Comparing `FlexGet-3.5.9/flexget/components/history/api.py` & `FlexGet-3.6.0/flexget/components/history/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/history/cli.py` & `FlexGet-3.6.0/flexget/components/history/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/history/db.py` & `FlexGet-3.6.0/flexget/components/history/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/history/history.py` & `FlexGet-3.6.0/flexget/components/history/history.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/imdb/api.py` & `FlexGet-3.6.0/flexget/components/imdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/imdb/db.py` & `FlexGet-3.6.0/flexget/components/imdb/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/imdb/from_imdb.py` & `FlexGet-3.6.0/flexget/components/imdb/from_imdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/imdb/imdb.py` & `FlexGet-3.6.0/flexget/components/imdb/imdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,20 +101,18 @@
         },
         'additionalProperties': False,
     }
 
     # Run later to avoid unnecessary lookups
     @plugin.priority(120)
     def on_task_filter(self, task, config):
-
         lookup = plugin.get('imdb_lookup', self).lookup
 
         # since the plugin does not reject anything, no sense going trough accepted
         for entry in task.undecided:
-
             force_accept = False
 
             try:
                 lookup(entry)
             except plugin.PluginError as e:
                 # logs skip message once trough log_once (info) and then only when ran from cmd line (w/o --cron)
                 log_once(
```

### Comparing `FlexGet-3.5.9/flexget/components/imdb/imdb_lookup.py` & `FlexGet-3.6.0/flexget/components/imdb/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/imdb/imdb_url.py` & `FlexGet-3.6.0/flexget/components/imdb/imdb_url.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/imdb/imdb_watchlist.py` & `FlexGet-3.6.0/flexget/components/imdb/imdb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/imdb/utils.py` & `FlexGet-3.6.0/flexget/components/imdb/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/irc/api.py` & `FlexGet-3.6.0/flexget/components/irc/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/irc/cli.py` & `FlexGet-3.6.0/flexget/components/irc/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/irc/irc.py` & `FlexGet-3.6.0/flexget/components/irc/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,18 +167,16 @@
         # If we have a tracker config file, load it
         tracker_config_file = config.get('tracker_file')
         if tracker_config_file:
             self.tracker_config = self.retrieve_tracker_config(tracker_config_file)
 
         channel_list = []
         if self.tracker_config is not None:
-
             # Validate config with the settings in the torrent file
             for param in self.tracker_config.find('settings'):
-
                 # Handle textbox entries
                 if param.tag == 'textbox':
                     value_name = param.get('name')
                 else:
                     value_name = param.tag
 
                 # Strip the gazelle prefix
@@ -280,15 +278,17 @@
     @classmethod
     def retrieve_tracker_config(cls, tracker_config_file):
         """
         Will attempt to retrieve the .tracker file from disk or github. Returns the parsed XML.
         :param tracker_config_file: URL or path to .tracker file
         :return: parsed XML
         """
-        base_url = 'https://raw.githubusercontent.com/autodl-community/autodl-trackers/master/'
+        base_url = (
+            'https://raw.githubusercontent.com/autodl-community/autodl-trackers/master/trackers/'
+        )
         tracker_config_file = os.path.expanduser(tracker_config_file)
 
         # First we attempt to find the file locally as-is
         if os.path.exists(tracker_config_file):
             logger.debug('Found tracker file: {}', tracker_config_file)
             return cls.read_tracker_config(tracker_config_file)
 
@@ -341,15 +341,18 @@
                         'autodl-trackers/git/trees/master?recursive=1'
                     )
                     .json()
                     .get('tree', [])
                 )
                 for t in trackers:
                     name = t.get('path', '')
-                    if not name.endswith('.tracker') or name.lower() != tracker_name.lower():
+                    if (
+                        not name.endswith('.tracker')
+                        or name.lower() != 'trackers/' + tracker_name.lower()
+                    ):
                         continue
                     tracker = requests.get(base_url + name)
                     tracker_name = name
                     break
             except (requests.RequestException, OSError) as e:
                 raise TrackerFileError(e)
         if not tracker:
```

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/list_add.py` & `FlexGet-3.6.0/flexget/components/managed_lists/list_add.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/list_clear.py` & `FlexGet-3.6.0/flexget/components/managed_lists/list_clear.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/list_match.py` & `FlexGet-3.6.0/flexget/components/managed_lists/list_match.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/list_remove.py` & `FlexGet-3.6.0/flexget/components/managed_lists/list_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/couchpotato_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/couchpotato_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/api.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/cli.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/db.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/entry_list/entry_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/entry_list/entry_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/imdb_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/imdb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/api.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/cli.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/db.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/movie_list/movie_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/movie_list/movie_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/api.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/cli.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/db.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/pending_list/pending_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/pending_list/pending_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/radarr_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/radarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/regexp_list/cli.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/regexp_list/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/regexp_list/db.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/regexp_list/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/regexp_list/regexp_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/regexp_list/regexp_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/sonarr_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/sonarr_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/subtitle_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/subtitle_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/thetvdb_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/thetvdb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/managed_lists/lists/yaml_list.py` & `FlexGet-3.6.0/flexget/components/managed_lists/lists/yaml_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notification_framework.py` & `FlexGet-3.6.0/flexget/components/notify/notification_framework.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/bark.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/bark.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/cronitor.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/cronitor.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/discord.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/discord.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/email.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/email.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/gotify.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/gotify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/ifttt.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/ifttt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/join.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/join.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/matrix.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/matrix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/microsoftteams.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/microsoftteams.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/mqtt.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/mqtt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/notifymyandroid.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/notifymyandroid.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/ntfysh.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/ntfysh.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/prowl.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/prowl.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/pushalot.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/pushalot.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/pushbullet.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/pushbullet.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/pushover.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/pushover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/rapidpush.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/rapidpush.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/slack.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/slack.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/sms_ru.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/sms_ru.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/telegram.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/toast.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/toast.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notifiers/xmpp.py` & `FlexGet-3.6.0/flexget/components/notify/notifiers/xmpp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/notify/notify.py` & `FlexGet-3.6.0/flexget/components/notify/notify.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/parsing/parsers/parser_common.py` & `FlexGet-3.6.0/flexget/components/parsing/parsers/parser_common.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/parsing/parsers/parser_guessit.py` & `FlexGet-3.6.0/flexget/components/parsing/parsers/parser_guessit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/parsing/parsers/parser_internal.py` & `FlexGet-3.6.0/flexget/components/parsing/parsers/parser_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 try:
     preferred_clock = time.process_time
 except AttributeError:
     preferred_clock = time.clock
 
 
 class ParserInternal:
-
     # movie_parser API
 
     @plugin.priority(1)
     def parse_movie(self, data, **kwargs):
         logger.debug('Parsing movie: `{}` kwargs: {}', data, kwargs)
         start = preferred_clock()
         parser = MovieParser()
```

### Comparing `FlexGet-3.5.9/flexget/components/parsing/plugin_parsing.py` & `FlexGet-3.6.0/flexget/components/parsing/plugin_parsing.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/pending_approval/api.py` & `FlexGet-3.6.0/flexget/components/pending_approval/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/pending_approval/cli.py` & `FlexGet-3.6.0/flexget/components/pending_approval/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/pending_approval/db.py` & `FlexGet-3.6.0/flexget/components/pending_approval/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/pending_approval/pending_approval.py` & `FlexGet-3.6.0/flexget/components/pending_approval/pending_approval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/rejected/api.py` & `FlexGet-3.6.0/flexget/components/rejected/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/rejected/cli.py` & `FlexGet-3.6.0/flexget/components/rejected/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/rejected/db.py` & `FlexGet-3.6.0/flexget/components/rejected/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/rejected/remember_rejected.py` & `FlexGet-3.6.0/flexget/components/rejected/remember_rejected.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/scheduler/api.py` & `FlexGet-3.6.0/flexget/components/scheduler/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/scheduler/scheduler.py` & `FlexGet-3.6.0/flexget/components/scheduler/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import hashlib
 import logging
 import os
 import struct
 
 from apscheduler.jobstores.sqlalchemy import SQLAlchemyJobStore
 from apscheduler.schedulers.background import BackgroundScheduler
@@ -122,15 +121,14 @@
     database_uri = 'sqlite:///%s' % db_filename
     jobstores = {'default': SQLAlchemyJobStore(url=database_uri)}
     # If job was meant to run within last day while daemon was shutdown, run it once when continuing
     job_defaults = {'coalesce': True, 'misfire_grace_time': 60 * 60 * 24}
     scheduler = BackgroundScheduler(
         jobstores=jobstores,
         job_defaults=job_defaults,
-        timezone=datetime.datetime.now().astimezone().tzinfo,
     )
     setup_jobs(manager)
 
 
 @event('manager.config_updated')
 def setup_jobs(manager):
     """Set up the jobs for apscheduler to run."""
```

### Comparing `FlexGet-3.5.9/flexget/components/seen/api.py` & `FlexGet-3.6.0/flexget/components/seen/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/seen/cli.py` & `FlexGet-3.6.0/flexget/components/seen/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/seen/db.py` & `FlexGet-3.6.0/flexget/components/seen/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/seen/seen.py` & `FlexGet-3.6.0/flexget/components/seen/seen.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/seen/seen_info_hash.py` & `FlexGet-3.6.0/flexget/components/seen/seen_info_hash.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/seen/seen_movies.py` & `FlexGet-3.6.0/flexget/components/seen/seen_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/all_series.py` & `FlexGet-3.6.0/flexget/components/series/all_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/api.py` & `FlexGet-3.6.0/flexget/components/series/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/cli.py` & `FlexGet-3.6.0/flexget/components/series/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/configure_series.py` & `FlexGet-3.6.0/flexget/components/series/configure_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
                 'from': {'$ref': '/schema/plugins?phase=input'},
             },
             'required': ['from'],
             'additionalProperties': False,
         }
 
     def on_task_prepare(self, task, config):
-
         series = {}
         for input_name, input_config in config.get('from', {}).items():
             input_plugin = plugin.get_plugin_by_name(input_name)
             method = input_plugin.phase_handlers['input']
             try:
                 result = method(task, input_config)
             except PluginError as e:
```

### Comparing `FlexGet-3.5.9/flexget/components/series/db.py` & `FlexGet-3.6.0/flexget/components/series/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/gen_series.py` & `FlexGet-3.6.0/flexget/components/series/gen_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/internal_estimator.py` & `FlexGet-3.6.0/flexget/components/series/internal_estimator.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/metainfo_series.py` & `FlexGet-3.6.0/flexget/components/series/metainfo_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/next_series_episodes.py` & `FlexGet-3.6.0/flexget/components/series/next_series_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/next_series_seasons.py` & `FlexGet-3.6.0/flexget/components/series/next_series_seasons.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/series.py` & `FlexGet-3.6.0/flexget/components/series/series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/series_begin.py` & `FlexGet-3.6.0/flexget/components/series/series_begin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/series_premiere.py` & `FlexGet-3.6.0/flexget/components/series/series_premiere.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/series/series_remove.py` & `FlexGet-3.6.0/flexget/components/series/series_remove.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/allyoulike.py` & `FlexGet-3.6.0/flexget/components/sites/sites/allyoulike.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/alpharatio.py` & `FlexGet-3.6.0/flexget/components/sites/sites/alpharatio.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/animeindex.py` & `FlexGet-3.6.0/flexget/components/sites/sites/animeindex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/anirena.py` & `FlexGet-3.6.0/flexget/components/sites/sites/anirena.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/archetorrent.py` & `FlexGet-3.6.0/flexget/components/sites/sites/archetorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/argenteam.py` & `FlexGet-3.6.0/flexget/components/sites/sites/argenteam.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         """
         Search for releases
         """
 
         entries = set()
 
         for search_string in entry.get('search_strings', [entry['title']]):
-
             try:
                 params = {'q': normalize_scene(search_string)}
                 resp = task.requests.get(self.base_url + 'search', params=params)
                 logger.debug('Requesting: {}', resp.url)
                 response = resp.json()
             except RequestException as e:
                 logger.error('Argenteam request failed: {}', e)
```

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/awesomehd.py` & `FlexGet-3.6.0/flexget/components/sites/sites/awesomehd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/bakabt.py` & `FlexGet-3.6.0/flexget/components/sites/sites/bakabt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/btn.py` & `FlexGet-3.6.0/flexget/components/sites/sites/btn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/cinemageddon.py` & `FlexGet-3.6.0/flexget/components/sites/sites/cinemageddon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/cpasbien.py` & `FlexGet-3.6.0/flexget/components/sites/sites/cpasbien.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/deadfrog.py` & `FlexGet-3.6.0/flexget/components/sites/sites/deadfrog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/descargas2020.py` & `FlexGet-3.6.0/flexget/components/sites/sites/descargas2020.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/ettv.py` & `FlexGet-3.6.0/flexget/components/sites/sites/ettv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/eztv.py` & `FlexGet-3.6.0/flexget/components/sites/sites/eztv.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def url_rewritable(self, task, entry):
         return urlparse(entry['url']).netloc == 'eztv.ch'
 
     def url_rewrite(self, task, entry):
         url = entry['url']
         page = None
-        for (scheme, netloc) in EZTV_MIRRORS:
+        for scheme, netloc in EZTV_MIRRORS:
             try:
                 _, _, path, params, query, fragment = urlparse(url)
                 url = urlunparse((scheme, netloc, path, params, query, fragment))
                 page = task.requests.get(url).content
             except RequestException as e:
                 logger.debug('Eztv mirror `{}` seems to be down', url)
                 continue
```

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/filelist.py` & `FlexGet-3.6.0/flexget/components/sites/sites/filelist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/filelist_api.py` & `FlexGet-3.6.0/flexget/components/sites/sites/filelist_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
             'doubleup': {'type': 'boolean', 'default': False},
         },
         'required': ['username', 'passkey'],
         'additionalProperties': False,
     }
 
     def get(self, url, params):
-
         try:
             response = requests.get(url, params=params, raise_status=False)
         except RequestException as e:
             raise plugin.PluginError(f'FileList request failed badly! {e}')
 
         if not response.ok:
             http_status = HTTPStatus(response.status_code)
@@ -112,15 +111,14 @@
         # set season/episode if series
         if entry.get('series_episode'):
             params['episode'] = entry.get('series_episode')
         if entry.get('series_season'):
             params['season'] = entry.get('series_season')
 
         for search_title in entry.get('search_strings', [entry.get('title')]):
-
             if entry.get('imdb_id'):
                 params['type'] = 'imdb'
                 params['query'] = entry.get('imdb_id')
                 params['name'] = search_title
             else:
                 params['type'] = 'name'
                 params['query'] = search_title
```

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/frenchtorrentdb.py` & `FlexGet-3.6.0/flexget/components/sites/sites/frenchtorrentdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/fuzer.py` & `FlexGet-3.6.0/flexget/components/sites/sites/fuzer.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/google_cse.py` & `FlexGet-3.6.0/flexget/components/sites/sites/google_cse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/hebits.py` & `FlexGet-3.6.0/flexget/components/sites/sites/hebits.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/hliang.py` & `FlexGet-3.6.0/flexget/components/sites/sites/hliang.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/horriblesubs.py` & `FlexGet-3.6.0/flexget/components/sites/sites/horriblesubs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/iptorrents.py` & `FlexGet-3.6.0/flexget/components/sites/sites/iptorrents.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,37 +49,44 @@
     'TV-SD-x264': 79,
     'TV-x264': 5,
     'TV-x265': 99,
     'TV-XVID': 4,
     'TV-Web-DL': 22,
 }
 
-BASE_URL = 'https://iptorrents.com'
-SEARCH_URL = 'https://iptorrents.com/t?'
-FREE_SEARCH_URL = 'https://iptorrents.com/t?free=on'
+DOMAIN = "iptorrents.com"
+BASE_URL = f"https://{DOMAIN}"
+SEARCH_URL = f"https://{DOMAIN}/t?"
+FREE_SEARCH_URL = f"https://{DOMAIN}/t?free=on"
+DELAY = "2 seconds"
 
 
 class UrlRewriteIPTorrents:
     """
     IpTorrents urlrewriter and search plugin.
 
     iptorrents:
       rss_key: xxxxxxxxx  (required)
       uid: xxxxxxxx  (required)
       password: xxxxxxxx  (required)
       category: HD
+      free: False
+      search_delay: "1 seconds"
 
       Category is any combination of: Movie-all, Movie-3D, Movie-480p,
       Movie-4K, Movie-BD-R, Movie-BD-Rip, Movie-Cam, Movie-DVD-R,
       Movie-HD-Bluray, Movie-Kids, Movie-MP4, Movie-Non-English,
       Movie-Packs, Movie-Web-DL, Movie-x265, Movie-XviD,
-
       TV-all, TV-Documentaries, TV-Sports, TV-480p, TV-BD, TV-DVD-R,
       TV-DVD-Rip, TV-MP4, TV-Mobile, TV-Non-English, TV-Packs,
       TV-Packs-Non-English, TV-SD-x264, TV-x264, TV-x265, TV-XVID, TV-Web-DL
+
+      free is a boolean to control search result filtering for freeleach torrents only.
+
+      search_delay is a timedelta string that configures rate limit for requests to iptorrents.com.
     """
 
     schema = {
         'type': 'object',
         'properties': {
             'rss_key': {'type': 'string'},
             'uid': {'oneOf': [{'type': 'integer'}, {'type': 'string'}]},
@@ -91,23 +98,29 @@
         },
         'required': ['rss_key', 'uid', 'password'],
         'additionalProperties': False,
     }
 
     # urlrewriter API
     def url_rewritable(self, task, entry):
+        """
+        Determines if the entry's URL is rewriteable (not pointing at a downloadable torrent).
+        """
         url = entry['url']
         if url.startswith(BASE_URL + '/download.php/'):
             return False
         if url.startswith(BASE_URL + '/'):
             return True
         return False
 
     # urlrewriter API
     def url_rewrite(self, task, entry):
+        """
+        Resets the entry's url to one pointing directly at a torrent.
+        """
         if 'url' not in entry:
             logger.error("Didn't actually get a URL...")
         else:
             logger.debug('Got the URL: {}', entry['url'])
         if entry['url'].startswith(SEARCH_URL):
             # use search
             results = self.search(task, entry)
@@ -115,43 +128,48 @@
                 raise UrlRewritingError("No search results found")
             # TODO: Search doesn't enforce close match to title, be more picky
             entry['url'] = results[0]['url']
 
     @plugin.internet(logger)
     def search(self, task, entry, config=None):
         """
-        Search for name from iptorrents
+        Search for name from iptorrents.
         """
 
         categories = config.get('category', 'All')
         # Make sure categories is a list
         if not isinstance(categories, list):
             categories = [categories]
 
         # If there are any text categories, turn them into their id number
         categories = [c if isinstance(c, int) else CATEGORIES[c] for c in categories]
         category_params = {str(c): '' for c in categories if str(c)}
 
         entries = set()
 
+        if not task.requests.domain_limiters.get(DOMAIN, None):
+            logger.debug('limiting requests with a delay of {}', DELAY)
+            rate_limiter = requests.TokenBucketLimiter(DOMAIN, 1, DELAY, True)
+            task.requests.add_domain_limiter(rate_limiter)
+
         for search_string in entry.get('search_strings', [entry['title']]):
             search_params = {key: value for (key, value) in category_params.items()}
 
             query = normalize_unicode(search_string)
             search_params.update({'q': query, 'qf': ''})
 
             logger.debug('searching with params: {}', search_params)
             if config.get('free'):
-                req = requests.get(
+                req = task.requests.get(
                     FREE_SEARCH_URL,
                     params=search_params,
                     cookies={'uid': str(config['uid']), 'pass': config['password']},
                 )
             else:
-                req = requests.get(
+                req = task.requests.get(
                     SEARCH_URL,
                     params=search_params,
                     cookies={'uid': str(config['uid']), 'pass': config['password']},
                 )
             logger.debug('full search URL: {}', req.url)
 
             if '/u/' + str(config['uid']) not in req.text:
@@ -164,15 +182,14 @@
             for idx, header in enumerate(torrents.thead.find('tr').findAll('th', recursive=False)):
                 header_text = header.text
                 if 'seeders' in header_text:
                     seeders_idx = idx
                 if 'leechers' in header_text:
                     leechers_idx = idx
 
-            results = torrents.findAll('tr')
             for torrent in torrents.tbody.findAll('tr', recursive=False):
                 if torrent.th and 'ac' in torrent.th.get('class'):
                     # Header column
                     continue
                 cols = list(torrent.findAll('td', recursive=False))
                 if len(cols) == 1 and 'No Torrents Found' in cols[0].text:
                     logger.debug('No results found for search {}', search_string)
@@ -198,10 +215,13 @@
                 entries.add(entry)
 
         return entries
 
 
 @event('plugin.register')
 def register_plugin():
+    """
+    Registers the plugin with FlexGet's plugin system.
+    """
     plugin.register(
         UrlRewriteIPTorrents, 'iptorrents', interfaces=['urlrewriter', 'search'], api_ver=2
     )
```

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/koreus.py` & `FlexGet-3.6.0/flexget/components/sites/sites/koreus.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/limetorrents.py` & `FlexGet-3.6.0/flexget/components/sites/sites/limetorrents.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
             except RequestException as e:
                 logger.error('Limetorrents request failed: {}', e)
                 continue
 
             soup = get_soup(page.content)
             if soup.find('a', attrs={'class': 'csprite_dl14'}) is not None:
                 for link in soup.findAll('a', attrs={'class': 'csprite_dl14'}):
-
                     row = link.find_parent('tr')
                     info_url = str(link.get('href'))
 
                     # Get the title from the URL as it's complete versus the actual Title text which gets cut off
                     title = str(link.next_sibling.get('href'))
                     title = title[: title.rfind('-torrent')].replace('-', ' ')
                     title = title[1:]
```

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/lostfilm.py` & `FlexGet-3.6.0/flexget/components/sites/sites/lostfilm.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/magnetdl.py` & `FlexGet-3.6.0/flexget/components/sites/sites/magnetdl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import random
 import re
 import time
+import unicodedata
 from urllib.parse import quote
 
 from loguru import logger
 from requests import RequestException
 
 from flexget import plugin
 from flexget.entry import Entry
@@ -150,15 +151,22 @@
                 message='CLOudscraper module required. ImportError: %s' % e,
             )
         scraper = cloudscraper.create_scraper()
         entries = []
         for search_string in entry.get('search_strings', [entry['title']]):
             logger.debug('Searching `{}`', search_string)
             try:
-                term = search_string.lower().replace(' ', '-')
+                # magnetdl.com search path accepts only [a-z0-9] and dashes/-
+                normalized_string = ''.join(
+                    c
+                    for c in unicodedata.normalize('NFD', search_string)
+                    if unicodedata.category(c) != 'Mn'
+                )
+                term = re.sub('[^a-z0-9]', '-', normalized_string.lower())
+                term = re.sub('-+', '-', term).strip('-')
                 # note: weird url convention, uses first letter of search term
                 slash = term[0]
                 url = 'https://www.magnetdl.com/{}/{}/'.format(slash, term)
                 for entry in self.parse_page(scraper, url):
                     entries.append(entry)
             except Page404Error:
                 logger.warning('Url {} returned 404', url)
```

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/morethantv.py` & `FlexGet-3.6.0/flexget/components/sites/sites/morethantv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/ncore.py` & `FlexGet-3.6.0/flexget/components/sites/sites/ncore.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/newtorrents.py` & `FlexGet-3.6.0/flexget/components/sites/sites/newtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/newznab.py` & `FlexGet-3.6.0/flexget/components/sites/sites/newznab.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/nnmclub.py` & `FlexGet-3.6.0/flexget/components/sites/sites/nnmclub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/nyaa.py` & `FlexGet-3.6.0/flexget/components/sites/sites/nyaa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/passthepopcorn.py` & `FlexGet-3.6.0/flexget/components/sites/sites/passthepopcorn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/piratebay.py` & `FlexGet-3.6.0/flexget/components/sites/sites/piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/ptn.py` & `FlexGet-3.6.0/flexget/components/sites/sites/ptn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/rarbg.py` & `FlexGet-3.6.0/flexget/components/sites/sites/rarbg.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/redirect.py` & `FlexGet-3.6.0/flexget/components/sites/sites/redirect.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/rlsbb.py` & `FlexGet-3.6.0/flexget/components/sites/sites/rlsbb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/rmz.py` & `FlexGet-3.6.0/flexget/components/sites/sites/rmz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/rss.py` & `FlexGet-3.6.0/flexget/components/sites/sites/rss.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/rutracker.py` & `FlexGet-3.6.0/flexget/components/sites/sites/rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/serienjunkies.py` & `FlexGet-3.6.0/flexget/components/sites/sites/serienjunkies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/shortened.py` & `FlexGet-3.6.0/flexget/components/sites/sites/shortened.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/site_1337x.py` & `FlexGet-3.6.0/flexget/components/sites/sites/site_1337x.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
             if config['order_by'] != 'leechers':
                 order_by = '/{0}/desc'.format(config['order_by'])
                 sort_order = 'sort-'
 
         entries = set()
 
         for search_string in entry.get('search_strings', [entry['title']]):
-
             query = '{0}search/{1}{2}/1/'.format(
                 sort_order, quote(search_string.encode('utf8')), order_by
             )
             logger.debug(
                 'Using search params: {}; ordering by: {}', search_string, order_by or 'default'
             )
             try:
```

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/site_rutracker.py` & `FlexGet-3.6.0/flexget/components/sites/sites/site_rutracker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/solidtorrents.py` & `FlexGet-3.6.0/flexget/components/sites/sites/solidtorrents.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/torrent_cache.py` & `FlexGet-3.6.0/flexget/components/sites/sites/torrent_cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/torrentday.py` & `FlexGet-3.6.0/flexget/components/sites/sites/torrentday.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         # If there are any text categories, turn them into their id number
         categories = [c if isinstance(c, int) else CATEGORIES[c] for c in categories]
         params = {'cata': 'yes', 'clear-new': 1}
         params.update({str(c): 1 for c in categories})
 
         entries = set()
         for search_string in entry.get('search_strings', [entry['title']]):
-
             url = 'https://www.torrentday.com/t'
             params['q'] = normalize_unicode(search_string).replace(':', '')
             cookies = {
                 'uid': str(config['uid']),
                 'pass': config['passkey'],
                 '__cfduid': config['cfduid'],
             }
```

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/torrentleech.py` & `FlexGet-3.6.0/flexget/components/sites/sites/torrentleech.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/torrentz.py` & `FlexGet-3.6.0/flexget/components/sites/sites/torrentz.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/wordpress.py` & `FlexGet-3.6.0/flexget/components/sites/sites/wordpress.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/sites/yts.py` & `FlexGet-3.6.0/flexget/components/sites/sites/yts.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/urlrewrite.py` & `FlexGet-3.6.0/flexget/components/sites/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/urlrewrite_search.py` & `FlexGet-3.6.0/flexget/components/sites/urlrewrite_search.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/urlrewriting.py` & `FlexGet-3.6.0/flexget/components/sites/urlrewriting.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/sites/utils.py` & `FlexGet-3.6.0/flexget/components/sites/utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/status/api.py` & `FlexGet-3.6.0/flexget/components/status/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/status/cli.py` & `FlexGet-3.6.0/flexget/components/status/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/status/db.py` & `FlexGet-3.6.0/flexget/components/status/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/status/status.py` & `FlexGet-3.6.0/flexget/components/status/status.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/thetvdb/api.py` & `FlexGet-3.6.0/flexget/components/thetvdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/thetvdb/api_tvdb.py` & `FlexGet-3.6.0/flexget/components/thetvdb/api_tvdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/thetvdb/thetvdb_lookup.py` & `FlexGet-3.6.0/flexget/components/thetvdb/thetvdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/tmdb/api.py` & `FlexGet-3.6.0/flexget/components/tmdb/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/tmdb/api_tmdb.py` & `FlexGet-3.6.0/flexget/components/tmdb/api_tmdb.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/tmdb/tmdb_lookup.py` & `FlexGet-3.6.0/flexget/components/tmdb/tmdb_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/trakt/api.py` & `FlexGet-3.6.0/flexget/components/trakt/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/trakt/api_trakt.py` & `FlexGet-3.6.0/flexget/components/trakt/api_trakt.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/trakt/cli.py` & `FlexGet-3.6.0/flexget/components/trakt/cli.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/trakt/db.py` & `FlexGet-3.6.0/flexget/components/trakt/db.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/trakt/next_trakt_episodes.py` & `FlexGet-3.6.0/flexget/components/trakt/next_trakt_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/trakt/trakt_calendar.py` & `FlexGet-3.6.0/flexget/components/trakt/trakt_calendar.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/trakt/trakt_list.py` & `FlexGet-3.6.0/flexget/components/trakt/trakt_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/trakt/trakt_lookup.py` & `FlexGet-3.6.0/flexget/components/trakt/trakt_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/tvmaze/api.py` & `FlexGet-3.6.0/flexget/components/tvmaze/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/tvmaze/api_tvmaze.py` & `FlexGet-3.6.0/flexget/components/tvmaze/api_tvmaze.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/tvmaze/tvmaze_lookup.py` & `FlexGet-3.6.0/flexget/components/tvmaze/tvmaze_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/variables/api.py` & `FlexGet-3.6.0/flexget/components/variables/api.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/components/variables/variables.py` & `FlexGet-3.6.0/flexget/components/variables/variables.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/config_schema.py` & `FlexGet-3.6.0/flexget/config_schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/db_schema.py` & `FlexGet-3.6.0/flexget/db_schema.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/entry.py` & `FlexGet-3.6.0/flexget/entry.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/event.py` & `FlexGet-3.6.0/flexget/event.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ipc.py` & `FlexGet-3.6.0/flexget/ipc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/log.py` & `FlexGet-3.6.0/flexget/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-import codecs
 import collections
 import contextlib
 import functools
-import io
 import logging
 import logging.handlers
 import os
 import sys
 import threading
 import uuid
 import warnings
 from typing import Callable, Deque, Iterator, List, Optional, Union
 
-import colorama
 import loguru
 from loguru import logger
 
+import flexget
 from flexget import __version__
+from flexget.event import event
 from flexget.utils.tools import io_encoding
 
 # A level more detailed than INFO
 VERBOSE = 15
 # environment variables to modify rotating log parameters from defaults of 1 MB and 9 files
 ENV_MAXBYTES = 'FLEXGET_LOG_MAXBYTES'
 ENV_MAXCOUNT = 'FLEXGET_LOG_MAXCOUNT'
@@ -161,17 +160,18 @@
     std_logger.addHandler(InterceptHandler())
 
 
 def start(
     filename: str = None, level: str = 'INFO', to_console: bool = True, to_file: bool = True
 ) -> None:
     """After initialization, start file logging."""
-    global _logging_started
+    global _logging_started, _startup_buffer, _startup_buffer_id
 
     assert _logging_configured
+
     if _logging_started:
         return
 
     if level == 'NONE':
         return
 
     # Make sure stdlib logger is set so that dependency logging gets propagated
@@ -190,30 +190,21 @@
 
     # without --cron we log to console
     if to_console:
         if not sys.stdout:
             logger.debug("No sys.stdout, can't log to console.")
         else:
             # Make sure we don't send any characters that the current terminal doesn't support printing
-            if sys.version_info >= (3, 7):
-                sys.stdout.reconfigure(errors='replace')
-                out = sys.stdout
-            else:
-                out = io.TextIOWrapper(sys.stdout.buffer, encoding=io_encoding, errors='replace')
-                # Loguru only autodetects whether we need to wrap the stream only when it's sys.__stdout__
-                # since we've already wrapped it we need to add the colorama support ourselves
-                if os.name == "nt":
-                    out = colorama.AnsiToWin32(
-                        out, convert=True, strip=False, autoreset=False
-                    ).stream
-            logger.add(out, level=level, format=LOG_FORMAT, filter=_log_filterer)
+            sys.stdout.reconfigure(errors='replace')
+            logger.add(sys.stdout, level=level, format=LOG_FORMAT, filter=_log_filterer)
 
-    # flush what we have stored from the plugin initialization
-    global _startup_buffer, _startup_buffer_id
-    if _startup_buffer_id:
+    if _startup_buffer_id is not None:
         logger.remove(_startup_buffer_id)
+        _startup_buffer_id = None
+
+    # flush what we have stored from the plugin initialization
+    if _startup_buffer:
         for record in _startup_buffer:
             level, message = record['level'].name, record['message']
             logger.patch(lambda r: r.update(record)).log(level, message)
         _startup_buffer = []
-        _startup_buffer_id = None
     _logging_started = True
```

### Comparing `FlexGet-3.5.9/flexget/manager.py` & `FlexGet-3.6.0/flexget/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,21 +42,15 @@
 Base = declarative_base()
 Session: Type[ContextSession] = sessionmaker(class_=ContextSession)
 
 import flexget.log  # noqa
 from flexget import config_schema, db_schema, plugin  # noqa
 from flexget.event import fire_event  # noqa
 from flexget.ipc import IPCClient, IPCServer  # noqa
-from flexget.options import (  # noqa
-    CoreArgumentParser,
-    ParserError,
-    get_parser,
-    manager_parser,
-    unicode_argv,
-)
+from flexget.options import CoreArgumentParser, ParserError, get_parser, manager_parser  # noqa
 from flexget.task import Task  # noqa
 from flexget.task_queue import TaskQueue  # noqa
 from flexget.terminal import console, get_console_output  # noqa
 
 if TYPE_CHECKING:
     from flexget.tray_icon import TrayIcon
     from flexget.utils.simple_persistence import SimplePersistence
@@ -120,27 +114,24 @@
     * manager.daemon.completed
     * manager.db_cleanup
     """
 
     unit_test = False
     options: argparse.Namespace
 
-    def __init__(self, args: Optional[List[str]]) -> None:
+    def __init__(self, args: List[str]) -> None:
         """
         :param args: CLI args
         """
         global manager
         if not self.unit_test:
             assert not manager, 'Only one instance of Manager should be created at a time!'
         elif manager:
             logger.info('last manager was not torn down correctly')
 
-        if args is None:
-            # Decode all arguments to unicode before parsing
-            args = unicode_argv()[1:]
         self.args = args
         self.autoreload_config = False
         self.config_file_hash: Optional[str] = None
         self.config_base: str = ''
         self.config_name: str = ''
         self.config_path: str = ''
         self.log_filename: str = ''
@@ -154,20 +145,20 @@
         self.ipc_server: IPCServer
         self.task_queue: TaskQueue
         self.persist: 'SimplePersistence'
         self.initialized = False
 
         self.config: Dict = {}
 
-        self.options = self._init_options(self.args)
-        try:
-            self._init_config(create=False)
-        except Exception:
-            flexget.log.start(level=self.options.loglevel, to_file=False)
-            raise
+        self.options = self.parse_initial_options(args)
+        self._init_config(create=False)
+        # When we are in test mode, we use a different lock file and db
+        if self.options.test:
+            self.lockfile = os.path.join(self.config_base, f'.test-{self.config_name}-lock')
+        self._init_logging()
 
         manager = self
 
         logger.debug('sys.defaultencoding: {}', sys.getdefaultencoding())
         logger.debug('sys.getfilesystemencoding: {}', sys.getfilesystemencoding())
         logger.debug('flexget detected io encoding: {}', io_encoding)
         logger.debug('os.path.supports_unicode_filenames: {}', os.path.supports_unicode_filenames)
@@ -183,39 +174,36 @@
 
     def _add_tray_icon_items(self, tray_icon: 'TrayIcon'):
         tray_icon.add_menu_item(text='Shutdown', action=self.shutdown, index=2)
         tray_icon.add_menu_item(text='Reload Config', action=self.load_config, index=3)
         tray_icon.add_menu_separator(index=4)
 
     @staticmethod
-    def _init_options(args: List[str]) -> argparse.Namespace:
-        """Initialize argument parsing"""
+    def parse_initial_options(args: List[str]) -> argparse.Namespace:
+        """Parse what we can from cli args before plugins are loaded."""
         try:
             options = CoreArgumentParser().parse_known_args(args, do_help=False)[0]
         except ParserError as exc:
             try:
                 # If a non-built-in command was used, we need to parse with a parser that
                 # doesn't define the subparsers
                 options = manager_parser.parse_known_args(args, do_help=False)[0]
             except ParserError:
                 manager_parser.print_help()
                 print(f'\nError: {exc.message}')
                 sys.exit(1)
         return options
 
-    def _init_logging(self, to_file: bool = True) -> None:
-        """Initialize logging facilities"""
+    def _init_logging(self) -> None:
+        """Initialize logging variables"""
         log_file = os.path.expanduser(self.options.logfile)
         # If an absolute path is not specified, use the config directory.
         if not os.path.isabs(log_file):
             log_file = os.path.join(self.config_base, log_file)
         self.log_filename = log_file
-        flexget.log.start(
-            log_file, self.options.loglevel, to_file=to_file, to_console=not self.options.cron
-        )
 
     def initialize(self) -> None:
         """
         Load plugins, database, and config. Also initializes (but does not start) the task queue and ipc server.
         This should only be called after obtaining a lock.
         """
         if self.initialized:
@@ -338,22 +326,18 @@
         """
         Starting point when executing from commandline, dispatch execution to correct destination.
 
         If there is a FlexGet process with an ipc server already running, the command will be sent there for execution
         and results will be streamed back.
         If not, this will attempt to obtain a lock, initialize the manager, and run the command here.
         """
-        # When we are in test mode, we use a different lock file and db
-        if self.options.test:
-            self.lockfile = os.path.join(self.config_base, f'.test-{self.config_name}-lock')
         # If another process is started, send the execution to the running process
         ipc_info = self.check_ipc_info()
         # If we are connecting to a running daemon, we don't want to log to the log file,
         # the daemon is already handling that.
-        self._init_logging(to_file=not ipc_info)
         if ipc_info:
             console(
                 'There is a FlexGet process already running for this config, sending execution there.'
             )
             logger.debug('Sending command to running FlexGet process: {}', self.args)
             try:
                 client = IPCClient(ipc_info['port'], ipc_info['password'])
@@ -1071,14 +1055,14 @@
             with codecs.open(filename, 'w', encoding='utf-8') as outfile:
                 outfile.writelines(flexget.log.debug_buffer)
                 traceback.print_exc(file=outfile)
             logger.critical(
                 'An unexpected crash has occurred. Writing crash report to {}. '
                 'Please verify you are running the latest version of flexget by using "flexget -V" '
                 'from CLI or by using version_checker plugin'
-                ' at http://flexget.com/wiki/Plugins/version_checker. '
+                ' at https://flexget.com/Plugins/version_checker. '
                 'You are currently using version {}',
                 filename,
                 get_current_flexget_version(),
             )
         logger.opt(exception=True).debug('Traceback:')
         return traceback.format_exc()
```

### Comparing `FlexGet-3.5.9/flexget/options.py` & `FlexGet-3.6.0/flexget/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,14 @@
 from flexget.utils.tools import get_current_flexget_version, get_latest_flexget_version_number
 
 _UNSET = object()
 
 core_parser: Optional['CoreArgumentParser'] = None
 
 
-def unicode_argv() -> List[str]:
-    """Like sys.argv, but decodes all arguments."""
-    args = []
-    for arg in sys.argv:
-        if isinstance(arg, bytes):
-            arg = arg.decode(sys.getfilesystemencoding())
-        args.append(arg)
-    return args
-
-
 def get_parser(command: str = None) -> 'ArgumentParser':
     global core_parser
     if not core_parser:
         core_parser = CoreArgumentParser()
         # Add all plugin options to the parser
         fire_event('options.register')
     if command:
@@ -279,15 +269,15 @@
 
     def __init__(self, **kwargs):
         """
         :param nested_namespace_name: When used as a subparser, options from this parser will be stored nested under
             this attribute name in the root parser's namespace
         """
         # Do this early, so even option processing stuff is caught
-        if '--bugreport' in unicode_argv():
+        if '--bugreport' in sys.argv:
             self._debug_tb_callback()
 
         self.subparsers = None
         self.raise_errors = None
         add_help = kwargs.pop('add_help', True)
         kwargs['add_help'] = False
         ArgParser.__init__(self, **kwargs)
@@ -365,16 +355,15 @@
     def parse_known_args(
         self,
         args: List[str] = None,
         namespace: Namespace = None,
         do_help: bool = None,
     ):
         if args is None:
-            # Decode all arguments to unicode before parsing
-            args = unicode_argv()[1:]
+            args = sys.argv[1:]
         if namespace is None:
             namespace = ScopedNamespace()
         old_do_help = ArgumentParser.do_help
         if do_help is not None:
             ArgumentParser.do_help = do_help
         try:
             namespace, args = super().parse_known_args(args, namespace)
```

### Comparing `FlexGet-3.5.9/flexget/plugin.py` & `FlexGet-3.6.0/flexget/plugin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/check.py` & `FlexGet-3.6.0/flexget/plugins/cli/check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/cli_config.py` & `FlexGet-3.6.0/flexget/plugins/cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/database.py` & `FlexGet-3.6.0/flexget/plugins/cli/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/debug_info.py` & `FlexGet-3.6.0/flexget/plugins/cli/debug_info.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/doc.py` & `FlexGet-3.6.0/flexget/plugins/cli/doc.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/explain_sql.py` & `FlexGet-3.6.0/flexget/plugins/cli/explain_sql.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/filters.py` & `FlexGet-3.6.0/flexget/plugins/cli/filters.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/inject.py` & `FlexGet-3.6.0/flexget/plugins/cli/inject.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/perf_tests.py` & `FlexGet-3.6.0/flexget/plugins/cli/perf_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         return
 
     # commence testing
 
     log_query_count('test')
     start_time = time.time()
     for url in track(imdb_urls, description='Benchmarking...'):
-
         # movie = session.query(Movie).filter(Movie.url == url).first()
         # movie = session.query(Movie).options(subqueryload(Movie.genres)).filter(Movie.url == url).one()
 
         movie = (
             session.query(Movie)
             .options(
                 joinedload(Movie.genres),
```

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/performance.py` & `FlexGet-3.6.0/flexget/plugins/cli/performance.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/plugins.py` & `FlexGet-3.6.0/flexget/plugins/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/templates.py` & `FlexGet-3.6.0/flexget/plugins/cli/templates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/try_regexp.py` & `FlexGet-3.6.0/flexget/plugins/cli/try_regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/web.py` & `FlexGet-3.6.0/flexget/plugins/cli/web.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/wiki_qualities.py` & `FlexGet-3.6.0/flexget/plugins/cli/wiki_qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/cli/win32_service.py` & `FlexGet-3.6.0/flexget/plugins/cli/win32_service.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/clients/aria2.py` & `FlexGet-3.6.0/flexget/plugins/clients/aria2.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/clients/deluge.py` & `FlexGet-3.6.0/flexget/plugins/clients/deluge.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/clients/nzbget.py` & `FlexGet-3.6.0/flexget/plugins/clients/nzbget.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/clients/pyload.py` & `FlexGet-3.6.0/flexget/plugins/clients/pyload.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,19 +151,25 @@
             add_package_command = 'add_package'
             set_package_data_command = 'set_package_date'
 
         hoster = config.get('hoster', self.DEFAULT_HOSTER)
 
         for entry in task.accepted:
             # bunch of urls now going to check
-            content = entry.get('description', '') + ' ' + quote(entry['url'])
-            content = json.dumps(content)
+            contents = []
+            description = entry.get('description')
+            if description is not None:
+                contents.append(description)
+            contents.append(quote(entry['url']))
+            content = " ".join(contents)
+
+            content = repr(content)
 
             if is_pyload_ng:
-                url = entry['url'] if config.get('parse_url', self.DEFAULT_PARSE_URL) else ''
+                url = repr(entry['url'] if config.get('parse_url', self.DEFAULT_PARSE_URL) else '')
             else:
                 url = (
                     json.dumps(entry['url'])
                     if config.get('parse_url', self.DEFAULT_PARSE_URL)
                     else "''"
                 )
 
@@ -218,16 +224,16 @@
                     name = entry.render(name)
                 except RenderError as e:
                     name = entry['title']
                     logger.error('Error rendering jinja event: {}', e)
 
                 if is_pyload_ng:
                     data = {
-                        'name': name.encode('ascii', 'ignore').decode(),
-                        'links': urls,
+                        'name': repr(name.encode('ascii', 'ignore').decode()),
+                        'links': repr(urls),
                         'dest': dest,
                     }
                 else:
                     data = {
                         'name': json.dumps(name.encode('ascii', 'ignore').decode()),
                         'links': json.dumps(urls),
                         'dest': json.dumps(dest),
```

### Comparing `FlexGet-3.5.9/flexget/plugins/clients/qbittorrent.py` & `FlexGet-3.6.0/flexget/plugins/clients/qbittorrent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
+from datetime import datetime
 
 from loguru import logger
 from requests import Session
 from requests.exceptions import RequestException
 
 from flexget import plugin
+from flexget.entry import Entry
 from flexget.event import event
 from flexget.utils.template import RenderError
 
 logger = logger.bind(name='qbittorrent')
 
 
 class OutputQBitTorrent:
@@ -220,15 +222,14 @@
         config.setdefault('maxupspeed', 0)
         config.setdefault('maxdownspeed', 0)
         config.setdefault('fail_html', True)
         return config
 
     def add_entries(self, task, config):
         for entry in task.accepted:
-
             form_data = {}
             try:
                 save_path = entry.render(entry.get('path', config.get('path', '')))
                 if save_path:
                     form_data['savepath'] = save_path
             except RenderError as e:
                 logger.error('Error setting path for {}: {}', entry['title'], e)
@@ -319,10 +320,84 @@
         """Add torrents to qBittorrent at exit."""
         if task.accepted:
             config = self.prepare_config(config)
             self.connect(config)
             self.add_entries(task, config)
 
 
+class FromQBitTorrent:
+    schema = {
+        'type': 'object',
+        'properties': {
+            'category': {'type': 'string'},
+            'completed': {'type': 'boolean'},
+            'username': {'type': 'string'},
+            'password': {'type': 'string'},
+            'host': {'type': 'string'},
+            'port': {'type': 'integer'},
+        },
+        'additionalProperties': False,
+        'required': ['username', 'password', 'host', 'port'],
+    }
+
+    @staticmethod
+    def client(host: str, port: int, username: str, password: str):
+        """
+        Import client or abort task
+        """
+        try:
+            import qbittorrentapi
+        except ImportError:
+            raise plugin.DependencyError(issued_by='from_qbittorrent', missing='qbittorrent-api')
+
+        return qbittorrentapi.Client(host=host, port=port, username=username, password=password)
+
+    def on_task_input(self, task, config):
+        client = self.client(
+            config['host'], int(config['port']), config['username'], config['password']
+        )
+
+        for torrent in client.torrents_info():
+            if 'category' in config:
+                logger.debug("filtered `%s` by wrong category" % torrent['name'])
+                if torrent['category'] != config['category']:
+                    continue
+
+            if 'completed' in config:
+                if not torrent.state_enum.is_complete:
+                    logger.debug("filtered `%s` by not completed" % torrent['name'])
+                    continue
+
+            yield Entry(
+                title=torrent['name'],
+                url=torrent['magnet_uri'],
+                content_files=[f['name'] for f in torrent.files],
+                content_size=torrent['size'] // 1024 // 1024,
+                torrent_info_hash=torrent['infohash_v1'],
+                torrent_info_hash_v2=torrent['infohash_v2'],
+                torrent_seeds=torrent['num_seeds'],
+                torrent_peers=torrent['num_leechs'],
+                qbittorrent_ratio=torrent['ratio'],
+                qbittorrent_category=torrent['category'],
+                qbittorrent_state=torrent['state'],
+                qbittorrent_eta=torrent['eta'],
+                qbittorrent_added_on=datetime.fromtimestamp(torrent['added_on']),
+                qbittorrent_completion_on=datetime.fromtimestamp(torrent['completion_on']),
+                qbittorrent_completed_path=torrent['content_path'],
+                qbittorrent_download_path=torrent['download_path'],
+                qbittorrent_save_path=torrent['save_path'],
+                qbittorrent_size=torrent['size'],
+                qbittorrent_dl_speed=torrent['dlspeed'],
+                qbittorrent_up_speed=torrent['upspeed'],
+                qbittorrent_is_checking=torrent.state_enum.is_checking,
+                qbittorrent_is_complete=torrent.state_enum.is_complete,
+                qbittorrent_is_downloading=torrent.state_enum.is_downloading,
+                qbittorrent_is_errored=torrent.state_enum.is_errored,
+                qbittorrent_is_paused=torrent.state_enum.is_paused,
+                qbittorrent_is_uploading=torrent.state_enum.is_uploading,
+            )
+
+
 @event('plugin.register')
 def register_plugin():
     plugin.register(OutputQBitTorrent, 'qbittorrent', api_ver=2)
+    plugin.register(FromQBitTorrent, 'from_qbittorrent', api_ver=2)
```

### Comparing `FlexGet-3.5.9/flexget/plugins/clients/rtorrent.py` & `FlexGet-3.6.0/flexget/plugins/clients/rtorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,14 @@
         for field in ['up_total', 'down_total', 'down_rate', 'timestamp_finished']:
             if field in fields:
                 fields[fields.index(field)] = field.replace('_', '.')
 
         return fields
 
     def load(self, raw_torrent, fields=None, start=False, mkdir=True):
-
         if fields is None:
             fields = {}
         # First param is empty 'target'
         params = ['', xmlrpc_client.Binary(raw_torrent)]
 
         # Additional fields to set
         for key, val in fields.items():
@@ -447,15 +446,14 @@
         # our temp .torrent files
         if config['action'] == 'add' and 'download' not in task.config:
             download = plugin.get('download', self)
             download.get_temp_files(task, handle_magnets=True, fail_html=True)
 
     @plugin.priority(135)
     def on_task_output(self, task, config):
-
         client = RTorrent(
             os.path.expanduser(config['uri']),
             username=config.get('username'),
             password=config.get('password'),
             digest_auth=config['digest_auth'],
             session=task.requests,
         )
@@ -562,15 +560,14 @@
             client.update(info_hash, options)
             logger.verbose('Updated {} ({}) in rtorrent ', entry['title'], info_hash)
         except xmlrpc_client.Error as e:
             entry.fail('Failed to update: %s' % str(e))
             return
 
     def add_entry(self, client, entry, options, start=True, mkdir=False, fast_resume=False):
-
         if 'torrent_info_hash' not in entry:
             entry.fail('missing torrent_info_hash')
             return
 
         if entry['url'].startswith('magnet:'):
             torrent_raw = 'd10:magnet-uri%d:%se' % (len(entry['url']), entry['url'])
             torrent_raw = torrent_raw.encode('ascii')
```

### Comparing `FlexGet-3.5.9/flexget/plugins/clients/transmission.py` & `FlexGet-3.6.0/flexget/plugins/clients/transmission.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,60 @@
-import base64
 import os
+import pathlib
 import re
 from datetime import datetime, timedelta
 from fnmatch import fnmatch
 from functools import partial
 from netrc import NetrcParseError, netrc
 from time import sleep
+from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
+try:
+    import importlib.metadata as importlib_metadata
+except ImportError:
+    import importlib_metadata  # TODO: remove this after we drop python 3.7
+
+import packaging.specifiers
+import packaging.version
 from loguru import logger
 
 from flexget import plugin
 from flexget.config_schema import one_or_more
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.utils.pathscrub import pathscrub
 from flexget.utils.template import RenderError
 from flexget.utils.tools import parse_timedelta
 
 try:
-    import requests.exceptions
-    import transmission_rpc as transmissionrpc
-    from transmission_rpc import TransmissionError
+    import transmission_rpc
+    from transmission_rpc.error import (
+        TransmissionAuthError,
+        TransmissionConnectError,
+        TransmissionError,
+        TransmissionTimeoutError,
+    )
 except ImportError:
     # If transmissionrpc is not found, errors will be shown later
-    pass
+    transmission_rpc = None
+    TransmissionError = None
+    TransmissionAuthError = None
+    TransmissionConnectError = None
+    TransmissionTimeoutError = None
+
+if TYPE_CHECKING:
+    from transmission_rpc import Torrent
 
 logger = logger.bind(name='transmission')
 
+__version__ = '>=4.1.4,<5.0.0'
+__package__ = 'transmission-rpc'
+__requirement__ = packaging.specifiers.SpecifierSet(__version__)
+
 
 class TransmissionBase:
     def prepare_config(self, config):
         if isinstance(config, bool):
             config = {'enabled': config}
         config.setdefault('enabled', True)
         config.setdefault('host', 'localhost')
@@ -45,103 +68,104 @@
                 )
             except OSError as e:
                 logger.error('netrc: unable to open: {}', e.filename)
             except NetrcParseError as e:
                 logger.error('netrc: {}, file: {}, line: {}', e.msg, e.filename, e.lineno)
         return config
 
-    def create_rpc_client(self, config) -> 'transmissionrpc.Client':
+    def create_rpc_client(self, config) -> 'transmission_rpc.Client':
         user, password = config.get('username'), config.get('password')
         urlo = urlparse(config['host'])
 
         if urlo.scheme == '':
             urlo = urlparse('http://' + config['host'])
 
         protocol = urlo.scheme if urlo.scheme else 'http'
         port = str(urlo.port) if urlo.port else config['port']
         path = urlo.path.rstrip('rpc') if urlo.path else '/transmission/'
 
         logger.debug('Connecting to {}://{}:{}{}', protocol, urlo.hostname, port, path)
 
         try:
-            cli = transmissionrpc.Client(
+            cli = transmission_rpc.Client(
                 protocol=protocol,
                 host=urlo.hostname,
                 port=port,
                 path=path,
                 username=user,
                 password=password,
+                timeout=30,
             )
-        except TransmissionError as e:
-            if e.original and e.original.code == 401:
-                raise plugin.PluginError(
-                    "Username/password for transmission is incorrect. Cannot connect."
-                )
-            else:
-                raise plugin.PluginError("Error connecting to transmission: %s" % e.message)
-        except requests.exceptions.ConnectTimeout as e:
+        except TransmissionAuthError as e:
+            raise plugin.PluginError(
+                "Username/password for transmission is incorrect. Cannot connect."
+            )
+        except TransmissionTimeoutError as e:
             raise plugin.PluginError("Cannot connect to transmission: Connection timed out.")
-        except requests.exceptions.ConnectionError as e:
+        except TransmissionConnectError as e:
             raise plugin.PluginError("Error connecting to transmission: %s" % e.args[0].reason)
-        except ValueError as e:
+        except TransmissionError as e:
             raise plugin.PluginError("Error connecting to transmission")
         return cli
 
-    def torrent_info(self, torrent, config):
-        done = torrent.totalSize > 0
+    def torrent_info(self, torrent: 'Torrent', config):
+        done = torrent.total_size > 0
         vloc = None
         best = None
-        for t in torrent.files().items():
-            tf = t[1]
-            if tf['selected']:
-                if tf['size'] <= 0 or tf['completed'] < tf['size']:
+        for _, tf in enumerate(torrent.get_files()):
+            if tf.selected:
+                if tf.size <= 0 or tf.completed < tf.size:
                     done = False
                     break
-                if not best or tf['size'] > best[1]:
-                    best = (tf['name'], tf['size'])
+                if not best or tf.size > best[1]:
+                    best = (tf.name, tf.size)
         if (
             done
             and best
-            and (100 * float(best[1]) / float(torrent.totalSize))
+            and (100 * float(best[1]) / float(torrent.total_size))
             >= (config['main_file_ratio'] * 100)
         ):
-            vloc = ('%s/%s' % (torrent.downloadDir, best[0])).replace('/', os.sep)
+            vloc = ('%s/%s' % (torrent.download_dir, best[0])).replace('/', os.sep)
         return done, vloc
 
-    def check_seed_limits(self, torrent, session):
+    def check_seed_limits(self, torrent: 'Torrent', session):
         seed_limit_ok = True  # will remain if no seed ratio defined
         idle_limit_ok = True  # will remain if no idle limit defined
 
-        if torrent.seedRatioMode == 1:  # use torrent's own seed ratio limit
-            seed_limit_ok = torrent.uploadRatio >= torrent.seedRatioLimit
-        elif torrent.seedRatioMode == 0:  # use global rules
+        if torrent.get('seedRatioMode') == 1:  # use torrent's own seed ratio limit
+            seed_limit_ok = torrent.upload_ratio >= torrent.seed_ratio_limit
+        elif torrent.get('seedRatioMode') == 0:  # use global rules
             if session.seedRatioLimited:
-                seed_limit_ok = torrent.uploadRatio >= session.seedRatioLimit
+                seed_limit_ok = torrent.upload_ratio >= session.seedRatioLimit
 
-        if torrent.seedIdleMode == 1:  # use torrent's own idle limit
+        if torrent.get('seedIdleMode') == 1:  # use torrent's own idle limit
             idle_limit_ok = (
-                torrent.date_active + timedelta(minutes=torrent.seedIdleLimit)
+                torrent.activity_date + timedelta(minutes=torrent.seed_idle_limit)
                 < datetime.now().astimezone()
             )
-        elif torrent.seedIdleMode == 0:  # use global rules
+        elif torrent.get('seedIdleMode') == 0:  # use global rules
             if session.idle_seeding_limit_enabled:
                 idle_limit_ok = (
-                    torrent.date_active + timedelta(minutes=session.idle_seeding_limit)
+                    torrent.activity_date + timedelta(minutes=session.idle_seeding_limit)
                     < datetime.now().astimezone()
                 )
 
         return seed_limit_ok, idle_limit_ok
 
     def on_task_start(self, task, config):
-        try:
-            import transmission_rpc as transmissionrpc
-            from transmission_rpc import TransmissionError  # noqa
-        except:
+        if transmission_rpc is None:
             raise plugin.PluginError(
-                'transmission-rpc module version 3.0 or higher required.', logger
+                f'{__package__} module version {__version__} required.', logger
+            )
+
+        v = importlib_metadata.version(__package__)
+        if not __requirement__.contains(v):
+            raise plugin.PluginError(
+                f'{__package__} module version mismatch, requiring {__package__}{__version__}',
+                logger,
             )
 
         # Mark rpc client for garbage collector so every task can start
         # a fresh new according its own config - fix to bug #2804
         config = self.prepare_config(config)
         if config['enabled']:
             if task.options.test:
@@ -194,74 +218,77 @@
                 seed_ratio_ok and idle_limit_ok and torrent.progress == 100
             ):
                 continue
             entry = Entry(
                 title=torrent.name,
                 url='',
                 torrent_info_hash=torrent.hashString,
-                content_size=torrent.totalSize / (1024 * 1024),
+                content_size=torrent.total_size / (1024 * 1024),
             )
             # Location of torrent is only valid if transmission is on same machine as flexget
             if config['host'] in ('localhost', '127.0.0.1'):
-                entry['location'] = torrent.torrentFile
-                entry['url'] = 'file://' + torrent.torrentFile
-            for attr in [
-                'id',
-                'activityDate',
-                'comment',
-                'desiredAvailable',
-                'downloadDir',
-                'isFinished',
-                'isPrivate',
-                'isStalled',
-                'leftUntilDone',
-                'ratio',
-                'status',
-                'date_active',
-                'date_added',
-                'date_done',
-                'date_started',
-                'errorString',
-                'priority',
-                'progress',
-                'secondsDownloading',
-                'secondsSeeding',
-                'torrentFile',
-            ]:
+                entry['location'] = torrent.torrent_file
+                entry['url'] = pathlib.Path(torrent.torrent_file)
+            for attr, field in {
+                'id': 'id',
+                'activityDate': 'activity_date',
+                'comment': 'comment',
+                'desiredAvailable': 'desired_available',
+                'downloadDir': 'download_dir',
+                'isFinished': 'is_finished',
+                'isPrivate': 'is_private',
+                'isStalled': 'is_stalled',
+                'leftUntilDone': 'left_until_done',
+                'ratio': 'ratio',
+                'status': 'status',
+                'date_active': 'date_active',
+                'date_added': 'date_added',
+                'date_done': 'date_done',
+                'date_started': 'date_started',
+                'errorString': 'error_string',
+                'priority': 'priority',
+                'progress': 'progress',
+                'secondsDownloading': 'seconds_downloading',
+                'secondsSeeding': 'seconds_seeding',
+                'torrentFile': 'torrent_file',
+                'labels': 'labels',
+            }.items():
                 try:
-                    value = getattr(torrent, attr)
+                    value = getattr(torrent, field)
                 except Exception:
                     logger.opt(exception=True).debug(
                         'error when requesting transmissionrpc attribute {}', attr
                     )
                 else:
-                    # transmission-rpc adds timezone info to datetimes, which makes them hard to deal with. Strip it.
+                    # transmission-rpc adds timezone info to datetimes,
+                    # which makes them hard to deal with. Strip it.
                     if isinstance(value, datetime):
                         value = value.replace(tzinfo=None)
                     entry['transmission_' + attr] = value
             # Availability in percent
             entry['transmission_availability'] = (
-                (torrent.desiredAvailable / torrent.leftUntilDone) if torrent.leftUntilDone else 0
+                (torrent.desired_available / torrent.left_until_done)
+                if torrent.left_until_done
+                else 0
             )
 
-            entry['transmission_trackers'] = [t['announce'] for t in torrent.trackers]
+            entry['transmission_trackers'] = [t.announce for t in torrent.trackers]
             entry['transmission_seed_ratio_ok'] = seed_ratio_ok
             entry['transmission_idle_limit_ok'] = idle_limit_ok
             st_error_to_desc = {
                 0: 'OK',
                 1: 'tracker_warning',
                 2: 'tracker_error',
                 3: 'local_error',
             }
             entry['transmission_error_state'] = st_error_to_desc[torrent.error]
             # Built in done_date doesn't work when user adds an already completed file to transmission
             if torrent.progress == 100:
-                entry['transmission_date_done'] = datetime.fromtimestamp(
-                    max(torrent.addedDate, torrent.doneDate)
-                )
+                entry['transmission_date_done'] = max(torrent.added_date, torrent.done_date)
+
             entries.append(entry)
         return entries
 
 
 class PluginTransmission(TransmissionBase):
     """
     Add url from entry url to transmission
@@ -313,14 +340,15 @@
                     'include_subs': {'type': 'boolean'},
                     'bandwidth_priority': {'type': 'number'},
                     'honor_limits': {'type': 'boolean'},
                     'include_files': one_or_more({'type': 'string'}),
                     'skip_files': one_or_more({'type': 'string'}),
                     'rename_like_files': {'type': 'boolean'},
                     'queue_position': {'type': 'integer'},
+                    'labels': {'type': 'array', 'items': {'type': 'string'}},
                 },
                 'additionalProperties': False,
             },
         ]
     }
 
     def prepare_config(self, config):
@@ -413,22 +441,19 @@
                     logger.debug('temp: {}', ', '.join(os.listdir(tmp_path)))
                     entry.fail("Downloaded temp file '%s' doesn't exist!?" % entry['file'])
                     continue
 
                 try:
                     if downloaded:
                         with open(entry['file'], 'rb') as f:
-                            filedump = base64.b64encode(f.read()).decode('utf-8')
-                        torrent_info = client.add_torrent(filedump, 30, **options['add'])
+                            torrent_info = client.add_torrent(f, 30, **options['add'])
                     else:
                         if options['post'].get('magnetization_timeout', 0) > 0:
                             options['add']['paused'] = False
-                        torrent_info = client.add_torrent(
-                            entry['url'], timeout=30, **options['add']
-                        )
+                        torrent_info = client.add_torrent(entry['url'], **options['add'])
                 except TransmissionError as e:
                     logger.opt(exception=True).debug('TransmissionError')
                     logger.debug('Failed options dict: {}', options['add'])
                     msg = 'Error adding {} to transmission. TransmissionError: {}'.format(
                         entry['title'], e.message or 'N/A'
                     )
                     logger.error(msg)
@@ -436,49 +461,54 @@
                     continue
                 logger.info('"{}" torrent added to transmission', entry['title'])
                 # The info returned by the add call is incomplete, refresh it
                 torrent_info = client.get_torrent(torrent_info.id)
             else:
                 # Torrent already loaded in transmission
                 if options['add'].get('download_dir'):
-                    logger.verbose(
-                        'Moving {} to "{}"', torrent_info.name, options['add']['download_dir']
+                    logger.log(
+                        "VERBOSE",
+                        'Moving {} to "{}"',
+                        torrent_info.name,
+                        options['add']['download_dir'],
                     )
                     # Move data even if current reported torrent location matches new location
                     # as transmission may fail to automatically move completed file to final
                     # location but continue reporting final location instead of real location.
                     # In such case this will kick transmission to really move data.
                     # If data is already located at new location then transmission just ignore
                     # this command.
-                    client.move_torrent_data(torrent_info.id, options['add']['download_dir'], 120)
+                    client.move_torrent_data(
+                        torrent_info.hashString, options['add']['download_dir'], 120
+                    )
 
             try:
-                total_size = torrent_info.totalSize
+                total_size = torrent_info.total_size
                 main_id = None
                 find_main_file = (
                     options['post'].get('main_file_only') or 'content_filename' in options['post']
                 )
                 skip_files = options['post'].get('skip_files')
                 # We need to index the files if any of the following are defined
                 if find_main_file or skip_files:
-                    file_list = client.get_files(torrent_info.id)[torrent_info.id]
+                    file_list = torrent_info.get_files()
 
                     if options['post'].get('magnetization_timeout', 0) > 0 and not file_list:
                         logger.debug(
                             'Waiting {} seconds for "{}" to magnetize',
                             options['post']['magnetization_timeout'],
                             entry['title'],
                         )
                         for _ in range(options['post']['magnetization_timeout']):
                             sleep(1)
-                            file_list = client.get_files(torrent_info.id)[torrent_info.id]
+                            file_list = torrent_info.get_files()
                             if file_list:
                                 total_size = client.get_torrent(
                                     torrent_info.id, ['id', 'totalSize']
-                                ).totalSize
+                                ).total_size
                                 break
                         else:
                             logger.warning(
                                 '"{}" did not magnetize before the timeout elapsed, file list unavailable for processing.',
                                 entry['title'],
                             )
 
@@ -607,15 +637,15 @@
                                 'Downloading {} of {} files in torrent.',
                                 len(options['change']['files_wanted']),
                                 len(file_list),
                             )
 
                 # Set any changed file properties
                 if list(options['change'].keys()):
-                    client.change_torrent(torrent_info.id, 30, **options['change'])
+                    client.change_torrent(torrent_info.id, **options['change'])
 
                 start_torrent = partial(client.start_torrent, [torrent_info.id])
 
                 if config['action'] == 'add':
                     # if add_paused was defined and set to False start the torrent;
                     # prevents downloading data before we set what files we want
                     start_paused = (
@@ -648,15 +678,14 @@
                 msg = 'Error trying to {} {}, TransmissionError: {}'.format(
                     config['action'], entry['title'], e.message or 'N/A'
                 )
                 logger.error(msg)
                 continue
 
     def _make_torrent_options_dict(self, config, entry):
-
         opt_dic = {}
 
         for opt_key in (
             'path',
             'add_paused',
             'honor_limits',
             'bandwidth_priority',
@@ -669,14 +698,15 @@
             'magnetization_timeout',
             'include_subs',
             'content_filename',
             'include_files',
             'skip_files',
             'rename_like_files',
             'queue_position',
+            'labels',
         ):
             # Values do not merge config with task
             # Task takes priority then config is used
             if opt_key in entry:
                 opt_dic[opt_key] = entry[opt_key]
             elif opt_key in config:
                 opt_dic[opt_key] = config[opt_key]
@@ -720,14 +750,17 @@
                 change['seedRatioMode'] = 2
             else:
                 change['seedRatioMode'] = 1
 
         if 'queue_position' in opt_dic:
             change['queuePosition'] = opt_dic['queue_position']
 
+        if 'labels' in opt_dic:
+            change['labels'] = opt_dic['labels']
+
         post = options['post']
         # set to modify paused status after
         if 'add_paused' in opt_dic:
             post['paused'] = opt_dic['add_paused']
         if 'main_file_only' in opt_dic:
             post['main_file_only'] = opt_dic['main_file_only']
         if 'main_file_ratio' in opt_dic:
@@ -836,48 +869,48 @@
             else None
         )
 
         session = client.get_session()
 
         remove_ids = []
         for torrent in client.get_torrents():
-            logger.verbose(
+            logger.log(
+                "VERBOSE",
                 'Torrent "{}": status: "{}" - ratio: {} - date added: {}',
                 torrent.name,
                 torrent.status,
                 torrent.ratio,
-                torrent.date_added,
+                torrent.added_date,
             )
             downloaded, dummy = self.torrent_info(torrent, config)
             if not downloaded:
                 continue
             if config.get('transmission_seed_limits'):
                 seed_ratio_ok, idle_limit_ok = self.check_seed_limits(torrent, session)
                 if not seed_ratio_ok or not idle_limit_ok:
                     continue
             if 'min_ratio' in config:
                 if torrent.ratio < config['min_ratio']:
                     continue
             if 'finished_for' in config:
                 # done date might be invalid if this torrent was added to transmission when already completed
-                started_seeding = datetime.fromtimestamp(max(torrent.addedDate, torrent.doneDate))
+                started_seeding = max(torrent.added_date, torrent.done_date)
                 if started_seeding + parse_timedelta(config['finished_for']) > datetime.now():
                     continue
-            tracker_hosts = (
-                urlparse(tracker['announce']).hostname for tracker in torrent.trackers
-            )
+            tracker_hosts = [urlparse(tracker.announce).hostname for tracker in torrent.trackers]
             if 'tracker' in config:
                 if not any(tracker_re.search(tracker) for tracker in tracker_hosts):
                     continue
             if 'preserve_tracker' in config:
                 if any(preserve_tracker_re.search(tracker) for tracker in tracker_hosts):
                     continue
             if config.get('directories'):
                 if not any(
-                    re.search(d, torrent.downloadDir, re.IGNORECASE) for d in config['directories']
+                    re.search(d, torrent.download_dir, re.IGNORECASE)
+                    for d in config['directories']
                 ):
                     continue
             if task.options.test:
                 logger.info('Would remove finished torrent `{}` from transmission', torrent.name)
                 continue
             logger.info('Removing finished torrent `{}` from transmission', torrent.name)
             remove_ids.append(torrent.id)
```

### Comparing `FlexGet-3.5.9/flexget/plugins/daemon/web_server.py` & `FlexGet-3.6.0/flexget/plugins/daemon/web_server.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/abort_if_exists.py` & `FlexGet-3.6.0/flexget/plugins/filter/abort_if_exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/accept_all.py` & `FlexGet-3.6.0/flexget/plugins/filter/accept_all.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/age.py` & `FlexGet-3.6.0/flexget/plugins/filter/age.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/best_quality.py` & `FlexGet-3.6.0/flexget/plugins/filter/best_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/content_filter.py` & `FlexGet-3.6.0/flexget/plugins/filter/content_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/content_size.py` & `FlexGet-3.6.0/flexget/plugins/filter/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/crossmatch.py` & `FlexGet-3.6.0/flexget/plugins/filter/crossmatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
             'case_sensitive': {'type': 'boolean', 'default': True},
         },
         'required': ['fields', 'action', 'from'],
         'additionalProperties': False,
     }
 
     def on_task_filter(self, task, config):
-
         fields = config['fields']
         action = config['action']
         all_fields = config['all_fields']
 
         if not task.entries:
             logger.trace('Stopping crossmatch filter because of no entries to check')
             return
```

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/delay.py` & `FlexGet-3.6.0/flexget/plugins/filter/delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/duplicates.py` & `FlexGet-3.6.0/flexget/plugins/filter/duplicates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/exists.py` & `FlexGet-3.6.0/flexget/plugins/filter/exists.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/exists_movie.py` & `FlexGet-3.6.0/flexget/plugins/filter/exists_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/exists_series.py` & `FlexGet-3.6.0/flexget/plugins/filter/exists_series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/if_condition.py` & `FlexGet-3.6.0/flexget/plugins/filter/if_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 logger = logger.bind(name='if')
 
 
 class FilterIf:
     """Can run actions on entries that satisfy a given condition.
 
-    Actions include accept, reject, and fail, as well as the ability to run other filter plugins on the entries."""
+    Actions include accept, reject, and fail, as well as the ability to run other filter plugins on the entries.
+    """
 
     schema = {
         'type': 'array',
         'items': {
             'type': 'object',
             'additionalProperties': {
                 'anyOf': [{'$ref': '/schema/plugins'}, {'enum': ['accept', 'reject', 'fail']}]
```

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/limit_new.py` & `FlexGet-3.6.0/flexget/plugins/filter/limit_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/magnets.py` & `FlexGet-3.6.0/flexget/plugins/filter/magnets.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/only_new.py` & `FlexGet-3.6.0/flexget/plugins/filter/only_new.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/proper_movies.py` & `FlexGet-3.6.0/flexget/plugins/filter/proper_movies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/quality.py` & `FlexGet-3.6.0/flexget/plugins/filter/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/regexp.py` & `FlexGet-3.6.0/flexget/plugins/filter/regexp.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/require_field.py` & `FlexGet-3.6.0/flexget/plugins/filter/require_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/rottentomatoes.py` & `FlexGet-3.6.0/flexget/plugins/filter/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/thetvdb.py` & `FlexGet-3.6.0/flexget/plugins/filter/thetvdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
             else:
                 if entryitem in configlist:
                     return True
         return False
 
     @plugin.priority(126)
     def on_task_filter(self, task, config):
-
         lookup = plugin.get('thetvdb_lookup', self).lookup
 
         for entry in task.entries:
             force_accept = False
 
             try:
                 lookup(task, entry)
```

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/timeframe.py` & `FlexGet-3.6.0/flexget/plugins/filter/timeframe.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/unique.py` & `FlexGet-3.6.0/flexget/plugins/filter/unique.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/filter/upgrade.py` & `FlexGet-3.6.0/flexget/plugins/filter/upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
         config.setdefault('on_lower', 'do_nothing')
         config.setdefault('target', None)
         config.setdefault('timeframe', None)
         config.setdefault('propers', True)
         return config
 
     def filter_entries(self, entries, existing, target, action_on_lower):
-
         target_requirement = qualities.Requirements(target) if target else None
         filtered = []
 
         for entry in entries:
             # Filter out entries within target
             if target:
                 if not target_requirement.allows(entry['quality']):
```

### Comparing `FlexGet-3.5.9/flexget/plugins/generic/cron_env.py` & `FlexGet-3.6.0/flexget/plugins/generic/cron_env.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/generic/db_vacuum.py` & `FlexGet-3.6.0/flexget/plugins/generic/db_vacuum.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/generic/log_start.py` & `FlexGet-3.6.0/flexget/plugins/generic/log_start.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/generic/urlfix.py` & `FlexGet-3.6.0/flexget/plugins/generic/urlfix.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/generic/welcome.py` & `FlexGet-3.6.0/flexget/plugins/generic/welcome.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/anidb_list.py` & `FlexGet-3.6.0/flexget/plugins/input/anidb_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/anilist.py` & `FlexGet-3.6.0/flexget/plugins/input/anilist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/apple_trailers.py` & `FlexGet-3.6.0/flexget/plugins/input/apple_trailers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/betaseries_list.py` & `FlexGet-3.6.0/flexget/plugins/input/betaseries_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/discover.py` & `FlexGet-3.6.0/flexget/plugins/input/discover.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/filesystem.py` & `FlexGet-3.6.0/flexget/plugins/input/filesystem.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/filmweb_watchlist.py` & `FlexGet-3.6.0/flexget/plugins/input/filmweb_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/from_piratebay.py` & `FlexGet-3.6.0/flexget/plugins/input/from_piratebay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/from_task.py` & `FlexGet-3.6.0/flexget/plugins/input/from_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/from_telegram.py` & `FlexGet-3.6.0/flexget/plugins/input/from_telegram.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/gazelle.py` & `FlexGet-3.6.0/flexget/plugins/input/gazelle.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,14 @@
 
         if r.status_code != 200:
             raise PluginError("{} returned a non-200 status code".format(self.base_url))
 
         try:
             json_response = r.json()
             if json_response['status'] != "success":
-
                 # Try to deal with errors returned by the API
                 error = json_response.get('error', json_response.get('status'))
                 if not error or error == "failure":
                     error = json_response.get('response', str(json_response))
 
                 raise PluginError(
                     "{} gave a failure response of '{}'".format(self.base_url, error)
```

### Comparing `FlexGet-3.5.9/flexget/plugins/input/generate.py` & `FlexGet-3.6.0/flexget/plugins/input/generate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/html.py` & `FlexGet-3.6.0/flexget/plugins/input/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,14 @@
             if match:
                 name = match.group(1)
         else:
             name = Path(parts.path).name
         return parse.unquote_plus(name)
 
     def create_entries(self, page_url, soup, config):
-
         queue = []
         duplicates = {}
         duplicate_limit = 4
 
         def title_exists(title):
             """Helper method. Return True if title is already added to entries"""
             for entry in queue:
```

### Comparing `FlexGet-3.5.9/flexget/plugins/input/input_csv.py` & `FlexGet-3.6.0/flexget/plugins/input/input_csv.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/inputs.py` & `FlexGet-3.6.0/flexget/plugins/input/inputs.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/json.py` & `FlexGet-3.6.0/flexget/plugins/input/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/kitsu.py` & `FlexGet-3.6.0/flexget/plugins/input/kitsu.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/letterboxd.py` & `FlexGet-3.6.0/flexget/plugins/input/letterboxd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/limit.py` & `FlexGet-3.6.0/flexget/plugins/input/limit.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/medusa.py` & `FlexGet-3.6.0/flexget/plugins/input/medusa.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/mock.py` & `FlexGet-3.6.0/flexget/plugins/input/mock.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/my_anime_list.py` & `FlexGet-3.6.0/flexget/plugins/input/my_anime_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/myepisodes_list.py` & `FlexGet-3.6.0/flexget/plugins/input/myepisodes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/next_sonarr_episodes.py` & `FlexGet-3.6.0/flexget/plugins/input/next_sonarr_episodes.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/npo_watchlist.py` & `FlexGet-3.6.0/flexget/plugins/input/npo_watchlist.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/parameterize.py` & `FlexGet-3.6.0/flexget/plugins/input/parameterize.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from flexget.event import event
 from flexget.utils.template import RenderError, render_from_entry
 
 log = logging.getLogger('parameterize')
 
 
 class Parameterize(object):
-
     schema = {
         'type': 'object',
         'properties': {
             'plugin': {'$ref': '/schema/plugins?phase=input'},
             'using': {'$ref': '/schema/plugins?phase=input'},
         },
     }
```

### Comparing `FlexGet-3.5.9/flexget/plugins/input/plex.py` & `FlexGet-3.6.0/flexget/plugins/input/plex.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/pogcal.py` & `FlexGet-3.6.0/flexget/plugins/input/pogcal.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
                 raise plugin.PluginError('Invalid username/password for pogdesign.')
             page = session.get('https://www.pogdesign.co.uk/cat/show-select')
         except requests.RequestException as e:
             raise plugin.PluginError('Error retrieving source: %s' % e)
         soup = get_soup(page.text)
         entries = []
         for row in soup.find_all('li', {'class': 'selectgrp checked'}):
-
             # Get name
             t = row.find('strong')
 
             # Remove <span> tags
             spantags = t.find_all('span')
             for s in spantags:
                 s.extract()
```

### Comparing `FlexGet-3.5.9/flexget/plugins/input/regexp_parse.py` & `FlexGet-3.6.0/flexget/plugins/input/regexp_parse.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/rlslog.py` & `FlexGet-3.6.0/flexget/plugins/input/rlslog.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/rottentomatoes_list.py` & `FlexGet-3.6.0/flexget/plugins/input/rottentomatoes_list.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/rss.py` & `FlexGet-3.6.0/flexget/plugins/input/rss.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,14 @@
 
     def escape_content(self, content):
         valid_escapes = (b'&quot;', b'&apos;', b'&lt;', b'&gt;', b'&amp;')
         future_result = []
         in_cdata_block = False
 
         for idx, char in enumerate(bytes(content)):
-
             char = bytes([char])
             if not in_cdata_block and char == b'&':
                 if not content[idx : idx + 7].startswith(valid_escapes):
                     char = b'&amp;'
             elif not in_cdata_block and char == b'<' and content[idx : idx + 9] == b'<![CDATA[':
                 in_cdata_block = True
             elif in_cdata_block and char == b']' and content[idx - 1 : idx + 2] == b']]>':
@@ -409,15 +408,14 @@
         for field_map in config.get('other_fields', []):
             fields.update(field_map)
 
         # field name for url can be configured by setting link.
         # default value is auto but for example guid is used in some feeds
         ignored = 0
         for entry in rss.entries:
-
             # Check if title field is overridden in config
             title_field = config.get('title', 'title')
             # ignore entries without title
             if not entry.get(title_field):
                 logger.debug('skipping entry without title')
                 ignored += 1
                 continue
```

### Comparing `FlexGet-3.5.9/flexget/plugins/input/sceper.py` & `FlexGet-3.6.0/flexget/plugins/input/sceper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/sickbeard.py` & `FlexGet-3.6.0/flexget/plugins/input/sickbeard.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/tail.py` & `FlexGet-3.6.0/flexget/plugins/input/tail.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     }
 
     def format_entry(self, entry, d):
         for k, v in d.items():
             entry[k] = v % entry
 
     def on_task_input(self, task, config):
-
         # Let details plugin know that it is ok if this task doesn't produce any entries
         task.no_entries_ok = True
 
         filename = os.path.expanduser(config['file'])
         encoding = config.get('encoding', 'utf-8')
         with Session() as session:
             db_pos = (
```

### Comparing `FlexGet-3.5.9/flexget/plugins/input/text.py` & `FlexGet-3.6.0/flexget/plugins/input/text.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/input/torznab.py` & `FlexGet-3.6.0/flexget/plugins/input/torznab.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from flexget import plugin
 from flexget.components.sites.utils import torrent_availability
 from flexget.entry import Entry
 from flexget.event import event
 from flexget.plugin import PluginError
 from flexget.utils.requests import RequestException
+from flexget.utils.tools import parse_timedelta
 
 logger = logger.bind(name='torznab')
 
 
 class Torznab:
     """Torznab search plugin
 
@@ -29,14 +30,15 @@
                 'categories': {'type': 'array', 'items': {'type': 'integer'}, 'default': []},
                 'searcher': {
                     'type': 'string',
                     'enum': ['movie', 'tv', 'tvsearch', 'search'],
                     'default': 'search',
                 },
                 'website': {'type': 'string', 'format': 'url'},
+                'timeout': {"type": "string", "format": "interval"},
             },
             'required': ['website', 'apikey'],
             'additionalProperties': False,
         }
         return schema
 
     def search(self, task, entry, config=None):
@@ -70,28 +72,30 @@
         url = '{}/api?'.format(self.base_url)
         url = '{}{}'.format(url, urlencode(params))
         return url
 
     def _setup(self, task, config):
         """Set up parameters"""
         self.base_url = config['website'].rstrip('/')
+        config.setdefault('timeout', '30 seconds')
+        self.timeout = parse_timedelta(config['timeout']).total_seconds()
         self.supported_params = []
         if config['searcher'] == 'tv':
             config['searcher'] = 'tvsearch'
 
         self.params = {'apikey': config['apikey'], 'extended': 1}
 
         logger.debug('Config: {}', config)
         self._setup_caps(task, config['searcher'], config['categories'])
 
     @plugin.internet(logger)
     def _setup_caps(self, task, searcher, categories):
         """Gets the capabilities of the torznab indexer and matches it with the provided configuration"""
 
-        response = task.requests.get(self._build_url(t='caps'))
+        response = task.requests.get(self._build_url(t='caps'), timeout=self.timeout)
         logger.debug('Raw caps response {}', response.content)
         root = ElementTree.fromstring(response.content)
         self._setup_searcher(root, searcher, categories)
 
     def _setup_searcher(self, xml_root, searcher, categories):
         """Gets the available searchers (tv, movie, etc) for the indexer and their supported parameters"""
         aliases = {'movie': 'movie-search', 'search': 'search', 'tvsearch': 'tv-search'}
@@ -157,15 +161,15 @@
     @plugin.internet(logger)
     def create_entries_from_query(self, url, task):
         """Fetch feed and fill entries from"""
 
         logger.info('Fetching URL: {}', url)
 
         try:
-            response = task.requests.get(url)
+            response = task.requests.get(url, timeout=self.timeout)
         except RequestException as e:
             raise PluginError("Failed fetching '{}': {}".format(url, e))
 
         entries = []
         root = ElementTree.fromstring(response.content)
         for item in root.findall('.//item'):
             entry = Entry()
```

### Comparing `FlexGet-3.5.9/flexget/plugins/input/twitterfeed.py` & `FlexGet-3.6.0/flexget/plugins/input/twitterfeed.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/internal/api_bluray.py` & `FlexGet-3.6.0/flexget/plugins/internal/api_bluray.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/internal/api_rottentomatoes.py` & `FlexGet-3.6.0/flexget/plugins/internal/api_rottentomatoes.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,14 @@
                                 lambda x: x == ' ', movie_res['title'].lower(), title.lower()
                             )
                             movie_res['match'] = seq.ratio()
                         results.sort(key=lambda x: x['match'], reverse=True)
 
                         # Remove all movies below MIN_MATCH, and different year
                         for movie_res in results[:]:
-
                             if year and movie_res.get('year'):
                                 movie_res['year'] = int(movie_res['year'])
                                 if movie_res['year'] != year:
                                     release_year = False
                                     if movie_res.get('release_dates', {}).get('theater'):
                                         logger.debug('Checking year against theater release date')
                                         release_year = time.strptime(
```

### Comparing `FlexGet-3.5.9/flexget/plugins/internal/change_warn.py` & `FlexGet-3.6.0/flexget/plugins/internal/change_warn.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/assume_quality.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/assume_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/bluray_lookup.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/bluray_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/content_size.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/content_size.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/media_id.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/media_id.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/metainfo_movie.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/metainfo_movie.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/nfo_lookup.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/nfo_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/nzb_size.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/nzb_size.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
         for entry in task.accepted:
             if (
                 entry.get('mime-type') in ['text/nzb', 'application/x-nzb']
                 or entry.get('filename')
                 and entry['filename'].endswith('.nzb')
             ):
-
                 if 'file' not in entry:
                     logger.warning(
                         '`{}` does not have a `file` that could be used to get size information',
                         entry['title'],
                     )
                     continue
```

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/quality.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/rottentomatoes_lookup.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/rottentomatoes_lookup.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/subtitles_check.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/subtitles_check.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/metainfo/task.py` & `FlexGet-3.6.0/flexget/plugins/metainfo/task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/extension.py` & `FlexGet-3.6.0/flexget/plugins/modify/extension.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/headers.py` & `FlexGet-3.6.0/flexget/plugins/modify/headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/manipulate.py` & `FlexGet-3.6.0/flexget/plugins/modify/manipulate.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/path_by_ext.py` & `FlexGet-3.6.0/flexget/plugins/modify/path_by_ext.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/path_by_space.py` & `FlexGet-3.6.0/flexget/plugins/modify/path_by_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/plugin_priority.py` & `FlexGet-3.6.0/flexget/plugins/modify/plugin_priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/regex_extract.py` & `FlexGet-3.6.0/flexget/plugins/modify/regex_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         try:
             for _ in self.regex_list:
                 pass
         except re.error as e:
             raise plugin.PluginError('Error compiling regex: %s' % str(e))
 
     def on_task_modify(self, task, config):
-
         prefix = config.get('prefix')
         modified = 0
 
         for entry in task.entries:
             for rx in self.regex_list:
                 entry_field = entry.get('title')
                 logger.debug('Matching {} with regex: {}', entry_field, rx)
```

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/reorder_quality.py` & `FlexGet-3.6.0/flexget/plugins/modify/reorder_quality.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/set_field.py` & `FlexGet-3.6.0/flexget/plugins/modify/set_field.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/sort_by.py` & `FlexGet-3.6.0/flexget/plugins/modify/sort_by.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/modify/sort_by_weight.py` & `FlexGet-3.6.0/flexget/plugins/modify/sort_by_weight.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/cfscraper.py` & `FlexGet-3.6.0/flexget/plugins/operate/cfscraper.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/cookies.py` & `FlexGet-3.6.0/flexget/plugins/operate/cookies.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/debug_db_sessions.py` & `FlexGet-3.6.0/flexget/plugins/operate/debug_db_sessions.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/debug_warnings.py` & `FlexGet-3.6.0/flexget/plugins/operate/debug_warnings.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/digest.py` & `FlexGet-3.6.0/flexget/plugins/operate/digest.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/disable.py` & `FlexGet-3.6.0/flexget/plugins/operate/disable.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/disable_phases.py` & `FlexGet-3.6.0/flexget/plugins/operate/disable_phases.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/domain_delay.py` & `FlexGet-3.6.0/flexget/plugins/operate/domain_delay.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/entry_trace.py` & `FlexGet-3.6.0/flexget/plugins/operate/entry_trace.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/formlogin.py` & `FlexGet-3.6.0/flexget/plugins/operate/formlogin.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/free_space.py` & `FlexGet-3.6.0/flexget/plugins/operate/free_space.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/include.py` & `FlexGet-3.6.0/flexget/plugins/operate/include.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/interval.py` & `FlexGet-3.6.0/flexget/plugins/operate/interval.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/log_filter.py` & `FlexGet-3.6.0/flexget/plugins/operate/log_filter.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/manual.py` & `FlexGet-3.6.0/flexget/plugins/operate/manual.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/max_reruns.py` & `FlexGet-3.6.0/flexget/plugins/operate/max_reruns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/pathscrub.py` & `FlexGet-3.6.0/flexget/plugins/operate/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/priority.py` & `FlexGet-3.6.0/flexget/plugins/operate/priority.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/proxy.py` & `FlexGet-3.6.0/flexget/plugins/operate/proxy.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/rerun.py` & `FlexGet-3.6.0/flexget/plugins/operate/rerun.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/run_task.py` & `FlexGet-3.6.0/flexget/plugins/operate/run_task.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/sequence.py` & `FlexGet-3.6.0/flexget/plugins/operate/sequence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/sleep.py` & `FlexGet-3.6.0/flexget/plugins/operate/sleep.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/spy_headers.py` & `FlexGet-3.6.0/flexget/plugins/operate/spy_headers.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/template.py` & `FlexGet-3.6.0/flexget/plugins/operate/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/verbose.py` & `FlexGet-3.6.0/flexget/plugins/operate/verbose.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/verbose_details.py` & `FlexGet-3.6.0/flexget/plugins/operate/verbose_details.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/verify_ssl_certificates.py` & `FlexGet-3.6.0/flexget/plugins/operate/verify_ssl_certificates.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/operate/version_checker.py` & `FlexGet-3.6.0/flexget/plugins/operate/version_checker.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/download.py` & `FlexGet-3.6.0/flexget/plugins/output/download.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/download_auth.py` & `FlexGet-3.6.0/flexget/plugins/output/download_auth.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/dump.py` & `FlexGet-3.6.0/flexget/plugins/output/dump.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/dump_config.py` & `FlexGet-3.6.0/flexget/plugins/output/dump_config.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/exec.py` & `FlexGet-3.6.0/flexget/plugins/output/exec.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/file_operations.py` & `FlexGet-3.6.0/flexget/plugins/output/file_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def get_directory_size(directory):
     """
     :param directory: Path
     :return: Size in bytes (recursively)
     """
     dir_size = 0
-    for (path, _, files) in os.walk(directory):
+    for path, _, files in os.walk(directory):
         for file in files:
             filename = os.path.join(path, file)
             dir_size += os.path.getsize(filename)
     return dir_size
 
 
 def get_siblings(ext, main_file_no_ext, main_file_ext, abs_path):
```

### Comparing `FlexGet-3.5.9/flexget/plugins/output/html.py` & `FlexGet-3.6.0/flexget/plugins/output/html.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/memusage.py` & `FlexGet-3.6.0/flexget/plugins/output/memusage.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from flexget.event import event
 from flexget.terminal import console
 
 try:
     from guppy import hpy
 except ImportError:
     # this will leave the plugin unloaded
-    raise plugin.DependencyError(issued_by='memusage', missing='ext lib `guppy`', silent=True)
+    raise plugin.DependencyError(issued_by='memusage', missing='guppy3', silent=True)
 
 logger = logger.bind(name='mem_usage')
 
 """
 http://blog.mfabrik.com/2008/03/07/debugging-django-memory-leak-with-trackrefs-and-guppy/
 
 # Print memory statistics
@@ -42,20 +42,24 @@
 
 
 @event('manager.shutdown')
 def on_manager_shutdown(manager):
     if not manager.options.mem_usage:
         return
 
-    import resource
+    try:
+        import resource
+
+        console(
+            'Resource Module memory usage: %s (kb)'
+            % resource.getrusage(resource.RUSAGE_SELF).ru_maxrss
+        )
+    except ImportError:
+        console('Resource Module memory usage:')
 
-    console(
-        'Resource Module memory usage: %s (kb)'
-        % resource.getrusage(resource.RUSAGE_SELF).ru_maxrss
-    )
     global heapy
     console('Heapy module calculating memory usage:')
     console(heapy.heap())
     console('-' * 79)
     console('Heapy module calculating report (this may take a while):')
     console(heapy.heap().get_rp(40))
     heapy = None
```

### Comparing `FlexGet-3.5.9/flexget/plugins/output/mock_output.py` & `FlexGet-3.6.0/flexget/plugins/output/mock_output.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/rss.py` & `FlexGet-3.6.0/flexget/plugins/output/rss.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
                 logger.error(
                     'Error rendering jinja title for `{}` falling back to entry title: {}',
                     entry['title'],
                     e,
                 )
                 rss.title = entry['title']
             for field in config['link']:
-                if field in entry:
+                if entry.get(field) is not None:
                     rss.link = entry[field]
                     break
 
             try:
                 template = get_template(config['template'], scope='task')
             except ValueError as e:
                 raise plugin.PluginError('Invalid template specified: %s' % e)
```

### Comparing `FlexGet-3.5.9/flexget/plugins/output/rtorrent_magnet.py` & `FlexGet-3.6.0/flexget/plugins/output/rtorrent_magnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             with open(path, 'w') as f:
                 f.write('d10:magnet-uri%d:%se' % (len(entry['url']), entry['url']))
         entry['output'] = path
 
     # Run after download plugin to only pick up entries it did not already handle
     @plugin.priority(0)
     def on_task_output(self, task, config):
-
         for entry in task.accepted:
             if 'output' in entry:
                 logger.debug(
                     'Ignoring, {} already has an output file: {}', entry['title'], entry['output']
                 )
                 continue
```

### Comparing `FlexGet-3.5.9/flexget/plugins/output/sabnzbd.py` & `FlexGet-3.6.0/flexget/plugins/output/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/sns.py` & `FlexGet-3.6.0/flexget/plugins/output/sns.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/subtitles.py` & `FlexGet-3.6.0/flexget/plugins/output/subtitles.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         if not isinstance(config, dict):
             config = {}
         config.setdefault('output', task.manager.config_base)
         config['output'] = os.path.expanduser(config['output'])
         return config
 
     def on_task_download(self, task, config):
-
         # filter all entries that have IMDB ID set
         try:
             entries = [e for e in task.accepted if e['imdb_id'] is not None]
         except KeyError:
             # No imdb urls on this task, skip it
             # TODO: should do lookup via imdb_lookup plugin?
             return
```

### Comparing `FlexGet-3.5.9/flexget/plugins/output/subtitles_periscope.py` & `FlexGet-3.6.0/flexget/plugins/output/subtitles_periscope.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/subtitles_subliminal.py` & `FlexGet-3.6.0/flexget/plugins/output/subtitles_subliminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/output/symlink.py` & `FlexGet-3.6.0/flexget/plugins/output/symlink.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from flexget.utils.pathscrub import pathscrub
 from flexget.utils.template import RenderError, render_from_entry
 
 logger = logger.bind(name='symlink')
 
 
 class Symlink:
-
     schema = {
         'oneOf': [
             {
                 'title': 'specify options',
                 'type': 'object',
                 'properties': {
                     'to': {'type': 'string', 'format': 'path'},
```

### Comparing `FlexGet-3.5.9/flexget/plugins/output/utorrent.py` & `FlexGet-3.6.0/flexget/plugins/output/utorrent.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/services/kodi_library.py` & `FlexGet-3.6.0/flexget/plugins/services/kodi_library.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/plugins/services/myepisodes.py` & `FlexGet-3.6.0/flexget/plugins/services/myepisodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
         Return: boolean
         """
         if (
             'series_season' not in entry
             or 'series_episode' not in entry
             or 'series_name' not in entry
         ):
-
             raise plugin.PluginWarning(
                 'Can\'t mark entry `%s` in myepisodes without series_season, series_episode and series_name '
                 'fields' % entry['title'],
                 logger,
             )
 
     def _lookup_myepisodes_id(self, entry):
```

### Comparing `FlexGet-3.5.9/flexget/plugins/services/pogcal_acquired.py` & `FlexGet-3.6.0/flexget/plugins/services/pogcal_acquired.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/resources/flexget.png` & `FlexGet-3.6.0/flexget/resources/flexget.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/task.py` & `FlexGet-3.6.0/flexget/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,14 +741,15 @@
                         'Task has been re-run {} times already, stopping for now',
                         self._rerun_count,
                     )
                 break
             fire_event('task.execute.completed', self)
         finally:
             self.finished_event.set()
+            self.requests.close()
 
     @staticmethod
     def validate_config(config):
         schema = plugin_schemas(interface='task')
         # Don't validate commented out plugins
         schema['patternProperties'] = {'^_': {}}
         return config_schema.process_config(config, schema)
```

### Comparing `FlexGet-3.5.9/flexget/task_queue.py` & `FlexGet-3.6.0/flexget/task_queue.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/templates/task/default.template` & `FlexGet-3.6.0/flexget/templates/task/default.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/templates/task/html.template` & `FlexGet-3.6.0/flexget/templates/task/html.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/templates/task/rss.template` & `FlexGet-3.6.0/flexget/templates/task/rss.template`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/terminal.py` & `FlexGet-3.6.0/flexget/terminal.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/tray_icon.py` & `FlexGet-3.6.0/flexget/tray_icon.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/__init__.py` & `FlexGet-3.6.0/flexget/ui/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/app.html` & `FlexGet-3.6.0/flexget/ui/v1/app/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/assets/images/header.png` & `FlexGet-3.6.0/flexget/ui/v1/app/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/favicon.ico` & `FlexGet-3.6.0/flexget/ui/v1/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/FontAwesome.otf` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.eot` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.svg` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/ui-grid.eot` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/ui-grid.eot`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/ui-grid.svg` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/ui-grid.svg`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/ui-grid.ttf` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/ui-grid.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/fonts/ui-grid.woff` & `FlexGet-3.6.0/flexget/ui/v1/app/fonts/ui-grid.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/scripts/app.js` & `FlexGet-3.6.0/flexget/ui/v1/app/scripts/app.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/scripts/splash.js` & `FlexGet-3.6.0/flexget/ui/v1/app/scripts/splash.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/scripts/vendor.js` & `FlexGet-3.6.0/flexget/ui/v1/app/scripts/vendor.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/styles/app.css` & `FlexGet-3.6.0/flexget/ui/v1/app/styles/app.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/styles/splash.css` & `FlexGet-3.6.0/flexget/ui/v1/app/styles/splash.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/app/styles/vendor.css` & `FlexGet-3.6.0/flexget/ui/v1/app/styles/vendor.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/bower.json` & `FlexGet-3.6.0/flexget/ui/v1/bower.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/gulp/build.js` & `FlexGet-3.6.0/flexget/ui/v1/gulp/build.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/gulp/inject.js` & `FlexGet-3.6.0/flexget/ui/v1/gulp/inject.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/gulp/lint.js` & `FlexGet-3.6.0/flexget/ui/v1/gulp/lint.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/gulp/proxy.js` & `FlexGet-3.6.0/flexget/ui/v1/gulp/proxy.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/gulp/server.js` & `FlexGet-3.6.0/flexget/ui/v1/gulp/server.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/gulp/styles.js` & `FlexGet-3.6.0/flexget/ui/v1/gulp/styles.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/gulp/test.js` & `FlexGet-3.6.0/flexget/ui/v1/gulp/test.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/gulp/watch.js` & `FlexGet-3.6.0/flexget/ui/v1/gulp/watch.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/karma.conf.js` & `FlexGet-3.6.0/flexget/ui/v1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/package.json` & `FlexGet-3.6.0/flexget/ui/v1/package.json`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/specs.html` & `FlexGet-3.6.0/flexget/ui/v1/specs.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/app.html` & `FlexGet-3.6.0/flexget/ui/v1/src/app.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/app.module.js` & `FlexGet-3.6.0/flexget/ui/v1/src/app.module.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/app.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/app.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/assets/images/header.png` & `FlexGet-3.6.0/flexget/ui/v1/src/assets/images/header.png`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error-dialog.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error-dialog.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/error/error.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/error/error.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/exception/exception.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/exception/exception.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/exception/exception.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/exception/exception.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/_pagination.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/_pagination.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/pagination.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/pagination.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/pagination/pagination.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/router/router-helper.provider.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/router/router-helper.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/blocks/url-interceptor/url-interceptor.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/404/404.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/components/404/404.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.config.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.config.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.config.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/auth.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/auth.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/auth/login.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/components/auth/login.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/core/core.config.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/core/core.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/core/core.provider.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/core/core.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.config.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/database/database.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/components/database/database.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/home/home.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/components/home/home.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/_sidenav.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/_sidenav.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.semver.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.semver.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/components/sidenav/sidenav.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.provider.js` & `FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.provider.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/components/toolbar/toolbar.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/construction.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/construction.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js` & `FlexGet-3.6.0/flexget/ui/v1/src/directives/palette-background/palette-background.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/favicon.ico` & `FlexGet-3.6.0/flexget/ui/v1/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/config/config.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/config/config.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-input/execute-input.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/components/execute-stream/execute-stream.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.filter.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.filter.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.filter.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/execute/execute.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/execute/execute.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/history/history.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/history/history.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/log/log.tmpl.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/log/log.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-input.directive.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie-item.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.controller.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/add-movie/add-movie.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-entry/movie-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/movie-list/movie-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/components/new-list/new-list.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/movies/movies.tmpl.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/pending/pending.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/pending/pending.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/schedule/schedule.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/components/seen-entry/seen-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/seen/seen.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/seen/seen.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-release/episode-release.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/episode-releases/episode-releases.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-begin-dialog/series-begin-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-entry/series-entry.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episode/series-episode.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/components/series-episodes/series-episodes.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.component.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.component.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.route.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.route.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.service.spec.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.service.spec.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/series/series.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/series/series.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/loading-dialog.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/loading-dialog.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/loading-dialog.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/server.config.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/server.config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/server/server.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/server/server.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.component.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.component.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.route.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.route.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/plugins/status/status.tmpl.html` & `FlexGet-3.6.0/flexget/ui/v1/src/plugins/status/status.tmpl.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/scss/_header.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/scss/flexget.scss` & `FlexGet-3.6.0/flexget/ui/v1/src/scss/flexget.scss`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/src/services/schema.service.js` & `FlexGet-3.6.0/flexget/ui/v1/src/services/schema.service.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/config.js` & `FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/config.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/execute.js` & `FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/execute.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/history.js` & `FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/history.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/movie_list.js` & `FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/movie_list.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/seen.js` & `FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/seen.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/series.js` & `FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/series.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v1/tests-mock-data/states.js` & `FlexGet-3.6.0/flexget/ui/v1/tests-mock-data/states.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/__init__.py` & `FlexGet-3.6.0/flexget/ui/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/020c97dc8e0463259c2f9df929bb0c69.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/14.18cf3ab07df2cff9c980.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/14286f3ba79c6627433572dfa925202e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/15.df643f032866e7897440.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/16.d99413fe0332d02516c9.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/2735a3a69b509faf3577afd25bdf552e.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/288ad9c6e8b43cf02443a1f499bdf67e.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/28f9151055c950874d2c6803a39b425b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/35bb8d560db5205616671eab8c4d0303.ttf`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/479970ffb74f2117317f9d24d9e317fe.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/4cb446d4c3b18f2f69df.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/4df32891a5f2f98a363314f595482e08.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/51521a2a8da71e50d871ac6fd2187e87.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/5cb7edfceb233100075dc9a1e12e8da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/60fa3c0614b8fb2f394fa29944c21540.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/68c852c85ea688dfa942.worker.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/7370c3679472e9560965ff48a4399d0b.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/81f57861ed4ac74741f5671e1dff2fd9.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/87284894879f5b1c229cb49c8ff6decc.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/9b3766ef4a402ad3fdeef7501a456512.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/ConfigPlugin.1da6683df8713f0ee5cc.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/EntryListPlugin.c4b35103ad1660e69c44.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/HistoryPlugin.0201ee39aecaa7452270.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/LogPlugin.c8192b546c7f37a23fe0.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/MovieListPlugin.17e519c9d031c1cd9477.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/PendingListPlugin.7ddbee4abf831e808220.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/SeriesPlugin.f46122b2f63739898cd5.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/TasksHomeCard.0f1a9b4992c80e636a4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/TasksPlugin.78a8bc05a72c9f25d7c3.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/adcde98f1d584de52060ad7b16373da3.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/b00849e00f4c2331cddd8ffb44a6720b.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/bb1e4dc6333675d11ada2e857e7f95d7.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/da0e717829e033a69dec97f1e155ae42.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/db4a2a231f52e497c0191e8966b0ee58.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin.5c83b88e8b99cf5955dd.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~SeriesPlugin.82114e5d38c3136caad1.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/default~EntryListPlugin~MovieListPlugin~PendingListPlugin~TasksPlugin.17910c3356c98ded086b.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/ebf6d1640ccddb99fb49f73c052c55a8.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/ef7c6637c68f269a882e73bcb57a7f6a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/f8b1df51ba843179fa1cc9b53d58127a.woff2`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/f9e8e590b4e0f1ff83469bb2a55b8488.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/fe65b8335ee19dd944289f9ed3178c78.woff`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/main.cce4d52f6988bfadab4f.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.css.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map` & `FlexGet-3.6.0/flexget/ui/v2/dist/assets/vendors~main.8ecffb935c6f15cf2922.js.map`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/ui/v2/dist/index.html` & `FlexGet-3.6.0/flexget/ui/v2/dist/index.html`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/bittorrent.py` & `FlexGet-3.6.0/flexget/utils/bittorrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     return encoded
 
 
 def encode_dictionary(data: dict) -> bytes:
     encoded = b'd'
     items = list(data.items())
     items.sort()
-    for (key, value) in items:
+    for key, value in items:
         encoded += bencode(key)
         encoded += bencode(value)
     encoded += b'e'
     return encoded
 
 
 def bencode(data: Union[bytes, str, int, list, dict]) -> bytes:
```

### Comparing `FlexGet-3.5.9/flexget/utils/cache.py` & `FlexGet-3.6.0/flexget/utils/cache.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/cached_input.py` & `FlexGet-3.6.0/flexget/utils/cached_input.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/database.py` & `FlexGet-3.6.0/flexget/utils/database.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/json.py` & `FlexGet-3.6.0/flexget/utils/json.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/lazy_dict.py` & `FlexGet-3.6.0/flexget/utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/log.py` & `FlexGet-3.6.0/flexget/utils/log.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/parsers/generic.py` & `FlexGet-3.6.0/flexget/utils/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/parsers/movie.py` & `FlexGet-3.6.0/flexget/utils/parsers/movie.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from flexget.utils.tools import str_to_int
 
 logger = logger.bind(name='movieparser')
 
 
 def diff_pos(string1, string2):
     """Returns first position where string1 and string2 differ."""
-    for (count, c) in enumerate(string1):
+    for count, c in enumerate(string1):
         if len(string2) <= count:
             return count
         if string2[count] != c:
             return count
 
 
 class MovieParser(TitleParser):
```

### Comparing `FlexGet-3.5.9/flexget/utils/parsers/parser.py` & `FlexGet-3.6.0/flexget/utils/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/parsers/series.py` & `FlexGet-3.6.0/flexget/utils/parsers/series.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/pathscrub.py` & `FlexGet-3.6.0/flexget/utils/pathscrub.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/qualities.py` & `FlexGet-3.6.0/flexget/utils/qualities.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/requests.py` & `FlexGet-3.6.0/flexget/utils/requests.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/serialization.py` & `FlexGet-3.6.0/flexget/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/simple_persistence.py` & `FlexGet-3.6.0/flexget/utils/simple_persistence.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/sqlalchemy_utils.py` & `FlexGet-3.6.0/flexget/utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/template.py` & `FlexGet-3.6.0/flexget/utils/template.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/utils/tools.py` & `FlexGet-3.6.0/flexget/utils/tools.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/flexget/webserver.py` & `FlexGet-3.6.0/flexget/webserver.py`

 * *Files identical despite different names*

### Comparing `FlexGet-3.5.9/pyproject.toml` & `FlexGet-3.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -57,38 +57,39 @@
 python = "^3.7"
 apscheduler = ">=3.2.0"
 beautifulsoup4 = ">=4.5"
 colorama = ">=0.4.4"
 feedparser = ">=6.0.2"
 guessit = ">=3.4,<4.0"
 html5lib = ">=0.11"
+importlib-metadata = { version = "*", python = "<3.8" }  # TODO: remove this after we drop python3.7
 jinja2 = ">=3.0,<4.0"
 jsonschema = ">=2.0"
 loguru = ">=0.4.1"
 psutil = ">=5.8.0"
 pynzb = "^0.1.0"
 pyrss2gen = "^1.1"
 python-dateutil = "^2.8.2"
 pyyaml = ">=4.2b1"
 rebulk = ">=2.0.0"
 requests = ">=2.20.0"
 rich = ">=9.0.0"
-rpyc = ">=5.0,<5.2.0"  # 5.2.1 is causing a hang right now https://github.com/Flexget/Flexget/issues/3601
+rpyc = ">=5.0,!=5.2.*,!=5.3.0"  # 5.2.1-5.3.0 cause a hang https://github.com/Flexget/Flexget/issues/3601
 sqlalchemy = ">=1.3.10,<1.999"
 # WebUI/API Deps
 cherrypy = ">=18.0.0"
 flask-compress = ">=1.2.1"
 flask-cors = ">=2.1.2"
 flask-login = ">=0.4.0"
 flask-restful = ">=0.3.3"
 flask-restx = ">=0.5.1"
 flask = ">=0.7"
 packaging = ">=21.3"
 pyparsing = ">=2.4.7"
-werkzeug = ">=2.0.3"
+werkzeug = ">=2.2.3"
 zxcvbn-python = "^4.4.24"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=18.9b0"
 build = ">=0.9.0"
 click = ">=8.1.3"
 codacy-coverage = ">=1.2.18"
@@ -105,16 +106,21 @@
 sqlalchemy-stubs = "^0.4"
 twine = ">=3.6.0"
 vcrpy = ">=4.1.1"
 
 [tool.poetry.group.plugin-test.dependencies]
 # These are optional dependencies for plugins that have tests in the test suite
 boto3 = ">=1.24.89"
+plexapi = ">=4.13.1"
 subliminal = ">= 2.0rc1"
 
+
+[tool.poetry.group.plugin-tests.dependencies]
+pysftp = "^0.2.9"
+
 [tool.poetry.scripts]
 flexget = 'flexget:main'
 
 
 ## Other tool settings
 
 [tool.pytest.ini_options]
```

### Comparing `FlexGet-3.5.9/requirements.txt` & `FlexGet-3.6.0/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 aniso8601==9.0.1 ; python_version >= "3.7" and python_version < "4.0"
-apscheduler==3.9.1 ; python_version >= "3.7" and python_version < "4"
+apscheduler==3.9.1.post1 ; python_version >= "3.7" and python_version < "4"
 attrs==22.1.0 ; python_version >= "3.7" and python_version < "4.0"
-autocommand==2.2.1 ; python_version >= "3.7" and python_version < "4.0"
+autocommand==2.2.2 ; python_version >= "3.7" and python_version < "4.0"
 babelfish==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 backports-zoneinfo==0.2.1 ; python_version >= "3.7" and python_version < "3.9"
 beautifulsoup4==4.11.1 ; python_version >= "3.7" and python_version < "4.0"
 brotli==1.0.9 ; python_version >= "3.7" and python_version < "4.0"
-certifi==2022.9.24 ; python_version >= "3.7" and python_version < "4"
+certifi==2022.12.7 ; python_version >= "3.7" and python_version < "4"
 charset-normalizer==2.1.1 ; python_version >= "3.7" and python_version < "4"
-cheroot==8.6.0 ; python_version >= "3.7" and python_version < "4.0"
+cheroot==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
 cherrypy==18.8.0 ; python_version >= "3.7" and python_version < "4.0"
 click==8.1.3 ; python_version >= "3.7" and python_version < "4.0"
 colorama==0.4.6 ; python_version >= "3.7" and python_version < "4.0"
 commonmark==0.9.1 ; python_version >= "3.7" and python_version < "4.0"
 feedparser==6.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-compress==1.13 ; python_version >= "3.7" and python_version < "4.0"
 flask-cors==3.0.10 ; python_version >= "3.7" and python_version < "4.0"
 flask-login==0.6.2 ; python_version >= "3.7" and python_version < "4.0"
 flask-restful==0.3.9 ; python_version >= "3.7" and python_version < "4.0"
 flask-restx==1.0.3 ; python_version >= "3.7" and python_version < "4.0"
 flask==2.2.2 ; python_version >= "3.7" and python_version < "4.0"
-greenlet==2.0.0.post0 ; python_version >= "3.7" and (platform_machine == "aarch64" or platform_machine == "ppc64le" or platform_machine == "x86_64" or platform_machine == "amd64" or platform_machine == "AMD64" or platform_machine == "win32" or platform_machine == "WIN32") and python_version < "4.0"
+greenlet==2.0.1 ; python_version >= "3.7" and platform_machine == "aarch64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "ppc64le" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "x86_64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "amd64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "AMD64" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "win32" and python_version < "4.0" or python_version >= "3.7" and platform_machine == "WIN32" and python_version < "4.0"
 guessit==3.5.0 ; python_version >= "3.7" and python_version < "4.0"
 html5lib==1.1 ; python_version >= "3.7" and python_version < "4.0"
 idna==3.4 ; python_version >= "3.7" and python_version < "4"
-importlib-metadata==5.0.0 ; python_version >= "3.7" and python_version < "3.10"
-importlib-resources==5.10.0 ; python_version >= "3.7" and python_version < "3.9"
+importlib-metadata==6.1.0 ; python_version >= "3.7" and python_version < "3.10"
+importlib-resources==5.10.1 ; python_version >= "3.7" and python_version < "3.9"
 inflect==6.0.2 ; python_version >= "3.7" and python_version < "4.0"
 itsdangerous==2.1.2 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-classes==3.2.3 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-collections==3.8.0 ; python_version >= "3.7" and python_version < "4.0"
-jaraco-context==4.1.2 ; python_version >= "3.7" and python_version < "4.0"
+jaraco-context==4.2.0 ; python_version >= "3.7" and python_version < "4.0"
 jaraco-functools==3.5.2 ; python_version >= "3.7" and python_version < "4.0"
-jaraco-text==3.10.0 ; python_version >= "3.7" and python_version < "4.0"
+jaraco-text==3.11.0 ; python_version >= "3.7" and python_version < "4.0"
 jinja2==3.1.2 ; python_version >= "3.7" and python_version < "4.0"
-jsonschema==4.17.0 ; python_version >= "3.7" and python_version < "4.0"
+jsonschema==4.17.3 ; python_version >= "3.7" and python_version < "4.0"
 loguru==0.6.0 ; python_version >= "3.7" and python_version < "4.0"
 markupsafe==2.1.1 ; python_version >= "3.7" and python_version < "4.0"
 more-itertools==9.0.0 ; python_version >= "3.7" and python_version < "4.0"
-packaging==21.3 ; python_version >= "3.7" and python_version < "4.0"
+packaging==22.0 ; python_version >= "3.7" and python_version < "4.0"
 pkgutil-resolve-name==1.3.10 ; python_version >= "3.7" and python_version < "3.9"
 plumbum==1.8.0 ; python_version >= "3.7" and python_version < "4.0"
 portend==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
-psutil==5.9.3 ; python_version >= "3.7" and python_version < "4.0"
+psutil==5.9.4 ; python_version >= "3.7" and python_version < "4.0"
 pydantic==1.10.2 ; python_version >= "3.7" and python_version < "4.0"
 pygments==2.13.0 ; python_version >= "3.7" and python_version < "4.0"
 pynzb==0.1.0 ; python_version >= "3.7" and python_version < "4.0"
 pyparsing==3.0.9 ; python_version >= "3.7" and python_version < "4.0"
 pyrsistent==0.19.2 ; python_version >= "3.7" and python_version < "4.0"
 pyrss2gen==1.1 ; python_version >= "3.7" and python_version < "4.0"
 python-dateutil==2.8.2 ; python_version >= "3.7" and python_version < "4.0"
 pytz-deprecation-shim==0.1.0.post0 ; python_version >= "3.7" and python_version < "4"
 pytz==2022.6 ; python_version >= "3.7" and python_version < "4"
-pywin32==305 ; sys_platform == "win32" and implementation_name == "cpython" and python_version < "3.10" and python_version >= "3.7" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
+pywin32==305 ; sys_platform == "win32" and python_version >= "3.7" and python_version < "3.10" and implementation_name == "cpython" or platform_system == "Windows" and platform_python_implementation != "PyPy" and python_version >= "3.7" and python_version < "4.0"
 pyyaml==6.0 ; python_version >= "3.7" and python_version < "4.0"
 rebulk==3.1.0 ; python_version >= "3.7" and python_version < "4.0"
 requests==2.28.1 ; python_version >= "3.7" and python_version < "4"
 rich==12.6.0 ; python_version >= "3.7" and python_version < "4.0"
-rpyc==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
-setuptools==65.5.1 ; python_version >= "3.7" and python_version < "4"
+rpyc==5.3.1 ; python_version >= "3.7" and python_version < "4.0"
+setuptools==65.6.3 ; python_version >= "3.7" and python_version < "4"
 sgmllib3k==1.0.0 ; python_version >= "3.7" and python_version < "4.0"
 six==1.16.0 ; python_version >= "3.7" and python_version < "4"
 soupsieve==2.3.2.post1 ; python_version >= "3.7" and python_version < "4.0"
-sqlalchemy==1.4.43 ; python_version >= "3.7" and python_version < "4.0"
-tempora==5.0.2 ; python_version >= "3.7" and python_version < "4.0"
+sqlalchemy==1.4.45 ; python_version >= "3.7" and python_version < "4.0"
+tempora==5.1.0 ; python_version >= "3.7" and python_version < "4.0"
 typing-extensions==4.4.0 ; python_version >= "3.7" and python_version < "4.0"
-tzdata==2022.6 ; python_version >= "3.7" and python_version < "4"
+tzdata==2022.7 ; python_version >= "3.7" and python_version < "4"
 tzlocal==4.2 ; python_version >= "3.7" and python_version < "4"
-urllib3==1.26.12 ; python_version >= "3.7" and python_version < "4"
+urllib3==1.26.13 ; python_version >= "3.7" and python_version < "4"
 webencodings==0.5.1 ; python_version >= "3.7" and python_version < "4.0"
-werkzeug==2.2.2 ; python_version >= "3.7" and python_version < "4.0"
+werkzeug==2.2.3 ; python_version >= "3.7" and python_version < "4.0"
 win32-setctime==1.1.0 ; python_version >= "3.7" and python_version < "4.0" and sys_platform == "win32"
 zc-lockfile==2.0 ; python_version >= "3.7" and python_version < "4.0"
-zipp==3.10.0 ; python_version >= "3.7" and python_version < "3.10"
+zipp==3.11.0 ; python_version >= "3.7" and python_version < "3.10"
 zxcvbn-python==4.4.24 ; python_version >= "3.7" and python_version < "4.0"
```

