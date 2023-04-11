# Comparing `tmp/aicsimageio-4.9.3.tar.gz` & `tmp/aicsimageio-4.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicsimageio-4.9.3.tar", last modified: Tue Nov 15 21:46:41 2022, max compression
+gzip compressed data, was "aicsimageio-4.9.4.tar", last modified: Tue Dec  6 22:36:28 2022, max compression
```

## Comparing `aicsimageio-4.9.3.tar` & `aicsimageio-4.9.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.368457 aicsimageio-4.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    15045 2022-11-15 21:46:41.368457 aicsimageio-4.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13868 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.352457 aicsimageio-4.9.3/aicsimageio/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    37542 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/aics_image.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5088 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    25763 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/formats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/image_container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.356457 aicsimageio-4.9.3/aicsimageio/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.348457 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.360457 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/
--rw-r--r--   0 runner    (1001) docker     (121)     5053 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Channels.xsl
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/CommonTypes.xsl
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Constants.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/DocumentUser.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Image.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/ImagingEnvironment.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     9151 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Instrument.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/ObjectiveSettings.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     9753 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Pixels.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     3793 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Plane.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     2811 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Plate.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/StructuredAnnotations.xsl
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-11-15 21:46:36.000000 aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/czi-to-ome.xsl
--rw-r--r--   0 runner    (1001) docker     (121)    25251 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/metadata/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.364457 aicsimageio-4.9.3/aicsimageio/readers/
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18299 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/array_like_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    10237 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/bfio_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    22767 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/bioformats_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    35110 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/czi_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    20707 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/default_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/dv_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    25858 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/lif_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/nd2_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    12749 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/ome_tiff_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    29727 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    23837 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/tiff_glob_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    20635 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/readers/tiff_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    14907 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.364457 aicsimageio-4.9.3/aicsimageio/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/utils/io_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.364457 aicsimageio-4.9.3/aicsimageio/writers/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30211 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/writers/ome_tiff_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7534 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/writers/timeseries_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4758 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/writers/two_d_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/aicsimageio/writers/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.356457 aicsimageio-4.9.3/aicsimageio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15045 2022-11-15 21:46:41.000000 aicsimageio-4.9.3/aicsimageio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2163 2022-11-15 21:46:41.000000 aicsimageio-4.9.3/aicsimageio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 21:46:41.000000 aicsimageio-4.9.3/aicsimageio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 21:46:41.000000 aicsimageio-4.9.3/aicsimageio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-11-15 21:46:41.000000 aicsimageio-4.9.3/aicsimageio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-15 21:46:41.000000 aicsimageio-4.9.3/aicsimageio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:46:41.368457 aicsimageio-4.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    23768 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/docs/INSTALLATION.rst
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (121)     5566 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/docs/developer_resources.rst
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-11-15 21:46:41.368457 aicsimageio-4.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-11-15 21:46:35.000000 aicsimageio-4.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.954802 aicsimageio-4.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2022-12-06 22:36:28.954802 aicsimageio-4.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.950802 aicsimageio-4.9.4/aicsimageio/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37542 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/aics_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25763 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/image_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.950802 aicsimageio-4.9.4/aicsimageio/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.946802 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.950802 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Channels.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/CommonTypes.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Constants.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/DocumentUser.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Image.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/ImagingEnvironment.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Instrument.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/ObjectiveSettings.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Pixels.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Plane.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Plate.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/StructuredAnnotations.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2022-12-06 22:36:24.000000 aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/czi-to-ome.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)    25251 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/metadata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.954802 aicsimageio-4.9.4/aicsimageio/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18299 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/array_like_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/bfio_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/bioformats_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35110 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/czi_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20707 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/default_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/dv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25858 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/lif_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/nd2_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/ome_tiff_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29727 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24330 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/tiff_glob_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20635 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/readers/tiff_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.954802 aicsimageio-4.9.4/aicsimageio/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/utils/io_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.954802 aicsimageio-4.9.4/aicsimageio/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30211 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/writers/ome_tiff_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/writers/timeseries_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/writers/two_d_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/aicsimageio/writers/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.950802 aicsimageio-4.9.4/aicsimageio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2022-12-06 22:36:28.000000 aicsimageio-4.9.4/aicsimageio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2022-12-06 22:36:28.000000 aicsimageio-4.9.4/aicsimageio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 22:36:28.000000 aicsimageio-4.9.4/aicsimageio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 22:36:28.000000 aicsimageio-4.9.4/aicsimageio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2022-12-06 22:36:28.000000 aicsimageio-4.9.4/aicsimageio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-06 22:36:28.000000 aicsimageio-4.9.4/aicsimageio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 22:36:28.954802 aicsimageio-4.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    23768 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/docs/INSTALLATION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5566 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/docs/developer_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-06 22:36:28.954802 aicsimageio-4.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2022-12-06 22:36:23.000000 aicsimageio-4.9.4/setup.py
```

### Comparing `aicsimageio-4.9.3/LICENSE` & `aicsimageio-4.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/PKG-INFO` & `aicsimageio-4.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicsimageio
-Version: 4.9.3
+Version: 4.9.4
 Summary: Image Reading, Metadata Conversion, and Image Writing for Microscopy Images in Pure Python
 Home-page: https://github.com/AllenCellModeling/aicsimageio
 Author: Eva Maxfield Brown, Allen Institute for Cell Science
 Author-email: evamaxfieldbrown@gmail.com, jamie.sherman@gmail.com, bowdenm@spu.edu
 License: BSD-3-Clause
 Keywords: imageio,image reading,image writing,metadata,microscopy,allen cell
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aicsimageio-4.9.3/README.md` & `aicsimageio-4.9.4/README.md`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/__init__.py` & `aicsimageio-4.9.4/aicsimageio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 from .aics_image import imread_xarray  # noqa: F401
 from .aics_image import imread_xarray_dask  # noqa: F401
 
 __author__ = "Eva Maxfield Brown, Allen Institute for Cell Science"
 __email__ = "evamaxfieldbrown@gmail.com, jamie.sherman@gmail.com, bowdenm@spu.edu"
 # Do not edit this string manually, always use bumpversion
 # Details in CONTRIBUTING.md
-__version__ = "4.9.3"
+__version__ = "4.9.4"
 
 
 def get_module_version() -> str:
     return __version__
```

