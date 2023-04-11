# Comparing `tmp/gplately-0.3.3.tar.gz` & `tmp/gplately-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gplately-0.3.3.tar", last modified: Fri Mar 10 05:04:34 2023, max compression
+gzip compressed data, was "gplately-0.4.tar", last modified: Tue Apr 11 11:35:46 2023, max compression
```

## Comparing `gplately-0.3.3.tar` & `gplately-0.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 05:04:34.371908 gplately-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (122)    12404 2023-03-10 05:04:34.371908 gplately-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10130 2023-03-10 05:03:08.000000 gplately-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 05:04:34.371908 gplately-0.3.3/gplately/
--rw-r--r--   0 runner    (1001) docker     (122)     4476 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14476 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    59493 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/download.py
--rw-r--r--   0 runner    (1001) docker     (122)    20072 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/geometry.py
--rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/gpml.py
--rw-r--r--   0 runner    (1001) docker     (122)    72061 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/grids.py
--rw-r--r--   0 runner    (1001) docker     (122)     4103 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    74257 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/oceans.py
--rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/parallel.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    89900 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/pygplates.py
--rw-r--r--   0 runner    (1001) docker     (122)   104564 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (122)    24596 2023-03-10 05:03:08.000000 gplately-0.3.3/gplately/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 05:04:34.371908 gplately-0.3.3/gplately.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    12404 2023-03-10 05:04:33.000000 gplately-0.3.3/gplately.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-03-10 05:04:34.000000 gplately-0.3.3/gplately.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-10 05:04:33.000000 gplately-0.3.3/gplately.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-03-10 05:04:33.000000 gplately-0.3.3/gplately.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-10 05:04:33.000000 gplately-0.3.3/gplately.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-10 05:04:34.371908 gplately-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4012 2023-03-10 05:03:08.000000 gplately-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-10 05:04:34.371908 gplately-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (122)      796 2023-03-10 05:03:08.000000 gplately-0.3.3/test/test_0_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-03-10 05:03:08.000000 gplately-0.3.3/test/test_1_reconstructions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-03-10 05:03:08.000000 gplately-0.3.3/test/test_2_points.py
--rw-r--r--   0 runner    (1001) docker     (122)     6359 2023-03-10 05:03:08.000000 gplately-0.3.3/test/test_3_plottopologies.py
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-03-10 05:03:08.000000 gplately-0.3.3/test/test_4_rasters.py
--rw-r--r--   0 runner    (1001) docker     (122)     6011 2023-03-10 05:03:08.000000 gplately-0.3.3/test/test_5_seafloorgrid.py
--rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-03-10 05:03:08.000000 gplately-0.3.3/test/test_6_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:35:46.211823 gplately-0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    18092 2023-04-11 11:34:21.000000 gplately-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    15922 2023-04-11 11:35:46.211823 gplately-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13290 2023-04-11 11:34:22.000000 gplately-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:35:46.207822 gplately-0.4/gplately/
+-rw-r--r--   0 runner    (1001) docker     (122)     6279 2023-04-11 11:34:22.000000 gplately-0.4/gplately/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15195 2023-04-11 11:34:22.000000 gplately-0.4/gplately/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80675 2023-04-11 11:34:22.000000 gplately-0.4/gplately/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20072 2023-04-11 11:34:22.000000 gplately-0.4/gplately/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-04-11 11:34:22.000000 gplately-0.4/gplately/gpml.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75773 2023-04-11 11:34:22.000000 gplately-0.4/gplately/grids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4103 2023-04-11 11:34:22.000000 gplately-0.4/gplately/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68818 2023-04-11 11:34:22.000000 gplately-0.4/gplately/oceans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-04-11 11:34:22.000000 gplately-0.4/gplately/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)   126380 2023-04-11 11:34:22.000000 gplately-0.4/gplately/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5142 2023-04-11 11:34:22.000000 gplately-0.4/gplately/pygplates.py
+-rw-r--r--   0 runner    (1001) docker     (122)   105151 2023-04-11 11:34:22.000000 gplately-0.4/gplately/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24596 2023-04-11 11:34:22.000000 gplately-0.4/gplately/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:35:46.207822 gplately-0.4/gplately.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15922 2023-04-11 11:35:45.000000 gplately-0.4/gplately.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-04-11 11:35:46.000000 gplately-0.4/gplately.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 11:35:45.000000 gplately-0.4/gplately.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-04-11 11:35:45.000000 gplately-0.4/gplately.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 11:35:45.000000 gplately-0.4/gplately.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 11:35:46.211823 gplately-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4010 2023-04-11 11:34:22.000000 gplately-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 11:35:46.211823 gplately-0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-11 11:34:22.000000 gplately-0.4/test/test_0_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5923 2023-04-11 11:34:22.000000 gplately-0.4/test/test_1_reconstructions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-04-11 11:34:22.000000 gplately-0.4/test/test_2_points.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6359 2023-04-11 11:34:22.000000 gplately-0.4/test/test_3_plottopologies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-04-11 11:34:22.000000 gplately-0.4/test/test_4_rasters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6011 2023-04-11 11:34:22.000000 gplately-0.4/test/test_5_seafloorgrid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-04-11 11:34:22.000000 gplately-0.4/test/test_6_geometry.py
```

### Comparing `gplately-0.3.3/PKG-INFO` & `gplately-0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,141 @@
 Metadata-Version: 2.1
 Name: gplately
-Version: 0.3.3
+Version: 0.4
 Summary: Object-orientated Python interface to pyGPlates for plate tectonic reconstructions
 Home-page: https://github.com/GPlates/gplately
 Author: Ben Mather
 Author-email: ben.mather@sydney.edu.au
 License: UNKNOWN
