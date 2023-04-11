# Comparing `tmp/pydar-0.1.0.tar.gz` & `tmp/pydar-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydar-0.1.0.tar", last modified: Fri Jan 20 02:04:14 2023, max compression
+gzip compressed data, was "dist/pydar-1.0.0.tar", last modified: Tue Apr 11 21:00:05 2023, max compression
```

## Comparing `pydar-0.1.0.tar` & `pydar-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 02:04:14.091428 pydar-0.1.0/
--rw-rw-r--   0 user      (1000) user      (1000)       25 2023-01-04 06:11:53.000000 pydar-0.1.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    37242 2023-01-20 02:04:14.091428 pydar-0.1.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32029 2023-01-19 03:23:33.000000 pydar-0.1.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 02:04:14.079428 pydar-0.1.0/pydar/
--rw-rw-r--   0 user      (1000) user      (1000)     2180 2023-01-19 02:30:53.000000 pydar-0.1.0/pydar/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 02:04:14.087428 pydar-0.1.0/pydar/data/
--rw-rw-r--   0 user      (1000) user      (1000)     1218 2023-01-01 06:47:05.000000 pydar-0.1.0/pydar/data/cassini_flyby.csv
--rw-rw-r--   0 user      (1000) user      (1000)    15662 2023-01-12 07:14:56.000000 pydar-0.1.0/pydar/data/coradr_jpl_options.csv
--rw-rw-r--   0 user      (1000) user      (1000)    30062 2023-01-15 06:54:19.000000 pydar-0.1.0/pydar/data/feature_name_details.csv
--rw-rw-r--   0 user      (1000) user      (1000)    36144 2023-01-13 02:14:43.000000 pydar-0.1.0/pydar/data/sar_swath_details.csv
--rw-rw-r--   0 user      (1000) user      (1000)   545452 2023-01-14 03:19:28.000000 pydar-0.1.0/pydar/data/swath_coverage_by_time_position.csv
--rw-rw-r--   0 user      (1000) user      (1000)      940 2023-01-10 09:12:40.000000 pydar-0.1.0/pydar/display_image.py
--rw-rw-r--   0 user      (1000) user      (1000)    11518 2023-01-19 03:13:13.000000 pydar-0.1.0/pydar/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)    13730 2023-01-14 06:38:52.000000 pydar-0.1.0/pydar/extract_flyby_parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)       41 2023-01-01 03:29:13.000000 pydar-0.1.0/pydar/pydar_testing.py
--rw-rw-r--   0 user      (1000) user      (1000)    11607 2023-01-13 21:46:51.000000 pydar-0.1.0/pydar/read_readme.py
--rw-rw-r--   0 user      (1000) user      (1000)     7715 2023-01-19 03:18:04.000000 pydar-0.1.0/pydar/retrieve_ids_by_time_position.py
--rw-rw-r--   0 user      (1000) user      (1000)     3588 2023-01-13 03:26:53.000000 pydar-0.1.0/pydar/retrieve_supplementary_backplanes.py
--rw-rw-r--   0 user      (1000) user      (1000)    10229 2023-01-15 08:59:10.000000 pydar-0.1.0/pydar/update_csv.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-01-20 02:04:14.083428 pydar-0.1.0/pydar.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    37242 2023-01-20 02:04:14.000000 pydar-0.1.0/pydar.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      598 2023-01-20 02:04:14.000000 pydar-0.1.0/pydar.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-20 02:04:14.000000 pydar-0.1.0/pydar.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       90 2023-01-20 02:04:14.000000 pydar-0.1.0/pydar.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2023-01-20 02:04:14.000000 pydar-0.1.0/pydar.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-01-20 02:04:14.091428 pydar-0.1.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1471 2023-01-20 02:02:40.000000 pydar-0.1.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.238731 pydar-1.0.0/
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2023-01-04 06:11:53.000000 pydar-1.0.0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)    49553 2023-04-11 21:00:05.238731 pydar-1.0.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    42653 2023-04-11 20:30:20.000000 pydar-1.0.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.222731 pydar-1.0.0/pydar/
+-rw-rw-r--   0 user      (1000) user      (1000)     2345 2023-03-25 01:17:08.000000 pydar-1.0.0/pydar/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.226731 pydar-1.0.0/pydar/data/
+-rw-rw-r--   0 user      (1000) user      (1000)     1218 2023-01-01 06:47:05.000000 pydar-1.0.0/pydar/data/cassini_flyby.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    15662 2023-02-19 01:03:57.000000 pydar-1.0.0/pydar/data/coradr_jpl_options.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    30062 2023-02-19 01:20:45.000000 pydar-1.0.0/pydar/data/feature_name_details.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    36144 2023-01-13 02:14:43.000000 pydar-1.0.0/pydar/data/sar_swath_details.csv
+-rw-rw-r--   0 user      (1000) user      (1000)   545452 2023-02-19 01:17:22.000000 pydar-1.0.0/pydar/data/swath_coverage_by_time_position.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     1774 2023-03-29 19:49:01.000000 pydar-1.0.0/pydar/display_image.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19293 2023-03-29 05:23:48.000000 pydar-1.0.0/pydar/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15941 2023-04-11 20:17:28.000000 pydar-1.0.0/pydar/extract_flyby_parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)      259 2023-03-29 22:21:31.000000 pydar-1.0.0/pydar/pydar_testing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.238731 pydar-1.0.0/pydar/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     1425 2023-04-11 20:25:57.000000 pydar-1.0.0/pydar/pytests/test_extract_flyby_parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12401 2023-03-25 01:33:08.000000 pydar-1.0.0/pydar/read_readme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14316 2023-03-21 20:58:40.000000 pydar-1.0.0/pydar/retrieve_ids_by_time_position.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4081 2023-03-18 07:53:32.000000 pydar-1.0.0/pydar/retrieve_supplementary_backplanes.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12251 2023-02-25 05:04:59.000000 pydar-1.0.0/pydar/sbdr_make_shapefile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      969 2023-02-18 06:42:56.000000 pydar-1.0.0/pydar/test_bearing_correction.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3021 2023-03-21 20:49:44.000000 pydar-1.0.0/pydar/updateCsvCORADARJPLOptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4075 2023-03-21 20:49:20.000000 pydar-1.0.0/pydar/updateCsvFeatureNameDetails.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5609 2023-03-21 20:48:33.000000 pydar-1.0.0/pydar/updateCsvSwathCoverage.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-11 21:00:05.222731 pydar-1.0.0/pydar.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    49553 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      792 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      132 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-04-11 21:00:05.000000 pydar-1.0.0/pydar.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-11 21:00:05.238731 pydar-1.0.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1669 2023-03-29 20:59:27.000000 pydar-1.0.0/setup.py
```

### Comparing `pydar-0.1.0/PKG-INFO` & `pydar-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,98 @@
 Metadata-Version: 2.1
 Name: pydar
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Python package to access, download, view, and manipulate Cassini RADAR images
 Home-page: https://github.com/unaschneck/pydar
-Author: Una Schneck (unaschneck), C. Y. Schneck (cyschneck)
+Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.0.0.tar.gz
 Description: # PYDAR
