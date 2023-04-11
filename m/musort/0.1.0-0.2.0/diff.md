# Comparing `tmp/musort-0.1.0.tar.gz` & `tmp/musort-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musort-0.1.0.tar", last modified: Wed Dec 28 13:35:35 2022, max compression
+gzip compressed data, was "musort-0.2.0.tar", last modified: Tue Apr 11 17:38:45 2023, max compression
```

## Comparing `musort-0.1.0.tar` & `musort-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-12-28 13:35:35.122666 musort-0.1.0/
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1081 2022-12-28 10:53:13.000000 musort-0.1.0/LICENSE
--rw-r--r--   0 ernie     (1000) ernie     (1000)       88 2022-12-28 10:53:13.000000 musort-0.1.0/MANIFEST.in
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1427 2022-12-28 13:35:35.122666 musort-0.1.0/PKG-INFO
--rw-r--r--   0 ernie     (1000) ernie     (1000)      760 2022-12-28 13:13:13.000000 musort-0.1.0/README.md
--rwxr-xr-x   0 ernie     (1000) ernie     (1000)       88 2022-12-28 10:53:13.000000 musort-0.1.0/musort
--rw-r--r--   0 ernie     (1000) ernie     (1000)      228 2022-12-28 10:53:13.000000 musort-0.1.0/pyproject.toml
--rw-r--r--   0 ernie     (1000) ernie     (1000)       61 2022-12-28 10:53:13.000000 musort-0.1.0/requirements-dev.txt
--rw-r--r--   0 ernie     (1000) ernie     (1000)       44 2022-12-28 10:53:13.000000 musort-0.1.0/requirements.txt
--rw-r--r--   0 ernie     (1000) ernie     (1000)       38 2022-12-28 13:35:35.122666 musort-0.1.0/setup.cfg
--rwxr-xr-x   0 ernie     (1000) ernie     (1000)     1493 2022-12-28 10:53:13.000000 musort-0.1.0/setup.py
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-12-28 13:35:35.120666 musort-0.1.0/src/
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-12-28 13:35:35.121666 musort-0.1.0/src/musort/
--rw-r--r--   0 ernie     (1000) ernie     (1000)      472 2022-12-28 10:53:13.000000 musort-0.1.0/src/musort/__init__.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)       80 2022-12-28 10:53:13.000000 musort-0.1.0/src/musort/__main__.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)      149 2022-12-28 13:34:43.000000 musort-0.1.0/src/musort/info.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)      130 2022-12-28 10:53:13.000000 musort-0.1.0/src/musort/sort_files.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)     3525 2022-12-28 13:20:11.000000 musort-0.1.0/src/musort/sort_folders.py
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-12-28 13:35:35.121666 musort-0.1.0/src/musort/tools/
--rw-r--r--   0 ernie     (1000) ernie     (1000)     5705 2022-12-28 13:09:57.000000 musort-0.1.0/src/musort/tools/__init__.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)     3951 2022-12-28 13:20:11.000000 musort-0.1.0/src/musort/tools/clargparser.py
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-12-28 13:35:35.121666 musort-0.1.0/src/musort/tools/os_locale/
--rw-r--r--   0 ernie     (1000) ernie     (1000)      259 2022-12-28 10:53:13.000000 musort-0.1.0/src/musort/tools/os_locale/__init__.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)      225 2022-12-28 10:53:13.000000 musort-0.1.0/src/musort/tools/os_locale/linux.py
--rw-r--r--   0 ernie     (1000) ernie     (1000)      674 2022-12-28 10:53:13.000000 musort-0.1.0/src/musort/tools/os_locale/windows.py
-drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2022-12-28 13:35:35.121666 musort-0.1.0/src/musort.egg-info/
--rw-r--r--   0 ernie     (1000) ernie     (1000)     1427 2022-12-28 13:35:35.000000 musort-0.1.0/src/musort.egg-info/PKG-INFO
--rw-r--r--   0 ernie     (1000) ernie     (1000)      558 2022-12-28 13:35:35.000000 musort-0.1.0/src/musort.egg-info/SOURCES.txt
--rw-r--r--   0 ernie     (1000) ernie     (1000)        1 2022-12-28 13:35:35.000000 musort-0.1.0/src/musort.egg-info/dependency_links.txt
--rw-r--r--   0 ernie     (1000) ernie     (1000)       44 2022-12-28 13:35:35.000000 musort-0.1.0/src/musort.egg-info/requires.txt
--rw-r--r--   0 ernie     (1000) ernie     (1000)        7 2022-12-28 13:35:35.000000 musort-0.1.0/src/musort.egg-info/top_level.txt
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2023-04-11 17:38:45.416802 musort-0.2.0/
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1081 2023-03-28 22:54:22.000000 musort-0.2.0/LICENSE
+-rw-r--r--   0 ernie     (1000) ernie     (1000)       88 2023-03-28 22:54:22.000000 musort-0.2.0/MANIFEST.in
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1420 2023-04-11 17:38:45.416802 musort-0.2.0/PKG-INFO
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      753 2023-03-28 22:54:22.000000 musort-0.2.0/README.md
+-rwxr-xr-x   0 ernie     (1000) ernie     (1000)       88 2023-03-28 22:54:22.000000 musort-0.2.0/musort
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      261 2023-04-06 16:57:05.000000 musort-0.2.0/pyproject.toml
+-rw-r--r--   0 ernie     (1000) ernie     (1000)       61 2023-03-28 22:54:22.000000 musort-0.2.0/requirements-dev.txt
+-rw-r--r--   0 ernie     (1000) ernie     (1000)       44 2023-03-28 22:54:22.000000 musort-0.2.0/requirements.txt
+-rw-r--r--   0 ernie     (1000) ernie     (1000)       38 2023-04-11 17:38:45.416802 musort-0.2.0/setup.cfg
+-rwxr-xr-x   0 ernie     (1000) ernie     (1000)     1493 2023-03-28 22:54:22.000000 musort-0.2.0/setup.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2023-04-11 17:38:45.413802 musort-0.2.0/src/
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2023-04-11 17:38:45.415802 musort-0.2.0/src/musort/
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      586 2023-04-07 04:39:47.000000 musort-0.2.0/src/musort/__init__.py
+-rw-r--r--   0 ernie     (1000) ernie     (1000)       80 2023-03-28 22:54:22.000000 musort-0.2.0/src/musort/__main__.py
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      149 2023-04-11 17:38:17.000000 musort-0.2.0/src/musort/info.py
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      116 2023-04-07 04:15:11.000000 musort-0.2.0/src/musort/sort_files.py
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     4002 2023-04-07 04:22:42.000000 musort-0.2.0/src/musort/sort_folders.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2023-04-11 17:38:45.416802 musort-0.2.0/src/musort/tools/
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     5697 2023-03-28 22:54:22.000000 musort-0.2.0/src/musort/tools/__init__.py
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     4759 2023-04-07 04:33:17.000000 musort-0.2.0/src/musort/tools/clargparser.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2023-04-11 17:38:45.416802 musort-0.2.0/src/musort/tools/os_locale/
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      259 2023-03-28 22:54:22.000000 musort-0.2.0/src/musort/tools/os_locale/__init__.py
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      209 2023-03-28 22:54:22.000000 musort-0.2.0/src/musort/tools/os_locale/linux.py
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      645 2023-03-28 22:54:22.000000 musort-0.2.0/src/musort/tools/os_locale/windows.py
+drwxr-xr-x   0 ernie     (1000) ernie     (1000)        0 2023-04-11 17:38:45.415802 musort-0.2.0/src/musort.egg-info/
+-rw-r--r--   0 ernie     (1000) ernie     (1000)     1420 2023-04-11 17:38:45.000000 musort-0.2.0/src/musort.egg-info/PKG-INFO
+-rw-r--r--   0 ernie     (1000) ernie     (1000)      558 2023-04-11 17:38:45.000000 musort-0.2.0/src/musort.egg-info/SOURCES.txt
+-rw-r--r--   0 ernie     (1000) ernie     (1000)        1 2023-04-11 17:38:45.000000 musort-0.2.0/src/musort.egg-info/dependency_links.txt
+-rw-r--r--   0 ernie     (1000) ernie     (1000)       44 2023-04-11 17:38:45.000000 musort-0.2.0/src/musort.egg-info/requires.txt
+-rw-r--r--   0 ernie     (1000) ernie     (1000)        7 2023-04-11 17:38:45.000000 musort-0.2.0/src/musort.egg-info/top_level.txt
```

### Comparing `musort-0.1.0/LICENSE` & `musort-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `musort-0.1.0/PKG-INFO` & `musort-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musort
-Version: 0.1.0
+Version: 0.2.0
 Summary: A music-sorting package.
 Home-page: https://github.com/ernieIzde8ski/mus_sort
 Author: Ernest Izdebski
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -41,16 +41,16 @@
 make init build
 ```
 
 ## Usage
 
 See `python -m musort --help` for usage.
 