-Description: # GPlately
+Description: <p align="center">
+        <picture>
+          <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_White_logo.png">
+          <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
+          <img alt="GPlately logo." src="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
+        </picture>
+        </p>
+        
+        ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/GPlates/gplately/build_and_test.yml?branch=master&style=for-the-badge)
+        ![PyPI](https://img.shields.io/pypi/v/gplately?style=for-the-badge)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dw/gplately?style=for-the-badge)
         
-        GPlately was created to accelerate spatio-temporal data analysis leveraging pyGPlates and PlateTectonicTools within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
+        
+        GPlately was created to accelerate spatio-temporal data analysis leveraging [pyGPlates](https://www.gplates.org/docs/pygplates/index.html) and [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
         
         ![SeedPointGIF](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/muller19_seedpoints.gif)
         
         
         GPlately requires a working installation of pyGPlates, which is freely
         available at https://www.gplates.org/download.
         All major system architectures (e.g. Linux, MacOS, Windows) are supported and installation instructions
         are [well documented](https://www.gplates.org/docs/pygplates/pygplates_getting_started.html\#installation).
         Sample data is also available from [EarthByte servers](https://www.earthbyte.org/category/resources/), which
         includes rasters, seafloor age grids, rotation files, and more to get started with plate reconstructions.
         
         #### Citation
         
-        _Coming soon!_
+        > Mather, B.R., Müller, R.D., Zahirovic, S., Cannon, J., Chin, M., Ilano, L., Wright, N.M., Alfonso, C., Williams, S., Tetley, M., Merdith, A. (2023) Deep time spatio-temporal data analysis using pyGPlates with PlateTectonicTools and GPlately. _Geoscience Data Journal_, 1–8. Available from: https://doi.org/10.1002/gdj3.185
+        
+        ```bib
+        @article{Mather2023,
+        author = {Mather, Ben R. and Müller, R. Dietmar and Zahirovic, Sabin and Cannon, John and Chin, Michael and Ilano, Lauren and Wright, Nicky M. and Alfonso, Christopher and Williams, Simon and Tetley, Michael and Merdith, Andrew},
+        title = {Deep time spatio-temporal data analysis using pyGPlates with PlateTectonicTools and GPlately},
+        year = {2023},
+        journal = {Geoscience Data Journal},
+        pages = {1-8},
+        keywords = {geospatial, plate reconstructions, pyGPlates, python, tectonics},
+        doi = {https://doi.org/10.1002/gdj3.185},
+        url = {https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/gdj3.185},
+        eprint = {https://rmets.onlinelibrary.wiley.com/doi/pdf/10.1002/gdj3.185},
+        }
+        ```
         
         ## Dependencies
         
         - [pyGPlates](https://www.gplates.org/docs/pygplates/pygplates_getting_started.html#installation)
         - [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools)
-        - [Shapely <2.0](https://shapely.readthedocs.io/en/stable/project.html#installing-shapely)
-        - NumPy
-        - SciPy 1.10
-        - Matplotlib
+        - [Shapely](https://shapely.readthedocs.io/en/stable/project.html#installing-shapely)
+        - [NumPy](https://numpy.org/install/) > 1.16
+        - [SciPy](https://scipy.org/install/) > 1.0
+        - [Matplotlib](https://matplotlib.org/stable/users/installing/index.html)
         - [Cartopy](https://scitools.org.uk/cartopy/docs/latest/index.html#getting-started) (for mapping)
-        - Shapely
+        - [Shapely](https://shapely.readthedocs.io/en/stable/installation.html)
         - [Pooch](https://github.com/fatiando/pooch)
-        - GeoPandas
-        - netCDF4
+        - [GeoPandas](https://geopandas.org/en/stable/getting_started.html)
+        - [netCDF4](https://unidata.github.io/netcdf4-python/#quick-install)
         
         
         ## Installation
         
-        ### Stable release
-        You can install the latest stable public release of `GPlately` using the pip package manager.
+        ### 1. Using conda (recommended)
         
-        ```python
+        You can install the latest stable public release of `GPlately` and all of its dependencies using conda.
+        This is the preferred method to install `GPlately` which downloads binaries from the conda-forge channel.
+        
+        ```sh
+        conda install -c conda-forge gplately
+        ```
+        
+        #### Creating a new conda environment
+        
+        We recommend creating a new conda environment inside which to install `GPlately`. This avoids any potential conflicts in your base Python environment. In the example below we create a new environment called "`my-env`":
+        
+        ```sh
+        conda create -n my-env
+        conda activate my-env
+        conda install -c conda-forge gplately
+        ```
+        
+        `my-env` needs to be activated whenever you use `GPlately`: i.e. `conda activate my-env`.
+        
+        ### 2. Using pip
+        
+        Alternatively, you can install the latest stable public release of `GPlately` using the pip package manager.
+        
+        ```sh
         pip install gplately
         ```
-        or:
+        or from this GitHub repository:
         
-        ```python
+        ```sh
         pip install git+https://github.com/GPlates/gplately.git 
         ```
         
-        ### Pull from repository 
+        #### Pull from repository 
         
         **First-time installation:** To install the latest version of GPlately from a specific repository branch (e.g. `master`), copy the following commands into your terminal:
         
-        ```python
+        ```sh
         cd /path/to/desired/directory #Change your command directory to where you'd like to clone GPlately
         git clone https://github.com/GPlates/gplately.git
-        pwd # Just to check your directory - should end with /.../gplately
+        cd gplately # navigate within the gplately folder
         git checkout master # or the name of whichever branch you need
         git pull # fetch all recent changes from this branch
         pip install .
         ```
         
         **Update installation from cloned repo:** To update your installation of GPlately by fetching the latest pushes from a specific repository branch (e.g. `master`), copy the following commands into your terminal:
         
-        ```python
+        ```sh
         cd /path/to/gplately/directory #Should be where gplately is cloned - must end in /.../gplately
         git checkout master # or the name of whichever branch you need
         git pull # fetch all recent changes from this branch
         pip install .
         ```
         
         
         ## Usage
         
         GPlately uses objects to accomplish a variety of common tasks. The common objects include:
         
-        - `DataServer` - download rotation files and topology features from plate models on EarthByte's webDAV server
-        - `PlateReconstruction` - reconstruct features, tesselate mid ocean ridges, subduction zones
-        - `Points` - partition points onto plates, rotate back through time
-        - `Raster` - read in NetCDF grids, interpolation, resampling
-        - `PlotTopologies` - one stop shop for plotting ridges, trenches, subduction teeth
+        - [`DataServer`](#the-dataserver-object) - download rotation files and topology features from plate models on EarthByte's webDAV server
+        - [`PlateReconstruction`](#the-platereconstruction-object) - reconstruct features, tesselate mid ocean ridges, subduction zones
+        - [`Points`](#the-points-object) - partition points onto plates, rotate back through time
+        - [`Raster`](#the-raster-object) - read in NetCDF grids, interpolation, resampling
+        - [`PlotTopologies`](#the-plottopologies-object) - one stop shop for plotting ridges, trenches, subduction teeth
         
         
         ### The `DataServer` object
         
         `GPlately`'s `DataServer` object can be used to download:
         
         - rotation models
@@ -116,46 +163,28 @@
         the object by passing a `rotation model`, a set of `topology features` and some `static polygons`: 
         
         ```python
         model = gplately.PlateReconstruction(rotation_model, topology_features, static_polygons)
         ```
         Launch the [Plate Reconstruction](https://github.com/GPlates/gplately/blob/master/Notebooks/02-PlateReconstructions.ipynb) notebook to see more.
         
-        
-        ### The `PlotTopologies` object
-        
-        ... can be used to visualise reconstructed feature geometries through time. To call the object, pass a set of `continents`, 
-        `coastlines` and `COBs` (either as file paths or as `<pyGPlates.FeatureCollection>` objects), as well as a `PlateReconstruction`
-        object, and a reconstruction `time`. 
-        
-        ```python
-        coastlines, continents, COBs = gDownload.get_topology_geometries()
-        time = 50 #Ma
-        gPlot = gplately.plot.PlotTopologies(model, time, coastlines, continents, COBs)
-        ```
-        Below are some continents, coastlines, COBs, ridges and transforms, trenches, subduction teeth and
-        seafloor age grids plotted using `PlotTopologies`!
-        
-        ![ReconstructionImage](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/plot_topologies_img.png)
-        
         ### The `Points` object
         
         ... can be used to reconstruct the positions of geological point features and calculate their underlying plate velocities 
         through geological time. 
         
         ```python
         pt_lon = np.array([-107.662152, -58.082792, 17.483189, 133.674590, 80.412876])
         pt_lat = np.array([48.797807, -12.654857, 11.884395, -26.415630, 31.368509])
         
         # Call the Points object: pass the PlateReconstruction object, and the latitudes and longitudes of the seed points!
         gpts = gplately.Points(model, pt_lon, pt_lat)
         ```
         ![PointData](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/surface_hotspot_plumes.png)
         
-        
         ### The `Raster` object
         
         ...can be used to read, resample and resize assorted raster data like `netCDF4` seafloor age grids, continental grids and ETOPO
         relief rasters. You can also reconstruct raster data back through geological time!
         
         ```python
         etopo = gdownload.get_raster("ETOPO1_tif")
@@ -175,27 +204,43 @@
         )
         ```
         
         Below is a plot of the [ETOPO1 global relief raster](https://www.ncei.noaa.gov/products/etopo-global-relief-model) at present day, and reconstructed to 50Ma:
         
         ![RasterImg](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/etopo_reconstruction.png)
         
+        ### The `PlotTopologies` object
+        
+        ... can be used to visualise reconstructed feature geometries through time. To call the object, pass a set of `continents`, 
+        `coastlines` and `COBs` (either as file paths or as `<pyGPlates.FeatureCollection>` objects), as well as a `PlateReconstruction`
+        object, and a reconstruction `time`. 
+        
+        ```python
+        coastlines, continents, COBs = gDownload.get_topology_geometries()
+        time = 50 #Ma
+        gPlot = gplately.plot.PlotTopologies(model, time, coastlines, continents, COBs)
+        ```
+        Below are some continents, coastlines, COBs, ridges and transforms, trenches, subduction teeth and
+        seafloor age grids plotted using `PlotTopologies`!
+        
+        ![ReconstructionImage](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/plot_topologies_img.png)
+        
         
         ## Sample workflows
         
         To see GPlately in action, launch a Jupyter Notebook environment and check out the [sample notebooks](./Notebooks):
         
         - [__01 - Getting Started__](https://github.com/GPlates/gplately/blob/master/Notebooks/01-GettingStarted.ipynb): A brief overview of how to initialise GPlately's main objects
         - [__02 - Plate Reconstructions__](https://github.com/GPlates/gplately/blob/master/Notebooks/02-PlateReconstructions.ipynb): Setting up a `PlateReconstruction` object, reconstructing geological data through time 
         - [__03 - Working with Points__](https://github.com/GPlates/gplately/blob/master/Notebooks/03-WorkingWithPoints.ipynb): Setting up a `Points` object, reconstructing seed point locations through time with. This notebook uses point data from the Paleobiology Database (PBDB).
         - [__04 - Velocity Basics__](https://github.com/GPlates/gplately/blob/master/Notebooks/04-VelocityBasics.ipynb): Calculating plate velocities, plotting velocity vector fields
         - [__05 - Working with Feature Geometries__](https://github.com/GPlates/gplately/blob/master/Notebooks/05-WorkingWithFeatureGeometries.ipynb): Processing and plotting assorted polyline, polygon and point data from [GPlates 2.3's sample data sets](https://www.earthbyte.org/gplates-2-3-software-and-data-sets/)
         - [__06 - Rasters__](https://github.com/GPlates/gplately/blob/master/Notebooks/06-Rasters.ipynb): Reading, resizing, resampling raster data, and linearly interpolating point data onto raster data
         - [__07 - Plate Tectonic Stats__](https://github.com/GPlates/gplately/blob/master/Notebooks/07-WorkingWithPlateTectonicStats.ipynb): Using [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) to calculate and plot subduction zone and ridge data (convergence/spreading velocities, subduction angles, subduction zone and ridge lengths, crustal surface areas produced and subducted etc.) 
-        - [__08 - Predicting Slab Dip__](https://github.com/GPlates/gplately/blob/master/Notebooks/08-PredictingSlabDip.ipynb): Predicting the average slab dip angle of subducting oceanic lithosphere.
+        - [__08 - Predicting Slab Flux__](https://github.com/GPlates/gplately/blob/master/Notebooks/08-PredictingSlabFlux.ipynb): Predicting the average slab dip angle of subducting oceanic lithosphere.
         - [__09 - Motion Paths and Flowlines__](https://github.com/GPlates/gplately/blob/master/Notebooks/09-CreatingMotionPathsAndFlowlines.ipynb): Using pyGPlates to create motion paths and flowines of points on a tectonic plate to illustrate the plate's trajectory through geological time.
         - [__10 - SeafloorGrid__](https://github.com/GPlates/gplately/blob/master/Notebooks/10-SeafloorGrids.ipynb): Defines the parameters needed to set up a `SeafloorGrid` object, and demonstrates how to produce age and spreading rate grids from a set of plate reconstruction model files.
         
         ## API Documentation
         
         Documentation of GPlately's objects and methods can be found [here](https://gplates.github.io/gplately/)!
```

### Comparing `gplately-0.3.3/README.md` & `gplately-0.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,133 @@
-# GPlately
+<p align="center">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_White_logo.png">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
+  <img alt="GPlately logo." src="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
+</picture>
+</p>
+
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/GPlates/gplately/build_and_test.yml?branch=master&style=for-the-badge)
+![PyPI](https://img.shields.io/pypi/v/gplately?style=for-the-badge)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/gplately?style=for-the-badge)
 
-GPlately was created to accelerate spatio-temporal data analysis leveraging pyGPlates and PlateTectonicTools within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
+
+GPlately was created to accelerate spatio-temporal data analysis leveraging [pyGPlates](https://www.gplates.org/docs/pygplates/index.html) and [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
 
 ![SeedPointGIF](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/muller19_seedpoints.gif)
 
 
 GPlately requires a working installation of pyGPlates, which is freely
 available at https://www.gplates.org/download.
 All major system architectures (e.g. Linux, MacOS, Windows) are supported and installation instructions
 are [well documented](https://www.gplates.org/docs/pygplates/pygplates_getting_started.html\#installation).
 Sample data is also available from [EarthByte servers](https://www.earthbyte.org/category/resources/), which
 includes rasters, seafloor age grids, rotation files, and more to get started with plate reconstructions.
 
 #### Citation
 
-_Coming soon!_
+> Mather, B.R., Müller, R.D., Zahirovic, S., Cannon, J., Chin, M., Ilano, L., Wright, N.M., Alfonso, C., Williams, S., Tetley, M., Merdith, A. (2023) Deep time spatio-temporal data analysis using pyGPlates with PlateTectonicTools and GPlately. _Geoscience Data Journal_, 1–8. Available from: https://doi.org/10.1002/gdj3.185
+
+```bib
+@article{Mather2023,
+author = {Mather, Ben R. and Müller, R. Dietmar and Zahirovic, Sabin and Cannon, John and Chin, Michael and Ilano, Lauren and Wright, Nicky M. and Alfonso, Christopher and Williams, Simon and Tetley, Michael and Merdith, Andrew},
+title = {Deep time spatio-temporal data analysis using pyGPlates with PlateTectonicTools and GPlately},
+year = {2023},
+journal = {Geoscience Data Journal},
+pages = {1-8},
+keywords = {geospatial, plate reconstructions, pyGPlates, python, tectonics},
+doi = {https://doi.org/10.1002/gdj3.185},
+url = {https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/gdj3.185},
+eprint = {https://rmets.onlinelibrary.wiley.com/doi/pdf/10.1002/gdj3.185},
+}
+```
 
 ## Dependencies
 
 - [pyGPlates](https://www.gplates.org/docs/pygplates/pygplates_getting_started.html#installation)
 - [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools)
-- [Shapely <2.0](https://shapely.readthedocs.io/en/stable/project.html#installing-shapely)
-- NumPy
-- SciPy 1.10
-- Matplotlib
+- [Shapely](https://shapely.readthedocs.io/en/stable/project.html#installing-shapely)
+- [NumPy](https://numpy.org/install/) > 1.16
+- [SciPy](https://scipy.org/install/) > 1.0
+- [Matplotlib](https://matplotlib.org/stable/users/installing/index.html)
 - [Cartopy](https://scitools.org.uk/cartopy/docs/latest/index.html#getting-started) (for mapping)
-- Shapely
+- [Shapely](https://shapely.readthedocs.io/en/stable/installation.html)
 - [Pooch](https://github.com/fatiando/pooch)
-- GeoPandas
-- netCDF4
+- [GeoPandas](https://geopandas.org/en/stable/getting_started.html)
+- [netCDF4](https://unidata.github.io/netcdf4-python/#quick-install)
 
 
 ## Installation
 
-### Stable release
-You can install the latest stable public release of `GPlately` using the pip package manager.
+### 1. Using conda (recommended)
 
-```python
+You can install the latest stable public release of `GPlately` and all of its dependencies using conda.
+This is the preferred method to install `GPlately` which downloads binaries from the conda-forge channel.
+
+```sh
+conda install -c conda-forge gplately
+```
+
+#### Creating a new conda environment
+
+We recommend creating a new conda environment inside which to install `GPlately`. This avoids any potential conflicts in your base Python environment. In the example below we create a new environment called "`my-env`":
+
+```sh
+conda create -n my-env
+conda activate my-env
+conda install -c conda-forge gplately
+```
+
+`my-env` needs to be activated whenever you use `GPlately`: i.e. `conda activate my-env`.
+
+### 2. Using pip
+
+Alternatively, you can install the latest stable public release of `GPlately` using the pip package manager.
+
+```sh
 pip install gplately
 ```
-or:
+or from this GitHub repository:
 
-```python
+```sh
 pip install git+https://github.com/GPlates/gplately.git 
 ```
 
-### Pull from repository 
+#### Pull from repository 
 
 **First-time installation:** To install the latest version of GPlately from a specific repository branch (e.g. `master`), copy the following commands into your terminal:
 
-```python
+```sh
 cd /path/to/desired/directory #Change your command directory to where you'd like to clone GPlately
 git clone https://github.com/GPlates/gplately.git
-pwd # Just to check your directory - should end with /.../gplately
+cd gplately # navigate within the gplately folder
 git checkout master # or the name of whichever branch you need
 git pull # fetch all recent changes from this branch
 pip install .
 ```
 
 **Update installation from cloned repo:** To update your installation of GPlately by fetching the latest pushes from a specific repository branch (e.g. `master`), copy the following commands into your terminal:
 
-```python
+```sh
 cd /path/to/gplately/directory #Should be where gplately is cloned - must end in /.../gplately
 git checkout master # or the name of whichever branch you need
 git pull # fetch all recent changes from this branch
 pip install .
 ```
 
 
 ## Usage
 
 GPlately uses objects to accomplish a variety of common tasks. The common objects include:
 
-- `DataServer` - download rotation files and topology features from plate models on EarthByte's webDAV server
-- `PlateReconstruction` - reconstruct features, tesselate mid ocean ridges, subduction zones
-- `Points` - partition points onto plates, rotate back through time
-- `Raster` - read in NetCDF grids, interpolation, resampling
-- `PlotTopologies` - one stop shop for plotting ridges, trenches, subduction teeth
+- [`DataServer`](#the-dataserver-object) - download rotation files and topology features from plate models on EarthByte's webDAV server
+- [`PlateReconstruction`](#the-platereconstruction-object) - reconstruct features, tesselate mid ocean ridges, subduction zones
+- [`Points`](#the-points-object) - partition points onto plates, rotate back through time
+- [`Raster`](#the-raster-object) - read in NetCDF grids, interpolation, resampling
+- [`PlotTopologies`](#the-plottopologies-object) - one stop shop for plotting ridges, trenches, subduction teeth
 
 
 ### The `DataServer` object
 
 `GPlately`'s `DataServer` object can be used to download:
 
 - rotation models
@@ -108,46 +155,28 @@
 the object by passing a `rotation model`, a set of `topology features` and some `static polygons`: 
 
 ```python
 model = gplately.PlateReconstruction(rotation_model, topology_features, static_polygons)
 ```
 Launch the [Plate Reconstruction](https://github.com/GPlates/gplately/blob/master/Notebooks/02-PlateReconstructions.ipynb) notebook to see more.
 
-
-### The `PlotTopologies` object
-
-... can be used to visualise reconstructed feature geometries through time. To call the object, pass a set of `continents`, 
-`coastlines` and `COBs` (either as file paths or as `<pyGPlates.FeatureCollection>` objects), as well as a `PlateReconstruction`
-object, and a reconstruction `time`. 
-
-```python
-coastlines, continents, COBs = gDownload.get_topology_geometries()
-time = 50 #Ma
-gPlot = gplately.plot.PlotTopologies(model, time, coastlines, continents, COBs)
-```
-Below are some continents, coastlines, COBs, ridges and transforms, trenches, subduction teeth and
-seafloor age grids plotted using `PlotTopologies`!
-
-![ReconstructionImage](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/plot_topologies_img.png)
-
 ### The `Points` object
 
 ... can be used to reconstruct the positions of geological point features and calculate their underlying plate velocities 
 through geological time. 
 
 ```python
 pt_lon = np.array([-107.662152, -58.082792, 17.483189, 133.674590, 80.412876])
 pt_lat = np.array([48.797807, -12.654857, 11.884395, -26.415630, 31.368509])
 
 # Call the Points object: pass the PlateReconstruction object, and the latitudes and longitudes of the seed points!
 gpts = gplately.Points(model, pt_lon, pt_lat)
 ```
 ![PointData](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/surface_hotspot_plumes.png)
 
-
 ### The `Raster` object
 
 ...can be used to read, resample and resize assorted raster data like `netCDF4` seafloor age grids, continental grids and ETOPO
 relief rasters. You can also reconstruct raster data back through geological time!
 
 ```python
 etopo = gdownload.get_raster("ETOPO1_tif")
@@ -167,26 +196,42 @@
 )
 ```
 
 Below is a plot of the [ETOPO1 global relief raster](https://www.ncei.noaa.gov/products/etopo-global-relief-model) at present day, and reconstructed to 50Ma:
 
 ![RasterImg](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/etopo_reconstruction.png)
 
+### The `PlotTopologies` object
+
+... can be used to visualise reconstructed feature geometries through time. To call the object, pass a set of `continents`, 
+`coastlines` and `COBs` (either as file paths or as `<pyGPlates.FeatureCollection>` objects), as well as a `PlateReconstruction`
+object, and a reconstruction `time`. 
+
+```python
+coastlines, continents, COBs = gDownload.get_topology_geometries()
+time = 50 #Ma
+gPlot = gplately.plot.PlotTopologies(model, time, coastlines, continents, COBs)
+```
+Below are some continents, coastlines, COBs, ridges and transforms, trenches, subduction teeth and
+seafloor age grids plotted using `PlotTopologies`!
+
+![ReconstructionImage](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/plot_topologies_img.png)
+
 
 ## Sample workflows
 
 To see GPlately in action, launch a Jupyter Notebook environment and check out the [sample notebooks](./Notebooks):
 
 - [__01 - Getting Started__](https://github.com/GPlates/gplately/blob/master/Notebooks/01-GettingStarted.ipynb): A brief overview of how to initialise GPlately's main objects
 - [__02 - Plate Reconstructions__](https://github.com/GPlates/gplately/blob/master/Notebooks/02-PlateReconstructions.ipynb): Setting up a `PlateReconstruction` object, reconstructing geological data through time 
 - [__03 - Working with Points__](https://github.com/GPlates/gplately/blob/master/Notebooks/03-WorkingWithPoints.ipynb): Setting up a `Points` object, reconstructing seed point locations through time with. This notebook uses point data from the Paleobiology Database (PBDB).
 - [__04 - Velocity Basics__](https://github.com/GPlates/gplately/blob/master/Notebooks/04-VelocityBasics.ipynb): Calculating plate velocities, plotting velocity vector fields
 - [__05 - Working with Feature Geometries__](https://github.com/GPlates/gplately/blob/master/Notebooks/05-WorkingWithFeatureGeometries.ipynb): Processing and plotting assorted polyline, polygon and point data from [GPlates 2.3's sample data sets](https://www.earthbyte.org/gplates-2-3-software-and-data-sets/)
 - [__06 - Rasters__](https://github.com/GPlates/gplately/blob/master/Notebooks/06-Rasters.ipynb): Reading, resizing, resampling raster data, and linearly interpolating point data onto raster data
 - [__07 - Plate Tectonic Stats__](https://github.com/GPlates/gplately/blob/master/Notebooks/07-WorkingWithPlateTectonicStats.ipynb): Using [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) to calculate and plot subduction zone and ridge data (convergence/spreading velocities, subduction angles, subduction zone and ridge lengths, crustal surface areas produced and subducted etc.) 
-- [__08 - Predicting Slab Dip__](https://github.com/GPlates/gplately/blob/master/Notebooks/08-PredictingSlabDip.ipynb): Predicting the average slab dip angle of subducting oceanic lithosphere.
+- [__08 - Predicting Slab Flux__](https://github.com/GPlates/gplately/blob/master/Notebooks/08-PredictingSlabFlux.ipynb): Predicting the average slab dip angle of subducting oceanic lithosphere.
 - [__09 - Motion Paths and Flowlines__](https://github.com/GPlates/gplately/blob/master/Notebooks/09-CreatingMotionPathsAndFlowlines.ipynb): Using pyGPlates to create motion paths and flowines of points on a tectonic plate to illustrate the plate's trajectory through geological time.
 - [__10 - SeafloorGrid__](https://github.com/GPlates/gplately/blob/master/Notebooks/10-SeafloorGrids.ipynb): Defines the parameters needed to set up a `SeafloorGrid` object, and demonstrates how to produce age and spreading rate grids from a set of plate reconstruction model files.
 
 ## API Documentation
 
 Documentation of GPlately's objects and methods can be found [here](https://gplates.github.io/gplately/)!
```

### Comparing `gplately-0.3.3/gplately/data.py` & `gplately-0.4/gplately/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re as _re
+import numpy as _np
 from numpy import size as _size
 
 # ============ LINKS FOR DOWNLOADING PLATE RECONSTRUCTION FILES ON-THE-FLY ==============
 """ This auxiliary script contains links to download plate model data from web servers
 such as EarthByte's webDAV server. These links are accessed by GPlately's DataServer object
 and downloaded into the "gplately" folder in your machine's cache via Pooch.
 """
@@ -14,33 +15,74 @@
     ):
     """Search through link databases and time arrays (or single integer
     time) for requested download links."""
 
     all_urls = []
     for collection, url in data_dictionary.items():
         if collection_identifier.lower() == collection.lower():
+
             if time is not None:
-                if _size(time) == 1:
-                    all_urls.append(url[0].format(str(int(time))))
-                    return all_urls
-                else:
+
+                valid_times_dict = DataCollection(collection_identifier).plate_model_valid_reconstruction_times()
+
+                for collection, valid_times in list(valid_times_dict.items()):
+                    if collection_identifier.lower() == collection.lower():
+                        min_time = valid_times[0]
+                        max_time = valid_times[1]
+
+                if isinstance(time, list) or isinstance(time, _np.ndarray):
+
                     for t in time:
-                        url_current_time = url[0].format(str(int(t)))
-                        all_urls.append(url_current_time)
+                        if t < min_time or t > max_time:
+                            all_urls.append(None)
+                        else:
+                            url_current_time = url[0].format(str(int(t)))
+                            all_urls.append(url_current_time)
                     return all_urls
+
+                else:
+                    if time < min_time or time > max_time:
+                        all_urls.append(None)
+                    else:
+                        all_urls.append(url[0].format(str(int(time))))
+                        return all_urls
             else:
                 return url
 
 
 def _studyname(study_name):
     """Locate the citation surname for a particular identifier string
     (i.e. "Muller" for "Muller2019")."""
     name = _re.findall(r'[A-Za-z]+|\d+', study_name)[0]
     return name
 
+
+def _rasters():
+
+        database = {
+
+            "ETOPO1_grd" : ["https://www.ngdc.noaa.gov/mgg/global/relief/ETOPO1/data/ice_surface/grid_registered/netcdf/ETOPO1_Ice_g_gmt4.grd.gz"],
+            "ETOPO1_tif" : ["https://www.ngdc.noaa.gov/mgg/global/relief/ETOPO1/image/color_etopo1_ice_low.tif.gz"],
+        }
+        return database
+
+
+def _feature_data():
+    """Assorted feature data from EarthByte's GPlates 2.3 sample data repository."""
+
+    database = {
+
+        "SeafloorFabric" : ["https://www.earthbyte.org/webdav/ftp/earthbyte/GPlates/GPlates2.3_GeoData/Individual/SeafloorFabric.zip"],
+        "Johansson2018" : ["https://www.earthbyte.org/webdav/ftp/earthbyte/GPlates/GPlates2.3_GeoData/Individual/IgneousProvinces.zip"],
+        "Whittaker2015" : ["https://www.earthbyte.org/webdav/ftp/earthbyte/GPlates/GPlates2.3_GeoData/Individual/IgneousProvinces.zip"],
+        "Hotspots" : ["https://www.earthbyte.org/webdav/ftp/earthbyte/GPlates/GPlates2.3_GeoData/Individual/Hotspots.zip"]
+    }
+    return database
+
+
 class DataCollection(object):
     """GPlately's collection of plate model data is a dictionary where
     the plate model's identifier string is the key, and values are 
     lists containing any relevant file download links."""
 
     def __init__(self, file_collection):
         """Uses a string to identify the needed plate model, taken from
@@ -109,34 +151,34 @@
             "Clennett2020_S2013" : ["https://www.earthbyte.org/webdav/ftp/Data_Collections/Clennett_etal_2020_G3/Clennett_etal_2020_S2013.zip"],
 
         }
 
         return database
 
 
-    def plate_model_max_reconstruction_times(self):
+    def plate_model_valid_reconstruction_times(self):
 
         database = {
 
-            "Cao2020" : [1000],
-            "Muller2019" : [250], 
-            "Muller2016" : [240],
-            "Clennett2020" : [170],
-            "Seton2012" : [200],
-            "Merdith2021" : [1000],
-            "Matthews2016" : [410], 
-            "Merdith2017" : [410], 
-            "Li2008" : [410],
+            "Cao2020" : [0, 1000],
+            "Muller2019" : [0, 250], 
+            "Muller2016" : [0, 230],
+            "Clennett2020" : [0, 170],
+            "Seton2012" : [0, 200],
+            "Merdith2021" : [0, 1000],
+            "Matthews2016" : [0, 410], 
+            "Merdith2017" : [0, 410], 
+            "Li2008" : [0, 410],
             # "Pehrsson2015" : [25], (First implement continuous rotation)
-            "TorsvikCocks2017" : [410],
-            "Young2019" : [410], 
-            "Scotese2008" : [410],      
-            "Golonka2007" : [410],
-            "Clennett2020_M2019" : [170],
-            "Clennett2020_S2013" : [170],
+            "TorsvikCocks2017" : [0, 410],
+            "Young2019" : [0, 410], 
+            "Scotese2008" : [0, 410],      
+            "Golonka2007" : [0, 410],
+            "Clennett2020_M2019" : [0, 170],
+            "Clennett2020_S2013" : [0, 170],
 
         }  
         return database
 
 
     def rotation_strings_to_ignore(self):
 
@@ -323,31 +365,8 @@
 
         strings = [
 
             "DO_NOT",
             "OLD",
             "__MACOSX",
         ]
-        return strings
-
-
-    def rasters(self):
-
-        database = {
-
-            "ETOPO1_grd" : ["https://www.ngdc.noaa.gov/mgg/global/relief/ETOPO1/data/ice_surface/grid_registered/netcdf/ETOPO1_Ice_g_gmt4.grd.gz"],
-            "ETOPO1_tif" : ["https://www.ngdc.noaa.gov/mgg/global/relief/ETOPO1/image/color_etopo1_ice_low.tif.gz"],
-        }
-        return database
-
-
-    def feature_data(self):
-        """Assorted feature data from EarthByte's GPlates 2.3 sample data repository."""
-
-        database = {
-
-            "SeafloorFabric" : ["https://www.earthbyte.org/webdav/ftp/earthbyte/GPlates/GPlates2.3_GeoData/Individual/SeafloorFabric.zip"],
-            "Johansson2018" : ["https://www.earthbyte.org/webdav/ftp/earthbyte/GPlates/GPlates2.3_GeoData/Individual/IgneousProvinces.zip"],
-            "Whittaker2015" : ["https://www.earthbyte.org/webdav/ftp/earthbyte/GPlates/GPlates2.3_GeoData/Individual/IgneousProvinces.zip"],
-            "Hotspots" : ["https://www.earthbyte.org/webdav/ftp/earthbyte/GPlates/GPlates2.3_GeoData/Individual/Hotspots.zip"]
-        }
-        return database
+        return strings
```

### Comparing `gplately-0.3.3/gplately/download.py` & `gplately-0.4/gplately/download.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,26 +55,63 @@
         ext = ".decomp"
     else:
         processor = None
         ext = ""
     return processor, ext
 
 
-def _path_of_cached_file(url):
-    """Determine the full path to the cache where the file in `url` 
-    will be downloaded to."""
+def path_of_cached_file(url, model_name=None):
+    """Determine the absolute path where the file(s) from `url` 
+    will be downloaded to.
+
+    Parameters
+    ----------
+    url : str
+        The full download URL for the file passed as a string.
+
+    model_name : str, default None
+        An optional substring that ideally describes/labels the file.
+        This will help name the file(s) when it is downloaded to the 
+        gplately cache (this directory can be
+        found using `gplately.download.path_to_cache()`). 
+        """
+
     cached_filename = _pooch.utils.unique_file_name(url)
-    path = _pooch.utils.cache_location(
-        _os_cache('gplately'), 
-        env=None, 
-        version=None
-    )
+    cached_filename = _remove_hash(cached_filename)
+    path = path_to_cache()
+
+    processor_to_use, processor_extension = _determine_processor(url)
+
+    # If the requested files need processing (i.e. zip, gz folders)
+    if processor_extension:
+        # Are they from plate models? These typically are the .zip folders for plate models
+        if model_name:
+            cached_filename  = str(path) + '/' + model_name + processor_extension+'/'
+            unprocessed_path = str(path) + '/' + model_name
+            #cached_filename = cached_filename = str(path) + '/' + model_name
+
+        # If not from plate models but need processing, i.e. ETOPO1
+        else:
+            cached_filename = str(path) + '/' + "gplately_"+_parse_url_for_filenames(url) + processor_extension+'/'
+            unprocessed_path = str(path) + '/' + "gplately_"+_parse_url_for_filenames(url)
+            #cached_filename = "gplately_"+_parse_url_for_filenames(url) 
+
+    # If the requested files do not need processing, like standalone .nc files:
+    else:
+        if model_name:
+            cached_filename = str(path) + '/' + model_name + "_" + _parse_url_for_filenames(url)
+            unprocessed_path = None
+        else:
+            cached_filename = str(path) + '/' + "gplately_"+_parse_url_for_filenames(url)
+            unprocessed_path = None
+      
     _pooch.utils.make_local_storage(path)
     full_path = path.resolve() / cached_filename
-    return full_path
+
+    return full_path, unprocessed_path
 
 
 def _extract_processed_files(processed_directory):
     """Return a list of all full filenames from a given directory 
     in the GPlately cache.
     """
     if _os.path.isdir(processed_directory):
@@ -82,69 +119,185 @@
         for root, dirs, files in _os.walk(processed_directory):
             for file in files:
                 fnames.append(_os.path.join(root,file))
         return(fnames)
     elif _os.path.isfile(str(processed_directory)):
         return(processed_directory)
 
+
+def path_to_cache():
+    """Determine the absolute path to the system gplately cache. 
+    """
+    path = _pooch.utils.cache_location(
+        _os_cache('gplately'), 
+        env=None, 
+        version=None
+    )
+    return path
+
+
+def clear_cache():
+    """Clear the `gplately` cache directory. 
+
+    The absolute path of this directory can be found by running
+    [gplately.download.path_to_cache()](file:///Users/laurenilano/gplately/api/gplately/download.html#gplately.download.path_to_cache).
+
+    Caution - when called, all files in /path/to/caches/gplately will
+    be deleted. This action cannot be undone.
+    """
+    cache_path = path_to_cache()
+    _shutil.rmtree(str(cache_path))
+    _pooch.utils.make_local_storage(str(cache_path))
+    return
+
     
+def _parse_url_for_filenames(url, return_hash=False):
+    # Determine the filename of an E-Tag txt file
+    md5 = _hashlib.md5(url.encode()).hexdigest()
+    fname = _os.path.basename(_pooch.utils.parse_url(url)["path"])
+    fname = fname[-(255 - len(md5) - 1) :]
+    if return_hash:
+        return str(fname), str(md5)
+    else:
+        return str(fname)
+
+
 def _get_url_etag(url):
     """Obtain the E-Tag of a web server URL. 
     
     The E-Tag identifies a resource under a URL. If the resource
     is modified, a new E-Tag is generated. DataServer uses the
     E-Tag to determine whether local copies of plate model files
     available from a web server need to be updated to match the
     version on the web server.
     """
     # Determine E-Tag of the URL
     etag = str(_requests.head(url).headers.get("ETag"))
 
     # Determine the filename of an E-Tag txt file
-    md5 = _hashlib.md5(url.encode()).hexdigest()
-    fname = _pooch.utils.parse_url(url)["path"].split("/")[-1]
-    fname = fname[-(255 - len(md5) - 1) :]
-    unique_name = f"{md5}-{fname}".split(".")[0]+"-ETAG.txt"
+    parsed_fname, filehash = _parse_url_for_filenames(url, return_hash=True)
+
+    unique_name = filehash + "-ETAG.txt"
+
     cachepath = str(
         _pathlib.Path(
             _os.path.expanduser(str(_os_cache('gplately'))))
     )
-    text_path = cachepath+"/"+unique_name 
+
+    text_path = _os.path.join(cachepath, unique_name)
     return(etag, text_path)
     
     
 def _save_url_etag_to_txt(etag, text_path):
     """Write an E-Tag to a text file.
     """       
     # Write E-Tag to a text file on the GPlately cache. 
     text_file = open(text_path, "w")
     text_file.write(etag)
     text_file.close()
     
-    
-def _first_time_download_from_web(url):
+
+def _match_url_to_extension(url):
+    url = str(url)
+    if url.endswith(".nc"):
+        return ".nc"
+    elif url.endswith(".jpg"):
+        return ".jpg"
+    elif url.endswith(".png"):
+        return ".png"
+    elif url.endswith(".tif"):
+        return ".tif"
+
+
+def _first_time_download_from_web(url, model_name=None, verbose=True):
     """
     # Provided a web connection to a server can be established,
     download the files from the URL into the GPlately cache.
     """
+
     if _test_internet_connection(url):
-        fnames = _retrieve(
-                url=url,
-                known_hash=None,  
-                downloader=_HTTPDownloader(progressbar=True),
-                path=_os_cache('gplately'),
-                processor=_determine_processor(url)[0]
-        )
+
+        if not verbose:
+            logger = _pooch.get_logger()
+            log_level = logger.level
+            logger.setLevel("WARNING")
+
+        # The filename pooch saves the requested file is derived from
+        # one of four permutations:
+        # 1. File is from a plate model and needs processing (i.e. zip --> unzip)
+        # 2. File is from a plate model and does not need processing (i.e. .nc age grids)
+        # 3. File is not from a plate model but needs processing (i.e. ETOPO, .grd.gz --> .decomp)
+        # 4. File is not from a plate model and does not need processing
+        processor_to_use, processor_extension = _determine_processor(url)
+
+        # If the requested files need processing (i.e. zip, gz folders)
+        if processor_extension:
+            # Are they from plate models? These typically are the .zip folders for plate models
+            if model_name:
+                # Download the files with a naming structure like:
+                # /path/to/cache/gplately/model_name+processor_extension
+                used_fname = model_name
+                fnames = _retrieve(
+                        url=url,
+                        known_hash=None,  
+                        downloader=_HTTPDownloader(progressbar=verbose),
+                        fname=used_fname,
+                        path=_os_cache('gplately'),
+                        processor=processor_to_use
+                )
+            # If not from plate models but need processing, i.e. ETOPO1
+            else:
+                # Download the files with a naming structure like:
+                # /path/to/cache/gplately/file_name-as_inteded_in_url+processor_extension
+                used_fname = "gplately_"+_parse_url_for_filenames(url)
+                fnames = _retrieve(
+                    url=url,
+                    known_hash=None,  
+                    downloader=_HTTPDownloader(progressbar=verbose),
+                    fname=used_fname,
+                    path=_os_cache('gplately'),
+                    processor=processor_to_use
+                )
+        # If the requested files do not need processing, like standalone .nc files:
+        else:
+            # Are they from plate models? These typically are age or spreading rate grids
+            if model_name:
+                # Download the files with a naming structure like:
+                # /path/to/cache/gplately/file_name-as_inteded_in_url+processor_extension
+                used_fname = model_name+"_"+_parse_url_for_filenames(url)
+                fnames = _retrieve(
+                        url=url,
+                        known_hash=None,  
+                        downloader=_HTTPDownloader(progressbar=verbose),
+                        fname=used_fname,
+                        path=_os_cache('gplately'),
+                        processor=processor_to_use
+                )
+            # If not from plate models and do not need processing,
+            else:
+                used_fname = "gplately_"+_parse_url_for_filenames(url)
+                fnames = _retrieve(
+                        url=url,
+                        known_hash=None,  
+                        downloader=_HTTPDownloader(progressbar=verbose),
+                        fname=used_fname,
+                        path=_os_cache('gplately'),
+                        processor=processor_to_use
+                )
+        
+        if not verbose:
+            logger.setLevel(log_level)
+
         # Get the URL's E-Tag for the first time
         etag, textfilename = _get_url_etag(url)
         _save_url_etag_to_txt(etag, textfilename)
-        return(fnames, etag, textfilename)
-    
+        return(fnames, etag, textfilename, used_fname)
+
     
-def download_from_web(url, verbose=True, download_changes=True):
+def download_from_web(url, verbose=True, download_changes=True, model_name=None):
     """Download a file from a `url` into the `gplately` cache.
     
     Notes
     -----
     After the file belonging to the given `url` is downloaded 
     to the `gplately` cache once, subsequent runs of 
     `download_from_web` with this `url` will not redownload 
@@ -200,51 +353,131 @@
     ------
     ConnectionError
         If a connection to the web server and file(s) in the given `url` is
         unsuccessful (because there is no internet access, and/or the `url`
         is incorrect) and no version of the requested file(s) have been
         cached before. In this case, nothing is returned. 
     """
-    # Identify the final filename from the given url within the GPlately cache
-    full_path = _path_of_cached_file(url)
+
+
+    #   NOTE: We need a way to verify the existence of requested file(s) in the gplately
+    #   cache to determine whether a file needs to be installed, updated, or re-accessed 
+    #   from the cache. Every time a file is installed for the first time,
+    #   DataServer creates a directory called `full_path`. Its existence verifies the 
+    #   existence
+    #
+    #   The nature of `full_path` is dependent on the file-type:
+    #
+    #   .zip files will be downloaded and expanded in an inside folder:
+    #   
+    #   /path/to/cache/gplately/fname.zip.unzip/
+    #
+    #   Thus, for zips, `full_path` is a directory that ends in ".zip.unzip":
+    #
+    #   For example: /Users/laurenilano/Library/Caches/gplately/Muller2019.zip.unzip/
+
+    #   Other types of files that need processing, like .gz --> .decomp, aren't
+    #   expanded in an internal folder. This is also the case for files that do not 
+    #   need processing, e.g. ".nc" files. In these cases, `full_path` is the exact
+    #   directory that the cached file is saved to.
+    # 
+    #
+    #   For example: /Users/laurenilano/Library/Caches/gplately/Muller_etal_2019_Tectonics_v2.0_AgeGrid-100.nc
+    #
+    #   `full_path` is an empty directory for non-zips, and is the parent directory of
+    #   unzipped contents in ".zip" URLs. 
+    #
+    #   Why do we need `full_path`?
+    #   We search the top-level gplately cache directory for the `full_path` directory as it is
+    #   installed with the requested files. Its existence verifies the
+    #   existence of the requested file(s), and thus to decide whether to install the
+    #   files or re-access existing cached versions. This also helps with E-Tag versioning
+    #   in instances where the download URL remains the same but its contents may have changed
+    #   since the file(s) were last cached. 
     
-    # If the files are not yet on the cache,
-    if not _os.path.isfile(str(full_path)):
-        
+    full_path, unprocessed_path = path_of_cached_file(url, model_name)
+
+    # If the file required processing (zips make a directory to unzip in, and .gz for example
+    # makes a file just saved to the top-level directory), and the directory or file is not 
+    # yet on the cache,
+    if _determine_processor(url)[1] and not (
+        _os.path.isdir(str(full_path)) or _os.path.isfile(str(full_path))
+        ):
+
+        # ...and if a connection to the web server can be established,
+        # download files from the URL and create a textfile for this URL's E-Tag
+        if _test_internet_connection(url):
+            fnames, etag, textfilename, used_fname = _first_time_download_from_web(
+                url, 
+                model_name=model_name,
+                verbose=verbose
+            )
+            if verbose:
+                print("Requested files downloaded to the GPlately cache folder!")
+            return(fnames)
+    
+        # ... if a connection to the web server cannot be established
+        else:
+            raise ConnectionError(
+                    "A connection to {} could not be made. Please check your internet connection and/or ensure the URL is correct. No file from the given URL has been cached to {} yet - nothing has been returned.".format(url, full_path.parent))
+
+
+    # If the file does not require processing, it did not open up a directory, so check isfile,
+    # and if the file is not yet on the cache,
+    elif not _determine_processor(url)[1] and not _os.path.isfile(str(full_path)):
         # ...and if a connection to the web server can be established,
         # download files from the URL and create a textfile for this URL's E-Tag
         if _test_internet_connection(url):
-            fnames, etag, textfilename = _first_time_download_from_web(url)
+            fnames, etag, textfilename, used_fname = _first_time_download_from_web(
+                url, 
+                model_name=model_name,
+                verbose=verbose
+            )
             if verbose:
                 print("Requested files downloaded to the GPlately cache folder!")
             return(fnames)
     
         # ... if a connection to the web server cannot be established
         else:
             raise ConnectionError(
                     "A connection to {} could not be made. Please check your internet connection and/or ensure the URL is correct. No file from the given URL has been cached to {} yet - nothing has been returned.".format(url, full_path.parent))
 
+
     # If the files have been downloaded before...
     else:
         #... and if a connection to the web server can be made...
         if _test_internet_connection(url):
             
+            _, local_etag_txtfile = _get_url_etag(url)
+
             # If the newest version of the files in `url` must be cached 
             # at all times, perform E-Tag comparisons:
             if download_changes:
 
-                # Get the path to the file's E-Tag textfile
-                local_etag_txtfile = str(full_path).split(".")[0]+"-ETAG.txt"
+                # Walk through the top-level cache directory to find an E-Tag textfile unique to the URL
+                etag_exists = False
+
+                cache_path = str(path_to_cache())
+                if _os.path.isfile(local_etag_txtfile):
+                    etag_exists = True
 
                 # If an e-tag text file does not exist, erase the cached files
                 # and download the latest version from the web server. This, in turn,
                 # creates an e-tag textfile for this version.
-                if not _os.path.isfile(local_etag_txtfile):
-                    _os.remove(str(full_path))
-                    fnames, etag, local_etag_txtfile = _first_time_download_from_web(url)
+                if not etag_exists:
+                    if _os.path.isdir(full_path):
+                        _shutil.rmtree(str(full_path))
+                    elif _os.path.isfile(full_path):
+                        _os.remove(full_path)
+
+                    fnames, etag, local_etag_txtfile, used_fname = _first_time_download_from_web(
+                        url, 
+                        model_name=model_name,
+                        verbose=verbose
+                    )
                     return(fnames)
 
                 # If the e-tag textfile exists for the local files,
                 else: 
                     if verbose:
                         print("Checking whether the requested files need to be updated...")
 
@@ -258,49 +491,66 @@
                     # If the local and remote e-tags are unequal, the web-server URL 
                     # contains an updated version of the cached files.
                     if str(remote_etag) != str(local_etag):
                         if verbose:
                             print("Yes - updating requested files...")
                         
                         # Update the e-tag textfile with this newly-identified URL e-tag
-                        _save_url_etag_to_txt(remote_etag, remote_etag_textfile)
+                        _save_url_etag_to_txt(remote_etag, local_etag_txtfile)
 
                         # Re-download the file, and process it if need-be.
                         with _pooch.utils.temporary_file(path=str(full_path.parent)) as tmp:
-                            downloader = _HTTPDownloader(progressbar=True)
+                            downloader = _HTTPDownloader(progressbar=verbose)
                             downloader(url, tmp, _pooch) 
                             _shutil.move(tmp, str(full_path))
                             processor=_determine_processor(url)[0]
-                            processor(str(full_path), "update", None)
-                            # determine_processor gives the file its processed filename
-                            processed_file = str(full_path)+_determine_processor(url)[1]
 
+                            # If the file to update needs processing, pass the unprocessed file's
+                            # absolute path to the processor
+                            if unprocessed_path:
+                                processor(str(unprocessed_path), "update", None)
+                            
+                        # full_path holds the files to return to the user, irrespective of whether
+                        # proceessing was needed
                         if verbose:
                             print("Requested files downloaded to the GPlately cache folder!")
-                        return(_extract_processed_files(processed_file))
+                        return(_extract_processed_files(str(full_path)))
 
                     # If the e-tags are equal, the local and remote files are the same.
                     # Just return the file(s) as-is.
                     else:
                         if verbose:
                             print("Requested files are up-to-date!")
-                        return(_extract_processed_files(
-                            str(full_path)+_determine_processor(url)[1]))
-            
+
+                        # If files were processed once, return the processed files.
+                        if _determine_processor(url):
+                            if str(full_path).endswith(_determine_processor(url)[1]):
+                                return(_extract_processed_files((str(full_path))))
+                            else:
+                                return(_extract_processed_files(
+                                    str(full_path)+_determine_processor(url)[1]))
+                        # If not, return as-is.
+                        else:
+                            return(_extract_processed_files(
+                                str(full_path)+_match_url_to_extension(url)))
+
             # If file versioning doesn't matter, just keep returning the cached files.
             else:
-                fnames, etag, local_etag_txtfile = _first_time_download_from_web(url)
+                fnames, etag, local_etag_txtfile = _first_time_download_from_web(url, model_name)
                 return(fnames)
                 
         # If a connection to the web server could not be made, and the files exist in
         # the GPlately cache, just return the files as-is.
         else:
             print("No connection to {} established. The requested file(s) (potentially older versions) exist in the GPlately cache ({}) and have been returned.".format(url, full_path.parent))
+            #print(str(full_path)+_determine_processor(url)[1])
             return(_extract_processed_files(
-                    str(full_path)+_determine_processor(url)[1]))
+                    str(full_path)))
+            # This created zip.unzip.unzip, so i deleted it but not sure if this will affect other files. 
+            # return(_extract_processed_files(str(full_path)+_determine_processor(url)[1]))
 
 
 
 def _collect_file_extension(fnames, file_extension):
     """Searches cached directory for filenames with a specified extension(s)."""
     sorted_fnames = []
     file_extension=tuple(file_extension)
@@ -311,52 +561,50 @@
 
 
 def _str_in_folder(fnames, strings_to_include=None, strings_to_ignore=None):
     fnames_to_ignore = []
     fnames_to_include = []
     sorted_fnames = []
     for i, fname in enumerate(fnames):
-        parent_directory = '/'.join(fname.split("/")[:-1])
+        parent_directory = _os.path.dirname(fname)
         if strings_to_ignore is not None:
             for s in strings_to_ignore:
                 if s in parent_directory:
                     fnames_to_ignore.append(fname)
             sorted_fnames = list(set(fnames) - set(fnames_to_ignore))
 
     if strings_to_include is not None:
         for fname in sorted_fnames:
-            parent_directory = '/'.join(fname.split("/")[:-1])
+            parent_directory = _os.path.dirname(fname)
             for s in strings_to_include:
                 if s in parent_directory:
                     fnames_to_include.append(fname)
         sorted_fnames = list(set(sorted_fnames).intersection(set(fnames_to_include)))
     return sorted_fnames
 
 
 def _str_in_filename(fnames, strings_to_include=None, strings_to_ignore=None):
-    sorted_fnames = []
-    if strings_to_include is not None:
-        for f in fnames:
-            f_splitted = f.split("/")[-1]
-            check = [s for s in strings_to_include if s.lower() in f_splitted.lower()]
-            if check:
-                sorted_fnames.append(f)
-    else:
-        sorted_fnames = fnames
-    
-    if strings_to_ignore is not None:
-        more_sorted = []
-        for f in sorted_fnames:
-            f_splitted = f.split("/")[-1]
-            check = [s for s in strings_to_ignore if s.lower() in f_splitted.lower()]
-            if not check:
-                more_sorted.append(f)
-        return(more_sorted)
-    else:
-        return(sorted_fnames)
+    out = []
+    def filter_func(fname):
+        basename = _os.path.basename(fname)
+        keep = False
+        if strings_to_include is None:
+            keep = True
+        else:
+            for s in strings_to_include:
+                if s.lower() in basename.lower():
+                    keep = True
+                    break
+        if strings_to_ignore is not None:
+            for s in strings_to_ignore:
+                if s.lower() in basename.lower():
+                    keep = False
+                    break
+        return keep
+    return list(filter(filter_func, fnames))
 
 
 def _check_gpml_or_shp(fnames):
     """For topology features, returns GPML by default. Searches for ESRI Shapefiles 
     instead if GPML files not found."""
     sorted_fnames = []
     for file in fnames:
@@ -445,14 +693,243 @@
     elif filetype == "png":
         extensions.append(".png")
     elif filetype == "TIFF":
         extensions.append(".tif")
     return extensions
 
 
+def get_raster(raster_id_string=None, verbose=True):
+    """Downloads assorted raster data that are not associated with the plate 
+    reconstruction models supported by GPlately's `DataServer`. Stores rasters in the 
+    "gplately" cache.
+
+    Currently, gplately supports the following rasters and images:
+
+    * __[ETOPO1](https://www.ngdc.noaa.gov/mgg/global/)__: 
+        * Filetypes available : TIF, netCDF (GRD)
+        * `raster_id_string` = `"ETOPO1_grd"`, `"ETOPO1_tif"` (depending on the requested format)
+        * A 1-arc minute global relief model combining lang topography and ocean bathymetry.
+        * Citation: doi:10.7289/V5C8276M
+
+
+    Parameters
+    ----------
+    raster_id_string : str, default=None
+        A string to identify which raster to download.
+
+    Returns
+    -------
+    a gplately.Raster object
+        A gplately.Raster object containing the raster data. The gridded data can be extracted 
+        into a numpy ndarray or MaskedArray by appending `.data` to the variable assigned to `get_raster()`.
+
+        For example:
+
+            graster = gplately.download.get_raster(raster_id_string, verbose)
+
+            graster_data = graster.data
+
+        where `graster_data` is a numpy ndarray. This array can be visualised using 
+        `matplotlib.pyplot.imshow` on a `cartopy.mpl.GeoAxis` GeoAxesSubplot 
+        (see example below).
+
+    Raises
+    ------
+    ValueError
+        * if a `raster_id_string` is not supplied.
+
+    Notes
+    -----
+    Rasters obtained by this method are (so far) only reconstructed to present-day. 
+
+    Examples
+    --------
+    To download ETOPO1 and plot it on a Mollweide projection:
+
+        import gplately
+        import numpy as np
+        import matplotlib.pyplot as plt
+        import cartopy.crs as ccrs
+
+        etopo1 = gplately.download.get_raster("ETOPO1_tif")
+
+        fig = plt.figure(figsize=(18,14), dpi=300)
+        ax = fig.add_subplot(111, projection=ccrs.Mollweide(central_longitude = -150))
+        etopo1.imshow(ax) 
+
+    """
+    from matplotlib import image
+    if raster_id_string is None:
+        raise ValueError(
+            "Please specify which raster to download."
+        )
+    #filetype = "."+"_".split(raster_id_string)[-1]
+
+    archive_formats = tuple([".gz", ".xz", ".bz2"])
+    grid_extensions = tuple([".grd", ".nc"])
+
+    # Set to true if we find the given collection in database
+    found_collection = False
+    raster_filenames = []
+    database = _gplately.data._rasters()
+
+    for collection, zip_url in database.items():
+        # Isolate the raster name and the file type
+        #raster_name = collection.split("_")[0]
+        #raster_type = "."+collection.split("_")[-1]
+        if (raster_id_string.lower() == collection.lower()):
+            raster_filenames = download_from_web(zip_url[0], verbose)
+            found_collection = True
+            break
+
+    if found_collection is False:
+        raise ValueError("{} not in collection database.".format(raster_id_string))
+    else:
+        # If the downloaded raster is a grid, process it with the gplately.Raster object
+        if any(grid_extension in raster_filenames for grid_extension in grid_extensions):
+            raster = _gplately.grids.Raster(data=raster_filenames)
+
+        # Otherwise, the raster is an image; use imread to process
+        else:
+            raster_matrix = image.imread(raster_filenames)
+            raster = _gplately.grids.Raster(data=raster_matrix)
+
+        if raster_id_string.lower() == "etopo1_tif":
+            raster.lats = raster.lats[::-1]
+        if raster_id_string.lower() == "etopo1_grd":
+            raster._data = raster._data.astype(float)
+
+    return raster
+
+
+def get_feature_data(feature_data_id_string=None, verbose=True):
+    """Downloads assorted geological feature data from web servers (i.e. 
+    [GPlates 2.3 sample data](https://www.earthbyte.org/gplates-2-3-software-and-data-sets/))
+    into the "gplately" cache.
+
+    Currently, gplately supports the following feature data:
+
+    * __Large igneous provinces from Johansson et al. (2018)__
+
+        Information
+        -----------
+        * Formats: .gpmlz
+        * `feature_data_id_string` = `Johansson2018`
+
+        Citations
+        ---------
+        * Johansson, L., Zahirovic, S., and Müller, R. D., In Prep, The 
+        interplay between the eruption and weathering of Large Igneous Provinces and 
+        the deep-time carbon cycle: Geophysical Research Letters.
+
+
+    - __Large igneous province products interpreted as plume products from Whittaker 
+    et al. (2015)__.
+
+        Information
+        -----------
+        * Formats: .gpmlz, .shp
+        * `feature_data_id_string` = `Whittaker2015`
+        
+        Citations
+        ---------
+        * Whittaker, J. M., Afonso, J. C., Masterton, S., Müller, R. D., 
+        Wessel, P., Williams, S. E., & Seton, M. (2015). Long-term interaction between 
+        mid-ocean ridges and mantle plumes. Nature Geoscience, 8(6), 479-483. 
+        doi:10.1038/ngeo2437.
+
+
+    - __Seafloor tectonic fabric (fracture zones, discordant zones, V-shaped structures, 
+    unclassified V-anomalies, propagating ridge lineations and extinct ridges) from 
+    Matthews et al. (2011)__
+
+        Information
+        -----------
+        * Formats: .gpml
+        * `feature_data_id_string` = `SeafloorFabric`
+
+        Citations
+        ---------
+        * Matthews, K.J., Müller, R.D., Wessel, P. and Whittaker, J.M., 2011. The 
+        tectonic fabric of the ocean basins. Journal of Geophysical Research, 116(B12): 
+        B12109, DOI: 10.1029/2011JB008413. 
+
+
+    - __Present day surface hotspot/plume locations from Whittaker et al. (2013)__
+
+        Information
+        -----------
+        * Formats: .gpmlz
+        * `feature_data_id_string` = `Hotspots`
+
+        Citation
+        --------
+        * Whittaker, J., Afonso, J., Masterton, S., Müller, R., Wessel, P., 
+        Williams, S., and Seton, M., 2015, Long-term interaction between mid-ocean ridges and 
+        mantle plumes: Nature Geoscience, v. 8, no. 6, p. 479-483, doi:10.1038/ngeo2437.
+
+    
+    Parameters
+    ----------
+    feature_data_id_string : str, default=None
+        A string to identify which feature data to download to the cache (see list of supported
+        feature data above).
+
+    Returns
+    -------
+    feature_data_filenames : instance of <pygplates.FeatureCollection>, or list of instance <pygplates.FeatureCollection>
+        If a single set of feature data is downloaded, a single pyGPlates `FeatureCollection` 
+        object is returned. Otherwise, a list containing multiple pyGPlates `FeatureCollection` 
+        objects is returned (like for `SeafloorFabric`). In the latter case, feature reconstruction 
+        and plotting may have to be done iteratively.
+
+    Raises
+    ------
+    ValueError
+        If a `feature_data_id_string` is not provided.
+
+    Examples
+    --------
+    For examples of plotting data downloaded with `get_feature_data`, see GPlately's sample 
+    notebook 05 - Working With Feature Geometries [here](https://github.com/GPlates/gplately/blob/master/Notebooks/05-WorkingWithFeatureGeometries.ipynb).
+    """
+    if feature_data_id_string is None:
+        raise ValueError(
+            "Please specify which feature data to fetch."
+        )
+
+    database = _gplately.data._feature_data()
+
+    found_collection = False
+    for collection, zip_url in database.items():
+        if feature_data_id_string.lower() == collection.lower():
+            found_collection = True
+            feature_data_filenames = _collection_sorter(
+                _collect_file_extension(
+                download_from_web(zip_url[0], verbose), [".gpml", ".gpmlz"]
+                ),
+                collection
+            )
+
+            break
+
+    if found_collection is False:
+        raise ValueError("{} are not in GPlately's DataServer.".format(feature_data_id_string))
+
+    feat_data = _FeatureCollection()
+    if len(feature_data_filenames) == 1:
+            feat_data.add(_FeatureCollection(feature_data_filenames[0]))
+            return feat_data
+    else:    
+        feat_data=[]
+        for file in feature_data_filenames:
+            feat_data.append(_FeatureCollection(file))
+        return feat_data
+
+
 class DataServer(object):
     """Uses [Pooch](https://www.fatiando.org/pooch/latest/) to download plate reconstruction 
     feature data from plate models and other studies that are stored on web servers 
     (e.g. EarthByte's [webDAV server](https://www.earthbyte.org/webdav/ftp/Data_Collections/)). 
     
     If the `DataServer` object and its methods are called for the first time, i.e. by:
 
@@ -810,15 +1287,15 @@
         for collection, url in database.items():
 
             # Only continue if the user's chosen collection exists in our database
             if self.file_collection.lower() == collection.lower():
                 found_collection = True
                 if len(url) == 1:
                     fnames = _collection_sorter(
-                        download_from_web(url[0], verbose), self.file_collection
+                        download_from_web(url[0], verbose, model_name=self.file_collection), self.file_collection
                     )
                     rotation_filenames = _collect_file_extension(
                         _str_in_folder(
                             _str_in_filename(fnames,
                                 strings_to_ignore=DataCollection.rotation_strings_to_ignore(self)
                             ),
                         strings_to_ignore=DataCollection.rotation_strings_to_ignore(self)
@@ -853,27 +1330,27 @@
                     )
                     #print(static_polygon_filenames)
                     for stat in static_polygon_filenames:
                         static_polygons.add(_FeatureCollection(stat))
 
                 else:
                     for file in url[0]:
-                        rotation_filenames.append(_collect_file_extension(download_from_web(file, verbose), [".rot"]))
+                        rotation_filenames.append(_collect_file_extension(download_from_web(file, verbose, model_name=self.file_collection), [".rot"]))
                         rotation_model = _RotationModel(rotation_filenames)
 
                     for file in url[1]:
-                        topology_filenames.append(_collect_file_extension(download_from_web(file, verbose), [".gpml"]))
+                        topology_filenames.append(_collect_file_extension(download_from_web(file, verbose, model_name=self.file_collection), [".gpml"]))
                         for file in topology_filenames:
                             topology_features.add(_FeatureCollection(file))
 
                     for file in url[2]:
                         static_polygon_filenames.append(
                             _check_gpml_or_shp(
                                 _str_in_folder(
-                                    _str_in_filename(download_from_web(url[0], verbose), 
+                                    _str_in_filename(download_from_web(url[0], verbose, model_name=self.file_collection), 
                                         strings_to_include=DataCollection.static_polygon_strings_to_include(self)
                                     ),    
                                         strings_to_ignore=DataCollection.static_polygon_strings_to_ignore(self)
                                 )
                             )   
                         )
                         for stat in static_polygon_filenames:
@@ -970,15 +1447,15 @@
 
                 if len(url) == 1:
                     # Some plate models do not have reconstructable geometries i.e. Li et al. 2008
                     if url[0] is None:
                         break
                     else:
                         fnames = _collection_sorter(
-                            download_from_web(url[0], verbose), self.file_collection
+                            download_from_web(url[0], verbose, model_name=self.file_collection), self.file_collection
                         )
                         coastlines = _check_gpml_or_shp(
                             _str_in_folder(
                                 _str_in_filename(
                                     fnames,
                                     strings_to_include=DataCollection.coastline_strings_to_include(self),
                                     strings_to_ignore=DataCollection.coastline_strings_to_ignore(self)
@@ -1006,35 +1483,35 @@
                                 strings_to_ignore=DataCollection.COB_strings_to_ignore(self)
                             )
                         )
                 else:
                     for file in url[0]:
                         if url[0] is not None:
                             coastlines.append(_str_in_filename(
-                                download_from_web(file, verbose), 
+                                download_from_web(file, verbose, model_name=self.file_collection), 
                                 strings_to_include=["coastline"])
                             )
                             coastlines = _check_gpml_or_shp(coastlines)
                         else:
                             coastlines = []
 
                     for file in url[1]:
                         if url[1] is not None:
                             continents.append(_str_in_filename(
-                                download_from_web(file, verbose), 
+                                download_from_web(file, verbose, model_name=self.file_collection), 
                                 strings_to_include=["continent"])
                             )
                             continents = _check_gpml_or_shp(continents)
                         else:
                             continents = []
 
                     for file in url[2]:
                         if url[2] is not None:
                             COBs.append(_str_in_filename(
-                                download_from_web(file, verbose), 
+                                download_from_web(file, verbose, model_name=self.file_collection), 
                                 strings_to_include=["cob"])
                             )
                             COBs = _check_gpml_or_shp(COBs)
                         else:
                             COBs = []
                 break
 
@@ -1101,17 +1578,28 @@
         ----------
         time : int, or list of int, default=None
             Request an age grid from one (an integer) or multiple reconstruction times (a
             list of integers).
 
         Returns
         -------
-        raster_array : MaskedArray
-            A masked array containing the netCDF4 age grid ready for plotting or for
-            passing into GPlately's `Raster` object for raster manipulation.
+        a gplately.Raster object
+            A gplately.Raster object containing the age grid. The age grid data can be extracted 
+            into a numpy ndarray or MaskedArray by appending `.data` to the variable assigned to 
+            `get_age_grid()`.
+
+            For example:
+
+                gdownload = gplately.DataServer("Muller2019")
+
+                graster = gdownload.get_age_grid(time=100)
+
+                graster_data = graster.data
+
+            where `graster_data` is a numpy ndarray. 
 
         Raises
         -----
         ValueError
             If `time` (a single integer, or a list of integers representing reconstruction
             times to extract the age grids from) is not passed.
 
@@ -1137,22 +1625,44 @@
 
             age_grids = gDownload.get_age_grid([0, 1, 100])
             
         """
         age_grids = []
         age_grid_links = DataCollection.netcdf4_age_grids(self, time)
 
+        if not isinstance(time, list):
+            time = [time]
+
+        # For a single time passed that isn't in the valid time range, 
         if not age_grid_links:
-            raise ValueError("{} age grids are not on GPlately's DataServer.".format(self.file_collection))
+            raise ValueError(
+                "{} {}Ma age grids are not on GPlately's DataServer.".format(
+                    self.file_collection, 
+                    time[0]
+                )
+            )
 
-        for link in age_grid_links:
-            age_grid_file = download_from_web(link, self.verbose)
-            age_grid = _gplately.grids.read_netcdf_grid(age_grid_file)
+        # For a list of times passed...
+        for i, link in enumerate(age_grid_links):
+            if not link:
+                raise ValueError(
+                    "{} {}Ma age grids are not on GPlately's DataServer.".format(
+                        self.file_collection,
+                        time[i]
+                    )
+                )
+            age_grid_file = download_from_web(
+                link, 
+                verbose=self.verbose, 
+                model_name=self.file_collection
+            )
+            age_grid = _gplately.grids.Raster(data=age_grid_file)
             age_grids.append(age_grid)
 
+        # One last check to alert user if the masked array grids were not processed properly
         if not age_grids:
             raise ValueError("{} netCDF4 age grids not found.".format(self.file_collection))
 
         if len(age_grids) == 1:
             return age_grids[0]
         else: 
             return age_grids
@@ -1177,17 +1687,28 @@
         ----------
         time : int, or list of int, default=None
             Request a spreading grid from one (an integer) or multiple reconstruction 
             times (a list of integers).
 
         Returns
         -------
-        raster_array : MaskedArray
-            A masked array containing the netCDF4 spreading rate grid ready for 
-            plotting or for passing into GPlately's `Raster` object.
+        a gplately.Raster object
+            A gplately.Raster object containing the spreading rate grid. The spreading 
+            rate grid data can be extracted into a numpy ndarray or MaskedArray by 
+            appending `.data` to the variable assigned to `get_spreading_rate_grid()`.
+
+            For example:
+
+                gdownload = gplately.DataServer("Clennett2020")
+
+                graster = gdownload.get_spreading_rate_grid(time=100)
+
+                graster_data = graster.data
+
+            where `graster_data` is a numpy ndarray.
 
         Raises
         -----
         ValueError
             If `time` (a single integer, or a list of integers representing reconstruction
             times to extract the spreading rate grids from) is not passed.
 
@@ -1215,31 +1736,69 @@
 
             spreading_rate_grids = gDownload.get_spreading_rate_grid([0, 1, 100])
             
         """
         spreading_rate_grids = []
         spreading_rate_grid_links = DataCollection.netcdf4_spreading_rate_grids(self, time)
 
-        if not spreading_rate_grid_links:
-            raise ValueError("{} spreading rate grids are not on GPlately's DataServer.".format(self.file_collection))
+        if not isinstance(time, list):
+            time = [time]
 
-        for link in spreading_rate_grid_links:
-            spreading_rate_grid_file = download_from_web(link, self.verbose)
-            spreading_rate_grid = _gplately.grids.read_netcdf_grid(spreading_rate_grid_file)
+        # For a single time passed that isn't in the valid time range, 
+        if not spreading_rate_grid_links:
+            raise ValueError(
+                "{} {}Ma spreading rate grids are not on GPlately's DataServer.".format(
+                    self.file_collection,
+                    time[0]
+                )
+            )
+        # For a list of times passed...
+        for i, link in enumerate(spreading_rate_grid_links):
+            if not link:
+                raise ValueError(
+                    "{} {}Ma spreading rate grids are not on GPlately's DataServer.".format(
+                        self.file_collection,
+                        time[i]
+                    )
+                )
+            spreading_rate_grid_file = download_from_web(
+                link, 
+                verbose=self.verbose, 
+                model_name=self.file_collection
+            )
+            spreading_rate_grid = _gplately.grids.Raster(data=spreading_rate_grid_file)
             spreading_rate_grids.append(spreading_rate_grid)
 
+        # One last check to alert user if the masked array grids were not processed properly
         if not spreading_rate_grids:
             raise ValueError("{} netCDF4 seafloor spreading rate grids not found.".format(self.file_collection))
 
         if len(spreading_rate_grids) == 1:
             return spreading_rate_grids[0]
         else: 
             return spreading_rate_grids
 
 
+    def get_valid_times(self):
+        """Returns a tuple of the valid plate model time range, (min_time, max_time).
+        """
+        all_model_valid_times = DataCollection.plate_model_valid_reconstruction_times(self)
+
+        min_time = None
+        max_time = None
+        for plate_model_name, valid_times in list(all_model_valid_times.items()):
+            if plate_model_name.lower() == self.file_collection.lower():
+                min_time = valid_times[0]
+                max_time = valid_times[1]
+        if not min_time and not max_time:
+            raise ValueError("Could not find the valid reconstruction time of {}".format(self.file_collection))
+
+        return (min_time, max_time)
+
+
     def get_raster(self, raster_id_string=None):
         """Downloads assorted raster data that are not associated with the plate 
         reconstruction models supported by GPlately's `DataServer`. Stores rasters in the 
         "gplately" cache.
 
         Currently, `DataServer` supports the following rasters and images:
 
@@ -1253,17 +1812,29 @@
         Parameters
         ----------
         raster_id_string : str, default=None
             A string to identify which raster to download.
 
         Returns
         -------
-        raster_filenames : ndarray or MaskedArray
-            An ndarray or MaskedArray of the cached raster. This can be plotted using 
-            `matplotlib.pyplot.imshow` on a `cartopy.mpl.GeoAxis` GeoAxesSubplot (see example below).
+        a gplately.Raster object
+            A gplately.Raster object containing the raster data. The gridded data can be extracted 
+            into a numpy ndarray or MaskedArray by appending `.data` to the variable assigned to `get_raster()`.
+
+            For example:
+
+                gdownload = gplately.DataServer("Muller2019")
+
+                graster = gdownload.get_raster(raster_id_string, verbose)
+
+                graster_data = graster.data
+
+            where `graster_data` is a numpy ndarray. This array can be visualised using 
+            `matplotlib.pyplot.imshow` on a `cartopy.mpl.GeoAxis` GeoAxesSubplot 
+            (see example below).
 
         Raises
         ------
         ValueError
             * if a `raster_id_string` is not supplied.
 
         Notes
@@ -1282,49 +1853,15 @@
             gdownload = gplately.DataServer("Muller2019")
             etopo1 = gdownload.get_raster("ETOPO1_tif")
             fig = plt.figure(figsize=(18,14), dpi=300)
             ax = fig.add_subplot(111, projection=ccrs.Mollweide(central_longitude = -150))
             ax2.imshow(etopo1, extent=[-180,180,-90,90], transform=ccrs.PlateCarree()) 
 
         """
-        from matplotlib import image
-        if raster_id_string is None:
-            raise ValueError(
-                "Please specify which raster to download."
-            )
-        #filetype = "."+"_".split(raster_id_string)[-1]
-
-        archive_formats = tuple([".gz", ".xz", ".bz2"])
-        grid_extensions = tuple([".grd", ".nc"])
-
-        # Set to true if we find the given collection in database
-        found_collection = False
-        raster_filenames = []
-        database = DataCollection.rasters(self)
-
-        for collection, zip_url in database.items():
-            # Isolate the raster name and the file type
-            #raster_name = collection.split("_")[0]
-            #raster_type = "."+collection.split("_")[-1]
-            if (raster_id_string.lower() == collection.lower()):
-                raster_filenames = download_from_web(zip_url[0], self.verbose)
-                found_collection = True
-                break
-
-        if found_collection is False:
-            raise ValueError("{} not in collection database.".format(raster_id_string))
-        else:
-            # If the downloaded raster is a grid, process it with the gplately.Raster object
-            if any(grid_extension in raster_filenames for grid_extension in grid_extensions):
-                raster_matrix = _gplately.grids.Raster(data=raster_filenames).data
-
-            # Otherwise, the raster is an image; use imread to process
-            else:
-                raster_matrix = image.imread(raster_filenames)
-        return raster_matrix
+        return get_raster(raster_id_string, self.verbose)
 
 
     def get_feature_data(self, feature_data_id_string=None):
         """Downloads assorted geological feature data from web servers (i.e. 
         [GPlates 2.3 sample data](https://www.earthbyte.org/gplates-2-3-software-and-data-sets/))
         into the "gplately" cache.
 
@@ -1415,15 +1952,15 @@
         notebook 05 - Working With Feature Geometries [here](https://github.com/GPlates/gplately/blob/master/Notebooks/05-WorkingWithFeatureGeometries.ipynb).
         """
         if feature_data_id_string is None:
             raise ValueError(
                 "Please specify which feature data to fetch."
             )
 
-        database = DataCollection.feature_data(self)
+        database = _gplately.data._feature_data()
 
         found_collection = False
         for collection, zip_url in database.items():
             if feature_data_id_string.lower() == collection.lower():
                 found_collection = True
                 feature_data_filenames = _collection_sorter(
                     _collect_file_extension(
```

### Comparing `gplately-0.3.3/gplately/geometry.py` & `gplately-0.4/gplately/geometry.py`

 * *Files identical despite different names*

### Comparing `gplately-0.3.3/gplately/gpml.py` & `gplately-0.4/gplately/gpml.py`

 * *Files identical despite different names*

### Comparing `gplately-0.3.3/gplately/grids.py` & `gplately-0.4/gplately/grids.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,32 @@
 * Grids with invalid (NaN-type) data cells can have their NaN entries replaced 
 with the values of their nearest valid neighbours. 
 
 Classes
 -------
 * RegularGridInterpolator
 * Raster
-* TimeRaster
 """
 import warnings
 from multiprocessing import cpu_count
 
 import matplotlib.colors
 import matplotlib.pyplot as plt
 import numpy as np
 import pygplates
 from cartopy.crs import PlateCarree as _PlateCarree
 from cartopy.mpl.geoaxes import GeoAxes as _GeoAxes
 from rasterio.enums import MergeAlg
 from rasterio.features import rasterize as _rasterize
 from rasterio.transform import from_bounds as _from_bounds
 from scipy.interpolate import RegularGridInterpolator as _RGI
-from scipy.ndimage import distance_transform_edt
+from scipy.ndimage import (
+    distance_transform_edt,
+    map_coordinates,
+)
 from scipy.spatial import cKDTree as _cKDTree
 from scipy.spatial.transform import Rotation as _Rotation
 
 from .geometry import pygplates_to_shapely
 from .reconstruction import PlateReconstruction as _PlateReconstruction
 
 __all__ = [
@@ -98,17 +100,33 @@
     if invalid is None:
         invalid = np.isnan(data)
         if masked_array:
             invalid += mask_fill_value
     ind = distance_transform_edt(invalid, return_distances=False, return_indices=True)
     return data[tuple(ind)]
 
-def read_netcdf_grid(filename, return_grids=False, resample=None):
+
+def realign_grid(array, lons, lats):
+    mask_lons = lons > 180
+
+    # realign to -180/180
+    if mask_lons.any():
+        dlon = np.diff(lons).mean()
+        array = np.hstack([array[:,mask_lons], array[:,~mask_lons]])
+        lons  = np.hstack([lons[mask_lons] - 360 - dlon, lons[~mask_lons]])
+
+    if lats[0] > lats[-1]:
+        array = np.flipud(array)
+        lats = lats[::-1]
+
+    return array, lons, lats
+
+def read_netcdf_grid(filename, return_grids=False, realign=False, resample=None):
     """Read a `netCDF` (.nc) grid from a given `filename` and return its data as a
-    `MaskedArray`. Re-align longitudes of raster data from -180 to 180 degrees.
+    `MaskedArray`.
 
     Notes
     -----
     If a `resample` tuple is passed with X and Y spacings (`spacingX`, `spacingY`), 
     the gridded data in `filename` will be resampled with these resolutions. 
 
     By default, only the `MaskedArray` is returned to the user. However, if `return_grids` is 
@@ -121,61 +139,100 @@
     Parameters
     ----------
     filename : str
         Full path to the `netCDF` raster file.
         
     return_grids : bool, optional, default=False
         If set to `True`, returns lon, lat arrays associated with the grid data.
+
+    realign : bool, optional, default=False
+        if set to `True`, realigns grid to -180/180 and flips the array if the
+        latitudinal coordinates are decreasing.
         
     resample : tuple, optional, default=None
         If passed as `resample = (spacingX, spacingY)`, the given `netCDF` grid is resampled 
         with these x and y resolutions.
 
     Returns
     -------
-    cdf_grid_z : MaskedArray
+    grid_z : MaskedArray
         A `MaskedArray` containing the gridded data from the supplied netCDF4 `filename`. 
         Entries' longitudes are re-aligned between -180 and 180 degrees.
 
-    cdf_lon, cdf_lat : 1d MaskedArrays
+    lon, lat : 1d MaskedArrays
         `MaskedArrays` encasing longitude and latitude variables belonging to the 
         supplied netCDF4 file. Longitudes are rescaled between -180 and 180 degrees. 
         An example output of `cdf_lat` is:
 
             masked_array(data=[-90. , -89.9, -89.8, ...,  89.8,  89.9,  90. ], mask=False, fill_value=1e+20)
     """
+
+    def find_label(keys, labels):
+        for label in labels:
+            if label in keys:
+                return label
+        return None
+
+
     import netCDF4
-    
+
+    # possible permutations of lon/lat/z
+    label_lon = ['lon', 'lons', 'longitude', 'x', 'east', 'easting', 'eastings']
+    label_lat = ['lat', 'lats', 'latitude', 'y', 'north', 'northing', 'northings']
+    label_z   = ['z', 'data', 'values']
+
+    # add capitalise and upper case permutations
+    label_lon = label_lon + [label.capitalize() for label in label_lon] + [label.upper() for label in label_lon]
+    label_lat = label_lat + [label.capitalize() for label in label_lat] + [label.upper() for label in label_lat]
+    label_z = label_z + [label.capitalize() for label in label_z] + [label.upper() for label in label_z]
+
     # open netCDF file and re-align from -180, 180 degrees
     with netCDF4.Dataset(filename, 'r') as cdf:
-        cdf_grid = cdf["z"]
-        try:
-            cdf_lon = cdf['lon'][:]
-            cdf_lat = cdf['lat'][:]
-        except:
-            cdf_lon = cdf['x'][:]
-            cdf_lat = cdf['y'][:]
-            
-        cdf_lon_mask = cdf_lon[:] > 180
-        dlon = np.diff(cdf_lon[:]).mean()
+        keys = cdf.variables.keys()
         
-        if cdf_lon_mask.any():
-            cdf_grid_z = np.hstack([cdf_grid[:,cdf_lon_mask], cdf_grid[:,~cdf_lon_mask]])
-            cdf_lon = np.hstack([cdf_lon[cdf_lon_mask]-360-dlon, cdf_lon[~cdf_lon_mask]])
-        else:
-            cdf_grid_z = cdf_grid[:]
+        # find the names of variables
+        key_z   = find_label(keys, label_z)
+        key_lon = find_label(keys, label_lon)
+        key_lat = find_label(keys, label_lat)
+
+        if key_lon is None or key_lat is None:
+            raise ValueError("Cannot find x,y or lon/lat coordinates in netcdf")
+        if key_z is None:
+            raise ValueError("Cannot find z data in netcdf")
+
+        # extract data from cdf variables
+        cdf_grid = cdf[key_z][:]
+        cdf_lon  = cdf[key_lon][:]
+        cdf_lat  = cdf[key_lat][:]
+
+    if realign:
+        # realign longitudes to -180/180 dateline
+        cdf_grid_z, cdf_lon, cdf_lat = realign_grid(cdf_grid, cdf_lon, cdf_lat)
+    else:
+        cdf_grid_z = cdf_grid
 
     # resample
     if resample is not None:
         spacingX, spacingY = resample
         lon_grid = np.arange(cdf_lon.min(), cdf_lon.max()+spacingX, spacingX)
         lat_grid = np.arange(cdf_lat.min(), cdf_lat.max()+spacingY, spacingY)
         lonq, latq = np.meshgrid(lon_grid, lat_grid)
-        interp = RegularGridInterpolator((cdf_lat, cdf_lon), cdf_grid_z, method='nearest', bounds_error=False)
-        cdf_grid_z = interp((latq, lonq))
+        original_extent = (
+            cdf_lon[0],
+            cdf_lon[-1],
+            cdf_lat[0],
+            cdf_lat[-1],
+        )
+        cdf_grid_z = sample_grid(
+            lonq, latq,
+            cdf_grid_z,
+            method="nearest",
+            extent=original_extent,
+            return_indices=False,
+        )
         cdf_lon = lon_grid
         cdf_lat = lat_grid
             
     # Fix grids with 9e36 as the fill value for nan. 
     #cdf_grid_z.fill_value = float('nan')
     #cdf_grid_z.data[cdf_grid_z.data > 1e36] = cdf_grid_z.fill_value
     
@@ -233,18 +290,18 @@
         cdf_lat = cdf.createVariable('lat', lat_grid.dtype, ('lat',), zlib=True)
         cdf_lon[:] = lon_grid
         cdf_lat[:] = lat_grid
 
         # Units for Geographic Grid type
         cdf_lon.units = "degrees_east"
         cdf_lon.standard_name = 'lon'
-        cdf_lon.actual_range = [np.nanmin(lon_grid), np.nanmax(lon_grid)]
+        cdf_lon.actual_range = [lon_grid[0], lon_grid[-1]]
         cdf_lat.units = "degrees_north"
         cdf_lat.standard_name = 'lat'
-        cdf_lat.actual_range = [np.nanmin(lat_grid), np.nanmax(lat_grid)]
+        cdf_lat.actual_range = [lat_grid[0], lat_grid[-1]]
 
         cdf_data = cdf.createVariable('z', grid.dtype, ('lat','lon'), zlib=True)
         # netCDF4 uses the missing_value attribute as the default _FillValue
         # without this, _FillValue defaults to 9.969209968386869e+36
         cdf_data.missing_value = np.nan
         cdf_data.standard_name = 'z'
         #Ensure pygmt registers min and max z values properly
@@ -456,90 +513,149 @@
         operations with all versions of scipy >1.0. 
         """
         idx_res = [np.where(yi <= .5, i, i + 1)
                    for i, yi in zip(indices, norm_distances)]
         return self.values[tuple(idx_res)]
 
 
-def sample_grid(lon, lat, grid, extent=[-180,180,-90,90], return_indices=False, return_distances=False, method='linear'):
-    """Sample point data with given `lon` and `lat` coordinates onto a `grid` using either a linear or nearest-neighbour 
-    interpolation `method`.
-
-    Notes
-    -----
-    If `return_indices` is set to `True`, the indices of raster points that were used as neighbouring sampling points
-    are returned as an array containing two arrays:
-
-    * array [0] is for the raster row coordinate (lat), and 
-    * array [1] is for the raster column (lon) coordinate.
-
-    An example output:
-
-        # The first array holds the rows of the raster where point data spatially falls near.
-        # The second array holds the columns of the raster where point data spatially falls near.
-        sampled_indices = [array([1019, 1019, 1019, ..., 1086, 1086, 1087]), array([2237, 2237, 2237, ...,  983,  983,  983])]
-
-    If `return_distances` is set to `True`, the distances between the raster sampling points and interpolated points 
-    are returned as an array containing two arrays:
-
-    * array [0] is for the latitudinal component of distance between the raster sampling point and the interpolated point.
-    * array [1] is for the longitudinal component of distance between the raster sampling point and the interpolated point.
-
-    An example output:
-
-        # The first array holds the lat-component of the normal dist, while the second array holds the lon-component.
-        sampled_dist = [array([5.30689060e-05, 3.47557804e-02, 1.03967049e-01, ..., 3.46526690e-02, 5.77772021e-01, 1.20890767e-01]), 
-        array([4.41756600e-04, 2.89440621e-01, 8.66576791e-01, ..., 4.08341107e-01, 3.74526858e-01, 3.40690957e-01])]
-
+def sample_grid(
+    lon,
+    lat,
+    grid,
+    method="linear",
+    extent="global",
+    origin=None,
+    return_indices=False,
+):
+    """Sample point data with given `lon` and `lat` coordinates onto a `grid`
+    using spline interpolation.
 
     Parameters
     ----------
-    lon, lat : 1d arrays
-        Two arrays each specifying the longitudes and latitudes of the points to interpolate on the grid.
-
-    grid : ndarray or MaskedArray
-        An array whose elements define a grid. The number of rows corresponds to the number of point latitudes, while
-        the number of columns corresponds to the number of point longitudes.
-
-    extent : 1D numpy array, default=[-180,180,-90,90]
-        A four-element array to specify the [min lon, max lon, min lat, max lat] with which to constrain lat and lon sampling
-        points with respect to the given grid. If no extents are supplied, full global extent is assumed. 
-
+    lon, lat : array_like
+        The longitudes and latitudes of the points to interpolate onto the
+        gridded data. Must be broadcastable to a common shape.
+    grid : Raster or array_like
+        An array whose elements define a grid. The number of rows corresponds
+        to the number of point latitudes, while the number of columns
+        corresponds to the number of point longitudes.
+    method : str or int; default: 'linear'
+        The order of spline interpolation. Must be an integer in the range
+        0-5. 'nearest', 'linear', and 'cubic' are aliases for 0, 1, and 3,
+        respectively.
+    extent : str or 4-tuple, default: 'global'
+        4-tuple to specify (min_lon, max_lon, min_lat, max_lat) extents
+        of the raster. If no extents are supplied, full global extent
+        [-180,180,-90,90] is assumed (equivalent to `extent='global'`).
+        For array data with an upper-left origin, make sure `min_lat` is
+        greater than `max_lat`, or specify `origin` parameter.
+    origin : {'lower', 'upper'}, optional
+        When `data` is an array, use this parameter to specify the origin
+        (upper left or lower left) of the data (overriding `extent`).
     return_indices : bool, default=False
-        Choose whether to return the row and column indices of points on the `grid` used to interpolate the point data. 
-
-    return_distances : bool, default=False
-        Choose whether to return the row and column normal distances between interpolated points and neighbouring 
-        sampling points.
-
-    method : str, default=’linear’
-        The method of interpolation to perform. Supported are "linear" and "nearest". Assumes “linear” by default.
+        Whether to return the row and column indices of the nearest grid
+        points.
 
     Returns
-    -----
-    output_tuple : tuple of ndarrays
-        By default, `output_tuple` has one ndarray - this holds the values of the grid data where interpolated points lie. 
-        If sample point indices and/or distances have been requested (by setting `return_indices` and/or `return_distances`
-        to `True`), these are returned as subsequent tuple elements. 
+    -------
+    numpy.ndarray
+        The values interpolated at the input points.
+    indices : 2-tuple of numpy.ndarray
+        The i- and j-indices of the nearest grid points to the input
+        points, only present if `return_indices=True`.
 
     Raises
     ------
     ValueError
-        * Raised if the string method supplied is not “linear” or “nearest”.
-        * Raised if the provided sample points for interpolation (xi) do not have the same dimensions as the supplied grid. 
-        * Raised if the provided sample points for interpolation include any point out of grid bounds. Alerts user which 
-        dimension (index) the point is located. Only raised if the RegularGridInterpolator attribute bounds_error is set 
-        to True. If suppressed, out-of-bound points are replaced with a set fill_value. 
+        If an invalid `method` is provided.
+    RuntimeWarning
+        If `lat` contains any invalid values outside of the interval
+        [-90, 90]. Invalid values will be clipped to this interval.
 
+    Notes
+    -----
+    If `return_indices` is set to `True`, the nearest array indices
+    are returned as a tuple of arrays, in (i, j) or (lat, lon) format.
+
+    An example output:
+
+        # The first array holds the rows of the raster where point data spatially falls near.
+        # The second array holds the columns of the raster where point data spatially falls near.
+        sampled_indices = (array([1019, 1019, 1019, ..., 1086, 1086, 1087]), array([2237, 2237, 2237, ...,  983,  983,  983]))
     """
-    interpolator = RegularGridInterpolator((np.linspace(extent[2], extent[3], grid.shape[0]),
-                                            np.linspace(extent[0], extent[1], grid.shape[1])),
-                                            grid, method=method)
+    order = {
+        "nearest": 0,
+        "linear": 1,
+        "cubic": 3,
+    }.get(method, method)
+    if order not in {0, 1, 2, 3, 4, 5}:
+        raise ValueError("Invalid `method` parameter: {}".format(method))
+
+    if isinstance(grid, Raster):
+        extent = grid.extent
+        grid = np.array(grid.data)
+    else:
+        extent = _parse_extent_origin(extent, origin)
+        grid = _check_grid(grid)
+
+    # Do not wrap from North to South Pole (or vice versa)
+    if np.any(np.abs(lat) > 90.0):
+        warnings.warn(
+            "Invalid values encountered in lat; clipping to [-90, 90]",
+            RuntimeWarning,
+        )
+        lat = np.clip(lat, -90.0, 90.0)
 
-    return interpolator(np.c_[lat, lon], return_indices=return_indices, return_distances=return_distances)
+    dx = (extent[1] - extent[0]) / (np.shape(grid)[1] - 1)
+    dy = (extent[3] - extent[2]) / (np.shape(grid)[0] - 1)
+    point_i = (lat - extent[2]) / dy
+    point_j = (lon - extent[0]) / dx
+
+    point_coords = np.row_stack(
+        (
+            np.ravel(point_i),
+            np.ravel(point_j),
+        )
+    )
+    if np.ndim(grid) == 2:
+        interpolated = map_coordinates(
+            np.array(grid, dtype="float"),
+            point_coords,
+            order=order,
+            mode="grid-wrap",
+            prefilter=order > 1,
+        )
+        interpolated = np.reshape(interpolated, np.shape(lon))
+    else:  # ndim(grid) == 3
+        depth = np.shape(grid)[2]
+        interpolated = []
+        for k in range(depth):
+            interpolated_k = map_coordinates(
+                grid[..., k],
+                point_coords,
+                order=order,
+                mode="grid-wrap",
+                prefilter=order > 1,
+            )
+            interpolated_k = np.reshape(
+                interpolated_k,
+                np.shape(lon),
+            )
+            interpolated.append(interpolated_k)
+        del interpolated_k
+        interpolated = np.stack(interpolated, axis=-1)
+
+    interpolated = interpolated.astype(grid.dtype)
+    if return_indices:
+        indices = (
+            np.rint(np.ravel(point_i)).astype(np.int_),
+            np.rint(np.ravel(point_j)).astype(np.int_),
+        )
+        return interpolated, indices
+    return interpolated
 
 
 def reconstruct_grid(
     grid,
     partitioning_features,
     rotation_model,
     to_time,
@@ -816,44 +932,51 @@
     key="plate_id",
     time=None,
     resx=1.0,
     resy=1.0,
     shape=None,
     extent="global",
     origin=None,
+    tessellate_degrees=0.1,
 ):
     """Rasterise GPlates objects at a given reconstruction time.
 
     This function is particularly useful for rasterising static polygons
     to extract a grid of plate IDs.
 
     Parameters
     ----------
-    features : valid argument for pygplates.FeaturesFunctionArgument
+    features : geometries or features
         `features` may be a single `pygplates.Feature`, a
         `pygplates.FeatureCollection`, a `str` filename,
         or a (potentially nested) sequence of any combination of the
         above types.
+        Alternatively, `features` may also be a sequence of geometry types
+        (`pygplates.GeometryOnSphere` or `pygplates.ReconstructionGeometry`).
+        In this case, `rotation_model` and `time` will be ignored, and
+        `key` must be an array_like of the same length as `features`.
     rotation_model : valid argument for pygplates.RotationModel, optional
         `rotation_model` may be a `pygplates.RotationModel`, a rotation
         feature collection (pygplates.FeatureCollection), a rotation filename
         (`str`), a rotation feature (`pygplates.Feature`), a sequence of
         rotation features, or a (potentially nested) sequence of any
         combination of the above types.
         Alternatively, if time not given, a rotation model is
         not usually required.
-    key : str, default "plate_id"
+    key : str or array_like, default "plate_id"
         The value used to create the rasterised grid. May be any of
         the following values:
         - "plate_id"
         - "conjugate_plate_id"
         - "from_age"
         - "to_age"
         - "left_plate"
         - "right_plate"
+        Alternatively, `key` may be a sequence of the same length as
+        `features`.
     time : float, optional
         Reconstruction time at which to perform rasterisation. If given,
         `rotation_model` must also be specified.
     resx, resy : float, default 1.0
         Resolution (in degrees) of the rasterised grid.
     shape : tuple, optional
         If given, the output grid will have the specified shape,
@@ -861,14 +984,18 @@
     extent : tuple or "global", default "global"
         Extent of the rasterised grid. Valid arguments are a tuple of
         the form (xmin, xmax, ymin, ymax), or the string "global",
         equivalent to (-180.0, 180.0, -90.0, 90.0).
     origin : {"upper", "lower"}, optional
         Origin (upper-left or lower-left) of the output array. By default,
         determined from `extent`.
+    tessellate_degrees : float, default 0.1
+        Densify pyGPlates geometries to this resolution before conversion.
+        Can be disabled by specifying `tessellate_degrees=None`, but this
+        may provide inaccurate results for low-resolution input geometries.
 
     Returns
     -------
     grid : numpy.ndarray
         The output array will have the shape specified in `shape`, if given.
         The origin of the array will be in the lower-left corner of
         the area specified in `extent`, unless `resx` or `resy` is negative.
@@ -889,23 +1016,21 @@
         "plate_id",
         "conjugate_plate_id",
         "from_age",
         "to_age",
         "left_plate",
         "right_plate",
     }
-    try:
+    if isinstance(key, str):
         key = key.lower()
-    except AttributeError as err:
-        raise TypeError("Invalid key type: {}".format(type(key))) from err
-    if key not in valid_keys:
-        raise ValueError(
-            "Invalid key: {}".format(key)
-            + "\nkey must be one of {}".format(valid_keys)
-        )
+        if key not in valid_keys:
+            raise ValueError(
+                "Invalid key: {}".format(key)
+                + "\nkey must be one of {}".format(valid_keys)
+            )
 
     extent = _parse_extent_origin(extent, origin)
     minx, maxx, miny, maxy = extent
 
     if minx > maxx:
         resx = -1.0 * np.abs(resx)
     if miny > maxy:
@@ -916,35 +1041,98 @@
         lats = np.linspace(miny, maxy, shape[0], endpoint=True)
     else:
         lons = np.arange(minx, maxx + resx, resx)
         lats = np.arange(miny, maxy + resy, resy)
     nx = lons.size
     ny = lats.size
 
-    if rotation_model is None:
-        if time is not None:
-            raise TypeError(
-                "Rotation model must be provided if `time` is not `None`"
+    try:
+        features = pygplates.FeaturesFunctionArgument(features).get_features()
+        geometries = None
+    except Exception as err:
+        if not str(err).startswith("Python argument types in"):
+            # Not a Boost.Python.ArgumentError
+            raise err
+        geometries = pygplates_to_shapely(
+            features,
+            tessellate_degrees=tessellate_degrees,
+        )
+        reconstructed = None
+
+    if geometries is None:
+        if rotation_model is None:
+            if time is not None:
+                raise TypeError(
+                    "Rotation model must be provided if `time` is not `None`"
+                )
+            rotation_model = pygplates.RotationModel(pygplates.Feature())
+            time = 0.0
+        features = pygplates.FeaturesFunctionArgument(features).get_features()
+        if time is None:
+            time = 0.0
+        time = float(time)
+
+        reconstructed = []
+        pygplates.reconstruct(
+            features,
+            rotation_model,
+            reconstructed,
+            time,
+        )
+        geometries = pygplates_to_shapely(
+            reconstructed,
+            tessellate_degrees=tessellate_degrees,
+        )
+    if not isinstance(geometries, list):
+        geometries = [geometries]
+
+    if isinstance(key, str):
+        values, fill_value, dtype = _get_rasterise_values(key, reconstructed)
+    else:
+        if not hasattr(key, "__len__"):
+            key = [key] * len(geometries)
+        if len(key) != len(geometries):
+            raise ValueError(
+                "Shape mismatch: len(key) = {}, ".format(len(key))
+                + "len(geometries) = {}".format(len(geometries))
             )
-        rotation_model = pygplates.RotationModel(pygplates.Feature())
-        time = 0.0
-    features = pygplates.FeaturesFunctionArgument(features).get_features()
-    if time is None:
-        time = 0.0
-    time = float(time)
-
-    reconstructed = []
-    pygplates.reconstruct(
-        features,
-        rotation_model,
-        reconstructed,
-        time,
+        values = np.array(key)
+        dtype = values.dtype
+        if dtype.kind == "u":
+            fill_value = np.iinfo(dtype).max
+        elif dtype.kind == "i":
+            fill_value = -1
+        elif dtype.kind == "f":
+            fill_value = np.nan
+        else:
+            raise TypeError("Unrecognised dtype for `key`: {}".format(dtype))
+
+    return _rasterise_geometries(
+        geometries=geometries,
+        values=values,
+        out_shape=(ny, nx),
+        fill_value=fill_value,
+        dtype=dtype,
+        merge_alg=MergeAlg.replace,
+        transform=_from_bounds(minx, miny, maxx, maxy, nx, ny),
     )
-    geometries = pygplates_to_shapely(reconstructed)
 
+
+def _get_rasterise_values(
+    key,
+    reconstructed,
+):
+    valid_keys = {
+        "plate_id",
+        "conjugate_plate_id",
+        "from_age",
+        "to_age",
+        "left_plate",
+        "right_plate",
+    }
     if key == "plate_id":
         values = [i.get_feature().get_reconstruction_plate_id() for i in reconstructed]
         fill_value = -1
         dtype = np.int32
     elif key == "conjugate_plate_id":
         values = [i.get_feature().get_conjugate_plate_id() for i in reconstructed]
         fill_value = -1
@@ -966,22 +1154,34 @@
         fill_value = -1
         dtype = np.int32
     else:
         raise ValueError(
             "Invalid key: {}".format(key)
             + "\nkey must be one of {}".format(valid_keys)
         )
+    return values, fill_value, dtype
+
 
+def _rasterise_geometries(
+    geometries,
+    values,
+    out_shape,
+    fill_value,
+    dtype,
+    transform,
+    merge_alg=MergeAlg.replace,
+):
+    shapes = zip(geometries, values)
     out = _rasterize(
-        shapes=zip(geometries, values),
-        out_shape=(ny, nx),
+        shapes=shapes,
+        out_shape=out_shape,
         fill=fill_value,
         dtype=dtype,
-        merge_alg=MergeAlg.replace,
-        transform=_from_bounds(minx, miny, maxx, maxy, nx, ny),
+        merge_alg=merge_alg,
+        transform=transform,
     )
     return np.flipud(out)
 
 
 rasterize = rasterise
 
 
@@ -1132,29 +1332,32 @@
             )
     return extent
 
 
 class Raster(object):
     """A class for working with raster data.
 
-    `Raster`'s functionalities inclue interpolating point data on rasters using Scipy's
-    RegularGridInterpolator, resampling rasters with new X and Y-direction spacings and
-    resizing rasters using new X and Y grid pixel resolutions. NaN-type data in rasters
-    can be replaced with the values of their nearest valid neighbours.
+    `Raster`'s functionalities inclue sampling data at points using spline
+    interpolation, resampling rasters with new X and Y-direction spacings and
+    resizing rasters using new X and Y grid pixel resolutions. NaN-type data
+    in rasters can be replaced with the values of their nearest valid
+    neighbours.
 
     Parameters
     ----------
-    plate_reconstruction : PlateReconstruction
-        Allows for the accessibility of PlateReconstruction object attributes. Namely, PlateReconstruction object
-        attributes rotation_model, topology_featues and static_polygons can be used in the points object if called using
-        “self.plate_reconstruction.X”, where X is the attribute.
-
     data : str or array-like
         The raster data, either as a filename (`str`) or array.
 
+    plate_reconstruction : PlateReconstruction
+        Allows for the accessibility of PlateReconstruction object attributes.
+        Namely, PlateReconstruction object attributes rotation_model,
+        topology_features and static_polygons can be used in the `Raster`
+        object if called using “self.plate_reconstruction.X”, where X is the
+        attribute.
+
     extent : str or 4-tuple, default: 'global'
         4-tuple to specify (min_lon, max_lon, min_lat, max_lat) extents
         of the raster. If no extents are supplied, full global extent
         [-180,180,-90,90] is assumed (equivalent to `extent='global'`).
         For array data with an upper-left origin, make sure `min_lat` is
         greater than `max_lat`, or specify `origin` parameter.
 
@@ -1172,44 +1375,44 @@
 
     **kwargs
         Handle deprecated arguments such as `PlateReconstruction_object`,
         `filename`, and `array`.
 
     Attributes
     ----------
-    plate_reconstruction : PlateReconstruction
-        An object of GPlately's `PlateReconstruction` class, like the
-        `rotation_model`, a set of reconstructable `topology_featues` and `static_polygons`
-        that belong to a particular plate model. These attributes can be used in the `Points`
-        object if called using “self.PlateReconstruction_object.X”, where X is the attribute.
-        This attribute can be modified after creation of the `Raster`.
-    extent : tuple of floats
-        Four-element array to specify [min lon, max lon, min lat, max lat] extents of any sampling
-        points. If no extents are supplied, full global extent [-180,180,-90,90] is assumed.
     data : ndarray, shape (ny, nx)
         Array containing the underlying raster data. This attribute can be
         modified after creation of the `Raster`.
+    plate_reconstruction : PlateReconstruction
+        An object of GPlately's `PlateReconstruction` class, like the
+        `rotation_model`, a set of reconstructable `topology_features` and
+        `static_polygons` that belong to a particular plate model. These
+        attributes can be used in the `Raster` object if called using
+        “self.plate_reconstruction.X”, where X is the attribute. This
+        attribute can be modified after creation of the `Raster`.
+    extent : tuple of floats
+        Four-element array to specify [min lon, max lon, min lat, max lat]
+        extents of any sampling points. If no extents are supplied, full
+        global extent [-180,180,-90,90] is assumed.
     lons : ndarray, shape (nx,)
         The x-coordinates of the raster data. This attribute can be modified
         after creation of the `Raster`.
     lats : ndarray, shape (ny,)
         The y-coordinates of the raster data. This attribute can be modified
         after creation of the `Raster`.
     origin : {'lower', 'upper'}
         The origin (lower or upper left) or the data array.
     filename : str or None
         The filename used to create the `Raster` object. If the object was
         created directly from an array, this attribute is `None`.
 
     Methods
     -------
-    interpolate(lons, lats, method='linear', return_indices=False,
-                return_distances=False)
-        Sample gridded data on a set of points using interpolation from
-        `scipy.interpolate.RegularGridInterpolator`.
+    interpolate(lons, lats, method='linear', return_indices=False)
+        Sample gridded data at a set of points using spline interpolation.
 
     resample(spacingX, spacingY, overwrite=False)
         Resamples the grid using X & Y-spaced lat-lon arrays, meshed with
         linear interpolation.
 
     resize(resX, resY, overwrite=False)
         Resizes the grid with a specific resolution and samples points
@@ -1222,36 +1425,37 @@
     reconstruct(time, fill_value=None, partitioning_features=None,
                 threads=1, anchor_plate_id=0, inplace=False)
         Reconstruct the raster from its initial time (`self.time`) to a new
         time.
     """
     def __init__(
         self,
-        plate_reconstruction=None,
         data=None,
+        plate_reconstruction=None,
         extent="global",
+        realign=False,
         resample=None,
         time=0.0,
         origin=None,
         **kwargs
     ):
         """Constructs all necessary attributes for the raster object.
 
         Note: either a str path to a netCDF file OR an ndarray representing a grid must be specified.
 
         Parameters
         ----------
+        data : str or array-like
+            The raster data, either as a filename (`str`) or array.
+
         plate_reconstruction : PlateReconstruction
             Allows for the accessibility of PlateReconstruction object attributes. Namely, PlateReconstruction object
             attributes rotation_model, topology_featues and static_polygons can be used in the points object if called using
             “self.plate_reconstruction.X”, where X is the attribute.
 
-        data : str or array-like
-            The raster data, either as a filename (`str`) or array.
-
         extent : str or 4-tuple, default: 'global'
             4-tuple to specify (min_lon, max_lon, min_lat, max_lat) extents
             of the raster. If no extents are supplied, full global extent
             [-180,180,-90,90] is assumed (equivalent to `extent='global'`).
             For array data with an upper-left origin, make sure `min_lat` is
             greater than `max_lat`, or specify `origin` parameter.
 
@@ -1318,29 +1522,31 @@
             )
         if isinstance(data, str):
             # Filename
             self._filename = data
             self._data, lons, lats = read_netcdf_grid(
                 data,
                 return_grids=True,
+                realign=realign,
                 resample=resample,
             )
             self._lons = lons
             self._lats = lats
 
         else:
             # numpy array
             self._filename = None
             extent = _parse_extent_origin(extent, origin)
             data = _check_grid(data)
             self._data = np.array(data)
             self._lons = np.linspace(extent[0], extent[1], self.data.shape[1])
             self._lats = np.linspace(extent[2], extent[3], self.data.shape[0])
-
-        self._update()
+            if realign:
+                # realign to -180,180 and flip grid
+                self._data, self._lons, self._lats = realign_grid(self._data, self._lons, self._lats)
 
         if (not isinstance(data, str)) and (resample is not None):
             self.resample(*resample, overwrite=True)
 
     @property
     def time(self):
         """The time step represented by the raster data."""
@@ -1361,15 +1567,14 @@
             raise ValueError(
                 "Shape mismatch: old dimensions are {}, new are {}".format(
                     np.shape(self.data),
                     z.shape,
                 )
             )
         self._data = z
-        self._update()
 
     @property
     def lons(self):
         """The x-coordinates of the raster data.
 
         Can be modified.
         """
@@ -1382,15 +1587,14 @@
             raise ValueError(
                 "Shape mismatch: data x-dimension is {}, new value is {}".format(
                     np.shape(self.data)[1],
                     x.size,
                 )
             )
         self._lons = x
-        self._update()
 
     @property
     def lats(self):
         """The y-coordinates of the raster data.
 
         Can be modified.
         """
@@ -1403,15 +1607,14 @@
             raise ValueError(
                 "Shape mismatch: data y-dimension is {}, new value is {}".format(
                     np.shape(self.data)[0],
                     y.size,
                 )
             )
         self._lats = y
-        self._update()
 
     @property
     def extent(self):
         """The spatial extent (x0, x1, y0, y1) of the data.
 
         If y0 < y1, the origin is the lower-left corner; else the upper-left.
         """
@@ -1429,27 +1632,32 @@
             return "lower"
         else:
             return "upper"
 
     @property
     def shape(self):
         """The shape of the data array."""
-        return self.data.shape
+        return np.shape(self.data)
 
     @property
     def size(self):
         """The size of the data array."""
-        return self.data.size
+        return np.size(self.data)
 
     @property
     def dtype(self):
         """The data type of the array."""
         return self.data.dtype
 
     @property
+    def ndim(self):
+        """The number of dimensions in the array."""
+        return np.ndim(self.data)
+
+    @property
     def filename(self):
         """The filename of the raster file used to create the object.
 
         If a NumPy array was used instead, this attribute is `None`.
         """
         return self._filename
 
@@ -1469,266 +1677,241 @@
             # Convert to a `PlateReconstruction` if possible
             try:
                 reconstruction = _PlateReconstruction(*reconstruction)
             except Exception:
                 reconstruction = _PlateReconstruction(reconstruction)
         self._plate_reconstruction = reconstruction
 
-    # Deprecated name of `plate_reconstruction` attribute
-    PlateReconstruction_object = plate_reconstruction
 
-    def _update(self):
-        """Stores the RegularGridInterpolator object's method for sampling gridded data at a set of 
-        point coordinates. 
-
-        Allows methods of the Raster object to access grid sampling functionalities. The gridded data 
-        used is the “data” attribute - either read from a netCDF4 file, or supplied as an ndarray. 
-        Points to sample are either variables of the netCDF4 file, or are generated from the “extent” 
-        attribute and scaled to fit the grid “data”.
+    def copy(self):
+        """ Returns a copy of the Raster
+        
+        Returns
+        -------
+        Raster
+            A copy of the current Raster object
         """
-        # store interpolation object
-        interpolator = RegularGridInterpolator((self.lats, self.lons), self.data, method='linear')
-        self._interpolator = interpolator
-
-
-    def interpolate(self, lons, lats, method='linear', return_indices=False, return_distances=False):
-        """Interpolate a set of point data (either linearly or through nearest-neighbour methods) 
-        onto the gridded data provided to the `Raster` object. 
-
-        Notes
-        -----
-        If `return_indices` is set to `True`, the indices of raster data used for interpolating the
-        points are returned as an array containing two arrays:
-
-        * array [0] is for the raster row coordinate (lat), and 
-        * array [1] is for the raster column (lon) coordinate.
-
-        An example output:
+        return Raster(self.data.copy(), self.plate_reconstruction, self.extent, self.time)
 
-            # The first array holds the rows of the raster where point data spatially falls near.
-            # The second array holds the columns of the raster where point data spatially falls near.
-            sampled_indices = [array([1019, 1019, 1019, ..., 1086, 1086, 1087]), array([2237, 2237, 2237, ...,  983,  983,  983])]
-
-
-        If `return_distances` is set to `True`, the distances between the raster data used for 
-        interpolating the points are returned as an array containing two arrays:
-
-        * array [0] is for the latitudinal component of distance between the raster sampling 
-        point and the interpolated point.
-        * array [1] is for the longitudinal component of distance between the raster sampling 
-        point and the interpolated point.
-
-        An example output:
+    def interpolate(
+        self,
+        lons,
+        lats,
+        method="linear",
+        return_indices=False,
+    ):
+        """Interpolate a set of point data onto the gridded data provided
+        to the `Raster` object.
 
-            # The first array holds the lat-component of the normal dist, while the second array holds the lon-component.
-            sampled_dist = [array([5.30689060e-05, 3.47557804e-02, 1.03967049e-01, ..., 3.46526690e-02, 5.77772021e-01, 1.20890767e-01]), 
-            array([4.41756600e-04, 2.89440621e-01, 8.66576791e-01, ..., 4.08341107e-01, 3.74526858e-01, 3.40690957e-01])]
-    
         Parameters
         ----------
-        lons, lats : array
-            1d arrays containing the longitudes and latitudes of the points to interpolate onto the
-            gridded data. 
-
-        method : str, default='linear'
-            The method of interpolation to perform. Supported are `linear` and `Nearest`. Assumes 
-            `linear` interpolation if `None` provided.  
-
+        lons, lats : array_like
+            The longitudes and latitudes of the points to interpolate onto the
+            gridded data. Must be broadcastable to a common shape.
+        method : str or int; default: 'linear'
+            The order of spline interpolation. Must be an integer in the range
+            0-5. 'nearest', 'linear', and 'cubic' are aliases for 0, 1, and 3,
+            respectively.
         return_indices : bool, default=False
-            Choose whether to return the row and column indices of points on the `grid` used to 
-            interpolate the point data. 
-
-        return_distances : bool, default=False
-            Choose whether to return the row and column normal distances between interpolated 
-            points and neighbouring sampling points.
+            Whether to return the row and column indices of the nearest grid
+            points.
 
         Returns
         -------
-        data_interp : tuple of ndarrays
-            By default, `data_interp` has one ndarray - this holds the values of the grid data 
-            where interpolated points lie. If sample point indices and/or distances have been 
-            requested (by setting `return_indices` and/or `return_distances`
-            to `True`), these are returned as subsequent tuple elements. 
+        numpy.ndarray
+            The values interpolated at the input points.
+        indices : 2-tuple of numpy.ndarray
+            The i- and j-indices of the nearest grid points to the input
+            points, only present if `return_indices=True`.
 
         Raises
         ------
         ValueError
-            * Raised if the string method supplied is not `linear` or `nearest`.
-            * Raised if the provided lat, lon arrays generate sample points that do not have the 
-            same dimensions as the 
-            supplied grid. 
-            * Raised if the provided lat, lon arrays generate sample points that include any point 
-            out of grid bounds. 
-            Alerts user which dimension (index) the point is located. 
-        """
-        interp = self._interpolator
-        interp.values = self.data
+            If an invalid `method` is provided.
+        RuntimeWarning
+            If `lats` contains any invalid values outside of the interval
+            [-90, 90]. Invalid values will be clipped to this interval.
+
+        Notes
+        -----
+        If `return_indices` is set to `True`, the nearest array indices
+        are returned as a tuple of arrays, in (i, j) or (lat, lon) format.
 
-        lons = np.atleast_1d(lons)
-        lats = np.atleast_1d(lats)
-        lons[lons > 180] -= 360
-        lons[lons < -180] += 360
-        results = interp(
-            (lats,lons),
+        An example output:
+
+            # The first array holds the rows of the raster where point data spatially falls near.
+            # The second array holds the columns of the raster where point data spatially falls near.
+            sampled_indices = (array([1019, 1019, 1019, ..., 1086, 1086, 1087]), array([2237, 2237, 2237, ...,  983,  983,  983]))
+        """
+        return sample_grid(
+            lon=lons,
+            lat=lats,
+            grid=self,
             method=method,
             return_indices=return_indices,
-            return_distances=return_distances,
         )
 
-        if return_indices or return_distances:
-            data_interp = results[0]
-            if self.origin == "upper":
-                data_interp = np.flipud(data_interp)
-            return data_interp.astype(self.dtype), *results[1:]
-
-        if self.origin == "upper":
-            results = np.flipud(results)
-        return results.astype(self.dtype)
-
-
-    def resample(self, spacingX, spacingY, overwrite=False):
+    def resample(self, spacingX, spacingY, method="linear", inplace=False):
         """Resample the `grid` passed to the `Raster` object with a new `spacingX` and 
         `spacingY` using linear interpolation.
 
         Notes
         -----
         Ultimately, `resample` changes the lat-lon resolution of the gridded data. The
         larger the x and y spacings given are, the larger the pixellation of raster data. 
 
         `resample` creates new latitude and longitude arrays with specified spacings in the
         X and Y directions (`spacingX` and `spacingY`). These arrays are linearly interpolated 
-        into a new raster. If `overwrite` is set to `True`, the respaced latitude array, longitude 
-        array and raster will overwrite the ones currently attributed to the `Raster` object.
+        into a new raster. If `inplace` is set to `True`, the respaced latitude array, longitude 
+        array and raster will inplace the ones currently attributed to the `Raster` object.
 
         Parameters
         ----------
         spacingX, spacingY : ndarray
             Specify the spacing in the X and Y directions with which to resample. The larger 
             `spacingX` and `spacingY` are, the larger the raster pixels become (less resolved).
             Note: to keep the size of the raster consistent, set `spacingX = spacingY`; 
             otherwise, if for example `spacingX > spacingY`, the raster will appear stretched 
             longitudinally. 
 
-        overwrite : bool, default=False
-            Choose to overwrite the raster (the `self.data` attribute), latitude array 
+        method : str or int; default: 'linear'
+            The order of spline interpolation. Must be an integer in the range
+            0-5. 'nearest', 'linear', and 'cubic' are aliases for 0, 1, and 3,
+            respectively.
+
+        inplace : bool, default=False
+            Choose to overwrite the data (the `self.data` attribute), latitude array 
             (`self.lats`) and longitude array (`self.lons`) currently attributed to the 
             `Raster` object. 
 
         Returns
         -------
-        data : ndarray grid
-            A new version of the raster data attributed to the `Raster` object resampled to 
-            the given `spacingX` and `spacingY` spacings.
+        Raster
+            The resampled grid. If `inplace` is set to `True`, this raster overwrites the
+            one attributed to `data`.
         """
         spacingX = np.abs(spacingX)
         spacingY = np.abs(spacingY)
         if self.origin == "upper":
             spacingY *= -1.0
 
         lons = np.arange(self.extent[0], self.extent[1]+spacingX, spacingX)
         lats = np.arange(self.extent[2], self.extent[3]+spacingY, spacingY)
         lonq, latq = np.meshgrid(lons, lats)
 
-        data = self.interpolate(lonq, latq)
-        if overwrite:
+        data = self.interpolate(lonq, latq, method=method)
+        if inplace:
             self._data = data
             self._lons = lons
             self._lats = lats
-            self._update()
-
-        return data
+        else:
+            return Raster(data, self.plate_reconstruction, self.extent, self.time)
 
 
-    def resize(self, resX, resY, overwrite=False):
+    def resize(self, resX, resY, inplace=False, method="linear", return_array=False):
         """Resize the grid passed to the `Raster` object with a new x and y resolution 
         (`resX` and `resY`) using linear interpolation. 
 
         Notes
         -----
         Ultimately, `resize` "stretches" a raster in the x and y directions. The larger
         the resolutions in x and y, the more stretched the raster appears in x and y.
 
         It creates new latitude and longitude arrays with specific resolutions in 
         the X and Y directions (`resX` and `resY`). These arrays are linearly interpolated
-        into a new raster. If `overwrite` is set to `True`, the resized latitude, longitude 
-        arrays and raster will overwrite the ones currently attributed to the `Raster` object.
+        into a new raster. If `inplace` is set to `True`, the resized latitude, longitude 
+        arrays and raster will inplace the ones currently attributed to the `Raster` object.
 
         Parameters
         ----------
         resX, resY : ndarray
             Specify the resolutions with which to resize the raster. The larger `resX` is,
             the more longitudinally-stretched the raster becomes. The larger `resY` is, the
             more latitudinally-stretched the raster becomes.
 
-        overwrite : bool, default=False
-            Choose to overwrite the raster (the `self.data` attribute), latitude array 
+        method : str or int; default: 'linear'
+            The order of spline interpolation. Must be an integer in the range
+            0-5. 'nearest', 'linear', and 'cubic' are aliases for 0, 1, and 3,
+            respectively.
+
+        inplace : bool, default=False
+            Choose to overwrite the data (the `self.data` attribute), latitude array 
             (`self.lats`) and longitude array (`self.lons`) currently attributed to the 
             `Raster` object. 
 
+        return_array : bool, default False
+            Return a `numpy.ndarray`, rather than a `Raster`.
+
         Returns
         -------
-        data : meshed ndarray grid
-            A new resized raster. If `overwrite` is set to `True`, this raster overwrites the
+        Raster
+            The resized grid. If `inplace` is set to `True`, this raster overwrites the
             one attributed to `data`.
         """
         # construct grid
         lons = np.linspace(self.extent[0], self.extent[1], resX)
         lats = np.linspace(self.extent[2], self.extent[3], resY)
         lonq, latq = np.meshgrid(lons, lats)
 
-        data = self.interpolate(lonq, latq)
-        if overwrite:
+        data = self.interpolate(lonq, latq, method=method)
+        if inplace:
             self._data = data
             self._lons = lons
             self._lats = lats
-            self._update()
-
-        return data
+        if return_array:
+            return data
+        else:
+            return Raster(data, self.plate_reconstruction, self.extent, self.time)
 
 
-    def fill_NaNs(self, overwrite=False):
+    def fill_NaNs(self, inplace=False, return_array=False):
         """Search raster for invalid ‘data’ cells containing NaN-type entries replaces them 
         with the value of their nearest valid data cells.
 
         Parameters
         ---------
-        overwrite : bool, default=False
+        inplace : bool, default=False
             Choose whether to overwrite the grid currently held in the `data` attribute with
             the filled grid.
 
+        return_array : bool, default False
+            Return a `numpy.ndarray`, rather than a `Raster`.
+
         Returns
         --------
-        data : ndarray
-            An updated grid of data where each invalid cell has been replaced with the v
-            alue of its nearest valid neighbour. If `overwrite` is set to `True`, this raster 
-            overwrites the one attributed to `data`.
+        Raster
+            The resized grid. If `inplace` is set to `True`, this raster overwrites the
+            one attributed to `data`.
         """
         data = fill_raster(self.data)
-        if overwrite:
+        if inplace:
             self._data = data
-
-        return data
+        if return_array:
+            return data
+        else:
+            return Raster(data, self.plate_reconstruction, self.extent, self.time)
 
 
-    def save_to_NetCDF4(self, filename):
+    def save_to_netcdf4(self, filename):
         """ Saves the grid attributed to the `Raster` object to the given `filename` (including
         the ".nc" extension) in netCDF4 format."""
         write_netcdf_grid(str(filename), self.data, self.extent)
 
 
     def reconstruct(
         self,
         time,
         fill_value=None,
         partitioning_features=None,
         threads=1,
         anchor_plate_id=0,
         inplace=False,
+        return_array=False,
     ):
-        """Reconstruct the raster data to a given time.
+        """Reconstruct raster data to a given time.
 
         Parameters
         ----------
         time : float
             Time to which the data will be reconstructed.
         fill_value : float, int, str, or tuple, optional
             The value to be used for regions outside of the static polygons
@@ -1743,18 +1926,20 @@
             Number of threads to use for certain computationally heavy
             routines.
         anchor_plate_id : int, default 0
             ID of the anchored plate.
         inplace : bool, default False
             Perform the reconstruction in-place (replace the raster's data
             with the reconstructed data).
+        return_array : bool, default False
+            Return a `numpy.ndarray`, rather than a `Raster`.
 
         Returns
         -------
-        numpy.ndarray
+        Raster or np.ndarray
             The reconstructed grid. Areas for which no plate ID could be
             determined will be filled with `fill_value`.
 
         Raises
         ------
         TypeError
             If this `Raster` has no `plate_reconstruction` set.
@@ -1791,19 +1976,33 @@
             to_time=time,
             extent=self.extent,
             origin=self.origin,
             fill_value=fill_value,
             threads=threads,
             anchor_plate_id=anchor_plate_id,
         )
+
         if inplace:
             self.data = result
             self._time = time
+            if return_array:
+                return result
+            return self
+
+        if not return_array:
+            result = type(self)(
+                data=result,
+                plate_reconstruction=self.plate_reconstruction,
+                extent=self.extent,
+                time=time,
+                origin=self.origin,
+            )
         return result
 
+
     def imshow(self, ax=None, projection=None, **kwargs):
         """Display raster data.
 
         A pre-existing matplotlib `Axes` instance is used if available,
         else a new one is created. The `origin` and `extent` of the image
         are determined automatically and should not be specified.
 
@@ -1868,15 +2067,17 @@
                 extent[1],
                 extent[3],
                 extent[2],
             )
         im = ax.imshow(self.data, origin=self.origin, extent=extent, **kwargs)
         return im
 
+    plot = imshow
 
-class TimeRaster(Raster):
-    """A class for the temporal manipulation of raster data. To be added soon!"""
-    def __init__(self, PlateReconstruction_object=None, filename=None, array=None, extent=None, resample=None):
-        raise NotImplementedError(
-            "This class has not been implemented; use `Raster` instead"
-        )
-        # super(TimeRaster, self).__init__(PlateReconstruction_object)
+
+# class TimeRaster(Raster):
+#     """A class for the temporal manipulation of raster data. To be added soon!"""
+#     def __init__(self, PlateReconstruction_object=None, filename=None, array=None, extent=None, resample=None):
+#         raise NotImplementedError(
+#             "This class has not been implemented; use `Raster` instead"
+#         )
+#         super(TimeRaster, self).__init__(PlateReconstruction_object)
```

### Comparing `gplately-0.3.3/gplately/io.py` & `gplately-0.4/gplately/io.py`

 * *Files identical despite different names*

### Comparing `gplately-0.3.3/gplately/oceans.py` & `gplately-0.4/gplately/oceans.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,32 +100,30 @@
 interpolation and written to a netCDF4 format.
 
 Classes
 -------
 * SeafloorGrid
 
 """
-import warnings
-import pygplates
-import numpy as np
-import stripy 
-import ptt
-import multiprocessing
 import glob
 import os
 import re
-import math
-from scipy.interpolate import griddata
+import warnings
+
+import numpy as np
 import pandas as pd
+import ptt
+import pygplates
+import stripy
+from ptt import separate_ridge_transform_segments
+from scipy.interpolate import griddata
 
 from . import reconstruction
-from . import plot
 from . import grids
 from . import tools
-from ptt import separate_ridge_transform_segments
 
 # -------------------------------------------------------------------------
 # Auxiliary functions for SeafloorGrid
 
 def create_icosahedral_mesh(refinement_levels):
     """ Define a global point mesh with Stripy's
     [icosahedral triangulated mesh](https://github.com/underworldcode/stripy/blob/294354c00dd72e085a018e69c345d9353c6fafef/stripy/spherical_meshes.py#L27)
@@ -283,46 +281,46 @@
     pygplates.MultiPointOnSphere(points_out_arr) : instance <pygplates.MultiPointOnSphere>
         Point features that are outside COB terrane polygons.
     zvals : list
         A binary list. If an entry is == 0, its corresponing point in the 
         MultiPointOnSphere object is on the ocean. If == 1, the point is 
         in the COB terrane polygon.
     """
+    # Convert MultiPointOnSphere to array of PointOnSphere
+    multi_point = np.array(multi_point.get_points(), dtype="object")
 
-    # Collect reconstructed geometries and features of continental polygons
-    # Both are needed for PTT's PIP routine.
-    polygons = []
-    polygon_features = []
-    for reconstructed_continental_geometry in COB_polygons:
-        polygons.append(
-            reconstructed_continental_geometry.get_reconstructed_geometry()
-        )
-        polygon_features.append(
-            reconstructed_continental_geometry.get_feature()
-        )
-
-    # Determine which continental polygons contain points from the isocahedral mesh
-    continental_polygon_features_containing_points = ptt.utils.points_in_polygons.find_polygons(
-        multi_point, polygons, polygon_features, all_polygons=True
+    # Collect reconstructed geometries of continental polygons
+    polygons = np.empty(len(COB_polygons), dtype="object")
+    for ind, i in enumerate(COB_polygons):
+        if isinstance(i, pygplates.ReconstructedFeatureGeometry):
+            geom = i.get_reconstructed_geometry()
+        elif isinstance(i, pygplates.GeometryOnSphere):
+            geom = i
+        else:  # e.g. ndarray of coordinates
+            geom = pygplates.PolygonOnSphere(i)
+        polygons[ind] = geom
+    proxies = np.ones(polygons.size)
+
+    pip_result = ptt.utils.points_in_polygons.find_polygons(
+        multi_point, polygons, proxies, all_polygons=False
+    )  # 1 for points in polygons, None for points outside
+    zvals = np.array(
+        pip_result,
+        dtype="float",
+    ).ravel()
+    zvals[np.isnan(zvals)] = 0.0
+    zvals = zvals.astype("int")
+    points_in_arr = multi_point[zvals == 1]
+    points_out_arr = multi_point[zvals != 1]
+
+    return (
+        pygplates.MultiPointOnSphere(points_in_arr),
+        pygplates.MultiPointOnSphere(points_out_arr),
+        zvals,
     )
-    # Look for points inside polygons, i.e. points in COB terrane polygons
-    points_in_arr = []
-    points_out_arr = []
-    zvals = []
-    for point_index, polygon_feature_list in enumerate(continental_polygon_features_containing_points):
-        # If inside, set zval of masking grid to True
-        if polygon_feature_list:
-            points_in_arr.append(multi_point[point_index])
-            zvals.append(1)
-        # If outside, set zval of masking grid to False
-        else:
-            points_out_arr.append(multi_point[point_index])
-            zvals.append(0)
-
-    return pygplates.MultiPointOnSphere(points_in_arr), pygplates.MultiPointOnSphere(points_out_arr), zvals
 
 
 def _deg2pixels(deg_res, deg_min, deg_max):
     return int(np.floor((deg_max - deg_min) / deg_res)) + 1
 
 
 def _pixels2deg(spacing_pixel, deg_min, deg_max):
@@ -356,36 +354,18 @@
         Control the number of points in the icosahedral mesh (higher integer
         means higher resolution of continent masks).
     ridge_sampling : float, default 0.5
         Spatial resolution (in degrees) at which points that emerge from ridges are tessellated.
     extent : list of float or int, default [-180.,180.,-90.,90.]
         A list containing the mininum longitude, maximum longitude, minimum latitude and 
         maximum latitude extents for all masking and final grids.
-    spacing_degrees : float, default None
+    grid_spacing : float, default None
         The degree spacing/interval with which to space grid points across all masking and
-        final grids. If `spacing_degrees` is provided, all grids will use it, and `spacingX`
-        and/or `spacingY` cannot be provided too. However, if `spacingX` and `spacingY` are 
-        provided instead, `spacing_degrees` defaults to the equivalent degree spacing of 
-        `spacingX` and `spacingY`. If insufficient grid resolution information is given, 
-        `spacing_degrees` defaults to 0.1, `spacingX` defaults to 3601 and `spacingY` defaults
-        to 1801. 
-    spacingX : int, default None
-        Number of pixels in the longitudinal direction of the regular grid to interpolate 
-        the grid points onto. If provided with the correct `spacingY`, it creates 
-        an even grid point distribution across `extent`. Otherwise, `spacingX` and `spacingY` 
-        are shifted to values that create an even point distribution. If `spacingX` is provided
-        alone, `spacingX` defaults to 3601 and `spacingY` defaults to 1801, which translates to
-        a `spacing_degree` of 0.1. If provided, `spacing_degrees` cannot be provided too.
-    spacingY : int, default None
-        Number of pixels in the latitudinal direction of the regular grid to interpolate
-        the grid points onto. If provided with the correct `spacingX`, it creates 
-        an even grid point distribution across `extent`. Otherwise, `spacingX` and `spacingY` 
-        are shifted to values that create an even point distribution. If `spacingY` is provided
-        alone, `spacingX` defaults to 3601 and `spacingY` defaults to 1801, which translates to
-        a `spacing_degree` of 0.1. If provided, `spacing_degrees` cannot be provided too.
+        final grids. If `grid_spacing` is provided, all grids will use it. If not,
+        `grid_spacing` defaults to 0.1.
     subduction_collision_parameters : len-2 tuple of float, default (5.0, 10.0)
         A 2-tuple of (threshold velocity delta in kms/my, threshold distance to boundary 
         per My in kms/my)
     initial_ocean_mean_spreading_rate : float, default 75.
         A spreading rate to uniformly allocate to points that define the initial ocean 
         basin. These points will have inaccurate ages, but most of them will be phased
         out after points with plate-model prescribed ages emerge from ridges and spread 
@@ -410,144 +390,101 @@
         max_time,
         min_time,
         ridge_time_step,
         save_directory=None,
         file_collection=None,
         refinement_levels=5, 
         ridge_sampling=0.5,
-        extent = [-180,180,-90,90],
-        spacing_degrees = None, 
-        spacingX = None,
-        spacingY = None,
+        extent = (-180, 180, -90, 90),
+        grid_spacing = None, 
         subduction_collision_parameters = (5.0, 10.0),
         initial_ocean_mean_spreading_rate = 75.,
         resume_from_checkpoints = False,
-        zval_names = ['SPREADING_RATE']
-        ):
+        zval_names = ("SPREADING_RATE",),
+    ):
 
         # Provides a rotation model, topology features and reconstruction time for 
         # the SeafloorGrid
         self.PlateReconstruction_object = PlateReconstruction_object
         self.rotation_model = self.PlateReconstruction_object.rotation_model
         self.topology_features = self.PlateReconstruction_object.topology_features
         self._PlotTopologies_object = PlotTopologies_object
         #self.save_directory = str(os.path.abspath(save_directory))
+        if (save_directory is not None) and (not os.path.isdir(save_directory)):
+            print(
+                "Output directory does not exist; creating now: "
+                + str(save_directory)
+            )
+            os.makedirs(save_directory, exist_ok=True)
         self.save_directory = save_directory
         self.file_collection = file_collection
 
         # Topological parameters
         self.refinement_levels = refinement_levels
         self.ridge_sampling = ridge_sampling
         self.subduction_collision_parameters = subduction_collision_parameters
         self.initial_ocean_mean_spreading_rate = initial_ocean_mean_spreading_rate
 
         # Gridding parameters
         self.extent = extent
 
-        if spacing_degrees and (spacingX or spacingY):
-            raise ValueError("Please provide only spacing_degrees OR spacingX & spacingY.")
-
+        # A list of degree spacings that allow an even division of the global lat-lon extent.
         divisible_degree_spacings = [0.1, 0.25, 0.5, 0.75, 1.]
 
-        if spacing_degrees:
+        if grid_spacing:
 
-            if spacing_degrees in divisible_degree_spacings:
-                self.spacing_degrees = spacing_degrees
-                self.spacingX = _deg2pixels(spacing_degrees, self.extent[0], self.extent[1])
-                self.spacingY = _deg2pixels(spacing_degrees, self.extent[2], self.extent[3])
+            # If the provided degree spacing is in the list of permissible spacings, use it
+            # and prepare the number of pixels in x and y (spacingX and spacingY)
+            if grid_spacing in divisible_degree_spacings:
+                self.grid_spacing = grid_spacing
+                self.spacingX = _deg2pixels(grid_spacing, self.extent[0], self.extent[1])
+                self.spacingY = _deg2pixels(grid_spacing, self.extent[2], self.extent[3])
 
             # If the provided spacing is >>1 degree, use 1 degree
-            elif spacing_degrees >= divisible_degree_spacings[-1]:
-                self.spacing_degrees = divisible_degree_spacings[-1]
+            elif grid_spacing >= divisible_degree_spacings[-1]:
+                self.grid_spacing = divisible_degree_spacings[-1]
                 self.spacingX = _deg2pixels(divisible_degree_spacings[-1], self.extent[0], self.extent[1])
                 self.spacingY = _deg2pixels(divisible_degree_spacings[-1], self.extent[2], self.extent[3])
 
                 with warnings.catch_warnings():
                     warnings.simplefilter("always")
                     warnings.warn(
-                        "The provided spacing_degrees of {} is quite large. To preserve the grid resolution, a {} degree spacing and spacingX of {} and spacingY of {} has been employed instead".format(
-                            spacing_degrees, self.spacing_degrees, self.spacing_degrees, self.spacingX, self.spacingY
+                        "The provided grid_spacing of {} is quite large. To preserve the grid resolution, a {} degree spacing has been employed instead".format(
+                            grid_spacing, self.grid_spacing
                         )
                     )
 
+            # If the provided degree spacing is not in the list of permissible spacings, but below
+            # a degree, find the closest permissible degree spacing. Use this and find 
+            # spacingX and spacingY.
             else:
                 for divisible_degree_spacing in divisible_degree_spacings:
                 # The tolerance is half the difference between consecutive divisible spacings.
                 # Max is 1 degree for now - other integers work but may provide too little of a
                 # grid resolution.
-                    if (abs(spacing_degrees - divisible_degree_spacing) <= 0.125):
+                    if (abs(grid_spacing - divisible_degree_spacing) <= 0.125):
                         new_deg_res = divisible_degree_spacing
-                        self.spacing_degrees = new_deg_res
+                        self.grid_spacing = new_deg_res
                         self.spacingX = _deg2pixels(new_deg_res, self.extent[0], self.extent[1])
                         self.spacingY = _deg2pixels(new_deg_res, self.extent[2], self.extent[3])
 
                 with warnings.catch_warnings():
                     warnings.simplefilter("always")
                     warnings.warn(
-                        "The provided spacing_degrees of {} does not cleanly divide into the global extent. A degree spacing of {} with spacingX of {} and spacingY of {} has been employed instead.".format(
-                            spacing_degrees, self.spacing_degrees, self.spacingX, self.spacingY
+                        "The provided grid_spacing of {} does not cleanly divide into the global extent. A degree spacing of {} has been employed instead.".format(
+                            grid_spacing, self.grid_spacing
                         )
                     )
 
         else:
-            # If either spacingX and/or spacingY is still none, use default resolutions
-            if None in (spacingX, spacingY):
-                self.spacing_degrees = 0.1
-                self.spacingX = 3601
-                self.spacingY = 1801
-
-            # If both spacingX and spacingY are given,
-            else:
-                # Find their equivalent degree spacings
-                equivalent_lon_deg = _pixels2deg(spacingX, self.extent[0], self.extent[1])
-                equivalent_lat_deg = _pixels2deg(spacingY, self.extent[2], self.extent[3])
-
-                # Can use the provided spacings if they provide an equal degree interval in x and y
-                if equivalent_lon_deg == equivalent_lat_deg:
-                    self.spacingX = spacingX
-                    self.spacingY = spacingY
-                    self.spacing_degrees = equivalent_lon_deg
-
-                # If they do not provide an equal degree interval in x and y,
-                else:
-
-                    # Use the average degree of both the lon and lat equivalent degrees
-                    spacing_degrees = (equivalent_lat_deg + equivalent_lon_deg)/2
-
-                    # If the average spacing is much higher than the last permissible degree interval,
-                    # use the last permissible degree interval.
-                    if spacing_degrees >= divisible_degree_spacings[-1]:
-                        self.spacing_degrees = divisible_degree_spacings[-1]
-                        self.spacingX = _deg2pixels(divisible_degree_spacings[-1], self.extent[0], self.extent[1])
-                        self.spacingY = _deg2pixels(divisible_degree_spacings[-1], self.extent[2], self.extent[3])
-
-                        with warnings.catch_warnings():
-                            warnings.simplefilter("always")
-                            warnings.warn(
-                                "The provided spacingX of {} and spacingY of {} gives a large and uneven degree spacing. To preserve the grid resolution, a {} degree spacing and spacingX of {} and spacingY of {} has been employed instead.".format(
-                                    spacingX, spacingY, self.spacing_degrees, self.spacingX, self.spacingY
-                                )
-                            )
-                    else:
-                        # Get the closest divisible degree to this average degree 
-                        for divisible_degree_spacing in divisible_degree_spacings:
-
-                            if (abs(spacing_degrees - divisible_degree_spacing) <= 0.125):
-                                new_deg_res = divisible_degree_spacing
-                                self.spacing_degrees = new_deg_res
-                                self.spacingX = _deg2pixels(new_deg_res, self.extent[0], self.extent[1])
-                                self.spacingY = _deg2pixels(new_deg_res, self.extent[2], self.extent[3])
-
-                        with warnings.catch_warnings():
-                            warnings.simplefilter("always")
-                            warnings.warn(
-                                "The provided pixel spacingX of {} and spacingY of {} do not cleanly divide into the global extent. A degree spacing of {} with spacingX of {} and spacingY of {} has been employed instead.".format(
-                                    spacingX, spacingY, self.spacing_degrees, self.spacingX, self.spacingY
-                                )
-                            )
+            # If a spacing degree is not provided, use default 
+            # resolution and get default spacingX and spacingY
+            self.grid_spacing = 0.1
+            self.spacingX = 3601
+            self.spacingY = 1801
 
         self.resume_from_checkpoints = resume_from_checkpoints
 
         # Temporal parameters
         self._max_time = float(max_time)
         self.min_time = float(min_time)
         self.ridge_time_step = float(ridge_time_step)
@@ -987,67 +924,46 @@
 
         # Build all continental masks and spreading ridge points (with z values)
         self._get_mid_ocean_ridge_seedpoints(time_array)
         return
 
 
     def _create_continental_mask(self, time_array):
-
-        # Create a mask for each timestep
+        """Create a continental mask for each timestep."""
         if time_array[0] != self._max_time:
             print("Masking interrupted - resuming continental mask building at {} Ma!".format(time_array[0]))
 
-        # Output grid coordinates
-        extent_globe = self.extent
-        grid_lon = np.linspace(extent_globe[0], extent_globe[1], self.spacingX)
-        grid_lat = np.linspace(extent_globe[2], extent_globe[3], self.spacingY)
-        grid_lon, grid_lat = np.meshgrid(grid_lon, grid_lat)
-        output_shape = np.shape(grid_lon)
-        grid_lon = np.ravel(grid_lon)
-        grid_lat = np.ravel(grid_lat)
-        multipoint = pygplates.MultiPointOnSphere(
-            np.column_stack((grid_lat, grid_lon))
-        )
-
         for time in time_array:
             self._PlotTopologies_object.time = time
-
-            # Ensure COB terranes have reconstruction IDs and valid times
-            COB_polygons = ensure_polygon_geometry(
-                self._PlotTopologies_object.continents,
-                self.rotation_model,
-                time) 
-
-            # grid_z1 is a binary array encoding whether a grid
-            # coordinate is within a COB terrane polygon or not
-            _, _, grid_z1 = point_in_polygon_routine(
-                multipoint,
-                COB_polygons,
+            geoms = self._PlotTopologies_object.continents
+            final_grid = grids.rasterise(
+                geoms,
+                key=1.0,
+                shape=(self.spacingY, self.spacingX),
+                extent=self.extent,
+                origin="lower",
             )
-            grid_z1 = np.array(grid_z1)
-            final_grid = np.abs(np.rint(grid_z1)).reshape(output_shape)
+            final_grid[np.isnan(final_grid)] = 0.0
 
             if self.save_directory is not None:
+                output_basename = "continent_mask_{}Ma.nc".format(time)
                 if self.file_collection is not None:
-                    full_directory = "{}/{}_continent_mask_{}Ma.nc".format(
-                        self.save_directory, 
-                        self.file_collection, 
-                        time
-                    )
-                else:
-                    full_directory = "{}/continent_mask_{}Ma.nc".format(
-                        self.save_directory, 
-                        time
+                    output_basename = "{}_{}".format(
+                        self.file_collection,
+                        output_basename,
                     )
+                output_filename = os.path.join(
+                    self.save_directory,
+                    output_basename,
+                )
                 grids.write_netcdf_grid(
-                    full_directory, 
-                    final_grid, 
+                    output_filename,
+                    final_grid,
                     extent=[-180,180,-90,90]
                 )
-            #all_continental_masks.append(final_grid)
             print("Finished building a continental mask at {} Ma!".format(time))
 
         return
 
 
     def build_all_continental_masks(self):
         """Create a continental mask to define the ocean basin for all times between 
@@ -1257,20 +1173,22 @@
             (pygplates.FeatureType.gpml_subduction_zone, self.subduction_collision_parameters)
             ]
         )
         # In addition to the default subduction detection, also detect continental collisions
         if self.file_collection is not None:
             collision_spec = reconstruction._ContinentCollision(
                 self.save_directory+"/"+self.file_collection+"_continent_mask_{}Ma.nc", 
-                default_collision
+                default_collision,
+                verbose=False,
             )
         else:
             collision_spec = reconstruction._ContinentCollision(
                 self.save_directory+"/continent_mask_{}Ma.nc", 
-                default_collision
+                default_collision,
+                verbose=False,
             )
 
         # Call the reconstruct by topologies object
         topology_reconstruction = reconstruction._ReconstructByTopologies(
             self.rotation_model, 
             self.topology_features,
             self._max_time,
```

### Comparing `gplately-0.3.3/gplately/parallel.py` & `gplately-0.4/gplately/parallel.py`

 * *Files identical despite different names*

### Comparing `gplately-0.3.3/gplately/plot.py` & `gplately-0.4/gplately/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Cartopy GeoAxes using Shapely and GeoPandas.
 
 Classes
 -------
 PlotTopologies
 """
 import re
+import warnings
 
 import pygplates
 import cartopy.crs as ccrs
 import matplotlib.pyplot as plt
 import numpy as np
 import ptt
 from shapely.geometry import Point, Polygon
@@ -563,28 +564,28 @@
     geological time; 
     * Turn these reconstructed features into Shapely geometries for plotting 
     on `cartopy.mpl.geoaxes.GeoAxes` or `cartopy.mpl.geoaxes.GeoAxesSubplot` map 
     Projections. 
 
     To call the `PlotTopologies` object, supply: 
 
-    * an instance of the GPlately `PlateReconstruction_object`
+    * an instance of the GPlately `plate_reconstruction` object
     * a reconstruction `time`
 
     and optionally, 
 
     * a `coastline_filename`
     * a `continent_filename`
     * a `COB_filename`
     * an `anchor_plate_id`
 
     For example:
 
         # Calling the PlotTopologies object
-        gplot = gplately.plot.PlotTopologies(plate_reconstruction_object,
+        gplot = gplately.plot.PlotTopologies(plate_reconstruction,
                                             time,
                                             coastline_filename,
                                             continent_filename,
                                             COB_filename,
                                             anchor_plate_id,
                 )
 
@@ -616,15 +617,15 @@
     * assorted reconstructable feature data, for example:
         - seafloor fabric
         - large igneous provinces 
         - volcanic provinces
 
     Attributes
     ----------
-    PlateReconstruction_object : instance of <gplately.reconstruction.PlateReconstruction>
+    plate_reconstruction : instance of <gplately.reconstruction.PlateReconstruction>
         The GPlately `PlateReconstruction` object will be used to access a plate 
         `rotation_model` and a set of `topology_features` which contains plate boundary 
         features like trenches, ridges and transforms.
 
     anchor_plate_id : int, default 0
         The anchor plate ID used for reconstruction.
 
@@ -692,25 +693,24 @@
         A list containing other geological features like unclassified features, extended continental crusts,
         continental rifts, faults, orogenic belts, fracture zones, inferred paleo boundaries, terrane 
         boundaries and passive continental boundaries.
 
     """
     def __init__(
         self,
-        PlateReconstruction_object,
-        time,
+        plate_reconstruction,
+        time=None,
         coastlines=None,
         continents=None,
         COBs=None,
         anchor_plate_id=0,
     ):
-        self.PlateReconstruction_object = PlateReconstruction_object
-        self.plate_model = self.PlateReconstruction_object
+        self.plate_reconstruction = plate_reconstruction
 
-        if self.plate_model.topology_features is None:
+        if self.plate_reconstruction.topology_features is None:
             raise ValueError("Plate model must have topology features.")
 
         self.base_projection = ccrs.PlateCarree()
 
         # store these for when time is updated
         # make sure these are initialised as FeatureCollection objects
 
@@ -722,45 +722,38 @@
         self.continents = None
         self.COBs = None
 
         self._anchor_plate_id = self._check_anchor_plate_id(anchor_plate_id)
 
         # store topologies for easy access
         # setting time runs the update_time routine
-        self.time = time
+        if time is not None:
+            self.time = time
+        else:
+            self._time = None
 
     def __getstate__(self):
 
-        filenames = self.PlateReconstruction_object.__getstate__()
+        filenames = self.plate_reconstruction.__getstate__()
 
         # add important variables from Points object
         if self._coastlines:
             filenames["coastlines"] = self._coastlines.filenames
         if self._continents:
             filenames["continents"] = self._continents.filenames
         if self._COBs:
             filenames["COBs"] = self._COBs.filenames
         filenames['time'] = self.time
         filenames['plate_id'] = self._anchor_plate_id
 
-        del self.coastlines, self.continents, self.COBs
-        del self._coastlines, self._continents, self._COBs
-
-        self.coastlines = None
-        self.continents = None
-        self.COBs = None
-        self._coastlines = None
-        self._continents = None
-        self._COBs = None
-
         return filenames
 
     def __setstate__(self, state):
 
-        self.PlateReconstruction_object = _PlateReconstruction(state['rotation_model'], state['topology_features'], state['static_polygons'])
+        self.plate_reconstruction = _PlateReconstruction(state['rotation_model'], state['topology_features'], state['static_polygons'])
 
         self._coastlines = None
         self._continents = None
         self._COBs = None
         self.coastlines = None
         self.continents = None
         self.COBs = None
@@ -779,15 +772,16 @@
         if 'COBs' in state:
             self._COBs = _FeatureCollection()
             for feature in state['COBs']:
                 self._COBs.add( _FeatureCollection(feature) )
 
 
         self._anchor_plate_id = state["plate_id"]
-        self.time = state['time']
+        self.base_projection = ccrs.PlateCarree()
+        self._time = None
 
 
     @property
     def time(self):
         """ The reconstruction time."""
         return self._time
 
@@ -843,16 +837,16 @@
         - other boundary sections (resolved features) that are not subduction zones or mid-ocean ridges 
         (ridge/transform)
 
         Moreover, coastlines, continents and COBs are reconstructed to the new specified `time`.
         """
         self._time = float(time)
         resolved_topologies = ptt.resolve_topologies.resolve_topologies_into_features(
-            self.PlateReconstruction_object.rotation_model,
-            self.PlateReconstruction_object.topology_features,
+            self.plate_reconstruction.rotation_model,
+            self.plate_reconstruction.topology_features,
             self.time)
 
         self.topologies, self.ridge_transforms, self.ridges, self.transforms, self.trenches, self.trench_left, self.trench_right, self.other = resolved_topologies
 
         # miscellaneous boundaries
         self.continental_rifts = []
         self.faults = []
@@ -910,23 +904,23 @@
                 self.misc_transforms.append(topol)
                 
             elif topol.get_feature_type() == pygplates.FeatureType.gpml_unclassified_feature:
                 self.unclassified_features.append(topol)
 
         # reconstruct other important polygons and lines
         if self._coastlines:
-            self.coastlines = self.PlateReconstruction_object.reconstruct(
+            self.coastlines = self.plate_reconstruction.reconstruct(
                 self._coastlines, self.time, from_time=0, anchor_plate_id=self.anchor_plate_id)
 
         if self._continents:
-            self.continents = self.PlateReconstruction_object.reconstruct(
+            self.continents = self.plate_reconstruction.reconstruct(
                 self._continents, self.time, from_time=0, anchor_plate_id=self.anchor_plate_id)
 
         if self._COBs:
-            self.COBs = self.PlateReconstruction_object.reconstruct(
+            self.COBs = self.plate_reconstruction.reconstruct(
                 self._COBs, self.time, from_time=0, anchor_plate_id=self.anchor_plate_id)
 
 
     # subduction teeth
     def _tesselate_triangles(self, features, tesselation_radians, triangle_base_length, triangle_aspect=1.0):
         """Places subduction teeth along subduction boundary line segments within a MultiLineString shapefile. 
 
@@ -994,19 +988,106 @@
                             triangle_pointsX.append( [A[0], C[0], D[0]] )
                             triangle_pointsY.append( [A[1], C[1], D[1]] )
 
                             cum_distance = 0.0
 
         return np.array(triangle_pointsX), np.array(triangle_pointsY)
 
-    def plot_feature(self, ax, feature, **kwargs):
+
+    def get_feature(self, feature):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed features. 
+
+        Notes
+        -----
+        The feature needed to produce the GeoDataFrame should already be constructed to a `time`.
+        This function converts the feature into a set of Shapely geometries whose coordinates are 
+        passed to a geopandas GeoDataFrame.
+
+        Parameters
+        ----------
+        feature : instance of <pygplates.Feature>
+            A feature reconstructed to `time`.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `feature` geometries.
+
+        """
         shp = shapelify_features(feature)
         gdf = gpd.GeoDataFrame({'geometry': shp}, geometry='geometry')
+        return gdf
+
+    def plot_feature(self, ax, feature, **kwargs):
+        """ Plot pygplates.FeatureCollection  or pygplates.Feature onto a map.
+
+        Parameters
+        ----------
+        ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
+            A subclass of `matplotlib.axes.Axes` which represents a map Projection.
+            The map should be set at a particular Cartopy projection.
+
+        **kwargs : 
+            Keyword arguments for parameters such as `facecolor`, `alpha`, 
+            etc. for plotting coastline geometries.
+            See `Matplotlib` keyword arguments 
+            [here](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html).
+
+        Returns
+        -------
+        ax : instance of <geopandas.GeoDataFrame.plot>
+            A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
+            with coastline features plotted onto the chosen map projection.
+        """
+        gdf = self.get_feature(feature)
         return gdf.plot(ax=ax, transform=self.base_projection, **kwargs)
 
+
+    def get_coastlines(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed coastline polygons. 
+
+        Notes
+        -----
+        The `coastlines` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `coastlines` are reconstructed, they are 
+        converted into Shapely polygons whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `coastlines` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `coastlines` to the requested `time` and thus populate the GeoDataFrame.
+
+        """
+        if self._time is None:
+            raise ValueError("No coastlines have been resolved. Set `PlotTopologies.time` to construct coastlines.")
+
+        if self.coastlines is None:
+            raise ValueError("Supply coastlines to PlotTopologies object")
+
+        coastline_polygons = shapelify_feature_polygons(self.coastlines)
+        gdf = gpd.GeoDataFrame({"geometry": coastline_polygons}, geometry="geometry")
+        return gdf
+
+
     def plot_coastlines(self, ax, **kwargs):
         """Plot reconstructed coastline polygons onto a standard map Projection. 
 
         Notes
         -----
         The `coastlines` for plotting are accessed from the `PlotTopologies` object's
         `coastlines` attribute. These `coastlines` are reconstructed to the `time` 
@@ -1030,21 +1111,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with coastline features plotted onto the chosen map projection. 
         """
+        gdf = self.get_coastlines()
+        return gdf.plot(ax=ax, transform=self.base_projection, **kwargs)
 
-        if self.coastlines is None:
-            raise ValueError("Supply coastline_filename to PlotTopologies object")
 
-        coastline_polygons = shapelify_feature_polygons(self.coastlines)
-        gdf = gpd.GeoDataFrame({"geometry": coastline_polygons}, geometry="geometry")
-        return gdf.plot(ax=ax, transform=self.base_projection, **kwargs)
+    def get_continents(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed continental polygons. 
+
+        Notes
+        -----
+        The `continents` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `continents` are reconstructed, they are 
+        converted into Shapely polygons whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `continents` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `continents` to the requested `time` and thus populate the GeoDataFrame.
+
+        """
+        if self._time is None:
+            raise ValueError("No continents have been resolved. Set `PlotTopologies.time` to construct continents.")
+
+        if self.continents is None:
+            raise ValueError("Supply continents to PlotTopologies object")
+
+        continent_polygons = shapelify_feature_polygons(self.continents)
+        gdf = gpd.GeoDataFrame({"geometry": continent_polygons}, geometry="geometry")
+        return gdf
+
 
     def plot_continents(self, ax, **kwargs):
         """Plot reconstructed continental polygons onto a standard map Projection. 
 
         Notes
         -----
         The `continents` for plotting are accessed from the `PlotTopologies` object's
@@ -1069,21 +1188,61 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with continent features plotted onto the chosen map projection. 
         """
-        if self.continents is None:
-            raise ValueError("Supply continent_filename to PlotTopologies object")
-
-        continent_polygons = shapelify_feature_polygons(self.continents)
-        gdf = gpd.GeoDataFrame({"geometry": continent_polygons}, geometry="geometry")
+        gdf = self.get_continents()
         return gdf.plot(ax=ax, transform=self.base_projection, **kwargs)
 
+
+    def get_continent_ocean_boundaries(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed continent-ocean
+        boundary lines. 
+
+        Notes
+        -----
+        The `COBs` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `COBs` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `COBs` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `COBs` to the requested `time` and thus populate the GeoDataFrame.
+
+        """
+        if self._time is None:
+            raise ValueError("No geometries have been resolved. Set `PlotTopologies.time` to construct topologies.")
+
+        if self.COBs is None:
+            raise ValueError("Supply COBs to PlotTopologies object")
+
+        COB_lines = shapelify_feature_lines(self.COBs)
+        gdf = gpd.GeoDataFrame({"geometry": COB_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_continent_ocean_boundaries(self, ax, **kwargs):
         """Plot reconstructed continent-ocean boundary (COB) polygons onto a standard 
         map Projection. 
 
         Notes
         -----
         The `COBs` for plotting are accessed from the `PlotTopologies` object's
@@ -1112,21 +1271,60 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with COB features plotted onto the chosen map projection. 
         """
-        if self.COBs is None:
-            raise ValueError("Supply COB_filename to PlotTopologies object")
-
-        COB_lines = shapelify_feature_lines(self.COBs)
-        gdf = gpd.GeoDataFrame({"geometry": COB_lines}, geometry="geometry")
+        gdf = self.get_continent_ocean_boundaries()
         return gdf.plot(ax=ax, transform=self.base_projection, **kwargs)
 
+
+    def get_ridges(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed ridge lines. 
+
+        Notes
+        -----
+        The `ridges` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `ridges` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `ridges` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `ridges` to the requested `time` and thus populate the GeoDataFrame.
+
+        """
+        if self._time is None:
+            raise ValueError("No ridges have been resolved. Set `PlotTopologies.time` to construct ridges.")
+
+        if self.ridges is None:
+            raise ValueError("No ridge topologies passed to PlotTopologies.")
+
+        ridge_lines = shapelify_feature_lines(self.ridges)
+        gdf = gpd.GeoDataFrame({"geometry": ridge_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_ridges(self, ax, color='black', **kwargs):
         """Plot reconstructed ridge polylines onto a standard map Projection. 
         
         Notes
         -----
         The `ridges` for plotting are accessed from the `PlotTopologies` object's
         `ridges` attribute. These `ridges` are reconstructed to the `time` 
@@ -1159,18 +1357,60 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with ridge features plotted onto the chosen map projection. 
         """
-        ridge_lines = shapelify_feature_lines(self.ridges)
-        gdf = gpd.GeoDataFrame({"geometry": ridge_lines}, geometry="geometry")
+        gdf = self.get_ridges()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
+
+    def get_ridges_and_transforms(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed ridge and transform lines. 
+
+        Notes
+        -----
+        The `ridge_transforms` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `ridge_transforms` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `ridges` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `ridge_transforms` to the requested `time` and thus populate the GeoDataFrame.
+
+        """
+        if self._time is None:
+            raise ValueError("No ridges and transforms have been resolved. Set `PlotTopologies.time` to construct ridges and transforms.")
+
+        if self.ridge_transforms is None:
+            raise ValueError("No ridge and transform topologies passed to PlotTopologies.")
+
+        ridge_transform_lines = shapelify_feature_lines(self.ridge_transforms)
+        gdf = gpd.GeoDataFrame({"geometry": ridge_transform_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_ridges_and_transforms(self, ax, color='black', **kwargs):
         """Plot reconstructed ridge & transform boundary polylines onto a standard map
         Projection. 
 
         Notes
         -----
         The ridge & transform sections for plotting are accessed from the 
@@ -1204,18 +1444,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with ridge & transform features plotted onto the chosen map projection. 
         """
-        ridge_transform_lines = shapelify_feature_lines(self.ridge_transforms)
-        gdf = gpd.GeoDataFrame({"geometry": ridge_transform_lines}, geometry="geometry")
+        gdf = self.get_ridges_and_transforms()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
+
+    def get_transforms(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed transform lines. 
+
+        Notes
+        -----
+        The `transforms` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `transforms` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `transforms` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `transforms` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No transforms have been resolved. Set `PlotTopologies.time` to construct transforms.")
+
+        if self.transforms is None:
+            raise ValueError("No transform topologies passed to PlotTopologies.")
+
+        transform_lines = shapelify_feature_lines(self.transforms)
+        gdf = gpd.GeoDataFrame({"geometry": transform_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_transforms(self, ax, color='black', **kwargs):
         """Plot reconstructed transform boundary polylines onto a standard map. 
 
         Notes
         -----
         The transform sections for plotting are accessed from the 
         `PlotTopologies` object's `transforms` attribute. These `transforms` 
@@ -1248,18 +1529,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with transform features plotted onto the chosen map projection.
         """
-        transform_lines = shapelify_feature_lines(self.transforms)
-        gdf = gpd.GeoDataFrame({"geometry": transform_lines}, geometry="geometry")
+        gdf = self.get_transforms()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
+
+    def get_trenches(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed trench lines. 
+
+        Notes
+        -----
+        The `trenches` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `trenches` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `trenches` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `trenches` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No trenches have been resolved. Set `PlotTopologies.time` to construct trenches.")
+
+        if self.trenches is None:
+            raise ValueError("No trenches passed to PlotTopologies.")
+
+        trench_lines = shapelify_feature_lines(self.trenches)
+        gdf = gpd.GeoDataFrame({"geometry": trench_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_trenches(self, ax, color='black', **kwargs):
         """Plot reconstructed subduction trench polylines onto a standard map
         Projection. 
 
         Notes
         -----
         The trench sections for plotting are accessed from the 
@@ -1293,18 +1615,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with transform features plotted onto the chosen map projection.
         """
-        trench_lines = shapelify_feature_lines(self.trenches)
-        gdf = gpd.GeoDataFrame({"geometry": trench_lines}, geometry="geometry")
+        gdf = self.get_trenches()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
+
+    def get_misc_boundaries(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of other reconstructed lines. 
+
+        Notes
+        -----
+        The `other` geometries needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `other` geometries are reconstructed, they are 
+        converted into Shapely features whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `other` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `other` geometries to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No miscellaneous topologies have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.other is None:
+            raise ValueError("No miscellaneous topologies passed to PlotTopologies.")
+
+        lines = shapelify_features(self.other)
+        gdf = gpd.GeoDataFrame({"geometry": lines}, geometry="geometry")
+        return gdf
+
+
     def plot_misc_boundaries(self, ax, color="black", **kwargs):
         """Plot reconstructed miscellaneous plate boundary polylines onto a standard 
         map Projection.
 
         Notes
         -----
         The miscellaneous boundary sections for plotting are accessed from the 
@@ -1338,18 +1701,18 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with miscellaneous boundary features plotted onto the chosen map projection.
         """
-        lines = shapelify_features(self.other)
-        gdf = gpd.GeoDataFrame({"geometry": lines}, geometry="geometry")
+        gdf = self.get_misc_boundaries()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
+
     def plot_subduction_teeth_deprecated(self, ax, spacing=0.1, size=2.0, aspect=1, color='black', **kwargs):
         """Plot subduction teeth onto a standard map Projection. 
 
         Notes
         -----
         Subduction teeth are tessellated from `PlotTopologies` object attributes `trench_left` and 
         `trench_right`, and transformed into Shapely polygons for plotting. 
@@ -1469,14 +1832,15 @@
         trench_right_features = shapelify_feature_lines(self.trench_right)
 
         return(
             plot_subduction_teeth(trench_left_features,  size, 'l', height, spacing, ax=ax, color=color, **kwargs),
             plot_subduction_teeth(trench_right_features,  size, 'r', height, spacing, ax=ax, color=color, **kwargs)
         )
 
+
     def plot_plate_id(self, ax, plate_id, **kwargs):
         """Plot a plate polygon with an associated `plate_id` onto a standard map Projection. 
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1631,16 +1995,16 @@
         lons = np.arange(-180, 180+spacingX, spacingX)
         lats = np.arange(-90, 90+spacingY, spacingY)
         lonq, latq = np.meshgrid(lons, lats)
 
         # create a feature from all the points
         velocity_domain_features = ptt.velocity_tools.make_GPML_velocity_feature(lonq.ravel(), latq.ravel())
 
-        rotation_model = self.PlateReconstruction_object.rotation_model
-        topology_features = self.PlateReconstruction_object.topology_features
+        rotation_model = self.plate_reconstruction.rotation_model
+        topology_features = self.plate_reconstruction.topology_features
 
         delta_time = 5.0
         all_velocities = ptt.velocity_tools.get_plate_velocities(
             velocity_domain_features,
             topology_features,
             rotation_model,
             self.time,
@@ -1651,15 +2015,64 @@
 
         if normalise:
             mag = np.hypot(U, V)
             mag[mag == 0] = 1
             U /= mag
             V /= mag
 
-        return ax.quiver(X, Y, U, V, transform=self.base_projection, **kwargs)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", UserWarning)
+            quiver = ax.quiver(
+                X, Y,
+                U, V,
+                transform=self.base_projection,
+                **kwargs
+            )
+        return quiver
+
+
+    def get_continental_rifts(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed contiental rift lines. 
+
+        Notes
+        -----
+        The `continental_rifts` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `continental_rifts` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `continental_rifts` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `continental_rifts` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No continental rifts have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.continental_rifts is None:
+            raise ValueError("No continental rifts passed to PlotTopologies.")
+
+        continental_rift_lines = shapelify_feature_lines(self.continental_rifts)
+        gdf = gpd.GeoDataFrame({"geometry": continental_rift_lines}, geometry="geometry")
+        return gdf
 
 
     def plot_continental_rifts(self, ax, color='black', **kwargs):
         """Plot continental rifts on a standard map projection.
 
         Parameters
         ----------
@@ -1678,19 +2091,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with continental rifts plotted onto the chosen map projection.
         """
-        continental_rift_lines = shapelify_feature_lines(self.continental_rifts)
-        gdf = gpd.GeoDataFrame({"geometry": continental_rift_lines}, geometry="geometry")
+        gdf = self.get_continental_rifts()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_faults(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed fault lines. 
+
+        Notes
+        -----
+        The `faults` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `faults` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `faults` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `faults` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No faults have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.faults is None:
+            raise ValueError("No faults passed to PlotTopologies.")
+
+        fault_lines = shapelify_feature_lines(self.faults)
+        gdf = gpd.GeoDataFrame({"geometry": fault_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_faults(self, ax, color='black', **kwargs):
         """Plot faults on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1707,19 +2160,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with faults plotted onto the chosen map projection.
         """
-        fault_lines = shapelify_feature_lines(self.faults)
-        gdf = gpd.GeoDataFrame({"geometry": fault_lines}, geometry="geometry")
+        gdf = self.get_faults()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_fracture_zones(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed fracture zone lines. 
+
+        Notes
+        -----
+        The `fracture_zones` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `fracture_zones` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `fracture_zones` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `fracture_zones` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No fracture zones have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.fracture_zones is None:
+            raise ValueError("No fracture zones passed to PlotTopologies.")
+
+        fracture_zone_lines = shapelify_feature_lines(self.fracture_zones)
+        gdf = gpd.GeoDataFrame({"geometry": fracture_zone_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_fracture_zones(self, ax, color='black', **kwargs):
         """Plot fracture zones on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1736,19 +2229,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with fracture zones plotted onto the chosen map projection.
         """
-        fracture_zone_lines = shapelify_feature_lines(self.fracture_zones)
-        gdf = gpd.GeoDataFrame({"geometry": fracture_zone_lines}, geometry="geometry")
+        gdf = self.get_fracture_zones()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_inferred_paleo_boundaries(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed inferred paleo boundary lines. 
+
+        Notes
+        -----
+        The `inferred_paleo_boundaries` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `inferred_paleo_boundaries` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `inferred_paleo_boundaries` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `inferred_paleo_boundaries` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No inferred paleo boundaries have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.inferred_paleo_boundaries is None:
+            raise ValueError("No inferred paleo boundaries passed to PlotTopologies.")
+
+        inferred_paleo_boundary_lines = shapelify_feature_lines(self.inferred_paleo_boundaries)
+        gdf = gpd.GeoDataFrame({"geometry": inferred_paleo_boundary_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_inferred_paleo_boundaries(self, ax, color='black', **kwargs):
         """Plot inferred paleo boundaries on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1765,19 +2298,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with inferred paleo boundaries plotted onto the chosen map projection.
         """
-        inferred_paleo_boundary_lines = shapelify_feature_lines(self.inferred_paleo_boundaries)
-        gdf = gpd.GeoDataFrame({"geometry": inferred_paleo_boundary_lines}, geometry="geometry")
+        gdf = get_inferred_paleo_boundaries()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_terrane_boundaries(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed terrane boundary lines. 
+
+        Notes
+        -----
+        The `terrane_boundaries` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `terrane_boundaries` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `terrane_boundaries` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `terrane_boundaries` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No terrane boundaries have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.terrane_boundaries is None:
+            raise ValueError("No terrane boundaries passed to PlotTopologies.")
+
+        terrane_boundary_lines = shapelify_feature_lines(self.terrane_boundaries)
+        gdf = gpd.GeoDataFrame({"geometry": terrane_boundary_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_terrane_boundaries(self, ax, color='black', **kwargs):
         """Plot terrane boundaries on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1794,19 +2367,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with terrane boundaries plotted onto the chosen map projection.
         """
-        terrane_boundary_lines = shapelify_feature_lines(self.terrane_boundaries)
-        gdf = gpd.GeoDataFrame({"geometry": terrane_boundary_lines}, geometry="geometry")
+        gdf = self.get_terrane_boundaries()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_transitional_crusts(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed transitional crust lines. 
+
+        Notes
+        -----
+        The `transitional_crusts` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `transitional_crusts` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `transitional_crusts` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `transitional_crusts` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No transitional crusts have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.transitional_crusts is None:
+            raise ValueError("No transitional crusts passed to PlotTopologies.")
+
+        transitional_crust_lines = shapelify_feature_lines(self.transitional_crusts)
+        gdf = gpd.GeoDataFrame({"geometry": transitional_crust_lines}, geometry="geometry")
+        return gdf 
+
+
     def plot_transitional_crusts(self, ax, color='black', **kwargs):
         """Plot transitional crust on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1823,19 +2436,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with transitional crust plotted onto the chosen map projection.
         """
-        transitional_crust_lines = shapelify_feature_lines(self.transitional_crusts)
-        gdf = gpd.GeoDataFrame({"geometry": transitional_crust_lines}, geometry="geometry")
+        gdf = self.get_transitional_crusts()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_orogenic_belts(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed orogenic belt lines. 
+
+        Notes
+        -----
+        The `orogenic_belts` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `orogenic_belts` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `orogenic_belts` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `orogenic_belts` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No orogenic belts have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.orogenic_belts is None:
+            raise ValueError("No orogenic belts passed to PlotTopologies.")
+
+        orogenic_belt_lines = shapelify_feature_lines(self.orogenic_belts)
+        gdf = gpd.GeoDataFrame({"geometry": orogenic_belt_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_orogenic_belts(self, ax, color='black', **kwargs):
         """Plot orogenic belts on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1852,19 +2505,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with orogenic belts plotted onto the chosen map projection.
         """
-        orogenic_belt_lines = shapelify_feature_lines(self.orogenic_belts)
-        gdf = gpd.GeoDataFrame({"geometry": transitional_crust_lines}, geometry="geometry")
+        gdf = self.get_orogenic_belts()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_sutures(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed suture lines. 
+
+        Notes
+        -----
+        The `sutures` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `sutures` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `sutures` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `sutures` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No sutures have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.sutures is None:
+            raise ValueError("No sutures passed to PlotTopologies.")
+
+        suture_lines = shapelify_feature_lines(self.sutures)
+        gdf = gpd.GeoDataFrame({"geometry": suture_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_sutures(self, ax, color='black', **kwargs):
         """Plot sutures on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1881,19 +2574,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with sutures plotted onto the chosen map projection.
         """
-        suture_lines = shapelify_feature_lines(self.sutures)
-        gdf = gpd.GeoDataFrame({"geometry": suture_lines}, geometry="geometry")
+        gdf = self.get_sutures()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_continental_crusts(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed continental crust lines. 
+
+        Notes
+        -----
+        The `continental_crusts` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `continental_crusts` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `continental_crusts` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `continental_crusts` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No continental crust topologies have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.continental_crusts is None:
+            raise ValueError("No continental crust topologies passed to PlotTopologies.")
+
+        continental_crust_lines = shapelify_feature_lines(self.continental_crusts)
+        gdf = gpd.GeoDataFrame({"geometry": continental_crust_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_continental_crusts(self, ax, color='black', **kwargs):
         """Plot continental crust lines on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1910,19 +2643,58 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with continental crust lines plotted onto the chosen map projection.
         """
-        continental_crust_lines = shapelify_feature_lines(self.continental_crusts)
-        gdf = gpd.GeoDataFrame({"geometry": continental_crust_lines}, geometry="geometry")
+        gdf = self.get_continental_crusts()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_extended_continental_crusts(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed extended continental crust lines. 
+
+        Notes
+        -----
+        The `extended_continental_crusts` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `extended_continental_crusts` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `extended_continental_crusts` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `extended_continental_crusts` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No extended continental crust topologies have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.extended_continental_crusts is None:
+            raise ValueError("No extended continental crust topologies passed to PlotTopologies.")
+
+        extended_continental_crust_lines = shapelify_feature_lines(self.extended_continental_crusts)
+        gdf = gpd.GeoDataFrame({"geometry": extended_continental_crust_lines}, geometry="geometry")
+        return gdf
+
     def plot_extended_continental_crusts(self, ax, color='black', **kwargs): 
         """Plot extended continental crust lines on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1939,19 +2711,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with extended continental crust lines plotted onto the chosen map projection.
         """
-        extended_continental_crust_lines = shapelify_feature_lines(self.extended_continental_crusts)
-        gdf = gpd.GeoDataFrame({"geometry": extended_continental_crust_lines}, geometry="geometry")
+        gdf = self.get_extended_continental_crusts()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_passive_continental_boundaries(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed passive continental boundary lines. 
+
+        Notes
+        -----
+        The `passive_continental_boundaries` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `passive_continental_boundaries` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `passive_continental_boundaries` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `passive_continental_boundaries` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No passive continental boundaries have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.passive_continental_boundaries is None:
+            raise ValueError("No passive continental boundaries passed to PlotTopologies.")
+
+        passive_continental_boundary_lines = shapelify_feature_lines(self.passive_continental_boundaries)
+        gdf = gpd.GeoDataFrame({"geometry": passive_continental_boundary_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_passive_continental_boundaries(self, ax, color='black', **kwargs): 
         """Plot passive continental boundaries on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1968,19 +2780,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with passive continental boundaries plotted onto the chosen map projection.
         """
-        passive_continental_boundary_lines = shapelify_feature_lines(self.passive_continental_boundaries)
-        gdf = gpd.GeoDataFrame({"geometry": passive_continental_boundary_lines}, geometry="geometry")
+        gdf = self.get_passive_continental_boundaries()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_slab_edges(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed slab edge lines. 
+
+        Notes
+        -----
+        The `slab_edges` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `slab_edges` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `slab_edges` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `slab_edges` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No slab edges have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.slab_edges is None:
+            raise ValueError("No slab edges passed to PlotTopologies.")
+
+        slab_edge_lines = shapelify_feature_lines(self.slab_edges)
+        gdf = gpd.GeoDataFrame({"geometry": slab_edge_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_slab_edges(self, ax, color='black', **kwargs): 
         """Plot slab edges on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -1997,19 +2849,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with slab edges plotted onto the chosen map projection.
         """
-        slab_edge_lines = shapelify_feature_lines(self.slab_edges)
-        gdf = gpd.GeoDataFrame({"geometry": slab_edge_lines}, geometry="geometry")
+        gdf = self.get_slab_edges()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_misc_transforms(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed misc transform lines. 
+
+        Notes
+        -----
+        The `misc_transforms` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `misc_transforms` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `misc_transforms` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `misc_transforms` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No miscellaneous transforms have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.misc_transforms is None:
+            raise ValueError("No miscellaneous transforms passed to PlotTopologies.")
+
+        misc_transform_lines = shapelify_feature_lines(self.misc_transforms)
+        gdf = gpd.GeoDataFrame({"geometry": misc_transform_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_misc_transforms(self, ax, color='black', **kwargs): 
         """Plot miscellaneous transform boundaries on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -2026,19 +2918,59 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with miscellaneous transform boundaries plotted onto the chosen map projection.
         """
-        misc_transform_lines = shapelify_feature_lines(self.misc_transforms)
-        gdf = gpd.GeoDataFrame({"geometry": misc_transform_lines}, geometry="geometry")
+        gdf = self.get_misc_transforms()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
 
 
+    def get_unclassified_features(self):
+        """Create a geopandas.GeoDataFrame object containing geometries of reconstructed unclassified feature lines. 
+
+        Notes
+        -----
+        The `unclassified_features` needed to produce the GeoDataFrame are automatically constructed if the optional `time` 
+        parameter is passed to the `PlotTopologies` object before calling this function. `time` can be passed 
+        either when `PlotTopologies` is first called...
+
+            gplot = gplately.PlotTopologies(..., time=100,...)
+
+        or anytime afterwards, by setting:
+
+            time = 100 #Ma
+            gplot.time = time
+
+        ...after which this function can be re-run. Once the `unclassified_features` are reconstructed, they are 
+        converted into Shapely lines whose coordinates are passed to a geopandas GeoDataFrame.
+
+        Returns
+        -------
+        gdf : instance of <geopandas.GeoDataFrame>
+            A pandas.DataFrame that has a column with `unclassified_features` geometry.
+
+        Raises 
+        ------
+        ValueError
+            If the optional `time` parameter has not been passed to `PlotTopologies`. This is needed to construct
+            `unclassified_features` to the requested `time` and thus populate the GeoDataFrame.
+        """
+        if self._time is None:
+            raise ValueError("No unclassified features have been resolved. Set `PlotTopologies.time` to construct them.")
+
+        if self.unclassified_features is None:
+            raise ValueError("No unclassified features passed to PlotTopologies.")
+
+        unclassified_feature_lines = shapelify_feature_lines(self.unclassified_features)
+        gdf = gpd.GeoDataFrame({"geometry": unclassified_feature_lines}, geometry="geometry")
+        return gdf
+
+
     def plot_unclassified_features(self, ax, color='black', **kwargs): 
         """Plot GPML unclassified features on a standard map projection.
 
         Parameters
         ----------
         ax : instance of <cartopy.mpl.geoaxes.GeoAxes> or <cartopy.mpl.geoaxes.GeoAxesSubplot>
             A subclass of `matplotlib.axes.Axes` which represents a map Projection.
@@ -2055,11 +2987,10 @@
 
         Returns
         -------
         ax : instance of <geopandas.GeoDataFrame.plot>
             A standard cartopy.mpl.geoaxes.GeoAxes or cartopy.mpl.geoaxes.GeoAxesSubplot map 
             with unclassified features plotted onto the chosen map projection.
         """
-        unclassified_feature_lines = shapelify_feature_lines(self.unclassified_features)
-        gdf = gpd.GeoDataFrame({"geometry": unclassified_feature_lines}, geometry="geometry")
+        gdf = self.get_unclassified_features()
         return gdf.plot(ax=ax, facecolor='none', edgecolor=color, transform=self.base_projection, **kwargs)
```

### Comparing `gplately-0.3.3/gplately/reconstruction.py` & `gplately-0.4/gplately/reconstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Tools that wrap up pyGplates and Plate Tectonic Tools functionalities for reconstructing features,
  working with point data, and calculating plate velocities at specific geological times. 
 """
-import pygplates
+import math
+import os
+import warnings
+
 import numpy as np
 import ptt
-import warnings
-import math
+import pygplates
+
 from . import tools as _tools
+from .gpml import _load_FeatureCollection
 from .pygplates import RotationModel as _RotationModel
 from .pygplates import FeatureCollection as _FeatureCollection
-from .gpml import _load_FeatureCollection
 
 
 class PlateReconstruction(object):
     """The `PlateReconstruction` class contains methods to reconstruct topology features to specific 
     geological times given a `rotation_model`, a set of `topology_features` and a set of 
     `static_polygons`. Topological plate velocity data at specific geological times can also be 
     calculated from these reconstructed features. 
@@ -246,106 +249,114 @@
                     clat, clon = shared_sub_segment.get_resolved_geometry().get_centroid().to_lat_lon()
                     earth_radius = _tools.geocentric_radius(clat) / 1e3
                     total_subduction_zone_length_kms += shared_sub_segment.get_resolved_geometry().get_arc_length()*earth_radius
 
             return total_subduction_zone_length_kms
 
 
-    def total_continental_arc_length(self, time, continental_grid=None, trench_arc_distance=0.0, ignore_warnings=True):
+    def total_continental_arc_length(
+        self,
+        time,
+        continental_grid,
+        trench_arc_distance,
+        ignore_warnings=True,
+    ):
         """Calculates the total length of all global continental arcs (km) at the specified geological time (Ma).
 
         Uses Plate Tectonic Tools' `subduction_convergence` workflow to sample a given plate model's trench features into 
         point features and obtain their subduction polarities. The resolved points are projected out by the `trench_arc_distance`
         and their new locations are linearly interpolated onto the supplied `continental_grid`. If the projected trench 
         points lie in the grid, they are considered continental arc points, and their arc segment lengths are appended 
         to the total continental arc length for the specified `time`. The total length is scaled to kilometres using the geocentric 
         Earth radius. 
 
         Parameters
         ----------
         time : int
             The geological time at which to calculate total continental arc lengths.
-        continental_grid: str or MaskedArray, default=None
-            A MaskedArray or full string path to a continental grid with which to interpolate projected trench points on 
-            (thereby identifying continental arc points). 
-        trench_arc_distance : float, default=0.0
+        continental_grid: Raster, array_like, or str
+            The continental grid used to identify continental arc points. Must
+            be convertible to `Raster`. For an array, a global extent is
+            assumed [-180,180,-90,90]. For a filename, the extent is obtained
+            from the file.
+        trench_arc_distance : float
             The trench-to-arc distance (in kilometres) to project sampled trench points out by in the direction of their 
             subduction polarities. 
-        ignore_warnings : bool, default=False
+        ignore_warnings : bool, default=True
             Choose whether to ignore warning messages from PTT's subduction_convergence workflow that alerts the user of 
             subduction sub-segments that are ignored due to unidentified polarities and/or subducting plates. 
 
-        Raises
-        ------
-        ValueError
-            * If a continental grid directory is not supplied.
-            * If the trench_arc_distance is not supplied or kept at 0.0km.
-
         Returns
         -------
         total_continental_arc_length_kms : float
             The continental arc length (in km) at the specified time.
         """
         from . import grids as _grids
-        # Right now, raster reconstruction is not supported.
-        if continental_grid is None:
-            raise ValueError("Please provide a directory to a continental grid or a masked array for the current time.")
-        
-        elif isinstance(continental_grid, np.ndarray):
-            # Process the masked continental grid
-            graster = _grids.Raster(data=continental_grid, extent=[-180,180,-90,90])
 
+        if isinstance(continental_grid, _grids.Raster):
+            graster = continental_grid
         elif isinstance(continental_grid, str):
             # Process the continental grid directory
-            graster = _grids.Raster(data=continental_grid, extent=[-180,180,-90,90])
+            graster = _grids.Raster(
+                data=continental_grid,
+                realign=True,
+                time=float(time),
+            )
+        else:
+            # Process the masked continental grid
+            try:
+                continental_grid = np.array(continental_grid)
+                graster = _grids.Raster(
+                    data=continental_grid,
+                    extent=[-180,180,-90,90],
+                    time=float(time),
+                )
+            except Exception as e:
+                raise TypeError(
+                    "Invalid type for `continental_grid` (must be Raster,"
+                    + " str, or array_like)"
+                ) from e
+        if (time != graster.time) and (not ignore_warnings):
+            raise RuntimeWarning(
+                "`continental_grid.time` ({}) ".format(graster.time)
+                + "does not match `time` ({})".format(time)
+            )
 
         # Obtain trench data with Plate Tectonic Tools
         trench_data = self.tesselate_subduction_zones(time, ignore_warnings=ignore_warnings)
-        
+
         # Extract trench data
         trench_normal_azimuthal_angle = trench_data[:,7]
         trench_arcseg = trench_data[:,6]
         trench_pt_lon = trench_data[:,0]
         trench_pt_lat = trench_data[:,1]
-        
+
         # Modify the trench-arc distance using the geocentric radius
         arc_distance = trench_arc_distance / (_tools.geocentric_radius(trench_pt_lat)/1000)
-        
+
         # Project trench points out along trench-arc distance, and obtain their new lat-lon coordinates
         dlon = arc_distance*np.sin(np.radians(trench_normal_azimuthal_angle))
         dlat = arc_distance*np.cos(np.radians(trench_normal_azimuthal_angle))
         ilon = trench_pt_lon + np.degrees(dlon)
         ilat = trench_pt_lat + np.degrees(dlat)
-        
+
         # Linearly interpolate projected points onto continental grids, and collect the indices of points that lie
         # within the grids.
-        sampled_points = graster.interpolate(ilon, ilat, method='linear', return_indices=True, return_distances=False)     
-        in_raster = [i for i, point in enumerate(sampled_points[0]) if point > 0]
-        
-        # Define arrays + total arc length
-        lat_in = []
-        lon_in = []
-        total_continental_arc_length_kms = 0
-        subd_we_count_lat = []
-        subd_we_count_lon = []
-        
-        # Loop through all successful in-raster indices
-        for index in in_raster:
-            
-            # Get the lat-lon coordinate of the in-raster point, and the corresponding trench point
-            lat_in.append(ilat[index])
-            lon_in.append(ilon[index])
-            subd_we_count_lat.append(trench_pt_lat[index])
-            subd_we_count_lon.append(trench_pt_lon[index])
-
-            # Append the continental trench segment to the total arc length
-            earth_radius = _tools.geocentric_radius(trench_pt_lat[index])/1000
-            total_continental_arc_length_kms += np.deg2rad(trench_data[:,6][index])*earth_radius
-            
-        return total_continental_arc_length_kms
+        sampled_points = graster.interpolate(
+            ilon,
+            ilat,
+            method='linear',
+            return_indices=False,
+        )
+        continental_indices = np.where(sampled_points > 0)
+        point_lats = ilat[continental_indices]
+        point_radii = _tools.geocentric_radius(point_lats) * 1.0e-3  # km
+        segment_arclens = np.deg2rad(trench_arcseg[continental_indices])
+        segment_lengths = point_radii * segment_arclens
+        return np.sum(segment_lengths)
 
 
     def tesselate_mid_ocean_ridges(self, time, tessellation_threshold_radians=0.001, ignore_warnings=False, **kwargs):
         """Samples points along resolved spreading features (e.g. mid-ocean ridges) and calculates spreading rates and 
         lengths of ridge segments at a particular geological time.
          
         Resolves topologies at `time`, tessellates all resolved spreading features to within 'tessellation_threshold_radians'
@@ -923,17 +934,17 @@
     """`Points` contains methods to reconstruct and work with with geological point data. For example, the 
     locations and plate velocities of point data can be calculated at a specific geological `time`. The `Points` 
     object requires the `PlateReconstruction` object to work because it holds the `rotation_model` and `static_polygons` 
     needed to classify topological plates and quantify feature rotations through time. 
 
     Attributes
     ----------
-    PlateReconstruction_object : object pointer
+    plate_reconstruction : object pointer
         Allows for the accessibility of `PlateReconstruction` object attributes: `rotation_model`, `topology_featues` 
-        and `static_polygons` for use in the `Points` object if called using “self.PlateReconstruction_object.X”, 
+        and `static_polygons` for use in the `Points` object if called using “self.plate_reconstruction.X”, 
         where X is the attribute.
 
     lons : float, or 1D array
         A single float, or a 1D array containing the longitudes of point data.
 
     lats : float 1D array
         A single float, or a 1D array containing the latitudes of point data.
@@ -943,25 +954,23 @@
         the present day (0 Ma).
 
     plate_id : int, default=None
         The plate ID of a particular tectonic plate on which point data lies, if known. This is obtained in `init` 
         if not provided.
 
     """
-    def __init__(self, PlateReconstruction_object, lons, lats, time=0, plate_id=None):
+    def __init__(self, plate_reconstruction, lons, lats, time=0, plate_id=None):
         self.lons = lons
         self.lats = lats
         self.time = time
 
-        self.PlateReconstruction_object = PlateReconstruction_object
+        self.plate_reconstruction = plate_reconstruction
 
         self.update(lons, lats, time, plate_id)
 
-        # Deprecated name of `plate_reconstruction` attribute
-        self.plate_reconstruction = self.PlateReconstruction_object
 
     def update(self, lons, lats, time=0, plate_id=None):
 
         # get Cartesian coordinates
         self.x, self.y, self.z = _tools.lonlat2xyz(lons, lats, degrees=False)
 
         # scale by average radius of the Earth
@@ -970,16 +979,16 @@
         self.z *= _tools.EARTH_RADIUS
 
         # store concatenated arrays
         self.lonlat = np.c_[self.lons, self.lats]
         self.xyz = np.c_[self.x, self.y, self.z]
 
 
-        rotation_model = self.PlateReconstruction_object.rotation_model
-        static_polygons = self.PlateReconstruction_object.static_polygons
+        rotation_model = self.plate_reconstruction.rotation_model
+        static_polygons = self.plate_reconstruction.static_polygons
         
 
         features = _tools.points_to_features(lons, lats, plate_id)
 
         if plate_id is not None:
             plate_id = np.atleast_1d(plate_id)
             self.features = features
@@ -999,43 +1008,47 @@
 
         self.plate_id = plate_id
         self.FeatureCollection = pygplates.FeatureCollection(self.features)
 
 
     def __getstate__(self):
 
-        filenames = self.PlateReconstruction_object.__getstate__()
+        filenames = self.plate_reconstruction.__getstate__()
 
         # add important variables from Points object
         filenames["lons"] = self.lons
         filenames["lats"] = self.lats
         filenames['time'] = self.time
         filenames['plate_id'] = self.plate_id
 
-        del self.FeatureCollection, self.features
-
-        self.FeatureCollection = None
-        self.features = None
-
         return filenames
 
     def __setstate__(self, state):
 
-        self.PlateReconstruction_object = PlateReconstruction(state['rotation_model'], state['topology_features'], state['static_polygons'])
+        self.plate_reconstruction = PlateReconstruction(state['rotation_model'], state['topology_features'], state['static_polygons'])
 
         # reinstate unpicklable items
         self.lons = state['lons']
         self.lats = state['lats']
         self.time = state['time']
         self.plate_id = state['plate_id']
 
         self.update(self.lons, self.lats, self.time, self.plate_id)
 
+    def copy(self):
+        """ Returns a copy of the Points object
+
+        Returns
+        -------
+        Points
+            A copy of the current Points object
+        """
+        return Points(self.plate_reconstruction, self.lons, self.lats, self.time, self.plate_id)
 
-    def reconstruct(self, time, anchor_plate_id=0, **kwargs):
+    def reconstruct(self, time, anchor_plate_id=0, return_array=False, **kwargs):
         """Reconstructs regular geological features, motion paths or flowlines to a specific geological time and extracts 
         the latitudinal and longitudinal points of these features.
 
         Note: this method accesses and uses the rotation model attribute from the PointReconstruction object, and reconstructs 
         the feature lat-lon point attributes of the Points object.
 
         Parameters
@@ -1044,14 +1057,17 @@
             The specific geological time (Ma) to reconstruct features to.
 
         anchor_plate_id : int, default=0
             Reconstruct features with respect to a certain anchor plate. By default, reconstructions are made 
             with respect to the absolute reference frame, like a stationary geological element (e.g. a mantle
             plume). This frame is given the plate ID of 0.
 
+        return_array : bool, default False
+            Return a `numpy.ndarray`, rather than a `Points` object.
+
         **reconstruct_type : ReconstructType, default=ReconstructType.feature_geometry
             The specific reconstruction type to generate based on input feature geometry type. Can be provided as
             ReconstructType.feature_geometry to only reconstruct regular feature geometries, or ReconstructType.MotionPath to
             only reconstruct motion path features, or ReconstructType.Flowline to only reconstruct flowline features. Generates
             :class:`reconstructed feature geometries<ReconstructedFeatureGeometry>’, or :class:`reconstructed motion
             paths<ReconstructedMotionPath>’, or :class:`reconstructed flowlines<ReconstructedFlowline>’ respectively.
 
@@ -1076,19 +1092,22 @@
         Raises
         ------
         NotImplementedError
             if the starting time for reconstruction `from_time` is not equal to 0.0
         """
         from_time = self.time
         to_time = time
-        reconstructed_features = self.PlateReconstruction_object.reconstruct(
+        reconstructed_features = self.plate_reconstruction.reconstruct(
             self.features, to_time, from_time, anchor_plate_id=anchor_plate_id, **kwargs)
 
         rlons, rlats = _tools.extract_feature_lonlat(reconstructed_features)
-        return rlons, rlats
+        if return_array:
+            return rlons, rlats
+        else:
+            return Points(self.plate_reconstruction, rlons, rlats, time=to_time, plate_id=self.plate_id)
 
 
     def reconstruct_to_birth_age(self, ages, anchor_plate_id=0, **kwargs):
         """ Reconstructs point features supplied to the `Points` object from the supplied initial time (`self.time`)
         to a range of times. The number of supplied times must equal the number of point features supplied to the Points object. 
 
         Attributes
@@ -1139,15 +1158,15 @@
         unique_ages = np.unique(ages)
         rlons = np.zeros(ages.shape)
         rlats = np.zeros(ages.shape)
 
         for age in unique_ages:
             mask_age = ages == age
 
-            reconstructed_features = self.PlateReconstruction_object.reconstruct(
+            reconstructed_features = self.plate_reconstruction.reconstruct(
                 self.features, age, from_time, anchor_plate_id=anchor_plate_id, **kwargs)
 
             lons, lats = _tools.extract_feature_lonlat(reconstructed_features)
 
             rlons[mask_age] = lons[mask_age]
             rlats[mask_age] = lats[mask_age]
 
@@ -1177,15 +1196,15 @@
         all_velocities.T : 2D numpy list
             A transposed 2D numpy list with two rows and a number of columns equal to the number of x,y Cartesian velocity 
             components obtained (and thus the number of feature points extracted from a supplied feature). Each list column 
             stores one point’s x,y, velocity components along its two rows.
         """
         time = float(time)
 
-        rotation_model = self.PlateReconstruction_object.rotation_model
+        rotation_model = self.plate_reconstruction.rotation_model
         all_velocities = np.empty((len(self.features), 2))
 
         for i, feature in enumerate(self.features):
             geometry = feature.get_geometry()
             partitioning_plate_id = feature.get_reconstruction_plate_id()
             equivalent_stage_rotation = rotation_model.get_rotation(time, partitioning_plate_id, time+delta_time)
             
@@ -1258,15 +1277,15 @@
                 time_array.tolist(),
                 valid_time=(time_array.max(), time_array.min()),
                 #relative_plate=int(self.plate_id[i]),
                 #reconstruction_plate_id=int(anchor_plate_id))
                 relative_plate=int(anchor_plate_id),
                 reconstruction_plate_id=int(self.plate_id[i]))
 
-            reconstructed_motion_paths = self.PlateReconstruction_object.reconstruct(
+            reconstructed_motion_paths = self.plate_reconstruction.reconstruct(
                 motion_path_feature, 
                 to_time=0, 
                 #from_time=0, 
                 reconstruct_type=pygplates.ReconstructType.motion_path)
 
             # Turn motion paths in to lat-lon coordinates
             for reconstructed_motion_path in reconstructed_motion_paths:
@@ -1367,15 +1386,15 @@
         
             for i in np.arange(0,len(seed_points)):
                 left_flowline_longitudes = left_lon[:,i] 
                 left_flowline_latitudes = left_lat[:,i] 
                 right_flowline_longitudes = right_lon[:,i]
                 right_flowline_latitudes = right_lat[:,i]
         """
-        model = self.PlateReconstruction_object
+        model = self.plate_reconstruction
         return model.create_flowline(self.lons, self.lats, time_array, left_plate_ID, right_plate_ID, return_rate_of_motion)
 
 
     def save(self, filename):
         """Saves the feature collection used in the Points object under a given filename to the current directory. 
 
         The needed file format to save to is determined from the filename extension. 
@@ -1614,30 +1633,62 @@
 
 class _ContinentCollision(object):
     """
     Continental collision detection function class (the function is the '__call__' method).
     """
 
     def __init__(
-            self,
-            grd_output_dir,
-            chain_collision_detection=_DEFAULT_COLLISION):
+        self,
+        grd_output_dir,
+        chain_collision_detection=_DEFAULT_COLLISION,
+        verbose=False,
+    ):
         """
         grd_output_dir: The directory containing the continental grids.
 
         chain_collision_detection: Another collision detection class/function to reference if we find no collision.
                                    If None then no collision detection is chained. Defaults to the default collision detection.
+
+        verbose: Print progress messages
         """
         
         self.grd_output_dir = grd_output_dir
         self.chain_collision_detection = chain_collision_detection
+        self.verbose = verbose
         
         # Load a new grid each time the reconstruction time changes.
         self.grid_time = None
 
+    @property
+    def grid_time(self):
+        return self._grid_time
+
+    @grid_time.setter
+    def grid_time(self, time):
+        from .grids import read_netcdf_grid
+
+        if time is None:
+            self._grid_time = time
+        else:
+            filename = '{:s}'.format(self.grd_output_dir.format(time))
+            if self.verbose:
+                print(
+                    'Points masked against grid: {0}'.format(
+                        os.path.basename(filename)
+                    )
+                )
+            gridZ, gridX, gridY = read_netcdf_grid(filename, return_grids=True)
+            self.gridZ = gridZ
+            self.ni, self.nj = gridZ.shape
+            self.xmin = np.nanmin(gridX)
+            self.xmax = np.nanmax(gridX)
+            self.ymin = np.nanmin(gridY)
+            self.ymax = np.nanmax(gridY)
+            self._grid_time = float(time)
+
 
     def __call__(
             self,
             rotation_model,
             time,
             reconstruction_time_interval,
             prev_point,
@@ -1646,44 +1697,42 @@
             prev_resolved_plate_boundary,
             curr_topology_plate_id,
             curr_resolved_plate_boundary):
         """
         Returns True if a collision with a continent was detected, or returns result of
         chained collision detection if 'self.chain_collision_detection' is not None.
         """
-
-        # Import locally so that we only get import errors if we use this class (and don't have the required dependencies).
-        # Not sure if importing locally like this will slow down executation a lot ?
-        from scipy.interpolate import RegularGridInterpolator
-        # from gprm.utils.fileio import load_netcdf
-        from .grids import read_netcdf_grid
-
         # Load the grid for the current time if encountering a new time.
         if time != self.grid_time:
             self.grid_time = time
-            
-            # Load a grid that is based on the continent masks, assuming the detect_continents
-            # are represented by NaNs
-            # The grid is sampled at each point, and in NaN retrurned, the point is set to inactive
-            filename = '{:s}'.format(self.grd_output_dir.format(time))
-            print('Points masked against grid: {0}'.format(filename))
-            gridZ,gridX,gridY = read_netcdf_grid(filename, return_grids=True)
             self.continent_deletion_count = 0
 
-            self.f = RegularGridInterpolator((gridX,gridY), gridZ.T, method='nearest')
-
-        # interpolate grid, which is one over continents and zero over oceans.
-        # if value is >0.5 we deactivate
-        #print curr_point
-        if self.f([curr_point.to_lat_lon()[1], curr_point.to_lat_lon()[0]])>0.5:
-            #print 'deactivating point within continent'
-            self.continent_deletion_count += 1
+        # Sample mask grid, which is one over continents and zero over oceans.
+        point_lat, point_lon = curr_point.to_lat_lon()
+        point_i = (self.ni - 1) * (
+            (point_lat - self.ymin)
+            / (self.ymax - self.ymin)
+        )
+        point_j = (self.nj - 1) * (
+            (point_lon - self.xmin)
+            / (self.xmax - self.xmin)
+        )
+        point_i_uint = np.rint(point_i).astype(np.uint)
+        point_j_uint = np.rint(point_j).astype(np.uint)
+        try:
+            mask_value = self.gridZ[point_i_uint, point_j_uint]
+        except IndexError:
+            point_i = np.clip(np.rint(point_i), 0, self.ni - 1).astype(np.int_)
+            point_j = np.clip(np.rint(point_j), 0, self.nj - 1).astype(np.int_)
+            mask_value = self.gridZ[point_i, point_j]
+        if mask_value >= 0.5:
             # Detected a collision.
+            self.continent_deletion_count += 1
             return True
-        
+
         # We didn't find a collision, so ask the chained collision detection if it did (if we have anything chained).
         if self.chain_collision_detection:
             return self.chain_collision_detection(
                     rotation_model,
                     time,
                     reconstruction_time_interval,
                     prev_point,
@@ -2083,9 +2132,7 @@
             # topologies. So it will be skipped and thrown away from future iterations.
             if curr_polygon is None:
                 self.curr_topology_plate_ids[point_index] = None
                 continue
             
             # Set the plate ID of resolved topology containing current point.
             self.curr_topology_plate_ids[point_index] = curr_polygon.get_feature().get_reconstruction_plate_id()
-
-
```

### Comparing `gplately-0.3.3/gplately/tools.py` & `gplately-0.4/gplately/tools.py`

 * *Files identical despite different names*

### Comparing `gplately-0.3.3/gplately.egg-info/PKG-INFO` & `gplately-0.4/gplately.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,141 @@
 Metadata-Version: 2.1
 Name: gplately
-Version: 0.3.3
+Version: 0.4
 Summary: Object-orientated Python interface to pyGPlates for plate tectonic reconstructions
 Home-page: https://github.com/GPlates/gplately
 Author: Ben Mather
 Author-email: ben.mather@sydney.edu.au
 License: UNKNOWN
-Description: # GPlately
+Description: <p align="center">
+        <picture>
+          <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_White_logo.png">
+          <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
+          <img alt="GPlately logo." src="https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/GPlately_Main_logo.png">
+        </picture>
+        </p>
+        
+        ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/GPlates/gplately/build_and_test.yml?branch=master&style=for-the-badge)
+        ![PyPI](https://img.shields.io/pypi/v/gplately?style=for-the-badge)
+        ![PyPI - Downloads](https://img.shields.io/pypi/dw/gplately?style=for-the-badge)
         
-        GPlately was created to accelerate spatio-temporal data analysis leveraging pyGPlates and PlateTectonicTools within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
+        
+        GPlately was created to accelerate spatio-temporal data analysis leveraging [pyGPlates](https://www.gplates.org/docs/pygplates/index.html) and [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) within a simplified Python interface. This object-oriented package enables the reconstruction of data through deep geologic time (points, lines, polygons, and rasters), the interrogation of plate kinematic information (plate velocities, rates of subduction and seafloor spreading), the rapid comparison between multiple plate motion models, and the plotting of reconstructed output data on maps. All tools are designed to be parallel-safe to accelerate spatio-temporal analysis over multiple CPU processors.
         
         ![SeedPointGIF](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/muller19_seedpoints.gif)
         
         
         GPlately requires a working installation of pyGPlates, which is freely
         available at https://www.gplates.org/download.
         All major system architectures (e.g. Linux, MacOS, Windows) are supported and installation instructions
         are [well documented](https://www.gplates.org/docs/pygplates/pygplates_getting_started.html\#installation).
         Sample data is also available from [EarthByte servers](https://www.earthbyte.org/category/resources/), which
         includes rasters, seafloor age grids, rotation files, and more to get started with plate reconstructions.
         
         #### Citation
         
-        _Coming soon!_
+        > Mather, B.R., Müller, R.D., Zahirovic, S., Cannon, J., Chin, M., Ilano, L., Wright, N.M., Alfonso, C., Williams, S., Tetley, M., Merdith, A. (2023) Deep time spatio-temporal data analysis using pyGPlates with PlateTectonicTools and GPlately. _Geoscience Data Journal_, 1–8. Available from: https://doi.org/10.1002/gdj3.185
+        
+        ```bib
+        @article{Mather2023,
+        author = {Mather, Ben R. and Müller, R. Dietmar and Zahirovic, Sabin and Cannon, John and Chin, Michael and Ilano, Lauren and Wright, Nicky M. and Alfonso, Christopher and Williams, Simon and Tetley, Michael and Merdith, Andrew},
+        title = {Deep time spatio-temporal data analysis using pyGPlates with PlateTectonicTools and GPlately},
+        year = {2023},
+        journal = {Geoscience Data Journal},
+        pages = {1-8},
+        keywords = {geospatial, plate reconstructions, pyGPlates, python, tectonics},
+        doi = {https://doi.org/10.1002/gdj3.185},
+        url = {https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/gdj3.185},
+        eprint = {https://rmets.onlinelibrary.wiley.com/doi/pdf/10.1002/gdj3.185},
+        }
+        ```
         
         ## Dependencies
         
         - [pyGPlates](https://www.gplates.org/docs/pygplates/pygplates_getting_started.html#installation)
         - [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools)
-        - [Shapely <2.0](https://shapely.readthedocs.io/en/stable/project.html#installing-shapely)
-        - NumPy
-        - SciPy 1.10
-        - Matplotlib
+        - [Shapely](https://shapely.readthedocs.io/en/stable/project.html#installing-shapely)
+        - [NumPy](https://numpy.org/install/) > 1.16
+        - [SciPy](https://scipy.org/install/) > 1.0
+        - [Matplotlib](https://matplotlib.org/stable/users/installing/index.html)
         - [Cartopy](https://scitools.org.uk/cartopy/docs/latest/index.html#getting-started) (for mapping)
-        - Shapely
+        - [Shapely](https://shapely.readthedocs.io/en/stable/installation.html)
         - [Pooch](https://github.com/fatiando/pooch)
-        - GeoPandas
-        - netCDF4
+        - [GeoPandas](https://geopandas.org/en/stable/getting_started.html)
+        - [netCDF4](https://unidata.github.io/netcdf4-python/#quick-install)
         
         
         ## Installation
         
-        ### Stable release
-        You can install the latest stable public release of `GPlately` using the pip package manager.
+        ### 1. Using conda (recommended)
         
-        ```python
+        You can install the latest stable public release of `GPlately` and all of its dependencies using conda.
+        This is the preferred method to install `GPlately` which downloads binaries from the conda-forge channel.
+        
+        ```sh
+        conda install -c conda-forge gplately
+        ```
+        
+        #### Creating a new conda environment
+        
+        We recommend creating a new conda environment inside which to install `GPlately`. This avoids any potential conflicts in your base Python environment. In the example below we create a new environment called "`my-env`":
+        
+        ```sh
+        conda create -n my-env
+        conda activate my-env
+        conda install -c conda-forge gplately
+        ```
+        
+        `my-env` needs to be activated whenever you use `GPlately`: i.e. `conda activate my-env`.
+        
+        ### 2. Using pip
+        
+        Alternatively, you can install the latest stable public release of `GPlately` using the pip package manager.
+        
+        ```sh
         pip install gplately
         ```
-        or:
+        or from this GitHub repository:
         
-        ```python
+        ```sh
         pip install git+https://github.com/GPlates/gplately.git 
         ```
         
-        ### Pull from repository 
+        #### Pull from repository 
         
         **First-time installation:** To install the latest version of GPlately from a specific repository branch (e.g. `master`), copy the following commands into your terminal:
         
-        ```python
+        ```sh
         cd /path/to/desired/directory #Change your command directory to where you'd like to clone GPlately
         git clone https://github.com/GPlates/gplately.git
-        pwd # Just to check your directory - should end with /.../gplately
+        cd gplately # navigate within the gplately folder
         git checkout master # or the name of whichever branch you need
         git pull # fetch all recent changes from this branch
         pip install .
         ```
         
         **Update installation from cloned repo:** To update your installation of GPlately by fetching the latest pushes from a specific repository branch (e.g. `master`), copy the following commands into your terminal:
         
-        ```python
+        ```sh
         cd /path/to/gplately/directory #Should be where gplately is cloned - must end in /.../gplately
         git checkout master # or the name of whichever branch you need
         git pull # fetch all recent changes from this branch
         pip install .
         ```
         
         
         ## Usage
         
         GPlately uses objects to accomplish a variety of common tasks. The common objects include:
         
-        - `DataServer` - download rotation files and topology features from plate models on EarthByte's webDAV server
-        - `PlateReconstruction` - reconstruct features, tesselate mid ocean ridges, subduction zones
-        - `Points` - partition points onto plates, rotate back through time
-        - `Raster` - read in NetCDF grids, interpolation, resampling
-        - `PlotTopologies` - one stop shop for plotting ridges, trenches, subduction teeth
+        - [`DataServer`](#the-dataserver-object) - download rotation files and topology features from plate models on EarthByte's webDAV server
+        - [`PlateReconstruction`](#the-platereconstruction-object) - reconstruct features, tesselate mid ocean ridges, subduction zones
+        - [`Points`](#the-points-object) - partition points onto plates, rotate back through time
+        - [`Raster`](#the-raster-object) - read in NetCDF grids, interpolation, resampling
+        - [`PlotTopologies`](#the-plottopologies-object) - one stop shop for plotting ridges, trenches, subduction teeth
         
         
         ### The `DataServer` object
         
         `GPlately`'s `DataServer` object can be used to download:
         
         - rotation models
@@ -116,46 +163,28 @@
         the object by passing a `rotation model`, a set of `topology features` and some `static polygons`: 
         
         ```python
         model = gplately.PlateReconstruction(rotation_model, topology_features, static_polygons)
         ```
         Launch the [Plate Reconstruction](https://github.com/GPlates/gplately/blob/master/Notebooks/02-PlateReconstructions.ipynb) notebook to see more.
         
-        
-        ### The `PlotTopologies` object
-        
-        ... can be used to visualise reconstructed feature geometries through time. To call the object, pass a set of `continents`, 
-        `coastlines` and `COBs` (either as file paths or as `<pyGPlates.FeatureCollection>` objects), as well as a `PlateReconstruction`
-        object, and a reconstruction `time`. 
-        
-        ```python
-        coastlines, continents, COBs = gDownload.get_topology_geometries()
-        time = 50 #Ma
-        gPlot = gplately.plot.PlotTopologies(model, time, coastlines, continents, COBs)
-        ```
-        Below are some continents, coastlines, COBs, ridges and transforms, trenches, subduction teeth and
-        seafloor age grids plotted using `PlotTopologies`!
-        
-        ![ReconstructionImage](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/plot_topologies_img.png)
-        
         ### The `Points` object
         
         ... can be used to reconstruct the positions of geological point features and calculate their underlying plate velocities 
         through geological time. 
         
         ```python
         pt_lon = np.array([-107.662152, -58.082792, 17.483189, 133.674590, 80.412876])
         pt_lat = np.array([48.797807, -12.654857, 11.884395, -26.415630, 31.368509])
         
         # Call the Points object: pass the PlateReconstruction object, and the latitudes and longitudes of the seed points!
         gpts = gplately.Points(model, pt_lon, pt_lat)
         ```
         ![PointData](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/surface_hotspot_plumes.png)
         
-        
         ### The `Raster` object
         
         ...can be used to read, resample and resize assorted raster data like `netCDF4` seafloor age grids, continental grids and ETOPO
         relief rasters. You can also reconstruct raster data back through geological time!
         
         ```python
         etopo = gdownload.get_raster("ETOPO1_tif")
@@ -175,27 +204,43 @@
         )
         ```
         
         Below is a plot of the [ETOPO1 global relief raster](https://www.ncei.noaa.gov/products/etopo-global-relief-model) at present day, and reconstructed to 50Ma:
         
         ![RasterImg](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/etopo_reconstruction.png)
         
+        ### The `PlotTopologies` object
+        
+        ... can be used to visualise reconstructed feature geometries through time. To call the object, pass a set of `continents`, 
+        `coastlines` and `COBs` (either as file paths or as `<pyGPlates.FeatureCollection>` objects), as well as a `PlateReconstruction`
+        object, and a reconstruction `time`. 
+        
+        ```python
+        coastlines, continents, COBs = gDownload.get_topology_geometries()
+        time = 50 #Ma
+        gPlot = gplately.plot.PlotTopologies(model, time, coastlines, continents, COBs)
+        ```
+        Below are some continents, coastlines, COBs, ridges and transforms, trenches, subduction teeth and
+        seafloor age grids plotted using `PlotTopologies`!
+        
+        ![ReconstructionImage](https://raw.githubusercontent.com/GPlates/gplately/master/Notebooks/NotebookFiles/ReadMe_Files/plot_topologies_img.png)
+        
         
         ## Sample workflows
         
         To see GPlately in action, launch a Jupyter Notebook environment and check out the [sample notebooks](./Notebooks):
         
         - [__01 - Getting Started__](https://github.com/GPlates/gplately/blob/master/Notebooks/01-GettingStarted.ipynb): A brief overview of how to initialise GPlately's main objects
         - [__02 - Plate Reconstructions__](https://github.com/GPlates/gplately/blob/master/Notebooks/02-PlateReconstructions.ipynb): Setting up a `PlateReconstruction` object, reconstructing geological data through time 
         - [__03 - Working with Points__](https://github.com/GPlates/gplately/blob/master/Notebooks/03-WorkingWithPoints.ipynb): Setting up a `Points` object, reconstructing seed point locations through time with. This notebook uses point data from the Paleobiology Database (PBDB).
         - [__04 - Velocity Basics__](https://github.com/GPlates/gplately/blob/master/Notebooks/04-VelocityBasics.ipynb): Calculating plate velocities, plotting velocity vector fields
         - [__05 - Working with Feature Geometries__](https://github.com/GPlates/gplately/blob/master/Notebooks/05-WorkingWithFeatureGeometries.ipynb): Processing and plotting assorted polyline, polygon and point data from [GPlates 2.3's sample data sets](https://www.earthbyte.org/gplates-2-3-software-and-data-sets/)
         - [__06 - Rasters__](https://github.com/GPlates/gplately/blob/master/Notebooks/06-Rasters.ipynb): Reading, resizing, resampling raster data, and linearly interpolating point data onto raster data
         - [__07 - Plate Tectonic Stats__](https://github.com/GPlates/gplately/blob/master/Notebooks/07-WorkingWithPlateTectonicStats.ipynb): Using [PlateTectonicTools](https://github.com/EarthByte/PlateTectonicTools) to calculate and plot subduction zone and ridge data (convergence/spreading velocities, subduction angles, subduction zone and ridge lengths, crustal surface areas produced and subducted etc.) 
-        - [__08 - Predicting Slab Dip__](https://github.com/GPlates/gplately/blob/master/Notebooks/08-PredictingSlabDip.ipynb): Predicting the average slab dip angle of subducting oceanic lithosphere.
+        - [__08 - Predicting Slab Flux__](https://github.com/GPlates/gplately/blob/master/Notebooks/08-PredictingSlabFlux.ipynb): Predicting the average slab dip angle of subducting oceanic lithosphere.
         - [__09 - Motion Paths and Flowlines__](https://github.com/GPlates/gplately/blob/master/Notebooks/09-CreatingMotionPathsAndFlowlines.ipynb): Using pyGPlates to create motion paths and flowines of points on a tectonic plate to illustrate the plate's trajectory through geological time.
         - [__10 - SeafloorGrid__](https://github.com/GPlates/gplately/blob/master/Notebooks/10-SeafloorGrids.ipynb): Defines the parameters needed to set up a `SeafloorGrid` object, and demonstrates how to produce age and spreading rate grids from a set of plate reconstruction model files.
         
         ## API Documentation
         
         Documentation of GPlately's objects and methods can be found [here](https://gplates.github.io/gplately/)!
```

### Comparing `gplately-0.3.3/gplately.egg-info/SOURCES.txt` & `gplately-0.4/gplately.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 gplately/__init__.py
 gplately/data.py
 gplately/download.py
 gplately/geometry.py
 gplately/gpml.py
```

### Comparing `gplately-0.3.3/setup.py` & `gplately-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 link_args = []
  
 if "Windows" in platform.system():
     link_args = ["-static"]
 
 # in development set version to none and ...
-PYPI_VERSION = "0.3.3"  # Note: don't add any dashes if you want to use conda, use b1 not .b1 
+PYPI_VERSION = "0.4"  # Note: don't add any dashes if you want to use conda, use b1 not .b1 
 
 # Return the git revision as a string (from numpy)
 
 def git_version():
     
     def _minimal_ext_cmd(cmd):
         # construct minimal environment
```

### Comparing `gplately-0.3.3/test/test_0_imports.py` & `gplately-0.4/test/test_0_imports.py`

 * *Files identical despite different names*

### Comparing `gplately-0.3.3/test/test_1_reconstructions.py` & `gplately-0.4/test/test_1_reconstructions.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,19 +74,44 @@
     assert total_ridge_length, "Could not calculate total MOR lengths for Muller et al. (2019) at {} Ma.".format(time)
 
 
 # TOTAL CONTINENTAL ARC LENGTHS AT 0 AND 100 MA
 @pytest.mark.parametrize("time", reconstruction_times)
 def test_cont_arc_length(time, model):
     gdownload = gplately.download.DataServer("Muller2019")
-    continental_grid_directory = gdownload.get_age_grid(time)
+
+    agegrid = gdownload.get_age_grid(time)
+    agegrid = agegrid.data
+    continental_grid = np.isnan(np.array(agegrid))
     # Use 281km as the trench-arc distance 281 km; the median distance frin global analysis at the present-day (Pall et al. 2018)
     trench_arc_distance = 281
-    total_cont_arc_length = model.total_continental_arc_length(time, continental_grid_directory, trench_arc_distance, ignore_warnings=True)
-    assert total_cont_arc_length, "Could not calculate total continental arc lengths for Muller et al. (2019) at {} Ma.".format(time)
+    total_cont_arc_length = model.total_continental_arc_length(
+        time,
+        continental_grid,
+        trench_arc_distance,
+        ignore_warnings=True,
+    )
+    approx_lengths = {
+        0: 51500,
+        100: 44000,
+    }
+    err_msg = (
+        "Could not calculate total continental arc lengths for Muller et "
+        + "al. (2019) at {} Ma.".format(time)
+    )
+    if time in approx_lengths.keys():
+        # Check arc length approximately matches precomputed value
+        cmp = approx_lengths[time]
+        diff = np.abs(total_cont_arc_length - cmp)
+        assert diff <= 500.0, err_msg
+    else:
+        # Value for this time has not been computed, so just make sure no
+        # errors were encountered
+        assert total_cont_arc_length >= 0.0, err_msg
+
 
 
 # POINT VELOCITIES
 @pytest.mark.parametrize("time", reconstruction_times)
 def test_point_velocities(time, model):
     lons = [-30]
     lats = [15]
```

### Comparing `gplately-0.3.3/test/test_2_points.py` & `gplately-0.4/test/test_2_points.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Ensures plate velocities are <insert condition here>. 
 
 """
 
 # TESTING THE POINTS OBJECT
 @pytest.mark.parametrize("time", reconstruction_times)
 def test_point_reconstruction(time, gpts):
-    rlons, rlats = gpts.reconstruct(time, anchor_plate_id=0)
+    rlons, rlats = gpts.reconstruct(time, return_array=True, anchor_plate_id=0)
     assert (rlons, rlats), "Unable to reconstruct point data to {} Ma with Muller et al. (2019).".format(time)
 
        
 # TESTING PLATE VELOCITY CALCULATIONS
 @pytest.mark.parametrize("time", reconstruction_times)
 def test_plate_velocity(time, gpts):
     plate_vel = gpts.plate_velocity(time, delta_time=1)
```

### Comparing `gplately-0.3.3/test/test_3_plottopologies.py` & `gplately-0.4/test/test_3_plottopologies.py`

 * *Files identical despite different names*

### Comparing `gplately-0.3.3/test/test_4_rasters.py` & `gplately-0.4/test/test_4_rasters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pytest
-import gplately
 import numpy as np
 from conftest import (
     reconstruction_times,
     pt_lon,
     pt_lat,
     gplately_raster_object as graster,
     gplately_merdith_raster,
@@ -25,32 +23,39 @@
     - reconstruct
         For the test, the present-day Müller et al. 2019 age grid is reconstructed to its
         configuration at 50 Ma.
 """
 
 # TEST LINEAR POINT DATA INTERPOLATION (WITH PT. COORDS FROM CONFTEST)
 def test_point_interpolation(graster):
-    interpolated_points = graster.interpolate(pt_lon, pt_lat, method='linear', return_indices=False, return_distances=False)
+    interpolated_points = graster.interpolate(
+        pt_lon,
+        pt_lat,
+        method='linear',
+        return_indices=False,
+    )
     assert interpolated_points.any(), "Unable to interpolate points"
 
 
 # TEST AGE GRID RESIZING (AT RESOLUTIONS OF RES_X = 1000, RES_Y = 400)
 def test_resizing(graster):
-    resized_agegrid = graster.resize(1000, 400, overwrite=False)
+    resized_agegrid = graster.resize(1000, 400, return_array=True)
     assert np.shape(resized_agegrid)==(400,1000), "Unable to rezise"
 
 
 # TEST FILLING NaNs IN AGE GRIDS
 def test_fill_NaNs(graster):
-    no_NaNs = graster.fill_NaNs(overwrite=False)
+    no_NaNs = graster.fill_NaNs(return_array=True)
     assert not np.isnan(no_NaNs).all(), "Unable to fill NaNs"
 
 def test_reconstruct(graster):
     reconstructed_raster = graster.reconstruct(50)
-    assert np.shape(reconstructed_raster), "Unable to reconstruct age grid"
+    assert (
+        np.shape(reconstructed_raster) == np.shape(graster)
+    ), "Unable to reconstruct age grid"
 
 
 def test_reverse_reconstruct(
     gplately_merdith_raster,
     gplately_merdith_static_geometries,
 ):
     continents = gplately_merdith_static_geometries[1]
```

### Comparing `gplately-0.3.3/test/test_5_seafloorgrid.py` & `gplately-0.4/test/test_5_seafloorgrid.py`

 * *Files identical despite different names*

### Comparing `gplately-0.3.3/test/test_6_geometry.py` & `gplately-0.4/test/test_6_geometry.py`

 * *Files identical despite different names*