### Comparing `aicsimageio-4.9.3/aicsimageio/aics_image.py` & `aicsimageio-4.9.4/aicsimageio/aics_image.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/dimensions.py` & `aicsimageio-4.9.4/aicsimageio/dimensions.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/exceptions.py` & `aicsimageio-4.9.4/aicsimageio/exceptions.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/formats.py` & `aicsimageio-4.9.4/aicsimageio/formats.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/image_container.py` & `aicsimageio-4.9.4/aicsimageio/image_container.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Channels.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Channels.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/CommonTypes.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/CommonTypes.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/DocumentUser.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/DocumentUser.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Image.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Image.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/ImagingEnvironment.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/ImagingEnvironment.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Instrument.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Instrument.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/ObjectiveSettings.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/ObjectiveSettings.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Pixels.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Pixels.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Plane.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Plane.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/Plate.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/Plate.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/StructuredAnnotations.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/StructuredAnnotations.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/czi-to-ome-xslt/xslt/czi-to-ome.xsl` & `aicsimageio-4.9.4/aicsimageio/metadata/czi-to-ome-xslt/xslt/czi-to-ome.xsl`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/metadata/utils.py` & `aicsimageio-4.9.4/aicsimageio/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/__init__.py` & `aicsimageio-4.9.4/aicsimageio/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/array_like_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/array_like_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/bfio_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/bfio_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/bioformats_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/bioformats_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/czi_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/czi_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/default_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/default_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/dv_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/dv_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/lif_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/lif_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/nd2_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/nd2_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/ome_tiff_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/ome_tiff_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/tiff_glob_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/tiff_glob_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import glob
 import re
 from collections import OrderedDict
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import dask.array as da
 import numpy as np
 import pandas as pd
 import xarray as xr
 from fsspec.spec import AbstractFileSystem
 from tifffile import TiffFile, TiffFileError, TiffSequence, imread
