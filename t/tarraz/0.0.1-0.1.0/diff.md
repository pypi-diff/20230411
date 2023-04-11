# Comparing `tmp/tarraz-0.0.1.tar.gz` & `tmp/tarraz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarraz-0.0.1.tar", last modified: Mon Apr 10 20:56:37 2023, max compression
+gzip compressed data, was "tarraz-0.1.0.tar", last modified: Tue Apr 11 02:02:14 2023, max compression
```

## Comparing `tarraz-0.0.1.tar` & `tarraz-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:56:37.318230 tarraz-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-10 20:56:26.000000 tarraz-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-10 20:56:37.318230 tarraz-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-10 20:56:26.000000 tarraz-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-10 20:56:37.318230 tarraz-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-10 20:56:26.000000 tarraz-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:56:37.314230 tarraz-0.0.1/tarraz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:56:26.000000 tarraz-0.0.1/tarraz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 20:56:26.000000 tarraz-0.0.1/tarraz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-10 20:56:26.000000 tarraz-0.0.1/tarraz/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-10 20:56:26.000000 tarraz-0.0.1/tarraz/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-10 20:56:26.000000 tarraz-0.0.1/tarraz/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-10 20:56:26.000000 tarraz-0.0.1/tarraz/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-10 20:56:26.000000 tarraz-0.0.1/tarraz/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 20:56:26.000000 tarraz-0.0.1/tarraz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:56:37.318230 tarraz-0.0.1/tarraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-10 20:56:37.000000 tarraz-0.0.1/tarraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-10 20:56:37.000000 tarraz-0.0.1/tarraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:56:37.000000 tarraz-0.0.1/tarraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-10 20:56:37.000000 tarraz-0.0.1/tarraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 20:56:37.000000 tarraz-0.0.1/tarraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-10 20:56:37.000000 tarraz-0.0.1/tarraz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:14.867668 tarraz-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-11 02:02:05.000000 tarraz-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-11 02:02:14.867668 tarraz-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-11 02:02:05.000000 tarraz-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-11 02:02:14.867668 tarraz-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-11 02:02:05.000000 tarraz-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:14.867668 tarraz-0.1.0/tarraz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:05.000000 tarraz-0.1.0/tarraz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-11 02:02:05.000000 tarraz-0.1.0/tarraz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-11 02:02:05.000000 tarraz-0.1.0/tarraz/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-11 02:02:05.000000 tarraz-0.1.0/tarraz/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-11 02:02:05.000000 tarraz-0.1.0/tarraz/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-11 02:02:05.000000 tarraz-0.1.0/tarraz/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-11 02:02:05.000000 tarraz-0.1.0/tarraz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 02:02:05.000000 tarraz-0.1.0/tarraz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:02:14.867668 tarraz-0.1.0/tarraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-11 02:02:14.000000 tarraz-0.1.0/tarraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-11 02:02:14.000000 tarraz-0.1.0/tarraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:02:14.000000 tarraz-0.1.0/tarraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 02:02:14.000000 tarraz-0.1.0/tarraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 02:02:14.000000 tarraz-0.1.0/tarraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 02:02:14.000000 tarraz-0.1.0/tarraz.egg-info/top_level.txt
```

### Comparing `tarraz-0.0.1/LICENSE` & `tarraz-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarraz-0.0.1/setup.py` & `tarraz-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tarraz-0.0.1/tarraz/constants.py` & `tarraz-0.1.0/tarraz/constants.py`

 * *Files identical despite different names*

### Comparing `tarraz-0.0.1/tarraz/logger.py` & `tarraz-0.1.0/tarraz/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import json
 import logging
 
 
 class JsonFormatter(logging.Formatter):
     def format(self, record):
-        # TODO: remove this
-        return f"{record.levelname}\t {record.getMessage()}"
         log_record = {
             "timestamp": self.formatTime(record),
             "message": record.getMessage(),
             "severity": record.levelname,
             "module": record.module,
             "line": record.lineno,
         }
```

### Comparing `tarraz-0.0.1/tarraz/main.py` & `tarraz-0.1.0/tarraz/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import argparse
 
-import version
-import constants
-from logger import logger
-from processor import Tarraz
-from providers import DMCProvider
-from stitcher import DisplayStitcher, SVGStitcher
-from utils import parser, file_choices, color_choices
+from tarraz import version
+from tarraz import constants
+from tarraz.logger import logger
+from tarraz.processor import Tarraz
+from tarraz.providers import DMCProvider
+from tarraz.stitcher import DisplayStitcher, SVGStitcher
+from tarraz.utils import parser, file_choices, color_choices
 
 
 def init_argparse() -> argparse.ArgumentParser:
     parser.add_argument(
         "-v",
         "--version",
         action="version",
@@ -102,15 +102,15 @@
 
     if args.transparent:
         logger.info("Transparent colors: %s", args.transparent)
 
     provider = DMCProvider(args.dmc)
     tarraz = Tarraz(
         args.image,
-        provider,
+        provider=provider,
         x_count=args.stitches_count,
         colors_num=args.colors,
         result_width=args.width,
         cleanup=not args.no_cleanup,
     )
 
     pattern, colors = tarraz.process()
@@ -135,8 +135,8 @@
             save_to=f"{args.dist}/{base_file_name}",
         )
 
     logger.info("Tarraz process finished successfully!")
 
 
 if __name__ == "__main__":
-    main()
+    exit(main())
```

### Comparing `tarraz-0.0.1/tarraz/models.py` & `tarraz-0.1.0/tarraz/models.py`

 * *Files identical despite different names*

### Comparing `tarraz-0.0.1/tarraz/processor.py` & `tarraz-0.1.0/tarraz/processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from PIL import Image
 from typing import List, TYPE_CHECKING, Union
 
-from logger import logger
-from models import Color, Coordinate, ImageSize, RGB
-from utils import generate_image, get_neighbours, index_of
+from tarraz.logger import logger
+from tarraz.models import Color, Coordinate, ImageSize, RGB
+from tarraz.providers import DMCProvider
+from tarraz.utils import generate_image, get_neighbours, index_of
 
 if TYPE_CHECKING:
-    from models import Palette, PaletteImage, PaletteImageRow, RGBImage, RGBImageRow
-    from providers import ColorProvider
+    from tarraz.models import (
+        Palette,
+        PaletteImage,
+        PaletteImageRow,
+        RGBImage,
+        RGBImageRow,
+    )
+    from tarraz.providers import ColorProvider
 
 
 class Tarraz(object):
     def __init__(
         self,
         image_path: str,
-        provider: "ColorProvider",
+        provider: "ColorProvider" = DMCProvider(),
         cleanup: bool = True,
         colors_num: int = 3,
         result_width: int = 1000,
         x_count: int = 50,
     ) -> None:
         self.new_width = result_width
```

### Comparing `tarraz-0.0.1/tarraz/utils.py` & `tarraz-0.1.0/tarraz/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import math
 import os
 from bisect import bisect_left
 from typing import TYPE_CHECKING, List
 
 from PIL import Image, ImageColor
 
-from logger import logger
-from models import ImageSize, RGB
+from tarraz.logger import logger
+from tarraz.models import ImageSize, RGB
 
 if TYPE_CHECKING:
-    from models import Coordinate, RGBImage
     from PIL.Image import Image as ImageType
+    from tarraz.models import Coordinate, RGBImage
 
 
 parser = argparse.ArgumentParser(
     description="Generate a DMC-colored cross-stitch pattern from a given image.",
 )
```