-If found in the present working directory, configuration files named either
-`musort.txt` or `mus_sort.txt` will be loaded. A sample is provided:
+If found in the present working directory, configuration files named `musort-conf` or
+`musort_conf` will be loaded. A sample is provided:
 
 ```sh
 .
 # reorganize by folder and rename tracks
 --folder-mode --file-mode
 # ignore FileExistsError
 --replace-duplicates
```

### Comparing `musort-0.1.0/setup.py` & `musort-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `musort-0.1.0/src/musort/sort_folders.py` & `musort-0.2.0/src/musort/sort_folders.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,25 +43,27 @@
         if sfile.is_file():
             sfile.replace(tfile)
         elif sfile.is_dir():
             tfile.mkdir(exist_ok=True)
             replace_folder(sfile, tfile)
 
 
-def sort_folder(music: MusicFile) -> None:
+def sort_music_folder(music: MusicFile) -> None:
     """Sort a folder containing a music file."""
     source = music.path.parent
     target = music.get_new_dir()
 
     if source == target:
         logging.debug(f"Directory at `{source}` is equal to new directory, short-circuiting")
         return
 
     try:
         target.parent.mkdir(parents=True, exist_ok=True)
+        if target.exists():
+            raise FileExistsError(str(target))
         source.rename(target)
         logging.info(f"Renamed {source.as_posix()} -> {target.as_posix()}")
     except OSError as err:
         if not clargs.replace_duplicates:
             raise
 
         # the error must be either a) directory not empty or b) file already exists
