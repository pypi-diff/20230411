# Comparing `tmp/ssb_sgis-0.1.3.tar.gz` & `tmp/ssb_sgis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.1.3.tar", max compression
+gzip compressed data, was "ssb_sgis-0.1.4.tar", max compression
```

## Comparing `ssb_sgis-0.1.3.tar` & `ssb_sgis-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0     1074 2023-03-31 10:36:42.065223 ssb_sgis-0.1.3/LICENSE
--rw-r--r--   0        0        0     6955 2023-03-31 10:36:42.065223 ssb_sgis-0.1.3/README.md
--rw-r--r--   0        0        0     2465 2023-03-31 10:37:04.337545 ssb_sgis-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1579 2023-03-31 10:36:42.081224 ssb_sgis-0.1.3/src/sgis/__init__.py
--rw-r--r--   0        0        0     2634 2023-03-31 10:36:42.081224 ssb_sgis-0.1.3/src/sgis/dapla.py
--rw-r--r--   0        0        0      666 2023-03-31 10:36:42.081224 ssb_sgis-0.1.3/src/sgis/exceptions.py
--rw-r--r--   0        0        0    38956 2023-03-31 10:37:04.337545 ssb_sgis-0.1.3/src/sgis/explore.py
--rw-r--r--   0        0        0        0 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8776 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    26187 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5456 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    34650 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/geopandas_tools/line_operations.py
--rw-r--r--   0        0        0    16279 2023-03-31 10:37:04.337545 ssb_sgis-0.1.3/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    14044 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6280 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0     5046 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     2468 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/helpers.py
--rw-r--r--   0        0        0    16390 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/maps.py
--rw-r--r--   0        0        0        0 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     5171 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2521 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4819 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4426 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    11360 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0    23901 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0     6120 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/network_norway.py
--rw-r--r--   0        0        0    58050 2023-03-31 10:37:04.341545 ssb_sgis-0.1.3/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12655 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0        0 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/py.typed
--rw-r--r--   0        0        0     3765 2023-03-31 10:36:42.085224 ssb_sgis-0.1.3/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8286 1970-01-01 00:00:00.000000 ssb_sgis-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-11 16:36:33.486727 ssb_sgis-0.1.4/LICENSE
+-rw-r--r--   0        0        0     7070 2023-04-11 16:36:48.967527 ssb_sgis-0.1.4/README.md
+-rw-r--r--   0        0        0     2484 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1651 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/dapla.py
+-rw-r--r--   0        0        0      666 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8776 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    27301 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5456 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    34762 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/line_operations.py
+-rw-r--r--   0        0        0    16647 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    14044 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6316 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0     5046 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     2468 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    21371 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0    17271 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    16587 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    12535 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    11182 2023-04-11 16:36:48.991528 ssb_sgis-0.1.4/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     5171 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2521 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4819 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4426 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    11360 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0    23953 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0     6124 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/network_norway.py
+-rw-r--r--   0        0        0    58054 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12655 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/py.typed
+-rw-r--r--   0        0        0     3765 2023-04-11 16:36:33.522729 ssb_sgis-0.1.4/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8441 1970-01-01 00:00:00.000000 ssb_sgis-0.1.4/PKG-INFO
```

### Comparing `ssb_sgis-0.1.3/LICENSE` & `ssb_sgis-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/README.md` & `ssb_sgis-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 GIS Python tools used in [Statistics Norway](https://www.ssb.no/en).
 
 [![PyPI](https://img.shields.io/pypi/v/ssb-sgis.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/ssb-sgis.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/ssb-sgis)][python version]
 [![License](https://img.shields.io/pypi/l/ssb-sgis)][license]
 
-[![Read the documentation at https://ssb-sgis.readthedocs.io/](https://img.shields.io/readthedocs/ssb-sgis/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Documentation](https://img.shields.io/badge/Documentation-GitHub_Pages-green.svg)](https://statisticsnorway.github.io/ssb-sgis/index.html)
 [![Tests](https://github.com/statisticsnorway/ssb-sgis/workflows/Tests/badge.svg)][tests]
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=statisticsnorway_ssb-sgis&metric=coverage)][coverage]
+[![Coverage](https://sonarcloud.io/component_measures?id=statisticsnorway_ssb-gis-utils&metric=new_coverage&view=list)][coverage]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi_]: https://pypi.org/project/ssb-sgis/
 [status]: https://pypi.org/project/ssb-sgis/
 [python version]: https://pypi.org/project/ssb-sgis
@@ -53,87 +53,86 @@
 rules = sg.NetworkAnalysisRules(weight="minutes")
 
 nwa = sg.NetworkAnalysis(network=nw, rules=rules)
 
 nwa
 ```
 
-```
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
         rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
-```
 
 Get number of times each line segment was visited.
 
 ```python
-freq = nwa.get_route_frequencies(points.sample(75), points.sample(75))
+frequencies = nwa.get_route_frequencies(points.sample(75), points.sample(75))
 
-sg.qtm(
-    sg.buff(freq, 15),
-    "frequency",
-    scheme="naturalbreaks",
-    cmap="plasma",
-    title="Number of times each road was used.",
-)
+m = sg.ThematicMap(sg.buff(frequencies, 15), column="frequency", black=True)
+m.cmap = "plasma"
+m.title = "Number of times each road was used."
+m.plot()
 ```
 
-![png](docs/examples/network_analysis_examples_files/network_analysis_examples_6_0.png)
+![png](docs/examples/network_analysis_examples_files/network_analysis_examples_5_0.png)
 
 Fast many-to-many travel times/distances.
 
 ```python
 od = nwa.od_cost_matrix(points, points)
 
 print(od)
 ```
 
-```
             origin  destination    minutes
     0            0            0   0.000000
     1            0            1  13.039830
     2            0            2  10.902453
     3            0            3   8.297021
     4            0            4  14.742294
     ...        ...          ...        ...
     999995     999          995  11.038673
     999996     999          996  17.820664
     999997     999          997  10.288465
     999998     999          998  14.798257
     999999     999          999   0.000000
 
     [1000000 rows x 3 columns]
-```
 
 Get the area that can be reached within one or more breaks.
 
 ```python
-sa = nwa.service_area(
+service_areas = nwa.service_area(
     points.iloc[[0]],
     breaks=np.arange(1, 11),
 )
 
-sg.qtm(sa, "minutes", k=10, title="Roads that can be reached within 1 to 10 minutes")
+m = sg.ThematicMap(service_areas, column="minutes", black=True, size=10)
+m.k = 10
+m.title = "Roads that can be reached within 1 to 10 minutes"
+m.plot()
 ```
 
-![png](docs/examples/network_analysis_examples_files/network_analysis_examples_10_0.png)
+![png](docs/examples/network_analysis_examples_files/network_analysis_examples_9_0.png)
 
 Get one or more route per origin-destination pair.
 
 ```python
 routes = nwa.get_k_routes(
-    points.iloc[[0]], points.iloc[[1]], k=5, drop_middle_percent=50
+    points.iloc[[0]], points.iloc[[1]], k=4, drop_middle_percent=50
 )
 
-sg.qtm(sg.buff(routes, 15), "k", title="Five fastest routes from A to B", legend=False)
+m = sg.ThematicMap(sg.buff(routes, 15), column="k", black=True)
+m.title = "Four fastest routes from A to B"
+m.legend.title = "Rank"
+m.plot()
 ```
 
-![png](docs/examples/network_analysis_examples_files/network_analysis_examples_12_1.png)
+![png](docs/examples/network_analysis_examples_files/network_analysis_examples_11_0.png)
 
 More network analysis examples can be found here: https://github.com/statisticsnorway/ssb-sgis/blob/main/docs/network_analysis_demo_template.md
 
 Road data for Norway can be downloaded here: https://kartkatalog.geonorge.no/metadata/nvdb-ruteplan-nettverksdatasett/8d0f9066-34f9-4423-be12-8e8523089313
 
 ## Developer information
```

### Comparing `ssb_sgis-0.1.3/pyproject.toml` & `ssb_sgis-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.1.3"
+version = "0.1.4"
 description = "GIS utility functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
@@ -28,14 +28,15 @@
 numpy = "^1.24.2"
 pandas = "^1.5.3"
 pyarrow = "^11.0.0"
 requests = "^2.28.2"
 scikit-learn = "^1.2.1"
 shapely = "^2.0.1"
 xyzservices = "^2023.2.0"
+jenkspy = "^0.3.2"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["d", "jupyter"], version = "^23.1.0"}
 coverage = {extras = ["toml"], version = "^7.2.1"}
 darglint = "^1.8.1"
 deptry = "^0.8.0"
 flake8 = "^6.0.0"
```

### Comparing `ssb_sgis-0.1.3/src/sgis/__init__.py` & `ssb_sgis-0.1.4/src/sgis/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # flake8: noqa: F401
-from .explore import Explore
 from .geopandas_tools.buffer_dissolve_explode import (
     buff,
     buffdiss,
     buffdissexp,
     buffexp,
     dissexp,
 )
 from .geopandas_tools.general import (
     clean_clip,
     clean_geoms,
     coordinate_array,
+    points_in_bounds,
     random_points,
     random_points_in_polygons,
     to_gdf,
     to_lines,
     to_multipoint,
 )
 from .geopandas_tools.geometry_types import (
@@ -38,15 +38,17 @@
     get_all_distances,
     get_k_nearest_neighbors,
     get_neighbor_indices,
 )
 from .geopandas_tools.overlay import clean_shapely_overlay, overlay, overlay_update
 from .geopandas_tools.point_operations import snap_all, snap_within_distance
 from .geopandas_tools.polygon_operations import close_all_holes, close_small_holes
-from .maps import clipmap, explore, qtm, samplemap
+from .maps.legend import Legend
+from .maps.maps import clipmap, explore, qtm, samplemap
+from .maps.thematicmap import ThematicMap
 from .networkanalysis.directednetwork import DirectedNetwork
 from .networkanalysis.network import Network
 from .networkanalysis.networkanalysis import NetworkAnalysis
 from .networkanalysis.networkanalysisrules import NetworkAnalysisRules
 from .read_parquet import read_parquet_url
```

### Comparing `ssb_sgis-0.1.3/src/sgis/dapla.py` & `ssb_sgis-0.1.4/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/exceptions.py` & `ssb_sgis-0.1.4/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/explore.py` & `ssb_sgis-0.1.4/src/sgis/geopandas_tools/line_operations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,1138 +1,1005 @@
-"""Interactive map of one or more GeoDataFrames with layers that can be toggles on/off.
+"""Functions for line geometries.
 
-This module holds the Explore class, which is the basis for the explore, samplemap and
-clipmap functions from the 'maps' module.
+The module includes functions for cutting and splitting lines, cutting lines into
+pieces, filling holes in a network of lines, finding isolated network islands and
+creating unique node ids.
+
+The functions are also methods of the Network class, where some checks and
+preperation is done before each method is run, making sure the lines are correct.
 """
 import warnings
-from statistics import mean
 
-import branca as bc
-import folium
-import geopandas
-import matplotlib
-import matplotlib.cm as cm
-import matplotlib.colors as colors
+import geopandas as gpd
+import networkx as nx
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
-from mapclassify import classify
-from shapely import Geometry
-from shapely.geometry import LineString
-
-from .geopandas_tools.general import (
-    clean_geoms,
-    drop_inactive_geometry_columns,
-    random_points_in_polygons,
-    rename_geometry_if,
-)
-from .geopandas_tools.geometry_types import get_geom_type
-from .helpers import get_name
-
-
-# the geopandas._explore raises a deprication warning. Ignoring for now.
-warnings.filterwarnings(
-    action="ignore", category=matplotlib.MatplotlibDeprecationWarning
-)
-pd.options.mode.chained_assignment = None
-
-
-# custom default colors for non-numeric data, because the geopandas default has very
-# similar colors. The palette is like the "Set2" cmap from matplotlib, but with more
-# colors. If more than 14 categories, the geopandas default cmap is used.
-_CATEGORICAL_CMAP = {
-    0: "#4576ff",
-    1: "#ff455e",
-    2: "#59d45f",
-    3: "#b51d8b",
-    4: "#ffa514",
-    5: "#f2dc4e",
-    6: "#ff8cc9",
-    7: "#6bf2eb",
-    8: "#916209",
-    9: "#008d94",
-    10: "#8a030a",
-    11: "#9c65db",
-    12: "#228000",
-    13: "#80ff00",
-}
-
-# gray for NaNs
-NAN_COLOR = "#969696"
-
-
-# cols to not show when hovering over geometries (tooltip)
-COLS_TO_DROP = ["color", "geometry"]
-
-
-# from geopandas
-_MAP_KWARGS = [
-    "location",
-    "prefer_canvas",
-    "no_touch",
-    "disable_3d",
-    "png_enabled",
-    "zoom_control",
-    "crs",
-    "zoom_start",
-    "left",
-    "top",
-    "position",
-    "min_zoom",
-    "max_zoom",
-    "min_lat",
-    "max_lat",
-    "min_lon",
-    "max_lon",
-    "max_bounds",
-]
-
-
-def _all_are_geom(gdfs: tuple) -> bool:
-    """Returns True if all elements in the tuple are geopandas/shapely geometries."""
-    return all(isinstance(gdf, (GeoDataFrame, GeoSeries, Geometry)) for gdf in gdfs)
-
-
-def _separate_args(
-    args: tuple,
-    column: str | None,
-    kwargs: dict,
-) -> tuple[tuple[GeoDataFrame], str, dict]:
-    """Separate GeoDataFrames from string (column)."""
-    if _all_are_geom(args):
-        return args, column, kwargs
-
-    gdfs: tuple[GeoDataFrame] = ()
-    for arg in args:
-        if isinstance(arg, str):
-            if column is None:
-                column = arg
-            else:
-                raise ValueError(
-                    "Can specify at most one string as a positional argument."
-                )
-        elif isinstance(arg, (GeoDataFrame, GeoSeries, Geometry)):
-            gdfs = gdfs + (arg,)
-
-    if column and not kwargs["column"]:
-        kwargs["column"] = column
-
-    return gdfs, column, kwargs
-
-
-class Explore:
-    """Interactive map of GeoDataFrames with layers that can be toggles on/off.
-
-    It takes all the given GeoDataFrames and displays them together in an
-    interactive map with a common legend. The layers can be toggled on and off.
-
-    If 'column' is not specified, each GeoDataFrame is given a unique color. The
-    default colormap is a custom, strongly colored palette. If a numerical column
-    is given, the 'viridis' palette is the default.
+from pandas import DataFrame, Series
+from shapely import force_2d, shortest_line
+from shapely.geometry import LineString, Point
+
+from .buffer_dissolve_explode import buff
+from .general import _push_geom_col, coordinate_array, to_gdf
+from .neighbors import get_k_nearest_neighbors, k_nearest_neighbors
+from .point_operations import snap_all, snap_within_distance
+
+
+def get_largest_component(lines: GeoDataFrame) -> GeoDataFrame:
+    """Finds the largest network component.
+
+    It takes a GeoDataFrame of lines and finds the lines that are
+    part of the largest connected network component. These lines are given the value
+    1 in the added column 'connected', while isolated network islands get the value
+    0.
+
+    Uses the connected_components function from the networkx package.
+
+    Args:
+        lines: A GeoDataFrame of lines.
+
+    Returns:
+        The GeoDataFrame with a new column "connected".
+
+    Examples
+    --------
+    >>> from sgis import read_parquet_url, get_largest_component
+    >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
+
+    >>> roads = get_largest_component(roads)
+    >>> roads.connected.value_counts()
+    1.0    85638
+    0.0     7757
+    Name: connected, dtype: int64
+    """
+    lines, _ = make_node_ids(lines)
+
+    edges = [
+        (str(source), str(target))
+        for source, target in zip(lines["source"], lines["target"], strict=True)
+    ]
+
+    graph = nx.Graph()
+    graph.add_edges_from(edges)
+
+    largest_component = max(nx.connected_components(graph), key=len)
+
+    largest_component_dict = {node_id: 1 for node_id in largest_component}
+
+    lines["connected"] = lines.source.map(largest_component_dict).fillna(0)
+
+    return lines
+
+
+def get_component_size(lines: GeoDataFrame) -> GeoDataFrame:
+    """Finds the size of each component in the network.
+
+    Takes a GeoDataFrame of linea and creates the column "component_size", which
+    indicates the size of the network component the line is a part of.
+
+    Args:
+        lines: a GeoDataFrame of lines.
+
+    Returns:
+        A GeoDataFrame with a new column "component_size".
+
+    Examples
+    --------
+    >>> from sgis import read_parquet_url, get_component_size
+    >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
+
+    >>> roads = get_component_size(roads)
+    >>> roads.component_size.value_counts().head()
+    79180    85638
+    2         1601
+    4          688
+    6          406
+    3          346
+    Name: component_size, dtype: int64
+    """
+    lines, _ = make_node_ids(lines)
+
+    edges = [
+        (str(source), str(target))
+        for source, target in zip(lines["source"], lines["target"], strict=True)
+    ]
+
+    graph = nx.Graph()
+    graph.add_edges_from(edges)
+    components = [list(x) for x in nx.connected_components(graph)]
+
+    componentsdict = {
+        idx: len(component) for component in components for idx in component
+    }
+
+    lines["component_size"] = lines.source.map(componentsdict)
+
+    return lines
+
+
+def split_lines_by_nearest_point(
+    lines: GeoDataFrame,
+    points: GeoDataFrame,
+    max_distance: int | None = None,
+) -> DataFrame:
+    """Split lines that are closest to s point.
+
+    Snaps points to nearest lines and splits the lines in two at the snap point.
+    The splitting is done pointwise, meaning each point splits one line in two.
+    The line will not be split if the point is closest to the endpoint of the line.
+
+    This function is used in NetworkAnalysis if split_lines is set to True.
+
+    Args:
+        lines: GeoDataFrame of lines that will be split.
+        points: GeoDataFrame of points to split the lines with.
+        max_distance: the maximum distance between the point and the line. Points further
+            away than max_distance will not split any lines. Defaults to None.
+
+    Returns:
+        A GeoDataFrame with the same columns as the input lines, but with the lines
+        split at the closest point to the points.
+
+    Raises:
+        ValueError: If the crs of the input data differs.
+
+    Examples
+    --------
+    >>> from sgis import read_parquet_url, split_lines_by_nearest_point
+    >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
+    >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
+    >>> rows = len(roads)
+    >>> rows
+    93395
+
+    Splitting lines for points closer than 10 meters from the lines.
+
+    >>> roads = split_lines_by_nearest_point(roads, points, max_distance=10)
+    >>> print("number of lines that were split:", len(roads) - rows)
+    number of lines that were split: 380
+
+    Splitting lines by all points.
+
+    >>> roads = split_lines_by_nearest_point(roads, points)
+    >>> print("number of lines that were split:", len(roads) - rows)
+    number of lines that were split: 848
+
+    Not all lines were split. That is because some points were closest to an endpoint
+    of a line.
+    """
+    BUFFDIST = 0.000001
+
+    if points.crs != lines.crs:
+        raise ValueError("crs mismatch:", points.crs, "and", lines.crs)
+
+    lines["temp_idx_"] = lines.index
+
+    # move the points to the nearest exact point of the line
+    if max_distance:
+        snapped = snap_within_distance(points, lines, max_distance=max_distance)
+    else:
+        snapped = snap_all(points, lines)
+
+    # find the lines that were snapped to (or are very close)
+    snapped_buff = buff(snapped, BUFFDIST)
+    intersect = lines.intersects(snapped_buff.unary_union)
+    relevant_lines = lines.loc[intersect]
+    the_other_lines = lines.loc[~intersect]
+
+    # need consistent coordinate dimensions later
+    # (doing it down here to not overwrite the original data)
+    relevant_lines.geometry = force_2d(relevant_lines.geometry)
+    snapped.geometry = force_2d(snapped.geometry)
+
+    # split the lines with buffer + difference, since shaply.split usually doesn't work
+    splitted = relevant_lines.overlay(snapped_buff, how="difference").explode(
+        ignore_index=True
+    )
+
+    # the endpoints of the new lines are now sligtly off. To get the exact snapped
+    # point coordinates, using get_k_nearest_neighbors. This will map the sligtly
+    # off line endpoints with the point the line was split by.
+
+    snapped["point_coords"] = [(geom.x, geom.y) for geom in snapped.geometry]
+
+    # get the endpoints of the lines as columns
+    splitted = make_edge_coords_cols(splitted)
+
+    splitted_source = to_gdf(splitted["source_coords"], crs=lines.crs)
+    splitted_target = to_gdf(splitted["target_coords"], crs=lines.crs)
+
+    # find the nearest snapped point for each source and target of the lines
+    snapped = snapped.set_index("point_coords")
+    dists_source = get_k_nearest_neighbors(splitted_source, snapped, k=1)
+    dists_target = get_k_nearest_neighbors(splitted_target, snapped, k=1)
+
+    dists_source = dists_source.loc[dists_source.distance <= BUFFDIST * 2]
+    dists_target = dists_target.loc[dists_target.distance <= BUFFDIST * 2]
+
+    pointmapper_source: pd.Series = dists_source["neighbor_index"]
+    pointmapper_target: pd.Series = dists_target["neighbor_index"]
+
+    # now, we can finally replace the source/target coordinate with the coordinates of
+    # the snapped points.
+
+    # loop for each line where the source is the endpoint that was split
+    # change the first point of the line to the point it was split by
+    for idx in dists_source.index:
+        line = splitted.loc[idx, "geometry"]
+        coordslist = list(line.coords)
+        coordslist[0] = pointmapper_source[idx]
+        splitted.loc[idx, "geometry"] = LineString(coordslist)
+
+    # same for the lines where the target was split, but change the last point of the
+    # line
+    for idx in dists_target.index:
+        line = splitted.loc[idx, "geometry"]
+        coordslist = list(line.coords)
+        coordslist[-1] = pointmapper_target[idx]
+        splitted.loc[idx, "geometry"] = LineString(coordslist)
+
+    splitted["splitted"] = 1
+
+    lines = pd.concat([the_other_lines, splitted], ignore_index=True).drop(
+        ["temp_idx_", "source_coords", "target_coords"], axis=1
+    )
+
+    return lines
+
+
+def cut_lines(gdf: GeoDataFrame, max_length: int, ignore_index=False) -> GeoDataFrame:
+    """Cuts lines of a GeoDataFrame into pieces of a given length.
+
+    Args:
+        gdf: GeoDataFrame.
+        max_length: The maximum length of the lines in the output GeoDataFrame.
+        ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
+            Defaults to False.
+
+    Returns:
+        A GeoDataFrame with lines cut to the maximum distance.
 
     Note:
-        The maximum zoom level only works on the OpenStreetMap background map.
+        This method is time consuming for large networks and low 'max_length'.
+
+    Examples
+    --------
+    >>> from sgis import read_parquet_url, cut_lines
+    >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
+    >>> roads.length.describe().round(1)
+    count    93395.0
+    mean        41.2
+    std         78.5
+    min          0.2
+    25%         14.0
+    50%         27.7
+    75%         47.5
+    max       5213.7
+    dtype: float64
+    >>> roads = cut_lines(roads, max_length=100)
+    >>> roads.length.describe().round(1)
+    count    126304.0
+    mean         30.5
+    std          30.1
+    min           0.0
+    25%           5.7
+    50%          22.5
+    75%          44.7
+    max         100.0
+    dtype: float64
     """
+    gdf["geometry"] = force_2d(gdf.geometry)
 
-    def __init__(
-        self,
-        *gdfs: GeoDataFrame,
-        column: str | None = None,
-        labels: tuple[str] | None = None,
-        popup: bool = True,
-        max_zoom: int = 30,
-        show_in_browser: bool = False,
-        **kwargs,
-    ) -> None:
-        """Takes the GeoDataFrames and mapping rules and prepares the mapmaking.
-
-        The maps are displayed with the methods explore, samplemap and clipmap.
-
-        Note:
-            The maximum zoom level only works on the OpenStreetMap background map.
-
-        Args:
-            *gdfs: one or more GeoDataFrames. Separated by a comma in the function call,
-                with no keyword.
-            column: The column to color the geometries by. Defaults to None, which means
-                each GeoDataFrame will get a unique color.
-            labels: By default, the GeoDataFrames will be labeled by their object names.
-                Alternatively, labels can be specified as a tuple of strings the same
-                length as the number of gdfs.
-            popup: If True (default), clicking on a geometry will create a popup box
-                with column names and values for the given geometry. The box stays
-                until clicking elsewhere. If False (the geopandas default), the box
-                will only show when hovering over the geometry.
-            max_zoom: The maximum allowed level of zoom. Higher number means more zoom
-                allowed. Defaults to 30, which is higher than the geopandas default.
-            show_in_browser: If False (default), the maps will be shown in Jupyter.
-                If True the maps will be opened in a browser folder.
-            **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
-                instance 'cmap' to change the colors, 'scheme' to change how the data
-                is grouped. This defaults to 'fisherjenks' for numeric data.
-        """
-        self.show_in_browser = show_in_browser
-        all_kwargs: dict = kwargs | {
-            "popup": popup,
-            "column": column,
-            "max_zoom": max_zoom,
-        }
-
-        gdfs, column, all_kwargs = _separate_args(gdfs, column, all_kwargs)
-
-        if not all(isinstance(gdf, GeoDataFrame) for gdf in gdfs):
-            raise ValueError("gdfs must be GeoDataFrames.")
-
-        if not any(len(gdf) for gdf in gdfs):
-            raise ValueError("None of the GeoDataFrames have rows.")
-
-        if "namedict" in all_kwargs:
-            for i, gdf in enumerate(gdfs):
-                gdf.name = all_kwargs["namedict"][i]
-            all_kwargs.pop("namedict")
-
-        # need to get the object names of the gdfs before copying
-        self.labels = labels
-        if not self.labels:
-            self._get_labels(gdfs)
-
-        self.gdfs: list[GeoDataFrame] = [gdf.copy() for gdf in gdfs]
-        self.kwargs = all_kwargs
-
-        # setting labels here to not get the column on the input gdfs
-        if not self.labels:
-            self._set_labels()
-
-        if not self.kwargs["column"]:
-            for gdf, label in zip(self.gdfs, self.labels, strict=True):
-                gdf["label"] = label
-            self.kwargs["column"] = "label"
-
-        # cannot have more than one geometry column. Also setting common crs
-        crss = list({gdf.crs for gdf in self.gdfs if gdf.crs is not None})
-        new_gdfs = []
-        for gdf in self.gdfs:
-            gdf = drop_inactive_geometry_columns(gdf).pipe(rename_geometry_if)
-            if crss:
-                try:
-                    gdf = gdf.to_crs(crss[0])
-                except ValueError:
-                    gdf = gdf.set_crs(crss[0])
-            new_gdfs.append(gdf)
-            self.gdfs = new_gdfs
-
-        self._is_categorical = self._check_if_categorical()
-        self._fill_missings()
-
-        self.gdf = pd.concat(self.gdfs, ignore_index=True)
-
-        self.kwargs["k"] = self.kwargs.get("k", 5)
-
-        if "title" not in self.kwargs:
-            self.kwargs["title"] = self.kwargs["column"]
-
-        if "categories" not in self.kwargs:
-            self._choose_cmap()
-
-        if self._is_categorical:
-            self._get_categorical_colors()
-
-        self.to_show: tuple[GeoDataFrame] = self.gdfs
-
-    def explore(self, column: str | None = None, **kwargs) -> None:
-        """Interactive map of the GeoDataFrames with layers that can be toggles on/off.
-
-        It displays all the GeoDataFrames and displays them together in an interactive
-        map with a common legend. The layers can be toggled on and off.
-
-        Args:
-            column: The column to color the geometries by. Defaults to the column
-                that was specified last.
-            **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
-                instance 'cmap' to change the colors, 'scheme' to change how the data
-                is grouped. This defaults to 'fisherjenks' for numeric data.
-
-        See also:
-            samplemap: same functionality, but shows only a random area of a given size.
-            clipmap: same functionality, but shows only the areas clipped by a given
-            mask.
-
-        Examples
-        --------
-        >>> from sgis import read_parquet_url
-        >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
-
-        Simple explore of two GeoDataFrames.
-
-        >>> from sgis import Explore
-        >>> ex = Explore(roads, points)
-        >>> ex.explore()
-
-        With column.
-
-        >>> roads["meters"] = roads.length
-        >>> points["meters"] = points.length
-        >>> ex = Explore(roads, points, column="meters")
-        >>> ex.samplemap()
-        """
-        if column:
-            kwargs["column"] = column
-        self.to_show = self.gdfs
-        self._explore(**kwargs)
-
-    def samplemap(
-        self,
-        size: int = 1000,
-        column: str | None = None,
-        sample_from_first: bool = True,
-        **kwargs,
-    ) -> None:
-        """Shows an interactive map of a random area of the GeoDataFrames.
-
-        It takes a random sample point of the GeoDataFrames, and shows all geometries
-        within a given radius of this point. Displays an interactive map with a common
-        legend. The layers can be toggled on and off.
-
-        The radius to plot can be changed with the 'size' parameter.
-
-        For more info about the labeling and coloring of the map, see the explore
-        method.
-
-        Args:
-            size: the radius to buffer the sample point by before clipping with the
-                data.
-            column: The column to color the geometries by. Defaults to the column
-                that was specified last.
-            sample_from_first: If True (default), the sample point is taken from
-                the first specified GeoDataFrame. If False, all GeoDataFrames are
-                considered.
-            **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
-                instance 'cmap' to change the colors, 'scheme' to change how the data
-                is grouped. This defaults to 'fisherjenks' for numeric data.
-
-        See also:
-            explore: same functionality, but shows the entire area of the geometries.
-            clipmap: same functionality, but shows only the areas clipped by a given
-            mask.
-        """
-        if column:
-            kwargs["column"] = column
-        self.previous_sample_count = 0
-        self.to_show = self.gdfs
+    gdf = gdf.explode(ignore_index=ignore_index, index_parts=False)
 
-        if sample_from_first:
-            sample = self.gdfs[0].sample(1)
-        else:
-            sample = self.gdf.sample(1)
+    long_lines = gdf.loc[gdf.length > max_length]
 
-        if get_geom_type(sample) == "polygon":
-            random_point = random_points_in_polygons(sample, 1)
-        else:
-            random_point = sample.centroid
+    if not len(long_lines):
+        return gdf
 
-        to_show: tuple[GeoDataFrame] = ()
-        for gdf in self.to_show:
-            gdf = gdf.clip(random_point.buffer(size))
-            to_show = to_show + (gdf,)
-        self.to_show = to_show
-        self._explore(**kwargs)
-
-    def clipmap(
-        self,
-        mask,
-        column: str | None = None,
-        **kwargs,
-    ) -> None:
-        """Shows an interactive map of a of the GeoDataFrames clipped by the mask.
-
-        It clips all the GeoDataFrames in the Explore instance to the mask extent,
-        and displays the resulting geometries in an interactive map with a common
-        legends. The layers can be toggled on and off.
-
-        For more info about the labeling and coloring of the map, see the explore
-        method.
-
-        Args:
-            mask: the geometry to clip the data by.
-            column: The column to color the geometries by. Defaults to the column
-                that was specified last.
-            **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
-                instance 'cmap' to change the colors, 'scheme' to change how the data
-                is grouped. This defaults to 'fisherjenks' for numeric data.
-
-        See also:
-            explore: same functionality, but shows the entire area of the geometries.
-            samplemap: same functionality, but shows only a random area of a given size.
-        """
-        if column:
-            kwargs["column"] = column
-        to_show: tuple[GeoDataFrame] = ()
-        for gdf in self.gdfs:
-            gdf = gdf.clip(mask)
-            to_show = to_show + (gdf,)
-        self.to_show = to_show
-        self._explore(**kwargs)
-
-    def _explore(self, **kwargs):
-        self.kwargs = self.kwargs | kwargs
-        self._is_categorical = self._check_if_categorical()
+    for x in [10, 5, 1]:
+        max_ = max(long_lines.length)
+        while max_ > max_length * x + 1:
+            max_ = max(long_lines.length)
+
+            long_lines = cut_lines_once(long_lines, max_length)
+
+            if max_ == max(long_lines.length):
+                break
+
+    long_lines = long_lines.explode(ignore_index=ignore_index, index_parts=False)
+
+    short_lines = gdf.loc[gdf.length <= max_length]
+
+    return pd.concat([short_lines, long_lines], ignore_index=ignore_index)
+
+
+def cut_lines_once(
+    lines: GeoDataFrame,
+    distances: int | float | str | Series,
+    ignore_index: bool = False,
+) -> GeoDataFrame:
+    """Cuts lines of a GeoDataFrame in two at the given distance or distances.
+
+    Takes a GeoDataFrame of lines and cuts each line in two. If distances is a number,
+    all lines will be cut at the same length.
+
+    Args:
+        gdf: GeoDataFrame.
+        distances: The distance from the start of the lines to cut at. Either a number,
+            the name of a column or array-like of same length as the line GeoDataFrame.
+        ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
+            Defaults to False.
+
+    Examples
+    --------
+    >>> from sgis import cut_lines_once, to_gdf
+    >>> import pandas as pd
+    >>> from shapely.geometry import LineString
+    >>> gdf = to_gdf(LineString([(0, 0), (1, 1), (2, 2)]))
+    >>> gdf = pd.concat([gdf, gdf, gdf])
+    >>> gdf
+                                                geometry
+    0  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...
+    0  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...
+    0  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...
+
+    Cut all lines at 1 unit from the start of the lines.
+
+    >>> cut_lines_once(gdf, 1)
+                                                geometry
+    0      LINESTRING (0.00000 0.00000, 0.70711 0.70711)
+    1  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...
+    2      LINESTRING (0.00000 0.00000, 0.70711 0.70711)
+    3  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...
+    4      LINESTRING (0.00000 0.00000, 0.70711 0.70711)
+    5  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...
+
+    Cut distance as column.
+
+    >>> gdf["dist"] = [1, 2, 3]
+    >>> cut_lines_once(gdf, "dist")
+                                                geometry  dist
+    0      LINESTRING (0.00000 0.00000, 0.70711 0.70711)     1
+    1  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...     1
+    2  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     2
+    3      LINESTRING (1.41421 1.41421, 2.00000 2.00000)     2
+    4  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     3
+
+    Cut distance as list (same result as above).
+
+    >>> cut_lines_once(gdf, [1, 2, 3])
+                                                geometry  dist
+    0      LINESTRING (0.00000 0.00000, 0.70711 0.70711)     1
+    1  LINESTRING (0.70711 0.70711, 1.00000 1.00000, ...     1
+    2  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     2
+    3      LINESTRING (1.41421 1.41421, 2.00000 2.00000)     2
+    4  LINESTRING (0.00000 0.00000, 1.00000 1.00000, ...     3
+    """
 
-        if self._is_categorical:
-            self._create_categorical_map()
-        else:
-            self._create_continous_map()
-        if self.show_in_browser:
-            self.map.show_in_browser()
-        else:
-            display(self.map)
+    def _cut(line: LineString, distance: int | float) -> list[LineString]:
+        """From the shapely docs"""
+        if distance <= 0.0 or distance >= line.length:
+            return line
+        coords = list(line.coords)
+        for i, p in enumerate(coords):
+            prd = line.project(Point(p))
+            if prd == distance:
+                return [LineString(coords[: i + 1]), LineString(coords[i:])]
+            if prd > distance:
+                cp = line.interpolate(distance)
+                return [
+                    LineString(coords[:i] + [(cp.x, cp.y)]),
+                    LineString([(cp.x, cp.y)] + coords[i:]),
+                ]
+
+    crs = lines.crs
+    geom_col = lines._geometry_column_name
+
+    lines = lines.copy()
+
+    # cutting lines will give lists of linestrings in the geometry column. Ignoring
+    # the warning it triggers
+    warnings.filterwarnings(
+        "ignore", message="Geometry column does not contain geometry."
+    )
 
-    def _get_labels(self, gdfs: tuple[GeoDataFrame]) -> None:
-        """Putting the labels/names in a list before copying the gdfs"""
-        self.labels: list[str] = []
-        for i, gdf in enumerate(gdfs):
-            if hasattr(gdf, "name"):
-                name = gdf.name
-            else:
-                name = get_name(gdf)
-                if not name:
-                    name = str(i)
-            self.labels.append(name)
-
-    def _set_labels(self) -> None:
-        """Setting the labels after copying the gdfs."""
-        for i, gdf in enumerate(self.gdfs):
-            gdf["label"] = self.labels[i]
-
-    def _fill_missings(self) -> None:
-        for gdf in self.gdfs:
-            if self.kwargs["column"] in gdf.columns:
-                continue
-            if self._is_categorical:
-                gdf[self.kwargs["column"]] = "missing"
-            else:
-                gdf[self.kwargs["column"]] = np.nan
-
-    def _check_if_categorical(self) -> bool:
-        """Quite messy this..."""
-        if not self.kwargs["column"]:
-            return True
-
-        maybe_area = 1 if "area" in self.kwargs["column"] else 0
-        maybe_length = (
-            1
-            if any(x in self.kwargs["column"] for x in ["meter", "metre", "leng"])
-            else 0
-        )
+    if isinstance(distances, str):
+        lines[geom_col] = np.vectorize(_cut)(lines[geom_col], lines[distances])
+    else:
+        lines[geom_col] = np.vectorize(_cut)(lines[geom_col], distances)
 
-        all_nan = 0
-        col_not_present = 0
-        for gdf in self.gdfs:
-            if self.kwargs["column"] not in gdf:
-                if maybe_area:
-                    gdf["area"] = gdf.area
-                    maybe_area += 1
-                elif maybe_length:
-                    gdf["length"] = gdf.length
-                    maybe_length += 1
-                else:
-                    col_not_present += 1
-            elif not pd.api.types.is_numeric_dtype(gdf[self.kwargs["column"]]):
-                if all(gdf[self.kwargs["column"]].isna()):
-                    all_nan += 1
-                return True
-
-        if maybe_area > 1:
-            self.kwargs["column"] = "area"
-            return False
-        if maybe_length > 1:
-            self.kwargs["column"] = "length"
-            return False
-
-        if all_nan == len(self.gdfs):
-            raise ValueError(f"All values are NaN in column {self.kwargs['column']!r}.")
-
-        if col_not_present == len(self.gdfs):
-            raise ValueError(f"{self.kwargs['column']} not found.")
-
-        return False
-
-    def _choose_cmap(self) -> None:
-        if "cmap" not in self.kwargs:
-            if self._is_categorical:
-                self.kwargs["cmap"] = None
-            else:
-                self.kwargs["cmap"] = "viridis"
-        if "scheme" not in self.kwargs:
-            self.kwargs["scheme"] = "fisherjenks"
-
-    def _get_categorical_colors(self) -> None:
-        cat_col = self.kwargs["column"]
-        self._unique_categories = sorted(
-            list(self.gdf.loc[self.gdf[cat_col] != "missing", cat_col].unique())
-        )
-        if len(self._unique_categories) <= len(_CATEGORICAL_CMAP):
-            self.kwargs["cmap"] = None
-            self._categories_colors_dict = {
-                category: _CATEGORICAL_CMAP[i]
-                for i, category in enumerate(self._unique_categories)
-            }
-        else:
-            cmap = matplotlib.colormaps.get_cmap("tab20")
+    # explode will give pandas df if not gdf is constructed
+    lines = GeoDataFrame(
+        lines.explode(ignore_index=ignore_index, index_parts=False),
+        geometry=geom_col,
+        crs=crs,
+    )
+
+    return lines
+
+
+def make_node_ids(
+    lines: GeoDataFrame,
+    wkt: bool = True,
+) -> tuple[GeoDataFrame, GeoDataFrame]:
+    """Gives the lines unique node ids and returns lines (edges) and nodes.
+
+    Takes the first and last point of each line and creates a GeoDataFrame of
+    nodes (points) with a column 'node_id'. The node ids are then assigned to the
+    input GeoDataFrame of lines as the columns 'source' and 'target'.
+
+    Args:
+        lines: GeoDataFrame with line geometries
+        wkt: If True (default), the resulting nodes will include the column 'wkt',
+            containing the well-known text representation of the geometry. If False, it
+            will include the column 'coords', a tuple with x and y geometries.
+
+    Returns:
+        A tuple of two GeoDataFrames, one with the lines and one with the nodes.
+
+    Note:
+        The lines must be singlepart linestrings.
+    """
+    if wkt:
+        lines = make_edge_wkt_cols(lines)
+        geomcol1, geomcol2, geomcol_final = "source_wkt", "target_wkt", "wkt"
+    else:
+        lines = make_edge_coords_cols(lines)
+        geomcol1, geomcol2, geomcol_final = "source_coords", "target_coords", "coords"
 
-            self._categories_colors_dict = {
-                category: colors.to_hex(cmap(int(i)))
-                for i, category in enumerate(self._unique_categories)
-            }
-
-        if any(self.gdf[self.kwargs["column"]].isna()) or any(
-            self.gdf[self.kwargs["column"]] == "missing"
-        ):
-            self._categories_colors_dict["missing"] = NAN_COLOR
+    # remove identical lines in opposite directions
+    lines["meters_"] = lines.length.astype(str)
 
-        for gdf in self.gdfs:
-            gdf["color"] = gdf[self.kwargs["column"]].map(self._categories_colors_dict)
+    sources = lines[[geomcol1, geomcol2, "meters_"]].rename(
+        columns={geomcol1: geomcol_final, geomcol2: "temp"}
+    )
+    targets = lines[[geomcol1, geomcol2, "meters_"]].rename(
+        columns={geomcol2: geomcol_final, geomcol1: "temp"}
+    )
+
+    nodes = (
+        pd.concat([sources, targets], axis=0, ignore_index=True)
+        .drop_duplicates([geomcol_final, "temp", "meters_"])
+        .drop("meters_", axis=1)
+    )
+
+    lines = lines.drop("meters_", axis=1)
+
+    nodes["n"] = nodes.assign(n=1).groupby(geomcol_final)["n"].transform("sum")
+
+    nodes = nodes.drop_duplicates(subset=[geomcol_final]).reset_index(drop=True)
+
+    nodes["node_id"] = nodes.index
+    nodes["node_id"] = nodes["node_id"].astype(str)
+
+    id_dict = {
+        geom: node_id
+        for geom, node_id in zip(nodes[geomcol_final], nodes["node_id"], strict=True)
+    }
+    lines["source"] = lines[geomcol1].map(id_dict)
+    lines["target"] = lines[geomcol2].map(id_dict)
+
+    n_dict = {geom: n for geom, n in zip(nodes[geomcol_final], nodes["n"], strict=True)}
+    lines["n_source"] = lines[geomcol1].map(n_dict)
+    lines["n_target"] = lines[geomcol2].map(n_dict)
 
-        self.gdf["color"] = self.gdf[self.kwargs["column"]].map(
-            self._categories_colors_dict
+    if wkt:
+        nodes["geometry"] = gpd.GeoSeries.from_wkt(nodes[geomcol_final], crs=lines.crs)
+    else:
+        nodes["geometry"] = GeoSeries(
+            [Point(geom) for geom in nodes[geomcol_final]], crs=lines.crs
         )
+    nodes = gpd.GeoDataFrame(nodes, geometry="geometry", crs=lines.crs)
+    nodes = nodes.reset_index(drop=True)
 
-    def _create_categorical_map(self):
-        gdfs = pd.concat(self.to_show, ignore_index=True)
+    lines = _push_geom_col(lines)
 
-        self.map = self._explore_return(gdfs, return_="empty_map", **self.kwargs)
+    return lines, nodes
 
-        for gdf, label in zip(self.to_show, self.labels, strict=True):
-            if not len(gdf):
-                continue
-            f = folium.FeatureGroup(name=label)
-
-            gjs = self._explore_return(
-                gdf,
-                color=gdf["color"],
-                return_="geojson",
-                tooltip=self._tooltip_cols(gdf),
-                **{
-                    key: value
-                    for key, value in self.kwargs.items()
-                    if key not in ["title", "cmap"]
-                },
-            )
-            f.add_child(gjs)
-            self.map.add_child(f)
-        _categorical_legend(
-            self.map,
-            self.kwargs["title"],
-            self._categories_colors_dict.keys(),
-            self._categories_colors_dict.values(),
+
+def make_edge_coords_cols(lines: GeoDataFrame) -> GeoDataFrame:
+    """Get the wkt of the first and last points of lines as columns.
+
+    It takes a GeoDataFrame of LineStrings and returns a GeoDataFrame with two new
+    columns, source_coords and target_coords, which are the x and y coordinates of the
+    first and last points of the LineStrings in a tuple. The lines all have to be
+
+    Args:
+        lines (GeoDataFrame): the GeoDataFrame with the lines
+
+    Returns:
+        A GeoDataFrame with new columns 'source_coords' and 'target_coords'
+    """
+    try:
+        lines, endpoints = _prepare_make_edge_cols_simple(lines)
+    except ValueError:
+        lines, endpoints = _prepare_make_edge_cols(lines)
+
+    coords = [(geom.x, geom.y) for geom in endpoints.geometry]
+    lines["source_coords"], lines["target_coords"] = (
+        coords[0::2],
+        coords[1::2],
+    )
+
+    return lines
+
+
+def make_edge_wkt_cols(lines: GeoDataFrame) -> GeoDataFrame:
+    """Get coordinate tuples of the first and last points of lines as columns.
+
+    It takes a GeoDataFrame of LineStrings and returns a GeoDataFrame with two new
+    columns, source_wkt and target_wkt, which are the WKT representations of the first
+    and last points of the LineStrings
+
+    Args:
+        lines (GeoDataFrame): the GeoDataFrame with the lines
+
+    Returns:
+        A GeoDataFrame with new columns 'source_wkt' and 'target_wkt'
+    """
+    try:
+        lines, endpoints = _prepare_make_edge_cols_simple(lines)
+    except ValueError:
+        lines, endpoints = _prepare_make_edge_cols(lines)
+
+    wkt_geom = [
+        f"POINT ({x} {y})" for x, y in zip(endpoints.x, endpoints.y, strict=True)
+    ]
+    lines["source_wkt"], lines["target_wkt"] = (
+        wkt_geom[0::2],
+        wkt_geom[1::2],
+    )
+
+    return lines
+
+
+def close_network_holes(
+    lines: GeoDataFrame,
+    max_distance: int | float,
+    max_angle: int,
+    hole_col: str | None = "hole",
+):
+    """Fills network gaps with straigt lines.
+
+    Fills holes in the network by connecting deadends with the nodes that are
+    within the 'max_distance' distance.
+
+    Args:
+        lines: GeoDataFrame with lines.
+        max_distance: The maximum distance for the holes to be filled.
+        max_angle: Absolute number between 0 and 180 that represents the maximum
+            difference in angle between the new line and the prior, i.e. the line
+            at which the deadend terminates. A value of 0 means the new lines must
+            have the exact same angle as the prior line, and 180 means the new
+            lines can go in any direction.
+        hole_col: If you want to keep track of which lines were added, you can add a
+            column with a value of 1. Defaults to 'hole'
+
+    Returns:
+        The input GeoDataFrame with new lines added.
+
+    Examples
+    --------
+    Read road data with small gaps.
+
+    >>> import sgis as sg
+    >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
+
+    Roads need to be singlepart linestrings for this to work.
+
+    >>> from shapely import line_merge
+    >>> roads.geometry = line_merge(roads.geometry)
+
+    Fill gaps shorter than 1.1 meters.
+
+    >>> filled = sg.close_network_holes(roads, max_distance=1.1, max_angle=180)
+    >>> filled.hole.value_counts()
+    Name: connected, dtype: int64
+    0    93395
+    1     7102
+    Name: hole, dtype: int64
+
+    Compare the number of isolated lines before and after.
+
+    >>> roads = sg.get_largest_component(roads)
+    >>> roads.connected.value_counts()
+    1.0    85638
+    0.0     7757
+    Name: connected, dtype: int64
+
+    >>> filled = sg.get_largest_component(filled)
+    >>> filled.connected.value_counts()
+    1.0    100315
+    0.0       180
+    Name: connected, dtype: int64
+
+    Fill only gaps with an angle deviation between 0 and 30 compared to the prior line.
+
+    >>> filled = sg.close_network_holes(roads, max_distance=1.1, max_angle=30)
+    >>> filled.hole.value_counts()
+    0    93395
+    1     7092
+    Name: hole, dtype: int64
+
+    It's not always wise to fill gaps. In the case of this data, these small gaps are
+    intentional. They are road blocks where most cars aren't allowed to pass. Fill the
+    holes only if it makes the travel times/routes more realistic.
+    """
+    lines, nodes = make_node_ids(lines)
+
+    new_lines = _find_holes_all_lines(
+        lines,
+        nodes,
+        max_distance,
+        max_angle=max_angle,
+    )
+
+    if not len(new_lines):
+        lines[hole_col] = (
+            0 if hole_col not in lines.columns else lines[hole_col].fillna(0)
+        )
+        return lines
+
+    new_lines = make_edge_wkt_cols(new_lines)
+
+    wkt_id_dict = {
+        wkt: id for wkt, id in zip(nodes["wkt"], nodes["node_id"], strict=True)
+    }
+    new_lines["source"] = new_lines["source_wkt"].map(wkt_id_dict)
+    new_lines["target"] = new_lines["target_wkt"].map(wkt_id_dict)
+
+    if hole_col:
+        new_lines[hole_col] = 1
+        lines[hole_col] = (
+            0 if hole_col not in lines.columns else lines[hole_col].fillna(0)
         )
-        folium.TileLayer("stamentoner").add_to(self.map)
-        folium.TileLayer("cartodbdark_matter").add_to(self.map)
-        self.map.add_child(folium.LayerControl())
 
-    def _create_continous_map(self):
-        gdfs = pd.concat(self.to_show, ignore_index=True)
+    return pd.concat([lines, new_lines], ignore_index=True)
+
+
+def close_network_holes_to_deadends(
+    lines: GeoDataFrame,
+    max_distance: int | float,
+    hole_col: str | None = "hole",
+):
+    """Fills gaps between two deadends if the distance is less than 'max_distance'.
+
+    Fills holes between deadends in the network with straight lines if the distance is
+    less than 'max_distance'.
 
-        unique_bins = self._create_bins(
-            gdfs, self.kwargs["column"], self.kwargs["scheme"]
+    Args:
+        lines: GeoDataFrame with lines
+        max_distance: The maximum distance between two nodes to be considered a hole.
+        hole_col: If you want to keep track of which lines were added, you can add a
+            column with a value of 1. Defaults to 'hole'
+
+    Returns:
+        The input GeoDataFrame with new lines added.
+
+    Examples
+    --------
+    Read road data with small gaps.
+
+    >>> import sgis as sg
+    >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
+
+    Roads need to be singlepart linestrings for this to work.
+
+    >>> from shapely import line_merge
+    >>> roads.geometry = line_merge(roads.geometry)
+
+    Check for number of isolated lines now.
+
+    >>> roads = sg.get_largest_component(roads)
+    >>> roads.connected.value_counts()
+    1.0    85638
+    0.0     7757
+    Name: connected, dtype: int64
+
+    Fill gaps shorter than 1.1 meters.
+
+    >>> filled = sg.close_network_holes_to_deadends(roads, max_distance=1.1, max_angle=30)
+    >>> roads = sg.get_largest_component(roads)
+    >>> roads.connected.value_counts()
+    1.0    100315
+    0.0       180
+    Name: connected, dtype: int64
+
+    It's not always wise to fill gaps. In the case of this data, these small gaps are
+    intentional. They are road blocks where most cars aren't allowed to pass. Fill the
+    holes only if it makes the travel times/routes more realistic.
+    """
+    lines, nodes = make_node_ids(lines)
+
+    new_lines = _find_holes_deadends(nodes, max_distance)
+
+    if not len(new_lines):
+        lines[hole_col] = (
+            0 if hole_col not in lines.columns else lines[hole_col].fillna(0)
         )
+        return lines
 
-        self.kwargs["classification_kwds"] = {"bins": unique_bins}
-        if len(unique_bins) < self.kwargs.get("k", 5):
-            self.kwargs["k"] = len(unique_bins)
+    new_lines = make_edge_wkt_cols(new_lines)
 
-        self.map, colorbar = self._explore_return(
-            gdfs, return_="empty_map_and_colorbar", **self.kwargs
+    wkt_id_dict = {
+        wkt: id for wkt, id in zip(nodes["wkt"], nodes["node_id"], strict=True)
+    }
+    new_lines["source"] = new_lines["source_wkt"].map(wkt_id_dict)
+    new_lines["target"] = new_lines["target_wkt"].map(wkt_id_dict)
+
+    if hole_col:
+        new_lines[hole_col] = 1
+        lines[hole_col] = (
+            0 if hole_col not in lines.columns else lines[hole_col].fillna(0)
         )
 
-        for gdf, label in zip(self.to_show, self.labels, strict=True):
-            if not len(gdf):
-                continue
-            f = folium.FeatureGroup(name=label)
-
-            gjs = self._explore_return(
-                gdf,
-                tooltip=self._tooltip_cols(gdf),
-                return_="geojson",
-                **{key: value for key, value in self.kwargs.items() if key != "title"},
-            )
-            f.add_child(gjs)
-            self.map.add_child(f)
+    return pd.concat([lines, new_lines], ignore_index=True)
+
+
+def _find_holes_all_lines(
+    lines: GeoDataFrame,
+    nodes: GeoDataFrame,
+    max_distance: int,
+    max_angle: int = 90,
+):
+    """Creates lines between deadends and closest node.
+
+    Creates lines if distance is less than max_distance and angle less than max_angle.
+
+    wkt: well-known text, e.g. "POINT (60 10)"
+    """
+    k = 50 if len(nodes) >= 50 else len(nodes)
+    crs = nodes.crs
+
+    # remove duplicates of lines going both directions
+    lines["sorted"] = [
+        "_".join(sorted([s, t]))
+        for s, t in zip(lines["source"], lines["target"], strict=True)
+    ]
 
-        self.map.add_child(colorbar)
-        folium.TileLayer("stamentoner").add_to(self.map)
-        folium.TileLayer("cartodbdark_matter").add_to(self.map)
-        self.map.add_child(folium.LayerControl())
-
-    def _tooltip_cols(self, gdf: GeoDataFrame) -> list:
-        if "tooltip" in self.kwargs:
-            tooltip = self.kwargs.pop("tooltip")
-            return tooltip
-        return [col for col in gdf.columns if col not in COLS_TO_DROP]
-
-    def _create_bins(self, gdf, column, scheme):
-        n_unique = len(gdf[column].unique())
-
-        if n_unique <= self.kwargs.get("k", 5):
-            self.kwargs["k"] = n_unique
-
-        binning = classify(
-            np.asarray(gdf.loc[gdf[column].notna(), column]),
-            scheme=scheme,
-            k=self.kwargs["k"],
+    no_dups = lines.drop_duplicates("sorted")
+
+    no_dups, nodes = make_node_ids(no_dups)
+
+    # make point gdf for the deadends and the other endpoint of the deadend lines
+    deadends_target = no_dups.loc[no_dups.n_target == 1].rename(
+        columns={"target_wkt": "wkt", "source_wkt": "wkt_other_end"}
+    )
+    deadends_source = no_dups.loc[no_dups.n_source == 1].rename(
+        columns={"source_wkt": "wkt", "target_wkt": "wkt_other_end"}
+    )
+    deadends = pd.concat([deadends_source, deadends_target], ignore_index=True)
+
+    if len(deadends) <= 1:
+        return []
+
+    deadends_other_end = deadends.copy()
+    deadends_other_end["geometry"] = gpd.GeoSeries.from_wkt(
+        deadends_other_end["wkt_other_end"], crs=crs
+    )
+
+    deadends["geometry"] = gpd.GeoSeries.from_wkt(deadends["wkt"], crs=crs)
+
+    deadends_array = coordinate_array(deadends)
+    nodes_array = coordinate_array(nodes)
+
+    all_dists, all_indices = k_nearest_neighbors(deadends_array, nodes_array, k=k)
+
+    deadends_other_end_array = coordinate_array(deadends_other_end)
+
+    def get_angle(array_a, array_b):
+        dx = array_b[:, 0] - array_a[:, 0]
+        dy = array_b[:, 1] - array_a[:, 1]
+
+        angles_rad = np.arctan2(dx, dy)
+        angles_degrees = np.degrees(angles_rad)
+        return angles_degrees
+
+    # now to find the lines that have the correct angle and distance
+    # and endpoints of the new lines in lists, looping through the k neighbour points
+    new_sources: list[str] = []
+    new_targets: list[str] = []
+    for i in np.arange(1, k):
+        # to break out of the loop if no new_targets that meet the condition are found
+        len_now = len(new_sources)
+
+        # selecting the arrays for the current k neighbour
+        indices = all_indices[:, i]
+        dists = all_dists[:, i]
+
+        these_nodes_array = coordinate_array(nodes.loc[indices])
+
+        if np.all(deadends_other_end_array == these_nodes_array):
+            continue
+
+        angles_deadend_to_node = get_angle(deadends_array, these_nodes_array)
+
+        angles_deadend_to_deadend_other_end = get_angle(
+            deadends_other_end_array, deadends_array
         )
 
-        unique_bins = list({round(bin, 5) for bin in binning.bins})
-        unique_bins.sort()
+        angles_difference = np.abs(
+            np.abs(angles_deadend_to_deadend_other_end) - np.abs(angles_deadend_to_node)
+        )
 
-        # adding a small amount to get the colors correct. Weird that this is
-        # nessecary...
-        return [bin + bin / 10_000 for bin in unique_bins]
-
-    @staticmethod
-    def _get_continous_color_idx(gdf, column, bins):
-        gdf.loc[gdf[column] < bins[0], "color_idx"] = 0
-        for i, (prev_bin, this_bin) in enumerate(zip(bins[:-1], bins[1:], strict=True)):
-            gdf.loc[
-                (gdf[column] >= prev_bin) & (gdf[column] < this_bin), "color_idx"
-            ] = i
+        angles_difference[
+            np.all(deadends_other_end_array == these_nodes_array, axis=1)
+        ] = np.nan
 
-        return gdf
+        condition = (dists <= max_distance) & (angles_difference <= max_angle)
 
-    def _explore_return(
-        self,
-        df,
-        return_: str,
-        column=None,
-        cmap=None,
-        color=None,
-        m=None,
-        tiles="OpenStreetMap",
-        attr=None,
-        tooltip=True,
-        popup=False,
-        highlight=True,
-        legend=True,
-        scheme=None,
-        k=5,
-        vmin=None,
-        vmax=None,
-        width="100%",
-        height="100%",
-        categories=None,
-        classification_kwds=None,
-        control_scale=True,
-        marker_type=None,
-        marker_kwds={},
-        style_kwds={},
-        highlight_kwds={},
-        missing_kwds={},
-        tooltip_kwds={},
-        popup_kwds={},
-        legend_kwds={},
-        map_kwds={},
-        **kwargs,
-    ):
-        """Contains the nessecary parts of the geopandas _explore function.
-
-        Also has a return_ parameter that controls what is returned. This should be
-        replaced by separate functions, and irrelevant parameters should be removed.
-        """
-        # xyservices is an optional dependency
-        try:
-            import xyzservices
-
-            has_xyzservices = True
-        except ImportError:
-            has_xyzservices = False
-
-        gdf = df.copy()
-
-        # convert LinearRing to LineString
-        rings_mask = df.geom_type == "LinearRing"
-        if rings_mask.any():
-            gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
-                lambda g: LineString(g)
-            )
+        from_wkt = deadends.loc[condition, "wkt"]
+        to_idx = indices[condition]
+        to_wkt = nodes.loc[to_idx, "wkt"]
 
-        if gdf.crs is None:
-            kwargs["crs"] = "Simple"
-            tiles = None
-        elif not gdf.crs.equals(4326):
-            gdf = gdf.to_crs(4326)
-
-        # create folium.Map object
-        if m is None:
-            # Get bounds to specify location and map extent
-            bounds = gdf.total_bounds
-            location = kwargs.pop("location", None)
-            if location is None:
-                x = mean([bounds[0], bounds[2]])
-                y = mean([bounds[1], bounds[3]])
-                location = (y, x)
-                if "zoom_start" in kwargs.keys():
-                    fit = False
-                else:
-                    fit = True
-            else:
-                fit = False
-
-            # get a subset of kwargs to be passed to folium.Map
-            for i in _MAP_KWARGS:
-                if i in map_kwds:
-                    raise ValueError(
-                        f"'{i}' cannot be specified in 'map_kwds'. "
-                        f"Use the '{i}={map_kwds[i]}' argument instead."
-                    )
-            map_kwds = {
-                **map_kwds,
-                **{i: kwargs[i] for i in kwargs.keys() if i in _MAP_KWARGS},
-            }
-
-            if has_xyzservices:
-                # match provider name string to xyzservices.TileProvider
-                if isinstance(tiles, str):
-                    try:
-                        tiles = xyzservices.providers.query_name(tiles)
-                    except ValueError:
-                        pass
-
-                if isinstance(tiles, xyzservices.TileProvider):
-                    attr = attr if attr else tiles.html_attribution
-                    map_kwds["min_zoom"] = tiles.get("min_zoom", 0)
-                    map_kwds["max_zoom"] = tiles.get("max_zoom", 18)
-                    tiles = tiles.build_url(scale_factor="{r}")
-
-            m = folium.Map(
-                location=location,
-                control_scale=control_scale,
-                tiles=tiles,
-                attr=attr,
-                width=width,
-                height=height,
-                **map_kwds,
-            )
+        # now add the wkts to the lists of new sources and targets. If the source
+        # is already added, the new wks will not be added again
+        new_targets = new_targets + [
+            t for f, t in zip(from_wkt, to_wkt, strict=True) if f not in new_sources
+        ]
+        new_sources = new_sources + [
+            f for f, _ in zip(from_wkt, to_wkt, strict=True) if f not in new_sources
+        ]
 
-            # fit bounds to get a proper zoom level
-            if fit:
-                m.fit_bounds([[bounds[1], bounds[0]], [bounds[3], bounds[2]]])
-
-        for map_kwd in _MAP_KWARGS:
-            kwargs.pop(map_kwd, None)
-
-        if pd.api.types.is_list_like(column):
-            if len(column) != gdf.shape[0]:
-                raise ValueError(
-                    "The GeoDataFrame and given column have different number of rows."
-                )
-            else:
-                column_name = "__plottable_column"
-                gdf[column_name] = column
-                column = column_name
-        elif pd.api.types.is_categorical_dtype(gdf[column]):
-            if categories is not None:
-                raise ValueError(
-                    "Cannot specify 'categories' when column has categorical dtype"
-                )
-
-        nan_idx = pd.isna(gdf[column])
-
-        if not self._is_categorical:
-            vmin = gdf[column].min() if vmin is None else vmin
-            vmax = gdf[column].max() if vmax is None else vmax
-
-            if len(gdf[column][~nan_idx]):
-                bins = classification_kwds["bins"]
-
-                binning = classify(
-                    np.asarray(gdf[column][~nan_idx]),
-                    "UserDefined",
-                    bins=bins,
-                    k=k,
-                )
-
-                color = np.apply_along_axis(
-                    colors.to_hex,
-                    1,
-                    cm.get_cmap(cmap, k)(binning.yb),  # ! changed 256 to k
-                )
-            else:
-                color = NAN_COLOR
-
-        # set default style
-        if "fillOpacity" not in style_kwds:
-            style_kwds["fillOpacity"] = 0.5
-        if "weight" not in style_kwds:
-            style_kwds["weight"] = 2
-        if "style_function" in style_kwds:
-            style_kwds_function = style_kwds["style_function"]
-            if not callable(style_kwds_function):
-                raise ValueError("'style_function' has to be a callable")
-            style_kwds.pop("style_function")
-        else:
+        # break out of the loop when no new new_targets meet the condition
+        if len_now == len(new_sources):
+            break
 
-            def _no_style(x):
-                return {}
+    # make GeoDataFrame with straight lines
+    new_sources = gpd.GeoSeries.from_wkt(new_sources, crs=crs)
+    new_targets = gpd.GeoSeries.from_wkt(new_targets, crs=crs)
+    new_lines = shortest_line(new_sources, new_targets)
+    new_lines = gpd.GeoDataFrame({"geometry": new_lines}, geometry="geometry", crs=crs)
 
-            style_kwds_function = _no_style
+    if not len(new_lines):
+        return new_lines
 
-        # specify color
-        if color is not None:
-            if (
-                isinstance(color, str)
-                and isinstance(gdf, geopandas.GeoDataFrame)
-                and color in gdf.columns
-            ):  # use existing column
-
-                def _style_color(x):
-                    base_style = {
-                        "fillColor": x["properties"][color],
-                        **style_kwds,
-                    }
-                    return {
-                        **base_style,
-                        **style_kwds_function(x),
-                    }
-
-                style_function = _style_color
-            else:  # assign new column
-                if isinstance(gdf, GeoSeries):
-                    gdf = GeoDataFrame(geometry=gdf)
-
-                if nan_idx is not None and nan_idx.any():
-                    nan_color = missing_kwds.pop("color", NAN_COLOR)
-
-                    gdf["__folium_color"] = nan_color
-                    gdf.loc[~nan_idx, "__folium_color"] = color
-                else:
-                    gdf["__folium_color"] = color
-
-                stroke_color = style_kwds.pop("color", None)
-                if not stroke_color:
-
-                    def _style_column(x):
-                        base_style = {
-                            "fillColor": x["properties"]["__folium_color"],
-                            "color": x["properties"]["__folium_color"],
-                            **style_kwds,
-                        }
-                        return {
-                            **base_style,
-                            **style_kwds_function(x),
-                        }
-
-                    style_function = _style_column
-                else:
-
-                    def _style_stroke(x):
-                        base_style = {
-                            "fillColor": x["properties"]["__folium_color"],
-                            "color": stroke_color,
-                            **style_kwds,
-                        }
-                        return {
-                            **base_style,
-                            **style_kwds_function(x),
-                        }
-
-                    style_function = _style_stroke
-        else:  # use folium default
-
-            def _style_default(x):
-                return {**style_kwds, **style_kwds_function(x)}
-
-            style_function = _style_default
-
-        if highlight:
-            if "fillOpacity" not in highlight_kwds:
-                highlight_kwds["fillOpacity"] = 0.75
+    new_lines = make_edge_wkt_cols(new_lines)
 
-            def _style_highlight(x):
-                return {**highlight_kwds}
+    return new_lines
 
-            highlight_function = _style_highlight
-        else:
-            highlight_function = None
 
-        # define default for points
-        if marker_type is None:
-            marker_type = "circle_marker"
-
-        marker = marker_type
-        if isinstance(marker_type, str):
-            if marker_type == "marker":
-                marker = folium.Marker(**marker_kwds)
-            elif marker_type == "circle":
-                marker = folium.Circle(**marker_kwds)
-            elif marker_type == "circle_marker":
-                marker_kwds["radius"] = marker_kwds.get("radius", 2)
-                marker_kwds["fill"] = marker_kwds.get("fill", True)
-                marker = folium.CircleMarker(**marker_kwds)
-            else:
-                raise ValueError(
-                    "Only 'marker', 'circle', and 'circle_marker' are "
-                    "supported as marker values"
-                )
-
-        # remove additional geometries
-        if isinstance(gdf, GeoDataFrame):
-            non_active_geoms = [
-                name
-                for name, val in (gdf.dtypes == "geometry").items()
-                if val and name != gdf.geometry.name
-            ]
-            gdf = gdf.drop(columns=non_active_geoms)
-
-        gdf = clean_geoms(gdf)
-
-        # prepare tooltip and popup
-        if isinstance(gdf, GeoDataFrame):
-            # add named index to the tooltip
-            if gdf.index.name is not None:
-                gdf = gdf.reset_index()
-            # specify fields to show in the tooltip
-            tooltip = _tooltip_popup("tooltip", tooltip, gdf, **tooltip_kwds)
-            popup = _tooltip_popup("popup", popup, gdf, **popup_kwds)
-        else:
-            tooltip = None
-            popup = None
+def _find_holes_deadends(nodes: GeoDataFrame, max_distance: float | int):
+    """Creates lines between two deadends if between max_distance and min_dist.
+
+    It takes a GeoDataFrame of nodes, chooses the deadends, and creates a straight line
+    between the closest deadends if the distance is no greater than 'max_distance'.
+
+    Args:
+        nodes: the nodes of the network
+        max_distance: The maximum distance between two nodes to be connected.
+
+    Returns:
+        A GeoDataFrame with the new lines.
+    """
+    crs = nodes.crs
+
+    # deadends are nodes that appear only once
+    deadends = nodes[nodes["n"] == 1]
+
+    # have to reset index to be able to integrate with numpy/scikit-learn
+    deadends = deadends.reset_index(drop=True)
+
+    if len(deadends) <= 1:
+        return []
 
-        if "geojson" in return_:
-            # add dataframe to map
-            gjs = folium.GeoJson(
-                gdf.__geo_interface__,
-                tooltip=tooltip,
-                popup=popup,
-                marker=marker,
-                style_function=style_function,
-                highlight_function=highlight_function,
-                **kwargs,
+    deadends_array = coordinate_array(deadends)
+
+    dists, indices = k_nearest_neighbors(deadends_array, deadends_array, k=2)
+
+    # choose the second column (the closest neighbour)
+    dists = dists[:, 1]
+    indices = indices[:, 1]
+
+    # get the geometry of the distances no greater than max_distance
+    # the from geometries can be taken directly from the deadends index,
+    # since 'dists' has the same index. 'to_geom' must be selected through the index
+    # of the neighbours ('indices')
+    condition = dists < max_distance
+    from_geom = deadends.loc[condition, "geometry"].reset_index(drop=True)
+    to_idx = indices[condition]
+    to_geom = deadends.loc[to_idx, "geometry"].reset_index(drop=True)
+
+    # GeoDataFrame with straight lines
+    new_lines = shortest_line(from_geom, to_geom)
+    new_lines = gpd.GeoDataFrame({"geometry": new_lines}, geometry="geometry", crs=crs)
+
+    if not len(new_lines):
+        return new_lines
+
+    return new_lines
+
+
+def _prepare_make_edge_cols(
+    lines: GeoDataFrame,
+) -> tuple[GeoDataFrame, GeoDataFrame]:
+    lines = lines.loc[lines.geom_type != "LinearRing"]
+
+    if not all(lines.geom_type == "LineString"):
+        multilinestring_error_message = (
+            "MultiLineStrings have more than two endpoints. "
+            "Try shapely.line_merge and/or explode() to get LineStrings. "
+            "Or use the Network class methods, where the lines are prepared correctly."
+        )
+        if any(lines.geom_type == "MultiLinestring"):
+            raise ValueError(multilinestring_error_message)
+        else:
+            raise ValueError(
+                "You have mixed geometries. Only lines are accepted. "
+                "Try using: to_single_geom_type(gdf, 'lines')."
             )
-            return gjs
 
-        if legend and not self._is_categorical:
-            # NOTE: overlaps will be resolved in branca #88
-            caption = column if column != "__plottable_column" else ""
-            caption = legend_kwds.pop("caption", caption)
-            if column is not None:
-                cbar = legend_kwds.pop("colorbar", True)
-                colormap_kwds = {}
-                if "max_labels" in legend_kwds:
-                    colormap_kwds["max_labels"] = legend_kwds.pop("max_labels")
-                if scheme and len(gdf[column][~nan_idx]):
-                    cb_colors = np.apply_along_axis(
-                        colors.to_hex, 1, cm.get_cmap(cmap, binning.k)(range(binning.k))
-                    )
-                    if cbar:
-                        if legend_kwds.pop("scale", True):
-                            index = [vmin] + binning.bins.tolist()
-                        else:
-                            index = None
-                        colorbar = bc.colormap.StepColormap(
-                            cb_colors,
-                            vmin=vmin,
-                            vmax=vmax,
-                            caption=caption,
-                            index=index,
-                            **colormap_kwds,
-                        )
-                    else:
-                        fmt = legend_kwds.pop("fmt", "{:.2f}")
-                        if "labels" in legend_kwds:
-                            categories = legend_kwds["labels"]
-                        else:
-                            categories = binning.get_legend_classes(fmt)
-                            show_interval = legend_kwds.pop("interval", False)
-                            if not show_interval:
-                                categories = [c[1:-1] for c in categories]
-
-                        if nan_idx.any() and nan_color:
-                            categories.append(missing_kwds.pop("label", "NaN"))
-                            cb_colors = np.append(cb_colors, nan_color)
-
-                else:
-                    if isinstance(cmap, bc.colormap.ColorMap):
-                        colorbar = cmap
-                    else:
-                        mp_cmap = cm.get_cmap(cmap)
-                        cb_colors = np.apply_along_axis(
-                            colors.to_hex, 1, mp_cmap(range(mp_cmap.N))
-                        )
-
-                        # linear legend
-                        if mp_cmap.N > 20:
-                            colorbar = bc.colormap.LinearColormap(
-                                cb_colors,
-                                vmin=vmin,
-                                vmax=vmax,
-                                caption=caption,
-                                **colormap_kwds,
-                            )
-
-                        # steps
-                        else:
-                            colorbar = bc.colormap.StepColormap(
-                                cb_colors,
-                                vmin=vmin,
-                                vmax=vmax,
-                                caption=caption,
-                                **colormap_kwds,
-                            )
-
-        if return_ == "empty_map":
-            return m
-
-        if return_ == "empty_map_and_colorbar":
-            return m, colorbar
-
-        if return_ == "map":
-            m.add_child(gjs)
-            if legend and cbar:
-                if nan_idx.any() and nan_color:
-                    _categorical_legend(
-                        m, "", [missing_kwds.pop("label", "NaN")], [nan_color]
-                    )
-                m.add_child(colorbar)
-            return m
-
-
-def _tooltip_popup(type, fields, gdf, **kwds):
-    """get tooltip or popup"""
-    import folium
-
-    # specify fields to show in the tooltip
-    if fields is False or fields is None or fields == 0:
-        return None
-    else:
-        if fields is True:
-            fields = gdf.columns.drop(gdf.geometry.name).to_list()
-        elif isinstance(fields, int):
-            fields = gdf.columns.drop(gdf.geometry.name).to_list()[:fields]
-        elif isinstance(fields, str):
-            fields = [fields]
-
-    for field in ["__plottable_column", "__folium_color"]:
-        if field in fields:
-            fields.remove(field)
-
-    # Cast fields to str
-    fields = list(map(str, fields))
-    if type == "tooltip":
-        return folium.GeoJsonTooltip(fields, **kwds)
-    elif type == "popup":
-        return folium.GeoJsonPopup(fields, **kwds)
+    geom_col = lines._geometry_column_name
 
+    # some LinearRings are coded as LineStrings and need to be removed manually
+    boundary = lines[geom_col].boundary
+    circles = boundary.loc[boundary.is_empty]
+    lines = lines[~lines.index.isin(circles.index)]
+
+    endpoints = lines[geom_col].boundary.explode(ignore_index=True)
+
+    if len(endpoints) / len(lines) != 2:
+        raise ValueError(
+            "The lines should have only two endpoints each. "
+            "Try splitting multilinestrings with explode."
+        )
 
-def _categorical_legend(m, title, categories, colors):
-    """
-    Add categorical legend to a map
+    return lines, endpoints
 
-    The implementation is using the code originally written by Michel Metran
-    (@michelmetran) and released on GitHub
-    (https://github.com/michelmetran/package_folium) under MIT license.
-
-    Copyright (c) 2020 Michel Metran
-
-    Parameters
-    ----------
-    m : folium.Map
-        Existing map instance on which to draw the plot
-    title : str
-        title of the legend (e.g. column name)
-    categories : list-like
-        list of categories
-    colors : list-like
-        list of colors (in the same order as categories)
-    """
 
-    # Header to Add
-    head = """
-    {% macro header(this, kwargs) %}
-    <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>
-    <script>$( function() {
-        $( ".maplegend" ).draggable({
-            start: function (event, ui) {
-                $(this).css({
-                    right: "auto",
-                    top: "auto",
-                    bottom: "auto"
-                });
-            }
-        });
-    });
-    </script>
-    <style type='text/css'>
-      .maplegend {
-        position: absolute;
-        z-index:9999;
-        background-color: rgba(255, 255, 255, .8);
-        border-radius: 5px;
-        box-shadow: 0 0 15px rgba(0,0,0,0.2);
-        padding: 10px;
-        font: 12px/14px Arial, Helvetica, sans-serif;
-        right: 10px;
-        bottom: 20px;
-      }
-      .maplegend .legend-title {
-        text-align: left;
-        margin-bottom: 5px;
-        font-weight: bold;
-        }
-      .maplegend .legend-scale ul {
-        margin: 0;
-        margin-bottom: 0px;
-        padding: 0;
-        float: left;
-        list-style: none;
-        }
-      .maplegend .legend-scale ul li {
-        list-style: none;
-        margin-left: 0;
-        line-height: 16px;
-        margin-bottom: 2px;
-        }
-      .maplegend ul.legend-labels li span {
-        display: block;
-        float: left;
-        height: 14px;
-        width: 14px;
-        margin-right: 5px;
-        margin-left: 0;
-        border: 0px solid #ccc;
-        }
-      .maplegend .legend-source {
-        color: #777;
-        clear: both;
-        }
-      .maplegend a {
-        color: #777;
-        }
-    </style>
-    {% endmacro %}
-    """
-    import branca as bc
+def _prepare_make_edge_cols_simple(
+    lines: GeoDataFrame,
+) -> tuple[GeoDataFrame, GeoDataFrame]:
+    """Faster version of _prepare_make_edge_cols."""
 
-    # Add CSS (on Header)
-    macro = bc.element.MacroElement()
-    macro._template = bc.element.Template(head)
-    m.get_root().add_child(macro)
-
-    body = f"""
-    <div id='maplegend {title}' class='maplegend'>
-        <div class='legend-title'>{title}</div>
-        <div class='legend-scale'>
-            <ul class='legend-labels'>"""
-
-    # Loop Categories
-    for label, color in zip(categories, colors, strict=True):
-        body += f"""
-                <li><span style='background:{color}'></span>{label}</li>"""
-
-    body += """
-            </ul>
-        </div>
-    </div>
-    """
+    endpoints = lines[lines._geometry_column_name].boundary.explode(ignore_index=True)
+
+    if len(endpoints) / len(lines) != 2:
+        raise ValueError(
+            "The lines should have only two endpoints each. "
+            "Try splitting multilinestrings with explode."
+        )
+
+    return lines, endpoints
+
+
+def _roundabouts_to_intersections(roads, query="ROADTYPE=='Rundkjøring'"):
+    from shapely.geometry import LineString
+    from shapely.ops import nearest_points
+
+    from .buffer_dissolve_explode import buffdissexp
+
+    roundabouts = roads.query(query)
+    not_roundabouts = roads.loc[~roads.index.isin(roundabouts.index)]
+
+    roundabouts = buffdissexp(roundabouts[["geometry"]], 1)
+    roundabouts["roundidx"] = roundabouts.index
+
+    border_to = roundabouts.overlay(not_roundabouts, how="intersection")
+
+    # for hver rundkjøring: lag linjer mellom rundkjøringens mitdpunkt og hver linje
+    # som grenser til rundkjøringen
+    as_intersections = []
+    for idx in roundabouts.roundidx:
+        this = roundabouts.loc[roundabouts.roundidx == idx]
+        border_to_this = border_to.loc[border_to.roundidx == idx].drop(
+            "roundidx", axis=1
+        )
+
+        midpoint = this.unary_union.centroid
+
+        # straight lines to the midpoint
+        for i, line in enumerate(border_to_this.geometry):
+            closest_point = nearest_points(midpoint, line)[1]
+            border_to_this.geometry.iloc[i] = LineString([closest_point, midpoint])
+
+        as_intersections.append(border_to_this)
+
+    as_intersections = GeoDataFrame(
+        pd.concat(as_intersections, ignore_index=True), crs=roads.crs
+    )
+    out = GeoDataFrame(
+        pd.concat([not_roundabouts, as_intersections], ignore_index=True), crs=roads.crs
+    )
 
-    # Add Body
-    body = bc.element.Element(body, "legend")
-    m.get_root().html.add_child(body)
+    return out
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ssb_sgis-0.1.3/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.1.4/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.1.4/src/sgis/geopandas_tools/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,20 +212,25 @@
     y = np.random.rand(n) * float(loc) * 2
 
     return GeoDataFrame(
         (Point(x, y) for x, y in zip(x, y, strict=True)), columns=["geometry"]
     )
 
 
-def random_points_in_polygons(gdf: GeoDataFrame, n: int) -> GeoDataFrame:
+def random_points_in_polygons(
+    gdf: GeoDataFrame, n: int, ignore_index=False
+) -> GeoDataFrame:
     """Creates n random points inside each polygon of a GeoDataFrame.
 
     Args:
         gdf: GeoDataFrame to use as mask for the points.
-        n: Number of points/rows to create.
+        n: Number of points to create per polygon in 'gdf'.
+        ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
+            Defaults to False, meaning the points will have the index of the polygon
+            it is within.
 
     Returns:
         A GeoDataFrame of points with 'n' rows per row in 'gdf'. It uses the index
         values of 'gdf'.
 
     Examples
     --------
@@ -267,40 +272,61 @@
 
     [300 rows x 1 columns]
     """
 
     if not all(gdf.geom_type.isin(["Polygon", "MultiPolygon"])):
         raise ValueError("Geometry types must be polygon.")
 
-    all_points = pd.DataFrame()
+    if gdf.index.is_unique:
+        gdf["temp_idx____"] = gdf.index
+    else:
+        gdf["temp_idx____"] = range(len(gdf))
 
-    for i in gdf.index:
-        polygon = gdf.loc[gdf.index == i]
+    all_points = pd.DataFrame()
 
+    for _ in range(n):
+        bounds = gdf.bounds
+        temp_idx____ = gdf["temp_idx____"].values
         overlapping = pd.DataFrame()
+        overlapping_indices = ()
+
+        while len(bounds):
+            xs = np.random.uniform(bounds.minx, bounds.maxx)
+            ys = np.random.uniform(bounds.miny, bounds.maxy)
 
-        while True:
-            minx, miny, maxx, maxy = polygon.total_bounds
-            x = np.random.uniform(minx, maxx, n)
-            y = np.random.uniform(miny, maxy, n)
-            points = to_gdf(
-                {"x": x, "y": y}, geometry=["x", "y"], crs=polygon.crs
-            ).drop(["x", "y"], axis=1)
-            overlapping = pd.concat(
-                [overlapping, points.clip(polygon)], ignore_index=True
+            points_df = pd.DataFrame({"x": xs, "y": ys}, index=temp_idx____)
+
+            points = to_gdf(points_df, geometry=["x", "y"], crs=gdf.crs).drop(
+                ["x", "y"], axis=1
             )
-            if len(overlapping) >= n:
-                break
 
-        overlapping = overlapping.sample(n)
-        overlapping.index = np.repeat(i, n)
+            overlapping = points.sjoin(gdf[["temp_idx____", "geometry"]], how="inner")
+
+            overlapping = overlapping.loc[overlapping.index == overlapping.temp_idx____]
+
+            all_points = pd.concat([all_points, overlapping], ignore_index=ignore_index)
+
+            overlapping_indices = overlapping_indices + tuple(overlapping.index.values)
+
+            gdf__ = gdf.loc[~gdf["temp_idx____"].isin(overlapping_indices)]
+            bounds = gdf__.bounds
+            temp_idx____ = gdf__["temp_idx____"].values
+
+    gdf = gdf.drop("temp_idx____", axis=1)
+
+    return all_points.sort_index().drop(["temp_idx____", "index_right"], axis=1)
 
-        all_points = pd.concat([all_points, overlapping], ignore_index=False)
 
-    return all_points
+def points_in_bounds(gdf: GeoDataFrame, n2: int):
+    minx, miny, maxx, maxy = gdf.total_bounds
+    xs = np.linspace(minx, maxx, num=n2)
+    ys = np.linspace(miny, maxy, num=n2)
+    x_coords, y_coords = np.meshgrid(xs, ys, indexing="ij")
+    coords = np.concatenate((x_coords.reshape(-1, 1), y_coords.reshape(-1, 1)), axis=1)
+    return to_gdf(coords, crs=gdf.crs)
 
 
 def to_lines(*gdfs: GeoDataFrame, copy: bool = True) -> GeoDataFrame:
     """Makes lines out of one or more GeoDataFrames and splits them at intersections.
 
     The GeoDataFrames' geometries are converted to LineStrings, then unioned together
     and made to singlepart. The lines are split at the intersections. Mimics
```

### Comparing `ssb_sgis-0.1.3/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.1.4/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.1.4/src/sgis/geopandas_tools/neighbors.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,72 +8,74 @@
 
 from .general import coordinate_array
 
 
 def get_neighbor_indices(
     gdf: GeoDataFrame | GeoSeries,
     neighbors: GeoDataFrame | GeoSeries,
-    max_dist: int = 0,
+    max_distance: int = 0,
     predicate: str = "intersects",
 ) -> Series:
     """Returns a pandas Series of neighbor indices.
 
-    The returned Series will contain values of all indices of 'neighbors' for each row in 'gdf'. will be the 'neighbours' indices. The Series index will be the
-    'gdf' indices.
+    The returned Series will contain values of all indices of 'neighbors' for each row
+    in 'gdf'. will be the 'neighbours' indices. The Series index will be the 'gdf'
+    indices.
 
     Finds all the geometries in 'neighbors' that intersect with 'gdf' and returns a
     list of the indices of the neighbors. Use set_index on the neighbors inside the
     function call to get values from a column instead of the current index.
 
     Args:
         gdf: GeoDataFrame or GeoSeries
         neighbors: GeoDataFrame or GeoSeries
-        max_dist: The maximum distance between the two geometries. Defaults to 0.
+        max_distance: The maximum distance between the two geometries. Defaults to 0.
         predicate: Spatial predicate to use in sjoin. Defaults to "intersects", meaning
             the geometry itself and geometries within will be considered neighbors if
             they are part of the 'neighbors' GeoDataFrame.
 
     Returns:
-        A list of the indices of the intersecting neighbors.
+        A pandas Series with indices of the intersecting 'neighbors'. The Series'
+        index will follow the index of the 'gdf'.
 
     Raises:
         ValueError: If gdf and neighbors do not have the same coordinate reference
             system.
 
     Examples
     --------
     >>> from sgis import get_neighbor_indices, to_gdf
     >>> points = to_gdf([(0, 0), (0.5, 0.5)])
     >>> points
                     geometry
     0  POINT (0.00000 0.00000)
     1  POINT (0.50000 0.50000)
 
-    Here, the points return the index of themselves.
+    With the default max_distance (0), the points return the index of themselves.
 
     >>> neighbor_indices = get_neighbor_indices(points, points)
     >>> neighbor_indices
     0    0
     1    1
     Name: neighbor_index, dtype: int64
 
-    With max_dist=1, each point find themselves and the neighbor.
+    With max_distance=1, each point find themselves and the neighbor.
 
-    >>> neighbor_indices = get_neighbor_indices(points, points, max_dist=1)
+    >>> neighbor_indices = get_neighbor_indices(points, points, max_distance=1)
     >>> neighbor_indices
     0    0
     1    0
     0    1
     1    1
     Name: neighbor_index, dtype: int64
 
     Using a column instead of the index.
 
     >>> points["text"] = [*"ab"]
-    >>> neighbor_indices = get_neighbor_indices(points, points.set_index("text"), max_dist=1)
+    >>> neighbor_indices = get_neighbor_indices(points, points.set_index("text"), max_distance=1)
     >>> neighbor_indices
     0    a
     1    a
     0    b
     1    b
     Name: neighbor_index, dtype: object
 
@@ -88,47 +90,52 @@
 
     """
 
     if gdf.crs != neighbors.crs:
         raise ValueError(f"'crs' mismatch. Got {gdf.crs} and {neighbors.crs}")
 
     # buffer and keep only geometry column
-    if max_dist:
+    if max_distance:
         if gdf.crs == 4326:
             warnings.warn(
-                "'gdf' has latlon crs, meaning the 'max_dist' paramter "
+                "'gdf' has latlon crs, meaning the 'max_distance' paramter "
                 "will not be in meters, but degrees."
             )
-        gdf = gdf.buffer(max_dist).to_frame()
+        gdf = gdf.buffer(max_distance).to_frame()
     else:
         gdf = gdf.geometry.to_frame()
 
-    joined = gdf.sjoin(neighbors, how="inner", predicate=predicate).rename(
-        columns={"index_right": "neighbor_index"}, errors="raise"
-    )
+    if predicate == "nearest":
+        joined = gdf.sjoin_nearest(neighbors, how="inner").rename(
+            columns={"index_right": "neighbor_index"}, errors="raise"
+        )
+    else:
+        joined = gdf.sjoin(neighbors, how="inner", predicate=predicate).rename(
+            columns={"index_right": "neighbor_index"}, errors="raise"
+        )
 
     return joined["neighbor_index"]
 
 
 def _get_unique_neighbor_indices(
     gdf: GeoDataFrame | GeoSeries,
     neighbors: GeoDataFrame | GeoSeries,
-    max_dist: int = 0,
+    max_distance: int = 0,
     predicate: str = "intersects",
 ) -> list:
     """Returns a list of the indices of a GeoDataFrame's neigbours.
 
     Finds all the geometries in 'neighbors' that intersect with 'gdf' and returns a
     list of the indices of the neighbors. Use set_index on the neighbors inside the
     function call to get values from a column instead of the current index.
 
     Args:
         gdf: GeoDataFrame or GeoSeries
         neighbors: GeoDataFrame or GeoSeries
-        max_dist: The maximum distance between the two geometries. Defaults to 0.
+        max_distance: The maximum distance between the two geometries. Defaults to 0.
         predicate: Spatial predicate to use in sjoin. Defaults to "intersects", meaning
             the geometry itself and geometries within will be considered neighbors if
             they are part of the 'neighbors' GeoDataFrame.
 
     Returns:
         A list of the indices of the intersecting neighbors.
 
@@ -145,39 +152,39 @@
     0  POINT (0.00000 0.00000)
     1  POINT (0.50000 0.50000)
     2  POINT (2.00000 2.00000)
 
     >>> p1 = points.iloc[[0]]
     >>> get_neighbor_indices(p1, points)
     [0]
-    >>> get_neighbor_indices(p1, points, max_dist=1)
+    >>> get_neighbor_indices(p1, points, max_distance=1)
     [0, 1]
-    >>> get_neighbor_indices(p1, points, max_dist=3)
+    >>> get_neighbor_indices(p1, points, max_distance=3)
     [0, 1, 2]
 
     Using a column instead of the index.
 
     >>> points["text"] = [*"abc"]
-    >>> get_neighbor_indices(p1, points.set_index("text"), max_dist=3)
+    >>> get_neighbor_indices(p1, points.set_index("text"), max_distance=3)
     ['a', 'b', 'c']
     """
 
     if gdf.crs != neighbors.crs:
         raise ValueError(f"'crs' mismatch. Got {gdf.crs} and {neighbors.crs}")
 
     id_col = "index_right"
 
     # buffer and keep only geometry column
-    if max_dist:
+    if max_distance:
         if gdf.crs == 4326:
             warnings.warn(
-                "'gdf' has latlon crs, meaning the 'max_dist' paramter "
+                "'gdf' has latlon crs, meaning the 'max_distance' paramter "
                 "will not be in meters, but degrees."
             )
-        gdf = gdf.buffer(max_dist).to_frame()
+        gdf = gdf.buffer(max_distance).to_frame()
     else:
         gdf = gdf.geometry.to_frame()
 
     joined = gdf.sjoin(neighbors, how="inner", predicate=predicate)
 
     return [x for x in joined[id_col].unique()]
```

### Comparing `ssb_sgis-0.1.3/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.1.4/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.1.4/src/sgis/geopandas_tools/point_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 from ..geopandas_tools.general import to_lines
 from ..geopandas_tools.geometry_types import get_geom_type, to_single_geom_type
 
 
 def snap_within_distance(
     points: GeoDataFrame,
     to: GeoDataFrame,
-    max_dist: int | float,
+    max_distance: int | float,
     *,
     distance_col: str | None = None,
 ) -> GeoDataFrame:
     """Snaps points to nearest geometry if within given distance.
 
     It takes a GeoDataFrame of points and snaps them to the nearest geometry in a
-    second GeoDataFrame if the snap distance is less than 'max_dist'. Returns distance
+    second GeoDataFrame if the snap distance is less than 'max_distance'. Returns distance
     column if specified.
 
     Args:
         points: The GeoDataFrame of points to snap.
         to: The GeoDataFrame to snap to.
-        max_dist: The maximum distance to snap to.
+        max_distance: The maximum distance to snap to.
         distance_col: Name of column with the snap distance. Defaults to
             'snap_distance'. Set to None to not get any distance column. This will make
             the function a bit faster.
 
     Returns:
         A GeoDataFrame or GeoSeries with the points snapped to the nearest point in the
         'to' GeoDataFrame or GeoSeries.
@@ -79,15 +79,15 @@
 
     copied = points.copy()
 
     geom_col = points._geometry_column_name
     copied[geom_col] = _series_snap(
         points=copied[geom_col],
         to=to,
-        max_dist=max_dist,
+        max_distance=max_distance,
     )
 
     if distance_col:
         copied[distance_col] = copied.distance(points)
         copied[distance_col] = np.where(
             copied[distance_col] == 0, pd.NA, copied[distance_col]
         )
@@ -152,15 +152,15 @@
 
     copied = points.copy()
 
     geom_col = points._geometry_column_name
     copied[geom_col] = _series_snap(
         points=copied[geom_col],
         to=to,
-        max_dist=None,
+        max_distance=None,
     )
 
     if distance_col:
         copied[distance_col] = copied.distance(points)
         copied[distance_col] = np.where(
             copied[distance_col] == 0, pd.NA, copied[distance_col]
         )
@@ -178,21 +178,21 @@
         return pd.concat([gdf_points, gdf_lines, gdf_polys])
     return gdf
 
 
 def _series_snap(
     points: GeoSeries,
     to: GeoSeries | GeoDataFrame | Geometry,
-    max_dist: int | float | None = None,
+    max_distance: int | float | None = None,
 ) -> GeoSeries:
     def snapfunc(point, to):
         nearest = nearest_points(point, to)[1]
-        if not max_dist:
+        if not max_distance:
             return nearest
-        return snap(point, nearest, tolerance=max_dist)
+        return snap(point, nearest, tolerance=max_distance)
 
     if isinstance(to, GeoDataFrame):
         unioned = to.unary_union
     elif isinstance(to, GeoSeries):
         unioned = to.to_frame().unary_union
     else:
         unioned = unary_union(to)
```

### Comparing `ssb_sgis-0.1.3/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.1.4/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/helpers.py` & `ssb_sgis-0.1.4/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/maps.py` & `ssb_sgis-0.1.4/src/sgis/maps/maps.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 The main function is 'explore', which displays one of more GeoDataFrames together in an
 interactive map with layers that can be toggled on and off. The 'samplemap' and
 'clipmap' functions do the same, but displays a random and chosen area respectfully.
 
 The 'qtm' function shows a static map of one or more GeoDataFrames.
 """
-import matplotlib.pyplot as plt
 from geopandas import GeoDataFrame, GeoSeries
 from matplotlib.axes._axes import Axes
 from matplotlib.figure import Figure
-from matplotlib.lines import Line2D
-from pandas.api.types import is_numeric_dtype
 from shapely import Geometry
 
-from .exceptions import NotInJupyterError
-from .explore import Explore, _separate_args
-from .helpers import make_namedict, return_two_vals
+from ..exceptions import NotInJupyterError
+from ..geopandas_tools.general import random_points_in_polygons
+from ..geopandas_tools.geometry_types import get_geom_type
+from ..helpers import make_namedict
+from .explore import Explore
+from .map import Map
+from .thematicmap import ThematicMap
 
 
 def _check_if_jupyter_is_needed(explore, show_in_browser):
     if explore and not show_in_browser:
         try:
             display
         except NameError as e:
@@ -37,19 +38,20 @@
     max_zoom: int = 30,
     show_in_browser: bool = False,
     **kwargs,
 ) -> None:
     """Interactive map of GeoDataFrames with layers that can be toggles on/off.
 
     It takes all the given GeoDataFrames and displays them together in an
-    interactive map with a common legend. The layers can be toggled on and off.
+    interactive map with a common legend. If 'column' is not specified, each
+    GeoDataFrame is given a unique color.
 
-    If 'column' is not specified, each GeoDataFrame is given a unique color. The
-    default colormap is a custom, strongly colored palette. If a numerical column
-    is given, the 'viridis' palette is used.
+    The coloring can be changed with the 'cmap' parameter. The default colormap is a
+    custom, strongly colored palette. If a numerical colum is given, the 'viridis'
+    palette is used.
 
     Note:
         The maximum zoom level only works on the OpenStreetMap background map.
 
     Args:
         *gdfs: one or more GeoDataFrames.
         column: The column to color the geometries by. Defaults to None, which means
@@ -59,15 +61,15 @@
             length as the number of gdfs.
         max_zoom: The maximum allowed level of zoom. Higher number means more zoom
             allowed. Defaults to 30, which is higher than the geopandas default.
         show_in_browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
-            is grouped. This defaults to 'fisherjenks' for numeric data.
+            is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
     See also
     --------
     samplemap: same functionality, but shows only a random area of a given size.
     clipmap: same functionality, but shows only the areas clipped by a given mask.
 
     Examples
@@ -82,17 +84,22 @@
 
     With additional arguments.
 
     >>> roads["meters"] = roads.length
     >>> points["meters"] = points.length
     >>> explore(roads, points, column="meters", cmap="plasma", max_zoom=60)
     """
-    kwargs: dict = kwargs | {"column": column, "max_zoom": max_zoom}
-
-    m = Explore(*gdfs, labels=labels, show_in_browser=show_in_browser, **kwargs)
+    m = Explore(
+        *gdfs,
+        column=column,
+        labels=labels,
+        show_in_browser=show_in_browser,
+        max_zoom=max_zoom,
+        **kwargs,
+    )
     m.explore()
 
 
 def samplemap(
     *gdfs: GeoDataFrame,
     column: str | None = None,
     size: int = 1500,
@@ -101,25 +108,17 @@
     max_zoom: int = 30,
     explore: bool = True,
     show_in_browser: bool = False,
     **kwargs,
 ) -> None:
     """Shows an interactive map of a random area of GeoDataFrames.
 
-    It takes all the GeoDataFrames specified, takes a random sample point, and shows
-    all geometries within a given radius of this point. Displays an interactive map
-    with a common legend. The layers can be toggled on and off.
-
-    The radius to plot can be changed with the 'size' parameter.
-
-    By default, tries to display interactive map, but falls back to static if not in
-    Jupyter. Can be changed to static by setting 'explore' to False. This will run the
-    function 'qtm'.
-
-    For more info about the labeling and coloring of the map, see the explore function.
+    It takes all the GeoDataFrames specified, takes a random sample point from the
+    first, and shows all geometries within a given radius of this point. Otherwise
+    works like the explore function.
 
     Note:
         The maximum zoom level only works on the OpenStreetMap background map.
 
     Args:
         *gdfs: one or more GeoDataFrames.
         column: The column to color the geometries by. Defaults to None, which means
@@ -135,20 +134,20 @@
             allowed. Defaults to 30, which is higher than the geopandas default.
         explore: If True (default), an interactive map will be displayed. If False,
             or not in Jupyter, a static plot will be shown.
         show_in_browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
-            is grouped. This defaults to 'fisherjenks' for numeric data.
+            is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
     See also
     --------
-    explore: same functionality, but shows the entire area of the geometries.
-    clipmap: same functionality, but shows only the areas clipped by a given mask.
+    explore: Same functionality, but shows the entire area of the geometries.
+    clipmap: Same functionality, but shows only the areas clipped by a given mask.
 
     Examples
     --------
     >>> from sgis import read_parquet_url, samplemap
     >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
     >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_eidskog.parquet")
 
@@ -157,47 +156,62 @@
     >>> samplemap(roads, points)
 
     Sample area with a radius of 5 kilometers.
 
     >>> samplemap(roads, points, size=5_000, column="meters")
 
     """
-    kwargs: dict = kwargs | {"column": column, "max_zoom": max_zoom}
-
     _check_if_jupyter_is_needed(explore, show_in_browser)
 
     if not size and isinstance(gdfs[-1], (float, int)):
         *gdfs, size = gdfs
 
-    gdfs, column, kwargs = _separate_args(gdfs, column, kwargs)
-
-    m = Explore(*gdfs, labels=labels, show_in_browser=show_in_browser, **kwargs)
-
     if explore:
+        m = Explore(
+            *gdfs,
+            column=column,
+            labels=labels,
+            show_in_browser=show_in_browser,
+            max_zoom=max_zoom,
+            **kwargs,
+        )
         m.samplemap(size, sample_from_first=sample_from_first)
     else:
+        m = Map(
+            *gdfs,
+            column=column,
+            labels=labels,
+            **kwargs,
+        )
+
         if sample_from_first:
-            random_point = m.gdfs[0].sample(1).centroid.buffer(size)
+            sample = m._gdfs[0].sample(1)
         else:
-            random_point = m.gdf.sample(1).centroid.buffer(size)
-        m.gdf = m.gdf.clip(random_point)
-        qtm(
-            m.gdf,
-            **{
-                key: value
-                for key, value in m.kwargs.items()
-                if key not in ["popup", "max_zoom"]
-            },
-        )
+            sample = m._gdf.sample(1)
+
+        # convert lines to polygons
+        if get_geom_type(sample) == "line":
+            sample["geometry"] = sample.buffer(1)
+
+        if get_geom_type(sample) == "polygon":
+            random_point = random_points_in_polygons(sample, 1)
+
+        # if point or mixed geometries
+        else:
+            random_point = sample.centroid.buffer
+
+        m._gdf = m._gdf.clip(random_point.buffer(size))
+
+        qtm(m._gdf, column=m.column, cmap=m._cmap, k=m.k)
 
 
 def clipmap(
     *gdfs: GeoDataFrame,
-    mask: GeoDataFrame | GeoSeries | Geometry,
     column: str | None = None,
+    mask: GeoDataFrame | GeoSeries | Geometry,
     labels: tuple[str] | None = None,
     explore: bool = True,
     max_zoom: int = 30,
     show_in_browser: bool = False,
     **kwargs,
 ) -> None:
     """Shows an interactive map of a of GeoDataFrames clipped to the mask extent.
@@ -223,207 +237,105 @@
             allowed. Defaults to 30, which is higher than the geopandas default.
         explore: If True (default), an interactive map will be displayed. If False,
             or not in Jupyter, a static plot will be shown.
         show_in_browser: If False (default), the maps will be shown in Jupyter.
             If True the maps will be opened in a browser folder.
         **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
             instance 'cmap' to change the colors, 'scheme' to change how the data
-            is grouped. This defaults to 'fisherjenks' for numeric data.
+            is grouped. This defaults to 'fisherjenkssampled' for numeric data.
 
     See also
     --------
     explore: same functionality, but shows the entire area of the geometries.
     samplemap: same functionality, but shows only a random area of a given size.
     """
 
-    kwargs: dict = kwargs | {"column": column, "max_zoom": max_zoom}
-
     _check_if_jupyter_is_needed(explore, show_in_browser)
 
-    clipped: tuple[GeoDataFrame] = ()
-
-    gdfs, column, kwargs = _separate_args(gdfs, column, kwargs)
+    gdfs, column = Explore._separate_args(gdfs, column)
 
-    # creating a dict of object names here, since the names disappear after clip
+    # storing object names in dict here, since the names disappear after clip
     if not labels:
         namedict = make_namedict(gdfs)
         kwargs["namedict"] = namedict
 
+    clipped: tuple[GeoDataFrame] = ()
+
     if mask is not None:
         for gdf in gdfs:
             clipped_ = gdf.clip(mask)
             clipped = clipped + (clipped_,)
 
     else:
         for gdf in gdfs[:-1]:
             clipped_ = gdf.clip(gdfs[-1])
             clipped = clipped + (clipped_,)
 
-    m = Explore(*clipped, labels=labels, show_in_browser=show_in_browser, **kwargs)
-
     if explore:
+        m = Explore(
+            *clipped,
+            column=column,
+            labels=labels,
+            show_in_browser=show_in_browser,
+            max_zoom=max_zoom,
+            **kwargs,
+        )
         m.explore()
     else:
-        qtm(
-            m.gdf,
-            **{
-                key: value
-                for key, value in m.kwargs.items()
-                if key not in ["popup", "max_zoom"]
-            },
+        m = Map(
+            *gdfs,
+            column=column,
+            labels=labels,
+            **kwargs,
         )
+        qtm(m._gdf, column=m.column, cmap=m._cmap, k=m.k)
 
 
 def qtm(
     *gdfs: GeoDataFrame,
     column: str | None = None,
-    bg_gdf: GeoDataFrame | None = None,
     title: str | None = None,
-    scheme: str | None = "fisherjenks",
-    legend: bool = True,
     black: bool = True,
     size: int = 10,
-    legend_title: str | None = None,
-    bbox_to_anchor: tuple[float | int, float | int] = (1, 0.2),
-    **kwargs,
-) -> tuple[Figure, Axes]:
+    legend: bool = True,
+    cmap: str | None = None,
+    k: int = 5,
+) -> None:
     """Quick, thematic map of one or more GeoDataFrames.
 
     Shows one or more GeoDataFrames in the same plot, with a common color scheme if
-    column is specified, or with unique colors for each GeoDataFrame if not. The
-    function simplifies the manual construction of a basic matplotlib plot. It also
-    returns the matplotlib figure and axis, so the plot can be changed afterwards.
+    column is specified, otherwise with unique colors for each GeoDataFrame.
 
-    Disclaimer: the 'qtm' name is taken from the tmap package in R.
+    The 'qtm' name is taken from the tmap package in R.
 
     Args:
         *gdfs: One or more GeoDataFrames to plot.
         column: The column to color the map by. Defaults to None, meaning each
             GeoDataFrame is given a unique color.
         title: Text to use as the map's heading.
-        scheme: How to group the column values. Defaults to 'fisherjenks' if numeric
-            column.
-        legend: Whether to include a legend explaining the colors and their values.
         black: If True (default), the background color will be black and the title
-            white. If False, it will be the opposite.
+            white. If False, it will be the opposite. The colormap will also be
+            'viridis' when black, and 'RdPu' when white.
         size: Size of the plot. Defaults to 10.
         title_fontsize: Size of the title.
-        **kwargs: Additional keyword arguments passed to the geopandas plot method.
+        cmap: Color palette of the map. See:
+            https://matplotlib.org/stable/tutorials/colors/colormaps.html
+        k: Number of color groups.
 
-    Returns:
-        The matplotlib figure and axis.
+    See also:
+        ThematicMap: Class with more options for customising the plot.
     """
 
-    if black:
-        facecolor, title_color, bg_gdf_color = "#0f0f0f", "#fefefe", "#383834"
-    else:
-        facecolor, title_color, bg_gdf_color = "#fefefe", "#0f0f0f", "#d1d1cd"
+    m = ThematicMap(*gdfs, column=column, size=size, black=black)
 
-    # run the gdfs through the __init__ of the Explore class
-    # this gives a custom categorical cmap and labels to be used in the legend
-    kwargs["column"] = column
-    gdfs, column, kwargs = _separate_args(gdfs, column, kwargs)
-    m = Explore(*gdfs, **kwargs)
-
-    # the 'column' in the kwargs has to be updated to the custom categorical column (if
-    # column was not specified).
-    kwargs["column"] = m.kwargs.pop("column")
-
-    if m._is_categorical and any(
-        kwarg in kwargs for kwarg in ("cmap", "color", "column")
-    ):
-        kwargs["color"] = m.gdf["color"]
-
-    if column and not is_numeric_dtype(m.gdf[column]):
-        scheme = None
-
-    size_x, size_y = return_two_vals(size)
-    fig, ax = _get_matplotlib_figure_and_axix(figsize=(size_x, size_y))
-
-    fig.patch.set_facecolor(facecolor)
-    ax.set_axis_off()
-
-    # manually add legend if categorical, since geopandas.plot removes it otherwise.
-    if legend and m._is_categorical:
-        kwargs.pop("column")
-        kwargs["color"] = m.gdf.color
-        patches, categories = [], []
-        for category, color in m._categories_colors_dict.items():
-            categories.append(category)
-            patches.append(
-                Line2D(
-                    [0],
-                    [0],
-                    linestyle="none",
-                    marker="o",
-                    alpha=kwargs.get("alpha", 1),
-                    markersize=10,
-                    markerfacecolor=color,
-                    markeredgewidth=0,
-                )
-            )
-        ax.legend(patches, categories, fontsize=size_x)
-
-    # if single color
-    elif legend and "color" in kwargs:
-        m.gdf["color"] = kwargs["color"]
-        kwargs.pop("column")
-        categories = [kwargs["color"] if isinstance(kwargs["color"], str) else "color"]
-        patches = [
-            Line2D(
-                [0],
-                [0],
-                linestyle="none",
-                marker="o",
-                alpha=kwargs.get("alpha", 1),
-                markersize=10,
-                markerfacecolor=kwargs["color"],
-                markeredgewidth=0,
-            )
-        ]
-        ax.legend(patches, categories, fontsize=size_x)
-
-    if not m._is_categorical:
-        # making unique bins manually so that all equal values get same color
-        unique_bins = m._create_bins(m.gdf, column, scheme)
-        kwargs["classification_kwds"] = {"bins": unique_bins}
-        if len(unique_bins) < kwargs.get("k", 5):
-            kwargs["k"] = len(unique_bins)
-
-    if title:
-        ax.set_title(title, fontsize=size_x * 2, color=title_color)
-
-    if bg_gdf is not None:
-        minx, miny, maxx, maxy = m.gdf.total_bounds
-        diffx = maxx - minx
-        diffy = maxy - miny
-        ax.set_xlim([minx - diffx * 0.03, maxx + diffx * 0.03])
-        ax.set_ylim([miny - diffy * 0.03, maxy + diffy * 0.03])
-        bg_gdf.plot(ax=ax, color=bg_gdf_color)
+    m.title = title
 
-    if "color" in kwargs:
-        kwargs.pop("column", None)
+    if k and len(m._unique_values) >= 6:
+        m.k = k
 
-    m.gdf.plot(scheme=scheme, legend=legend, ax=ax, **kwargs)
+    if cmap:
+        m.cmap = cmap
 
     if not legend:
-        return fig, ax
-
-    the_legend = plt.gca().get_legend()
-
-    for text in the_legend.get_texts():
-        text.set_fontsize(size_x)
-
-    the_legend.set_bbox_to_anchor(bbox_to_anchor)
-
-    legend_title = column if not legend_title else legend_title
-    the_legend.set_title(legend_title, prop={"size": size_x * 1.25})
-
-    plt.show()
-
-    return fig, ax
-
+        m.legend = None
 
-def _get_matplotlib_figure_and_axix(figsize):
-    fig = plt.figure(figsize=figsize)
-    ax = fig.add_subplot(1, 1, 1)
-    return fig, ax
+    m.plot()
```

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     1.0    85638
     Name: connected, dtype: int64
 
     Filling small gaps/holes in the network.
 
     >>> len(nw.gdf)
     85638
-    >>> nw = nw.close_network_holes(max_dist=1.5, fillna=0)
+    >>> nw = nw.close_network_holes(max_distance=1.5, fillna=0)
     >>> len(nw.gdf)
     86929
 
     Cutting long lines into pieces. This is only relevant for service area analysis and
     similar analyses.
 
     >>> nw.gdf.length.max()
@@ -277,26 +277,26 @@
         """
         self._update_nodes_if()
         self.gdf = get_component_size(self.gdf)
         return self
 
     def close_network_holes(
         self,
-        max_dist: int | float,
+        max_distance: int | float,
         max_angle: int,
         fillna: float | int | None,
         hole_col: str = "hole",
     ):
         """Fills network gaps with straigt lines.
 
         Fills holes in the network by connecting deadends with the the closest node
-        that is within the 'max_dist' distance and have an angle less 'max_angle'.
+        that is within the 'max_distance' distance and have an angle less 'max_angle'.
 
         Args:
-            max_dist: The maximum distance for the holes to be filled.
+            max_distance: The maximum distance for the holes to be filled.
             max_angle: Absolute number between 0 and 180 that represents the maximum
                 difference in angle between the new line and the prior, i.e. the line
                 at which the deadend ends. A value of 0 means the new lines must
                 have the exact same angle as the prior line, and 180 means the new
                 lines can go in any direction.
             fillna: Numeric value to assign to all NaN values of the holes. This is
                 chiefly the 'weight' column that is to be used in network analysis.
@@ -322,37 +322,37 @@
         1.0    85638
         0.0     7757
         Name: connected, dtype: int64
 
         Fill gaps shorter than 1.1 meters and an angle deviation of no more than
         30 degrees.
 
-        >>> nw = nw.close_network_holes(max_dist=1.1, max_angle=30, fillna=0)
+        >>> nw = nw.close_network_holes(max_distance=1.1, max_angle=30, fillna=0)
         >>> nw = nw.get_largest_component()
         >>> nw.gdf.connected.value_counts()
         1.0    100315
         0.0       191
         Name: connected, dtype: int64
 
         Fill gaps with all angles allowed.
 
-        >>> nw = nw.close_network_holes(max_dist=1.1, max_angle=180, fillna=0)
+        >>> nw = nw.close_network_holes(max_distance=1.1, max_angle=180, fillna=0)
         >>> nw = nw.get_largest_component()
         >>> nw.gdf.connected.value_counts()
         1.0    100315
         0.0       180
         Name: connected, dtype: int64
 
         It's not always wise to fill gaps. In the case of this data, these small gaps
         are intentional. They are road blocks where most cars aren't allowed to pass.
         Fill the holes only if it makes the travel times/routes more realistic.
         """
         self.gdf = close_network_holes(
             self.gdf,
-            max_dist,
+            max_distance,
             hole_col=hole_col,
             max_angle=max_angle,
         )
 
         if fillna is not None:
             self.gdf.loc[self.gdf[hole_col] == 1] = self.gdf.loc[
                 self.gdf[hole_col] == 1
@@ -360,26 +360,26 @@
 
         self._hole_col = hole_col
 
         return self
 
     def close_network_holes_to_deadends(
         self,
-        max_dist: int | float,
+        max_distance: int | float,
         fillna: int | float | None,
         hole_col: str = "hole",
     ):
-        """Fills holes between two deadends if the distance is less than the max_dist.
+        """Fills holes between two deadends if the distance is less than the max_distance.
 
         It fills gaps in the network by finding the nearest neighbors of each node,
-        then creating straigt lines between the nodes that are within the 'max_dist'
+        then creating straigt lines between the nodes that are within the 'max_distance'
         of each other.
 
         Args:
-            max_dist: The maximum distance between two nodes to be considered a hole.
+            max_distance: The maximum distance between two nodes to be considered a hole.
             fillna: The value to give the closed holes in all columns with NaN. This
                 has to be set in order for the closed holes to be included in network
                 analyses. If set to 0, the lines will get a weight of 0.
             hole_col: Holes will get the value 1 in a column named 'hole' by default,
                 or what is specified as hole_col. If set to None or False, no column
                 will be added.
 
@@ -400,28 +400,28 @@
         >>> nw.gdf.connected.value_counts()
         1.0    85638
         0.0     7757
         Name: connected, dtype: int64
 
         Fill gaps shorter than 1.1 meters and assign 0 to all columns.
 
-        >>> nw = nw.close_network_holes(max_dist=1.1, fillna=0)
+        >>> nw = nw.close_network_holes(max_distance=1.1, fillna=0)
         >>> nw = nw.get_largest_component()
         >>> nw.gdf.connected.value_counts()
         1.0    100315
         0.0       180
         Name: connected, dtype: int64
 
         It's not always wise to fill gaps. In the case of this data, these small gaps
         are intentional. They are road blocks where most cars aren't allowed to pass.
         Fill the holes only if it makes the travel times/routes more realistic.
         """
         self.gdf = close_network_holes_to_deadends(
             self.gdf,
-            max_dist,
+            max_distance,
             hole_col=hole_col,
         )
 
         if fillna is not None:
             self.gdf.loc[self.gdf[hole_col] == 1] = self.gdf.loc[
                 self.gdf[hole_col] == 1
             ].fillna(fillna)
```

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/network_norway.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/network_norway.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from geopandas import GeoDataFrame
 from pandas import DataFrame
 from shapely import force_2d
 
-from .directednetwork import DirectedNetwork
 from ..geopandas_tools.construction import gdf_concat
+from .directednetwork import DirectedNetwork
 from .network import Network
 
 
 class NetworkDaplaCar(DirectedNetwork):
     def __init__(
         self,
         gdf: GeoDataFrame | str = "daplasti_nyeste",
@@ -101,15 +101,15 @@
     nw = DirectedNetwork(roads)
 
     nw = nw.make_directed_network_norway()
 
     if turn_restrictions:
         nw.network = find_turn_restrictions(nw.network, turn_restrictions)
 
-    nw = nw.close_network_holes(max_dist=1.1, hole_col="hole")
+    nw = nw.close_network_holes(max_distance=1.1, hole_col="hole")
 
     nw = nw.get_largest_component()
 
     write_geopandas(nw.gdf, out_path)
 
     return nw
```

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/networkanalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1247,15 +1247,15 @@
 
         # create an id from before the split, used to revert the split later
         self.network.gdf["temp_idx__"] = range(len(self.network.gdf))
 
         lines = split_lines_by_nearest_point(
             lines=self.network.gdf,
             points=points,
-            max_dist=self.rules.search_tolerance,
+            max_distance=self.rules.search_tolerance,
         )
 
         # save the unsplit lines for later
         splitted = lines.loc[lines["splitted"] == 1, "temp_idx__"]
         self.network._not_splitted = self.network.gdf.loc[
             self.network.gdf["temp_idx__"].isin(splitted)
         ]
```

### Comparing `ssb_sgis-0.1.3/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.1.4/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/src/sgis/read_parquet.py` & `ssb_sgis-0.1.4/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.3/PKG-INFO` & `ssb_sgis-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.1.3
+Version: 0.1.4
 Summary: GIS utility functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: branca (>=0.6.0,<0.7.0)
 Requires-Dist: folium (>=0.14.0,<0.15.0)
 Requires-Dist: geopandas (>=0.12.2,<0.13.0)
 Requires-Dist: igraph (>=0.10.4,<0.11.0)
+Requires-Dist: jenkspy (>=0.3.2,<0.4.0)
 Requires-Dist: mapclassify (>=2.5.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
@@ -36,17 +37,17 @@
 GIS Python tools used in [Statistics Norway](https://www.ssb.no/en).
 
 [![PyPI](https://img.shields.io/pypi/v/ssb-sgis.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/ssb-sgis.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/ssb-sgis)][python version]
 [![License](https://img.shields.io/pypi/l/ssb-sgis)][license]
 
-[![Read the documentation at https://ssb-sgis.readthedocs.io/](https://img.shields.io/readthedocs/ssb-sgis/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Documentation](https://img.shields.io/badge/Documentation-GitHub_Pages-green.svg)](https://statisticsnorway.github.io/ssb-sgis/index.html)
 [![Tests](https://github.com/statisticsnorway/ssb-sgis/workflows/Tests/badge.svg)][tests]
-[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=statisticsnorway_ssb-sgis&metric=coverage)][coverage]
+[![Coverage](https://sonarcloud.io/component_measures?id=statisticsnorway_ssb-gis-utils&metric=new_coverage&view=list)][coverage]
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi_]: https://pypi.org/project/ssb-sgis/
 [status]: https://pypi.org/project/ssb-sgis/
 [python version]: https://pypi.org/project/ssb-sgis
@@ -86,87 +87,86 @@
 rules = sg.NetworkAnalysisRules(weight="minutes")
 
 nwa = sg.NetworkAnalysis(network=nw, rules=rules)
 
 nwa
 ```
 
-```
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
         rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
-```
 
 Get number of times each line segment was visited.
 
 ```python
-freq = nwa.get_route_frequencies(points.sample(75), points.sample(75))
+frequencies = nwa.get_route_frequencies(points.sample(75), points.sample(75))
 
-sg.qtm(
-    sg.buff(freq, 15),
-    "frequency",
-    scheme="naturalbreaks",
-    cmap="plasma",
-    title="Number of times each road was used.",
-)
+m = sg.ThematicMap(sg.buff(frequencies, 15), column="frequency", black=True)
+m.cmap = "plasma"
+m.title = "Number of times each road was used."
+m.plot()
 ```
 
-![png](docs/examples/network_analysis_examples_files/network_analysis_examples_6_0.png)
+![png](docs/examples/network_analysis_examples_files/network_analysis_examples_5_0.png)
 
 Fast many-to-many travel times/distances.
 
 ```python
 od = nwa.od_cost_matrix(points, points)
 
 print(od)
 ```
 
-```
             origin  destination    minutes
     0            0            0   0.000000
     1            0            1  13.039830
     2            0            2  10.902453
     3            0            3   8.297021
     4            0            4  14.742294
     ...        ...          ...        ...
     999995     999          995  11.038673
     999996     999          996  17.820664
     999997     999          997  10.288465
     999998     999          998  14.798257
     999999     999          999   0.000000
 
     [1000000 rows x 3 columns]
-```
 
 Get the area that can be reached within one or more breaks.
 
 ```python
-sa = nwa.service_area(
+service_areas = nwa.service_area(
     points.iloc[[0]],
     breaks=np.arange(1, 11),
 )
 
-sg.qtm(sa, "minutes", k=10, title="Roads that can be reached within 1 to 10 minutes")
+m = sg.ThematicMap(service_areas, column="minutes", black=True, size=10)
+m.k = 10
+m.title = "Roads that can be reached within 1 to 10 minutes"
+m.plot()
 ```
 
-![png](docs/examples/network_analysis_examples_files/network_analysis_examples_10_0.png)
+![png](docs/examples/network_analysis_examples_files/network_analysis_examples_9_0.png)
 
 Get one or more route per origin-destination pair.
 
 ```python
 routes = nwa.get_k_routes(
-    points.iloc[[0]], points.iloc[[1]], k=5, drop_middle_percent=50
+    points.iloc[[0]], points.iloc[[1]], k=4, drop_middle_percent=50
 )
 
-sg.qtm(sg.buff(routes, 15), "k", title="Five fastest routes from A to B", legend=False)
+m = sg.ThematicMap(sg.buff(routes, 15), column="k", black=True)
+m.title = "Four fastest routes from A to B"
+m.legend.title = "Rank"
+m.plot()
 ```
 
-![png](docs/examples/network_analysis_examples_files/network_analysis_examples_12_1.png)
+![png](docs/examples/network_analysis_examples_files/network_analysis_examples_11_0.png)
 
 More network analysis examples can be found here: https://github.com/statisticsnorway/ssb-sgis/blob/main/docs/network_analysis_demo_template.md
 
 Road data for Norway can be downloaded here: https://kartkatalog.geonorge.no/metadata/nvdb-ruteplan-nettverksdatasett/8d0f9066-34f9-4423-be12-8e8523089313
 
 ## Developer information
```

