# Comparing `tmp/noisepy_seis-0.5.3.tar.gz` & `tmp/noisepy_seis-0.5.8.tar.gz`

## Comparing `noisepy_seis-0.5.3.tar` & `noisepy_seis-0.5.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   112593 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35203 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/LICENSE
--rw-r--r--   0        0        0    13580 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/README.md
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    16001 2020-02-02 00:00:00.000000 noisepy_seis-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    19873 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   112593 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35203 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/LICENSE
+-rw-r--r--   0        0        0    13682 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/README.md
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0    16027 2020-02-02 00:00:00.000000 noisepy_seis-0.5.8/PKG-INFO
```

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.5.8/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.5.8/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.5.8/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.5.8/src/noisepy/seis/S2_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/main.py` & `noisepy_seis-0.5.8/src/noisepy/seis/main.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.5.8/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.5.8/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.5.8/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.5.8/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.5.8/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.5.8/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/LICENSE` & `noisepy_seis-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.5.3/README.md` & `noisepy_seis-0.5.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ### Note the order of the command lines below matters ###
 
 # With Conda:
 ```bash
 $ conda create -n noisepy python=3.8 pip
 $ conda activate noisepy
 $ conda install -c conda-forge openmpi
-$ pip install noisepy-seis 
+$ pip install noisepy-seis
 ```
 
 # With virtual environment:
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```sh
 $ brew install open-mpi
 ```
@@ -52,27 +52,27 @@
 * save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
 * offers high flexibility to handle messy SAC/miniSEED data stored on your local machine and convert them into ASDF format data that could easily be pluged into NoisePy
 * performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
 * includes a series of monitoring functions to measure dv/v on the resulted cross-correlation functions using some recently developed new methods (see our papers for more details<sup>**</sup>)
 
 # Short tutorial
 
-### 0A. Downloading seismic noise data 
+### 0A. Downloading seismic noise data
 This command allows to download all available broadband CI stations `(BH?)` located in a certain region and operated during 1/Jul/2016-2/Jul/2016 through the SCEC data center.
 
 In the script, short summary is provided for all input parameters that can be changed according to the user's needs. In the current form of the script, we set `inc_hours=24` to download day-long continous noise data as well as the meta info and store them into a single ASDF file. To increase the signal-to-noise (SNR) of the final cross-correlation functions (see Seats et al.,2012 for more details), we break the day-long sequence into smaller segments, each of `cc_len` (s) long with some overlapping defined by `step`. You may wanto to set `flag` to be `True` if intermediate outputs/operational time is preferred during the downloading process.
 
-```bash
-noisepy download
+```sh
+$ noisepy download
 ```
 The data to be downloaded can be customized via command line arguments. See `noisepy download --help` for details.
 
 If you want to use multiple cores (e.g, 4), run the script with the following command using [mpi4py](https://mpi4py.readthedocs.io/en/stable/).
-```bash
-mpirun -n 4 noisepy download
+```sh
+$ mpirun -n 4 noisepy download
 ```
 
 The outputted files from the download include ASDF files containing daily-long (24h) continous noise data, a parameter file recording all used parameters in the download and a CSV file of all station information (more details on reading the ASDF files with downloaded data can be found in docs/src/ASDF.md). The continous waveforms data stored in the ASDF file can be displayed using the plotting modules named as `plotting_modules` in the directory of `src` as shown below.
 
 ```python
 from noisepy.seis import plotting_modules
 sfile = '/Users/chengxin/Documents/SCAL/RAW_DATA/2016_07_01_00_00_00T2016_07_02_00_00_00.h5'
@@ -104,15 +104,15 @@
 from noisepy.seis import plotting_modules
 sfile = '/Users/chengxin/Documents/SCAL/CCF/2016_07_01_00_00_00T2016_07_02_00_00_00.h5'
 plotting_modules.plot_substack_cc(sfile,0.1,0.2,200,True,'/Users/chengxin/Documents/SCAL/CCF/figures')
 ```
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/substack_cc_NN.png" width="400" height="190"><img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/substack_cc_ZZ.png" width="400" height="190">
 
 
-### 2. Do stacking 
+### 2. Do stacking
 This script is used to assemble and/or stack all cross-correlation functions computed for the staion pairs in the `cross_correlate` step and save them into ASDF files for future analysis (e.g., temporal variation and/or dispersion extraction). In particular, there are two options for the stacking process, including linear and phase weighted stacking (pws). See ```noisepy stack --help```
 
 ```sh
 $ noisepy stack --method linear
 $ noisepy stack --method pws
 ```
 
@@ -150,19 +150,24 @@
 * ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
 * ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
 * ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
 * ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
 
 # Contributing
 
-After creating the virtual environment with either **pip** o **conda**, install `pre-commit` by running:
+After cloning the repo and creating a virtual environment with either **pip** o **conda**:
 
+Do an editable installation to get the dependencies (from the project root):
+```sh
+$ pip install -e ".[dev]"
 ```
-pip install pre-commit>=3.2.0
-pre-commit install
+
+Install the `pre-commit` hook:
+```sh
+$ pre-commit install
 ```
 
 This will run the linting and formatting checks configured in the project before every commit.
 
 ## Using VS Code
 
 The following extensions are recommended:
```

### Comparing `noisepy_seis-0.5.3/pyproject.toml` & `noisepy_seis-0.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     "h5py>=3.8.0",
     "mpi4py>=3.1.4",
     "numba>=0.56.4",
     "numpy>=1.22.0",
     "pandas>=1.5.3",
     "pyasdf>=0.7.5",
     "pycwt>=0.3.0a22",
-    "wheel>=0.38.4",
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/mdenolle/NoisePy"
 
 [tool.hatch.version]
@@ -59,15 +58,14 @@
 packages = ["src/noisepy"]
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.2.2",
     "memory-profiler>=0.61",
     "pre-commit>=3.2",
-    "hatchling>=1.14"
 ]
 
 [project.scripts]
 noisepy = "noisepy.seis:main.main_cli"
 
 [tool.black]
 line-length = 120