@@ -74,16 +76,22 @@
             )
             raise
 
         replace_folder(source, target)
         logging.info(f"Replaced {source.as_posix()} -> {target.as_posix()}")
 
 
-def sort(dir: Path = clargs.dir, /) -> None:
+def sort_folder(dir: Path) -> None:
     """Sort a given folder and all subfolders."""
+
+    # folders containing a .musort_ignore file are unconditionally skipped
+    if (dir / ".musort_ignore").exists():
+        logging.debug(f"short-circuiting, .musort_ignore file found in {dir}")
+        return
+
     music_path: Path | None = None
 
     for path in tools.iterdir(dir):
         if path.is_dir():
             sort(path)
         elif (clargs.file_mode or not music_path) and MusicFile.is_music(path):
             path = path.resolve()
@@ -95,8 +103,16 @@
                 # upon finding a music file, we save it for later
                 # I think this could probably cause some minimal lag but w/e
                 music_path = path
                 logging.debug(f"Found music file at {music_path.as_posix()}")
 
     if music_path is not None:
         with Suppress(*common_exceptions, path=music_path):
-            sort_folder(MusicFile.get(music_path))
+            sort_music_folder(MusicFile.get(music_path))
+
+
+def sort(*dirs: Path):
+    for dir in dirs:
+        if not dir.is_dir():
+            logging.error(f"error: path is not a directory: {dir}")
+        else:
+            sort_folder(dir)
```

### Comparing `musort-0.1.0/src/musort/tools/__init__.py` & `musort-0.2.0/src/musort/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,14 @@
         ".opus",
         ".wav",
         ".flac",
         ".wma",
         ".m4b",
         ".m4a",
         ".m4r",