+         <p align="center">
+          <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
+        </p>
+        
         ![PyPi](https://img.shields.io/pypi/v/pydar)
-        ![license](https://img.shields.io/github/license/unaschneck/pydar)
+        ![license](https://img.shields.io/pypi/l/pydar)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
+        ![PyPi-Versions](https://img.shields.io/pypi/pyversions/pydar)
+        [![update-dynamic-csv-data-files](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml)
+        [![pytests](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml)
+        
+        A Python package to access, download, view, and manipulate Cassini RADAR images in one place
+        
+        * **Find relevant flyby observation numbers/IDs for a feature, range of latitude/longitudes (or specific latitude/longitude), or a time range (or specific time)**
+        	* retrieveIDSByFeatureName()
+        	* retrieveIDSByLatitudeLongitude()
+        	* retrieveIDSByLatitudeLongitudeRange()
+        	* retrieveFeaturesFromLatitudeLongitude()
+        	* retrieveFeaturesFromLatitudeLongitudeRange()
+        	* retrieveIDSByTime()
+        	* retrieveIDSByTimeRange()
+        * **Use flyby observation numbers/IDs to retrieve flyby observation data (.FMT, .TAB, .LBL, .IMG) from SBDR and BIDR data files by default**
+        	* convertFlybyIDToObservationNumber()
+        	* convertObservationNumberToFlybyID()
+        	* extractFlybyDataImages()
+        * **Access specific observation data from AAREADME and .LBL readme information**
+        	* returnAAREADMEOptions()
+        	* readAAREADME()
+        	* returnLBLOptions()
+        	* readLBLREADME()
+        * **Display PDS image retrieved for flyby observation**
+        	* displayImages()
         
-        Python Package to access and manipulate CASSINI RADAR images in one place
+        NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.  
         
-        * Find relevant flyby observation numbers and IDs for a specific region, feature, or location
-        * Retrieve flyby observation data (.FMT, .TAB, .LBL, .IMG) from SBDR and BIDR by default
-        * Access AAREADME and .LBL readme information
-        * Display PDS image retrieved for flyby observation
+        ## Install
+        PyPi pip install at [pypi.org/project/pydar/](https://pypi.org/project/pydar/)
         
-        NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.  
+        ```
+        pip install pydar
+        ```
         
-        ## Overview
-        For information on instrument specifics and acronyms refer to the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+        ## Dependencies
+        Python 3.7+
         
-        The Cassini Radar data can be found at the [PDS Imaging Node](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/). The directory is organized by [PDS standards](https://pdssbn.astro.umd.edu/howto/understand.shtml). The file format are defined in the [Small Body Node](https://pdssbn.astro.umd.edu/howto/file_types.shtml). The radar echo is stored originally as floating points in LBDR files. The SAR processors turns the LBDR files to BIDR image. The BIDR data is organized as follows:
+        Verified compatibility with Python 3.7, 3.8, and 3.9
+        ```
+        pip install -r requirements.txt
+        ```
+        Requirements will also be downloaded as part of the pip download
+        
+        ## Quickstart: PYDAR
+        
+        All Cassini data for Titan is retrieved based on flyby observation numbers or IDs, so relevant flybys can be found based on time range, latitude/longitude position, or a known feature name
+        
+        ```python
+        import pydar
+        feature_name_example = "ontario lacus"
+        flyby_ids = pydar.retrieveIDSByFeatureName(feature_name=feature_name_example)
+        ```
+        Returns a dictionary of flyby IDs (and their relevant segments) that Ontario Lacus could be found from: `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
+        
+        The relevant data files can be downloaded for any combination of these flyby IDs and segment numbers. For example, flyby ID 'T65' and segment 'S01' at resolution 'D' for 8 pixels/degree
+        ```
+        # Extract Flyby Data Files to pydar_results/ directory
+        pydar.extractFlybyDataImages(flyby_id='T65',
+        				resolution='D',
+        				segment_num="S01")
+        ```
+        Note: extractFlybyDataImages() only needs to be run once for each flyby to retrieve new data but will take some time to download
+        ```
+        # Display all Images in pydar_results/ directory
+        pydar.displayImages(image_directory="pydar_results/CORADR_0211_V03_S01")
+        ```
+         <p align="center">
+          <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
+        </p>
+        
+        ## Overview and Background
+        For information on Cassini instrument specifics and acronyms refer to the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+        
+        The Cassini Radar data can be found at the [PDS Imaging Node](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/). The directory is organized by [PDS standards](https://pdssbn.astro.umd.edu/howto/understand.shtml). The file format are defined in the [Small Body Node](https://pdssbn.astro.umd.edu/howto/file_types.shtml). The radar echo is stored originally as floating points in LBDR files. The SAR processors turn the LBDR files into BIDR image. The BIDR data is organized as follows:
         ```
         Cassini RADAR Information (CORADR_xxxx_Vxx) where xxxx is the radar data take number and Vxx is the data version number
           |_ AAREADME.txt
             Information about observation xxxx (xxxx > 0035 for Titan flybys)
           |_CALIB/
           |_CATALOG/
             BIDRDS.CAT: Information about the BIDR dataset
@@ -99,449 +164,578 @@
           |_ERRATA.txt
           |_EXTRAS/
             |_BIbcdeefggg_Dhhh_Tiii_Vnn.JPG: jpg of IMG files in DATA 
           |_INDEX/
           |_SOFTWARE/
           |_VOLDESC.CAT <--- VERSION INFORMATION LISTED HERE ('VOLUME_VERSION_ID' = "Version 1", "Version 2", "Version 3") and in filename
         ```
+        .IMG files can be viewed using the [planetary images library](https://planetaryimage.readthedocs.io/_/downloads/en/latest/pdf/) or via `pydar.displayImages()`
         
-        .IMG files can be viewed using the [planetary images library](https://planetaryimage.readthedocs.io/_/downloads/en/latest/pdf/)
         ### Download Time
-        Download time varies depending on the number and size of files of interest. On average, most single feature downloads take between 2-5 minutes to download.
+        Download time for data files vary when using `pydar.extractFlybyDataImages()` and depends on the number and size of files of interest. On average, most single feature downloads take between 5-30 minutes to download, but can be longer for higher resolution files.
         
         ![image](https://user-images.githubusercontent.com/24469269/211881026-5bab329c-cf0d-416b-bedc-6d466b77b1f5.png)
         ([Cassini Radar Volume SIS, Version 2.1](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0284/DOCUMENT/VOLSIS.PDF) Table 1, pg. 3)
-        ### Cross-Reference Table for Observations and Flybys
-        The Titan flybys ID is not used in the naming convention for the CORADR filenames. The Titan flyby information is contained in the BIDR filenames and in the VOLDESC.CAT under 'Description' and can be found using the following cross-reference table: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
         
-        ```
-        Flyby ID Cross Reference Table
-        Prime Mission and Extended Mission
-        
-        Column 1: Titan flyby id
-        Column 2: Radar Data Take Number
-        Column 3: Sequence number
-        Column 4: Orbit Number/ID
-        
-        Ta   DTN 035   S05 Rev 0A
-        T3   DTN 045   S08 Rev 03
-        T4   DTN 048   S09 Rev 04
-        T7   DTN 059   S14 Rev 14
-        T8   DTN 065   S15 Rev 17
-        
-        ...
-        ```
+        ### Cross-Reference Table for Observations and Flybys
+        The Titan flyby IDs (e.g. 'T65') are not used in the naming convention for the CORADR filenames. Instead, all files are referred to by their observation number (e.g. '0211'). The Titan flyby information is contained in the BIDR filenames and in the VOLDESC.CAT under 'Description' and can be found using the following cross-reference table: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
         
-        To convert between a Titan Flyby ID and an observation number: `pydar.convertFlybyIDToObservationNumber(flyby_id)`
+        To convert between a Titan Flyby ID and an observation number use either `pydar.convertFlybyIDToObservationNumber(flyby_id)` or `pydar.convertObservationNumberToFlybyID(flyby_observation_num)`
         
         ### Observation Information as filename
-        The data filename contains a lot of information about the observation 
+        The data filename contains a lot of information about the observation
         
         (EXAMPLE) Filename: "BIBQD05S184_D065_T008S03_V03"
         
         - BI = BIDR data
         - B = data in dB normalized
-        - Q = obliquid dylindrical
+        - Q = oblique cylindrical
         - D = 8 pixels/degree
         - 05 = absolute value of latitude at center rounded to nearest degree
         - S = hemisphere of center of file (Southern)
         - 184 = West longitude at center of file rounded to nearest degree
         - D065 = 2-digit data take ID aka observation counter with left-padded zeros
         - T008 = 3-digit Titan flyby with left-padding
         - S03 = 2-digit segment number (00-99)
         - V03 = 2-digit version number (01-99)
         
-        BIBQD05S184_D065_T008S03_V03.JPG:
+        Image file from BIBQD05S184_D065_T008S03_V03.JPG:
         
         ![BIFQI10S251_D065_T008S01_V03](https://user-images.githubusercontent.com/24469269/210164143-427003ed-0043-45b4-a80f-8e9ddf28543a.jpg)
         
         ### Volume Version of Data
         
-        Some passes have multiple versions of the data.
-        
-        * Version 1 (V01) was the first archived version of the data and assumed Titan had zero obliquity, which resulted in misregistration between passes
-        
-        * Version 2 (V02) used a Titan spin model that reduced misregistration error 
+        Some passes have multiple versions of the data, up to 3 different versions currently.
         
-        * Version 3 (V03) used a long-term, accurate spin model for Titan along with other improvements
+        * **Version 1 (V01)** was the first archived version of the data and assumed Titan had zero obliquity, which resulted in misregistration between passes
+        * **Version 2 (V02)** used a Titan spin model that reduced misregistration error 
+        * **Version 3 (V03)** used a long-term, accurate spin model for Titan along with other improvements
         
         Only some Titan passes produced all of the version numbers.
         
         * TA-T25 : V01, V02, V03
         
         * $\gt$ T28: V02, V03
         
         * T108-T126: labeled only once as V02 but is actually V03
         
-        The version number is listed in the filenanme and in VOLDESC.CAT under the 'VOLUME_VERSION_ID'
+        The version number is listed in the filename and in VOLDESC.CAT under the 'VOLUME_VERSION_ID'
         
-        *Version 3 is the latest and preferred version*
+        _**Version 3 is currently the latest and preferred version and will be the version included when downloaded**_
         
         Example:
         
         Version 1 is named BIFQI48N071_D035_T00A_V01.IMG
         
         Version 2 is named BIFQI49N071_D035_T00AS01_V02.IMG
         
         Version 3 is named BIFQI49N071_D035_T00AS01_V03.IMG
         
         ### Segment Number of Data
         A single flyby can produce multiple image segments (Sxx). *S01 is the primary imaging segment* with other segments referring to periods in the flyby when the instrument went to/from altimetry/SAR/HiSAR or weird pointing profiles.  
         
         ![image](https://user-images.githubusercontent.com/24469269/210197286-c059ffed-281d-46c7-911a-f86c3bf7ea28.png)
-        Credit: Cassini Radar User Guide (Wall et al. 2019, pg.16)
-        ## Documentation
+        *Credit: Cassini Radar User Guide (Wall et al. 2019, pg.16)*
+        
+        ## Backend Data Files
+        
+        ### Dynamically Updated Backend Files
+        
+        Pydar includes multiple scripts to web scrape from relevant URLs to generate some of the backend data files
+        
+        Changes in the relevant URLs are checked once a month via Github Actions to keep csv files up to date and any changes found will be bundled into the subsequent release
+        
+        **coradr_jpl_options.csv**
+        
+        Contains all the CORADR IDs and available data types from [pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter)
+        
+        Headers: ["CORADR ID", "Is a Titan Flyby", "Contains ABDR", "Contains ASUM", "Contains BIDR", "Contains LBDR", "Contains SBDR", "Contains STDR"]
         
-        ## Data Files
+        View data file: [coradr_jpl_options.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/coradr_jpl_options.csv)
+        
+        **swath_coverage_by_time_position.csv**
+        
+        Contains all the information for .LBL files within all CORADR ID pages (for each segment and resolution file)
+        
+        Collected from URLs matching: pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/[CORADAR_ID]/DATA/BIDR/
+        
+        Headers: ["CORADR ID", "FLYBY ID", "SEGMENT NUMBER", "FILENAME", "DATE TYPE SYMBOL", "DATE TYPE", "RESOLUTION (pixels/degrees)", "TARGET_NAME", "MAXIMUM_LATITUDE (Degrees)", "MINIMUM_LATITUDE (Degrees)", "EASTERNMOST_LONGITUDE (Degrees)", "WESTERNMOST_LONGITUDE (Degrees)", "START_TIME", "STOP_TIME"]
+        
+        View data file: [swath_coverage_by_time_position.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/swath_coverage_by_time_position.csv)
         
         **feature_name_details.csv**
         
-        List of Features on Titan with names with their associated position and the origin of their name. Taken from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/Feature/6981)
+        Contains all named features on Titan with their furthest latitude/longitude position and origin of name
         
-        ## SBDR Files
-        [SBDR column descriptions](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0045/DOCUMENT/BODPSIS.PDF)
+        Collected from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
         
-        Total width of the RADAR swath is created by combining the five individual sub-swaths, where the center beam is the highest gain
-        ![image](https://user-images.githubusercontent.com/24469269/211431884-c201ac74-114a-4c17-b95a-f9edf0178d2e.png)
-        (_The Cassini Huygens Mission: Orbiter Remote Sensing Observation 2004_)
+        Headers: ["Feature Name", "Northernmost Latitude", "Southernmost Latitude", "Easternmost Longitude", "Westernmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
         
-        ```
-        test_file = "SBDR_15_D065_V03.TAB"
-        SBDR_FILE = pdr.read(test_file)
-        print("Table options: {0}".format(SBDR_FILE.keys()))
-        ```
+        View data file: [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
+        
+        ### Static Data Files
+        
+        **cassini_flyby.csv**
+        
+        Reference for converting between a Titan Flyby ID (e.g. "T7") and its Observation Number (e.g. "059") (and back)
+        
+        Headers: ["Titan flyby id", "Radar Data Take Number", "Sequence number", "Orbit Number/ID"]
+        
+        View data file: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
+        
+        **sar_swath_details.csv**
+        
+        Currently unused, but will potentially be used in the future for incidence angle, polarization, azimuth, SAR range resolution, SAR azimuth resolution, and number of looks
+        
+        Converted to a static csv file from the Cassini User Guide (pg. 136-139)
+        
+        View data file: [sar_swath_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/sar_swath_details.csv)
         
         ## BIDR and SBDR Files
         Note: "CORADR_0048", "CORADR_0186", "CORADR_0189", "CORADR_0209", "CORADR_0234" do not have associated BIDR values.
         
         There are data gaps and problems from the original downlinking and satellite location
         
-        CORADR_0048 (T4) did not have SAR data, only scatterometry and radiometery because of telemetry reasons in the handbook
+        CORADR_0048 (T4) did not have SAR data, only scatterometry and radiometry because of telemetry reasons in the handbook
         
-        CORADR_0186 (T52) only have rad and compressed scatterometry
+        CORADR_0186 (T52) only have radiometry and compressed scatterometry
         
-        CORADR_189 (T53) only has rad and compressed scatterometry because of what appears to be a downlink problem
+        CORADR_0189 (T53) only has radiometry and compressed scatterometry because of what appears to be a downlink problem
         
         CORADR_0209 (T63) only has scatterometry and radiometry
         
         CORADR_0234 (T80) only has scatterometry and radiometry 
-        ## Dependencies
-        Python 3.9
-        ```
-        pip3 install -r requirements.txt
-        ```
-        ## Install
-        PyPi pip install at [pypi.org/project/pydar/](https://pypi.org/project/pydar/)
         
-        ```
-        pip install pydar
-        ```
+        ## Coming Soon: SBDR Files
+        Total width of the RADAR swath is created by combining the five individual sub-swaths, where the center beam is the highest gain
+        ![image](https://user-images.githubusercontent.com/24469269/211431884-c201ac74-114a-4c17-b95a-f9edf0178d2e.png)
+        (_The Cassini Huygens Mission: Orbiter Remote Sensing Observation 2004_)
+        
+        [SBDR column descriptions](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0045/DOCUMENT/BODPSIS.PDF)
         
-        ## Examples
+        ## Retrieve Data from CASSINI Function Calls
         
-        To collect flyby information and images from a feature on Titan, start by selecting a feature, for example: "Ontario Lacus"
+        To collect flyby information and images for the latitude/longitude range of a named feature on Titan
         
-        **retrieveIDSByFeatureName**
+        ### retrieveIDSByFeatureName()
         
-        Retrieve a list of flyby IDs with their associated segments based on a feature name from titan
+        Retrieve a list of flyby IDs with their associated segment numbers based on a feature name from Titan
         
         ```python
         retrieveIDSByFeatureName(feature_name=None)
         ```
-        * **[REQUIRED]** feature_name (string): Feature name on Titan to give flyby ids and segments, not case-sensitive
+        * **[REQUIRED]** feature_name (string): Feature name on Titan, not case-sensitive
         
         Feature names are retrieved from [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
         <details closed>
         <summary>List of Valid Feature Names (Click to view all)</summary>
         <br>
         ['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
         </details>
         
         ```python
         import pydar
         pydar.retrieveIDSByFeatureName(feature_name="Ontario Lacus")
         ```
-        Output = `{'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
+        Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
         
-        **retrieveIDSByLatitudeLongitude**
+        ### retrieveIDSByLatitudeLongitude()
         
         Retrieve a list of flyby IDs with their associated segments based on specific latitude and longitude
         
         ```python
         retrieveIDSByLatitudeLongitude(latitude=None, longitude=None)
         ```
-        * **[REQUIRED]** latitude (float/int): Latitude (in degrees) where North = + and South = -
-        * **[REQUIRED]** longitude (float/int): Longitude (in degrees) where West = + and East = -
+        * **[REQUIRED]** latitude (float/int): Latitude (in degrees), range from -90° to 90°
+        * **[REQUIRED]** longitude (float/int): Longitude (in degrees), range from 0° to 360°
         
         ```python
         import pydar
-        pydar.retrieveIDSByLatitudeLongitude(latitude=10, longitude=10)
+        pydar.retrieveIDSByLatitudeLongitude(latitude=-80, longitude=170)
         ```
-        Output = `{'T19': ['S01'], 'T29': ['S01'], 'T55': ['S01'], 'T56': ['S01'], 'T57': ['S01'], 'T58': ['S01'], 'T64': ['S01'], 'T83': ['S02'], 'T84': ['S02'], 'T92': ['S01'], 'T98': ['S02'], 'T104': ['S01']}`
+        Output = `{'T39': ['S06', 'S05', 'S01'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S03'], 'T56': ['S01'], 'T57': ['S01'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
         
-        **retrieveIDSByLatitudeLongitudeRange**
+        ### retrieveIDSByLatitudeLongitudeRange()
+        
+        Retrieve a list of flyby IDs with their associated segments based on range of latitudes and longitudes
         
         ```python
-        retrieveIDSByLatitudeLongitudeRange(northernmost_latitude=None,
-        				southernmost_latitude=None,
-        				easternmost_longitude=None,
-        				westernmost_longitude=None)
+        retrieveIDSByLatitudeLongitudeRange(min_latitude=None,
+        				max_latitude=None,
+        				min_longitude=None,
+        				max_longitude=None)
         ```
-        * **[REQUIRED]** northernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, north must be greater than or equal to the south
-        * **[REQUIRED]** southernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, south must be less than or euqal to the north
-        * **[REQUIRED]** easternmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, west must be less than or equal to the east
-        * **[REQUIRED]** westernmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, east must be greater than or equal to the west
+        * **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be greater than or equal to the max_latitude, range from -90° to 90°
+        * **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be less than or equal to the min_latitude, range from -90° to 90°
+        * **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
+        * **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude be greater than or equal to the min_longitude, range from 0° to 360°
         
         ```python
-        retrieveIDSByLatitudeLongitudeRange(northernmost_latitude=15,
-        				southernmost_latitude=10,
-        				easternmost_longitude=12,
-        				westernmost_longitude=17)
+        import pydar
+        pydar.retrieveIDSByLatitudeLongitudeRange(min_latitude=-82,
+        					max_latitude=-72,
+        					min_longitude=183,
+        					max_longitude=185)
         ```
-        Output = `{'T19': ['S01'], 'T29': ['S01'], 'T55': ['S01'], 'T56': ['S01'], 'T57': ['S01'], 'T64': ['S01'], 'T83': ['S02'], 'T84': ['S02'], 'T92': ['S01'], 'T98': ['S02'], 'T104': ['S01']}`
+        Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
         
-        Ontario Lacus was visible in four swath observations: T57, T58, T65, T98 [(Page 163)](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf).
+        ### retrieveFeaturesFromLatitudeLongitude()
         
-        To access flyby of Ontario, first specify a flyby. For this example, Ontario Lacus with the features:
+        Return a list of features found at a specific latitude/longitude position
         
-        * Titan flyby id: 'T65'
-        * resolution: 'D' (8 pixels/degree)
-        * Main imaging segement 1: 'S01'
+        ```
+        retrieveFeaturesFromLatitudeLongitude(latitude=None, longitude=None)
+        ```
+        * **[REQUIRED]** latitude (float/int): Latitude (in degrees), range from -90° to 90°
+        * **[REQUIRED]** longitude (float/int): Longitude (in degrees), range from 0° to 360°
         
-        **extractFlybyDataImages()**
+        ```python
+        import pydar
+        pydar.retrieveFeaturesFromLatitudeLongitude(latitude=-72, longitude=183)
+        ```
+        
+        Output = `['Ontario Lacus', 'Rossak Planitia']`
         
-        Downloads flyby data SBDR: .FMT and .TAB files (for example: [SBDR.FMT](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR.FMT) and [SBDR_15_D087_V03.TAB](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR_15_D087_V03.TAB))
+        ### retrieveFeaturesFromLatitudeLongitudeRange()
         
-        Downloads flyby data BIDR: .LBL and .ZIP files (for example: [BIBQH80N051_D087_T016S01_V03.LBL](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.LBL) and [BIBQH80N051_D087_T016S01_V03.ZIP](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.ZIP))
+        Return a list of features found at a range of latitude/longitude positions
         
         ```
-        extractFlybyDataImages(flyby_observation_num=None,
-        			flyby_id=None,
-        			segment_num=None,
-        			additional_data_types_to_download=[],
-        			resolution='I',
-        			top_x_resolutions=None)
+        retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=None,
+        					max_latitude=None,
+        					min_longitude=None,
+        					max_longitude=None)
         ```
-        Either a flyby_id (for example: 'T65') or a flyby_observation_num (for example: '0065') is required. A flyby_id will be translated into a flyby_observation_number to access on the backend and the results will be saved under the observation number. 'T65' will become observation number '0021'
+        * **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be less than or equal to the max_latitude, range from -90° to 90°
+        * **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be greater than or equal to the min_latitude, range from -90° to 90°
+        * **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
+        * **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude must be greater than or equal to the min_longitude, range from 0° to 360°
         
-        * **[REQUIRED/OPTIONAL]** flyby_observation_num (string): required if flyby_id not included
-        * **[REQUIRED/OPTIONAL]** flyby_id (string): required if flyby_observation_num not included
-        * **[REQUIRED]** segment_num (string): 
-        * [OPTIONAL] additional_data_types_to_download (List of Strings): Possible options ["ABDR", "ASUM", "BIDR", "LBDR", "SBDR", "STDR"]
-        * [OPTIONAL] resolution (String): resolution options "B", "D", "F", "H", or "I" (2, 8, 32, 128, 256 pixels/degree), defaults to highest resolution 'I'
-        * [OPTIONAL] top_x_resolutions: Save the top x resolution types (5 total resolutions)
+        ```python
+        import pydar
+        
+        pydar.retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=-82,
+        						max_latitude=-72,
+        						min_longitude=183,
+        						max_longitude=190)
+        ```
+        Output = `['Crveno Lacus', 'Ontario Lacus', 'Romo Planitia', 'Rossak Planitia', 'Saraswati Flumen']`
+        
+        ### retrieveIDSByTime()
+        
+        Retrieve a dictionary of flyby IDs and segment numbers based on a specific timestamp
+        
+        ```
+        retrieveIDSByTime(year=None,
+        		doy=None,
+        		hour=None,
+        		minute=None,
+        		second=None,
+        		millisecond=None)
+        ```
+        * **[REQUIRED]** year (int): Year for observation, range from 2004 to 2014
+        * **[REQUIRED]** doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year)
+        * [OPTIONAL] hour (int): Hour, from 0 to 23 in UTC, defaults to 0 when undefined
+        * [OPTIONAL] minute (int): Minute, from 0 to 59, defaults to check the all minutes when undefined
+        * [OPTIONAL] second (int): Second, from 0 to 59, defaults to check the all seconds when undefined
+        * [OPTIONAL] millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined
+        
+        Where `2004 year, 300 doy, 15 hour, 30 minute, 7 second, 789 millisecond` becomes `2004-300T15:30:07.789`
+        
+        ```python
+        import pydar
+        pydar.retrieveIDSByTime(year=2004,
+        			doy=300,
+        			hour=15,
+        			minute=30, 
+        			second=7, 
+        			millisecond=789)
+        ```
+        Output = `{'Ta': ['S01']}`
+        
+        If hour, minute, second, or millisecond is left undefined, will search the entire range for all possible values and can find more possible ids
+        
+        For a single day, some flybys have segments that are defined in one large range, but not within a smaller range
         
+        ```python
+        import pydar
+        pydar.retrieveIDSByTime(year=2005, doy=301)
+        ```
+        Output for the entire day of 301 = `{'T8': ['S02', 'S03', 'S01']}`
         
         ```python
         import pydar
+        pydar.retrieveIDSByTime(year=2005, doy=301, hour=3)
+        ```
+        Output for the day 301 but just for hour 3 = `{'T8': ['S03', 'S01']}` (does not include S02)
+        
+        ### retrieveIDSByTimeRange()
         
-        # Extract Flyby Data Files to pydar_results/ directory: 
-        pydar.extractFlybyDataImages(flyby_id='T65', resolution='D', segment_num="S01", additional_data_types_to_download=["STDR", "LBDR"])
+        Retrieve a dictionary of flyby IDs and segment numbers based on a start and end datetime
+        
+        ```
+        retrieveIDSByTimeRange(start_year=None, 
+        			start_doy=None,
+        			start_hour=None,
+        			start_minute=None, 
+        			start_second=None,
+        			start_millisecond=None,
+        			end_year=None, 
+        			end_doy=None,
+        			end_hour=None,
+        			end_minute=None, 
+        			end_second=None,
+        			end_millisecond=None)
         ```
         
-        extractFlybyDataImages() will retrieve images from PDS website and saves results in a directory labeled 'pydar_results' with the flyby obsrevation number, version number, and segement number in the title (for example pydar_results/CORADR_0065_V03_S01)
+        * **[REQUIRED]** start_year (int): Year for observation, range from 2004 to 2014, start_year must be less than/equal to end_year
+        * **[REQUIRED]** end_year (int): Year for observation, range from 2004 to 2014, end_year must be greater than/equal to start_year
+        * **[REQUIRED]** start_doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year), start_doy must be less than/equal to end_doy
+        * **[REQUIRED]** end_doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year), end_doy must be less than/equal to start_doy
+        * [OPTIONAL] start_hour (int): Hour, from 0 to 23 in UTC, defaults to check all hours when undefined, start_hour must be less than/equal to end_hour
+        * [OPTIONAL] end_hour (int): Hour, from 0 to 23 in UTC, defaults to check all hours when undefined, end_hour must be less than/equal to start_hour
+        * [OPTIONAL] start_minute (int): Minute, from 0 to 59, defaults to check all minutes when undefined, start_minute must be less than/equal to end_minute
+        * [OPTIONAL] end_minute (int): Minute, from 0 to 59, defaults to check all minutes when undefined, end_minute must be greater than/equal to start_minute
+        * [OPTIONAL] start_second (int): Second, from 0 to 59, defaults to check all seconds when undefined, start_second must be less than/equal to end_second
+        * [OPTIONAL] end_second (int): Second, from 0 to 59, defaults to check all seconds when undefined, end_second must be greater than/equal to start_second
+        * [OPTIONAL] start_millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined, start_millisecond must be less than/equal to end_millisecond
+        * [OPTIONAL] end_millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined, end_millisecond must be greater than/equal to start_millisecond
         
-        **convertFlybyIDToObservationNumber**
+        ```python
+        import pydar
+        pydar.retrieveIDSByTimeRange(start_year=2004,
+        				start_doy=299,
+        				start_hour=2,
+        				start_minute=15,
+        				start_second=23,
+        				start_millisecond=987,
+        				end_year=2005, 
+        				end_doy=301,
+        				end_hour=2,
+        				end_minute=15,
+        				end_second=23,
+        				end_millisecond=987)
+        ```
+        Output = `{'Ta': ['S01'], 'T3': ['S01'], 'T7': ['S01']}`
+        
+        ### convertFlybyIDToObservationNumber()
         
         Converts a Titan Flyby ID (for example: 'T65') to an observation number with front padding ('T65' -> '0211')
         
         ```python
         convertFlybyIDToObservationNumber(flyby_id)
         ```
-        * **[REQUIRED/OPTIONAL]** flyby_id (string): a valid flyby ID with prefix 'T'
+        * **[REQUIRED]** flyby_id (string): a valid flyby ID with prefix 'T'
         
         ```python
         import pydar
-        
-        observation_number = convertFlybyIDToObservationNumber(flyby_id)
+        observation_number = convertFlybyIDToObservationNumber(flyby_id='T65')
         ```
+        Output = `0211`
         
-        Observation number based on the 'Radar Data Take Number' in the cassini_flyby.csv file with front padding to ensure that all observation numbers are 4 digits long (0065 and 0211)
+        Observation number based on the 'Radar Data Take Number' in the [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv) data file with front padding to ensure that all observation numbers are 4 digits long (0065 and 0211)
         
-        Requires each Titan flyby ID to be a valid value the cassini_flyby.csv 
+        ### convertObservationNumberToFlybyID()
         
-        **displayImages**
+        Converts a Titan Observation Number (for example: '211' or '0211') to an flyby id ('0211' -> 'T65')
         
+        ```python
+        convertObservationNumberToFlybyID(flyby_observation_num)
         ```
-        displayImages(image_directory=None)
+        * **[REQUIRED]** flyby_observation_num (string): a valid observation number
+        
+        ```python
+        import pydar
+        flyby_id = pydar.convertObservationNumberToFlybyID(flyby_observation_num='211')
         ```
+        Output = `T65`
         
-        * **[REQUIRED]** image_directory (string): 
+        Flyby ids are based on the 'Radar Data Take Number' in the [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv) data file with front padding of 'T'
         
-        Displays downloaded image .IMG files (unzipped from within the .ZIP files)
+        Requires each Titan flyby ID to be a valid flyby ID in [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
+        
+        ### extractFlybyDataImages()
+        
+        Downloads flyby data SBDR for a selected flyby observation number or flyby id: .FMT and .TAB files (for example: [SBDR.FMT](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR.FMT) and [SBDR_15_D087_V03.TAB](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR_15_D087_V03.TAB))
+        
+        Downloads flyby data BIDR for a selected flyby observation number or flyby id: .LBL and .ZIP files (for example: [BIBQH80N051_D087_T016S01_V03.LBL](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.LBL) and [BIBQH80N051_D087_T016S01_V03.ZIP](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.ZIP))
         
-        ```python
-        import pydar
-        # Display all Images in pydar_results/ directory
-        pydar.displayImages("pydar_results/CORADR_0065_V03_S01")
         ```
-        displayImages() will plt.show() all images in the saved results directory
+        extractFlybyDataImages(flyby_observation_num=None,
+        			flyby_id=None,
+        			segment_num=None,
+        			additional_data_types_to_download=[],
+        			resolution='I',
+        			top_x_resolutions=None)
+        ```
+        Either a flyby_id (for example: 'T65') or a flyby_observation_num (for example: '0035') is required. 
         
-        **extractMetadata**
+        Note: a flyby_id will be translated into a flyby_observation_number to access on the backend and the results will be saved under the observation number. For example, 'T65' will become observation number '0211'
         
-        Extract metadata from .TAB file (using .FMT as a reference)
+        * **[REQUIRED/OPTIONAL]** flyby_observation_num (string): required if flyby_id not included
+        * **[REQUIRED/OPTIONAL]** flyby_id (string): required if flyby_observation_num not included
+        * **[REQUIRED]** segment_num (string): a flyby includes multiple image segments (S0X) where S01 is the primary imaging segment ["S01", "S02", "S03", "S04"]
+        * [OPTIONAL] resolution (String): resolution options "B", "D", "F", "H", or "I" (2, 8, 32, 128, 256 pixels/degree), defaults to highest resolution 'I'
+        * [OPTIONAL] top_x_resolutions: Save the top x resolution types (5 total resolutions), will override any default resolution string
+        * [OPTIONAL] additional_data_types_to_download (List of Strings): Possible options ["ABDR", "ASUM", "BIDR", "LBDR", "SBDR", "STDR"] (__NOTE__: current v1 functionality does not download any additional data types)
         
         ```python
         import pydar
-        # Extract Metadata from .FMT and .TAB files
-        pydar.extractMetadata()
+        pydar.extractFlybyDataImages(flyby_id='T65',
+        			resolution='D',
+        			segment_num="S01")
         ```
         
-        **readAAREADME**
+        extractFlybyDataImages() will retrieve images from PDS website and saves results in a directory labeled 'pydar_results' with the flyby observation number, version number, and segment number in the title (for example pydar_results/CORADR_0065_V03_S01). Download time depends on file and resolution size but ranges from 5-30 minutes
+        
+        ### readAAREADME()
         
         Print AAREADME.TXT to console for viewing
         
         ```
         readAAREADME(coradr_results_directory=None,
-        			section_to_print=None, 
-        			print_to_console=True)
+        	section_to_print=None, 
+        	print_to_console=True)
         ```
         
-        * **[REQUIRED]** coradr_results_directory (string):
-        * [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT (readme options: ['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'OBJECT', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information'])
+        * **[REQUIRED]** coradr_results_directory (string): CORADAR results folder downloaded (example: "pydar_results/CORADR_0211_V03_S01/")
+        * [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT, not case-sensitive 
         * [OPTIONAL] print_to_console (boolean): Print to console, defaults to true, otherwise function will return output as a string
         
+        To see a list of all section_to_print options, see: `returnAAREADMEOptions()`
+        
         ```python
         import pydar
-        # Print AAREADME.TXT
         pydar.readAAREADME(coradr_results_directory="pydar_results/CORADR_0065_V03_S01",
-        						section_to_print="Volume")
+        		section_to_print="Volume")
         ```
-        Output = "Volume CORADR_0065:  Titan Flyby T8, Sequence S15, Oct 27, 2005"
-        
-        To get the section that are avaiable for printing: returnAllAAREADMEOptions()
-        
+        Output = `Volume CORADR_0065:  Titan Flyby T8, Sequence S15, Oct 27, 2005`
         ```python
         import pydar
-        pydar.returnAllAAREADMEOptions()
+        pydar.returnAAREADMEOptions()
         ```
         
-        ['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information']
+        Output = `['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information']`
         
-        **readLBLREADME**
+        ### readLBLREADME()
         
         Print .LBL README to console for viewing
         
         ```
         readLBLREADME(coradr_results_directory=None,
-        			section_to_print=None, 
-        			print_to_console=True)
+        	section_to_print=None, 
+        	print_to_console=True)
         ```
         
         * **[REQUIRED]** coradr_results_directory (string):
-        * [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT (readme options: ['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'OBJECT', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information'])
+        * [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT, not case-sensitive
         * [OPTIONAL] print_to_console (boolean): Print to console, defaults to true, otherwise function will return output as a string
         
+        To see a list of all section_to_print options, see: `returnLBLOptions()`
+        
         ```python
         import pydar
-        # Print .LBL README
         pydar.readLBLREADME(coradr_results_directory="pydar_results/CORADR_0035_S01/",
         		section_to_print="OBLIQUE_PROJ_X_AXIS_VECTOR")
         ```
         Output = `(0.13498322,0.00221225,-0.99084542)`
-        
-        To get the sections that are available for printing: returnAllLBLOptions()
         ```python
         import pydar
-        pydar.returnAllLBLOptions()
+        pydar.returnLBLOptions()
         ```
         <details closed>
         <summary>Line-By-Line Options (Click to view all)</summary>
         <br>
         ['PDS_VERSION_ID', 'DATA_SET_ID', 'DATA_SET_NAME', 'PRODUCER_INSTITUTION_NAME', 'PRODUCER_ID', 'PRODUCER_FULL_NAME', 'PRODUCT_ID', 'PRODUCT_VERSION_ID', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_HOST_ID', 'INSTRUMENT_NAME', 'INSTRUMENT_ID', 'TARGET_NAME', 'START_TIME', 'STOP_TIME', 'SPACECRAFT_CLOCK_START_COUNT', 'SPACECRAFT_CLOCK_STOP_COUNT', 'PRODUCT_CREATION_TIME', 'SOURCE_PRODUCT_ID', 'MISSION_PHASE_NAME', 'MISSION_NAME', 'SOFTWARE_VERSION_ID', 'FILE_NAME COMPRESSED', 'RECORD_TYPE COMPRESSED', 'ENCODING_TYPE', 'INTERCHANGE_FORMAT', 'UNCOMPRESSED_FILE_NAME', 'REQUIRED_STORAGE_BYTES', '^DESCRIPTION', 'FILE_NAME UNCOMPRESSED', 'RECORD_TYPE UNCOMPRESSED', 'RECORD_BYTES', 'FILE_RECORDS', 'LABEL_RECORDS', '^IMAGE', 'LINES', 'LINE_SAMPLES', 'SAMPLE_TYPE', 'SAMPLE_BITS', 'CHECKSUM', 'SCALING_FACTOR', 'OFFSET', 'MISSING_CONSTANT', 'NOTE', '^DATA_SET_MAP_PROJECTION', 'MAP_PROJECTION_TYPE', 'FIRST_STANDARD_PARALLEL', 'SECOND_STANDARD_PARALLEL', 'A_AXIS_RADIUS', 'B_AXIS_RADIUS', 'C_AXIS_RADIUS', 'POSITIVE_LONGITUDE_DIRECTION', 'CENTER_LATITUDE', 'CENTER_LONGITUDE', 'REFERENCE_LATITUDE', 'REFERENCE_LONGITUDE', 'LINE_FIRST_PIXEL', 'LINE_LAST_PIXEL', 'SAMPLE_FIRST_PIXEL', 'SAMPLE_LAST_PIXEL', 'MAP_PROJECTION_ROTATION', 'MAP_RESOLUTION', 'MAP_SCALE', 'MAXIMUM_LATITUDE', 'MINIMUM_LATITUDE', 'EASTERNMOST_LONGITUDE', 'WESTERNMOST_LONGITUDE', 'LINE_PROJECTION_OFFSET', 'SAMPLE_PROJECTION_OFFSET', 'OBLIQUE_PROJ_POLE_LATITUDE', 'OBLIQUE_PROJ_POLE_LONGITUDE', 'OBLIQUE_PROJ_POLE_ROTATION', 'OBLIQUE_PROJ_X_AXIS_VECTOR', 'OBLIQUE_PROJ_Y_AXIS_VECTOR', 'OBLIQUE_PROJ_Z_AXIS_VECTOR', 'LOOK_DIRECTION', 'COORDINATE_SYSTEM_NAME', 'COORDINATE_SYSTEM_TYPE']
         </details>
         <details closed>
         <summary>Section Header Options (Click to view all)</summary>
         <br>
         ['PRODUCT DESCRIPTION', 'DESCRIPTION OF COMPRESSED AND UNCOMPRESSED FILES', 'POINTERS TO START RECORDS OF OBJECTS IN FILE', 'DESCRIPTION OF OBJECTS CONTAINED IN FILE']
         </details>
         
-        **retrieveFeaturesFromLatitudeLongitude**
-        
-        Return a list of features found at a specific latitude/longitude position
+        ## Use Downloaded Data
+        ### displayImages()
         
         ```
-        retrieveFeaturesFromLatitudeLongitude(latitude=None, longitude=None)
+        displayImages(image_directory=None, fig_title=None, figsize_n=6, fig_dpi=120)
         ```
-        * **[REQUIRED]** latitude (float/int): Latitude (in degrees) where North = + and South = -
-        * **[REQUIRED]** longitude (float/int): Longitude (in degrees) where West = + and East = -
+        
+        * **[REQUIRED]** image_directory (string): directory containing pydar_results with IMG file
+        * [OPTIONAL] fig_title (str): figure title, defaults to filename
+        * [OPTIONAL] figsize_n (int): plot dimensions, defaults to 6x6
+        * [OPTIONAL] fig_dpi (int): plot dpi, defaults to 120
+        
+        Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
         
         ```python
         import pydar
-        feature_names_list = pydar.retrieveFeaturesFromLatitudeLongitude(latitude=-72, longitude=183)
+        pydar.displayImages(image_directory="pydar_results/CORADR_0065_V03_S01")
         ```
+         <p align="center">
+          <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
+        </p>
         
-        feature_names_list = `['Ontario Lacus']`
+        Note: displayImages() will plt.show() all images in the saved results directory
         
-        **retrieveFeaturesFromLatitudeLongitudeRange**
+        **COMING SOON: extractMetadata**
         
-        ```
-        retrieveFeaturesFromLatitudeLongitudeRange(northernmost_latitude=None,
-        										southernmost_latitude=None,
-        										easternmost_longitude=None,
-        										westernmost_longitude=None)
-        ```
-        * **[REQUIRED]** northernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, north must be greater than or equal to the south
-        * **[REQUIRED]** southernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, south must be less than or euqal to the north
-        * **[REQUIRED]** easternmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, west must be less than or equal to the east
-        * **[REQUIRED]** westernmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, east must be greater than or equal to the west
+        Extract Metadata from .FMT and .TAB files
         
-        ```python
-        import pydar
-        feature_names_list = pydar.retrieveFeaturesFromLatitudeLongitudeRange(northernmost_latitude=11,
-        																southernmost_latitude=-80,
-        																easternmost_longitude=339,
-        																westernmost_longitude=341)
-        ```
-        feature_names_list = `['Aaru', 'Rossak Planitia']`
+        COMING SOON: Extract metadata from .TAB file (using .FMT as a reference)
         
-        ## TODO:
+        ## Developer Notes TODO:
         ### TODO Code:
-        * retrieveIDSByTime() based on time or time range
         * add a colored outline around a feature when displaying as a 2D image
+        * save image pixel to an array
+        * extract pdr functionality to reduce overhead
+        * displayImages() bug fix: 87 displays invalid integer
         * segments will be less than 99 (default to 1 - 01 is the primary imaging)
-        * README for all the functions and their sections
         * progress bars print to command line (still downloading...)
+        * save .IMG as .SHP for ArcGIS
         
         ### TODO Questions:
-        * what is the timestamp for start/stop time: "2005-301T03:53:56.971" format? YYYY-MDDTHH:MM:SS.mms?
-        * get longitude values when greater than 180 (everything is relative to west)
-        * add details for what a segement_num is
+        * add details for what a segment_num is
         * associate burst ID from SBDR data to BIDR data for metadata
         * save .IMG as an array of pixel values
         * save .IMG as .SHP for ArcGIS
         * project image onto Titan spheriod
         * downloadAdditionalDataTypes() does not have functionality (["ABDR", "ASUM", "LBDR", "STDR"]), decide which files to download
         
         ### TODO: Tech Debt
         * use README information to gather files for download (save computing, tech debt)
-        * CSV script to be run before each pypi package update by developer not user
-        * make README options for .LBL and AAREADME case-insensitive
         * set up constant config file
-        * bug fix: "NOTE" in .lbl
+        * Add functionality for extractFlybyDataImages(): additional_data_types_to_download
         * Include URL for access to AAREADME and .LBL readme files
-        * rm -rf pydar_results/ between runs for clean image output
         * research Zenodo
         
         ### TODO: Test
         * test: pull up all passes that saw Ontario Lacus and colorcode with look angle 
         * test: pull beam information and number of looks for each pixel 
         
+        ## Credits
+        Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
+        
+        Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+        
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/unaschneck/pydar/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pydar-0.1.0/README.md` & `pydar-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,90 @@
 # PYDAR
+ <p align="center">
+  <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
+</p>
+
 ![PyPi](https://img.shields.io/pypi/v/pydar)
-![license](https://img.shields.io/github/license/unaschneck/pydar)
+![license](https://img.shields.io/pypi/l/pydar)
 [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
+![PyPi-Versions](https://img.shields.io/pypi/pyversions/pydar)
+[![update-dynamic-csv-data-files](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml)
+[![pytests](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml)
+
+A Python package to access, download, view, and manipulate Cassini RADAR images in one place
+
+* **Find relevant flyby observation numbers/IDs for a feature, range of latitude/longitudes (or specific latitude/longitude), or a time range (or specific time)**
+	* retrieveIDSByFeatureName()
+	* retrieveIDSByLatitudeLongitude()
+	* retrieveIDSByLatitudeLongitudeRange()
+	* retrieveFeaturesFromLatitudeLongitude()
+	* retrieveFeaturesFromLatitudeLongitudeRange()
+	* retrieveIDSByTime()
+	* retrieveIDSByTimeRange()
+* **Use flyby observation numbers/IDs to retrieve flyby observation data (.FMT, .TAB, .LBL, .IMG) from SBDR and BIDR data files by default**
+	* convertFlybyIDToObservationNumber()
+	* convertObservationNumberToFlybyID()
+	* extractFlybyDataImages()
+* **Access specific observation data from AAREADME and .LBL readme information**
+	* returnAAREADMEOptions()
+	* readAAREADME()
+	* returnLBLOptions()
+	* readLBLREADME()
+* **Display PDS image retrieved for flyby observation**
+	* displayImages()
 
-Python Package to access and manipulate CASSINI RADAR images in one place
+NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.  
 
-* Find relevant flyby observation numbers and IDs for a specific region, feature, or location
-* Retrieve flyby observation data (.FMT, .TAB, .LBL, .IMG) from SBDR and BIDR by default
-* Access AAREADME and .LBL readme information
-* Display PDS image retrieved for flyby observation
+## Install
+PyPi pip install at [pypi.org/project/pydar/](https://pypi.org/project/pydar/)
 
-NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.  
+```
+pip install pydar
+```
 
-## Overview
-For information on instrument specifics and acronyms refer to the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+## Dependencies
+Python 3.7+
 
-The Cassini Radar data can be found at the [PDS Imaging Node](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/). The directory is organized by [PDS standards](https://pdssbn.astro.umd.edu/howto/understand.shtml). The file format are defined in the [Small Body Node](https://pdssbn.astro.umd.edu/howto/file_types.shtml). The radar echo is stored originally as floating points in LBDR files. The SAR processors turns the LBDR files to BIDR image. The BIDR data is organized as follows:
+Verified compatibility with Python 3.7, 3.8, and 3.9
+```
+pip install -r requirements.txt
+```
+Requirements will also be downloaded as part of the pip download
+
+## Quickstart: PYDAR
+
+All Cassini data for Titan is retrieved based on flyby observation numbers or IDs, so relevant flybys can be found based on time range, latitude/longitude position, or a known feature name
+
+```python
+import pydar
+feature_name_example = "ontario lacus"
+flyby_ids = pydar.retrieveIDSByFeatureName(feature_name=feature_name_example)
+```
+Returns a dictionary of flyby IDs (and their relevant segments) that Ontario Lacus could be found from: `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
+
+The relevant data files can be downloaded for any combination of these flyby IDs and segment numbers. For example, flyby ID 'T65' and segment 'S01' at resolution 'D' for 8 pixels/degree
+```
+# Extract Flyby Data Files to pydar_results/ directory
+pydar.extractFlybyDataImages(flyby_id='T65',
+				resolution='D',
+				segment_num="S01")
+```
+Note: extractFlybyDataImages() only needs to be run once for each flyby to retrieve new data but will take some time to download
+```
+# Display all Images in pydar_results/ directory
+pydar.displayImages(image_directory="pydar_results/CORADR_0211_V03_S01")
+```
+ <p align="center">
+  <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
+</p>
+
+## Overview and Background
+For information on Cassini instrument specifics and acronyms refer to the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+
+The Cassini Radar data can be found at the [PDS Imaging Node](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/). The directory is organized by [PDS standards](https://pdssbn.astro.umd.edu/howto/understand.shtml). The file format are defined in the [Small Body Node](https://pdssbn.astro.umd.edu/howto/file_types.shtml). The radar echo is stored originally as floating points in LBDR files. The SAR processors turn the LBDR files into BIDR image. The BIDR data is organized as follows:
 ```
 Cassini RADAR Information (CORADR_xxxx_Vxx) where xxxx is the radar data take number and Vxx is the data version number
   |_ AAREADME.txt
     Information about observation xxxx (xxxx > 0035 for Titan flybys)
   |_CALIB/
   |_CATALOG/
     BIDRDS.CAT: Information about the BIDR dataset
@@ -91,433 +156,559 @@
   |_ERRATA.txt
   |_EXTRAS/
     |_BIbcdeefggg_Dhhh_Tiii_Vnn.JPG: jpg of IMG files in DATA 
   |_INDEX/
   |_SOFTWARE/
   |_VOLDESC.CAT <--- VERSION INFORMATION LISTED HERE ('VOLUME_VERSION_ID' = "Version 1", "Version 2", "Version 3") and in filename
 ```
+.IMG files can be viewed using the [planetary images library](https://planetaryimage.readthedocs.io/_/downloads/en/latest/pdf/) or via `pydar.displayImages()`
 
-.IMG files can be viewed using the [planetary images library](https://planetaryimage.readthedocs.io/_/downloads/en/latest/pdf/)
 ### Download Time
-Download time varies depending on the number and size of files of interest. On average, most single feature downloads take between 2-5 minutes to download.
+Download time for data files vary when using `pydar.extractFlybyDataImages()` and depends on the number and size of files of interest. On average, most single feature downloads take between 5-30 minutes to download, but can be longer for higher resolution files.
 
 ![image](https://user-images.githubusercontent.com/24469269/211881026-5bab329c-cf0d-416b-bedc-6d466b77b1f5.png)
 ([Cassini Radar Volume SIS, Version 2.1](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0284/DOCUMENT/VOLSIS.PDF) Table 1, pg. 3)
-### Cross-Reference Table for Observations and Flybys
-The Titan flybys ID is not used in the naming convention for the CORADR filenames. The Titan flyby information is contained in the BIDR filenames and in the VOLDESC.CAT under 'Description' and can be found using the following cross-reference table: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
 
-```
-Flyby ID Cross Reference Table
-Prime Mission and Extended Mission
-
-Column 1: Titan flyby id
-Column 2: Radar Data Take Number
-Column 3: Sequence number
-Column 4: Orbit Number/ID
-
-Ta   DTN 035   S05 Rev 0A
-T3   DTN 045   S08 Rev 03
-T4   DTN 048   S09 Rev 04
-T7   DTN 059   S14 Rev 14
-T8   DTN 065   S15 Rev 17
-
-...
-```
+### Cross-Reference Table for Observations and Flybys
+The Titan flyby IDs (e.g. 'T65') are not used in the naming convention for the CORADR filenames. Instead, all files are referred to by their observation number (e.g. '0211'). The Titan flyby information is contained in the BIDR filenames and in the VOLDESC.CAT under 'Description' and can be found using the following cross-reference table: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
 
-To convert between a Titan Flyby ID and an observation number: `pydar.convertFlybyIDToObservationNumber(flyby_id)`
+To convert between a Titan Flyby ID and an observation number use either `pydar.convertFlybyIDToObservationNumber(flyby_id)` or `pydar.convertObservationNumberToFlybyID(flyby_observation_num)`
 
 ### Observation Information as filename
-The data filename contains a lot of information about the observation 
+The data filename contains a lot of information about the observation
 
 (EXAMPLE) Filename: "BIBQD05S184_D065_T008S03_V03"
 
 - BI = BIDR data
 - B = data in dB normalized
-- Q = obliquid dylindrical
+- Q = oblique cylindrical
 - D = 8 pixels/degree
 - 05 = absolute value of latitude at center rounded to nearest degree
 - S = hemisphere of center of file (Southern)
 - 184 = West longitude at center of file rounded to nearest degree
 - D065 = 2-digit data take ID aka observation counter with left-padded zeros
 - T008 = 3-digit Titan flyby with left-padding
 - S03 = 2-digit segment number (00-99)
 - V03 = 2-digit version number (01-99)
 
-BIBQD05S184_D065_T008S03_V03.JPG:
+Image file from BIBQD05S184_D065_T008S03_V03.JPG:
 
 ![BIFQI10S251_D065_T008S01_V03](https://user-images.githubusercontent.com/24469269/210164143-427003ed-0043-45b4-a80f-8e9ddf28543a.jpg)
 
 ### Volume Version of Data
 
-Some passes have multiple versions of the data.
-
-* Version 1 (V01) was the first archived version of the data and assumed Titan had zero obliquity, which resulted in misregistration between passes
-
-* Version 2 (V02) used a Titan spin model that reduced misregistration error 
+Some passes have multiple versions of the data, up to 3 different versions currently.
 
-* Version 3 (V03) used a long-term, accurate spin model for Titan along with other improvements
+* **Version 1 (V01)** was the first archived version of the data and assumed Titan had zero obliquity, which resulted in misregistration between passes
+* **Version 2 (V02)** used a Titan spin model that reduced misregistration error 
+* **Version 3 (V03)** used a long-term, accurate spin model for Titan along with other improvements
 
 Only some Titan passes produced all of the version numbers.
 
 * TA-T25 : V01, V02, V03
 
 * $\gt$ T28: V02, V03
 
 * T108-T126: labeled only once as V02 but is actually V03
 
-The version number is listed in the filenanme and in VOLDESC.CAT under the 'VOLUME_VERSION_ID'
+The version number is listed in the filename and in VOLDESC.CAT under the 'VOLUME_VERSION_ID'
 
-*Version 3 is the latest and preferred version*
+_**Version 3 is currently the latest and preferred version and will be the version included when downloaded**_
 
 Example:
 
 Version 1 is named BIFQI48N071_D035_T00A_V01.IMG
 
 Version 2 is named BIFQI49N071_D035_T00AS01_V02.IMG
 
 Version 3 is named BIFQI49N071_D035_T00AS01_V03.IMG
 
 ### Segment Number of Data
 A single flyby can produce multiple image segments (Sxx). *S01 is the primary imaging segment* with other segments referring to periods in the flyby when the instrument went to/from altimetry/SAR/HiSAR or weird pointing profiles.  
 
 ![image](https://user-images.githubusercontent.com/24469269/210197286-c059ffed-281d-46c7-911a-f86c3bf7ea28.png)
-Credit: Cassini Radar User Guide (Wall et al. 2019, pg.16)
-## Documentation
+*Credit: Cassini Radar User Guide (Wall et al. 2019, pg.16)*
+
+## Backend Data Files
+
+### Dynamically Updated Backend Files
+
+Pydar includes multiple scripts to web scrape from relevant URLs to generate some of the backend data files
+
+Changes in the relevant URLs are checked once a month via Github Actions to keep csv files up to date and any changes found will be bundled into the subsequent release
+
+**coradr_jpl_options.csv**
+
+Contains all the CORADR IDs and available data types from [pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter)
+
+Headers: ["CORADR ID", "Is a Titan Flyby", "Contains ABDR", "Contains ASUM", "Contains BIDR", "Contains LBDR", "Contains SBDR", "Contains STDR"]
 
-## Data Files
+View data file: [coradr_jpl_options.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/coradr_jpl_options.csv)
+
+**swath_coverage_by_time_position.csv**
+
+Contains all the information for .LBL files within all CORADR ID pages (for each segment and resolution file)
+
+Collected from URLs matching: pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/[CORADAR_ID]/DATA/BIDR/
+
+Headers: ["CORADR ID", "FLYBY ID", "SEGMENT NUMBER", "FILENAME", "DATE TYPE SYMBOL", "DATE TYPE", "RESOLUTION (pixels/degrees)", "TARGET_NAME", "MAXIMUM_LATITUDE (Degrees)", "MINIMUM_LATITUDE (Degrees)", "EASTERNMOST_LONGITUDE (Degrees)", "WESTERNMOST_LONGITUDE (Degrees)", "START_TIME", "STOP_TIME"]
+
+View data file: [swath_coverage_by_time_position.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/swath_coverage_by_time_position.csv)
 
 **feature_name_details.csv**
 
-List of Features on Titan with names with their associated position and the origin of their name. Taken from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/Feature/6981)
+Contains all named features on Titan with their furthest latitude/longitude position and origin of name
 
-## SBDR Files
-[SBDR column descriptions](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0045/DOCUMENT/BODPSIS.PDF)
+Collected from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
 
-Total width of the RADAR swath is created by combining the five individual sub-swaths, where the center beam is the highest gain
-![image](https://user-images.githubusercontent.com/24469269/211431884-c201ac74-114a-4c17-b95a-f9edf0178d2e.png)
-(_The Cassini Huygens Mission: Orbiter Remote Sensing Observation 2004_)
+Headers: ["Feature Name", "Northernmost Latitude", "Southernmost Latitude", "Easternmost Longitude", "Westernmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
 
-```
-test_file = "SBDR_15_D065_V03.TAB"
-SBDR_FILE = pdr.read(test_file)
-print("Table options: {0}".format(SBDR_FILE.keys()))
-```
+View data file: [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
+
+### Static Data Files
+
+**cassini_flyby.csv**
+
+Reference for converting between a Titan Flyby ID (e.g. "T7") and its Observation Number (e.g. "059") (and back)
+
+Headers: ["Titan flyby id", "Radar Data Take Number", "Sequence number", "Orbit Number/ID"]
+
+View data file: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
+
+**sar_swath_details.csv**
+
+Currently unused, but will potentially be used in the future for incidence angle, polarization, azimuth, SAR range resolution, SAR azimuth resolution, and number of looks
+
+Converted to a static csv file from the Cassini User Guide (pg. 136-139)
+
+View data file: [sar_swath_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/sar_swath_details.csv)
 
 ## BIDR and SBDR Files
 Note: "CORADR_0048", "CORADR_0186", "CORADR_0189", "CORADR_0209", "CORADR_0234" do not have associated BIDR values.
 
 There are data gaps and problems from the original downlinking and satellite location
 
-CORADR_0048 (T4) did not have SAR data, only scatterometry and radiometery because of telemetry reasons in the handbook
+CORADR_0048 (T4) did not have SAR data, only scatterometry and radiometry because of telemetry reasons in the handbook
 
-CORADR_0186 (T52) only have rad and compressed scatterometry
+CORADR_0186 (T52) only have radiometry and compressed scatterometry
 
-CORADR_189 (T53) only has rad and compressed scatterometry because of what appears to be a downlink problem
+CORADR_0189 (T53) only has radiometry and compressed scatterometry because of what appears to be a downlink problem
 
 CORADR_0209 (T63) only has scatterometry and radiometry
 
 CORADR_0234 (T80) only has scatterometry and radiometry 
-## Dependencies
-Python 3.9
-```
-pip3 install -r requirements.txt
-```
-## Install
-PyPi pip install at [pypi.org/project/pydar/](https://pypi.org/project/pydar/)
 
-```
-pip install pydar
-```
+## Coming Soon: SBDR Files
+Total width of the RADAR swath is created by combining the five individual sub-swaths, where the center beam is the highest gain
+![image](https://user-images.githubusercontent.com/24469269/211431884-c201ac74-114a-4c17-b95a-f9edf0178d2e.png)
+(_The Cassini Huygens Mission: Orbiter Remote Sensing Observation 2004_)
+
+[SBDR column descriptions](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0045/DOCUMENT/BODPSIS.PDF)
 
-## Examples
+## Retrieve Data from CASSINI Function Calls
 
-To collect flyby information and images from a feature on Titan, start by selecting a feature, for example: "Ontario Lacus"
+To collect flyby information and images for the latitude/longitude range of a named feature on Titan
 
-**retrieveIDSByFeatureName**
+### retrieveIDSByFeatureName()
 
-Retrieve a list of flyby IDs with their associated segments based on a feature name from titan
+Retrieve a list of flyby IDs with their associated segment numbers based on a feature name from Titan
 
 ```python
 retrieveIDSByFeatureName(feature_name=None)
 ```
-* **[REQUIRED]** feature_name (string): Feature name on Titan to give flyby ids and segments, not case-sensitive
+* **[REQUIRED]** feature_name (string): Feature name on Titan, not case-sensitive
 
 Feature names are retrieved from [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
 <details closed>
 <summary>List of Valid Feature Names (Click to view all)</summary>
 <br>
 ['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
 </details>
 
 ```python
 import pydar
 pydar.retrieveIDSByFeatureName(feature_name="Ontario Lacus")
 ```
-Output = `{'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
+Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
 
-**retrieveIDSByLatitudeLongitude**
+### retrieveIDSByLatitudeLongitude()
 
 Retrieve a list of flyby IDs with their associated segments based on specific latitude and longitude
 
 ```python
 retrieveIDSByLatitudeLongitude(latitude=None, longitude=None)
 ```
-* **[REQUIRED]** latitude (float/int): Latitude (in degrees) where North = + and South = -
-* **[REQUIRED]** longitude (float/int): Longitude (in degrees) where West = + and East = -
+* **[REQUIRED]** latitude (float/int): Latitude (in degrees), range from -90° to 90°
+* **[REQUIRED]** longitude (float/int): Longitude (in degrees), range from 0° to 360°
 
 ```python
 import pydar
-pydar.retrieveIDSByLatitudeLongitude(latitude=10, longitude=10)
+pydar.retrieveIDSByLatitudeLongitude(latitude=-80, longitude=170)
 ```
-Output = `{'T19': ['S01'], 'T29': ['S01'], 'T55': ['S01'], 'T56': ['S01'], 'T57': ['S01'], 'T58': ['S01'], 'T64': ['S01'], 'T83': ['S02'], 'T84': ['S02'], 'T92': ['S01'], 'T98': ['S02'], 'T104': ['S01']}`
+Output = `{'T39': ['S06', 'S05', 'S01'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S03'], 'T56': ['S01'], 'T57': ['S01'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
 
-**retrieveIDSByLatitudeLongitudeRange**
+### retrieveIDSByLatitudeLongitudeRange()
+
+Retrieve a list of flyby IDs with their associated segments based on range of latitudes and longitudes
 
 ```python
-retrieveIDSByLatitudeLongitudeRange(northernmost_latitude=None,
-				southernmost_latitude=None,
-				easternmost_longitude=None,
-				westernmost_longitude=None)
+retrieveIDSByLatitudeLongitudeRange(min_latitude=None,
+				max_latitude=None,
+				min_longitude=None,
+				max_longitude=None)
 ```
-* **[REQUIRED]** northernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, north must be greater than or equal to the south
-* **[REQUIRED]** southernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, south must be less than or euqal to the north
-* **[REQUIRED]** easternmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, west must be less than or equal to the east
-* **[REQUIRED]** westernmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, east must be greater than or equal to the west
+* **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be greater than or equal to the max_latitude, range from -90° to 90°
+* **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be less than or equal to the min_latitude, range from -90° to 90°
+* **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
+* **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude be greater than or equal to the min_longitude, range from 0° to 360°
 
 ```python
-retrieveIDSByLatitudeLongitudeRange(northernmost_latitude=15,
-				southernmost_latitude=10,
-				easternmost_longitude=12,
-				westernmost_longitude=17)
+import pydar
+pydar.retrieveIDSByLatitudeLongitudeRange(min_latitude=-82,
+					max_latitude=-72,
+					min_longitude=183,
+					max_longitude=185)
 ```
-Output = `{'T19': ['S01'], 'T29': ['S01'], 'T55': ['S01'], 'T56': ['S01'], 'T57': ['S01'], 'T64': ['S01'], 'T83': ['S02'], 'T84': ['S02'], 'T92': ['S01'], 'T98': ['S02'], 'T104': ['S01']}`
+Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
 
-Ontario Lacus was visible in four swath observations: T57, T58, T65, T98 [(Page 163)](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf).
+### retrieveFeaturesFromLatitudeLongitude()
 
-To access flyby of Ontario, first specify a flyby. For this example, Ontario Lacus with the features:
+Return a list of features found at a specific latitude/longitude position
 
-* Titan flyby id: 'T65'
-* resolution: 'D' (8 pixels/degree)
-* Main imaging segement 1: 'S01'
+```
+retrieveFeaturesFromLatitudeLongitude(latitude=None, longitude=None)
+```
+* **[REQUIRED]** latitude (float/int): Latitude (in degrees), range from -90° to 90°
+* **[REQUIRED]** longitude (float/int): Longitude (in degrees), range from 0° to 360°
 
-**extractFlybyDataImages()**
+```python
+import pydar
+pydar.retrieveFeaturesFromLatitudeLongitude(latitude=-72, longitude=183)
+```
+
+Output = `['Ontario Lacus', 'Rossak Planitia']`
 
-Downloads flyby data SBDR: .FMT and .TAB files (for example: [SBDR.FMT](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR.FMT) and [SBDR_15_D087_V03.TAB](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR_15_D087_V03.TAB))
+### retrieveFeaturesFromLatitudeLongitudeRange()
 
-Downloads flyby data BIDR: .LBL and .ZIP files (for example: [BIBQH80N051_D087_T016S01_V03.LBL](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.LBL) and [BIBQH80N051_D087_T016S01_V03.ZIP](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.ZIP))
+Return a list of features found at a range of latitude/longitude positions
 
 ```
-extractFlybyDataImages(flyby_observation_num=None,
-			flyby_id=None,
-			segment_num=None,
-			additional_data_types_to_download=[],
-			resolution='I',
-			top_x_resolutions=None)
+retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=None,
+					max_latitude=None,
+					min_longitude=None,
+					max_longitude=None)
 ```
-Either a flyby_id (for example: 'T65') or a flyby_observation_num (for example: '0065') is required. A flyby_id will be translated into a flyby_observation_number to access on the backend and the results will be saved under the observation number. 'T65' will become observation number '0021'
+* **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be less than or equal to the max_latitude, range from -90° to 90°
+* **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be greater than or equal to the min_latitude, range from -90° to 90°
+* **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
+* **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude must be greater than or equal to the min_longitude, range from 0° to 360°
 
-* **[REQUIRED/OPTIONAL]** flyby_observation_num (string): required if flyby_id not included
-* **[REQUIRED/OPTIONAL]** flyby_id (string): required if flyby_observation_num not included
-* **[REQUIRED]** segment_num (string): 
-* [OPTIONAL] additional_data_types_to_download (List of Strings): Possible options ["ABDR", "ASUM", "BIDR", "LBDR", "SBDR", "STDR"]
-* [OPTIONAL] resolution (String): resolution options "B", "D", "F", "H", or "I" (2, 8, 32, 128, 256 pixels/degree), defaults to highest resolution 'I'
-* [OPTIONAL] top_x_resolutions: Save the top x resolution types (5 total resolutions)
+```python
+import pydar
+
+pydar.retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=-82,
+						max_latitude=-72,
+						min_longitude=183,
+						max_longitude=190)
+```
+Output = `['Crveno Lacus', 'Ontario Lacus', 'Romo Planitia', 'Rossak Planitia', 'Saraswati Flumen']`
+
+### retrieveIDSByTime()
+
+Retrieve a dictionary of flyby IDs and segment numbers based on a specific timestamp
+
+```
+retrieveIDSByTime(year=None,
+		doy=None,
+		hour=None,
+		minute=None,
+		second=None,
+		millisecond=None)
+```
+* **[REQUIRED]** year (int): Year for observation, range from 2004 to 2014
+* **[REQUIRED]** doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year)
+* [OPTIONAL] hour (int): Hour, from 0 to 23 in UTC, defaults to 0 when undefined
+* [OPTIONAL] minute (int): Minute, from 0 to 59, defaults to check the all minutes when undefined
+* [OPTIONAL] second (int): Second, from 0 to 59, defaults to check the all seconds when undefined
+* [OPTIONAL] millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined
+
+Where `2004 year, 300 doy, 15 hour, 30 minute, 7 second, 789 millisecond` becomes `2004-300T15:30:07.789`
+
+```python
+import pydar
+pydar.retrieveIDSByTime(year=2004,
+			doy=300,
+			hour=15,
+			minute=30, 
+			second=7, 
+			millisecond=789)
+```
+Output = `{'Ta': ['S01']}`
+
+If hour, minute, second, or millisecond is left undefined, will search the entire range for all possible values and can find more possible ids
+
+For a single day, some flybys have segments that are defined in one large range, but not within a smaller range
 
+```python
+import pydar
+pydar.retrieveIDSByTime(year=2005, doy=301)
+```
+Output for the entire day of 301 = `{'T8': ['S02', 'S03', 'S01']}`
 
 ```python
 import pydar
+pydar.retrieveIDSByTime(year=2005, doy=301, hour=3)
+```
+Output for the day 301 but just for hour 3 = `{'T8': ['S03', 'S01']}` (does not include S02)
+
+### retrieveIDSByTimeRange()
 
-# Extract Flyby Data Files to pydar_results/ directory: 
-pydar.extractFlybyDataImages(flyby_id='T65', resolution='D', segment_num="S01", additional_data_types_to_download=["STDR", "LBDR"])
+Retrieve a dictionary of flyby IDs and segment numbers based on a start and end datetime
+
+```
+retrieveIDSByTimeRange(start_year=None, 
+			start_doy=None,
+			start_hour=None,
+			start_minute=None, 
+			start_second=None,
+			start_millisecond=None,
+			end_year=None, 
+			end_doy=None,
+			end_hour=None,
+			end_minute=None, 
+			end_second=None,
+			end_millisecond=None)
 ```
 
-extractFlybyDataImages() will retrieve images from PDS website and saves results in a directory labeled 'pydar_results' with the flyby obsrevation number, version number, and segement number in the title (for example pydar_results/CORADR_0065_V03_S01)
+* **[REQUIRED]** start_year (int): Year for observation, range from 2004 to 2014, start_year must be less than/equal to end_year
+* **[REQUIRED]** end_year (int): Year for observation, range from 2004 to 2014, end_year must be greater than/equal to start_year
+* **[REQUIRED]** start_doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year), start_doy must be less than/equal to end_doy
+* **[REQUIRED]** end_doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year), end_doy must be less than/equal to start_doy
+* [OPTIONAL] start_hour (int): Hour, from 0 to 23 in UTC, defaults to check all hours when undefined, start_hour must be less than/equal to end_hour
+* [OPTIONAL] end_hour (int): Hour, from 0 to 23 in UTC, defaults to check all hours when undefined, end_hour must be less than/equal to start_hour
+* [OPTIONAL] start_minute (int): Minute, from 0 to 59, defaults to check all minutes when undefined, start_minute must be less than/equal to end_minute
+* [OPTIONAL] end_minute (int): Minute, from 0 to 59, defaults to check all minutes when undefined, end_minute must be greater than/equal to start_minute
+* [OPTIONAL] start_second (int): Second, from 0 to 59, defaults to check all seconds when undefined, start_second must be less than/equal to end_second
+* [OPTIONAL] end_second (int): Second, from 0 to 59, defaults to check all seconds when undefined, end_second must be greater than/equal to start_second
+* [OPTIONAL] start_millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined, start_millisecond must be less than/equal to end_millisecond
+* [OPTIONAL] end_millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined, end_millisecond must be greater than/equal to start_millisecond
 
-**convertFlybyIDToObservationNumber**
+```python
+import pydar
+pydar.retrieveIDSByTimeRange(start_year=2004,
+				start_doy=299,
+				start_hour=2,
+				start_minute=15,
+				start_second=23,
+				start_millisecond=987,
+				end_year=2005, 
+				end_doy=301,
+				end_hour=2,
+				end_minute=15,
+				end_second=23,
+				end_millisecond=987)
+```
+Output = `{'Ta': ['S01'], 'T3': ['S01'], 'T7': ['S01']}`
+
+### convertFlybyIDToObservationNumber()
 
 Converts a Titan Flyby ID (for example: 'T65') to an observation number with front padding ('T65' -> '0211')
 
 ```python
 convertFlybyIDToObservationNumber(flyby_id)
 ```
-* **[REQUIRED/OPTIONAL]** flyby_id (string): a valid flyby ID with prefix 'T'
+* **[REQUIRED]** flyby_id (string): a valid flyby ID with prefix 'T'
 
 ```python
 import pydar
-
-observation_number = convertFlybyIDToObservationNumber(flyby_id)
+observation_number = convertFlybyIDToObservationNumber(flyby_id='T65')
 ```
+Output = `0211`
 
-Observation number based on the 'Radar Data Take Number' in the cassini_flyby.csv file with front padding to ensure that all observation numbers are 4 digits long (0065 and 0211)
+Observation number based on the 'Radar Data Take Number' in the [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv) data file with front padding to ensure that all observation numbers are 4 digits long (0065 and 0211)
 
-Requires each Titan flyby ID to be a valid value the cassini_flyby.csv 
+### convertObservationNumberToFlybyID()
 
-**displayImages**
+Converts a Titan Observation Number (for example: '211' or '0211') to an flyby id ('0211' -> 'T65')
 
+```python
+convertObservationNumberToFlybyID(flyby_observation_num)
 ```
-displayImages(image_directory=None)
+* **[REQUIRED]** flyby_observation_num (string): a valid observation number
+
+```python
+import pydar
+flyby_id = pydar.convertObservationNumberToFlybyID(flyby_observation_num='211')
 ```
+Output = `T65`
 
-* **[REQUIRED]** image_directory (string): 
+Flyby ids are based on the 'Radar Data Take Number' in the [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv) data file with front padding of 'T'
 
-Displays downloaded image .IMG files (unzipped from within the .ZIP files)
+Requires each Titan flyby ID to be a valid flyby ID in [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
+
+### extractFlybyDataImages()
+
+Downloads flyby data SBDR for a selected flyby observation number or flyby id: .FMT and .TAB files (for example: [SBDR.FMT](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR.FMT) and [SBDR_15_D087_V03.TAB](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR_15_D087_V03.TAB))
+
+Downloads flyby data BIDR for a selected flyby observation number or flyby id: .LBL and .ZIP files (for example: [BIBQH80N051_D087_T016S01_V03.LBL](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.LBL) and [BIBQH80N051_D087_T016S01_V03.ZIP](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.ZIP))
 
-```python
-import pydar
-# Display all Images in pydar_results/ directory
-pydar.displayImages("pydar_results/CORADR_0065_V03_S01")
 ```
-displayImages() will plt.show() all images in the saved results directory
+extractFlybyDataImages(flyby_observation_num=None,
+			flyby_id=None,
+			segment_num=None,
+			additional_data_types_to_download=[],
+			resolution='I',
+			top_x_resolutions=None)
+```
+Either a flyby_id (for example: 'T65') or a flyby_observation_num (for example: '0035') is required. 
 
-**extractMetadata**
+Note: a flyby_id will be translated into a flyby_observation_number to access on the backend and the results will be saved under the observation number. For example, 'T65' will become observation number '0211'
 
-Extract metadata from .TAB file (using .FMT as a reference)
+* **[REQUIRED/OPTIONAL]** flyby_observation_num (string): required if flyby_id not included
+* **[REQUIRED/OPTIONAL]** flyby_id (string): required if flyby_observation_num not included
+* **[REQUIRED]** segment_num (string): a flyby includes multiple image segments (S0X) where S01 is the primary imaging segment ["S01", "S02", "S03", "S04"]
+* [OPTIONAL] resolution (String): resolution options "B", "D", "F", "H", or "I" (2, 8, 32, 128, 256 pixels/degree), defaults to highest resolution 'I'
+* [OPTIONAL] top_x_resolutions: Save the top x resolution types (5 total resolutions), will override any default resolution string
+* [OPTIONAL] additional_data_types_to_download (List of Strings): Possible options ["ABDR", "ASUM", "BIDR", "LBDR", "SBDR", "STDR"] (__NOTE__: current v1 functionality does not download any additional data types)
 
 ```python
 import pydar
-# Extract Metadata from .FMT and .TAB files
-pydar.extractMetadata()
+pydar.extractFlybyDataImages(flyby_id='T65',
+			resolution='D',
+			segment_num="S01")
 ```
 
-**readAAREADME**
+extractFlybyDataImages() will retrieve images from PDS website and saves results in a directory labeled 'pydar_results' with the flyby observation number, version number, and segment number in the title (for example pydar_results/CORADR_0065_V03_S01). Download time depends on file and resolution size but ranges from 5-30 minutes
+
+### readAAREADME()
 
 Print AAREADME.TXT to console for viewing
 
 ```
 readAAREADME(coradr_results_directory=None,
-			section_to_print=None, 
-			print_to_console=True)
+	section_to_print=None, 
+	print_to_console=True)
 ```
 
-* **[REQUIRED]** coradr_results_directory (string):
-* [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT (readme options: ['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'OBJECT', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information'])
+* **[REQUIRED]** coradr_results_directory (string): CORADAR results folder downloaded (example: "pydar_results/CORADR_0211_V03_S01/")
+* [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT, not case-sensitive 
 * [OPTIONAL] print_to_console (boolean): Print to console, defaults to true, otherwise function will return output as a string
 
+To see a list of all section_to_print options, see: `returnAAREADMEOptions()`
+
 ```python
 import pydar
-# Print AAREADME.TXT
 pydar.readAAREADME(coradr_results_directory="pydar_results/CORADR_0065_V03_S01",
-						section_to_print="Volume")
+		section_to_print="Volume")
 ```
-Output = "Volume CORADR_0065:  Titan Flyby T8, Sequence S15, Oct 27, 2005"
-
-To get the section that are avaiable for printing: returnAllAAREADMEOptions()
-
+Output = `Volume CORADR_0065:  Titan Flyby T8, Sequence S15, Oct 27, 2005`
 ```python
 import pydar
-pydar.returnAllAAREADMEOptions()
+pydar.returnAAREADMEOptions()
 ```
 
-['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information']
+Output = `['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information']`
 
-**readLBLREADME**
+### readLBLREADME()
 
 Print .LBL README to console for viewing
 
 ```
 readLBLREADME(coradr_results_directory=None,
-			section_to_print=None, 
-			print_to_console=True)
+	section_to_print=None, 
+	print_to_console=True)
 ```
 
 * **[REQUIRED]** coradr_results_directory (string):
-* [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT (readme options: ['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'OBJECT', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information'])
+* [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT, not case-sensitive
 * [OPTIONAL] print_to_console (boolean): Print to console, defaults to true, otherwise function will return output as a string
 
+To see a list of all section_to_print options, see: `returnLBLOptions()`
+
 ```python
 import pydar
-# Print .LBL README
 pydar.readLBLREADME(coradr_results_directory="pydar_results/CORADR_0035_S01/",
 		section_to_print="OBLIQUE_PROJ_X_AXIS_VECTOR")
 ```
 Output = `(0.13498322,0.00221225,-0.99084542)`
-
-To get the sections that are available for printing: returnAllLBLOptions()
 ```python
 import pydar
-pydar.returnAllLBLOptions()
+pydar.returnLBLOptions()
 ```
 <details closed>
 <summary>Line-By-Line Options (Click to view all)</summary>
 <br>
 ['PDS_VERSION_ID', 'DATA_SET_ID', 'DATA_SET_NAME', 'PRODUCER_INSTITUTION_NAME', 'PRODUCER_ID', 'PRODUCER_FULL_NAME', 'PRODUCT_ID', 'PRODUCT_VERSION_ID', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_HOST_ID', 'INSTRUMENT_NAME', 'INSTRUMENT_ID', 'TARGET_NAME', 'START_TIME', 'STOP_TIME', 'SPACECRAFT_CLOCK_START_COUNT', 'SPACECRAFT_CLOCK_STOP_COUNT', 'PRODUCT_CREATION_TIME', 'SOURCE_PRODUCT_ID', 'MISSION_PHASE_NAME', 'MISSION_NAME', 'SOFTWARE_VERSION_ID', 'FILE_NAME COMPRESSED', 'RECORD_TYPE COMPRESSED', 'ENCODING_TYPE', 'INTERCHANGE_FORMAT', 'UNCOMPRESSED_FILE_NAME', 'REQUIRED_STORAGE_BYTES', '^DESCRIPTION', 'FILE_NAME UNCOMPRESSED', 'RECORD_TYPE UNCOMPRESSED', 'RECORD_BYTES', 'FILE_RECORDS', 'LABEL_RECORDS', '^IMAGE', 'LINES', 'LINE_SAMPLES', 'SAMPLE_TYPE', 'SAMPLE_BITS', 'CHECKSUM', 'SCALING_FACTOR', 'OFFSET', 'MISSING_CONSTANT', 'NOTE', '^DATA_SET_MAP_PROJECTION', 'MAP_PROJECTION_TYPE', 'FIRST_STANDARD_PARALLEL', 'SECOND_STANDARD_PARALLEL', 'A_AXIS_RADIUS', 'B_AXIS_RADIUS', 'C_AXIS_RADIUS', 'POSITIVE_LONGITUDE_DIRECTION', 'CENTER_LATITUDE', 'CENTER_LONGITUDE', 'REFERENCE_LATITUDE', 'REFERENCE_LONGITUDE', 'LINE_FIRST_PIXEL', 'LINE_LAST_PIXEL', 'SAMPLE_FIRST_PIXEL', 'SAMPLE_LAST_PIXEL', 'MAP_PROJECTION_ROTATION', 'MAP_RESOLUTION', 'MAP_SCALE', 'MAXIMUM_LATITUDE', 'MINIMUM_LATITUDE', 'EASTERNMOST_LONGITUDE', 'WESTERNMOST_LONGITUDE', 'LINE_PROJECTION_OFFSET', 'SAMPLE_PROJECTION_OFFSET', 'OBLIQUE_PROJ_POLE_LATITUDE', 'OBLIQUE_PROJ_POLE_LONGITUDE', 'OBLIQUE_PROJ_POLE_ROTATION', 'OBLIQUE_PROJ_X_AXIS_VECTOR', 'OBLIQUE_PROJ_Y_AXIS_VECTOR', 'OBLIQUE_PROJ_Z_AXIS_VECTOR', 'LOOK_DIRECTION', 'COORDINATE_SYSTEM_NAME', 'COORDINATE_SYSTEM_TYPE']
 </details>
 <details closed>
 <summary>Section Header Options (Click to view all)</summary>
 <br>
 ['PRODUCT DESCRIPTION', 'DESCRIPTION OF COMPRESSED AND UNCOMPRESSED FILES', 'POINTERS TO START RECORDS OF OBJECTS IN FILE', 'DESCRIPTION OF OBJECTS CONTAINED IN FILE']
 </details>
 
-**retrieveFeaturesFromLatitudeLongitude**
-
-Return a list of features found at a specific latitude/longitude position
+## Use Downloaded Data
+### displayImages()
 
 ```
-retrieveFeaturesFromLatitudeLongitude(latitude=None, longitude=None)
+displayImages(image_directory=None, fig_title=None, figsize_n=6, fig_dpi=120)
 ```
-* **[REQUIRED]** latitude (float/int): Latitude (in degrees) where North = + and South = -
-* **[REQUIRED]** longitude (float/int): Longitude (in degrees) where West = + and East = -
+
+* **[REQUIRED]** image_directory (string): directory containing pydar_results with IMG file
+* [OPTIONAL] fig_title (str): figure title, defaults to filename
+* [OPTIONAL] figsize_n (int): plot dimensions, defaults to 6x6
+* [OPTIONAL] fig_dpi (int): plot dpi, defaults to 120
+
+Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
 
 ```python
 import pydar
-feature_names_list = pydar.retrieveFeaturesFromLatitudeLongitude(latitude=-72, longitude=183)
+pydar.displayImages(image_directory="pydar_results/CORADR_0065_V03_S01")
 ```
+ <p align="center">
+  <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
+</p>
 
-feature_names_list = `['Ontario Lacus']`
+Note: displayImages() will plt.show() all images in the saved results directory
 
-**retrieveFeaturesFromLatitudeLongitudeRange**
+**COMING SOON: extractMetadata**
 
-```
-retrieveFeaturesFromLatitudeLongitudeRange(northernmost_latitude=None,
-										southernmost_latitude=None,
-										easternmost_longitude=None,
-										westernmost_longitude=None)
-```
-* **[REQUIRED]** northernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, north must be greater than or equal to the south
-* **[REQUIRED]** southernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, south must be less than or euqal to the north
-* **[REQUIRED]** easternmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, west must be less than or equal to the east
-* **[REQUIRED]** westernmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, east must be greater than or equal to the west
+Extract Metadata from .FMT and .TAB files
 
-```python
-import pydar
-feature_names_list = pydar.retrieveFeaturesFromLatitudeLongitudeRange(northernmost_latitude=11,
-																southernmost_latitude=-80,
-																easternmost_longitude=339,
-																westernmost_longitude=341)
-```
-feature_names_list = `['Aaru', 'Rossak Planitia']`
+COMING SOON: Extract metadata from .TAB file (using .FMT as a reference)
 
-## TODO:
+## Developer Notes TODO:
 ### TODO Code:
-* retrieveIDSByTime() based on time or time range
 * add a colored outline around a feature when displaying as a 2D image
+* save image pixel to an array
+* extract pdr functionality to reduce overhead
+* displayImages() bug fix: 87 displays invalid integer
 * segments will be less than 99 (default to 1 - 01 is the primary imaging)
-* README for all the functions and their sections
 * progress bars print to command line (still downloading...)
+* save .IMG as .SHP for ArcGIS
 
 ### TODO Questions:
-* what is the timestamp for start/stop time: "2005-301T03:53:56.971" format? YYYY-MDDTHH:MM:SS.mms?
-* get longitude values when greater than 180 (everything is relative to west)
-* add details for what a segement_num is
+* add details for what a segment_num is
 * associate burst ID from SBDR data to BIDR data for metadata
 * save .IMG as an array of pixel values
 * save .IMG as .SHP for ArcGIS
 * project image onto Titan spheriod
 * downloadAdditionalDataTypes() does not have functionality (["ABDR", "ASUM", "LBDR", "STDR"]), decide which files to download
 
 ### TODO: Tech Debt
 * use README information to gather files for download (save computing, tech debt)
-* CSV script to be run before each pypi package update by developer not user
-* make README options for .LBL and AAREADME case-insensitive
 * set up constant config file
-* bug fix: "NOTE" in .lbl
+* Add functionality for extractFlybyDataImages(): additional_data_types_to_download
 * Include URL for access to AAREADME and .LBL readme files
-* rm -rf pydar_results/ between runs for clean image output
 * research Zenodo
 
 ### TODO: Test
 * test: pull up all passes that saw Ontario Lacus and colorcode with look angle 
 * test: pull beam information and number of looks for each pixel 
 
+## Credits
+Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
+
+Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+
 ## Bug and Feature Request
 
 Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/unaschneck/pydar/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
```

### Comparing `pydar-0.1.0/pydar/__init__.py` & `pydar-1.0.0/pydar/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,35 +13,37 @@
 # display_image.py function calls
 from .display_image import displayImages
 
 # retrieve_supplementary_backplanes.py function calls
 from .retrieve_supplementary_backplanes import extractMetadata
 
 # read_readme.py function calls
-from .read_readme import returnAllAAREADMEOptions
+from .read_readme import returnAAREADMEOptions
 from .read_readme import readAAREADME
-from .read_readme import returnAllLBLOptions
+from .read_readme import returnLBLOptions
 from .read_readme import readLBLREADME
 
-# update_csv.py function calls
-from .update_csv import csvCORADRJPLOptions
-from .update_csv import csvSwathCoverage
-from .update_csv import csvFeatureNameDetails
-
 # retrieve_ids_by_time_position.py function calls
 from .retrieve_ids_by_time_position import retrieveIDSByFeatureName
 from .retrieve_ids_by_time_position import retrieveIDSByLatitudeLongitude
 from .retrieve_ids_by_time_position import retrieveIDSByLatitudeLongitudeRange
 from .retrieve_ids_by_time_position import retrieveIDSByTime
+from .retrieve_ids_by_time_position import retrieveIDSByTimeRange
 from .retrieve_ids_by_time_position import retrieveFeaturesFromLatitudeLongitude
 from .retrieve_ids_by_time_position import retrieveFeaturesFromLatitudeLongitudeRange
 
+# sbdr_make_shapefile.py function calls
+from .sbdr_make_shapefile import sbdrMakeShapeFile
+from .sbdr_make_shapefile import field_options
+
 # error_handling.py function calls for testing
 from .error_handling import errorHandlingExtractFlybyDataImages
 from .error_handling import errorHandlingConvertFlybyIDToObservationNumber
 from .error_handling import errorHandlingConvertObservationNumberToFlybyID
 from .error_handling import errorHandlingDisplayImages
 from .error_handling import errorHandlingREADME
 from .error_handling import errorHandlingRetrieveIDSByFeature
-from .error_handling import errorHandlingRetrieveByLatitudeLongitude
-from .error_handling import errorHandlingRetrieveByLatitudeLongitudeRange
+from .error_handling import errorHandlingRetrieveIDSByLatitudeLongitude
+from .error_handling import errorHandlingRetrieveIDSByLatitudeLongitudeRange
 from .error_handling import errorHandlingRetrieveIDSByTime
+from .error_handling import errorHandlingRetrieveIDSByTimeRange
+from .error_handling import errorHandlingSbdrMakeShapeFile
```

### Comparing `pydar-0.1.0/pydar/data/cassini_flyby.csv` & `pydar-1.0.0/pydar/data/cassini_flyby.csv`

 * *Files identical despite different names*

### Comparing `pydar-0.1.0/pydar/data/coradr_jpl_options.csv` & `pydar-1.0.0/pydar/data/coradr_jpl_options.csv`

 * *Files identical despite different names*

### Comparing `pydar-0.1.0/pydar/data/feature_name_details.csv` & `pydar-1.0.0/pydar/data/feature_name_details.csv`

 * *Files identical despite different names*

### Comparing `pydar-0.1.0/pydar/data/sar_swath_details.csv` & `pydar-1.0.0/pydar/data/sar_swath_details.csv`

 * *Files identical despite different names*

### Comparing `pydar-0.1.0/pydar/data/swath_coverage_by_time_position.csv` & `pydar-1.0.0/pydar/data/swath_coverage_by_time_position.csv`

 * *Files identical despite different names*

### Comparing `pydar-0.1.0/pydar/extract_flyby_parameters.py` & `pydar-1.0.0/pydar/extract_flyby_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Extract flyby parameters from CASSINI
-import zipfile
-import os
+
+# Built in Python functions
 from datetime import datetime, timedelta
+import os
+import zipfile
 
-import pandas as pd
+# External Python libraries (installed via pip install)
+from bs4 import BeautifulSoup
 import logging
+import pandas as pd
 from urllib import request, error
-from bs4 import BeautifulSoup
 
+# Internal Pydar reference to access functions, global variables, and error handling
 import pydar
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
@@ -46,38 +50,61 @@
 			observation_number = row[1].split(" ")[1]
 			while len(observation_number) < 4:
 				observation_number = "0" + observation_number # set all radar take numbers to be four digits long: 229 -> 0229
 			return observation_number
 
 def convertObservationNumberToFlybyID(flyby_observation_num=None):
 	# convert Flyby ID to Observation Number to find data files
+	if flyby_observation_num is not None:
+		if type(flyby_observation_num) != str:
+			logger.critical("\nCRITICAL ERROR, [flyby_observation_num]: Must be a str, current type = '{0}'".format(type(flyby_observation_num)))
+			exit()
+		else:
+			while len(flyby_observation_num) < 4:
+				flyby_observation_num = "0" + flyby_observation_num # set all radar take numbers to be four digits long: 229 -> 0229
+
 	pydar.errorHandlingConvertObservationNumberToFlybyID(flyby_observation_num=flyby_observation_num)
 
 	flyby_csv_file = os.path.join(os.path.dirname(__file__), 'data', 'cassini_flyby.csv')  # get file's directory, up one level, /data/*.csv
 	flyby_dataframe = pd.read_csv(flyby_csv_file)
 	for index, row in flyby_dataframe.iterrows():
 		take_ob_num = "0" + row[1].split(" ")[1]
 		if take_ob_num == flyby_observation_num:
 			return row[0] # returns flyby ID
 
-def retrieveJPLCoradrOptions(flyby_observiation_num):
+def retrieveJPLCoradrOptions():
 	# Read JPL Options from CSV
-	jpl_coradr_options = []
 	coradr_csv_file = os.path.join(os.path.dirname(__file__), 'data', 'coradr_jpl_options.csv')  # get file's directory, up one level, /data/*.csv
 	coradr_dataframe = pd.read_csv(coradr_csv_file)
+	return coradr_dataframe
+
+def retrieveMostRecentVersionNumber(flyby_observiation_num=None):
+	# Return the CORADAR value with the most recent version from a list of possible options
+	coradr_dataframe = retrieveJPLCoradrOptions()
+	jpl_coradr_options = []
 	for index, row in coradr_dataframe.iterrows():
 		row = row.tolist()
 		jpl_coradr_options.append(row[0])
 
 	find_cordar_listing = 'CORADR_{0}'.format(flyby_observiation_num)
-	version_types_avaliable = list(filter(lambda x: find_cordar_listing in x, jpl_coradr_options))
-	more_accurate_model_number = version_types_avaliable[-1] # always choose the last and more up to date version number
-	logger.info("Most recent CORADR version is {0} from the available list {1}".format(more_accurate_model_number, version_types_avaliable))
+	version_types_available = list(filter(lambda x: find_cordar_listing in x, jpl_coradr_options))
+	more_accurate_model_number = version_types_available[-1] # always choose the last and more up to date version number (Currently, v3)
+	logger.info("Most recent CORADR version is {0} from the available list {1}".format(more_accurate_model_number, version_types_available))
 	return more_accurate_model_number
 
+def retrieveCoradrWithoutBIDR():
+	# Return a list of valid flyby observation numbers that do not contain BIDR
+	coradr_dataframe = retrieveJPLCoradrOptions()
+	coradar_without_bidr = []
+	for index, row in coradr_dataframe.iterrows():
+		if row["Is a Titan Flyby"]: # check only flybys that are valid Titan flybys
+			if "V" not in row["CORADR ID"] and row["Contains BIDR"] is False: # if not a version row, and does not contain BIDR
+				coradar_without_bidr.append(row["CORADR ID"].split("_")[1]) # store the observation number from the CORADR
+	return coradar_without_bidr
+
 def downloadAAREADME(cordar_file_name, segment_id):
 	# Download AAREADME.txt within a CORADR directory
 	aareadme_name = "AAREADME.TXT"
 	aareadme_url = "https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/{0}/{1}".format(cordar_file_name, aareadme_name)
 
 	# Retrieve a list of all elements from the base URL to download AAREADME.txt
 	logger.info("Retrieving {0} {1}".format(cordar_file_name, aareadme_name))
@@ -206,74 +233,82 @@
 
 	if flyby_id is not None and type(flyby_id) == str:
 		flyby_id = flyby_id.upper() # ensure that observation number set to capitalized 'T'
 	if flyby_observation_num is not None and type(flyby_observation_num) == str:
 		while len(flyby_observation_num) < 4:
 			flyby_observation_num = "0" + flyby_observation_num # set all radar take numbers to be four digits long: 229 -> 0229
 	if top_x_resolutions is not None:
+		logger.info("\nINFO: [top_x_resolutions] in use, overriding resolution '{0}' to save the top {1} resolutions".format(resolution, top_x_resolutions))
 		resolution = None # set default resolution to None if selecting the top x resolutions
 
 	# Error handling:
 	pydar.errorHandlingExtractFlybyDataImages(flyby_observation_num=flyby_observation_num,
 											flyby_id=flyby_id,
 											segment_num=segment_num,
 											additional_data_types_to_download=additional_data_types_to_download,
 											resolution=resolution,
 											top_x_resolutions=top_x_resolutions)
 
-	logger.info("flyby_observation_num = {0}".format(flyby_observation_num))
-	logger.info("flyby_id = {0}".format(flyby_id))
-	logger.info("segment_num = {0}".format(segment_num))
-	logger.info("additional_data_types_to_download = {0}".format(additional_data_types_to_download))
-	logger.info("resolution = {0}".format(resolution))
-	logger.info("top_x_resolutions = {0}".format(top_x_resolutions))
+	logger.debug("flyby_observation_num = {0}".format(flyby_observation_num))
+	logger.debug("flyby_id = {0}".format(flyby_id))
+	logger.debug("segment_num = {0}".format(segment_num))
+	logger.debug("additional_data_types_to_download = {0}".format(additional_data_types_to_download))
+	logger.debug("resolution = {0}".format(resolution))
+	logger.debug("top_x_resolutions = {0}".format(top_x_resolutions))
 
 	download_files = True # for debugging, does not always download files before running data
 
-	# update csv
-	days_between_checking_jpl_website = 7 # set to 0 to re-run currently without waiting
-	x_days_ago = datetime.now() - timedelta(days=days_between_checking_jpl_website)
-	filetime = datetime.fromtimestamp(os.path.getctime(os.path.join(os.path.dirname(__file__), 'data', 'coradr_jpl_options.csv')))
-	if filetime < x_days_ago:
-		# File it more than X days old
-		logger.info("file is older than {0} days, running html capture to update coradr_jpl_options.csv (will take about twenty minutes):".format(days_between_checking_jpl_website))
-		pydar.csvCORADRJPLOptions() # coradr_jpl_options.csv
-		pydar.csvSwathCoverage() # swath_coverage_by_time_position.csv
-		pydar.csvFeatureNameDetails() #feature_name_details.csv
-
 	if flyby_id is not None:  # convert flyby Id to an Observation Number
 		flyby_observation_num = convertFlybyIDToObservationNumber(flyby_id)
 
-	avaliable_flyby_id, avaliable_observation_numbers = getFlybyData()
+	# Data gaps and problems from the original downlinking and satellite location, report some special cases to user
+	no_associated_bidr_values = retrieveCoradrWithoutBIDR() # currently: ["0048", "0186", "0189", "0209", "0234"]
+	if flyby_observation_num in no_associated_bidr_values:
+		logger.info("\nINFO: due to data gaps or issues with downlinking, flyby does not have not have associated BIDR data.")
+		if flyby_observation_num == "0048":
+			logger.info("0048 (T4) did not have SAR data, only scatterometry and radiometry\n")
+		elif flyby_observation_num == "0186":
+			logger.info("0186 (T52) only has radiometery and compressed scatterometry\n")
+		elif flyby_observation_num == "0189":
+			logger.info("0189 (T53) only has radiometery and compressed scatterometry\n")
+		elif flyby_observation_num == "0209":
+			logger.info("0209 (T63) only has scatterometry and radiometry\n")
+		elif flyby_observation_num == "0234":
+			logger.info("0234 (T80) only has scatterometry and radiometry\n")
+		else:
+			logger.info("{0} does not BIDR data\n".format(flyby_observation_num)) # possible catch for new files found without BIDR
+
+	available_flyby_id, available_observation_numbers = getFlybyData()
 
-	if flyby_observation_num not in avaliable_observation_numbers:
-		logger.critical("Observation number '{0}' NOT FOUND in available observation numbers: {1}\n".format(flyby_observation_num, avaliable_observation_numbers))
+	if flyby_observation_num not in available_observation_numbers:
+		logger.critical("\nObservation number '{0}' NOT FOUND in available observation numbers: {1}\n".format(flyby_observation_num, available_observation_numbers))
 		exit()
 	else:
-		logger.debug("Observation number '{0}' FOUND in available observation numbers: {1}\n".format(flyby_observation_num, avaliable_observation_numbers))
+		logger.debug("Observation number '{0}' FOUND in available observation numbers: {1}\n".format(flyby_observation_num, available_observation_numbers))
 
 	# Download information from pds-imaging site for CORADR
-	flyby_observation_cordar_name = retrieveJPLCoradrOptions(flyby_observation_num)
+	flyby_observation_cordar_name = retrieveMostRecentVersionNumber(flyby_observation_num)
 	if not os.path.exists('pydar_results'): os.makedirs('pydar_results')
 	if not os.path.exists("pydar_results/{0}_{1}".format(flyby_observation_cordar_name, segment_num)): os.makedirs("pydar_results/{0}_{1}".format(flyby_observation_cordar_name, segment_num))
 
 	if download_files:
-		# AAREADME.TXT
+		# Download AAREADME.TXT
 		downloadAAREADME(flyby_observation_cordar_name, segment_num)
 		
-		# BIDR
-		if top_x_resolutions is not None:
-			downloadBIDRCORADRData(flyby_observation_cordar_name, segment_num, resolution_types[-top_x_resolutions:])
-		else:
-			downloadBIDRCORADRData(flyby_observation_cordar_name, segment_num, resolution)
+		# Download BIDR
+		if flyby_observation_num not in no_associated_bidr_values: # only attempt to download BIDR files for flybys that have BIDR files
+			if top_x_resolutions is not None:
+				downloadBIDRCORADRData(flyby_observation_cordar_name, segment_num, resolution_types[-top_x_resolutions:])
+			else:
+				downloadBIDRCORADRData(flyby_observation_cordar_name, segment_num, resolution)
 
-		# SBDR
+		# Download SBDR
 		downloadSBDRCORADRData(flyby_observation_cordar_name, segment_num)
 
-		# Download additional data types
+		# Download additional data types (TODO)
 		for data_type in additional_data_types_to_download:
 			if data_type not in ["BIDR", "SBDR"]: # ignore data files that have already been downloaded
 				downloadAdditionalDataTypes(flyby_observation_cordar_name, segment_num, data_type)
 
+	# No valid parameters given, empty file
 	if len(os.listdir("pydar_results/{0}_{1}".format(flyby_observation_cordar_name, segment_num))) == 0:
-		logger.critical("Unable to find any images with current parameters")
-		exit()
+		logger.critical("\npydar_results/{0}_{1} is empty. Unable to find any data files with current parameters".format(flyby_observation_cordar_name, segment_num))
```

### Comparing `pydar-0.1.0/pydar/read_readme.py` & `pydar-1.0.0/pydar/read_readme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # Read AAREADME.TXT and .LBL sections to console
+
+# Built in Python functions
 import logging
 import os
 
+# Internal Pydar reference to access functions, global variables, and error handling
 import pydar
 
 ## Logging set up for .INFO
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
+#######################################################################
+# Find relevant section to print by referencing built in options
 def determineSectionToPrint(section_to_print=None, aareadmeOrLBL=None):
 	# check which list the section_to_print is from
 	if aareadmeOrLBL == "LBL":
 		if section_to_print in lblreadme_general_options:
 			return lblreadme_general_options
 		if section_to_print in lblreadme_section_options:
 			return lblreadme_section_options
@@ -37,30 +42,34 @@
 							"File Formats",
 							"Volume Contents",
 							"Recommended DVD Drives and Driver Software",
 							"Errata and Disclaimer",
 							"Version Status",
 							"Contact Information"]
 
-def returnAllAAREADMEOptions():
+def returnAAREADMEOptions():
 	logger.info("Line-By-Line Options: {0}".format(aareadme_general_options))
 	logger.info("Section Header Options: {0}".format(aareadme_section_options))
 
 def readAAREADME(coradr_results_directory=None, section_to_print=None, print_to_console=True):
 	# Print AAREADME to console
-
 	pydar.errorHandlingREADME(coradr_results_directory=coradr_results_directory,
 							section_to_print=section_to_print,
 							print_to_console=print_to_console)
 
 	sectionList = determineSectionToPrint(section_to_print, "AAREADME")
 	if sectionList is None:
-		# TODO: error handling if section_to_print doesn't exist
-		logger.critical("Cannot find a revelant section_to_print: Invalid '{0}'".format(section_to_print))
-		exit()
+		section_to_print = section_to_print.upper() # check if the section is case-senstive
+		sectionList = determineSectionToPrint(section_to_print, "AAREADME")
+		if sectionList is None:
+			section_to_print = section_to_print.title() # check if the section is case-senstive
+			sectionList = determineSectionToPrint(section_to_print, "AAREADME")
+			if sectionList is None:
+				logger.critical("\nCRITICAL ERROR [readAAREADME]: Cannot find a revelant section_to_print: Invalid '{0}'".format(section_to_print))
+				exit()
 
 	# Define position to start console print, default to 'All' if no section is specified
 	if section_to_print is None:
 		start_index = 0
 		start_position = sectionList[start_index]
 	else:
 		start_index = sectionList.index(section_to_print)
@@ -76,18 +85,15 @@
 			if sectionList == aareadme_general_options:
 				end_position = aareadme_section_options[0] # the start of the section list is the end of the line-by-line list
 			if sectionList == aareadme_section_options:
 				end_position = None # display the last element in the list
 		else:
 			end_position = sectionList[end_index]
 
-	logger.debug("section_to_print = {0}".format(section_to_print))
-	logger.debug("start_position = {0}".format(start_position))
-	logger.debug("end_position = {0}\n".format(end_position))
-
+	# Find relevant line to print based on the starting text
 	output_string = ''
 	with open("{0}/AAREADME.TXT".format(coradr_results_directory), "r") as readme_file:
 		within_readme_section = False
 		for line in readme_file.readlines():
 			if start_position in line:
 				if start_position != "Volume":
 					within_readme_section = True
@@ -101,15 +107,15 @@
 					else:
 						if "Titan Flyby T" in line:
 							break
 			if within_readme_section:
 				if 'OBJECT' not in line and 'END' not in line:
 					output_string += line
 
-	output_string = output_string.rstrip()
+	output_string = output_string.rstrip() # remove excessive whitespace
 
 	if "=" in output_string and sectionList != aareadme_section_options:
 		output_string = (output_string.split("=")[1]).strip() # only return the value from the line (PDS_VERSION_ID       = PDS3 -> PDS3)
 	else:
 		output_string = output_string.strip() # 'Volume' option display entire row
 	if print_to_console: logger.info(output_string)
 	return output_string
@@ -196,38 +202,41 @@
 							"COORDINATE_SYSTEM_NAME",
 							"COORDINATE_SYSTEM_TYPE"]
 lblreadme_section_options = ["PRODUCT DESCRIPTION",
 							"DESCRIPTION OF COMPRESSED AND UNCOMPRESSED FILES",
 							"POINTERS TO START RECORDS OF OBJECTS IN FILE",
 							"DESCRIPTION OF OBJECTS CONTAINED IN FILE"]
 
-def returnAllLBLOptions():
+def returnLBLOptions():
 	# Print out all the .LBL options
 	logger.info("Line-By-Line Options: {0}".format(lblreadme_general_options))
 	logger.info("Section Header Options: {0}".format(lblreadme_section_options))
 
 def readLBLREADME(coradr_results_directory=None, section_to_print=None, print_to_console=True):
 	# Print .LBL to console
-
 	if section_to_print == "FILE_NAME" or section_to_print == "RECORD_TYPE":
+		# Same text used to reference both FILE_NAME and RECORD_TYPE, user needs to specify if UNCOMPRESSED or COMPRESSED file
 		logger.critical("CRITICAL ERROR: Specify {0} as either '{0} UNCOMPRESSED' or '{0} COMPRESSED'".format(section_to_print))
 		exit()
 	# Catch common mispelling: not including the ^ at the front of a line name
 	if section_to_print == "DESCRIPTION" or section_to_print == "IMAGE" or section_to_print == "DATA_SET_MAP_PROJECTION":
-		section_to_print = "^{0}".format(section_to_print) # set to specific object, easy to miss the ^
+		section_to_print = "^{0}".format(section_to_print) # sets the user's option to include the easy to miss ^
 
 	pydar.errorHandlingREADME(coradr_results_directory=coradr_results_directory,
 							section_to_print=section_to_print,
 							print_to_console=print_to_console)
 
 	sectionList = determineSectionToPrint(section_to_print, "LBL")
 	if sectionList is None:
-		# TODO: error handling if section_to_print doesn't exist
-		logger.critical("Cannot find a revelant section_to_print: Invalid '{0}'".format(section_to_print))
-		exit()
+		# check if the section is case-senstive
+		section_to_print = section_to_print.upper()
+		sectionList = determineSectionToPrint(section_to_print, "LBL")
+		if sectionList is None:
+			logger.critical("\nCRITICAL ERROR: [readLBLREADME]: Cannot find a revelant section_to_print: Invalid '{0}'".format(section_to_print))
+			exit()
 
 	# Define position to start console print, default to 'All' if no section is specified
 	if section_to_print is None:
 		start_index = 0
 		start_position = sectionList[start_index]
 	else:
 		start_index = sectionList.index(section_to_print)
@@ -259,25 +268,25 @@
 		if "UNCOMPRESSED" in section_to_print:
 			end_index = sectionList.index("FILE_RECORDS")
 			end_position = sectionList[end_index]
 
 	output_string = ''
 	lbl_file = [i for i in os.listdir(coradr_results_directory) if '.LBL' in i]
 	if len(lbl_file) != 1:
+		# error handling to check that .LBL exists
 		if len(lbl_file) == 0:
+			# No .LBL files found
 			logger.critical("No .LBL file found at {0}".format(coradr_results_directory))
 			exit()
 		if len(lbl_file) > 1:
+			# Multiple .LBL files found
 			logger.critical("Multiple .LBL file found = {0}, need to choose one to read from".format(lbl_file))
-			exit() # TODO: error handling to check that .LBL exists
-	lbl_file = lbl_file[0]
+			exit()
 
-	logger.debug("section_to_print = {0}".format(section_to_print))
-	logger.debug("start_position = {0}".format(start_position))
-	logger.debug("end_position = {0}\n".format(end_position))
+	lbl_file = lbl_file[0] # set to the LBL file, without extension
 
 	output_string = ''
 	with open("{0}/{1}".format(coradr_results_directory, lbl_file), "r") as readme_file:
 		within_readme_section = False
 		for line in readme_file.readlines():
 			if start_position in line:
 				within_readme_section = True
@@ -301,18 +310,18 @@
 			if section_to_print.split(" ")[0] in line:
 				output_string = line
 	
 	if section_to_print == "NOTE":
 		output_string = ""
 		for line in output_lines:
 			if "END_OBJECT" not in line:
-				output_string += line
+				output_string += " " + line.strip() + " " # fix additional tabs added in text file by stripping out
 			else:
 				break
 
-	output_string = output_string.rstrip()
+	output_string = output_string.rstrip() # remove excessive whitespace
+
 	if sectionList != lblreadme_section_options:
 		output_string = (output_string.split("=")[1]).strip() # only return the value from the line (PDS_VERSION_ID       = PDS3 -> PDS3)
 	if print_to_console: logger.info(output_string)
 	return output_string
-
 ########################################################################
```

### Comparing `pydar-0.1.0/pydar.egg-info/PKG-INFO` & `pydar-1.0.0/pydar.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,98 @@
 Metadata-Version: 2.1
 Name: pydar
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Python package to access, download, view, and manipulate Cassini RADAR images
 Home-page: https://github.com/unaschneck/pydar
-Author: Una Schneck (unaschneck), C. Y. Schneck (cyschneck)
+Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.0.0.tar.gz
 Description: # PYDAR
+         <p align="center">
+          <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
+        </p>
+        
         ![PyPi](https://img.shields.io/pypi/v/pydar)
-        ![license](https://img.shields.io/github/license/unaschneck/pydar)
+        ![license](https://img.shields.io/pypi/l/pydar)
         [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
+        ![PyPi-Versions](https://img.shields.io/pypi/pyversions/pydar)
+        [![update-dynamic-csv-data-files](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml)
+        [![pytests](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml)
+        
+        A Python package to access, download, view, and manipulate Cassini RADAR images in one place
+        
+        * **Find relevant flyby observation numbers/IDs for a feature, range of latitude/longitudes (or specific latitude/longitude), or a time range (or specific time)**
+        	* retrieveIDSByFeatureName()
+        	* retrieveIDSByLatitudeLongitude()
+        	* retrieveIDSByLatitudeLongitudeRange()
+        	* retrieveFeaturesFromLatitudeLongitude()
+        	* retrieveFeaturesFromLatitudeLongitudeRange()
+        	* retrieveIDSByTime()
+        	* retrieveIDSByTimeRange()
+        * **Use flyby observation numbers/IDs to retrieve flyby observation data (.FMT, .TAB, .LBL, .IMG) from SBDR and BIDR data files by default**
+        	* convertFlybyIDToObservationNumber()
+        	* convertObservationNumberToFlybyID()
+        	* extractFlybyDataImages()
+        * **Access specific observation data from AAREADME and .LBL readme information**
+        	* returnAAREADMEOptions()
+        	* readAAREADME()
+        	* returnLBLOptions()
+        	* readLBLREADME()
+        * **Display PDS image retrieved for flyby observation**
+        	* displayImages()
         
-        Python Package to access and manipulate CASSINI RADAR images in one place
+        NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.  
         
-        * Find relevant flyby observation numbers and IDs for a specific region, feature, or location
-        * Retrieve flyby observation data (.FMT, .TAB, .LBL, .IMG) from SBDR and BIDR by default
-        * Access AAREADME and .LBL readme information
-        * Display PDS image retrieved for flyby observation
+        ## Install
+        PyPi pip install at [pypi.org/project/pydar/](https://pypi.org/project/pydar/)
         
-        NOTE: This is Beta quality software that is being actively developed, use at your own risk. This project is not supported or endorsed by either JPL or NASA. The code is provided “as is”, use at your own risk.  
+        ```
+        pip install pydar
+        ```
         
-        ## Overview
-        For information on instrument specifics and acronyms refer to the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+        ## Dependencies
+        Python 3.7+
         
-        The Cassini Radar data can be found at the [PDS Imaging Node](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/). The directory is organized by [PDS standards](https://pdssbn.astro.umd.edu/howto/understand.shtml). The file format are defined in the [Small Body Node](https://pdssbn.astro.umd.edu/howto/file_types.shtml). The radar echo is stored originally as floating points in LBDR files. The SAR processors turns the LBDR files to BIDR image. The BIDR data is organized as follows:
+        Verified compatibility with Python 3.7, 3.8, and 3.9
+        ```
+        pip install -r requirements.txt
+        ```
+        Requirements will also be downloaded as part of the pip download
+        
+        ## Quickstart: PYDAR
+        
+        All Cassini data for Titan is retrieved based on flyby observation numbers or IDs, so relevant flybys can be found based on time range, latitude/longitude position, or a known feature name
+        
+        ```python
+        import pydar
+        feature_name_example = "ontario lacus"
+        flyby_ids = pydar.retrieveIDSByFeatureName(feature_name=feature_name_example)
+        ```
+        Returns a dictionary of flyby IDs (and their relevant segments) that Ontario Lacus could be found from: `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
+        
+        The relevant data files can be downloaded for any combination of these flyby IDs and segment numbers. For example, flyby ID 'T65' and segment 'S01' at resolution 'D' for 8 pixels/degree
+        ```
+        # Extract Flyby Data Files to pydar_results/ directory
+        pydar.extractFlybyDataImages(flyby_id='T65',
+        				resolution='D',
+        				segment_num="S01")
+        ```
+        Note: extractFlybyDataImages() only needs to be run once for each flyby to retrieve new data but will take some time to download
+        ```
+        # Display all Images in pydar_results/ directory
+        pydar.displayImages(image_directory="pydar_results/CORADR_0211_V03_S01")
+        ```
+         <p align="center">
+          <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
+        </p>
+        
+        ## Overview and Background
+        For information on Cassini instrument specifics and acronyms refer to the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+        
+        The Cassini Radar data can be found at the [PDS Imaging Node](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/). The directory is organized by [PDS standards](https://pdssbn.astro.umd.edu/howto/understand.shtml). The file format are defined in the [Small Body Node](https://pdssbn.astro.umd.edu/howto/file_types.shtml). The radar echo is stored originally as floating points in LBDR files. The SAR processors turn the LBDR files into BIDR image. The BIDR data is organized as follows:
         ```
         Cassini RADAR Information (CORADR_xxxx_Vxx) where xxxx is the radar data take number and Vxx is the data version number
           |_ AAREADME.txt
             Information about observation xxxx (xxxx > 0035 for Titan flybys)
           |_CALIB/
           |_CATALOG/
             BIDRDS.CAT: Information about the BIDR dataset
@@ -99,449 +164,578 @@
           |_ERRATA.txt
           |_EXTRAS/
             |_BIbcdeefggg_Dhhh_Tiii_Vnn.JPG: jpg of IMG files in DATA 
           |_INDEX/
           |_SOFTWARE/
           |_VOLDESC.CAT <--- VERSION INFORMATION LISTED HERE ('VOLUME_VERSION_ID' = "Version 1", "Version 2", "Version 3") and in filename
         ```
+        .IMG files can be viewed using the [planetary images library](https://planetaryimage.readthedocs.io/_/downloads/en/latest/pdf/) or via `pydar.displayImages()`
         
-        .IMG files can be viewed using the [planetary images library](https://planetaryimage.readthedocs.io/_/downloads/en/latest/pdf/)
         ### Download Time
-        Download time varies depending on the number and size of files of interest. On average, most single feature downloads take between 2-5 minutes to download.
+        Download time for data files vary when using `pydar.extractFlybyDataImages()` and depends on the number and size of files of interest. On average, most single feature downloads take between 5-30 minutes to download, but can be longer for higher resolution files.
         
         ![image](https://user-images.githubusercontent.com/24469269/211881026-5bab329c-cf0d-416b-bedc-6d466b77b1f5.png)
         ([Cassini Radar Volume SIS, Version 2.1](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0284/DOCUMENT/VOLSIS.PDF) Table 1, pg. 3)
-        ### Cross-Reference Table for Observations and Flybys
-        The Titan flybys ID is not used in the naming convention for the CORADR filenames. The Titan flyby information is contained in the BIDR filenames and in the VOLDESC.CAT under 'Description' and can be found using the following cross-reference table: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
         
-        ```
-        Flyby ID Cross Reference Table
-        Prime Mission and Extended Mission
-        
-        Column 1: Titan flyby id
-        Column 2: Radar Data Take Number
-        Column 3: Sequence number
-        Column 4: Orbit Number/ID
-        
-        Ta   DTN 035   S05 Rev 0A
-        T3   DTN 045   S08 Rev 03
-        T4   DTN 048   S09 Rev 04
-        T7   DTN 059   S14 Rev 14
-        T8   DTN 065   S15 Rev 17
-        
-        ...
-        ```
+        ### Cross-Reference Table for Observations and Flybys
+        The Titan flyby IDs (e.g. 'T65') are not used in the naming convention for the CORADR filenames. Instead, all files are referred to by their observation number (e.g. '0211'). The Titan flyby information is contained in the BIDR filenames and in the VOLDESC.CAT under 'Description' and can be found using the following cross-reference table: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
         
-        To convert between a Titan Flyby ID and an observation number: `pydar.convertFlybyIDToObservationNumber(flyby_id)`
+        To convert between a Titan Flyby ID and an observation number use either `pydar.convertFlybyIDToObservationNumber(flyby_id)` or `pydar.convertObservationNumberToFlybyID(flyby_observation_num)`
         
         ### Observation Information as filename
-        The data filename contains a lot of information about the observation 
+        The data filename contains a lot of information about the observation
         
         (EXAMPLE) Filename: "BIBQD05S184_D065_T008S03_V03"
         
         - BI = BIDR data
         - B = data in dB normalized
-        - Q = obliquid dylindrical
+        - Q = oblique cylindrical
         - D = 8 pixels/degree
         - 05 = absolute value of latitude at center rounded to nearest degree
         - S = hemisphere of center of file (Southern)
         - 184 = West longitude at center of file rounded to nearest degree
         - D065 = 2-digit data take ID aka observation counter with left-padded zeros
         - T008 = 3-digit Titan flyby with left-padding
         - S03 = 2-digit segment number (00-99)
         - V03 = 2-digit version number (01-99)
         
-        BIBQD05S184_D065_T008S03_V03.JPG:
+        Image file from BIBQD05S184_D065_T008S03_V03.JPG:
         
         ![BIFQI10S251_D065_T008S01_V03](https://user-images.githubusercontent.com/24469269/210164143-427003ed-0043-45b4-a80f-8e9ddf28543a.jpg)
         
         ### Volume Version of Data
         
-        Some passes have multiple versions of the data.
-        
-        * Version 1 (V01) was the first archived version of the data and assumed Titan had zero obliquity, which resulted in misregistration between passes
-        
-        * Version 2 (V02) used a Titan spin model that reduced misregistration error 
+        Some passes have multiple versions of the data, up to 3 different versions currently.
         
-        * Version 3 (V03) used a long-term, accurate spin model for Titan along with other improvements
+        * **Version 1 (V01)** was the first archived version of the data and assumed Titan had zero obliquity, which resulted in misregistration between passes
+        * **Version 2 (V02)** used a Titan spin model that reduced misregistration error 
+        * **Version 3 (V03)** used a long-term, accurate spin model for Titan along with other improvements
         
         Only some Titan passes produced all of the version numbers.
         
         * TA-T25 : V01, V02, V03
         
         * $\gt$ T28: V02, V03
         
         * T108-T126: labeled only once as V02 but is actually V03
         
-        The version number is listed in the filenanme and in VOLDESC.CAT under the 'VOLUME_VERSION_ID'
+        The version number is listed in the filename and in VOLDESC.CAT under the 'VOLUME_VERSION_ID'
         
-        *Version 3 is the latest and preferred version*
+        _**Version 3 is currently the latest and preferred version and will be the version included when downloaded**_
         
         Example:
         
         Version 1 is named BIFQI48N071_D035_T00A_V01.IMG
         
         Version 2 is named BIFQI49N071_D035_T00AS01_V02.IMG
         
         Version 3 is named BIFQI49N071_D035_T00AS01_V03.IMG
         
         ### Segment Number of Data
         A single flyby can produce multiple image segments (Sxx). *S01 is the primary imaging segment* with other segments referring to periods in the flyby when the instrument went to/from altimetry/SAR/HiSAR or weird pointing profiles.  
         
         ![image](https://user-images.githubusercontent.com/24469269/210197286-c059ffed-281d-46c7-911a-f86c3bf7ea28.png)
-        Credit: Cassini Radar User Guide (Wall et al. 2019, pg.16)
-        ## Documentation
+        *Credit: Cassini Radar User Guide (Wall et al. 2019, pg.16)*
+        
+        ## Backend Data Files
+        
+        ### Dynamically Updated Backend Files
+        
+        Pydar includes multiple scripts to web scrape from relevant URLs to generate some of the backend data files
+        
+        Changes in the relevant URLs are checked once a month via Github Actions to keep csv files up to date and any changes found will be bundled into the subsequent release
+        
+        **coradr_jpl_options.csv**
+        
+        Contains all the CORADR IDs and available data types from [pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter)
+        
+        Headers: ["CORADR ID", "Is a Titan Flyby", "Contains ABDR", "Contains ASUM", "Contains BIDR", "Contains LBDR", "Contains SBDR", "Contains STDR"]
         
-        ## Data Files
+        View data file: [coradr_jpl_options.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/coradr_jpl_options.csv)
+        
+        **swath_coverage_by_time_position.csv**
+        
+        Contains all the information for .LBL files within all CORADR ID pages (for each segment and resolution file)
+        
+        Collected from URLs matching: pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/[CORADAR_ID]/DATA/BIDR/
+        
+        Headers: ["CORADR ID", "FLYBY ID", "SEGMENT NUMBER", "FILENAME", "DATE TYPE SYMBOL", "DATE TYPE", "RESOLUTION (pixels/degrees)", "TARGET_NAME", "MAXIMUM_LATITUDE (Degrees)", "MINIMUM_LATITUDE (Degrees)", "EASTERNMOST_LONGITUDE (Degrees)", "WESTERNMOST_LONGITUDE (Degrees)", "START_TIME", "STOP_TIME"]
+        
+        View data file: [swath_coverage_by_time_position.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/swath_coverage_by_time_position.csv)
         
         **feature_name_details.csv**
         
-        List of Features on Titan with names with their associated position and the origin of their name. Taken from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/Feature/6981)
+        Contains all named features on Titan with their furthest latitude/longitude position and origin of name
         
-        ## SBDR Files
-        [SBDR column descriptions](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0045/DOCUMENT/BODPSIS.PDF)
+        Collected from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
         
-        Total width of the RADAR swath is created by combining the five individual sub-swaths, where the center beam is the highest gain
-        ![image](https://user-images.githubusercontent.com/24469269/211431884-c201ac74-114a-4c17-b95a-f9edf0178d2e.png)
-        (_The Cassini Huygens Mission: Orbiter Remote Sensing Observation 2004_)
+        Headers: ["Feature Name", "Northernmost Latitude", "Southernmost Latitude", "Easternmost Longitude", "Westernmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
         
-        ```
-        test_file = "SBDR_15_D065_V03.TAB"
-        SBDR_FILE = pdr.read(test_file)
-        print("Table options: {0}".format(SBDR_FILE.keys()))
-        ```
+        View data file: [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
+        
+        ### Static Data Files
+        
+        **cassini_flyby.csv**
+        
+        Reference for converting between a Titan Flyby ID (e.g. "T7") and its Observation Number (e.g. "059") (and back)
+        
+        Headers: ["Titan flyby id", "Radar Data Take Number", "Sequence number", "Orbit Number/ID"]
+        
+        View data file: [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
+        
+        **sar_swath_details.csv**
+        
+        Currently unused, but will potentially be used in the future for incidence angle, polarization, azimuth, SAR range resolution, SAR azimuth resolution, and number of looks
+        
+        Converted to a static csv file from the Cassini User Guide (pg. 136-139)
+        
+        View data file: [sar_swath_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/sar_swath_details.csv)
         
         ## BIDR and SBDR Files
         Note: "CORADR_0048", "CORADR_0186", "CORADR_0189", "CORADR_0209", "CORADR_0234" do not have associated BIDR values.
         
         There are data gaps and problems from the original downlinking and satellite location
         
-        CORADR_0048 (T4) did not have SAR data, only scatterometry and radiometery because of telemetry reasons in the handbook
+        CORADR_0048 (T4) did not have SAR data, only scatterometry and radiometry because of telemetry reasons in the handbook
         
-        CORADR_0186 (T52) only have rad and compressed scatterometry
+        CORADR_0186 (T52) only have radiometry and compressed scatterometry
         
-        CORADR_189 (T53) only has rad and compressed scatterometry because of what appears to be a downlink problem
+        CORADR_0189 (T53) only has radiometry and compressed scatterometry because of what appears to be a downlink problem
         
         CORADR_0209 (T63) only has scatterometry and radiometry
         
         CORADR_0234 (T80) only has scatterometry and radiometry 
-        ## Dependencies
-        Python 3.9
-        ```
-        pip3 install -r requirements.txt
-        ```
-        ## Install
-        PyPi pip install at [pypi.org/project/pydar/](https://pypi.org/project/pydar/)
         
-        ```
-        pip install pydar
-        ```
+        ## Coming Soon: SBDR Files
+        Total width of the RADAR swath is created by combining the five individual sub-swaths, where the center beam is the highest gain
+        ![image](https://user-images.githubusercontent.com/24469269/211431884-c201ac74-114a-4c17-b95a-f9edf0178d2e.png)
+        (_The Cassini Huygens Mission: Orbiter Remote Sensing Observation 2004_)
+        
+        [SBDR column descriptions](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0045/DOCUMENT/BODPSIS.PDF)
         
-        ## Examples
+        ## Retrieve Data from CASSINI Function Calls
         
-        To collect flyby information and images from a feature on Titan, start by selecting a feature, for example: "Ontario Lacus"
+        To collect flyby information and images for the latitude/longitude range of a named feature on Titan
         
-        **retrieveIDSByFeatureName**
+        ### retrieveIDSByFeatureName()
         
-        Retrieve a list of flyby IDs with their associated segments based on a feature name from titan
+        Retrieve a list of flyby IDs with their associated segment numbers based on a feature name from Titan
         
         ```python
         retrieveIDSByFeatureName(feature_name=None)
         ```
-        * **[REQUIRED]** feature_name (string): Feature name on Titan to give flyby ids and segments, not case-sensitive
+        * **[REQUIRED]** feature_name (string): Feature name on Titan, not case-sensitive
         
         Feature names are retrieved from [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
         <details closed>
         <summary>List of Valid Feature Names (Click to view all)</summary>
         <br>
         ['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
         </details>
         
         ```python
         import pydar
         pydar.retrieveIDSByFeatureName(feature_name="Ontario Lacus")
         ```
-        Output = `{'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
+        Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
         
-        **retrieveIDSByLatitudeLongitude**
+        ### retrieveIDSByLatitudeLongitude()
         
         Retrieve a list of flyby IDs with their associated segments based on specific latitude and longitude
         
         ```python
         retrieveIDSByLatitudeLongitude(latitude=None, longitude=None)
         ```
-        * **[REQUIRED]** latitude (float/int): Latitude (in degrees) where North = + and South = -
-        * **[REQUIRED]** longitude (float/int): Longitude (in degrees) where West = + and East = -
+        * **[REQUIRED]** latitude (float/int): Latitude (in degrees), range from -90° to 90°
+        * **[REQUIRED]** longitude (float/int): Longitude (in degrees), range from 0° to 360°
         
         ```python
         import pydar
-        pydar.retrieveIDSByLatitudeLongitude(latitude=10, longitude=10)
+        pydar.retrieveIDSByLatitudeLongitude(latitude=-80, longitude=170)
         ```
-        Output = `{'T19': ['S01'], 'T29': ['S01'], 'T55': ['S01'], 'T56': ['S01'], 'T57': ['S01'], 'T58': ['S01'], 'T64': ['S01'], 'T83': ['S02'], 'T84': ['S02'], 'T92': ['S01'], 'T98': ['S02'], 'T104': ['S01']}`
+        Output = `{'T39': ['S06', 'S05', 'S01'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S03'], 'T56': ['S01'], 'T57': ['S01'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
         
-        **retrieveIDSByLatitudeLongitudeRange**
+        ### retrieveIDSByLatitudeLongitudeRange()
+        
+        Retrieve a list of flyby IDs with their associated segments based on range of latitudes and longitudes
         
         ```python
-        retrieveIDSByLatitudeLongitudeRange(northernmost_latitude=None,
-        				southernmost_latitude=None,
-        				easternmost_longitude=None,
-        				westernmost_longitude=None)
+        retrieveIDSByLatitudeLongitudeRange(min_latitude=None,
+        				max_latitude=None,
+        				min_longitude=None,
+        				max_longitude=None)
         ```
-        * **[REQUIRED]** northernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, north must be greater than or equal to the south
-        * **[REQUIRED]** southernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, south must be less than or euqal to the north
-        * **[REQUIRED]** easternmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, west must be less than or equal to the east
-        * **[REQUIRED]** westernmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, east must be greater than or equal to the west
+        * **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be greater than or equal to the max_latitude, range from -90° to 90°
+        * **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be less than or equal to the min_latitude, range from -90° to 90°
+        * **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
+        * **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude be greater than or equal to the min_longitude, range from 0° to 360°
         
         ```python
-        retrieveIDSByLatitudeLongitudeRange(northernmost_latitude=15,
-        				southernmost_latitude=10,
-        				easternmost_longitude=12,
-        				westernmost_longitude=17)
+        import pydar
+        pydar.retrieveIDSByLatitudeLongitudeRange(min_latitude=-82,
+        					max_latitude=-72,
+        					min_longitude=183,
+        					max_longitude=185)
         ```
-        Output = `{'T19': ['S01'], 'T29': ['S01'], 'T55': ['S01'], 'T56': ['S01'], 'T57': ['S01'], 'T64': ['S01'], 'T83': ['S02'], 'T84': ['S02'], 'T92': ['S01'], 'T98': ['S02'], 'T104': ['S01']}`
+        Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
         
-        Ontario Lacus was visible in four swath observations: T57, T58, T65, T98 [(Page 163)](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf).
+        ### retrieveFeaturesFromLatitudeLongitude()
         
-        To access flyby of Ontario, first specify a flyby. For this example, Ontario Lacus with the features:
+        Return a list of features found at a specific latitude/longitude position
         
-        * Titan flyby id: 'T65'
-        * resolution: 'D' (8 pixels/degree)
-        * Main imaging segement 1: 'S01'
+        ```
+        retrieveFeaturesFromLatitudeLongitude(latitude=None, longitude=None)
+        ```
+        * **[REQUIRED]** latitude (float/int): Latitude (in degrees), range from -90° to 90°
+        * **[REQUIRED]** longitude (float/int): Longitude (in degrees), range from 0° to 360°
         
-        **extractFlybyDataImages()**
+        ```python
+        import pydar
+        pydar.retrieveFeaturesFromLatitudeLongitude(latitude=-72, longitude=183)
+        ```
+        
+        Output = `['Ontario Lacus', 'Rossak Planitia']`
         
-        Downloads flyby data SBDR: .FMT and .TAB files (for example: [SBDR.FMT](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR.FMT) and [SBDR_15_D087_V03.TAB](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR_15_D087_V03.TAB))
+        ### retrieveFeaturesFromLatitudeLongitudeRange()
         
-        Downloads flyby data BIDR: .LBL and .ZIP files (for example: [BIBQH80N051_D087_T016S01_V03.LBL](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.LBL) and [BIBQH80N051_D087_T016S01_V03.ZIP](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.ZIP))
+        Return a list of features found at a range of latitude/longitude positions
         
         ```
-        extractFlybyDataImages(flyby_observation_num=None,
-        			flyby_id=None,
-        			segment_num=None,
-        			additional_data_types_to_download=[],
-        			resolution='I',
-        			top_x_resolutions=None)
+        retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=None,
+        					max_latitude=None,
+        					min_longitude=None,
+        					max_longitude=None)
         ```
-        Either a flyby_id (for example: 'T65') or a flyby_observation_num (for example: '0065') is required. A flyby_id will be translated into a flyby_observation_number to access on the backend and the results will be saved under the observation number. 'T65' will become observation number '0021'
+        * **[REQUIRED]** min_latitude (float/int): Latitude (in degrees) where min_latitude must be less than or equal to the max_latitude, range from -90° to 90°
+        * **[REQUIRED]** max_latitude (float/int): Latitude (in degrees) where max_latitude must be greater than or equal to the min_latitude, range from -90° to 90°
+        * **[REQUIRED]** min_longitude (float/int): Longitude (in degrees) where min_longitude must be less than or equal to the max_longitude, range from 0° to 360°
+        * **[REQUIRED]** max_longitude (float/int): Longitude (in degrees) where max_longitude must be greater than or equal to the min_longitude, range from 0° to 360°
         
-        * **[REQUIRED/OPTIONAL]** flyby_observation_num (string): required if flyby_id not included
-        * **[REQUIRED/OPTIONAL]** flyby_id (string): required if flyby_observation_num not included
-        * **[REQUIRED]** segment_num (string): 
-        * [OPTIONAL] additional_data_types_to_download (List of Strings): Possible options ["ABDR", "ASUM", "BIDR", "LBDR", "SBDR", "STDR"]
-        * [OPTIONAL] resolution (String): resolution options "B", "D", "F", "H", or "I" (2, 8, 32, 128, 256 pixels/degree), defaults to highest resolution 'I'
-        * [OPTIONAL] top_x_resolutions: Save the top x resolution types (5 total resolutions)
+        ```python
+        import pydar
+        
+        pydar.retrieveFeaturesFromLatitudeLongitudeRange(min_latitude=-82,
+        						max_latitude=-72,
+        						min_longitude=183,
+        						max_longitude=190)
+        ```
+        Output = `['Crveno Lacus', 'Ontario Lacus', 'Romo Planitia', 'Rossak Planitia', 'Saraswati Flumen']`
+        
+        ### retrieveIDSByTime()
+        
+        Retrieve a dictionary of flyby IDs and segment numbers based on a specific timestamp
+        
+        ```
+        retrieveIDSByTime(year=None,
+        		doy=None,
+        		hour=None,
+        		minute=None,
+        		second=None,
+        		millisecond=None)
+        ```
+        * **[REQUIRED]** year (int): Year for observation, range from 2004 to 2014
+        * **[REQUIRED]** doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year)
+        * [OPTIONAL] hour (int): Hour, from 0 to 23 in UTC, defaults to 0 when undefined
+        * [OPTIONAL] minute (int): Minute, from 0 to 59, defaults to check the all minutes when undefined
+        * [OPTIONAL] second (int): Second, from 0 to 59, defaults to check the all seconds when undefined
+        * [OPTIONAL] millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined
+        
+        Where `2004 year, 300 doy, 15 hour, 30 minute, 7 second, 789 millisecond` becomes `2004-300T15:30:07.789`
+        
+        ```python
+        import pydar
+        pydar.retrieveIDSByTime(year=2004,
+        			doy=300,
+        			hour=15,
+        			minute=30, 
+        			second=7, 
+        			millisecond=789)
+        ```
+        Output = `{'Ta': ['S01']}`
+        
+        If hour, minute, second, or millisecond is left undefined, will search the entire range for all possible values and can find more possible ids
+        
+        For a single day, some flybys have segments that are defined in one large range, but not within a smaller range
         
+        ```python
+        import pydar
+        pydar.retrieveIDSByTime(year=2005, doy=301)
+        ```
+        Output for the entire day of 301 = `{'T8': ['S02', 'S03', 'S01']}`
         
         ```python
         import pydar
+        pydar.retrieveIDSByTime(year=2005, doy=301, hour=3)
+        ```
+        Output for the day 301 but just for hour 3 = `{'T8': ['S03', 'S01']}` (does not include S02)
+        
+        ### retrieveIDSByTimeRange()
         
-        # Extract Flyby Data Files to pydar_results/ directory: 
-        pydar.extractFlybyDataImages(flyby_id='T65', resolution='D', segment_num="S01", additional_data_types_to_download=["STDR", "LBDR"])
+        Retrieve a dictionary of flyby IDs and segment numbers based on a start and end datetime
+        
+        ```
+        retrieveIDSByTimeRange(start_year=None, 
+        			start_doy=None,
+        			start_hour=None,
+        			start_minute=None, 
+        			start_second=None,
+        			start_millisecond=None,
+        			end_year=None, 
+        			end_doy=None,
+        			end_hour=None,
+        			end_minute=None, 
+        			end_second=None,
+        			end_millisecond=None)
         ```
         
-        extractFlybyDataImages() will retrieve images from PDS website and saves results in a directory labeled 'pydar_results' with the flyby obsrevation number, version number, and segement number in the title (for example pydar_results/CORADR_0065_V03_S01)
+        * **[REQUIRED]** start_year (int): Year for observation, range from 2004 to 2014, start_year must be less than/equal to end_year
+        * **[REQUIRED]** end_year (int): Year for observation, range from 2004 to 2014, end_year must be greater than/equal to start_year
+        * **[REQUIRED]** start_doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year), start_doy must be less than/equal to end_doy
+        * **[REQUIRED]** end_doy (int): Day of the year, from 0 to 365 (where January 10 = 10) (__Note__: 'doy' not 'day' for days of the year), end_doy must be less than/equal to start_doy
+        * [OPTIONAL] start_hour (int): Hour, from 0 to 23 in UTC, defaults to check all hours when undefined, start_hour must be less than/equal to end_hour
+        * [OPTIONAL] end_hour (int): Hour, from 0 to 23 in UTC, defaults to check all hours when undefined, end_hour must be less than/equal to start_hour
+        * [OPTIONAL] start_minute (int): Minute, from 0 to 59, defaults to check all minutes when undefined, start_minute must be less than/equal to end_minute
+        * [OPTIONAL] end_minute (int): Minute, from 0 to 59, defaults to check all minutes when undefined, end_minute must be greater than/equal to start_minute
+        * [OPTIONAL] start_second (int): Second, from 0 to 59, defaults to check all seconds when undefined, start_second must be less than/equal to end_second
+        * [OPTIONAL] end_second (int): Second, from 0 to 59, defaults to check all seconds when undefined, end_second must be greater than/equal to start_second
+        * [OPTIONAL] start_millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined, start_millisecond must be less than/equal to end_millisecond
+        * [OPTIONAL] end_millisecond (int): Milliscond, from 0 to 999, defaults to check all milliseconds when undefined, end_millisecond must be greater than/equal to start_millisecond
         
-        **convertFlybyIDToObservationNumber**
+        ```python
+        import pydar
+        pydar.retrieveIDSByTimeRange(start_year=2004,
+        				start_doy=299,
+        				start_hour=2,
+        				start_minute=15,
+        				start_second=23,
+        				start_millisecond=987,
+        				end_year=2005, 
+        				end_doy=301,
+        				end_hour=2,
+        				end_minute=15,
+        				end_second=23,
+        				end_millisecond=987)
+        ```
+        Output = `{'Ta': ['S01'], 'T3': ['S01'], 'T7': ['S01']}`
+        
+        ### convertFlybyIDToObservationNumber()
         
         Converts a Titan Flyby ID (for example: 'T65') to an observation number with front padding ('T65' -> '0211')
         
         ```python
         convertFlybyIDToObservationNumber(flyby_id)
         ```
-        * **[REQUIRED/OPTIONAL]** flyby_id (string): a valid flyby ID with prefix 'T'
+        * **[REQUIRED]** flyby_id (string): a valid flyby ID with prefix 'T'
         
         ```python
         import pydar
-        
-        observation_number = convertFlybyIDToObservationNumber(flyby_id)
+        observation_number = convertFlybyIDToObservationNumber(flyby_id='T65')
         ```
+        Output = `0211`
         
-        Observation number based on the 'Radar Data Take Number' in the cassini_flyby.csv file with front padding to ensure that all observation numbers are 4 digits long (0065 and 0211)
+        Observation number based on the 'Radar Data Take Number' in the [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv) data file with front padding to ensure that all observation numbers are 4 digits long (0065 and 0211)
         
-        Requires each Titan flyby ID to be a valid value the cassini_flyby.csv 
+        ### convertObservationNumberToFlybyID()
         
-        **displayImages**
+        Converts a Titan Observation Number (for example: '211' or '0211') to an flyby id ('0211' -> 'T65')
         
+        ```python
+        convertObservationNumberToFlybyID(flyby_observation_num)
         ```
-        displayImages(image_directory=None)
+        * **[REQUIRED]** flyby_observation_num (string): a valid observation number
+        
+        ```python
+        import pydar
+        flyby_id = pydar.convertObservationNumberToFlybyID(flyby_observation_num='211')
         ```
+        Output = `T65`
         
-        * **[REQUIRED]** image_directory (string): 
+        Flyby ids are based on the 'Radar Data Take Number' in the [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv) data file with front padding of 'T'
         
-        Displays downloaded image .IMG files (unzipped from within the .ZIP files)
+        Requires each Titan flyby ID to be a valid flyby ID in [cassini_flyby.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/cassini_flyby.csv)
+        
+        ### extractFlybyDataImages()
+        
+        Downloads flyby data SBDR for a selected flyby observation number or flyby id: .FMT and .TAB files (for example: [SBDR.FMT](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR.FMT) and [SBDR_15_D087_V03.TAB](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/SBDR/SBDR_15_D087_V03.TAB))
+        
+        Downloads flyby data BIDR for a selected flyby observation number or flyby id: .LBL and .ZIP files (for example: [BIBQH80N051_D087_T016S01_V03.LBL](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.LBL) and [BIBQH80N051_D087_T016S01_V03.ZIP](https://pds-imaging.jpl.nasa.gov/data/cassini/cassini_orbiter/CORADR_0087_V03/DATA/BIDR/BIBQH80N051_D087_T016S01_V03.ZIP))
         
-        ```python
-        import pydar
-        # Display all Images in pydar_results/ directory
-        pydar.displayImages("pydar_results/CORADR_0065_V03_S01")
         ```
-        displayImages() will plt.show() all images in the saved results directory
+        extractFlybyDataImages(flyby_observation_num=None,
+        			flyby_id=None,
+        			segment_num=None,
+        			additional_data_types_to_download=[],
+        			resolution='I',
+        			top_x_resolutions=None)
+        ```
+        Either a flyby_id (for example: 'T65') or a flyby_observation_num (for example: '0035') is required. 
         
-        **extractMetadata**
+        Note: a flyby_id will be translated into a flyby_observation_number to access on the backend and the results will be saved under the observation number. For example, 'T65' will become observation number '0211'
         
-        Extract metadata from .TAB file (using .FMT as a reference)
+        * **[REQUIRED/OPTIONAL]** flyby_observation_num (string): required if flyby_id not included
+        * **[REQUIRED/OPTIONAL]** flyby_id (string): required if flyby_observation_num not included
+        * **[REQUIRED]** segment_num (string): a flyby includes multiple image segments (S0X) where S01 is the primary imaging segment ["S01", "S02", "S03", "S04"]
+        * [OPTIONAL] resolution (String): resolution options "B", "D", "F", "H", or "I" (2, 8, 32, 128, 256 pixels/degree), defaults to highest resolution 'I'
+        * [OPTIONAL] top_x_resolutions: Save the top x resolution types (5 total resolutions), will override any default resolution string
+        * [OPTIONAL] additional_data_types_to_download (List of Strings): Possible options ["ABDR", "ASUM", "BIDR", "LBDR", "SBDR", "STDR"] (__NOTE__: current v1 functionality does not download any additional data types)
         
         ```python
         import pydar
-        # Extract Metadata from .FMT and .TAB files
-        pydar.extractMetadata()
+        pydar.extractFlybyDataImages(flyby_id='T65',
+        			resolution='D',
+        			segment_num="S01")
         ```
         
-        **readAAREADME**
+        extractFlybyDataImages() will retrieve images from PDS website and saves results in a directory labeled 'pydar_results' with the flyby observation number, version number, and segment number in the title (for example pydar_results/CORADR_0065_V03_S01). Download time depends on file and resolution size but ranges from 5-30 minutes
+        
+        ### readAAREADME()
         
         Print AAREADME.TXT to console for viewing
         
         ```
         readAAREADME(coradr_results_directory=None,
-        			section_to_print=None, 
-        			print_to_console=True)
+        	section_to_print=None, 
+        	print_to_console=True)
         ```
         
-        * **[REQUIRED]** coradr_results_directory (string):
-        * [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT (readme options: ['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'OBJECT', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information'])
+        * **[REQUIRED]** coradr_results_directory (string): CORADAR results folder downloaded (example: "pydar_results/CORADR_0211_V03_S01/")
+        * [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT, not case-sensitive 
         * [OPTIONAL] print_to_console (boolean): Print to console, defaults to true, otherwise function will return output as a string
         
+        To see a list of all section_to_print options, see: `returnAAREADMEOptions()`
+        
         ```python
         import pydar
-        # Print AAREADME.TXT
         pydar.readAAREADME(coradr_results_directory="pydar_results/CORADR_0065_V03_S01",
-        						section_to_print="Volume")
+        		section_to_print="Volume")
         ```
-        Output = "Volume CORADR_0065:  Titan Flyby T8, Sequence S15, Oct 27, 2005"
-        
-        To get the section that are avaiable for printing: returnAllAAREADMEOptions()
-        
+        Output = `Volume CORADR_0065:  Titan Flyby T8, Sequence S15, Oct 27, 2005`
         ```python
         import pydar
-        pydar.returnAllAAREADMEOptions()
+        pydar.returnAAREADMEOptions()
         ```
         
-        ['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information']
+        Output = `['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information']`
         
-        **readLBLREADME**
+        ### readLBLREADME()
         
         Print .LBL README to console for viewing
         
         ```
         readLBLREADME(coradr_results_directory=None,
-        			section_to_print=None, 
-        			print_to_console=True)
+        	section_to_print=None, 
+        	print_to_console=True)
         ```
         
         * **[REQUIRED]** coradr_results_directory (string):
-        * [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT (readme options: ['PDS_VERSION_ID', 'RECORD_TYPE', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_NAME', 'OBJECT', 'PUBLICATION_DATE', 'NOTE', 'END_OBJECT', 'Volume', 'Introduction', 'Disk Format', 'File Formats', 'Volume Contents', 'Recommended DVD Drives and Driver Software', 'Errata and Disclaimer', 'Version Status', 'Contact Information'])
+        * [OPTIONAL] section_to_print (string): Specify a section to print to console from the AAREADME, defaults to print the entire AAREADME.TXT, not case-sensitive
         * [OPTIONAL] print_to_console (boolean): Print to console, defaults to true, otherwise function will return output as a string
         
+        To see a list of all section_to_print options, see: `returnLBLOptions()`
+        
         ```python
         import pydar
-        # Print .LBL README
         pydar.readLBLREADME(coradr_results_directory="pydar_results/CORADR_0035_S01/",
         		section_to_print="OBLIQUE_PROJ_X_AXIS_VECTOR")
         ```
         Output = `(0.13498322,0.00221225,-0.99084542)`
-        
-        To get the sections that are available for printing: returnAllLBLOptions()
         ```python
         import pydar
-        pydar.returnAllLBLOptions()
+        pydar.returnLBLOptions()
         ```
         <details closed>
         <summary>Line-By-Line Options (Click to view all)</summary>
         <br>
         ['PDS_VERSION_ID', 'DATA_SET_ID', 'DATA_SET_NAME', 'PRODUCER_INSTITUTION_NAME', 'PRODUCER_ID', 'PRODUCER_FULL_NAME', 'PRODUCT_ID', 'PRODUCT_VERSION_ID', 'INSTRUMENT_HOST_NAME', 'INSTRUMENT_HOST_ID', 'INSTRUMENT_NAME', 'INSTRUMENT_ID', 'TARGET_NAME', 'START_TIME', 'STOP_TIME', 'SPACECRAFT_CLOCK_START_COUNT', 'SPACECRAFT_CLOCK_STOP_COUNT', 'PRODUCT_CREATION_TIME', 'SOURCE_PRODUCT_ID', 'MISSION_PHASE_NAME', 'MISSION_NAME', 'SOFTWARE_VERSION_ID', 'FILE_NAME COMPRESSED', 'RECORD_TYPE COMPRESSED', 'ENCODING_TYPE', 'INTERCHANGE_FORMAT', 'UNCOMPRESSED_FILE_NAME', 'REQUIRED_STORAGE_BYTES', '^DESCRIPTION', 'FILE_NAME UNCOMPRESSED', 'RECORD_TYPE UNCOMPRESSED', 'RECORD_BYTES', 'FILE_RECORDS', 'LABEL_RECORDS', '^IMAGE', 'LINES', 'LINE_SAMPLES', 'SAMPLE_TYPE', 'SAMPLE_BITS', 'CHECKSUM', 'SCALING_FACTOR', 'OFFSET', 'MISSING_CONSTANT', 'NOTE', '^DATA_SET_MAP_PROJECTION', 'MAP_PROJECTION_TYPE', 'FIRST_STANDARD_PARALLEL', 'SECOND_STANDARD_PARALLEL', 'A_AXIS_RADIUS', 'B_AXIS_RADIUS', 'C_AXIS_RADIUS', 'POSITIVE_LONGITUDE_DIRECTION', 'CENTER_LATITUDE', 'CENTER_LONGITUDE', 'REFERENCE_LATITUDE', 'REFERENCE_LONGITUDE', 'LINE_FIRST_PIXEL', 'LINE_LAST_PIXEL', 'SAMPLE_FIRST_PIXEL', 'SAMPLE_LAST_PIXEL', 'MAP_PROJECTION_ROTATION', 'MAP_RESOLUTION', 'MAP_SCALE', 'MAXIMUM_LATITUDE', 'MINIMUM_LATITUDE', 'EASTERNMOST_LONGITUDE', 'WESTERNMOST_LONGITUDE', 'LINE_PROJECTION_OFFSET', 'SAMPLE_PROJECTION_OFFSET', 'OBLIQUE_PROJ_POLE_LATITUDE', 'OBLIQUE_PROJ_POLE_LONGITUDE', 'OBLIQUE_PROJ_POLE_ROTATION', 'OBLIQUE_PROJ_X_AXIS_VECTOR', 'OBLIQUE_PROJ_Y_AXIS_VECTOR', 'OBLIQUE_PROJ_Z_AXIS_VECTOR', 'LOOK_DIRECTION', 'COORDINATE_SYSTEM_NAME', 'COORDINATE_SYSTEM_TYPE']
         </details>
         <details closed>
         <summary>Section Header Options (Click to view all)</summary>
         <br>
         ['PRODUCT DESCRIPTION', 'DESCRIPTION OF COMPRESSED AND UNCOMPRESSED FILES', 'POINTERS TO START RECORDS OF OBJECTS IN FILE', 'DESCRIPTION OF OBJECTS CONTAINED IN FILE']
         </details>
         
-        **retrieveFeaturesFromLatitudeLongitude**
-        
-        Return a list of features found at a specific latitude/longitude position
+        ## Use Downloaded Data
+        ### displayImages()
         
         ```
-        retrieveFeaturesFromLatitudeLongitude(latitude=None, longitude=None)
+        displayImages(image_directory=None, fig_title=None, figsize_n=6, fig_dpi=120)
         ```
-        * **[REQUIRED]** latitude (float/int): Latitude (in degrees) where North = + and South = -
-        * **[REQUIRED]** longitude (float/int): Longitude (in degrees) where West = + and East = -
+        
+        * **[REQUIRED]** image_directory (string): directory containing pydar_results with IMG file
+        * [OPTIONAL] fig_title (str): figure title, defaults to filename
+        * [OPTIONAL] figsize_n (int): plot dimensions, defaults to 6x6
+        * [OPTIONAL] fig_dpi (int): plot dpi, defaults to 120
+        
+        Displays downloaded image .IMG files (unzipped from within the .ZIP files) and display all images in directory
         
         ```python
         import pydar
-        feature_names_list = pydar.retrieveFeaturesFromLatitudeLongitude(latitude=-72, longitude=183)
+        pydar.displayImages(image_directory="pydar_results/CORADR_0065_V03_S01")
         ```
+         <p align="center">
+          <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/ontario_example_output.png" />
+        </p>
         
-        feature_names_list = `['Ontario Lacus']`
+        Note: displayImages() will plt.show() all images in the saved results directory
         
-        **retrieveFeaturesFromLatitudeLongitudeRange**
+        **COMING SOON: extractMetadata**
         
-        ```
-        retrieveFeaturesFromLatitudeLongitudeRange(northernmost_latitude=None,
-        										southernmost_latitude=None,
-        										easternmost_longitude=None,
-        										westernmost_longitude=None)
-        ```
-        * **[REQUIRED]** northernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, north must be greater than or equal to the south
-        * **[REQUIRED]** southernmost_latitude (float/int): Latitude (in degrees) where North = + and South = -, south must be less than or euqal to the north
-        * **[REQUIRED]** easternmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, west must be less than or equal to the east
-        * **[REQUIRED]** westernmost_longitude (float/int): Longitude (in degrees) where West = + and East = -, east must be greater than or equal to the west
+        Extract Metadata from .FMT and .TAB files
         
-        ```python
-        import pydar
-        feature_names_list = pydar.retrieveFeaturesFromLatitudeLongitudeRange(northernmost_latitude=11,
-        																southernmost_latitude=-80,
-        																easternmost_longitude=339,
-        																westernmost_longitude=341)
-        ```
-        feature_names_list = `['Aaru', 'Rossak Planitia']`
+        COMING SOON: Extract metadata from .TAB file (using .FMT as a reference)
         
-        ## TODO:
+        ## Developer Notes TODO:
         ### TODO Code:
-        * retrieveIDSByTime() based on time or time range
         * add a colored outline around a feature when displaying as a 2D image
+        * save image pixel to an array
+        * extract pdr functionality to reduce overhead
+        * displayImages() bug fix: 87 displays invalid integer
         * segments will be less than 99 (default to 1 - 01 is the primary imaging)
-        * README for all the functions and their sections
         * progress bars print to command line (still downloading...)
+        * save .IMG as .SHP for ArcGIS
         
         ### TODO Questions:
-        * what is the timestamp for start/stop time: "2005-301T03:53:56.971" format? YYYY-MDDTHH:MM:SS.mms?
-        * get longitude values when greater than 180 (everything is relative to west)
-        * add details for what a segement_num is
+        * add details for what a segment_num is
         * associate burst ID from SBDR data to BIDR data for metadata
         * save .IMG as an array of pixel values
         * save .IMG as .SHP for ArcGIS
         * project image onto Titan spheriod
         * downloadAdditionalDataTypes() does not have functionality (["ABDR", "ASUM", "LBDR", "STDR"]), decide which files to download
         
         ### TODO: Tech Debt
         * use README information to gather files for download (save computing, tech debt)
-        * CSV script to be run before each pypi package update by developer not user
-        * make README options for .LBL and AAREADME case-insensitive
         * set up constant config file
-        * bug fix: "NOTE" in .lbl
+        * Add functionality for extractFlybyDataImages(): additional_data_types_to_download
         * Include URL for access to AAREADME and .LBL readme files
-        * rm -rf pydar_results/ between runs for clean image output
         * research Zenodo
         
         ### TODO: Test
         * test: pull up all passes that saw Ontario Lacus and colorcode with look angle 
         * test: pull beam information and number of looks for each pixel 
         
+        ## Credits
+        Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
+        
+        Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
+        
         ## Bug and Feature Request
         
         Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/unaschneck/pydar/issues) or to ugschneck@gmail.com/cyschneck@gmail.com
         
 Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pydar-0.1.0/pydar.egg-info/SOURCES.txt` & `pydar-1.0.0/pydar.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 pydar/display_image.py
 pydar/error_handling.py
 pydar/extract_flyby_parameters.py
 pydar/pydar_testing.py
 pydar/read_readme.py
 pydar/retrieve_ids_by_time_position.py
 pydar/retrieve_supplementary_backplanes.py
-pydar/update_csv.py
+pydar/sbdr_make_shapefile.py
+pydar/test_bearing_correction.py
+pydar/updateCsvCORADARJPLOptions.py
+pydar/updateCsvFeatureNameDetails.py
+pydar/updateCsvSwathCoverage.py
 pydar.egg-info/PKG-INFO
 pydar.egg-info/SOURCES.txt
 pydar.egg-info/dependency_links.txt
 pydar.egg-info/requires.txt
 pydar.egg-info/top_level.txt
 pydar/data/cassini_flyby.csv
 pydar/data/coradr_jpl_options.csv
 pydar/data/feature_name_details.csv
 pydar/data/sar_swath_details.csv
-pydar/data/swath_coverage_by_time_position.csv
+pydar/data/swath_coverage_by_time_position.csv
+pydar/pytests/test_extract_flyby_parameters.py
```

### Comparing `pydar-0.1.0/setup.py` & `pydar-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="0.1.0"
+VERSION="1.0.0"
 DESCRIPTION="A Python package to access, download, view, and manipulate Cassini RADAR images"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="pydar",
 	version=VERSION,
 	description=DESCRIPTION,
 	long_description=long_description_readme,
 	long_description_content_type='text/markdown',
 	url="https://github.com/unaschneck/pydar",
 	download_url="https://github.com/unaschneck/pydar/archive/refs/tags/v{0}.tar.gz".format(VERSION),
-	author="Una Schneck (unaschneck), C. Y. Schneck (cyschneck)",
+	author="Una Schneck (unaschneck), Cora Schneck (cyschneck)",
 	keywords=[],
 	license="MIT",
 	classifiers=[
-		"Development Status :: 1 - Planning",
+		"Development Status :: 4 - Beta",
 		"Intended Audience :: Developers",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
 		"License :: OSI Approved :: MIT License",
 		"Programming Language :: Python",
 		"Programming Language :: Python :: 3.9",
+		"Programming Language :: Python :: 3.8",
+		"Programming Language :: Python :: 3.7",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
 		"Topic :: Scientific/Engineering :: Physics",
+		"Topic :: Scientific/Engineering :: Image Processing",
 		"Topic :: Scientific/Engineering :: Visualization",
 		"Topic :: Scientific/Engineering :: Astronomy"
 	],
 	packages=find_namespace_packages(include=['pydar', 'pydar.*']),
 	include_package_data=True,
 	install_requires=[
 			"beautifulsoup4>=4.11.1",
 			"matplotlib>=3.1.0",
-			"pdf>=0.7.2",
+			"pandas>=1.5.2",
+			"pdr>=0.7.3",
 			"planetaryimage>=0.5.0",
+			"pyproj>=3.4.1",
+			"pytest>=7.2.2",
 			"urllib3>=1.26.9"
 			],
 	python_requires='>=3.9'
 )
```

