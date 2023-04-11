# Comparing `tmp/lpminimk3-0.5.0.tar.gz` & `tmp/lpminimk3-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpminimk3-0.5.0.tar", last modified: Thu May 19 09:13:51 2022, max compression
+gzip compressed data, was "lpminimk3-0.5.1.tar", last modified: Tue Apr 11 00:43:11 2023, max compression
```

## Comparing `lpminimk3-0.5.0.tar` & `lpminimk3-0.5.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7663 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7196 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.039646 lpminimk3-0.5.0/lpminimk3/
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/_core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36820 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/_core/components.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/_core/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    18931 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/_core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9386 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/_lpminimk3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/colors/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13807 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/colors/_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/examples/display_character.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/examples/flash.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/examples/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/examples/light_on_push.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/examples/party.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/examples/print_text_scroll.py
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/examples/text_scroll_region.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/graphics/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12045 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/_graphics.py
--rw-r--r--   0 runner    (1001) docker     (121)     8111 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    29194 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/_renderable.py
--rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5766 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/graphics/art/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/art/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/art/_art.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/graphics/bitmaps/
--rw-r--r--   0 runner    (1001) docker     (121)    11305 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/bitmaps/smiley.bitmap.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/graphics/glyphs/
--rw-r--r--   0 runner    (1001) docker     (121)     6553 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/glyphs/basic_latin.glyph.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/graphics/movies/
--rw-r--r--   0 runner    (1001) docker     (121)   130587 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/movies/ping_pong.movie.json
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/render.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/lpminimk3/graphics/schema/
--rw-r--r--   0 runner    (1001) docker     (121)     5507 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/schema/bitmap.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/schema/glyph.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     6078 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/schema/movie.schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/graphics/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/match.py
--rw-r--r--   0 runner    (1001) docker     (121)     4009 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/midi_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/lpminimk3/region.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-19 09:13:51.039646 lpminimk3-0.5.0/lpminimk3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7663 2022-05-19 09:13:50.000000 lpminimk3-0.5.0/lpminimk3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-05-19 09:13:50.000000 lpminimk3-0.5.0/lpminimk3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-19 09:13:50.000000 lpminimk3-0.5.0/lpminimk3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-05-19 09:13:50.000000 lpminimk3-0.5.0/lpminimk3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-19 09:13:50.000000 lpminimk3-0.5.0/lpminimk3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-19 09:13:51.043646 lpminimk3-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-05-19 09:13:37.000000 lpminimk3-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36820 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_core/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/_lpminimk3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/colors/_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/display_character.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/light_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/party.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/print_text_scroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/sync_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/examples/text_scroll_region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29194 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_renderable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/art/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/art/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/art/_art.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/bitmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/bitmaps/smiley.bitmap.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/glyphs/basic_latin.glyph.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/movies/
+-rw-r--r--   0 runner    (1001) docker     (123)   130587 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/movies/ping_pong.movie.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/lpminimk3/graphics/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/schema/bitmap.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/schema/glyph.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/schema/movie.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/graphics/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/midi_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/lpminimk3/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 00:43:11.338752 lpminimk3-0.5.1/lpminimk3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 00:43:11.000000 lpminimk3-0.5.1/lpminimk3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 00:43:11.342752 lpminimk3-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-11 00:43:02.000000 lpminimk3-0.5.1/setup.py
```

### Comparing `lpminimk3-0.5.0/LICENSE` & `lpminimk3-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/PKG-INFO` & `lpminimk3-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: lpminimk3
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python API for the Novation Launchpad Mini MK3
 Home-page: https://github.com/obeezzy/lpminimk3
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lpminimk3
@@ -212,9 +211,7 @@
 
 ## Notes
 * Work in progress, so expect things to break!
 
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
-
-
```

### Comparing `lpminimk3-0.5.0/README.md` & `lpminimk3-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/_core/components.py` & `lpminimk3-0.5.1/lpminimk3/_core/components.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/_core/logging.py` & `lpminimk3-0.5.1/lpminimk3/_core/logging.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/_core/utils.py` & `lpminimk3-0.5.1/lpminimk3/_core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,25 +179,25 @@
         if (self._direction == MidiPort.OUT
                 and not self._midi_out.is_port_open()):
             if self._virtual:
                 self._midi_out.open_virtual_port(self._system_port_name)
             else:
                 self._midi_out.open_port(self.port_index, MidiPort.OUT)
 
-            if platform.system() != 'Windows':
+            if platform.system() != 'Windows' and platform.system() != 'Darwin':
                 self._midi_out.set_client_name(MidiPort.DEFAULT_CLIENT_NAME)
 
         elif (self._direction == MidiPort.IN
                 and not self._midi_in.is_port_open()):
             if self._virtual:
                 self._midi_in.open_virtual_port(self._system_port_name)
             else:
                 self._midi_in.open_port(self.port_index, MidiPort.IN)
 
-            if platform.system() != 'Windows':
+            if platform.system() != 'Windows' and platform.system() != 'Darwin':
                 self._midi_in.set_client_name(MidiPort.DEFAULT_CLIENT_NAME)
 
     def close(self):
         if self.is_open():
             if self._midi_out and self._direction == MidiPort.OUT:
                 self._midi_out.close_port()
             elif self._midi_in and self._direction == MidiPort.IN:
```

### Comparing `lpminimk3-0.5.0/lpminimk3/_lpminimk3.py` & `lpminimk3-0.5.1/lpminimk3/_lpminimk3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-Software representation of the Launchpad Mini MK3.
-"""
-
 from rtmidi import MidiOut, MidiIn
 from ._core.components import Grid, Panel
 from ._core.utils import SystemMidiPortParser, \
                           MidiPort, MidiClient, \
                           Interface, Mode, Layout # noqa
 from .midi_messages import SysExMessages
```

### Comparing `lpminimk3-0.5.0/lpminimk3/colors/_colors.py` & `lpminimk3-0.5.1/lpminimk3/colors/_colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-Colors for the Launchpad Mini MK3.
-"""
-
 import re
 
 
 class RgbColor:
     """
     An RGB color.
     """
```

### Comparing `lpminimk3-0.5.0/lpminimk3/examples/display_character.py` & `lpminimk3-0.5.1/lpminimk3/examples/display_character.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/examples/flash.py` & `lpminimk3-0.5.1/lpminimk3/examples/flash.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/examples/hello.py` & `lpminimk3-0.5.1/lpminimk3/examples/hello.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/examples/light_on_push.py` & `lpminimk3-0.5.1/lpminimk3/examples/light_on_push.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/examples/party.py` & `lpminimk3-0.5.1/lpminimk3/examples/party.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/examples/text_scroll_region.py` & `lpminimk3-0.5.1/lpminimk3/examples/text_scroll_region.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/_graphics.py` & `lpminimk3-0.5.1/lpminimk3/graphics/_graphics.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/_parser.py` & `lpminimk3-0.5.1/lpminimk3/graphics/_parser.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/_renderable.py` & `lpminimk3-0.5.1/lpminimk3/graphics/_renderable.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/_renderer.py` & `lpminimk3-0.5.1/lpminimk3/graphics/_renderer.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/_utils.py` & `lpminimk3-0.5.1/lpminimk3/graphics/_utils.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/bitmaps/smiley.bitmap.json` & `lpminimk3-0.5.1/lpminimk3/graphics/bitmaps/smiley.bitmap.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/glyphs/basic_latin.glyph.json` & `lpminimk3-0.5.1/lpminimk3/graphics/glyphs/basic_latin.glyph.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/movies/ping_pong.movie.json` & `lpminimk3-0.5.1/lpminimk3/graphics/movies/ping_pong.movie.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/render.py` & `lpminimk3-0.5.1/lpminimk3/graphics/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Render script for rendering texts, bitmaps and movies.
+"""
+
 import json
 import sys
 from argparse import ArgumentParser, FileType
 from lpminimk3 import find_launchpads, Mode
 from lpminimk3.graphics import Text, Bitmap, Movie
```

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/schema/bitmap.schema.json` & `lpminimk3-0.5.1/lpminimk3/graphics/schema/bitmap.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/schema/glyph.schema.json` & `lpminimk3-0.5.1/lpminimk3/graphics/schema/glyph.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/graphics/schema/movie.schema.json` & `lpminimk3-0.5.1/lpminimk3/graphics/schema/movie.schema.json`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/match.py` & `lpminimk3-0.5.1/lpminimk3/match.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3/midi_messages.py` & `lpminimk3-0.5.1/lpminimk3/midi_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 MIDI messages for the Launchpad Mini MK3.
 """
+
 from abc import ABC
 from functools import reduce
 
 
 class SysExMessages:
     DEVICE_INQUIRY = [0xf0, 0x7e, 0xe7, 0xf0, 0x06, 0x01, 0xf7]
```

### Comparing `lpminimk3-0.5.0/lpminimk3/region.py` & `lpminimk3-0.5.1/lpminimk3/region.py`

 * *Files identical despite different names*

### Comparing `lpminimk3-0.5.0/lpminimk3.egg-info/PKG-INFO` & `lpminimk3-0.5.1/lpminimk3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: lpminimk3
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python API for the Novation Launchpad Mini MK3
 Home-page: https://github.com/obeezzy/lpminimk3
 Author: Chronic Coder
 Author-email: efeoghene.obebeduo@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lpminimk3
@@ -212,9 +211,7 @@
 
 ## Notes
 * Work in progress, so expect things to break!
 
 
 ## License
 [MIT](https://choosealicense.com/licenses/mit/)
-
-
```

### Comparing `lpminimk3-0.5.0/lpminimk3.egg-info/SOURCES.txt` & `lpminimk3-0.5.1/lpminimk3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 lpminimk3/examples/__init__.py
 lpminimk3/examples/display_character.py
 lpminimk3/examples/flash.py
 lpminimk3/examples/hello.py
 lpminimk3/examples/light_on_push.py
 lpminimk3/examples/party.py
 lpminimk3/examples/print_text_scroll.py
+lpminimk3/examples/sync_client.py
 lpminimk3/examples/text_scroll_region.py
 lpminimk3/graphics/__init__.py
 lpminimk3/graphics/_graphics.py
 lpminimk3/graphics/_parser.py
 lpminimk3/graphics/_renderable.py
 lpminimk3/graphics/_renderer.py
 lpminimk3/graphics/_utils.py
```

### Comparing `lpminimk3-0.5.0/setup.py` & `lpminimk3-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (ROOT_DIR / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="lpminimk3",
-    version="0.5.0",
+    version="0.5.1",
     description="Python API for the Novation Launchpad Mini MK3",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/obeezzy/lpminimk3",
     author="Chronic Coder",
     author_email="efeoghene.obebeduo@gmail.com",
     license="MIT",
```