-        ".mp4",
         ".aiff",
         ".aifc",
         ".aif",
         ".afc",
     }
     """Accepted file suffixes, as per `TinyTag._get_parser_for_filename`."""
 
@@ -154,15 +153,15 @@
     def prepare_component(tag: str | None, default="UNKNOWN", max_size=70):
         """Prepare a TinyTag component for being used as a file path."""
         if not tag:
             return default
         # sometimes a genre tag is actually multiple genres split by semicolons
         resp = tag.split(";")[0].strip()
         # remove characters that result in invalid filenames
-        for s0, s1 in REPLACEMENTS:
+        for s0, s1 in REPLACEMENTS.items():
             resp = resp.replace(s0, s1)
         # reducing the length of the string
         # the default being 70 is absolutely arbitrary
         return textwrap.fill(resp, width=max_size, placeholder="(…)", max_lines=1)
 
     def get_new_dir(self, target: Path = clargs.target, /) -> Path:
         genre = self.prepare_component(self.genre, default="UNKNOWN_GENRE")
```

### Comparing `musort-0.1.0/src/musort/tools/clargparser.py` & `musort-0.2.0/src/musort/tools/clargparser.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 
 from .. import info
 
 DEFAULT_IGNORED = (".git", "itunes")
 
 
 class ClargParser(Tap):
-    dir: Path
+    dirs: list[Path]
     """Folder to sort from."""
     target: Path
-    """Folder sorted into. Defaults to the folder positional argument."""
+    """Folder sorted into.
+    If not present, defaults to the folder containing the first config file found, or the
+    folder being sorted from if no config files were found."""
 
     folder_mode: bool = False
     """Sort by moving entire folders around at a time. Useful if your music is already sorted per-album."""
     file_mode: bool = False
     """Sort by moving individual music files around. Highly disrecommended if your metadata is
     inconsistent, or if you don't want to risk leaving album covers and the like behind.
-    
+
     Alternatively, when used in conjunction with folder-mode, files are renamed within their folders.
     """
 
     level: int = logging.INFO
     """Logging level. Accepts names from the logging module, eg 'debug' or 'info'."""
     ignored_paths: set[str] = set()
     """Ignored file/folder names. Case insensitive."""
@@ -36,14 +38,22 @@
 
     clean_after: bool = False
     """Delete empty folders afterwards."""
     replace_duplicates: bool = False
     """Replace existing paths upon FileExistsError. If artist or album is None, the replacement is ignored."""
     single_genre: bool = False
     """Force any given artist to stay in one genre folder."""
+    use_dashes: bool = False
+    """Replace slashes with dashes in paths."""
+
+
+    def _load_from_config_files(self, config_files: list[str] | None):
+        "override to save config file list to a private attribute"
+        self.config_files: list[str] = config_files if config_files else list()
+        return super()._load_from_config_files(config_files=config_files)
 
     @staticmethod
     def _get_level(name: str):
         """Get logging level from a string."""
         if name.isnumeric():
             num = int(name)
             if num in logging._levelToName:
@@ -56,53 +66,70 @@
 
     def configure(self) -> None:
         self.add_argument(
             "-V", "--version", action="version", version=f"musort v{info.__version__}"
         )
 
         # making the first argument positional, the second unrequired