@@ -33,16 +33,16 @@
 class TiffGlobReader(Reader):
     r"""
     Wraps the tifffile imread API to provide the same aicsimageio Reader API but for
     multifile tiff datasets (and other tifffile supported) images.
 
     Parameters
     ----------
-    glob_in: Union[PathLike, List[PathLike]]
-        Glob string that identifies all files to be loaded or a list
+    glob_in: Union[PathLike, Iterable[PathLike]]
+        Glob string that identifies all files to be loaded or an iterable
         of paths to the files as returned by glob.
     indexer: Union[Callable, pandas.DataFrame]
         If callable, should consume each filename and return a pd.Series with series
         index corresponding to the dimensions and values corresponding to the array
         index of that image file within the larger array.
         Default: None (Look for 4 numbers in the file name and use them as
         S, T, C, and Z indices.)
@@ -121,15 +121,15 @@
                     return True
 
         except (TiffFileError, TypeError):
             return False
 
     def __init__(
         self,
-        glob_in: Union[types.PathLike, List[types.PathLike]],
+        glob_in: Union[types.PathLike, Iterable[types.PathLike]],
         indexer: Union[pd.DataFrame, Callable] = None,
         scene_glob_character: str = "S",
         chunk_dims: Union[str, List[str]] = DEFAULT_CHUNK_DIMS,
         dim_order: Optional[Union[List[str], str]] = None,
         channel_names: Optional[Union[List[str], List[List[str]]]] = None,
         single_file_shape: Optional[Tuple] = None,
         single_file_dims: Sequence[str] = (
@@ -139,18 +139,23 @@
         fs_kwargs: Dict[str, Any] = {},
         **kwargs: Any,
     ):
 
         # Assemble glob list if given a string
         if isinstance(glob_in, str):
             file_series = pd.Series(glob.glob(glob_in))
-        elif isinstance(glob_in, list):
-            file_series = pd.Series(glob_in)
         elif isinstance(glob_in, Path) and "*" in str(glob_in):
             file_series = pd.Series(glob.glob(str(glob_in)))
+        elif isinstance(glob_in, pd.Series):
+            # Ensure all of our indices line up
+            file_series = glob_in.reset_index(drop=True, inplace=False)
+        elif isinstance(glob_in, Iterable):
+            file_series = pd.Series(glob_in)
+        else:
+            raise TypeError(f"Invalid type glob_in - got type {type(glob_in)}")
 
         if len(file_series) == 0:
             raise ValueError("No files found matching glob pattern")
 
         self.scene_glob_character = scene_glob_character
 
         if indexer is None:
@@ -170,15 +175,18 @@
                     re.findall(r"\d+", Path(x).name), index=series_idx
                 ).astype(int)
 
         if callable(indexer):
             self._all_files = file_series.apply(indexer)
             self._all_files["filename"] = file_series
         elif isinstance(indexer, pd.DataFrame):
-            self._all_files = indexer
+            # make a copy of the indexing dataframe and reset it index
+            # to ensure that we don't generate nans when aligning with
+            # file_series.
+            self._all_files = indexer.reset_index(drop=True, inplace=False)
             self._all_files["filename"] = file_series
 
         # If a dim doesn't exist on the file set the column value for that dim to zero.
         # If the dim is present, add it to the sort order. Because we are using
         # the default dimension ordering, this will naturally create a sort order
         # based off the standard dimension order.
         sort_order = []
```

### Comparing `aicsimageio-4.9.3/aicsimageio/readers/tiff_reader.py` & `aicsimageio-4.9.4/aicsimageio/readers/tiff_reader.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/transforms.py` & `aicsimageio-4.9.4/aicsimageio/transforms.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/types.py` & `aicsimageio-4.9.4/aicsimageio/types.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/utils/io_utils.py` & `aicsimageio-4.9.4/aicsimageio/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/writers/ome_tiff_writer.py` & `aicsimageio-4.9.4/aicsimageio/writers/ome_tiff_writer.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/writers/timeseries_writer.py` & `aicsimageio-4.9.4/aicsimageio/writers/timeseries_writer.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/writers/two_d_writer.py` & `aicsimageio-4.9.4/aicsimageio/writers/two_d_writer.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio/writers/writer.py` & `aicsimageio-4.9.4/aicsimageio/writers/writer.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio.egg-info/PKG-INFO` & `aicsimageio-4.9.4/aicsimageio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicsimageio
-Version: 4.9.3
+Version: 4.9.4
 Summary: Image Reading, Metadata Conversion, and Image Writing for Microscopy Images in Pure Python
 Home-page: https://github.com/AllenCellModeling/aicsimageio
 Author: Eva Maxfield Brown, Allen Institute for Cell Science
 Author-email: evamaxfieldbrown@gmail.com, jamie.sherman@gmail.com, bowdenm@spu.edu
 License: BSD-3-Clause
 Keywords: imageio,image reading,image writing,metadata,microscopy,allen cell
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aicsimageio-4.9.3/aicsimageio.egg-info/SOURCES.txt` & `aicsimageio-4.9.4/aicsimageio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/aicsimageio.egg-info/requires.txt` & `aicsimageio-4.9.4/aicsimageio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/docs/CHANGELOG.rst` & `aicsimageio-4.9.4/docs/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/docs/INSTALLATION.rst` & `aicsimageio-4.9.4/docs/INSTALLATION.rst`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/docs/Makefile` & `aicsimageio-4.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/docs/conf.py` & `aicsimageio-4.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/docs/developer_resources.rst` & `aicsimageio-4.9.4/docs/developer_resources.rst`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/docs/index.rst` & `aicsimageio-4.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/docs/make.bat` & `aicsimageio-4.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aicsimageio-4.9.3/setup.cfg` & `aicsimageio-4.9.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.9.3
+current_version = 4.9.4
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
 serialize = {major}.{minor}.{patch}
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
```

### Comparing `aicsimageio-4.9.3/setup.py` & `aicsimageio-4.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,10 +164,10 @@
     setup_requires=setup_requirements,
     test_suite="aicsimageio/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/AllenCellModeling/aicsimageio",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.md
-    version="4.9.3",
+    version="4.9.4",
     zip_safe=False,
 )
```