```

### Comparing `noisepy_seis-0.5.3/PKG-INFO` & `noisepy_seis-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.5.3
+Version: 0.5.8
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@fas.harvard.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -36,17 +36,15 @@
 Requires-Dist: h5py>=3.8.0
 Requires-Dist: mpi4py>=3.1.4
 Requires-Dist: numba>=0.56.4
 Requires-Dist: numpy>=1.22.0
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: pyasdf>=0.7.5
 Requires-Dist: pycwt>=0.3.0a22
-Requires-Dist: wheel>=0.38.4
 Provides-Extra: dev
-Requires-Dist: hatchling>=1.14; extra == 'dev'
 Requires-Dist: memory-profiler>=0.61; extra == 'dev'
 Requires-Dist: pre-commit>=3.2; extra == 'dev'
 Requires-Dist: pytest>=7.2.2; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # About NoisePy
 NoisePy is a Python package designed for fast and easy computation of ambient noise cross-correlation functions. It provides additional functionality for noise monitoring and surface wave dispersion analysis.
@@ -77,15 +75,15 @@
 ### Note the order of the command lines below matters ###
 
 # With Conda:
 ```bash
 $ conda create -n noisepy python=3.8 pip
 $ conda activate noisepy
 $ conda install -c conda-forge openmpi
-$ pip install noisepy-seis 
+$ pip install noisepy-seis
 ```
 
 # With virtual environment:
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```sh
 $ brew install open-mpi
 ```
@@ -102,27 +100,27 @@
 * save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
 * offers high flexibility to handle messy SAC/miniSEED data stored on your local machine and convert them into ASDF format data that could easily be pluged into NoisePy
 * performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
 * includes a series of monitoring functions to measure dv/v on the resulted cross-correlation functions using some recently developed new methods (see our papers for more details<sup>**</sup>)
 
 # Short tutorial
 
-### 0A. Downloading seismic noise data 
+### 0A. Downloading seismic noise data
 This command allows to download all available broadband CI stations `(BH?)` located in a certain region and operated during 1/Jul/2016-2/Jul/2016 through the SCEC data center.
 
 In the script, short summary is provided for all input parameters that can be changed according to the user's needs. In the current form of the script, we set `inc_hours=24` to download day-long continous noise data as well as the meta info and store them into a single ASDF file. To increase the signal-to-noise (SNR) of the final cross-correlation functions (see Seats et al.,2012 for more details), we break the day-long sequence into smaller segments, each of `cc_len` (s) long with some overlapping defined by `step`. You may wanto to set `flag` to be `True` if intermediate outputs/operational time is preferred during the downloading process.
 
-```bash
-noisepy download
+```sh
+$ noisepy download
 ```
 The data to be downloaded can be customized via command line arguments. See `noisepy download --help` for details.
 
 If you want to use multiple cores (e.g, 4), run the script with the following command using [mpi4py](https://mpi4py.readthedocs.io/en/stable/).
-```bash
-mpirun -n 4 noisepy download
+```sh
+$ mpirun -n 4 noisepy download
 ```
 
 The outputted files from the download include ASDF files containing daily-long (24h) continous noise data, a parameter file recording all used parameters in the download and a CSV file of all station information (more details on reading the ASDF files with downloaded data can be found in docs/src/ASDF.md). The continous waveforms data stored in the ASDF file can be displayed using the plotting modules named as `plotting_modules` in the directory of `src` as shown below.
 
 ```python
 from noisepy.seis import plotting_modules
 sfile = '/Users/chengxin/Documents/SCAL/RAW_DATA/2016_07_01_00_00_00T2016_07_02_00_00_00.h5'
@@ -154,15 +152,15 @@
 from noisepy.seis import plotting_modules
 sfile = '/Users/chengxin/Documents/SCAL/CCF/2016_07_01_00_00_00T2016_07_02_00_00_00.h5'
 plotting_modules.plot_substack_cc(sfile,0.1,0.2,200,True,'/Users/chengxin/Documents/SCAL/CCF/figures')
 ```
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/substack_cc_NN.png" width="400" height="190"><img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/substack_cc_ZZ.png" width="400" height="190">
 
 
-### 2. Do stacking 
+### 2. Do stacking
 This script is used to assemble and/or stack all cross-correlation functions computed for the staion pairs in the `cross_correlate` step and save them into ASDF files for future analysis (e.g., temporal variation and/or dispersion extraction). In particular, there are two options for the stacking process, including linear and phase weighted stacking (pws). See ```noisepy stack --help```
 
 ```sh
 $ noisepy stack --method linear
 $ noisepy stack --method pws
 ```
 
@@ -200,19 +198,24 @@
 * ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
 * ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
 * ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
 * ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
 
 # Contributing
 
-After creating the virtual environment with either **pip** o **conda**, install `pre-commit` by running:
+After cloning the repo and creating a virtual environment with either **pip** o **conda**:
 
+Do an editable installation to get the dependencies (from the project root):
+```sh
+$ pip install -e ".[dev]"
 ```
-pip install pre-commit>=3.2.0
-pre-commit install
+
+Install the `pre-commit` hook:
+```sh
+$ pre-commit install
 ```
 
 This will run the linting and formatting checks configured in the project before every commit.
 
 ## Using VS Code
 
 The following extensions are recommended:
```