-        self.add_argument("dir")
+        self.add_argument("dirs", nargs='+')
         self.add_argument("-T", "--target", required=False)
 
         # logging module weirdness
         self.add_argument("-l", "--level", type=self._get_level, choices=(logging._levelToName))
 
         # providing aliases
         self.add_argument("-i", "--ignored_paths")
         self.add_argument("-H", "--hidden")
         self.add_argument("-C", "--clean_after")
         self.add_argument("-S", "--single_genre")
 
-        # appending a line to --help
-        self.epilog = """This program sorts folders based on ID3 data. As such,
-        if the tags on your music are unruly, it's probably best to sort that out first."""
-
     def process_args(self) -> None:
         # ensure given directories exist
-        self.dir = self.dir.resolve()
-        self.target = self.dir if self.target is None else self.target.resolve()
-        if not self.dir.is_dir():
-            raise ArgumentError(None, "dir parameter must be a valid directory!")
-        elif not self.target.is_dir():
-            raise ArgumentError(None, "target parameter must be a valid directory!")
+        if not self.dirs:
+            raise ArgumentError(None, "")
+        if self.target is None:
+            if self.config_files:
+                self.target = Path(self.config_files[0]).parent
+            else:
+                self.target = self.dirs[0]
+
+        if not self.target.is_dir():
+            raise ArgumentError(
+                None, "target parameter must be a valid directory! got: " + str(self.target)
+            )
 
         # making case insensitive
         self.ignored_paths = {*(i.lower() for i in self.ignored_paths), *DEFAULT_IGNORED}
 
         # ensure at least one sort method is chosen
         if not (self.file_mode or self.folder_mode):
             raise ArgumentError(None, "Either --file-mode or --folder-mode should be active")
 
 
-def find_config_files(foldir: Path):
-    for path in foldir.iterdir():
-        if path.name.lower() in ["musort.txt", "mus_sort.txt"] and path.is_file():
-            yield path.name
+_VALID_CONFIGS = ("musort_conf", "musort-conf", "musort.txt", "mus_sort.txt")
 
 
+def find_config_file(folder: Path = Path.cwd()) -> Path | None:
+    for config_name in _VALID_CONFIGS:
+        path = folder / config_name
+        if path.is_file():
+            return path
+
+    # for root directory, path.parent == path
+    if folder.parent != folder:
+        return find_config_file(folder.parent)
+
+
+config = find_config_file()
 clargs = ClargParser(
-    underscores_to_dashes=True, config_files=list(find_config_files(Path()))
+    underscores_to_dashes=True,
+    config_files=[str(config)] if config else None,
+    epilog=(
+        "This program sorts folders based on ID3 data. "
+        "So, if the tags on your music are unruly, "
+        "it's probably best to sort that out first."
+    ),
 ).parse_args()
+
 logging.basicConfig(level=clargs.level, stream=sys.stdout)
 
-if __name__ == "__main__":
-    print(clargs)
+logging.debug(f"current command-line arguments:\n{clargs}")
```

### Comparing `musort-0.1.0/src/musort.egg-info/PKG-INFO` & `musort-0.2.0/src/musort.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musort
-Version: 0.1.0
+Version: 0.2.0
 Summary: A music-sorting package.
 Home-page: https://github.com/ernieIzde8ski/mus_sort
 Author: Ernest Izdebski
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -41,16 +41,16 @@
 make init build
 ```
 
 ## Usage
 
 See `python -m musort --help` for usage.
 
-If found in the present working directory, configuration files named either
-`musort.txt` or `mus_sort.txt` will be loaded. A sample is provided:
+If found in the present working directory, configuration files named `musort-conf` or
+`musort_conf` will be loaded. A sample is provided:
 
 ```sh
 .
 # reorganize by folder and rename tracks
 --folder-mode --file-mode
 # ignore FileExistsError
 --replace-duplicates
```

### Comparing `musort-0.1.0/src/musort.egg-info/SOURCES.txt` & `musort-0.2.0/src/musort.egg-info/SOURCES.txt`

 * *Files identical despite different names*

