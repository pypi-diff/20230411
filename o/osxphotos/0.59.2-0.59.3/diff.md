# Comparing `tmp/osxphotos-0.59.2.tar.gz` & `tmp/osxphotos-0.59.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.59.2.tar", last modified: Sat Apr  8 19:03:54 2023, max compression
+gzip compressed data, was "osxphotos-0.59.3.tar", last modified: Tue Apr 11 02:05:45 2023, max compression
```

## Comparing `osxphotos-0.59.2.tar` & `osxphotos-0.59.3.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.550893 osxphotos-0.59.2/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.59.2/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.59.2/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-08 19:03:54.550669 osxphotos-0.59.2/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   223055 2023-04-08 19:03:42.000000 osxphotos-0.59.2/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.59.2/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.466559 osxphotos-0.59.2/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1850 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.59.2/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15928 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-04-08 19:03:35.000000 osxphotos-0.59.2/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.59.2/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18234 2023-04-08 16:49:38.000000 osxphotos-0.59.2/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.483446 osxphotos-0.59.2/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3482 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.59.2/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6838 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9875 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3628 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    24737 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8517 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.59.2/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      433 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3457 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   106627 2023-04-08 16:09:26.000000 osxphotos-0.59.2/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    21765 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61618 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.59.2/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9663 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20532 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5361 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     7033 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23014 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.59.2/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3324 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26903 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.59.2/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28013 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.59.2/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      633 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.59.2/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5058 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.59.2/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-03-24 13:39:33.000000 osxphotos-0.59.2/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.484249 osxphotos-0.59.2/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.59.2/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1466587 2023-04-08 19:03:51.000000 osxphotos-0.59.2/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.59.2/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.59.2/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.59.2/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51732 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10002 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5048 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.59.2/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2906 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    88922 2023-04-08 18:10:39.000000 osxphotos-0.59.2/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    81848 2023-04-08 18:10:39.000000 osxphotos-0.59.2/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46166 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     5511 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5283 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.486915 osxphotos-0.59.2/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.59.2/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10370 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149198 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.59.2/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-04-08 19:03:41.000000 osxphotos-0.59.2/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78831 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.59.2/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21857 2023-03-24 13:39:33.000000 osxphotos-0.59.2/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.59.2/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.488157 osxphotos-0.59.2/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.59.2/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.59.2/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.59.2/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.59.2/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.59.2/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.59.2/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-03-24 13:39:33.000000 osxphotos-0.59.2/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.489199 osxphotos-0.59.2/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.59.2/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3201 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.59.2/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1682 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.59.2/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)    27026 2023-04-08 16:08:08.000000 osxphotos-0.59.2/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    18282 2023-04-08 16:08:11.000000 osxphotos-0.59.2/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.467600 osxphotos-0.59.2/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6319 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-04-08 19:03:54.000000 osxphotos-0.59.2/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-04-08 19:03:54.550933 osxphotos-0.59.2/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.59.2/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.546954 osxphotos-0.59.2/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-08 19:03:54.550270 osxphotos-0.59.2/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.59.2/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.59.2/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.59.2/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.59.2/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.59.2/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54606 2023-04-08 18:10:39.000000 osxphotos-0.59.2/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   269538 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1693 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4469 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2125 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6692 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.59.2/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 18:03:50.000000 osxphotos-0.59.2/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    29889 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.59.2/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3345 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.59.2/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.59.2/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.59.2/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1931 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.59.2/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.59.2/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.59.2/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18530 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.59.2/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.59.2/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5864 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.59.2/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.59.2/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.59.2/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.59.2/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5059 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.59.2/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.59.2/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.59.2/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.59.2/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.59.2/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.59.2/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18366 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.59.2/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50347 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.59.2/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.59.2/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13297 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.59.2/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.59.2/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.59.2/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.59.2/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.59.2/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.59.2/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.59.2/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.59.2/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.59.2/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.59.2/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.59.2/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.59.2/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.59.2/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.59.2/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.59.2/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    49786 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2324 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     1867 2023-04-08 16:08:08.000000 osxphotos-0.59.2/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.59.2/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    47586 2023-04-08 18:10:39.000000 osxphotos-0.59.2/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.59.2/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.052886 osxphotos-0.59.3/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.59.3/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.59.3/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-11 02:05:45.052663 osxphotos-0.59.3/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   223845 2023-04-11 02:05:33.000000 osxphotos-0.59.3/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.59.3/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:44.999197 osxphotos-0.59.3/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1850 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.59.3/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15928 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-04-11 02:05:26.000000 osxphotos-0.59.3/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.59.3/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.010712 osxphotos-0.59.3/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3482 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.59.3/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6838 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9875 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3628 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26501 2023-04-08 21:34:18.000000 osxphotos-0.59.3/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8517 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.59.3/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      433 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3457 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   106667 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21765 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    61618 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.59.3/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9663 2023-04-08 20:57:19.000000 osxphotos-0.59.3/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20532 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5361 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7033 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23014 2023-04-10 18:30:56.000000 osxphotos-0.59.3/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.59.3/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3324 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26903 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.59.3/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28013 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.59.3/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      633 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-02-03 04:08:06.000000 osxphotos-0.59.3/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5058 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.59.3/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-03-24 13:39:33.000000 osxphotos-0.59.3/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.011189 osxphotos-0.59.3/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.59.3/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1466350 2023-04-11 02:05:41.000000 osxphotos-0.59.3/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.59.3/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.59.3/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.59.3/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51732 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10002 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5048 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.59.3/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2906 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    88952 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    80371 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46166 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5511 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5283 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.013615 osxphotos-0.59.3/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2020-08-09 15:12:11.000000 osxphotos-0.59.3/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10370 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7615 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149077 2023-04-11 02:03:56.000000 osxphotos-0.59.3/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.59.3/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-04-11 02:05:33.000000 osxphotos-0.59.3/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78831 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.59.3/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21857 2023-03-24 13:39:33.000000 osxphotos-0.59.3/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.59.3/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.014494 osxphotos-0.59.3/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.59.3/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.59.3/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.59.3/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.59.3/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.59.3/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13457 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.59.3/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-03-24 13:39:33.000000 osxphotos-0.59.3/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.015090 osxphotos-0.59.3/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.59.3/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3201 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2282 2022-05-05 03:55:31.000000 osxphotos-0.59.3/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1682 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.59.3/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)    27026 2023-04-08 16:08:08.000000 osxphotos-0.59.3/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18282 2023-04-08 16:08:11.000000 osxphotos-0.59.3/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:44.999936 osxphotos-0.59.3/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6319 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-04-11 02:05:44.000000 osxphotos-0.59.3/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-04-11 02:05:45.052923 osxphotos-0.59.3/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.59.3/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.051583 osxphotos-0.59.3/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-04-11 02:05:45.052296 osxphotos-0.59.3/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.59.3/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.59.3/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11012 2022-02-07 05:54:47.000000 osxphotos-0.59.3/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4849 2021-06-12 05:33:53.000000 osxphotos-0.59.3/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5334 2021-06-12 05:33:48.000000 osxphotos-0.59.3/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54621 2023-04-11 02:03:56.000000 osxphotos-0.59.3/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   269538 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1693 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4469 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2125 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6692 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.59.3/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.59.3/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    29889 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6397 2022-05-05 04:33:28.000000 osxphotos-0.59.3/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3345 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.59.3/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.59.3/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.59.3/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1931 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2748 2022-05-06 13:53:04.000000 osxphotos-0.59.3/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-01-21 18:04:00.000000 osxphotos-0.59.3/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.59.3/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18530 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9781 2021-04-26 00:13:29.000000 osxphotos-0.59.3/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18308 2022-05-21 05:13:12.000000 osxphotos-0.59.3/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5864 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.59.3/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10301 2022-05-21 05:13:12.000000 osxphotos-0.59.3/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2021-03-14 19:20:10.000000 osxphotos-0.59.3/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155137 2022-06-17 17:31:26.000000 osxphotos-0.59.3/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5059 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4022 2022-01-01 04:28:52.000000 osxphotos-0.59.3/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.59.3/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1270 2021-06-12 05:43:32.000000 osxphotos-0.59.3/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.59.3/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      859 2021-06-12 05:45:42.000000 osxphotos-0.59.3/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      930 2021-06-12 05:46:24.000000 osxphotos-0.59.3/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18366 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1205 2020-01-12 08:00:41.000000 osxphotos-0.59.3/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50347 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4731 2020-06-27 19:46:37.000000 osxphotos-0.59.3/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4870 2020-06-27 19:50:41.000000 osxphotos-0.59.3/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13297 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5796 2020-10-27 13:37:01.000000 osxphotos-0.59.3/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.59.3/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.59.3/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.59.3/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.59.3/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3376 2022-01-02 07:10:11.000000 osxphotos-0.59.3/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2020-05-11 01:55:25.000000 osxphotos-0.59.3/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7530 2020-12-25 19:00:06.000000 osxphotos-0.59.3/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10047 2022-01-18 16:08:28.000000 osxphotos-0.59.3/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2020-10-05 13:13:43.000000 osxphotos-0.59.3/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.59.3/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3017 2020-08-23 23:26:56.000000 osxphotos-0.59.3/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.59.3/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.59.3/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.59.3/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      489 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    49786 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2324 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1867 2023-04-08 16:08:08.000000 osxphotos-0.59.3/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.59.3/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    47877 2023-04-11 02:03:56.000000 osxphotos-0.59.3/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-03-09 14:25:57.000000 osxphotos-0.59.3/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.59.2/LICENSE` & `osxphotos-0.59.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/PKG-INFO` & `osxphotos-0.59.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.59.2
+Version: 0.59.3
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.59.2/README.md` & `osxphotos-0.59.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/RhetTbull/osxphotos/workflows/Tests/badge.svg)](https://github.com/RhetTbull/osxphotos/workflows/Tests/badge.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/osxphotos)
 [![Downloads](https://static.pepy.tech/personalized-badge/osxphotos?period=month&units=international_system&left_color=black&right_color=brightgreen&left_text=downloads/month)](https://pepy.tech/project/osxphotos)
 [![subreddit](https://img.shields.io/reddit/subreddit-subscribers/osxphotos?style=social)](https://www.reddit.com/r/osxphotos/)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-57-orange.svg?style=flat)](#contributors)
+[![All Contributors](https://img.shields.io/badge/all_contributors-59-orange.svg?style=flat)](#contributors)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 OSXPhotos provides the ability to interact with and query Apple's Photos.app library on macOS. You can query the Photos library database — for example, file name, file path, and metadata such as keywords/tags, persons/faces, albums, etc. You can also easily export both the original and edited photos.
 
 <p align="center"><img src="docs/screencast/demo.gif?raw=true" width="713" height="430"/></p>
 
 # Table of Contents
@@ -2090,15 +2090,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.59.2'
+{osxphotos_version}             The osxphotos version, e.g. '0.59.3'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2577,15 +2577,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.59.2'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.59.3'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
@@ -2661,15 +2661,15 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://blog.dewost.com/"><img src="https://avatars.githubusercontent.com/u/17090228?v=4?s=75" width="75px;" alt="Philippe Dewost"/><br /><sub><b>Philippe Dewost</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=pdewost" title="Documentation">📖</a> <a href="#example-pdewost" title="Examples">💡</a> <a href="#ideas-pdewost" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kaduskj"><img src="https://avatars.githubusercontent.com/u/983067?v=4?s=75" width="75px;" alt="kaduskj"/><br /><sub><b>kaduskj</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Akaduskj" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/mkirkland4874"><img src="https://avatars.githubusercontent.com/u/36466711?v=4?s=75" width="75px;" alt="mkirkland4874"/><br /><sub><b>mkirkland4874</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Amkirkland4874" title="Bug reports">🐛</a> <a href="#example-mkirkland4874" title="Examples">💡</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jcommisso07"><img src="https://avatars.githubusercontent.com/u/3111054?v=4?s=75" width="75px;" alt="Joseph Commisso"/><br /><sub><b>Joseph Commisso</b></sub></a><br /><a href="#data-jcommisso07" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dssinger"><img src="https://avatars.githubusercontent.com/u/1817903?v=4?s=75" width="75px;" alt="David Singer"/><br /><sub><b>David Singer</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Adssinger" title="Bug reports">🐛</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/oPromessa"><img src="https://avatars.githubusercontent.com/u/21261491?v=4?s=75" width="75px;" alt="oPromessa"/><br /><sub><b>oPromessa</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3AoPromessa" title="Bug reports">🐛</a> <a href="#ideas-oPromessa" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=oPromessa" title="Tests">⚠️</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=oPromessa" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/oPromessa"><img src="https://avatars.githubusercontent.com/u/21261491?v=4?s=75" width="75px;" alt="oPromessa"/><br /><sub><b>oPromessa</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3AoPromessa" title="Bug reports">🐛</a> <a href="#ideas-oPromessa" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=oPromessa" title="Tests">⚠️</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=oPromessa" title="Code">💻</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=oPromessa" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://spencerchang.me"><img src="https://avatars.githubusercontent.com/u/14796580?v=4?s=75" width="75px;" alt="Spencer Chang"/><br /><sub><b>Spencer Chang</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aspencerc99" title="Bug reports">🐛</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://www.cs.purdue.edu/homes/dgleich"><img src="https://avatars.githubusercontent.com/u/33995?v=4?s=75" width="75px;" alt="David Gleich"/><br /><sub><b>David Gleich</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=dgleich" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://alandefreitas.github.io/alandefreitas/"><img src="https://avatars.githubusercontent.com/u/5369819?v=4?s=75" width="75px;" alt="Alan de Freitas"/><br /><sub><b>Alan de Freitas</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aalandefreitas" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://hyfen.net"><img src="https://avatars.githubusercontent.com/u/6291?v=4?s=75" width="75px;" alt="Andrew Louis"/><br /><sub><b>Andrew Louis</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=hyfen" title="Documentation">📖</a> <a href="https://github.com/RhetTbull/osxphotos/commits?author=hyfen" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/neebah"><img src="https://avatars.githubusercontent.com/u/71442026?v=4?s=75" width="75px;" alt="neebah"/><br /><sub><b>neebah</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aneebah" title="Bug reports">🐛</a></td>
@@ -2702,14 +2702,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/swduncan"><img src="https://avatars.githubusercontent.com/u/2053195?v=4?s=75" width="75px;" alt="Steve Duncan"/><br /><sub><b>Steve Duncan</b></sub></a><br /><a href="#ideas-swduncan" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://www.projany.com"><img src="https://avatars.githubusercontent.com/u/15144745?v=4?s=75" width="75px;" alt="Ian Moir"/><br /><sub><b>Ian Moir</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Aianmmoir" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pekingduck"><img src="https://avatars.githubusercontent.com/u/2597142?v=4?s=75" width="75px;" alt="Peking Duck"/><br /><sub><b>Peking Duck</b></sub></a><br /><a href="#ideas-pekingduck" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.patreon.com/cclauss"><img src="https://avatars.githubusercontent.com/u/3709715?v=4?s=75" width="75px;" alt="Christian Clauss"/><br /><sub><b>Christian Clauss</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=cclauss" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dvdkon"><img src="https://avatars.githubusercontent.com/u/3526303?v=4?s=75" width="75px;" alt="dvdkon"/><br /><sub><b>dvdkon</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/commits?author=dvdkon" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/wernerzj"><img src="https://avatars.githubusercontent.com/u/130370930?v=4?s=75" width="75px;" alt="wernerzj"/><br /><sub><b>wernerzj</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Awernerzj" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/rajscode"><img src="https://avatars.githubusercontent.com/u/99123253?v=4?s=75" width="75px;" alt="rajscode"/><br /><sub><b>rajscode</b></sub></a><br /><a href="https://github.com/RhetTbull/osxphotos/issues?q=author%3Arajscode" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `osxphotos-0.59.2/README.rst` & `osxphotos-0.59.3/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/__init__.py` & `osxphotos-0.59.3/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/_constants.py` & `osxphotos-0.59.3/osxphotos/_constants.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/adjustmentsinfo.py` & `osxphotos-0.59.3/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/albuminfo.py` & `osxphotos-0.59.3/osxphotos/albuminfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,16 @@
     Returns:
         list of values, sorted by sort_keys
 
     Raises:
         ValueError: raised if len(values) != len(sort_keys)
     """
     if len(values) != len(sort_keys):
-        return ValueError("values and sort_keys must have same length")
-
-    return list(zip(*sorted(zip(sort_keys, values))))[1]
+        raise ValueError("values and sort_keys must be same length")
+    return [x for _, x in sorted(zip(sort_keys, values))]
 
 
 class AlbumInfoBaseClass:
     """
     Base class for AlbumInfo, ImportInfo
     Info about a specific Album, contains all the details about the album
     including folders, photos, etc.
@@ -162,22 +161,21 @@
                     else None
                 )
             except KeyError:
                 self._owner = None
             return self._owner
 
     def asdict(self):
-        """Return album info as a dict"""
+        """Return album info as a dict; does not include photos"""
         return {
             "uuid": self.uuid,
             "creation_date": self.creation_date,
             "start_date": self.start_date,
             "end_date": self.end_date,
             "owner": self.owner,
-            "photos": [p.uuid for p in self.photos],
         }
 
     def __len__(self):
         """return number of photos contained in album"""
         return len(self.photos)
 
 
@@ -295,15 +293,15 @@
             if p.uuid == photo.uuid:
                 return index
         raise ValueError(
             f"Photo with uuid {photo.uuid} does not appear to be in this album"
         )
 
     def asdict(self):
-        """Return album info as a dict"""
+        """Return album info as a dict; does not include photos"""
         dict_data = super().asdict()
         dict_data["title"] = self.title
         dict_data["folder_names"] = self.folder_names
         dict_data["folder_list"] = [f.uuid for f in self.folder_list]
         dict_data["sort_order"] = self.sort_order
         dict_data["parent"] = self.parent.uuid if self.parent else None
         return dict_data
@@ -358,22 +356,21 @@
                     for u in self._db._dbphotos
                     if self._db._dbphotos[u]["import_uuid"] == self.uuid
                 ]
                 self._photos = self._db.photos_by_uuid(import_photo_uuids)
             return self._photos
 
     def asdict(self):
-        """Return import info as a dict"""
+        """Return import info as a dict; does not include photos"""
         return {
             "uuid": self.uuid,
             "creation_date": self.creation_date,
             "start_date": self.start_date,
             "end_date": self.end_date,
             "title": self.title,
-            "photos": [p.uuid for p in self.photos],
         }
 
     def __bool__(self):
         """Always returns True
         A photo without an import session will return None for import_info,
         thus if import_info is not None, it must be a valid import_info object (#820)
         """
```

### Comparing `osxphotos-0.59.2/osxphotos/cli/__init__.py` & `osxphotos-0.59.3/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/about.py` & `osxphotos-0.59.3/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/add_locations.py` & `osxphotos-0.59.3/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/albums.py` & `osxphotos-0.59.3/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/batch_edit.py` & `osxphotos-0.59.3/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/cli.py` & `osxphotos-0.59.3/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/cli_commands.py` & `osxphotos-0.59.3/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/cli_params.py` & `osxphotos-0.59.3/osxphotos/cli/cli_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Common options & parameters for osxphotos CLI commands"""
 
+
 from __future__ import annotations
 
 import functools
 from typing import Any, Callable
-
 import click
-
+import contextlib
+from textwrap import dedent
 from .common import OSXPHOTOS_HIDDEN, print_version
 from .param_types import *
 
 __all__ = [
     "DB_ARGUMENT",
     "DB_OPTION",
     "DEBUG_OPTIONS",
@@ -21,14 +22,57 @@
     "THEME_OPTION",
     "TIMESTAMP_OPTION",
     "VERBOSE_OPTION",
     "VERSION_OPTION",
 ]
 
 
+def validate_selected(ctx, param, value):
+    """ "Validate photos are actually selected when --selected is used"""
+
+    if not value:
+        # --selected not used, just return
+        return value
+
+    # imports here to avoid conflict with linux port
+    # TODO: fix this once linux port is complete
+    import photoscript
+    from applescript import ScriptError
+
+    selection = None
+    with contextlib.suppress(ScriptError):
+        # ScriptError raised if selection made in edit mode or Smart Albums (on older versions of Photos)
+        selection = photoscript.PhotosLibrary().selection
+
+    if not selection:
+        click.echo(
+            dedent(
+                """
+                --selected option used but no photos selected in Photos.
+
+                To select photos in Photos use one of the following methods:
+    
+                - Select a single photo: Click the photo, or press the arrow keys to quickly navigate to and select the photo.
+
+                - Select a group of adjacent photos in a day: Click the first photo, then hold down the Shift key while you click the last photo.
+                You can also hold down Shift and press the arrow keys, or simply drag to enclose the photos within the selection rectangle.
+
+                - Select photos in a day that are not adjacent to each other: Hold down the Command key as you click each photo.
+
+                - Deselect specific photos: Hold down the Command key and click the photos you want to deselect.
+
+                - Deselect all photos: Click an empty space in the window (not a photo).
+            """
+            ),
+            err=True,
+        )
+        ctx.exit(1)
+    return value
+
+
 def _param_memo(f: Callable[..., Any], param: click.Parameter) -> None:
     """Add param to the list of params for a click.Command
     This is directly from the click source code and
     the implementation is thus tightly coupled to click internals
     """
     if isinstance(f, click.Command):
         f.params.append(param)
@@ -553,14 +597,15 @@
         "For example, to find photos in an album that begins with 'Beach': '--regex \"^Beach\" \"{album}\"'. "
         "You may specify more than one regular expression match by repeating '--regex' with different arguments.",
     ),
     "--selected": click.Option(
         ["--selected"],
         is_flag=True,
         help="Filter for photos that are currently selected in Photos.",
+        callback=validate_selected,
     ),
     "--exif": click.Option(
         ["--exif"],
         metavar="EXIF_TAG VALUE",
         nargs=2,
         multiple=True,
         help="Search for photos where EXIF_TAG exists in photo's EXIF data and contains VALUE. "
```

### Comparing `osxphotos-0.59.2/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.59.3/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/color_themes.py` & `osxphotos-0.59.3/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/common.py` & `osxphotos-0.59.3/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/debug_dump.py` & `osxphotos-0.59.3/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/docs.py` & `osxphotos-0.59.3/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/dump.py` & `osxphotos-0.59.3/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.59.3/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/export.py` & `osxphotos-0.59.3/osxphotos/cli/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,15 +907,16 @@
     versions, live photo movies, burst photos, and associated raw images.
     See --skip-edited, --skip-live, --skip-bursts, and --skip-raw options
     to modify this behavior.
     """
 
     # capture locals for use with ConfigOptions before changing any of them
     locals_ = locals()
-    set_crash_data("locals", locals_)
+    crash_data = locals_.copy()
+    set_crash_data("locals", crash_data)
 
     # config expects --verbose to be named "verbose" not "verbose_flag"
     locals_["verbose"] = verbose_flag
     del locals_["verbose_flag"]
 
     # NOTE: because of the way ConfigOptions works, Click options must not
     # set defaults which are not None or False. If defaults need to be set
@@ -2250,15 +2251,15 @@
                 # if debug mode, don't swallow the exceptions
                 raise e
             rich_echo(
                 f"[error]Error exporting photo ([uuid]{photo.uuid}[/uuid]: [filename]{photo.original_filename}[/filename]) as [filepath]{filename}[/filepath]: {e}",
                 err=True,
             )
             if tries > retry:
-                results.error.append((str(pathlib.Path(dest) / filename), e))
+                results.error.append((str(pathlib.Path(dest) / filename), str(e)))
                 break
             else:
                 rich_echo(
                     f"Retrying export for photo ([uuid]{photo.uuid}[/uuid]: [filename]{photo.original_filename}[/filename])"
                 )
 
     if verbose:
```

### Comparing `osxphotos-0.59.2/osxphotos/cli/exportdb.py` & `osxphotos-0.59.3/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/grep.py` & `osxphotos-0.59.3/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/help.py` & `osxphotos-0.59.3/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/import_cli.py` & `osxphotos-0.59.3/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/info.py` & `osxphotos-0.59.3/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.59.3/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/keywords.py` & `osxphotos-0.59.3/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/kvstore.py` & `osxphotos-0.59.3/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/labels.py` & `osxphotos-0.59.3/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/list.py` & `osxphotos-0.59.3/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/orphans.py` & `osxphotos-0.59.3/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/param_types.py` & `osxphotos-0.59.3/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/persons.py` & `osxphotos-0.59.3/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/photo_inspect.py` & `osxphotos-0.59.3/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/places.py` & `osxphotos-0.59.3/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/print_photo_info.py` & `osxphotos-0.59.3/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/query.py` & `osxphotos-0.59.3/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/repl.py` & `osxphotos-0.59.3/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/report_writer.py` & `osxphotos-0.59.3/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/rich_progress.py` & `osxphotos-0.59.3/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/show_command.py` & `osxphotos-0.59.3/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/snap_diff.py` & `osxphotos-0.59.3/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/sync.py` & `osxphotos-0.59.3/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/sync_results.py` & `osxphotos-0.59.3/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/theme.py` & `osxphotos-0.59.3/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/timewarp.py` & `osxphotos-0.59.3/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/tutorial.py` & `osxphotos-0.59.3/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/uuid.py` & `osxphotos-0.59.3/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/verbose.py` & `osxphotos-0.59.3/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/cli/version.py` & `osxphotos-0.59.3/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/compare_exif.py` & `osxphotos-0.59.3/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/configoptions.py` & `osxphotos-0.59.3/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/crash_reporter.py` & `osxphotos-0.59.3/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/datetime_formatter.py` & `osxphotos-0.59.3/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/datetime_utils.py` & `osxphotos-0.59.3/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/debug.py` & `osxphotos-0.59.3/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/docs/docs.zip` & `osxphotos-0.59.3/osxphotos/docs/docs.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1466587 bytes, number of entries: 99
+Zip file size: 1466350 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Apr-08 19:03 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Apr-11 02:05 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
--rw-r--r--  3.0 unx   316898 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photoexporter.html
+-rw-r--r--  3.0 unx   317210 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296574 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/phototemplate.html
 -rw-r--r--  3.0 unx   200939 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
 -rw-r--r--  3.0 unx    49029 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   302969 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx   298462 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
 -rw-r--r--  3.0 unx    29240 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   522970 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx   522689 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/photosdb/photosdb.html
 -rw-r--r--  3.0 unx    36121 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/photosalbum.html
 -rw-r--r--  3.0 unx    92801 tx defN 23-Apr-01 16:39 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
--rw-r--r--  3.0 unx    82949 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/albuminfo.html
+-rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    59723 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
 -rw-r--r--  3.0 unx    61696 tx defN 23-Apr-08 19:03 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Apr-08 19:03 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Apr-11 02:05 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Apr-08 19:03 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Apr-11 02:05 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Apr-08 19:03 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Apr-11 02:05 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Apr-08 19:03 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Apr-11 02:05 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Apr-08 19:03 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Apr-11 02:05 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Apr-08 19:03 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Apr-11 02:05 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   414459 tx defN 23-Apr-08 19:03 docs/cli.html
+-rw-r--r--  3.0 unx   414459 tx defN 23-Apr-11 02:05 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   243757 tx defN 23-Apr-08 19:03 docs/genindex.html
--rw-r--r--  3.0 unx   103771 tx defN 23-Apr-08 19:03 docs/index.html
+-rw-r--r--  3.0 unx   243757 tx defN 23-Apr-11 02:05 docs/genindex.html
+-rw-r--r--  3.0 unx   103771 tx defN 23-Apr-11 02:05 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9391 bx stor 23-Apr-08 19:03 docs/objects.inv
+-rw-r--r--  3.0 unx     9391 bx stor 23-Apr-11 02:05 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Apr-08 19:03 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Apr-08 19:03 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Apr-08 19:03 docs/py-modindex.html
--rw-r--r--  3.0 unx   436053 tx defN 23-Apr-08 19:03 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Apr-11 02:05 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Apr-11 02:05 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Apr-11 02:05 docs/py-modindex.html
+-rw-r--r--  3.0 unx   437653 tx defN 23-Apr-11 02:05 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Apr-08 19:03 docs/search.html
--rw-r--r--  3.0 unx   215828 tx defN 23-Apr-08 19:03 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Apr-08 19:03 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Apr-08 19:03 docs/tutorial.html
-99 files, 6899418 bytes uncompressed, 1447855 bytes compressed:  79.0%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Apr-11 02:05 docs/search.html
+-rw-r--r--  3.0 unx   215837 tx defN 23-Apr-11 02:05 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Apr-11 02:05 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Apr-11 02:05 docs/tutorial.html
+99 files, 6895891 bytes uncompressed, 1447618 bytes compressed:  79.0%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.59.2 documentation</title>
+        <title>Overview: module code - osxphotos 0.59.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoexporter.html

```diff
@@ -1714,18 +1714,18 @@
         <span class="c1"># else, need to check the database to determine if we need to write</span>
         <span class="n">verbose</span><span class="p">(</span>
             <span class="sa">f</span><span class="s2">&quot;Writing metadata with exiftool for </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_filepath</span><span class="p">(</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
         <span class="p">)</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">options</span><span class="o">.</span><span class="n">dry_run</span><span class="p">:</span>
             <span class="n">warning_</span><span class="p">,</span> <span class="n">error_</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_write_exif_data</span><span class="p">(</span><span class="n">src</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="n">options</span><span class="p">)</span>
             <span class="k">if</span> <span class="n">warning_</span><span class="p">:</span>
-                <span class="n">exiftool_results</span><span class="o">.</span><span class="n">exiftool_warning</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">dest</span><span class="p">,</span> <span class="n">warning_</span><span class="p">))</span>
+                <span class="n">exiftool_results</span><span class="o">.</span><span class="n">exiftool_warning</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="nb">str</span><span class="p">(</span><span class="n">dest</span><span class="p">),</span> <span class="nb">str</span><span class="p">(</span><span class="n">warning_</span><span class="p">)))</span>
             <span class="k">if</span> <span class="n">error_</span><span class="p">:</span>
-                <span class="n">exiftool_results</span><span class="o">.</span><span class="n">exiftool_error</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">dest</span><span class="p">,</span> <span class="n">error_</span><span class="p">))</span>
-                <span class="n">exiftool_results</span><span class="o">.</span><span class="n">error</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">dest</span><span class="p">,</span> <span class="n">error_</span><span class="p">))</span>
+                <span class="n">exiftool_results</span><span class="o">.</span><span class="n">exiftool_error</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="nb">str</span><span class="p">(</span><span class="n">dest</span><span class="p">),</span> <span class="nb">str</span><span class="p">(</span><span class="n">error_</span><span class="p">)))</span>
+                <span class="n">exiftool_results</span><span class="o">.</span><span class="n">error</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="nb">str</span><span class="p">(</span><span class="n">dest</span><span class="p">),</span> <span class="nb">str</span><span class="p">(</span><span class="n">error_</span><span class="p">)))</span>
 
         <span class="n">exiftool_results</span><span class="o">.</span><span class="n">exif_updated</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
         <span class="n">exiftool_results</span><span class="o">.</span><span class="n">to_touch</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">dest</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">exiftool_results</span></div>
 
     <span class="k">def</span> <span class="nf">_should_run_exiftool</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dest</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="n">ExportOptions</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
         <span class="sd">&quot;&quot;&quot;Return True if exiftool should be run to update metadata&quot;&quot;&quot;</span>
```

##### html2text {}

```diff
@@ -1734,18 +1734,20 @@
         verbose(
             f"Writing metadata with exiftool for {self._filepath(pathlib.Path
 (dest).name)}"
         )
         if not options.dry_run:
             warning_, error_ = self._write_exif_data(src, options=options)
             if warning_:
-                exiftool_results.exiftool_warning.append((dest, warning_))
+                exiftool_results.exiftool_warning.append((str(dest), str
+(warning_)))
             if error_:
-                exiftool_results.exiftool_error.append((dest, error_))
-                exiftool_results.error.append((dest, error_))
+                exiftool_results.exiftool_error.append((str(dest), str
+(error_)))
+                exiftool_results.error.append((str(dest), str(error_)))
 
         exiftool_results.exif_updated.append(dest)
         exiftool_results.to_touch.append(dest)
         return exiftool_results
 
 
     def _should_run_exiftool(self, dest, options: ExportOptions) -> bool:
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -710,47 +710,34 @@
     <span class="k">def</span> <span class="nf">persons</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;list of persons in picture&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_dbpersons_pk</span><span class="p">[</span><span class="n">pk</span><span class="p">][</span><span class="s2">&quot;fullname&quot;</span><span class="p">]</span> <span class="k">for</span> <span class="n">pk</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;persons&quot;</span><span class="p">]]</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">person_info</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;list of PersonInfo objects for person in picture&quot;&quot;&quot;</span>
-        <span class="k">try</span><span class="p">:</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_personinfo</span>
-        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_personinfo</span> <span class="o">=</span> <span class="p">[</span>
-                <span class="n">PersonInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">pk</span><span class="o">=</span><span class="n">pk</span><span class="p">)</span> <span class="k">for</span> <span class="n">pk</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;persons&quot;</span><span class="p">]</span>
-            <span class="p">]</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_personinfo</span>
+        <span class="k">return</span> <span class="p">[</span><span class="n">PersonInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">pk</span><span class="o">=</span><span class="n">pk</span><span class="p">)</span> <span class="k">for</span> <span class="n">pk</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;persons&quot;</span><span class="p">]]</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">face_info</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;list of FaceInfo objects for faces in picture&quot;&quot;&quot;</span>
         <span class="k">try</span><span class="p">:</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_faceinfo</span>
-        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-            <span class="k">try</span><span class="p">:</span>
-                <span class="n">faces</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_faceinfo_uuid</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="p">]</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">_faceinfo</span> <span class="o">=</span> <span class="p">[</span><span class="n">FaceInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">pk</span><span class="o">=</span><span class="n">pk</span><span class="p">)</span> <span class="k">for</span> <span class="n">pk</span> <span class="ow">in</span> <span class="n">faces</span><span class="p">]</span>
-            <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
-                <span class="c1"># no faces</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">_faceinfo</span> <span class="o">=</span> <span class="p">[]</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_faceinfo</span>
+            <span class="n">faces</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_faceinfo_uuid</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="p">]</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_faceinfo</span> <span class="o">=</span> <span class="p">[</span><span class="n">FaceInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">pk</span><span class="o">=</span><span class="n">pk</span><span class="p">)</span> <span class="k">for</span> <span class="n">pk</span> <span class="ow">in</span> <span class="n">faces</span><span class="p">]</span>
+        <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
+            <span class="c1"># no faces</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_faceinfo</span> <span class="o">=</span> <span class="p">[]</span>
+        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_faceinfo</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">moment_info</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Moment photo belongs to&quot;&quot;&quot;</span>
         <span class="k">try</span><span class="p">:</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span>
-        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-            <span class="k">try</span><span class="p">:</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span> <span class="o">=</span> <span class="n">MomentInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">moment_pk</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;momentID&quot;</span><span class="p">])</span>
-            <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
-                <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span> <span class="o">=</span> <span class="kc">None</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_moment</span>
+            <span class="k">return</span> <span class="n">MomentInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">moment_pk</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;momentID&quot;</span><span class="p">])</span>
+        <span class="k">except</span> <span class="ne">ValueError</span><span class="p">:</span>
+            <span class="k">return</span> <span class="kc">None</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">albums</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;list of albums picture is contained in&quot;&quot;&quot;</span>
         <span class="k">try</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_albums</span>
         <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
@@ -759,88 +746,63 @@
                 <span class="p">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_dbalbum_details</span><span class="p">[</span><span class="n">album</span><span class="p">][</span><span class="s2">&quot;title&quot;</span><span class="p">]</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">album_uuids</span><span class="p">}</span>
             <span class="p">)</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_albums</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">burst_albums</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;If photo is burst photo, list of albums it is contained in as well as any albums the key photo is contained in, otherwise returns self.albums&quot;&quot;&quot;</span>
-        <span class="k">try</span><span class="p">:</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_burst_albums</span>
-        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-            <span class="n">burst_albums</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span>
-            <span class="k">for</span> <span class="n">photo</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_photos</span><span class="p">:</span>
-                <span class="k">if</span> <span class="n">photo</span><span class="o">.</span><span class="n">burst_key</span><span class="p">:</span>
-                    <span class="n">burst_albums</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">photo</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_burst_albums</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">burst_albums</span><span class="p">))</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_burst_albums</span>
+        <span class="n">burst_albums</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span>
+        <span class="k">for</span> <span class="n">photo</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_photos</span><span class="p">:</span>
+            <span class="k">if</span> <span class="n">photo</span><span class="o">.</span><span class="n">burst_key</span><span class="p">:</span>
+                <span class="n">burst_albums</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">photo</span><span class="o">.</span><span class="n">albums</span><span class="p">)</span>
+        <span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">burst_albums</span><span class="p">))</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">album_info</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;list of AlbumInfo objects representing albums the photo is contained in&quot;&quot;&quot;</span>
-        <span class="k">try</span><span class="p">:</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_album_info</span>
-        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-            <span class="n">album_uuids</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_album_uuids</span><span class="p">()</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_album_info</span> <span class="o">=</span> <span class="p">[</span>
-                <span class="n">AlbumInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="n">album</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">album_uuids</span>
-            <span class="p">]</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_album_info</span>
+        <span class="n">album_uuids</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_album_uuids</span><span class="p">()</span>
+        <span class="k">return</span> <span class="p">[</span><span class="n">AlbumInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="n">album</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">album_uuids</span><span class="p">]</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">burst_album_info</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;If photo is a burst photo, returns list of AlbumInfo objects representing albums the photo is contained in as well as albums the burst key photo is contained in, otherwise returns self.album_info.&quot;&quot;&quot;</span>
-        <span class="k">try</span><span class="p">:</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_burst_album_info</span>
-        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-            <span class="n">burst_album_info</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album_info</span><span class="p">)</span>
-            <span class="k">for</span> <span class="n">photo</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_photos</span><span class="p">:</span>
-                <span class="k">if</span> <span class="n">photo</span><span class="o">.</span><span class="n">burst_key</span><span class="p">:</span>
-                    <span class="n">burst_album_info</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">photo</span><span class="o">.</span><span class="n">album_info</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_burst_album_info</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">burst_album_info</span><span class="p">))</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_burst_album_info</span>
+        <span class="n">burst_album_info</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">album_info</span><span class="p">)</span>
+        <span class="k">for</span> <span class="n">photo</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_photos</span><span class="p">:</span>
+            <span class="k">if</span> <span class="n">photo</span><span class="o">.</span><span class="n">burst_key</span><span class="p">:</span>
+                <span class="n">burst_album_info</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">photo</span><span class="o">.</span><span class="n">album_info</span><span class="p">)</span>
+        <span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">burst_album_info</span><span class="p">))</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">import_info</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;ImportInfo object representing import session for the photo or None if no import session&quot;&quot;&quot;</span>
-        <span class="k">try</span><span class="p">:</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_import_info</span>
-        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_import_info</span> <span class="o">=</span> <span class="p">(</span>
-                <span class="n">ImportInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;import_uuid&quot;</span><span class="p">])</span>
-                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;import_uuid&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span>
-                <span class="k">else</span> <span class="kc">None</span>
-            <span class="p">)</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_import_info</span>
+        <span class="k">return</span> <span class="p">(</span>
+            <span class="n">ImportInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;import_uuid&quot;</span><span class="p">])</span>
+            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;import_uuid&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span>
+            <span class="k">else</span> <span class="kc">None</span>
+        <span class="p">)</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">project_info</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;list of AlbumInfo objects representing projects for the photo or None if no projects&quot;&quot;&quot;</span>
-        <span class="k">try</span><span class="p">:</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_project_info</span>
-        <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
-            <span class="n">project_uuids</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_album_uuids</span><span class="p">(</span><span class="n">project</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">_project_info</span> <span class="o">=</span> <span class="p">[</span>
-                <span class="n">ProjectInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="n">album</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">project_uuids</span>
-            <span class="p">]</span>
-            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_project_info</span>
+        <span class="n">project_uuids</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_album_uuids</span><span class="p">(</span><span class="n">project</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+        <span class="k">return</span> <span class="p">[</span><span class="n">ProjectInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="n">album</span><span class="p">)</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="n">project_uuids</span><span class="p">]</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">keywords</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;list of keywords for picture&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;keywords&quot;</span><span class="p">]</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">title</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;name / title of picture&quot;&quot;&quot;</span>
         <span class="c1"># if user sets then deletes title, Photos sets it to empty string in DB instead of NULL</span>
         <span class="c1"># in this case, return None so result is the same as if title had never been set (which returns NULL)</span>
         <span class="c1"># issue #512</span>
         <span class="n">title</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">]</span>
-        <span class="n">title</span> <span class="o">=</span> <span class="kc">None</span> <span class="k">if</span> <span class="n">title</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span> <span class="k">else</span> <span class="n">title</span>
-        <span class="k">return</span> <span class="n">title</span>
+        <span class="k">return</span> <span class="kc">None</span> <span class="k">if</span> <span class="n">title</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span> <span class="k">else</span> <span class="n">title</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">uuid</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;UUID of picture&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span>
 
     <span class="nd">@property</span>
@@ -1970,49 +1932,39 @@
             <span class="s2">&quot;original_height&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_height</span><span class="p">,</span>
             <span class="s2">&quot;original_width&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_width</span><span class="p">,</span>
             <span class="s2">&quot;original_orientation&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_orientation</span><span class="p">,</span>
             <span class="s2">&quot;original_filesize&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_filesize</span><span class="p">,</span>
         <span class="p">}</span>
         <span class="k">return</span> <span class="n">yaml</span><span class="o">.</span><span class="n">dump</span><span class="p">(</span><span class="n">info</span><span class="p">,</span> <span class="n">sort_keys</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
 
-<div class="viewcode-block" id="PhotoInfo.asdict"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo.asdict">[docs]</a>    <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;return dict representation&quot;&quot;&quot;</span>
+<div class="viewcode-block" id="PhotoInfo.asdict"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo.asdict">[docs]</a>    <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">shallow</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="n">Any</span><span class="p">]:</span>
+        <span class="sd">&quot;&quot;&quot;Return dict representation of PhotoInfo object.</span>
+
+<span class="sd">        Args:</span>
+<span class="sd">            shallow: if True, return shallow representation (does not contain folder_info, person_info, etc.)</span>
+
+<span class="sd">        Returns:</span>
+<span class="sd">            dict representation of PhotoInfo object</span>
+
+<span class="sd">        Note:</span>
+<span class="sd">            The shallow representation is used internally by export as it contains only the subset of data needed for export.</span>
+<span class="sd">        &quot;&quot;&quot;</span>
 
-        <span class="n">adjustments</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">adjustments</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">adjustments</span> <span class="k">else</span> <span class="p">{}</span>
-        <span class="n">album_info</span> <span class="o">=</span> <span class="p">[</span><span class="n">album</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album_info</span><span class="p">]</span>
-        <span class="n">burst_album_info</span> <span class="o">=</span> <span class="p">[</span><span class="n">a</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">a</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_album_info</span><span class="p">]</span>
-        <span class="n">burst_photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_photos</span><span class="p">]</span>
         <span class="n">comments</span> <span class="o">=</span> <span class="p">[</span><span class="n">comment</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">comment</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">comments</span><span class="p">]</span>
         <span class="n">exif_info</span> <span class="o">=</span> <span class="n">dataclasses</span><span class="o">.</span><span class="n">asdict</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">exif_info</span><span class="p">)</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">exif_info</span> <span class="k">else</span> <span class="p">{}</span>
         <span class="n">face_info</span> <span class="o">=</span> <span class="p">[</span><span class="n">face</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">face</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">face_info</span><span class="p">]</span>
         <span class="n">folders</span> <span class="o">=</span> <span class="p">{</span><span class="n">album</span><span class="o">.</span><span class="n">title</span><span class="p">:</span> <span class="n">album</span><span class="o">.</span><span class="n">folder_names</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album_info</span><span class="p">}</span>
-        <span class="n">import_info</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">import_info</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">import_info</span> <span class="k">else</span> <span class="p">{}</span>
         <span class="n">likes</span> <span class="o">=</span> <span class="p">[</span><span class="n">like</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">like</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">likes</span><span class="p">]</span>
-        <span class="n">person_info</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">person_info</span><span class="p">]</span>
         <span class="n">place</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">place</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">place</span> <span class="k">else</span> <span class="p">{}</span>
-        <span class="n">project_info</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">project_info</span><span class="p">]</span>
         <span class="n">score</span> <span class="o">=</span> <span class="n">dataclasses</span><span class="o">.</span><span class="n">asdict</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">score</span><span class="p">)</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">score</span> <span class="k">else</span> <span class="p">{}</span>
-        <span class="n">search_info</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">search_info</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">search_info</span> <span class="k">else</span> <span class="p">{}</span>
-        <span class="n">search_info_normalized</span> <span class="o">=</span> <span class="p">(</span>
-            <span class="bp">self</span><span class="o">.</span><span class="n">search_info_normalized</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">search_info_normalized</span> <span class="k">else</span> <span class="p">{}</span>
-        <span class="p">)</span>
 
-        <span class="k">return</span> <span class="p">{</span>
-            <span class="s2">&quot;adjustments&quot;</span><span class="p">:</span> <span class="n">adjustments</span><span class="p">,</span>
-            <span class="s2">&quot;album_info&quot;</span><span class="p">:</span> <span class="n">album_info</span><span class="p">,</span>
+        <span class="n">dict_data</span> <span class="o">=</span> <span class="p">{</span>
             <span class="s2">&quot;albums&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">albums</span><span class="p">,</span>
-            <span class="s2">&quot;burst_album_info&quot;</span><span class="p">:</span> <span class="n">burst_album_info</span><span class="p">,</span>
-            <span class="s2">&quot;burst_albums&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_albums</span><span class="p">,</span>
-            <span class="s2">&quot;burst_default_pick&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_default_pick</span><span class="p">,</span>
-            <span class="s2">&quot;burst_key&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_key</span><span class="p">,</span>
-            <span class="s2">&quot;burst_photos&quot;</span><span class="p">:</span> <span class="n">burst_photos</span><span class="p">,</span>
-            <span class="s2">&quot;burst_selected&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_selected</span><span class="p">,</span>
             <span class="s2">&quot;burst&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst</span><span class="p">,</span>
             <span class="s2">&quot;cloud_guid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">cloud_guid</span><span class="p">,</span>
-            <span class="s2">&quot;cloud_metadata&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">cloud_metadata</span><span class="p">,</span>
             <span class="s2">&quot;cloud_owner_hashed_id&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">cloud_owner_hashed_id</span><span class="p">,</span>
             <span class="s2">&quot;comments&quot;</span><span class="p">:</span> <span class="n">comments</span><span class="p">,</span>
             <span class="s2">&quot;date_added&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">date_added</span><span class="p">,</span>
             <span class="s2">&quot;date_modified&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">date_modified</span><span class="p">,</span>
             <span class="s2">&quot;date_trashed&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">date_trashed</span><span class="p">,</span>
             <span class="s2">&quot;date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">date</span><span class="p">,</span>
             <span class="s2">&quot;description&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">description</span><span class="p">,</span>
@@ -2024,25 +1976,23 @@
             <span class="s2">&quot;fingerprint&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">fingerprint</span><span class="p">,</span>
             <span class="s2">&quot;folders&quot;</span><span class="p">:</span> <span class="n">folders</span><span class="p">,</span>
             <span class="s2">&quot;has_raw&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">has_raw</span><span class="p">,</span>
             <span class="s2">&quot;hasadjustments&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">hasadjustments</span><span class="p">,</span>
             <span class="s2">&quot;hdr&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">hdr</span><span class="p">,</span>
             <span class="s2">&quot;height&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">height</span><span class="p">,</span>
             <span class="s2">&quot;hidden&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">hidden</span><span class="p">,</span>
-            <span class="s2">&quot;import_info&quot;</span><span class="p">:</span> <span class="n">import_info</span><span class="p">,</span>
             <span class="s2">&quot;incloud&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">incloud</span><span class="p">,</span>
             <span class="s2">&quot;intrash&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">intrash</span><span class="p">,</span>
             <span class="s2">&quot;iscloudasset&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">iscloudasset</span><span class="p">,</span>
             <span class="s2">&quot;ismissing&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">ismissing</span><span class="p">,</span>
             <span class="s2">&quot;ismovie&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">ismovie</span><span class="p">,</span>
             <span class="s2">&quot;isphoto&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">isphoto</span><span class="p">,</span>
             <span class="s2">&quot;israw&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">israw</span><span class="p">,</span>
             <span class="s2">&quot;isreference&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">isreference</span><span class="p">,</span>
             <span class="s2">&quot;keywords&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">keywords</span><span class="p">,</span>
-            <span class="s2">&quot;labels_normalized&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">labels_normalized</span><span class="p">,</span>
             <span class="s2">&quot;labels&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">labels</span><span class="p">,</span>
             <span class="s2">&quot;latitude&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">_latitude</span><span class="p">,</span>
             <span class="s2">&quot;library&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
             <span class="s2">&quot;likes&quot;</span><span class="p">:</span> <span class="n">likes</span><span class="p">,</span>
             <span class="s2">&quot;live_photo&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">live_photo</span><span class="p">,</span>
             <span class="s2">&quot;location&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">location</span><span class="p">,</span>
             <span class="s2">&quot;longitude&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">_longitude</span><span class="p">,</span>
@@ -2050,84 +2000,90 @@
             <span class="s2">&quot;original_filename&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_filename</span><span class="p">,</span>
             <span class="s2">&quot;original_filesize&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_filesize</span><span class="p">,</span>
             <span class="s2">&quot;original_height&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_height</span><span class="p">,</span>
             <span class="s2">&quot;original_orientation&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_orientation</span><span class="p">,</span>
             <span class="s2">&quot;original_width&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">original_width</span><span class="p">,</span>
             <span class="s2">&quot;owner&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">owner</span><span class="p">,</span>
             <span class="s2">&quot;panorama&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">panorama</span><span class="p">,</span>
-            <span class="s2">&quot;path_derivatives&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_derivatives</span><span class="p">,</span>
             <span class="s2">&quot;path_edited_live_photo&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_edited_live_photo</span><span class="p">,</span>
             <span class="s2">&quot;path_edited&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_edited</span><span class="p">,</span>
             <span class="s2">&quot;path_live_photo&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_live_photo</span><span class="p">,</span>
             <span class="s2">&quot;path_raw&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_raw</span><span class="p">,</span>
             <span class="s2">&quot;path&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">path</span><span class="p">,</span>
-            <span class="s2">&quot;person_info&quot;</span><span class="p">:</span> <span class="n">person_info</span><span class="p">,</span>
             <span class="s2">&quot;persons&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">persons</span><span class="p">,</span>
             <span class="s2">&quot;place&quot;</span><span class="p">:</span> <span class="n">place</span><span class="p">,</span>
             <span class="s2">&quot;portrait&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">portrait</span><span class="p">,</span>
-            <span class="s2">&quot;project_info&quot;</span><span class="p">:</span> <span class="n">project_info</span><span class="p">,</span>
             <span class="s2">&quot;raw_original&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">raw_original</span><span class="p">,</span>
             <span class="s2">&quot;score&quot;</span><span class="p">:</span> <span class="n">score</span><span class="p">,</span>
             <span class="s2">&quot;screenshot&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">screenshot</span><span class="p">,</span>
-            <span class="s2">&quot;search_info_normalized&quot;</span><span class="p">:</span> <span class="n">search_info_normalized</span><span class="p">,</span>
-            <span class="s2">&quot;search_info&quot;</span><span class="p">:</span> <span class="n">search_info</span><span class="p">,</span>
             <span class="s2">&quot;selfie&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">selfie</span><span class="p">,</span>
             <span class="s2">&quot;shared&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">,</span>
             <span class="s2">&quot;slow_mo&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">slow_mo</span><span class="p">,</span>
             <span class="s2">&quot;time_lapse&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">time_lapse</span><span class="p">,</span>
             <span class="s2">&quot;title&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="p">,</span>
             <span class="s2">&quot;tzoffset&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">tzoffset</span><span class="p">,</span>
             <span class="s2">&quot;uti_edited&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uti_edited</span><span class="p">,</span>
             <span class="s2">&quot;uti_original&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uti_original</span><span class="p">,</span>
             <span class="s2">&quot;uti_raw&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uti_raw</span><span class="p">,</span>
             <span class="s2">&quot;uti&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uti</span><span class="p">,</span>
             <span class="s2">&quot;uuid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">,</span>
             <span class="s2">&quot;visible&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">visible</span><span class="p">,</span>
             <span class="s2">&quot;width&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">width</span><span class="p">,</span>
-        <span class="p">}</span></div>
+        <span class="p">}</span>
+
+        <span class="c1"># non-shallow keys</span>
+        <span class="k">if</span> <span class="ow">not</span> <span class="n">shallow</span><span class="p">:</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;album_info&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">album</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">album_info</span><span class="p">]</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;path_derivatives&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">path_derivatives</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;adjustments&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">(</span>
+                <span class="bp">self</span><span class="o">.</span><span class="n">adjustments</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">adjustments</span> <span class="k">else</span> <span class="p">{}</span>
+            <span class="p">)</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;burst_album_info&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">a</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">a</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_album_info</span><span class="p">]</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;burst_albums&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_albums</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;burst_default_pick&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_default_pick</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;burst_key&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_key</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;burst_photos&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_photos</span><span class="p">]</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;burst_selected&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">burst_selected</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;cloud_metadata&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cloud_metadata</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;import_info&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">(</span>
+                <span class="bp">self</span><span class="o">.</span><span class="n">import_info</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">import_info</span> <span class="k">else</span> <span class="p">{}</span>
+            <span class="p">)</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;labels_normalized&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">labels_normalized</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;person_info&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">person_info</span><span class="p">]</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;project_info&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">project_info</span><span class="p">]</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;search_info&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">(</span>
+                <span class="bp">self</span><span class="o">.</span><span class="n">search_info</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">search_info</span> <span class="k">else</span> <span class="p">{}</span>
+            <span class="p">)</span>
+            <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;search_info_normalized&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">(</span>
+                <span class="bp">self</span><span class="o">.</span><span class="n">search_info_normalized</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span>
+                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">search_info_normalized</span>
+                <span class="k">else</span> <span class="p">{}</span>
+            <span class="p">)</span>
+
+        <span class="k">return</span> <span class="n">dict_data</span></div>
 
-<div class="viewcode-block" id="PhotoInfo.json"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo.json">[docs]</a>    <span class="k">def</span> <span class="nf">json</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">indent</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">shallow</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+<div class="viewcode-block" id="PhotoInfo.json"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotoInfo.json">[docs]</a>    <span class="k">def</span> <span class="nf">json</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">indent</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">shallow</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
         <span class="sd">&quot;&quot;&quot;Return JSON representation</span>
 
 <span class="sd">        Args:</span>
 <span class="sd">            indent: indent level for JSON, if None, no indent</span>
 <span class="sd">            shallow: if True, return shallow JSON representation (does not contain folder_info, person_info, etc.)</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">            JSON string</span>
+
+<span class="sd">        Note:</span>
+<span class="sd">            The shallow representation is used internally by export as it contains only the subset of data needed for export.</span>
 <span class="sd">        &quot;&quot;&quot;</span>
 
         <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="n">o</span><span class="p">):</span>
             <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">o</span><span class="p">,</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">date</span><span class="p">,</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">)):</span>
                 <span class="k">return</span> <span class="n">o</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span>
 
-        <span class="n">dict_data</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span>
-
-        <span class="k">if</span> <span class="n">shallow</span><span class="p">:</span>
-            <span class="c1"># delete items that are not needed for shallow JSON</span>
-            <span class="c1"># these are removed to match behavior of osxphotos &lt; 0.59.0 (See #999, #1039)</span>
-            <span class="k">for</span> <span class="n">key</span> <span class="ow">in</span> <span class="p">[</span>
-                <span class="s2">&quot;adjustments&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;album_info&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;burst_album_info&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;burst_albums&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;burst_default_pick&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;burst_key&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;burst_photos&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;burst_selected&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;cloud_metadata&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;import_info&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;labels_normalized&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;path_derivatives&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;person_info&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;project_info&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;search_info_normalized&quot;</span><span class="p">,</span>
-                <span class="s2">&quot;search_info&quot;</span><span class="p">,</span>
-            <span class="p">]:</span>
-                <span class="k">del</span> <span class="n">dict_data</span><span class="p">[</span><span class="n">key</span><span class="p">]</span>
+        <span class="n">dict_data</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">(</span><span class="n">shallow</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> <span class="k">if</span> <span class="n">shallow</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">(</span><span class="n">shallow</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
 
         <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">dict_data</span><span class="o">.</span><span class="n">items</span><span class="p">():</span>
             <span class="c1"># sort lists such as keywords so JSON is consistent</span>
             <span class="c1"># but do not sort certain items like location</span>
             <span class="k">if</span> <span class="n">k</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;location&quot;</span><span class="p">]:</span>
                 <span class="k">continue</span>
             <span class="k">if</span> <span class="n">v</span> <span class="ow">and</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">v</span><span class="p">,</span> <span class="p">(</span><span class="nb">list</span><span class="p">,</span> <span class="nb">tuple</span><span class="p">))</span> <span class="ow">and</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">v</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="nb">dict</span><span class="p">):</span>
@@ -2142,23 +2098,17 @@
         <span class="c1"># for computing hexdigest so we can ignore them</span>
         <span class="c1"># also don&#39;t use visible because it changes based on Photos UI state</span>
 
         <span class="k">def</span> <span class="nf">default</span><span class="p">(</span><span class="n">o</span><span class="p">):</span>
             <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">o</span><span class="p">,</span> <span class="p">(</span><span class="n">datetime</span><span class="o">.</span><span class="n">date</span><span class="p">,</span> <span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">)):</span>
                 <span class="k">return</span> <span class="n">o</span><span class="o">.</span><span class="n">isoformat</span><span class="p">()</span>
 
-        <span class="n">dict_data</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span>
+        <span class="n">dict_data</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">asdict</span><span class="p">(</span><span class="n">shallow</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
 
-        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="p">[</span>
-            <span class="s2">&quot;album_info&quot;</span><span class="p">,</span>
-            <span class="s2">&quot;burst_album_info&quot;</span><span class="p">,</span>
-            <span class="s2">&quot;face_info&quot;</span><span class="p">,</span>
-            <span class="s2">&quot;person_info&quot;</span><span class="p">,</span>
-            <span class="s2">&quot;visible&quot;</span><span class="p">,</span>
-        <span class="p">]:</span>
+        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;face_info&quot;</span><span class="p">,</span> <span class="s2">&quot;visible&quot;</span><span class="p">]:</span>
             <span class="k">del</span> <span class="n">dict_data</span><span class="p">[</span><span class="n">k</span><span class="p">]</span>
 
         <span class="k">for</span> <span class="n">k</span><span class="p">,</span> <span class="n">v</span> <span class="ow">in</span> <span class="n">dict_data</span><span class="o">.</span><span class="n">items</span><span class="p">():</span>
             <span class="c1"># sort lists such as keywords so JSON is consistent</span>
             <span class="c1"># but do not sort certain items like location</span>
             <span class="k">if</span> <span class="n">k</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;location&quot;</span><span class="p">]:</span>
                 <span class="k">continue</span>
```

##### html2text {}

```diff
@@ -578,48 +578,34 @@
         """list of persons in picture"""
         return [self._db._dbpersons_pk[pk]["fullname"] for pk in self._info
 ["persons"]]
 
     @property
     def person_info(self):
         """list of PersonInfo objects for person in picture"""
-        try:
-            return self._personinfo
-        except AttributeError:
-            self._personinfo = [
-                PersonInfo(db=self._db, pk=pk) for pk in self._info["persons"]
-            ]
-            return self._personinfo
+        return [PersonInfo(db=self._db, pk=pk) for pk in self._info["persons"]]
 
     @property
     def face_info(self):
         """list of FaceInfo objects for faces in picture"""
         try:
-            return self._faceinfo
-        except AttributeError:
-            try:
-                faces = self._db._db_faceinfo_uuid[self._uuid]
-                self._faceinfo = [FaceInfo(db=self._db, pk=pk) for pk in faces]
-            except KeyError:
-                # no faces
-                self._faceinfo = []
-            return self._faceinfo
+            faces = self._db._db_faceinfo_uuid[self._uuid]
+            self._faceinfo = [FaceInfo(db=self._db, pk=pk) for pk in faces]
+        except KeyError:
+            # no faces
+            self._faceinfo = []
+        return self._faceinfo
 
     @property
     def moment_info(self):
         """Moment photo belongs to"""
         try:
-            return self._moment
-        except AttributeError:
-            try:
-                self._moment = MomentInfo(db=self._db, moment_pk=self._info
-["momentID"])
-            except ValueError:
-                self._moment = None
-            return self._moment
+            return MomentInfo(db=self._db, moment_pk=self._info["momentID"])
+        except ValueError:
+            return None
 
     @property
     def albums(self):
         """list of albums picture is contained in"""
         try:
             return self._albums
         except AttributeError:
@@ -630,78 +616,55 @@
             )
             return self._albums
 
     @property
     def burst_albums(self):
         """If photo is burst photo, list of albums it is contained in as well
 as any albums the key photo is contained in, otherwise returns self.albums"""
-        try:
-            return self._burst_albums
-        except AttributeError:
-            burst_albums = list(self.albums)
-            for photo in self.burst_photos:
-                if photo.burst_key:
-                    burst_albums.extend(photo.albums)
-            self._burst_albums = list(set(burst_albums))
-            return self._burst_albums
+        burst_albums = list(self.albums)
+        for photo in self.burst_photos:
+            if photo.burst_key:
+                burst_albums.extend(photo.albums)
+        return list(set(burst_albums))
 
     @property
     def album_info(self):
         """list of AlbumInfo objects representing albums the photo is contained
 in"""
-        try:
-            return self._album_info
-        except AttributeError:
-            album_uuids = self._get_album_uuids()
-            self._album_info = [
-                AlbumInfo(db=self._db, uuid=album) for album in album_uuids
-            ]
-            return self._album_info
+        album_uuids = self._get_album_uuids()
+        return [AlbumInfo(db=self._db, uuid=album) for album in album_uuids]
 
     @property
     def burst_album_info(self):
         """If photo is a burst photo, returns list of AlbumInfo objects
 representing albums the photo is contained in as well as albums the burst key
 photo is contained in, otherwise returns self.album_info."""
-        try:
-            return self._burst_album_info
-        except AttributeError:
-            burst_album_info = list(self.album_info)
-            for photo in self.burst_photos:
-                if photo.burst_key:
-                    burst_album_info.extend(photo.album_info)
-            self._burst_album_info = list(set(burst_album_info))
-            return self._burst_album_info
+        burst_album_info = list(self.album_info)
+        for photo in self.burst_photos:
+            if photo.burst_key:
+                burst_album_info.extend(photo.album_info)
+        return list(set(burst_album_info))
 
     @property
     def import_info(self):
         """ImportInfo object representing import session for the photo or None
 if no import session"""
-        try:
-            return self._import_info
-        except AttributeError:
-            self._import_info = (
-                ImportInfo(db=self._db, uuid=self._info["import_uuid"])
-                if self._info["import_uuid"] is not None
-                else None
-            )
-            return self._import_info
+        return (
+            ImportInfo(db=self._db, uuid=self._info["import_uuid"])
+            if self._info["import_uuid"] is not None
+            else None
+        )
 
     @property
     def project_info(self):
         """list of AlbumInfo objects representing projects for the photo or
 None if no projects"""
-        try:
-            return self._project_info
-        except AttributeError:
-            project_uuids = self._get_album_uuids(project=True)
-            self._project_info = [
-                ProjectInfo(db=self._db, uuid=album) for album in project_uuids
-            ]
-            return self._project_info
+        project_uuids = self._get_album_uuids(project=True)
+        return [ProjectInfo(db=self._db, uuid=album) for album in
+project_uuids]
 
     @property
     def keywords(self):
         """list of keywords for picture"""
         return self._info["keywords"]
 
     @property
@@ -709,16 +672,15 @@
         """name / title of picture"""
         # if user sets then deletes title, Photos sets it to empty string in DB
 instead of NULL
         # in this case, return None so result is the same as if title had never
 been set (which returns NULL)
         # issue #512
         title = self._info["name"]
-        title = None if title == "" else title
-        return title
+        return None if title == "" else title
 
     @property
     def uuid(self):
         """UUID of picture"""
         return self._uuid
 
     @property
@@ -1957,52 +1919,43 @@
             "original_height": self.original_height,
             "original_width": self.original_width,
             "original_orientation": self.original_orientation,
             "original_filesize": self.original_filesize,
         }
         return yaml.dump(info, sort_keys=False)
 
-[docs]    def asdict(self):
-        """return dict representation"""
+[docs]    def asdict(self, shallow: bool = True) -> dict[str, Any]:
+        """Return dict representation of PhotoInfo object.
+
+        Args:
+            shallow: if True, return shallow representation (does not contain
+folder_info, person_info, etc.)
+
+        Returns:
+            dict representation of PhotoInfo object
+
+        Note:
+            The shallow representation is used internally by export as it
+contains only the subset of data needed for export.
+        """
 
-        adjustments = self.adjustments.asdict() if self.adjustments else {}
-        album_info = [album.asdict() for album in self.album_info]
-        burst_album_info = [a.asdict() for a in self.burst_album_info]
-        burst_photos = [p.uuid for p in self.burst_photos]
         comments = [comment.asdict() for comment in self.comments]
         exif_info = dataclasses.asdict(self.exif_info) if self.exif_info else
 {}
         face_info = [face.asdict() for face in self.face_info]
         folders = {album.title: album.folder_names for album in
 self.album_info}
-        import_info = self.import_info.asdict() if self.import_info else {}
         likes = [like.asdict() for like in self.likes]
-        person_info = [p.asdict() for p in self.person_info]
         place = self.place.asdict() if self.place else {}
-        project_info = [p.asdict() for p in self.project_info]
         score = dataclasses.asdict(self.score) if self.score else {}
-        search_info = self.search_info.asdict() if self.search_info else {}
-        search_info_normalized = (
-            self.search_info_normalized.asdict() if self.search_info_normalized
-else {}
-        )
 
-        return {
-            "adjustments": adjustments,
-            "album_info": album_info,
+        dict_data = {
             "albums": self.albums,
-            "burst_album_info": burst_album_info,
-            "burst_albums": self.burst_albums,
-            "burst_default_pick": self.burst_default_pick,
-            "burst_key": self.burst_key,
-            "burst_photos": burst_photos,
-            "burst_selected": self.burst_selected,
             "burst": self.burst,
             "cloud_guid": self.cloud_guid,
-            "cloud_metadata": self.cloud_metadata,
             "cloud_owner_hashed_id": self.cloud_owner_hashed_id,
             "comments": comments,
             "date_added": self.date_added,
             "date_modified": self.date_modified,
             "date_trashed": self.date_trashed,
             "date": self.date,
             "description": self.description,
@@ -2014,25 +1967,23 @@
             "fingerprint": self.fingerprint,
             "folders": folders,
             "has_raw": self.has_raw,
             "hasadjustments": self.hasadjustments,
             "hdr": self.hdr,
             "height": self.height,
             "hidden": self.hidden,
-            "import_info": import_info,
             "incloud": self.incloud,
             "intrash": self.intrash,
             "iscloudasset": self.iscloudasset,
             "ismissing": self.ismissing,
             "ismovie": self.ismovie,
             "isphoto": self.isphoto,
             "israw": self.israw,
             "isreference": self.isreference,
             "keywords": self.keywords,
-            "labels_normalized": self.labels_normalized,
             "labels": self.labels,
             "latitude": self._latitude,
             "library": self._db._library_path,
             "likes": likes,
             "live_photo": self.live_photo,
             "location": self.location,
             "longitude": self._longitude,
@@ -2040,30 +1991,25 @@
             "original_filename": self.original_filename,
             "original_filesize": self.original_filesize,
             "original_height": self.original_height,
             "original_orientation": self.original_orientation,
             "original_width": self.original_width,
             "owner": self.owner,
             "panorama": self.panorama,
-            "path_derivatives": self.path_derivatives,
             "path_edited_live_photo": self.path_edited_live_photo,
             "path_edited": self.path_edited,
             "path_live_photo": self.path_live_photo,
             "path_raw": self.path_raw,
             "path": self.path,
-            "person_info": person_info,
             "persons": self.persons,
             "place": place,
             "portrait": self.portrait,
-            "project_info": project_info,
             "raw_original": self.raw_original,
             "score": score,
             "screenshot": self.screenshot,
-            "search_info_normalized": search_info_normalized,
-            "search_info": search_info,
             "selfie": self.selfie,
             "shared": self.shared,
             "slow_mo": self.slow_mo,
             "time_lapse": self.time_lapse,
             "title": self.title,
             "tzoffset": self.tzoffset,
             "uti_edited": self.uti_edited,
@@ -2071,57 +2017,71 @@
             "uti_raw": self.uti_raw,
             "uti": self.uti,
             "uuid": self.uuid,
             "visible": self.visible,
             "width": self.width,
         }
 
+        # non-shallow keys
+        if not shallow:
+            dict_data["album_info"] = [album.asdict() for album in
+self.album_info]
+            dict_data["path_derivatives"] = self.path_derivatives
+            dict_data["adjustments"] = (
+                self.adjustments.asdict() if self.adjustments else {}
+            )
+            dict_data["burst_album_info"] = [a.asdict() for a in
+self.burst_album_info]
+            dict_data["burst_albums"] = self.burst_albums
+            dict_data["burst_default_pick"] = self.burst_default_pick
+            dict_data["burst_key"] = self.burst_key
+            dict_data["burst_photos"] = [p.uuid for p in self.burst_photos]
+            dict_data["burst_selected"] = self.burst_selected
+            dict_data["cloud_metadata"] = self.cloud_metadata
+            dict_data["import_info"] = (
+                self.import_info.asdict() if self.import_info else {}
+            )
+            dict_data["labels_normalized"] = self.labels_normalized
+            dict_data["person_info"] = [p.asdict() for p in self.person_info]
+            dict_data["project_info"] = [p.asdict() for p in self.project_info]
+            dict_data["search_info"] = (
+                self.search_info.asdict() if self.search_info else {}
+            )
+            dict_data["search_info_normalized"] = (
+                self.search_info_normalized.asdict()
+                if self.search_info_normalized
+                else {}
+            )
+
+        return dict_data
+
 
-[docs]    def json(self, indent: int | None = None, shallow: bool = False) -
+[docs]    def json(self, indent: int | None = None, shallow: bool = True) -
 > str:
         """Return JSON representation
 
         Args:
             indent: indent level for JSON, if None, no indent
             shallow: if True, return shallow JSON representation (does not
 contain folder_info, person_info, etc.)
 
         Returns:
             JSON string
+
+        Note:
+            The shallow representation is used internally by export as it
+contains only the subset of data needed for export.
         """
 
         def default(o):
             if isinstance(o, (datetime.date, datetime.datetime)):
                 return o.isoformat()
 
-        dict_data = self.asdict()
-
-        if shallow:
-            # delete items that are not needed for shallow JSON
-            # these are removed to match behavior of osxphotos < 0.59.0 (See
-#999, #1039)
-            for key in [
-                "adjustments",
-                "album_info",
-                "burst_album_info",
-                "burst_albums",
-                "burst_default_pick",
-                "burst_key",
-                "burst_photos",
-                "burst_selected",
-                "cloud_metadata",
-                "import_info",
-                "labels_normalized",
-                "path_derivatives",
-                "person_info",
-                "project_info",
-                "search_info_normalized",
-                "search_info",
-            ]:
-                del dict_data[key]
+        dict_data = self.asdict(shallow=True) if shallow else self.asdict
+(shallow=False)
 
         for k, v in dict_data.items():
             # sort lists such as keywords so JSON is consistent
             # but do not sort certain items like location
             if k in ["location"]:
                 continue
             if v and isinstance(v, (list, tuple)) and not isinstance(v[0],
@@ -2142,23 +2102,17 @@
         # for computing hexdigest so we can ignore them
         # also don't use visible because it changes based on Photos UI state
 
         def default(o):
             if isinstance(o, (datetime.date, datetime.datetime)):
                 return o.isoformat()
 
-        dict_data = self.asdict()
+        dict_data = self.asdict(shallow=True)
 
-        for k in [
-            "album_info",
-            "burst_album_info",
-            "face_info",
-            "person_info",
-            "visible",
-        ]:
+        for k in ["face_info", "visible"]:
             del dict_data[k]
 
         for k, v in dict_data.items():
             # sort lists such as keywords so JSON is consistent
             # but do not sort certain items like location
             if k in ["location"]:
                 continue
```

#### docs/_modules/osxphotos/photosdb/photosdb.html

```diff
@@ -709,15 +709,16 @@
                 <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_album_uuids</span><span class="p">(</span><span class="n">shared</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
             <span class="p">]</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_album_info</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">album_info_shared</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;return list of AlbumInfo objects for each shared album in the photos database</span>
-<span class="sd">        only valid for Photos 5; on Photos &lt;= 4, prints warning and returns empty list&quot;&quot;&quot;</span>
+<span class="sd">        only valid for Photos 5; on Photos &lt;= 4, prints warning and returns empty list</span>
+<span class="sd">        &quot;&quot;&quot;</span>
         <span class="c1"># if _dbalbum_details[key][&quot;cloudownerhashedpersonid&quot;] is not None, then it&#39;s a shared album</span>
         <span class="k">try</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_album_info_shared</span>
         <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_album_info_shared</span> <span class="o">=</span> <span class="p">[</span>
                 <span class="n">AlbumInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="n">album</span><span class="p">)</span>
                 <span class="k">for</span> <span class="n">album</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_album_uuids</span><span class="p">(</span><span class="n">shared</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
@@ -736,15 +737,16 @@
         <span class="k">except</span> <span class="ne">AttributeError</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_albums</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_albums</span><span class="p">(</span><span class="n">shared</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_albums</span>
 
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">albums_shared</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;return list of shared albums found in photos database</span>
-<span class="sd">        only valid for Photos 5; on Photos &lt;= 4, prints warning and returns empty list&quot;&quot;&quot;</span>
+<span class="sd">        only valid for Photos 5; on Photos &lt;= 4, prints warning and returns empty list</span>
+<span class="sd">        &quot;&quot;&quot;</span>
 
         <span class="c1"># Could be more than one album with same name</span>
         <span class="c1"># Right now, they are treated as same album and photos are combined from albums with same name</span>
 
         <span class="c1"># if _dbalbum_details[key][&quot;cloudownerhashedpersonid&quot;] is not None, then it&#39;s a shared album</span>
 
         <span class="k">try</span><span class="p">:</span>
@@ -3246,35 +3248,31 @@
 <span class="sd">            PhotoInfo instance for photo with UUID matching uuid or None if no match</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">try</span><span class="p">:</span>
             <span class="k">return</span> <span class="n">PhotoInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="n">uuid</span><span class="p">,</span> <span class="n">info</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">])</span>
         <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span></div>
 
-    <span class="c1"># TODO: add to docs and test</span>
 <div class="viewcode-block" id="PhotosDB.photos_by_uuid"><a class="viewcode-back" href="../../../reference.html#osxphotos.PhotosDB.photos_by_uuid">[docs]</a>    <span class="k">def</span> <span class="nf">photos_by_uuid</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">uuids</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns a list of photos with UUID in uuids.</span>
 <span class="sd">            Does not generate error if invalid or missing UUID passed.</span>
 <span class="sd">            This is faster than using PhotosDB.photos if you have list of UUIDs.</span>
 <span class="sd">            Returns photos regardless of intrash state.</span>
 
 <span class="sd">        Arguments:</span>
 <span class="sd">            uuid: list of UUIDs of photos to get</span>
 
 <span class="sd">        Returns:</span>
 <span class="sd">            list of PhotoInfo instance for photo with UUID matching uuid or [] if no match</span>
 <span class="sd">        &quot;&quot;&quot;</span>
-        <span class="n">photos</span> <span class="o">=</span> <span class="p">[]</span>
-        <span class="k">for</span> <span class="n">uuid</span> <span class="ow">in</span> <span class="n">uuids</span><span class="p">:</span>
-            <span class="k">try</span><span class="p">:</span>
-                <span class="n">photos</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">PhotoInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="n">uuid</span><span class="p">,</span> <span class="n">info</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">]))</span>
-            <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
-                <span class="c1"># ignore missing/invlaid UUID</span>
-                <span class="k">pass</span>
-        <span class="k">return</span> <span class="n">photos</span></div>
+        <span class="k">return</span> <span class="p">[</span>
+            <span class="n">PhotoInfo</span><span class="p">(</span><span class="n">db</span><span class="o">=</span><span class="bp">self</span><span class="p">,</span> <span class="n">uuid</span><span class="o">=</span><span class="n">uuid</span><span class="p">,</span> <span class="n">info</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">])</span>
+            <span class="k">for</span> <span class="n">uuid</span> <span class="ow">in</span> <span class="n">uuids</span>
+            <span class="k">if</span> <span class="n">uuid</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span>
+        <span class="p">]</span></div>
 
 <div class="viewcode-block" id="PhotosDB.query"><a class="viewcode-back" href="../../../reference.html#osxphotos.PhotosDB.query">[docs]</a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="n">QueryOptions</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">List</span><span class="p">[</span><span class="n">PhotoInfo</span><span class="p">]:</span>
         <span class="sd">&quot;&quot;&quot;Run a query against PhotosDB to extract the photos based on user supplied options</span>
 
 <span class="sd">        Args:</span>
 <span class="sd">            options: a QueryOptions instance</span>
 <span class="sd">        &quot;&quot;&quot;</span>
```

##### html2text {}

```diff
@@ -608,15 +608,16 @@
             return self._album_info
 
     @property
     def album_info_shared(self):
         """return list of AlbumInfo objects for each shared album in the photos
 database
         only valid for Photos 5; on Photos <= 4, prints warning and returns
-empty list"""
+empty list
+        """
         # if _dbalbum_details[key]["cloudownerhashedpersonid"] is not None,
 then it's a shared album
         try:
             return self._album_info_shared
         except AttributeError:
             self._album_info_shared = [
                 AlbumInfo(db=self, uuid=album)
@@ -638,15 +639,16 @@
             self._albums = self._get_albums(shared=False)
             return self._albums
 
     @property
     def albums_shared(self):
         """return list of shared albums found in photos database
         only valid for Photos 5; on Photos <= 4, prints warning and returns
-empty list"""
+empty list
+        """
 
         # Could be more than one album with same name
         # Right now, they are treated as same album and photos are combined
 from albums with same name
 
         # if _dbalbum_details[key]["cloudownerhashedpersonid"] is not None,
 then it's a shared album
@@ -3332,38 +3334,33 @@
         """
         try:
             return PhotoInfo(db=self, uuid=uuid, info=self._dbphotos[uuid])
         except KeyError:
             return None
 
 
-    # TODO: add to docs and test
 [docs]    def photos_by_uuid(self, uuids):
         """Returns a list of photos with UUID in uuids.
             Does not generate error if invalid or missing UUID passed.
             This is faster than using PhotosDB.photos if you have list of
 UUIDs.
             Returns photos regardless of intrash state.
 
         Arguments:
             uuid: list of UUIDs of photos to get
 
         Returns:
             list of PhotoInfo instance for photo with UUID matching uuid or []
 if no match
         """
-        photos = []
-        for uuid in uuids:
-            try:
-                photos.append(PhotoInfo(db=self, uuid=uuid, info=self._dbphotos
-[uuid]))
-            except KeyError:
-                # ignore missing/invlaid UUID
-                pass
-        return photos
+        return [
+            PhotoInfo(db=self, uuid=uuid, info=self._dbphotos[uuid])
+            for uuid in uuids
+            if uuid in self._dbphotos
+        ]
 
 
 [docs]    def query(self, options: QueryOptions) -> List[PhotoInfo]:
         """Run a query against PhotosDB to extract the photos based on user
 supplied options
 
         Args:
```

#### docs/_modules/osxphotos/albuminfo.html

```diff
@@ -243,17 +243,16 @@
 <span class="sd">    Returns:</span>
 <span class="sd">        list of values, sorted by sort_keys</span>
 
 <span class="sd">    Raises:</span>
 <span class="sd">        ValueError: raised if len(values) != len(sort_keys)</span>
 <span class="sd">    &quot;&quot;&quot;</span>
     <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">values</span><span class="p">)</span> <span class="o">!=</span> <span class="nb">len</span><span class="p">(</span><span class="n">sort_keys</span><span class="p">):</span>
-        <span class="k">return</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;values and sort_keys must have same length&quot;</span><span class="p">)</span>
-
-    <span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="nb">zip</span><span class="p">(</span><span class="o">*</span><span class="nb">sorted</span><span class="p">(</span><span class="nb">zip</span><span class="p">(</span><span class="n">sort_keys</span><span class="p">,</span> <span class="n">values</span><span class="p">))))[</span><span class="mi">1</span><span class="p">]</span>
+        <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="s2">&quot;values and sort_keys must be same length&quot;</span><span class="p">)</span>
+    <span class="k">return</span> <span class="p">[</span><span class="n">x</span> <span class="k">for</span> <span class="n">_</span><span class="p">,</span> <span class="n">x</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">zip</span><span class="p">(</span><span class="n">sort_keys</span><span class="p">,</span> <span class="n">values</span><span class="p">))]</span>
 
 
 <span class="k">class</span> <span class="nc">AlbumInfoBaseClass</span><span class="p">:</span>
     <span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Base class for AlbumInfo, ImportInfo</span>
 <span class="sd">    Info about a specific Album, contains all the details about the album</span>
 <span class="sd">    including folders, photos, etc.</span>
@@ -359,22 +358,21 @@
                     <span class="k">else</span> <span class="kc">None</span>
                 <span class="p">)</span>
             <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_owner</span> <span class="o">=</span> <span class="kc">None</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_owner</span>
 
     <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Return album info as a dict&quot;&quot;&quot;</span>
+        <span class="sd">&quot;&quot;&quot;Return album info as a dict; does not include photos&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="p">{</span>
             <span class="s2">&quot;uuid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">,</span>
             <span class="s2">&quot;creation_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">creation_date</span><span class="p">,</span>
             <span class="s2">&quot;start_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_date</span><span class="p">,</span>
             <span class="s2">&quot;end_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">end_date</span><span class="p">,</span>
             <span class="s2">&quot;owner&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">owner</span><span class="p">,</span>
-            <span class="s2">&quot;photos&quot;</span><span class="p">:</span> <span class="p">[</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">photos</span><span class="p">],</span>
         <span class="p">}</span>
 
     <span class="k">def</span> <span class="fm">__len__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;return number of photos contained in album&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">photos</span><span class="p">)</span>
 
 
@@ -492,15 +490,15 @@
             <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">uuid</span> <span class="o">==</span> <span class="n">photo</span><span class="o">.</span><span class="n">uuid</span><span class="p">:</span>
                 <span class="k">return</span> <span class="n">index</span>
         <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span>
             <span class="sa">f</span><span class="s2">&quot;Photo with uuid </span><span class="si">{</span><span class="n">photo</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2"> does not appear to be in this album&quot;</span>
         <span class="p">)</span></div>
 
 <div class="viewcode-block" id="AlbumInfo.asdict"><a class="viewcode-back" href="../../reference.html#osxphotos.AlbumInfo.asdict">[docs]</a>    <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Return album info as a dict&quot;&quot;&quot;</span>
+        <span class="sd">&quot;&quot;&quot;Return album info as a dict; does not include photos&quot;&quot;&quot;</span>
         <span class="n">dict_data</span> <span class="o">=</span> <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="n">asdict</span><span class="p">()</span>
         <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;title&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">title</span>
         <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;folder_names&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">folder_names</span>
         <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;folder_list&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">f</span><span class="o">.</span><span class="n">uuid</span> <span class="k">for</span> <span class="n">f</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">folder_list</span><span class="p">]</span>
         <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;sort_order&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sort_order</span>
         <span class="n">dict_data</span><span class="p">[</span><span class="s2">&quot;parent&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">uuid</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">parent</span> <span class="k">else</span> <span class="kc">None</span>
         <span class="k">return</span> <span class="n">dict_data</span></div></div>
@@ -555,22 +553,21 @@
                     <span class="k">for</span> <span class="n">u</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_dbphotos</span>
                     <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">u</span><span class="p">][</span><span class="s2">&quot;import_uuid&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span>
                 <span class="p">]</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_photos</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">photos_by_uuid</span><span class="p">(</span><span class="n">import_photo_uuids</span><span class="p">)</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_photos</span>
 
 <div class="viewcode-block" id="ImportInfo.asdict"><a class="viewcode-back" href="../../reference.html#osxphotos.ImportInfo.asdict">[docs]</a>    <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;Return import info as a dict&quot;&quot;&quot;</span>
+        <span class="sd">&quot;&quot;&quot;Return import info as a dict; does not include photos&quot;&quot;&quot;</span>
         <span class="k">return</span> <span class="p">{</span>
             <span class="s2">&quot;uuid&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">,</span>
             <span class="s2">&quot;creation_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">creation_date</span><span class="p">,</span>
             <span class="s2">&quot;start_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">start_date</span><span class="p">,</span>
             <span class="s2">&quot;end_date&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">end_date</span><span class="p">,</span>
             <span class="s2">&quot;title&quot;</span><span class="p">:</span> <span class="bp">self</span><span class="o">.</span><span class="n">title</span><span class="p">,</span>
-            <span class="s2">&quot;photos&quot;</span><span class="p">:</span> <span class="p">[</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">photos</span><span class="p">],</span>
         <span class="p">}</span></div>
 
     <span class="k">def</span> <span class="fm">__bool__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Always returns True</span>
 <span class="sd">        A photo without an import session will return None for import_info,</span>
 <span class="sd">        thus if import_info is not None, it must be a valid import_info object (#820)</span>
 <span class="sd">        &quot;&quot;&quot;</span>
```

##### html2text {}

```diff
@@ -86,17 +86,16 @@
     Returns:
         list of values, sorted by sort_keys
 
     Raises:
         ValueError: raised if len(values) != len(sort_keys)
     """
     if len(values) != len(sort_keys):
-        return ValueError("values and sort_keys must have same length")
-
-    return list(zip(*sorted(zip(sort_keys, values))))[1]
+        raise ValueError("values and sort_keys must be same length")
+    return [x for _, x in sorted(zip(sort_keys, values))]
 
 
 class AlbumInfoBaseClass:
     """
     Base class for AlbumInfo, ImportInfo
     Info about a specific Album, contains all the details about the album
     including folders, photos, etc.
@@ -209,22 +208,21 @@
                     else None
                 )
             except KeyError:
                 self._owner = None
             return self._owner
 
     def asdict(self):
-        """Return album info as a dict"""
+        """Return album info as a dict; does not include photos"""
         return {
             "uuid": self.uuid,
             "creation_date": self.creation_date,
             "start_date": self.start_date,
             "end_date": self.end_date,
             "owner": self.owner,
-            "photos": [p.uuid for p in self.photos],
         }
 
     def __len__(self):
         """return number of photos contained in album"""
         return len(self.photos)
 
 
@@ -353,15 +351,15 @@
                 return index
         raise ValueError(
             f"Photo with uuid {photo.uuid} does not appear to be in this album"
         )
 
 
 [docs]    def asdict(self):
-        """Return album info as a dict"""
+        """Return album info as a dict; does not include photos"""
         dict_data = super().asdict()
         dict_data["title"] = self.title
         dict_data["folder_names"] = self.folder_names
         dict_data["folder_list"] = [f.uuid for f in self.folder_list]
         dict_data["sort_order"] = self.sort_order
         dict_data["parent"] = self.parent.uuid if self.parent else None
         return dict_data
@@ -417,22 +415,21 @@
                     for u in self._db._dbphotos
                     if self._db._dbphotos[u]["import_uuid"] == self.uuid
                 ]
                 self._photos = self._db.photos_by_uuid(import_photo_uuids)
             return self._photos
 
 [docs]    def asdict(self):
-        """Return import info as a dict"""
+        """Return import info as a dict; does not include photos"""
         return {
             "uuid": self.uuid,
             "creation_date": self.creation_date,
             "start_date": self.start_date,
             "end_date": self.end_date,
             "title": self.title,
-            "photos": [p.uuid for p in self.photos],
         }
 
 
     def __bool__(self):
         """Always returns True
         A photo without an import session will return None for import_info,
         thus if import_info is not None, it must be a valid import_info object
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.59.2'
+     - The osxphotos version, e.g. '0.59.3'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.59.2',
+    VERSION: '0.59.3',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.59.2 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.59.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.59.2 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.59.3 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.59.2 documentation</title>
+        <title>osxphotos 0.59.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.59.2 documentation</title>
+        <title>OSXPhotos - osxphotos 0.59.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.59.2 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.59.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.59.2 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.59.3 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.59.2 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.59.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -203,15 +203,15 @@
 <dt class="sig sig-object py" id="osxphotos.AlbumInfo">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">AlbumInfo</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/albuminfo.html#AlbumInfo"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.AlbumInfo" title="Permalink to this definition">#</a></dt>
 <dd><p>Info about a specific Album, contains all the details about the album
 including folders, photos, etc.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.AlbumInfo.asdict">
 <span class="sig-name descname"><span class="pre">asdict</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/albuminfo.html#AlbumInfo.asdict"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.AlbumInfo.asdict" title="Permalink to this definition">#</a></dt>
-<dd><p>Return album info as a dict</p>
+<dd><p>Return album info as a dict; does not include photos</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.AlbumInfo.folder_list">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">folder_list</span></span><a class="headerlink" href="#osxphotos.AlbumInfo.folder_list" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns list of FolderInfo objects for each folder the album is contained in
 or empty list if album is not in any folders</p>
@@ -1229,15 +1229,15 @@
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.ImportInfo">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ImportInfo</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/albuminfo.html#ImportInfo"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ImportInfo" title="Permalink to this definition">#</a></dt>
 <dd><p>Information about import sessions</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.ImportInfo.asdict">
 <span class="sig-name descname"><span class="pre">asdict</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/albuminfo.html#ImportInfo.asdict"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ImportInfo.asdict" title="Permalink to this definition">#</a></dt>
-<dd><p>Return import info as a dict</p>
+<dd><p>Return import info as a dict; does not include photos</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.ImportInfo.photos">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">photos</span></span><a class="headerlink" href="#osxphotos.ImportInfo.photos" title="Permalink to this definition">#</a></dt>
 <dd><p>return list of photos contained in import session</p>
 </dd></dl>
@@ -1486,16 +1486,28 @@
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.albums">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">albums</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.albums" title="Permalink to this definition">#</a></dt>
 <dd><p>list of albums picture is contained in</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.asdict">
-<span class="sig-name descname"><span class="pre">asdict</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.asdict"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.asdict" title="Permalink to this definition">#</a></dt>
-<dd><p>return dict representation</p>
+<span class="sig-name descname"><span class="pre">asdict</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">shallow</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">dict</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.asdict"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.asdict" title="Permalink to this definition">#</a></dt>
+<dd><p>Return dict representation of PhotoInfo object.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><p><strong>shallow</strong> – if True, return shallow representation (does not contain folder_info, person_info, etc.)</p>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>dict representation of PhotoInfo object</p>
+</dd>
+</dl>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>The shallow representation is used internally by export as it contains only the subset of data needed for export.</p>
+</div>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.burst">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">burst</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.burst" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns True if photo is part of a Burst photo set, otherwise False</p>
 </dd></dl>
@@ -1810,27 +1822,31 @@
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.isreference">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">isreference</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.isreference" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns True if photo is a reference (not copied to the Photos library), otherwise False</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.json">
-<span class="sig-name descname"><span class="pre">json</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">indent</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shallow</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.json"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.json" title="Permalink to this definition">#</a></dt>
+<span class="sig-name descname"><span class="pre">json</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">indent</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">int</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shallow</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">str</span></span></span><a class="reference internal" href="_modules/osxphotos/photoinfo.html#PhotoInfo.json"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.PhotoInfo.json" title="Permalink to this definition">#</a></dt>
 <dd><p>Return JSON representation</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>indent</strong> – indent level for JSON, if None, no indent</p></li>
 <li><p><strong>shallow</strong> – if True, return shallow JSON representation (does not contain folder_info, person_info, etc.)</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>JSON string</p>
 </dd>
 </dl>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>The shallow representation is used internally by export as it contains only the subset of data needed for export.</p>
+</div>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.keywords">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">keywords</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.keywords" title="Permalink to this definition">#</a></dt>
 <dd><p>list of keywords for picture</p>
 </dd></dl>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -39,15 +39,15 @@
 
 ****** OSXPhotos Python Reference# ******
 __init__.py for osxphotos
   classosxphotos.AlbumInfo(db, uuid)[source]#
       Info about a specific Album, contains all the details about the album
       including folders, photos, etc.
         asdict()[source]#
-            Return album info as a dict
+            Return album info as a dict; does not include photos
         propertyfolder_list#
             Returns list of FolderInfo objects for each folder the album is
             contained in or empty list if album is not in any folders
         propertyfolder_names#
             Return hierarchical list of folders the album is contained in the
             folder list is in form: [âTop level folderâ, âsub folder
             1â, âsub folder 2â, â¦] or empty list if album is not in any
@@ -533,15 +533,15 @@
         propertytitle#
             return title / name of folder
         propertyuuid#
             return uuid of folder
   classosxphotos.ImportInfo(db, uuid)[source]#
       Information about import sessions
         asdict()[source]#
-            Return import info as a dict
+            Return import info as a dict; does not include photos
         propertyphotos#
             return list of photos contained in import session
         propertytitle#
             return title / name of import session
   classosxphotos.LikeInfo(datetime: datetime, user: str, ismine: bool)[source]#
       Class for shared photo likes
   classosxphotos.MomentInfo(db, moment_pk)[source]#
@@ -660,16 +660,24 @@
             Returns AdjustmentsInfo class for adjustment data or None if no
             adjustments; Photos 5+ only
         propertyalbum_info#
             list of AlbumInfo objects representing albums the photo is
             contained in
         propertyalbums#
             list of albums picture is contained in
-        asdict()[source]#
-            return dict representation
+        asdict(shallow: bool = True) &#x2192; dict[str, Any][source]#
+            Return dict representation of PhotoInfo object.
+              Parameters:
+                  shallow â if True, return shallow representation (does not
+                  contain folder_info, person_info, etc.)
+              Returns:
+                  dict representation of PhotoInfo object
+            Note
+            The shallow representation is used internally by export as it
+            contains only the subset of data needed for export.
         propertyburst#
             Returns True if photo is part of a Burst photo set, otherwise False
         propertyburst_album_info#
             If photo is a burst photo, returns list of AlbumInfo objects
             representing albums the photo is contained in as well as albums the
             burst key photo is contained in, otherwise returns self.album_info.
         propertyburst_albums#
@@ -868,23 +876,26 @@
             Returns True if file is an image, otherwise False
         propertyisraw#
             returns True if photo is a raw image. For images with an associated
             RAW+JPEG pair, see has_raw
         propertyisreference#
             Returns True if photo is a reference (not copied to the Photos
             library), otherwise False
-        json(indent: int | None = None, shallow: bool = False) &#x2192; str
+        json(indent: int | None = None, shallow: bool = True) &#x2192; str
         [source]#
             Return JSON representation
               Parameters:
                       * indent â indent level for JSON, if None, no indent
                       * shallow â if True, return shallow JSON representation
                         (does not contain folder_info, person_info, etc.)
               Returns:
                   JSON string
+            Note
+            The shallow representation is used internally by export as it
+            contains only the subset of data needed for export.
         propertykeywords#
             list of keywords for picture
         propertylabels#
             returns list of labels applied to photo by Photos image
             categorization only valid on Photos 5, on older libraries returns
             empty list
         propertylabels_normalized#
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.59.2 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.59.3 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -50,15 +50,15 @@
         "": [0, 2, 4, 5, 6],
         "compar": [0, 2, 4],
         "two": [0, 2, 6],
         "differ": [0, 2, 4, 6],
         "To": [0, 2, 4, 5, 6],
         "you": [0, 2, 3, 4, 5, 6],
         "ll": [0, 6],
-        "need": [0, 3, 5, 6],
+        "need": [0, 3, 4, 5, 6],
         "sqldiff": 0,
         "via": [0, 4, 6],
         "homebrew": [0, 2],
         "http": [0, 2, 4, 5, 6],
         "brew": [0, 2],
         "sh": [0, 2],
         "alreadi": [0, 4, 6],
@@ -1564,15 +1564,15 @@
         "dc": 5,
         "20009": 5,
         "postal_cod": 5,
         "summer": [5, 6],
         "algorithm": [5, 6],
         "iphon": [0, 5, 6],
         "15mm": 5,
-        "intern": [5, 6],
+        "intern": [4, 5, 6],
         "univers": 5,
         "128fb4c6": 5,
         "0b16": 5,
         "4e7d": 5,
         "9108": 5,
         "fb2e90da1546": 5,
         "shortuuid": 5,
@@ -1740,15 +1740,15 @@
         "excel": 6,
         "And": 6,
         "cover": 6,
         "50": 6,
         "better": 6,
         "understand": 6,
         "matter": 6,
-        "subset": [0, 6],
+        "subset": [0, 4, 6],
         "certainli": 6,
         "insid": 6,
         "2018": 6,
         "28": 6,
         "worst": 6,
         "9": 6,
         "describ": [0, 6],
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.59.2 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.59.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.59.2’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.59.3’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.59.2â
+{osxphotos_version}            The osxphotos version, e.g. â0.59.3â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.59.2 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.59.3 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.59.2 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.59.3 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.59.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.59.3 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.59.2_documentation
+osxphotos_0.59.3_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.59.2/osxphotos/exif_datetime_updater.py` & `osxphotos-0.59.3/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/exifinfo.py` & `osxphotos-0.59.3/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/exiftool.py` & `osxphotos-0.59.3/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/exiftool_filetypes.json` & `osxphotos-0.59.3/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/export_db.py` & `osxphotos-0.59.3/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/export_db_utils.py` & `osxphotos-0.59.3/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/fileutil.py` & `osxphotos-0.59.3/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/frozen_photoinfo.py` & `osxphotos-0.59.3/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/imageconverter.py` & `osxphotos-0.59.3/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/momentinfo.py` & `osxphotos-0.59.3/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/path_utils.py` & `osxphotos-0.59.3/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/personinfo.py` & `osxphotos-0.59.3/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photodates.py` & `osxphotos-0.59.3/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photoexporter.py` & `osxphotos-0.59.3/osxphotos/photoexporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1517,18 +1517,18 @@
         # else, need to check the database to determine if we need to write
         verbose(
             f"Writing metadata with exiftool for {self._filepath(pathlib.Path(dest).name)}"
         )
         if not options.dry_run:
             warning_, error_ = self._write_exif_data(src, options=options)
             if warning_:
-                exiftool_results.exiftool_warning.append((dest, warning_))
+                exiftool_results.exiftool_warning.append((str(dest), str(warning_)))
             if error_:
-                exiftool_results.exiftool_error.append((dest, error_))
-                exiftool_results.error.append((dest, error_))
+                exiftool_results.exiftool_error.append((str(dest), str(error_)))
+                exiftool_results.error.append((str(dest), str(error_)))
 
         exiftool_results.exif_updated.append(dest)
         exiftool_results.to_touch.append(dest)
         return exiftool_results
 
     def _should_run_exiftool(self, dest, options: ExportOptions) -> bool:
         """Return True if exiftool should be run to update metadata"""
```

### Comparing `osxphotos-0.59.2/osxphotos/photoinfo.py` & `osxphotos-0.59.3/osxphotos/photoinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -513,47 +513,34 @@
     def persons(self):
         """list of persons in picture"""
         return [self._db._dbpersons_pk[pk]["fullname"] for pk in self._info["persons"]]
 
     @property
     def person_info(self):
         """list of PersonInfo objects for person in picture"""
-        try:
-            return self._personinfo
-        except AttributeError:
-            self._personinfo = [
-                PersonInfo(db=self._db, pk=pk) for pk in self._info["persons"]
-            ]
-            return self._personinfo
+        return [PersonInfo(db=self._db, pk=pk) for pk in self._info["persons"]]
 
     @property
     def face_info(self):
         """list of FaceInfo objects for faces in picture"""
         try:
-            return self._faceinfo
-        except AttributeError:
-            try:
-                faces = self._db._db_faceinfo_uuid[self._uuid]
-                self._faceinfo = [FaceInfo(db=self._db, pk=pk) for pk in faces]
-            except KeyError:
-                # no faces
-                self._faceinfo = []
-            return self._faceinfo
+            faces = self._db._db_faceinfo_uuid[self._uuid]
+            self._faceinfo = [FaceInfo(db=self._db, pk=pk) for pk in faces]
+        except KeyError:
+            # no faces
+            self._faceinfo = []
+        return self._faceinfo
 
     @property
     def moment_info(self):
         """Moment photo belongs to"""
         try:
-            return self._moment
-        except AttributeError:
-            try:
-                self._moment = MomentInfo(db=self._db, moment_pk=self._info["momentID"])
-            except ValueError:
-                self._moment = None
-            return self._moment
+            return MomentInfo(db=self._db, moment_pk=self._info["momentID"])
+        except ValueError:
+            return None
 
     @property
     def albums(self):
         """list of albums picture is contained in"""
         try:
             return self._albums
         except AttributeError:
@@ -562,88 +549,63 @@
                 {self._db._dbalbum_details[album]["title"] for album in album_uuids}
             )
             return self._albums
 
     @property
     def burst_albums(self):
         """If photo is burst photo, list of albums it is contained in as well as any albums the key photo is contained in, otherwise returns self.albums"""
-        try:
-            return self._burst_albums
-        except AttributeError:
-            burst_albums = list(self.albums)
-            for photo in self.burst_photos:
-                if photo.burst_key:
-                    burst_albums.extend(photo.albums)
-            self._burst_albums = list(set(burst_albums))
-            return self._burst_albums
+        burst_albums = list(self.albums)
+        for photo in self.burst_photos:
+            if photo.burst_key:
+                burst_albums.extend(photo.albums)
+        return list(set(burst_albums))
 
     @property
     def album_info(self):
         """list of AlbumInfo objects representing albums the photo is contained in"""
-        try:
-            return self._album_info
-        except AttributeError:
-            album_uuids = self._get_album_uuids()
-            self._album_info = [
-                AlbumInfo(db=self._db, uuid=album) for album in album_uuids
-            ]
-            return self._album_info
+        album_uuids = self._get_album_uuids()
+        return [AlbumInfo(db=self._db, uuid=album) for album in album_uuids]
 
     @property
     def burst_album_info(self):
         """If photo is a burst photo, returns list of AlbumInfo objects representing albums the photo is contained in as well as albums the burst key photo is contained in, otherwise returns self.album_info."""
-        try:
-            return self._burst_album_info
-        except AttributeError:
-            burst_album_info = list(self.album_info)
-            for photo in self.burst_photos:
-                if photo.burst_key:
-                    burst_album_info.extend(photo.album_info)
-            self._burst_album_info = list(set(burst_album_info))
-            return self._burst_album_info
+        burst_album_info = list(self.album_info)
+        for photo in self.burst_photos:
+            if photo.burst_key:
+                burst_album_info.extend(photo.album_info)
+        return list(set(burst_album_info))
 
     @property
     def import_info(self):
         """ImportInfo object representing import session for the photo or None if no import session"""
-        try:
-            return self._import_info
-        except AttributeError:
-            self._import_info = (
-                ImportInfo(db=self._db, uuid=self._info["import_uuid"])
-                if self._info["import_uuid"] is not None
-                else None
-            )
-            return self._import_info
+        return (
+            ImportInfo(db=self._db, uuid=self._info["import_uuid"])
+            if self._info["import_uuid"] is not None
+            else None
+        )
 
     @property
     def project_info(self):
         """list of AlbumInfo objects representing projects for the photo or None if no projects"""
-        try:
-            return self._project_info
-        except AttributeError:
-            project_uuids = self._get_album_uuids(project=True)
-            self._project_info = [
-                ProjectInfo(db=self._db, uuid=album) for album in project_uuids
-            ]
-            return self._project_info
+        project_uuids = self._get_album_uuids(project=True)
+        return [ProjectInfo(db=self._db, uuid=album) for album in project_uuids]
 
     @property
     def keywords(self):
         """list of keywords for picture"""
         return self._info["keywords"]
 
     @property
     def title(self):
         """name / title of picture"""
         # if user sets then deletes title, Photos sets it to empty string in DB instead of NULL
         # in this case, return None so result is the same as if title had never been set (which returns NULL)
         # issue #512
         title = self._info["name"]
-        title = None if title == "" else title
-        return title
+        return None if title == "" else title
 
     @property
     def uuid(self):
         """UUID of picture"""
         return self._uuid
 
     @property
@@ -1773,49 +1735,39 @@
             "original_height": self.original_height,
             "original_width": self.original_width,
             "original_orientation": self.original_orientation,
             "original_filesize": self.original_filesize,
         }
         return yaml.dump(info, sort_keys=False)
 
-    def asdict(self):
-        """return dict representation"""
+    def asdict(self, shallow: bool = True) -> dict[str, Any]:
+        """Return dict representation of PhotoInfo object.
+
+        Args:
+            shallow: if True, return shallow representation (does not contain folder_info, person_info, etc.)
+
+        Returns:
+            dict representation of PhotoInfo object
+
+        Note:
+            The shallow representation is used internally by export as it contains only the subset of data needed for export.
+        """
 
-        adjustments = self.adjustments.asdict() if self.adjustments else {}
-        album_info = [album.asdict() for album in self.album_info]
-        burst_album_info = [a.asdict() for a in self.burst_album_info]
-        burst_photos = [p.uuid for p in self.burst_photos]
         comments = [comment.asdict() for comment in self.comments]
         exif_info = dataclasses.asdict(self.exif_info) if self.exif_info else {}
         face_info = [face.asdict() for face in self.face_info]
         folders = {album.title: album.folder_names for album in self.album_info}
-        import_info = self.import_info.asdict() if self.import_info else {}
         likes = [like.asdict() for like in self.likes]
-        person_info = [p.asdict() for p in self.person_info]
         place = self.place.asdict() if self.place else {}
-        project_info = [p.asdict() for p in self.project_info]
         score = dataclasses.asdict(self.score) if self.score else {}
-        search_info = self.search_info.asdict() if self.search_info else {}
-        search_info_normalized = (
-            self.search_info_normalized.asdict() if self.search_info_normalized else {}
-        )
 
-        return {
-            "adjustments": adjustments,
-            "album_info": album_info,
+        dict_data = {
             "albums": self.albums,
-            "burst_album_info": burst_album_info,
-            "burst_albums": self.burst_albums,
-            "burst_default_pick": self.burst_default_pick,
-            "burst_key": self.burst_key,
-            "burst_photos": burst_photos,
-            "burst_selected": self.burst_selected,
             "burst": self.burst,
             "cloud_guid": self.cloud_guid,
-            "cloud_metadata": self.cloud_metadata,
             "cloud_owner_hashed_id": self.cloud_owner_hashed_id,
             "comments": comments,
             "date_added": self.date_added,
             "date_modified": self.date_modified,
             "date_trashed": self.date_trashed,
             "date": self.date,
             "description": self.description,
@@ -1827,25 +1779,23 @@
             "fingerprint": self.fingerprint,
             "folders": folders,
             "has_raw": self.has_raw,
             "hasadjustments": self.hasadjustments,
             "hdr": self.hdr,
             "height": self.height,
             "hidden": self.hidden,
-            "import_info": import_info,
             "incloud": self.incloud,
             "intrash": self.intrash,
             "iscloudasset": self.iscloudasset,
             "ismissing": self.ismissing,
             "ismovie": self.ismovie,
             "isphoto": self.isphoto,
             "israw": self.israw,
             "isreference": self.isreference,
             "keywords": self.keywords,
-            "labels_normalized": self.labels_normalized,
             "labels": self.labels,
             "latitude": self._latitude,
             "library": self._db._library_path,
             "likes": likes,
             "live_photo": self.live_photo,
             "location": self.location,
             "longitude": self._longitude,
@@ -1853,30 +1803,25 @@
             "original_filename": self.original_filename,
             "original_filesize": self.original_filesize,
             "original_height": self.original_height,
             "original_orientation": self.original_orientation,
             "original_width": self.original_width,
             "owner": self.owner,
             "panorama": self.panorama,
-            "path_derivatives": self.path_derivatives,
             "path_edited_live_photo": self.path_edited_live_photo,
             "path_edited": self.path_edited,
             "path_live_photo": self.path_live_photo,
             "path_raw": self.path_raw,
             "path": self.path,
-            "person_info": person_info,
             "persons": self.persons,
             "place": place,
             "portrait": self.portrait,
-            "project_info": project_info,
             "raw_original": self.raw_original,
             "score": score,
             "screenshot": self.screenshot,
-            "search_info_normalized": search_info_normalized,
-            "search_info": search_info,
             "selfie": self.selfie,
             "shared": self.shared,
             "slow_mo": self.slow_mo,
             "time_lapse": self.time_lapse,
             "title": self.title,
             "tzoffset": self.tzoffset,
             "uti_edited": self.uti_edited,
@@ -1884,53 +1829,64 @@
             "uti_raw": self.uti_raw,
             "uti": self.uti,
             "uuid": self.uuid,
             "visible": self.visible,
             "width": self.width,
         }
 
-    def json(self, indent: int | None = None, shallow: bool = False) -> str:
+        # non-shallow keys
+        if not shallow:
+            dict_data["album_info"] = [album.asdict() for album in self.album_info]
+            dict_data["path_derivatives"] = self.path_derivatives
+            dict_data["adjustments"] = (
+                self.adjustments.asdict() if self.adjustments else {}
+            )
+            dict_data["burst_album_info"] = [a.asdict() for a in self.burst_album_info]
+            dict_data["burst_albums"] = self.burst_albums
+            dict_data["burst_default_pick"] = self.burst_default_pick
+            dict_data["burst_key"] = self.burst_key
+            dict_data["burst_photos"] = [p.uuid for p in self.burst_photos]
+            dict_data["burst_selected"] = self.burst_selected
+            dict_data["cloud_metadata"] = self.cloud_metadata
+            dict_data["import_info"] = (
+                self.import_info.asdict() if self.import_info else {}
+            )
+            dict_data["labels_normalized"] = self.labels_normalized
+            dict_data["person_info"] = [p.asdict() for p in self.person_info]
+            dict_data["project_info"] = [p.asdict() for p in self.project_info]
+            dict_data["search_info"] = (
+                self.search_info.asdict() if self.search_info else {}
+            )
+            dict_data["search_info_normalized"] = (
+                self.search_info_normalized.asdict()
+                if self.search_info_normalized
+                else {}
+            )
+
+        return dict_data
+
+    def json(self, indent: int | None = None, shallow: bool = True) -> str:
         """Return JSON representation
 
         Args:
             indent: indent level for JSON, if None, no indent
             shallow: if True, return shallow JSON representation (does not contain folder_info, person_info, etc.)
 
         Returns:
             JSON string
+
+        Note:
+            The shallow representation is used internally by export as it contains only the subset of data needed for export.
         """
 
         def default(o):
             if isinstance(o, (datetime.date, datetime.datetime)):
                 return o.isoformat()
 
-        dict_data = self.asdict()
-
-        if shallow:
-            # delete items that are not needed for shallow JSON
-            # these are removed to match behavior of osxphotos < 0.59.0 (See #999, #1039)
-            for key in [
-                "adjustments",
-                "album_info",
-                "burst_album_info",
-                "burst_albums",
-                "burst_default_pick",
-                "burst_key",
-                "burst_photos",
-                "burst_selected",
-                "cloud_metadata",
-                "import_info",
-                "labels_normalized",
-                "path_derivatives",
-                "person_info",
-                "project_info",
-                "search_info_normalized",
-                "search_info",
-            ]:
-                del dict_data[key]
+        dict_data = self.asdict(shallow=True) if shallow else self.asdict(shallow=False)
 
         for k, v in dict_data.items():
             # sort lists such as keywords so JSON is consistent
             # but do not sort certain items like location
             if k in ["location"]:
                 continue
             if v and isinstance(v, (list, tuple)) and not isinstance(v[0], dict):
@@ -1945,23 +1901,17 @@
         # for computing hexdigest so we can ignore them
         # also don't use visible because it changes based on Photos UI state
 
         def default(o):
             if isinstance(o, (datetime.date, datetime.datetime)):
                 return o.isoformat()
 
-        dict_data = self.asdict()
+        dict_data = self.asdict(shallow=True)
 
-        for k in [
-            "album_info",
-            "burst_album_info",
-            "face_info",
-            "person_info",
-            "visible",
-        ]:
+        for k in ["face_info", "visible"]:
             del dict_data[k]
 
         for k, v in dict_data.items():
             # sort lists such as keywords so JSON is consistent
             # but do not sort certain items like location
             if k in ["location"]:
                 continue
```

### Comparing `osxphotos-0.59.2/osxphotos/photokit.py` & `osxphotos-0.59.3/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photosalbum.py` & `osxphotos-0.59.3/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photoscript_utils.py` & `osxphotos-0.59.3/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.59.3/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/photosdb/photosdb.py` & `osxphotos-0.59.3/osxphotos/photosdb/photosdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,16 @@
                 for album in self._get_album_uuids(shared=False)
             ]
             return self._album_info
 
     @property
     def album_info_shared(self):
         """return list of AlbumInfo objects for each shared album in the photos database
-        only valid for Photos 5; on Photos <= 4, prints warning and returns empty list"""
+        only valid for Photos 5; on Photos <= 4, prints warning and returns empty list
+        """
         # if _dbalbum_details[key]["cloudownerhashedpersonid"] is not None, then it's a shared album
         try:
             return self._album_info_shared
         except AttributeError:
             self._album_info_shared = [
                 AlbumInfo(db=self, uuid=album)
                 for album in self._get_album_uuids(shared=True)
@@ -539,15 +540,16 @@
         except AttributeError:
             self._albums = self._get_albums(shared=False)
             return self._albums
 
     @property
     def albums_shared(self):
         """return list of shared albums found in photos database
-        only valid for Photos 5; on Photos <= 4, prints warning and returns empty list"""
+        only valid for Photos 5; on Photos <= 4, prints warning and returns empty list
+        """
 
         # Could be more than one album with same name
         # Right now, they are treated as same album and photos are combined from albums with same name
 
         # if _dbalbum_details[key]["cloudownerhashedpersonid"] is not None, then it's a shared album
 
         try:
@@ -3049,35 +3051,31 @@
             PhotoInfo instance for photo with UUID matching uuid or None if no match
         """
         try:
             return PhotoInfo(db=self, uuid=uuid, info=self._dbphotos[uuid])
         except KeyError:
             return None
 
-    # TODO: add to docs and test
     def photos_by_uuid(self, uuids):
         """Returns a list of photos with UUID in uuids.
             Does not generate error if invalid or missing UUID passed.
             This is faster than using PhotosDB.photos if you have list of UUIDs.
             Returns photos regardless of intrash state.
 
         Arguments:
             uuid: list of UUIDs of photos to get
 
         Returns:
             list of PhotoInfo instance for photo with UUID matching uuid or [] if no match
         """
-        photos = []
-        for uuid in uuids:
-            try:
-                photos.append(PhotoInfo(db=self, uuid=uuid, info=self._dbphotos[uuid]))
-            except KeyError:
-                # ignore missing/invlaid UUID
-                pass
-        return photos
+        return [
+            PhotoInfo(db=self, uuid=uuid, info=self._dbphotos[uuid])
+            for uuid in uuids
+            if uuid in self._dbphotos
+        ]
 
     def query(self, options: QueryOptions) -> List[PhotoInfo]:
         """Run a query against PhotosDB to extract the photos based on user supplied options
 
         Args:
             options: a QueryOptions instance
         """
```

### Comparing `osxphotos-0.59.2/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.59.3/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/phototemplate.cog.md` & `osxphotos-0.59.3/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/phototemplate.md` & `osxphotos-0.59.3/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/phototemplate.py` & `osxphotos-0.59.3/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/phototemplate.tx` & `osxphotos-0.59.3/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/phototz.py` & `osxphotos-0.59.3/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/placeinfo.py` & `osxphotos-0.59.3/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/pyrepl.py` & `osxphotos-0.59.3/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.59.3/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/query_builder.py` & `osxphotos-0.59.3/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/queryoptions.py` & `osxphotos-0.59.3/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/scoreinfo.py` & `osxphotos-0.59.3/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/searchinfo.py` & `osxphotos-0.59.3/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/sqlgrep.py` & `osxphotos-0.59.3/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/sqlite_utils.py` & `osxphotos-0.59.3/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/sqlitekvstore.py` & `osxphotos-0.59.3/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/template_counter.py` & `osxphotos-0.59.3/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.59.3/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.59.3/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/text_detection.py` & `osxphotos-0.59.3/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/timeutils.py` & `osxphotos-0.59.3/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/timezones.py` & `osxphotos-0.59.3/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/tutorial.md` & `osxphotos-0.59.3/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/uti.py` & `osxphotos-0.59.3/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos/utils.py` & `osxphotos-0.59.3/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.59.3/osxphotos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.59.2
+Version: 0.59.3
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.59.2/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.59.3/osxphotos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/osxphotos.egg-info/requires.txt` & `osxphotos-0.59.3/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/setup.py` & `osxphotos-0.59.3/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_10_12_6.py` & `osxphotos-0.59.3/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.59.3/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.59.3/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.59.3/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.59.3/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_catalina_10_15_7.py` & `osxphotos-0.59.3/tests/test_catalina_10_15_7.py`

 * *Files 0% similar despite different names*

```diff
@@ -1493,15 +1493,15 @@
     photo_dict = json.loads(photo.json())
     assert photo_dict["favorite"]
 
 
 def test_json_indent(photosdb: osxphotos.PhotosDB):
     """Test PhotoInfo.json() with indent"""
     photo = photosdb.get_photo(UUID_DICT["favorite"])
-    photo_dict = json.loads(photo.json(indent=4))
+    photo_dict = json.loads(photo.json(indent=4, shallow=False))
     assert photo_dict["favorite"]
     assert "album_info" in photo_dict
 
 
 def test_json_shallow(photosdb: osxphotos.PhotosDB):
     """Test PhotoInfo.json() with shallow=True"""
     photo = photosdb.get_photo(UUID_DICT["favorite"])
```

### Comparing `osxphotos-0.59.2/tests/test_cli.py` & `osxphotos-0.59.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_add_locations.py` & `osxphotos-0.59.3/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_add_to_album.py` & `osxphotos-0.59.3/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_all_commands.py` & `osxphotos-0.59.3/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_batch_edit.py` & `osxphotos-0.59.3/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_dump.py` & `osxphotos-0.59.3/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_exiftool.py` & `osxphotos-0.59.3/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_export_cloud.py` & `osxphotos-0.59.3/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_export_projects.py` & `osxphotos-0.59.3/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_exportdb.py` & `osxphotos-0.59.3/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_import.py` & `osxphotos-0.59.3/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_orphans.py` & `osxphotos-0.59.3/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_param_types.py` & `osxphotos-0.59.3/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_sync.py` & `osxphotos-0.59.3/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_timewarp.py` & `osxphotos-0.59.3/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_utils.py` & `osxphotos-0.59.3/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cli_verbose.py` & `osxphotos-0.59.3/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_cloud_owner_catalina.py` & `osxphotos-0.59.3/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_comments.py` & `osxphotos-0.59.3/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_concurrent_export.py` & `osxphotos-0.59.3/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_configoptions.py` & `osxphotos-0.59.3/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_datetime_formatter.py` & `osxphotos-0.59.3/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_datetime_utils.py` & `osxphotos-0.59.3/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_debug.py` & `osxphotos-0.59.3/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_empty_library_4_0.py` & `osxphotos-0.59.3/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_exif_info.py` & `osxphotos-0.59.3/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_exiftool.py` & `osxphotos-0.59.3/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_exiftool_caching.py` & `osxphotos-0.59.3/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.59.3/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.59.3/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.59.3/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_export_db.py` & `osxphotos-0.59.3/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.59.3/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.59.3/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_exportresults.py` & `osxphotos-0.59.3/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_faceinfo.py` & `osxphotos-0.59.3/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_fileutil.py` & `osxphotos-0.59.3/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_highsierra.py` & `osxphotos-0.59.3/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_image_converter.py` & `osxphotos-0.59.3/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.59.3/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.59.3/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.59.3/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.59.3/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.59.3/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.59.3/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.59.3/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_mojave_10_14_6.py` & `osxphotos-0.59.3/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.59.3/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_monterey_12_0_1.py` & `osxphotos-0.59.3/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.59.3/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_movies_4_0.py` & `osxphotos-0.59.3/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_movies_5_0.py` & `osxphotos-0.59.3/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_path_utils.py` & `osxphotos-0.59.3/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_personinfo.py` & `osxphotos-0.59.3/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_photokit.py` & `osxphotos-0.59.3/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_photosdb_utils.py` & `osxphotos-0.59.3/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_placeinfo.py` & `osxphotos-0.59.3/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.59.3/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.59.3/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.59.3/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_projects_catalina.py` & `osxphotos-0.59.3/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_projects_sierra.py` & `osxphotos-0.59.3/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_score_info.py` & `osxphotos-0.59.3/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_search_info_10_14_6.py` & `osxphotos-0.59.3/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_search_info_10_15_4.py` & `osxphotos-0.59.3/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_search_info_10_15_5.py` & `osxphotos-0.59.3/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_search_info_10_15_7.py` & `osxphotos-0.59.3/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.59.3/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.59.3/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_sidecar_xmp.py` & `osxphotos-0.59.3/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.59.3/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.59.3/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.59.3/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_specials_sierra_10_12.py` & `osxphotos-0.59.3/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_sqlitekvstore.py` & `osxphotos-0.59.3/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_template.py` & `osxphotos-0.59.3/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_template_counter.py` & `osxphotos-0.59.3/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_template_today.py` & `osxphotos-0.59.3/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_uti.py` & `osxphotos-0.59.3/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_utils.py` & `osxphotos-0.59.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.59.2/tests/test_ventura_13_0_0.py` & `osxphotos-0.59.3/tests/test_ventura_13_0_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -1281,18 +1281,26 @@
     photo_dict = json.loads(photo.json())
     assert photo_dict["favorite"]
 
 
 def test_json_indent(photosdb: osxphotos.PhotosDB):
     """Test PhotoInfo.json() with indent"""
     photo = photosdb.get_photo(UUID_DICT["favorite"])
-    photo_dict = json.loads(photo.json(indent=4))
+    photo_dict = json.loads(photo.json(indent=4, shallow=False))
     assert photo_dict["favorite"]
     assert "album_info" in photo_dict
 
 
 def test_json_shallow(photosdb: osxphotos.PhotosDB):
     """Test PhotoInfo.json() with shallow=True"""
     photo = photosdb.get_photo(UUID_DICT["favorite"])
     photo_dict = json.loads(photo.json(shallow=True))
     assert photo_dict["favorite"]
     assert "album_info" not in photo_dict
+
+
+def test_photosdb_photos_by_uuid(photosdb: osxphotos.PhotosDB):
+    """Test PhotosDB.photos_by_uuid"""
+    photos = photosdb.photos_by_uuid(UUID_DICT.values())
+    assert len(photos) == len(UUID_DICT)
+    for photo in photos:
+        assert photo.uuid in UUID_DICT.values()
```

### Comparing `osxphotos-0.59.2/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.59.3/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

