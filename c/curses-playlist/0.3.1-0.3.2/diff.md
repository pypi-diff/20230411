# Comparing `tmp/curses-playlist-0.3.1.tar.gz` & `tmp/curses-playlist-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curses-playlist-0.3.1.tar", max compression
+gzip compressed data, was "curses-playlist-0.3.2.tar", max compression
```

## Comparing `curses-playlist-0.3.1.tar` & `curses-playlist-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      180 2022-06-14 17:38:35.961625 curses-playlist-0.3.1/curses_playlist/__init__.py
--rw-r--r--   0        0        0     6362 2022-06-26 14:44:36.449783 curses-playlist-0.3.1/curses_playlist/controller.py
--rw-r--r--   0        0        0     5676 2022-06-05 16:32:09.171204 curses-playlist-0.3.1/curses_playlist/curses_gui.py
--rw-r--r--   0        0        0     6613 2022-06-05 16:32:09.171204 curses-playlist-0.3.1/curses_playlist/gui_state.py
--rw-r--r--   0        0        0      607 2022-06-23 18:26:55.174151 curses-playlist-0.3.1/curses_playlist/platform_defs.py
--rw-r--r--   0        0        0      788 2022-06-26 14:45:29.337269 curses-playlist-0.3.1/curses_playlist/plist.py
--rw-r--r--   0        0        0      359 2022-06-05 16:32:09.173200 curses-playlist-0.3.1/curses_playlist/tools.py
--rw-r--r--   0        0        0     2851 2022-06-14 18:00:31.270027 curses-playlist-0.3.1/curses_playlist/video_file.py
--rw-r--r--   0        0        0     3598 2022-06-05 16:32:09.173200 curses-playlist-0.3.1/curses_playlist/video_store.py
--rw-r--r--   0        0        0     1087 2022-05-28 12:45:13.748479 curses-playlist-0.3.1/LICENSE
--rw-r--r--   0        0        0      559 2022-06-26 15:19:05.069483 curses-playlist-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      980 2022-06-05 18:41:33.527480 curses-playlist-0.3.1/README.md
--rw-r--r--   0        0        0     1854 2022-06-26 15:19:07.593959 curses-playlist-0.3.1/setup.py
--rw-r--r--   0        0        0     1707 2022-06-26 15:19:07.593959 curses-playlist-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      180 2022-06-14 17:38:35.961625 curses-playlist-0.3.2/curses_playlist/__init__.py
+-rw-r--r--   0        0        0     6362 2022-06-26 14:44:36.449783 curses-playlist-0.3.2/curses_playlist/controller.py
+-rw-r--r--   0        0        0     5676 2022-06-05 16:32:09.171204 curses-playlist-0.3.2/curses_playlist/curses_gui.py
+-rw-r--r--   0        0        0     6613 2022-06-05 16:32:09.171204 curses-playlist-0.3.2/curses_playlist/gui_state.py
+-rw-r--r--   0        0        0      607 2022-06-23 18:26:55.174151 curses-playlist-0.3.2/curses_playlist/platform_defs.py
+-rw-r--r--   0        0        0      788 2022-06-26 14:45:29.337269 curses-playlist-0.3.2/curses_playlist/plist.py
+-rw-r--r--   0        0        0      359 2022-06-05 16:32:09.173200 curses-playlist-0.3.2/curses_playlist/tools.py
+-rw-r--r--   0        0        0     2869 2023-04-11 19:48:26.780588 curses-playlist-0.3.2/curses_playlist/video_file.py
+-rw-r--r--   0        0        0     3598 2022-06-05 16:32:09.173200 curses-playlist-0.3.2/curses_playlist/video_store.py
+-rw-r--r--   0        0        0     1087 2022-05-28 12:45:13.748479 curses-playlist-0.3.2/LICENSE
+-rw-r--r--   0        0        0      586 2023-04-11 19:49:26.471786 curses-playlist-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      980 2022-06-05 18:41:33.527480 curses-playlist-0.3.2/README.md
+-rw-r--r--   0        0        0     1887 2023-04-11 19:49:54.839746 curses-playlist-0.3.2/setup.py
+-rw-r--r--   0        0        0     1754 2023-04-11 19:49:54.839746 curses-playlist-0.3.2/PKG-INFO
```

### Comparing `curses-playlist-0.3.1/curses_playlist/controller.py` & `curses-playlist-0.3.2/curses_playlist/controller.py`

 * *Files identical despite different names*

### Comparing `curses-playlist-0.3.1/curses_playlist/curses_gui.py` & `curses-playlist-0.3.2/curses_playlist/curses_gui.py`

 * *Files identical despite different names*

### Comparing `curses-playlist-0.3.1/curses_playlist/gui_state.py` & `curses-playlist-0.3.2/curses_playlist/gui_state.py`

 * *Files identical despite different names*

### Comparing `curses-playlist-0.3.1/curses_playlist/platform_defs.py` & `curses-playlist-0.3.2/curses_playlist/platform_defs.py`

 * *Files identical despite different names*

### Comparing `curses-playlist-0.3.1/curses_playlist/plist.py` & `curses-playlist-0.3.2/curses_playlist/plist.py`

 * *Files identical despite different names*

### Comparing `curses-playlist-0.3.1/curses_playlist/video_file.py` & `curses-playlist-0.3.2/curses_playlist/video_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """
         self.stat = os.stat(self.locale_path)
         try:
             tmp_video = VideoFileClip(self.locale_path)
             self.duration = timedelta(seconds=tmp_video.duration)
             tmp_video.reader.close()
             tmp_video.audio.reader.close_proc()
-        except UnicodeDecodeError:
+        except (UnicodeDecodeError, AttributeError):
             self.duration = None
 
     def __str__(self):
 
         if self.duration:
             minutes = self.duration.total_seconds() // 60
             seconds = int(self.duration.total_seconds() - minutes * 60)
```

### Comparing `curses-playlist-0.3.1/curses_playlist/video_store.py` & `curses-playlist-0.3.2/curses_playlist/video_store.py`

 * *Files identical despite different names*

### Comparing `curses-playlist-0.3.1/LICENSE` & `curses-playlist-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `curses-playlist-0.3.1/pyproject.toml` & `curses-playlist-0.3.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "curses-playlist"
-version = '0.3.1'
+version = '0.3.2'
 description = "curses based interactive playlist creation for videos"
 authors = ["Dr. Dosn <dr.dosn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 windows-curses = "^2.3.0"
 moviepy = "^1.0.3"
 click = "^8.1.3"
 pydantic = "^1.9.1"
 pycaw = "^20220416"
+python-vlc = "^3.0.18121"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `curses-playlist-0.3.1/README.md` & `curses-playlist-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `curses-playlist-0.3.1/setup.py` & `curses-playlist-0.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'moviepy>=1.0.3,<2.0.0',
  'pycaw>=20220416,<20220417',
  'pydantic>=1.9.1,<2.0.0',
+ 'python-vlc>=3.0.18121,<4.0.0',
  'windows-curses>=2.3.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['plist = curses_playlist.plist:main']}
 
 setup_kwargs = {
     'name': 'curses-playlist',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'curses based interactive playlist creation for videos',
     'long_description': '# plist\ncurses based interactive playlist creation for video files.\n\n# usage\n\n```\nplist.exe --playlist c:\\tmp\\test.m3u --working-directory Z:\\movies\n```\n\n# docs\n\nInteractively create a `playlist.m3u` then launch it using `vlc.exe`. \nAutomatically loads last playlist on startup.\nThere are 2 modes which you can toggle using the `ESC` key:\n```\n[INPUT: ENTER - add | ESC - CMD] \n[CMD: m - mod | q | w | p - play | r - reset]\n```\n\nIn `INPUT` Mode, filenames in the playlist are searched for substrings that you enter, separated by a single whitespace. \n\nE.g.: `rick` `morty` `s01e01` would yield all filenames that contain all 3 strings.\n\nIn `CMD` mode you have the following options:\n\n* `m` move\n  * `j` navigate/move down\n  * `k` navigate/move up\n  * `d` del \n  * `m` toggle navigate/move\n* `p` play: start vlc player with playlist\n* `r` reset: reset the playlist\n* `q` quit: doing nothing\n\n# repo\n\nhttps://github.com/dosnpfand/curses-playlist\n',
     'author': 'Dr. Dosn',
     'author_email': 'dr.dosn@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `curses-playlist-0.3.1/PKG-INFO` & `curses-playlist-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curses-playlist
-Version: 0.3.1
+Version: 0.3.2
 Summary: curses based interactive playlist creation for videos
 License: MIT
 Author: Dr. Dosn
 Author-email: dr.dosn@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
 Requires-Dist: pycaw (>=20220416,<20220417)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
+Requires-Dist: python-vlc (>=3.0.18121,<4.0.0)
 Requires-Dist: windows-curses (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # plist
 curses based interactive playlist creation for video files.
 
 # usage
```

