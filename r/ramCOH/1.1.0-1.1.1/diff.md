# Comparing `tmp/ramCOH-1.1.0.tar.gz` & `tmp/ramCOH-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramCOH-1.1.0.tar", last modified: Fri Mar  3 23:19:44 2023, max compression
+gzip compressed data, was "ramCOH-1.1.1.tar", last modified: Tue Apr 11 09:40:56 2023, max compression
```

## Comparing `ramCOH-1.1.0.tar` & `ramCOH-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-03-03 23:19:44.924804 ramCOH-1.1.0/
--rw-r--r--   0 thomas     (501) staff       (20)     1064 2023-03-03 21:50:08.000000 ramCOH-1.1.0/LICENSE
--rw-r--r--   0 thomas     (501) staff       (20)       23 2023-03-03 22:43:32.000000 ramCOH-1.1.0/MANIFEST.in
--rw-r--r--   0 thomas     (501) staff       (20)     1995 2023-03-03 23:19:44.924630 ramCOH-1.1.0/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      270 2023-03-03 23:16:38.000000 ramCOH-1.1.0/README.md
--rw-r--r--   0 thomas     (501) staff       (20)      764 2023-03-03 23:19:37.000000 ramCOH-1.1.0/pyproject.toml
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-03-03 23:19:44.920802 ramCOH-1.1.0/ramCOH/
--rw-r--r--   0 thomas     (501) staff       (20)       27 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/__init__.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-03-03 23:19:44.923177 ramCOH-1.1.0/ramCOH/raman/
--rw-r--r--   0 thomas     (501) staff       (20)      133 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/raman/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)    22262 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/raman/baseclass.py
--rw-r--r--   0 thomas     (501) staff       (20)      730 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/raman/baseline_regions.py
--rw-r--r--   0 thomas     (501) staff       (20)     4674 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/raman/co2.py
--rw-r--r--   0 thomas     (501) staff       (20)    10169 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/raman/glass.py
--rw-r--r--   0 thomas     (501) staff       (20)     6002 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/raman/neon.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-03-03 23:19:44.924037 ramCOH-1.1.0/ramCOH/signal_processing/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/signal_processing/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     7698 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/signal_processing/curve_fitting.py
--rw-r--r--   0 thomas     (501) staff       (20)     3490 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/signal_processing/curves.py
--rw-r--r--   0 thomas     (501) staff       (20)     6939 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/signal_processing/deconvolution.py
--rw-r--r--   0 thomas     (501) staff       (20)     7758 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/signal_processing/functions.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-03-03 23:19:44.924370 ramCOH-1.1.0/ramCOH/static/
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-03-03 22:43:29.000000 ramCOH-1.1.0/ramCOH/static/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     9154 2023-03-03 21:50:08.000000 ramCOH-1.1.0/ramCOH/static/neon_emissionLines.csv
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-03-03 23:19:44.921810 ramCOH-1.1.0/ramCOH.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     1995 2023-03-03 23:19:44.000000 ramCOH-1.1.0/ramCOH.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      616 2023-03-03 23:19:44.000000 ramCOH-1.1.0/ramCOH.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-03-03 23:19:44.000000 ramCOH-1.1.0/ramCOH.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       38 2023-03-03 23:19:44.000000 ramCOH-1.1.0/ramCOH.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        7 2023-03-03 23:19:44.000000 ramCOH-1.1.0/ramCOH.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)       38 2023-03-03 23:19:44.924856 ramCOH-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.888039 ramCOH-1.1.1/
+-rw-rw-rw-   0        0        0     1928 2022-03-17 08:07:39.000000 ramCOH-1.1.1/.gitignore
+-rw-rw-rw-   0        0        0     1085 2022-03-17 08:07:39.000000 ramCOH-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       23 2023-03-06 13:35:09.000000 ramCOH-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2521 2023-04-11 09:40:56.887039 ramCOH-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2023-04-11 09:28:08.000000 ramCOH-1.1.1/README.md
+-rw-rw-rw-   0        0        0      799 2023-04-11 09:07:54.000000 ramCOH-1.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.737044 ramCOH-1.1.1/ramCOH/
+-rw-rw-rw-   0        0        0       28 2023-03-03 16:13:03.000000 ramCOH-1.1.1/ramCOH/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.856044 ramCOH-1.1.1/ramCOH/raman/
+-rw-rw-rw-   0        0        0     4801 2023-03-06 13:35:09.000000 ramCOH-1.1.1/ramCOH/raman/CO2.py
+-rw-rw-rw-   0        0        0      137 2023-03-06 16:24:34.000000 ramCOH-1.1.1/ramCOH/raman/__init__.py
+-rw-rw-rw-   0        0        0    22900 2023-04-07 09:46:43.000000 ramCOH-1.1.1/ramCOH/raman/baseclass.py
+-rw-rw-rw-   0        0        0      762 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/raman/baseline_regions.py
+-rw-rw-rw-   0        0        0    10484 2023-03-29 12:40:13.000000 ramCOH-1.1.1/ramCOH/raman/glass.py
+-rw-rw-rw-   0        0        0     6173 2023-03-03 16:15:07.000000 ramCOH-1.1.1/ramCOH/raman/neon.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.869041 ramCOH-1.1.1/ramCOH/signal_processing/
+-rw-rw-rw-   0        0        0        0 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/signal_processing/__init__.py
+-rw-rw-rw-   0        0        0     7988 2023-03-03 16:15:28.000000 ramCOH-1.1.1/ramCOH/signal_processing/curve_fitting.py
+-rw-rw-rw-   0        0        0     3644 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/signal_processing/curves.py
+-rw-rw-rw-   0        0        0     7133 2023-03-03 16:15:45.000000 ramCOH-1.1.1/ramCOH/signal_processing/deconvolution.py
+-rw-rw-rw-   0        0        0     8541 2023-04-06 12:27:33.000000 ramCOH-1.1.1/ramCOH/signal_processing/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.884037 ramCOH-1.1.1/ramCOH/static/
+-rw-rw-rw-   0        0        0        2 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/static/__init__.py
+-rw-rw-rw-   0        0        0     9547 2023-03-03 13:39:43.000000 ramCOH-1.1.1/ramCOH/static/neon_emissionLines.csv
+drwxrwxrwx   0        0        0        0 2023-04-11 09:40:56.778037 ramCOH-1.1.1/ramCOH.egg-info/
+-rw-rw-rw-   0        0        0     2521 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      647 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 09:40:56.000000 ramCOH-1.1.1/ramCOH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:40:56.888039 ramCOH-1.1.1/setup.cfg
```

### Comparing `ramCOH-1.1.0/PKG-INFO` & `ramCOH-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-Metadata-Version: 2.1
-Name: ramCOH
-Version: 1.1.0
-Summary: Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses
-Author: Thomas van Gerve
-License: MIT License
-        
-        Copyright (c) 2022 TDGerve
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/TDGerve/ramCOH
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ramCOH
-
-Library for processing and peak fitting of Raman spectra, targeted at CO<sub>2</sub> fluids and (hydrous) silicate glasses
-
-## Documentation
-Code documentation is available at [ramcoh.readthedocs.io](https://ramcoh.readthedocs.io/en/latest)
-
-## Installation
-
-
+Metadata-Version: 2.1
+Name: ramCOH
+Version: 1.1.1
+Summary: Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses
+Author: Thomas van Gerve
+License: MIT License
+        
+        Copyright (c) 2022 TDGerve
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/TDGerve/ramCOH
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Documentation Status](https://readthedocs.org/projects/ramcoh/badge/?version=latest)](https://ramcoh.readthedocs.io/en/latest/?badge=latest)
+# ramCOH
+
+Library for processing and peak fitting of Raman spectra, targeted at CO<sub>2</sub> fluids and (hydrous) silicate glasses
+
+## Documentation
+Code documentation is available at [ramcoh.readthedocs.io](https://ramcoh.readthedocs.io/en/latest)
+
+## Installation
+ramCOH can be installed with pip by running
+
+    pip install ramCOH
+
+in a terminal.
+
+If you would like to install from a specific git branch or release instead run
+
+    pip install git+https://github.com/TDGerve/ramCOH.git@tag
+
+where *tag* should be repleaced by the release tag or branch name (e.g. *v1.0* or *development*)
+
+
```

### Comparing `ramCOH-1.1.0/pyproject.toml` & `ramCOH-1.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[build-system]
-requires = [
-    "setuptools>=42",
-    "wheel"
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "ramCOH"
-version = "1.1.0"
-authors = [
-    {name = "Thomas van Gerve"},
-]
-description = "Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses"
-readme = "README.md"
-requires-python = ">=3.8"
-license = { file = "LICENSE" }
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "pandas",
-    "numpy",
-    "scipy",
-    "scikit-learn",
-    "csaps",
-]
-
-[project.urls]
-Homepage = "https://github.com/TDGerve/ramCOH"
-
-
-[tool.setuptools.package-data]
+[build-system]
+requires = [
+    "setuptools>=42",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "ramCOH"
+version = "1.1.1"
+authors = [
+    {name = "Thomas van Gerve"},
+]
+description = "Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses"
+readme = "README.md"
+requires-python = ">=3.8"
+license = { file = "LICENSE" }
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "pandas",
+    "numpy",
+    "scipy",
+    "scikit-learn",
+    "csaps",
+]
+
+[project.urls]
+Homepage = "https://github.com/TDGerve/ramCOH"
+
+
+[tool.setuptools.package-data]
 "ramCOH.static" = ["*.csv"]
```

### Comparing `ramCOH-1.1.0/ramCOH/raman/baseclass.py` & `ramCOH-1.1.1/ramCOH/raman/baseclass.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,622 +1,621 @@
-"""
-===============
-Generic classes
-===============
-The baseclass module provides generic classes for processing Raman data and storing spectral data
-"""
-
-from typing import Annotated, Dict, List, Literal, Optional, Tuple, Union
-from warnings import warn
-
-import csaps as cs
-import numpy as np
-import numpy.typing as npt
-import scipy.interpolate as itp
-import scipy.optimize as opt
-
-from ramCOH.signal_processing import curve_fitting as cf
-from ramCOH.signal_processing import curves as c
-from ramCOH.signal_processing import deconvolution as d
-from ramCOH.signal_processing import functions as f
-
-arrayNx2 = Annotated[npt.NDArray, Literal["N", 2]]
-
-
-class Signal:
-    """Container for spectral data
-
-    Parameters
-    ----------
-    x   :   array
-        1D array with x-axis data
-    y   :   array
-        1D array with intensity data
-
-    Attributes
-    ----------
-    x   :   array of float
-        x-axis data
-    raw :   array of float
-        unprocessed intensity data
-    names   :   list of str
-        names of all current spectra
-    all : dict
-        all current spectra as name: values
-    """
-
-    def __init__(self, x: npt.NDArray, y: npt.NDArray):
-        self.x = x
-        self.raw = y
-        self._names: List[str] = ["raw"]
-
-    @property
-    def names(self):
-        return self._names
-
-    @property
-    def all(self) -> Dict:
-        return {name: self.get(name) for name in self.names}
-
-    def add(self, name: str, values: npt.NDArray) -> None:
-        """
-        Add a new spectrum
-        """
-        if name in self._names:
-            self.set(name, values)
-            return
-        setattr(self, name, values)
-        self._names.append(name)
-
-    def set(self, name, values: npt.NDArray) -> None:
-        """
-        Set the values of a spectrum
-        """
-        if name not in self.names:
-            raise ValueError(f"{name} not in signals")
-        setattr(self, name, values)
-
-    def get(self, name: str) -> npt.NDArray:
-        """
-        Get the values of a spectrum
-        """
-        array = getattr(self, name, None)
-        if array is not None:
-            array = array.copy()
-        return array
-
-    def interpolate_spectrum(
-        self, old_x: npt.NDArray, old_y: npt.NDArray
-    ) -> npt.NDArray:
-        """
-        Linear interpolation a spectrum to match its x-axis with :py:attr:`~ramCOH.raman.baseclass.Signal.x`
-
-        """
-        interpolate = itp.interp1d(old_x, old_y, bounds_error=False, fill_value=0.0)
-        return interpolate(self.x)
-
-    def set_with_interpolation(self, name: str, x: npt.NDArray, y: npt.NDArray) -> None:
-        """
-        Add a new spectrum with interpolated intensities.
-
-        Interpolation is calculated with :py:meth:`~ramCOH.raman.baseclass.Signal.interpolate_spectrum`
-        """
-        new_y = self.interpolate_spectrum(x, y)
-        self.add(name, new_y)
-
-    def remove(self, names):
-        for name in names:
-            if name not in self._names:
-                continue
-            delattr(self, name)
-            self._names.remove(name)
-
-
-class RamanProcessing:
-    """Generic class for processing Raman spectral data
-
-    Parameters
-    ----------
-    x   :   array
-        1D array with x-axis data
-    y   :   array of float or int
-        1D array with intensity data
-    laser   : float, optional
-        laser wavelenghth in nm
-
-    Attributes
-    ----------
-    x : array
-        1D array with x-axis data
-    signal : Signal
-        container with all spectral data
-    noise   :   float
-        calculated average noise on the baseline corrected spectrum
-    laser   :   float, optional
-        laser wavelength in nm
-    processing  :   dict
-        dictionary of bool indicating which data treatments have been applied
-    birs    : ndarray
-        (n, 2) shaped array with left and right boundaries of the last used baseline interpolation regions
-    peaks   :   list of dict
-        list of best-fit parameters of peaks fitted to the spectrum by either deconvolution or simple peak fitting
-    _spectrumSelect :   str
-        default spectrum selected for processing. The selection hierarchy is raw -> interference_corrected -> interpolated,
-        where the last available spectrum is selected
-
-    """
-
-    def __init__(self, x: npt.NDArray, y: npt.NDArray, laser: Optional[float] = None):
-        x, y = f.trim_sort(x, y)
-        self.x = x
-        self.signal = Signal(x, y)
-
-        self.laser = laser
-        self._processing = {
-            "raw": True,
-            "interference_corrected": False,
-            "interpolated": False,
-        }
-
-        self.noise: Optional[float] = None
-        self.birs: Optional[arrayNx2[float]] = None
-        self.peaks: Optional[List[Dict]] = None
-
-    @property
-    def processing(self) -> dict:
-        return self._processing
-
-    @property
-    def _spectrumSelect(self) -> str:
-        spectra = ("interference_corrected", "interpolated")
-        selection = "raw"
-        for key in spectra:
-            selection = key if self._processing[key] else selection
-        return selection
-
-    def _set_processing(self, types: List[str], values: List[bool]) -> None:
-        for t, val in zip(types, values):
-            try:
-                _ = self._processing.get(t)
-                self._processing[t] = val
-            except KeyError:
-                warn(message=f"key '{t}' not found")
-
-    def smooth(self, type="gaussian", kernel_width=9, inplace=False, **kwargs) -> None:
-        """
-        Smoothing with either a moving average or with a Gaussian kernel.
-        Note that each application shortens the spectrum by one kernel width.
-        The raw spectrum will be used if keyword argment ``y`` is not set.
-
-        If inplace is set to True, the smoothed spectrum will overwrite the original spectrum.
-
-        Parameters
-        ----------
-        type    :   str
-            Smoothing kernel type: 'gaussian' or 'moving_average'
-        kernel_width    :   int, default 9
-            Size of the smoothing kernel in steps along the x-axis
-        inplace   :   bool, default False
-            Return the smoothed array
-        **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-        Other Parameters
-        -------------------
-        y   :   str, Optional
-            name of the spectrum to be treated
-
-        """
-
-        y = kwargs.get("y", "raw")
-        spectrum = self.signal.get(y)
-
-        smooth = f.smooth(y=spectrum, type=type, kernel_width=kernel_width)
-
-        x_shortened = self.x[(kernel_width - 1) // 2 : -(kernel_width - 1) // 2]
-
-        if not inplace:
-            return x_shortened, smooth
-
-        self.signal.set(y, smooth)
-
-        # match length of x with length of smoothed signal
-        self.x = x_shortened
-        # do the same for any other pre-existing spectra
-        for name, value in self.signal.all.items():
-            if name == self._spectrumSelect:
-                continue
-            shortened = value[(kernel_width - 1) // 2 : -(kernel_width - 1) // 2]
-            self.signal.set(name, shortened)
-
-    def baselineCorrect(self, baseline_regions=None, smooth_factor=1, **kwargs) -> None:
-        """
-        Baseline correction with natural smoothing splines from :py:func:`csaps:csaps.csaps` fitted to interpolation regions.
-
-        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.signal`.
-
-
-        Parameters
-        ----------
-        baseline_regions    :   ndarray, optional
-            (n, 2) array for n interpolation regions, where each row is [lower_limit, upper_limit]
-        smooth_factor: float, default 1
-            baseline smoothing factor between 0-1. As the value approaches 0, the baseline becomes linear.
-            It is passed to the smooth parameter of :py:func:`~csaps:csaps.csaps` as 1e-6 * smooth_factor
-        **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-        Other Parameters
-        ----------------
-        y   :   str, Optional
-            name of the spectrum to be treated
-        """
-        y = kwargs.get("y", self._spectrumSelect)
-        spectrum = self.signal.get(y)
-
-        if (self.birs_default is not None) & (baseline_regions is None):
-            baseline_regions = self.birs_default
-
-        self.birs = baseline_regions
-
-        xbir, ybir = f._extractBIR(self.x, spectrum, baseline_regions)
-
-        # max_difference = abs(ybir.max() - ybir.min())
-        smooth = 1e-6 * smooth_factor
-
-        spline = cs.csaps(xbir, ybir, smooth=smooth)
-        self.baseline = spline(self.x)
-        baseline_corrected = spectrum - self.baseline
-
-        self.signal.add("baseline_corrected", baseline_corrected)
-        self.signal.add("baseline", self.baseline)
-
-    def calculate_noise(self, baseline_regions: Optional[npt.NDArray] = None) -> None:
-
-        """
-        Calculate noise on a baseline corrected spectrum.
-
-        Noise is calculated within baseline interpolation regions as
-        2 standard deviations on the baseline corrected spectrum.
-
-        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.noise`
-
-        Other parameters
-        ----------------
-        baseline_regions    : ndarray, optional
-            (n, 2) shapped array with regions where noise will be calculated. If not set, the last set baseline interpolation regions will be used.
-        """
-
-        baseline_corrected = self.signal.get("baseline_corrected")
-        if baseline_corrected is None:
-            raise RuntimeError("Run baseline correction first")
-
-        if (self.birs is not None) & (baseline_regions is None):
-            baseline_regions = self.birs
-
-        _, ybir = f._extractBIR(self.x, baseline_corrected, baseline_regions)
-
-        self.noise = ybir.std(axis=None) * 2
-
-    def normalise(self, inplace=False, **kwargs):
-        """
-        Normalise spectrum to maximum intensity :math:`\\times` 100. The raw spectrum will be used if keyword argment ``y`` is not set.
-
-        If inplace is set to True, the smoothed spectrum will overwrite the original spectrum.
-
-        Parameters
-        ----------
-        inplace :   bool, default False
-            set normalised spectrum inplace
-        **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-        Other Parameters
-        ----------------
-        y   :   str, Optional
-            name of the spectrum to be treated
-        """
-
-        y = kwargs.get("y", "raw")
-        spectrum = getattr(self.signal, y)
-
-        # normalisation to maximum intensity
-        normalised = spectrum * 100 / spectrum.max()
-
-        if not inplace:
-            return normalised
-
-        self.signal.set(y, normalised)
-
-    def interpolate(
-        self,
-        interpolate=List[Tuple[float, float]],
-        smooth_factor=1,
-        add_noise=True,
-        output=False,
-        use=False,
-        **kwargs,
-    ) -> None:
-        """
-        Interpolate across one or more regions
-
-        Interpolated signal is calculated fitting smoothing splines from :py:func:`csaps:csaps.csaps` to the rest of the spectrum.
-
-        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.signal`
-
-        Parameters
-        ----------
-        interpolate :   list of lists
-            list of interpolation regions in pairs of [upper limit, lower limits]
-        smooth_factor   :   float, default 1
-            Smoothes the interpolation; as it approaches 0 the interpolation becomes linear.
-            Passed on to the smooth parameter in :py:func:`~csaps:csaps.csaps` as smooth_factor * 1e-5
-        add_noise   :   bool, default True
-            add spectrum noise to the interpolated sections
-        use :   bool, default False
-            set interpolated spectrum as source for further processing
-        **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-        Other Parameters
-        ----------------
-        y   :   str, Optional
-            name of the spectrum to be treated
-        output  :   bool, default False
-            return interpolated sections as as tuple(x, y)
-
-        """
-        y = kwargs.get("y", self._spectrumSelect)
-        spectrum = self.signal.get(y)
-        x = self.x
-
-        interpolate_index = f._extractBIR_bool(x, interpolate)
-        spectrum_index = ~interpolate_index
-
-        interpolated_x, interpolated_y, spline = f._interpolate_section(
-            x, spectrum, interpolate, smooth_factor
-        )
-
-        if add_noise:
-            for section in interpolate:
-                left, right = section
-                window = f._extractBIR_bool(x, [[left, right]])
-                noise_window = (
-                    f._extractBIR_bool(x, [[left - 50, right + 50]]) & ~window
-                )
-                local_noise = (spectrum[noise_window] - spline(x[noise_window])).std(
-                    axis=None
-                )
-
-                mask = (interpolated_x > left) & (interpolated_x < right)
-                interpolated_y[mask] = interpolated_y[mask] + np.random.normal(
-                    0, local_noise, sum(mask)
-                )
-
-        if use:
-            interpolated_spectrum = f.add_interpolation(
-                spectrum, interpolate_index, interpolated_y
-            )
-            self.signal.add("interpolated", interpolated_spectrum)
-            self._processing["interpolated"] = True
-
-        if output:
-            return interpolated_x, interpolated_y
-
-    def fit_peaks(self, peak_prominence=3, fit_window=12, curve="GL", **kwargs) -> None:
-        """
-        Find the best fit curves for peaks in the spectrum.
-
-        Does not take into account peak overlap,
-        use :py:meth:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve` instead if you expect overlapping peaks.
-        Initial guesses for peak centers, amplitudes and widths are made with :py:func:`scipy:scipy.signal.find_peaks`
-
-        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.peaks` as a list of dictionaries with fitted parameters for each individual peak.
-
-
-
-        Parameters
-        ----------
-        peak_prominence : float or int, default 3
-            minimum peak prominence of fitted peaks, passed to :py:func:`find_peaks`
-        fit_window  :   int, default 12
-            Intervals across which peaks are fitted range from (peak center - (fit_window * half width)) to (peak center + (fit_window * half width))
-        curve   :   str, default 'GL'
-            curve shape. Options are:
-
-            * 'GL' for mixed Gaussian-Lorentzian/pseudo-Voigt (default),
-            * 'G' for Gaussian and
-            * 'L' for Lorentzian
-        **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-        Other Parameters
-        ----------------
-        y   :   str, Optional
-            name of the spectrum to be treated
-
-        """
-
-        y = kwargs.get("y", self._spectrumSelect)
-        spectrum = self.signal.get(y)
-        # clear old peaks
-        self.peaks = []
-        self.curve = curve
-        curveDict = {"GL": c.GaussLorentz, "G": c.Gaussian, "L": c.Lorentzian}
-
-        residuals = lambda params, x, spectrum: curveDict[curve](x, *params) - spectrum
-
-        amplitudes, centers, widths = cf._find_peak_parameters(
-            x=self.x, y=spectrum, prominence=peak_prominence
-        )
-
-        # Gaussian - Lorentian mixing paramter
-        shape = 0.5
-        # baselevel should be 0 for baseline corrected spectra
-        baselevel = 0
-
-        for i, (amplitude, center, width) in enumerate(
-            zip(amplitudes, centers, widths)
-        ):
-            x_range = cf._get_peakFit_ranges(center, width, fit_window)
-            xtrim, ytrim = cf._trimxy_ranges(self.x, spectrum, x_range)
-
-            init_values = [amplitude, center, width, baselevel]
-            bounds = (-np.inf, np.inf)
-            if curve == "GL":
-                init_values.append(shape)
-                bounds = (
-                    [-np.inf, -np.inf, -np.inf, -np.inf, 0],
-                    [np.inf, np.inf, np.inf, np.inf, 1],
-                )
-
-            fitParams = opt.least_squares(
-                fun=residuals,
-                x0=init_values,
-                bounds=bounds,
-                args=(xtrim, ytrim),
-            ).x
-
-            params = ["amplitude", "center", "width", "baselevel"]
-            if curve == "GL":
-                params.append("shape")
-
-            self.peaks.append({k: fitParams[j] for j, k in enumerate(params)})
-
-    def deconvolve(
-        self,
-        *,
-        peak_height,
-        residuals_threshold: float = 10,
-        baseline0: bool = True,
-        min_amplitude: Union[int, float] = 1,
-        min_peak_width: Union[int, float] = 4,
-        fit_window: int = 4,
-        max_iterations: int = 5,
-        noise: Optional[float] = None,
-        inplace=True,
-        **kwargs,
-    ) -> None:
-        """
-        Deconvolve the spectrum into its constituent peaks.
-
-        Initial guesses for peak centers, amplitudes and widths are made with :py:func:`scipy:scipy.signal.find_peaks`.
-        The spectrum is subdivided into multiple windows with *width* = ``fit_window``\ :math:`\\times` *guessed width*,
-        where overlapping windows are merged. Within each window :py:func:`mixed Gaussian-Lorentzian <ramCOH.signal_processing.curves.GaussLorentz>`
-        peaks are iteratively fitted to the spectrum. With each new iteration an additional peak is summed with previous peaks.
-        Iterations are stopped when ``max_iteraton`` is reached or when the residuals have improved less then ``residuals_threshold``.
-
-
-        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.peaks`
-        as a list of dictionaries with fitted parameters for each individual peak.
-
-
-        Parameters
-        ----------
-        peak_height :   float or int
-            minimum absolute peak height for initial guesses
-        residuals_threshold : float or int, default 10
-            fit iterations are stopped when the root-mean squared error has decreased less than ``residuals_threshold``\% compared to the previous iteration.
-        baseline0   :   bool, default True
-            fix the baselevel at 0
-        min_amplitude   : int or float, default 1
-            minimum absolute height of fitted peaks.
-        min_peak_width  : int, default 8
-            minimum full width of fitted peaks in x-axis steps
-        fit_window  :   int, default 4
-            width parameter of individual fit frames. Actual width is calculated as ``fit_window``\ :math:`\\times` *guessed full width*.
-        max_iterations  : int, default 5
-            maximum fit iterations per window. Each iteration a new peak is added and ``max_iterations``
-        noise   :   float, optional
-            average noise on the spectrum. If no value is given it will be calculated with :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.calculate_noise`
-        inplace :   bool, default True
-            return fitted peaks when False
-        **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-        Other Parameters
-        ----------------
-        y   :   str, Optional
-            name of the spectrum to be treated
-        x_min   :   float or int, optional
-            x-axis lower limit of deconvolved spectrum
-        x_max   :   float or int, optional
-            x-axis upper limit of deconvolved spectrum
-        """
-
-        y = kwargs.get("y", self._spectrumSelect)
-        spectrum = self.signal.get(y)
-        x = self.x
-
-        if noise is None:
-            self.calculate_noise()
-            noise = self.noise
-
-        if x_max := kwargs.get("x_max", None):
-            spectrum = spectrum[x < x_max]
-            x = x[x < x_max]
-        if x_min := kwargs.get("x_min", None):
-            spectrum = spectrum[x > x_min]
-            x = x[x > x_min]
-
-        # clear old peaks
-        if self.peaks is not None:
-            self.peaks = []
-
-        # convert to half width (used by scipy.signal.find_peaks)
-        min_peak_width = min_peak_width / 2
-
-        # smooth_spectrum = sig.savgol_filter(spectrum, window_length=50, polyorder=2)
-        peak_prominence = peak_height + (noise / 2)
-
-        _, centers, widths = cf._find_peak_parameters(
-            x=x,
-            y=spectrum,
-            prominence=peak_prominence,
-            height=peak_height,
-            width=min_peak_width,
-        )
-        ranges = cf._get_peakFit_ranges(
-            centers=centers, half_widths=widths, fit_window=fit_window
-        )
-
-        fitted_parameters = []
-        residual = 0
-        total_length = 0
-        for i, range in enumerate(ranges):
-            xtrim, ytrim = cf._trimxy_ranges(x, spectrum, range)
-            # noise_threshold_local = threshold_scaler(ytrim.max())
-
-            print(f"processing range {i+1:02d}/{len(ranges):02d}\n")
-            try:
-                parameters, residual_local = d.deconvolve_signal(
-                    x=xtrim,
-                    y=ytrim,
-                    # noise_threshold=noise_threshold_local,
-                    residuals_threshold=residuals_threshold,
-                    baseline0=baseline0,
-                    min_peak_width=min_peak_width,
-                    min_amplitude=min_amplitude,
-                    noise=noise,
-                    max_iterations=max_iterations,
-                )
-                fitted_parameters.append(parameters)
-                residual += residual_local * len(xtrim)
-                total_length += len(xtrim)
-            except IndexError:
-                warn(f"range {[int(i) for i in range]}skipped.")
-
-        residual = residual / total_length
-
-        deconvolution_parameters = [np.concatenate(p) for p in zip(*fitted_parameters)]
-        self.signal.add(
-            name="deconvoluted", values=c.sum_GaussLorentz(x, *deconvolution_parameters)
-        )
-        peaks = [
-            {"center": i, "amplitude": j, "width": k, "shape": l, "baselevel": m}
-            for _, (i, j, k, l, m) in enumerate(zip(*deconvolution_parameters))
-        ]
-
-        if not inplace:
-            return peaks
-
-        self.peaks = peaks
+"""
+===============
+Generic classes
+===============
+The baseclass module provides generic classes for processing Raman data and storing spectral data
+"""
+
+from typing import Annotated, Dict, List, Literal, Optional, Tuple, Union
+from warnings import warn
+
+import csaps as cs
+import numpy as np
+import numpy.typing as npt
+import scipy.interpolate as itp
+import scipy.optimize as opt
+
+from ramCOH.signal_processing import curve_fitting as cf
+from ramCOH.signal_processing import curves as c
+from ramCOH.signal_processing import deconvolution as d
+from ramCOH.signal_processing import functions as f
+
+arrayNx2 = Annotated[npt.NDArray, Literal["N", 2]]
+
+
+class Signal:
+    """Container for spectral data
+
+    Parameters
+    ----------
+    x   :   array
+        1D array with x-axis data
+    y   :   array
+        1D array with intensity data
+
+    Attributes
+    ----------
+    x   :   array of float
+        x-axis data
+    raw :   array of float
+        unprocessed intensity data
+    names   :   list of str
+        names of all current spectra
+    all : dict
+        all current spectra as name: values
+    """
+
+    def __init__(self, x: npt.NDArray, y: npt.NDArray):
+        self.x = x
+        self.raw = y
+        self._names: List[str] = ["raw"]
+
+    @property
+    def names(self):
+        return self._names
+
+    @property
+    def all(self) -> Dict:
+        return {name: self.get(name) for name in self.names}
+
+    def add(self, name: str, values: npt.NDArray) -> None:
+        """
+        Add a new spectrum
+        """
+        if name in self._names:
+            self.set(name, values)
+            return
+        setattr(self, name, values)
+        self._names.append(name)
+
+    def set(self, name, values: npt.NDArray) -> None:
+        """
+        Set the values of a spectrum
+        """
+        if name not in self.names:
+            raise ValueError(f"{name} not in signals")
+        setattr(self, name, values)
+
+    def get(self, name: str) -> npt.NDArray:
+        """
+        Get the values of a spectrum
+        """
+        array = getattr(self, name, None)
+        if array is not None:
+            array = array.copy()
+        return array
+
+    def interpolate_spectrum(
+        self, old_x: npt.NDArray, old_y: npt.NDArray
+    ) -> npt.NDArray:
+        """
+        Linear interpolation a spectrum to match its x-axis with :py:attr:`~ramCOH.raman.baseclass.Signal.x`
+
+        """
+        interpolate = itp.interp1d(old_x, old_y, bounds_error=False, fill_value=0.0)
+        return interpolate(self.x)
+
+    def set_with_interpolation(self, name: str, x: npt.NDArray, y: npt.NDArray) -> None:
+        """
+        Add a new spectrum with interpolated intensities.
+
+        Interpolation is calculated with :py:meth:`~ramCOH.raman.baseclass.Signal.interpolate_spectrum`
+        """
+        new_y = self.interpolate_spectrum(x, y)
+        self.add(name, new_y)
+
+    def remove(self, names):
+        for name in names:
+            if name not in self._names:
+                continue
+            delattr(self, name)
+            self._names.remove(name)
+
+
+class RamanProcessing:
+    """Generic class for processing Raman spectral data
+
+    Parameters
+    ----------
+    x   :   array
+        1D array with x-axis data
+    y   :   array of float or int
+        1D array with intensity data
+    laser   : float, optional
+        laser wavelenghth in nm
+
+    Attributes
+    ----------
+    x : array
+        1D array with x-axis data
+    signal : Signal
+        container with all spectral data
+    noise   :   float
+        calculated average noise on the baseline corrected spectrum
+    laser   :   float, optional
+        laser wavelength in nm
+    processing  :   dict
+        dictionary of bool indicating which data treatments have been applied
+    birs    : ndarray
+        (n, 2) shaped array with left and right boundaries of the last used baseline interpolation regions
+    peaks   :   list of dict
+        list of best-fit parameters of peaks fitted to the spectrum by either deconvolution or simple peak fitting
+    _spectrumSelect :   str
+        default spectrum selected for processing. The selection hierarchy is raw -> interference_corrected -> interpolated,
+        where the last available spectrum is selected
+
+    """
+
+    def __init__(self, x: npt.NDArray, y: npt.NDArray, laser: Optional[float] = None):
+        x, y = f.trim_sort(x, y)
+        self.x = x
+        self.signal = Signal(x, y)
+
+        self.laser = laser
+        self._processing = {
+            "raw": True,
+            "interference_corrected": False,
+            "interpolated": False,
+        }
+
+        self.noise: Optional[float] = None
+        self.birs: Optional[arrayNx2[float]] = None
+        self.peaks: Optional[List[Dict]] = None
+
+    @property
+    def processing(self) -> dict:
+        return self._processing
+
+    @property
+    def _spectrumSelect(self) -> str:
+        spectra = ("interference_corrected", "interpolated")
+        selection = "raw"
+        for key in spectra:
+            selection = key if self._processing[key] else selection
+        return selection
+
+    def _set_processing(self, types: List[str], values: List[bool]) -> None:
+        for t, val in zip(types, values):
+            try:
+                _ = self._processing.get(t)
+                self._processing[t] = val
+            except KeyError:
+                warn(message=f"key '{t}' not found")
+
+    def smooth(self, type="gaussian", kernel_width=9, inplace=False, **kwargs) -> None:
+        """
+        Smoothing with either a moving average or with a Gaussian kernel.
+        Note that each application shortens the spectrum by one kernel width.
+        The raw spectrum will be used if keyword argment ``y`` is not set.
+
+        If inplace is set to True, the smoothed spectrum will overwrite the original spectrum.
+
+        Parameters
+        ----------
+        type    :   str
+            Smoothing kernel type: 'gaussian' or 'moving_average'
+        kernel_width    :   int, default 9
+            Size of the smoothing kernel in steps along the x-axis
+        inplace   :   bool, default False
+            Return the smoothed array
+        **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+        Other Parameters
+        -------------------
+        y   :   str, Optional
+            name of the spectrum to be treated
+
+        """
+
+        y = kwargs.get("y", "raw")
+        spectrum = self.signal.get(y)
+
+        smooth = f.smooth(y=spectrum, type=type, kernel_width=kernel_width)
+
+        x_shortened = self.x[(kernel_width - 1) // 2 : -(kernel_width - 1) // 2]
+
+        if not inplace:
+            return x_shortened, smooth
+
+        self.signal.set(y, smooth)
+
+        # match length of x with length of smoothed signal
+        self.x = x_shortened
+        # do the same for any other pre-existing spectra
+        for name, value in self.signal.all.items():
+            if name == self._spectrumSelect:
+                continue
+            shortened = value[(kernel_width - 1) // 2 : -(kernel_width - 1) // 2]
+            self.signal.set(name, shortened)
+
+    def baselineCorrect(self, baseline_regions=None, smooth_factor=1, **kwargs) -> None:
+        """
+        Baseline correction with natural smoothing splines from :py:func:`csaps:csaps.csaps` fitted to interpolation regions.
+
+        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.signal`.
+
+
+        Parameters
+        ----------
+        baseline_regions    :   ndarray, optional
+            (n, 2) array for n interpolation regions, where each row is [lower_limit, upper_limit]
+        smooth_factor: float, default 1
+            baseline smoothing factor between 0-1. As the value approaches 0, the baseline becomes linear.
+            It is passed to the smooth parameter of :py:func:`~csaps:csaps.csaps` as 1e-6 * smooth_factor
+        **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+        Other Parameters
+        ----------------
+        y   :   str, Optional
+            name of the spectrum to be treated
+        """
+        y = kwargs.get("y", self._spectrumSelect)
+        spectrum = self.signal.get(y)
+
+        if hasattr(self, "birs_default") & (baseline_regions is None):
+            baseline_regions = self.birs_default
+
+        self.birs = baseline_regions
+
+        xbir, ybir = f._extractBIR(self.x, spectrum, baseline_regions)
+
+        # max_difference = abs(ybir.max() - ybir.min())
+        smooth = 1e-6 * smooth_factor
+
+        spline = cs.csaps(xbir, ybir, smooth=smooth)
+        self.baseline = spline(self.x)
+        baseline_corrected = spectrum - self.baseline
+
+        self.signal.add("baseline_corrected", baseline_corrected)
+        self.signal.add("baseline", self.baseline)
+
+    def calculate_noise(self, baseline_regions: Optional[npt.NDArray] = None) -> None:
+        """
+        Calculate noise on a baseline corrected spectrum.
+
+        Noise is calculated within baseline interpolation regions as
+        2 standard deviations on the baseline corrected spectrum.
+
+        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.noise`
+
+        Other parameters
+        ----------------
+        baseline_regions    : ndarray, optional
+            (n, 2) shapped array with regions where noise will be calculated. If not set, the last set baseline interpolation regions will be used.
+        """
+
+        baseline_corrected = self.signal.get("baseline_corrected")
+        if baseline_corrected is None:
+            raise RuntimeError("Run baseline correction first")
+
+        if (self.birs is not None) & (baseline_regions is None):
+            baseline_regions = self.birs
+
+        _, ybir = f._extractBIR(self.x, baseline_corrected, baseline_regions)
+
+        self.noise = ybir.std(axis=None) * 2
+
+    def normalise(self, inplace=False, **kwargs):
+        """
+        Normalise spectrum to maximum intensity :math:`\\times` 100. The raw spectrum will be used if keyword argment ``y`` is not set.
+
+        If inplace is set to True, the smoothed spectrum will overwrite the original spectrum.
+
+        Parameters
+        ----------
+        inplace :   bool, default False
+            set normalised spectrum inplace
+        **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+        Other Parameters
+        ----------------
+        y   :   str, Optional
+            name of the spectrum to be treated
+        """
+
+        y = kwargs.get("y", "raw")
+        spectrum = getattr(self.signal, y)
+
+        # normalisation to maximum intensity
+        normalised = spectrum * 100 / spectrum.max()
+
+        if not inplace:
+            return normalised
+
+        self.signal.set(y, normalised)
+
+    def interpolate(
+        self,
+        interpolate: List[Tuple[float, float]],
+        smooth_factor=1,
+        add_noise=True,
+        output=False,
+        use=False,
+        **kwargs,
+    ) -> None:
+        """
+        Interpolate across one or more regions
+
+        Interpolated signal is calculated fitting smoothing splines from :py:func:`csaps:csaps.csaps` to the rest of the spectrum.
+
+        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.signal`
+
+        Parameters
+        ----------
+        interpolate :   list of lists
+            list of interpolation regions in pairs of [upper limit, lower limits]
+        smooth_factor   :   float, default 1
+            Smoothes the interpolation; as it approaches 0 the interpolation becomes linear.
+            Passed on to the smooth parameter in :py:func:`~csaps:csaps.csaps` as smooth_factor * 1e-5
+        add_noise   :   bool, default True
+            add spectrum noise to the interpolated sections
+        use :   bool, default False
+            set interpolated spectrum as source for further processing
+        **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+        Other Parameters
+        ----------------
+        y   :   str, Optional
+            name of the spectrum to be treated
+        output  :   bool, default False
+            return interpolated sections as as tuple(x, y)
+
+        """
+        y = kwargs.get("y", self._spectrumSelect)
+        spectrum = self.signal.get(y)
+        x = self.x
+
+        interpolate_index = f._extractBIR_bool(x, interpolate)
+        spectrum_index = ~interpolate_index
+
+        interpolated_x, interpolated_y, spline = f._interpolate_section(
+            x, spectrum, interpolate, smooth_factor
+        )
+
+        if add_noise:
+            for section in interpolate:
+                left, right = section
+                window = f._extractBIR_bool(x, [[left, right]])
+                noise_window = (
+                    f._extractBIR_bool(x, [[left - 50, right + 50]]) & ~window
+                )
+                local_noise = (spectrum[noise_window] - spline(x[noise_window])).std(
+                    axis=None
+                )
+
+                mask = (interpolated_x > left) & (interpolated_x < right)
+                interpolated_y[mask] = interpolated_y[mask] + np.random.normal(
+                    0, local_noise, sum(mask)
+                )
+
+        if use:
+            interpolated_spectrum = f.add_interpolation(
+                spectrum, interpolate_index, interpolated_y
+            )
+            self.signal.add("interpolated", interpolated_spectrum)
+            self._processing["interpolated"] = True
+
+        if output:
+            return interpolated_x, interpolated_y
+
+    def fit_peaks(self, peak_prominence=3, fit_window=12, curve="GL", **kwargs) -> None:
+        """
+        Find the best fit curves for peaks in the spectrum.
+
+        Does not take into account peak overlap,
+        use :py:meth:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve` instead if you expect overlapping peaks.
+        Initial guesses for peak centers, amplitudes and widths are made with :py:func:`scipy:scipy.signal.find_peaks`
+
+        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.peaks` as a list of dictionaries with fitted parameters for each individual peak.
+
+
+
+        Parameters
+        ----------
+        peak_prominence : float or int, default 3
+            minimum peak prominence of fitted peaks, passed to :py:func:`find_peaks`
+        fit_window  :   int, default 12
+            Intervals across which peaks are fitted range from (peak center - (fit_window * half width)) to (peak center + (fit_window * half width))
+        curve   :   str, default 'GL'
+            curve shape. Options are:
+
+            * 'GL' for mixed Gaussian-Lorentzian/pseudo-Voigt (default),
+            * 'G' for Gaussian and
+            * 'L' for Lorentzian
+        **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+        Other Parameters
+        ----------------
+        y   :   str, Optional
+            name of the spectrum to be treated
+
+        """
+
+        y = kwargs.get("y", self._spectrumSelect)
+        spectrum = self.signal.get(y)
+        # clear old peaks
+        self.peaks = []
+        self.curve = curve
+        curveDict = {"GL": c.GaussLorentz, "G": c.Gaussian, "L": c.Lorentzian}
+
+        residuals = lambda params, x, spectrum: curveDict[curve](x, *params) - spectrum
+
+        amplitudes, centers, widths = cf._find_peak_parameters(
+            x=self.x, y=spectrum, prominence=peak_prominence
+        )
+
+        # Gaussian - Lorentian mixing paramter
+        shape = 0.5
+        # baselevel should be 0 for baseline corrected spectra
+        baselevel = 0
+
+        for i, (amplitude, center, width) in enumerate(
+            zip(amplitudes, centers, widths)
+        ):
+            x_range = cf._get_peakFit_ranges(center, width, fit_window)
+            xtrim, ytrim = cf._trimxy_ranges(self.x, spectrum, x_range)
+
+            init_values = [amplitude, center, width, baselevel]
+            bounds = (-np.inf, np.inf)
+            if curve == "GL":
+                init_values.append(shape)
+                bounds = (
+                    [-np.inf, -np.inf, -np.inf, -np.inf, 0],
+                    [np.inf, np.inf, np.inf, np.inf, 1],
+                )
+
+            fitParams = opt.least_squares(
+                fun=residuals,
+                x0=init_values,
+                bounds=bounds,
+                args=(xtrim, ytrim),
+            ).x
+
+            params = ["amplitude", "center", "width", "baselevel"]
+            if curve == "GL":
+                params.append("shape")
+
+            self.peaks.append({k: fitParams[j] for j, k in enumerate(params)})
+
+    def deconvolve(
+        self,
+        *,
+        peak_height,
+        residuals_threshold: float = 10,
+        baseline0: bool = True,
+        min_amplitude: Union[int, float] = 3,
+        min_peak_width: Union[int, float] = 4,
+        fit_window: int = 4,
+        max_iterations: int = 5,
+        noise: Optional[float] = None,
+        inplace=True,
+        **kwargs,
+    ) -> None:
+        """
+        Deconvolve the spectrum into its constituent peaks.
+
+        Initial guesses for peak centers, amplitudes and widths are made with :py:func:`scipy:scipy.signal.find_peaks`.
+        The spectrum is subdivided into multiple windows with *width* = ``fit_window``\ :math:`\\times` *guessed width*,
+        where overlapping windows are merged. Within each window :py:func:`mixed Gaussian-Lorentzian <ramCOH.signal_processing.curves.GaussLorentz>`
+        peaks are iteratively fitted to the spectrum. With each new iteration an additional peak is summed with previous peaks.
+        Iterations are stopped when ``max_iteraton`` is reached or when the residuals have improved less then ``residuals_threshold``.
+
+
+        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.peaks`
+        as a list of dictionaries with fitted parameters for each individual peak.
+
+
+        Parameters
+        ----------
+        peak_height :   float or int
+            minimum absolute peak height for initial guesses
+        residuals_threshold : float or int, default 10
+            fit iterations are stopped when the root-mean squared error has decreased less than ``residuals_threshold``\% compared to the previous iteration.
+        baseline0   :   bool, default True
+            fix the baselevel at 0
+        min_amplitude   : int or float, default 3
+            minium amplitude of fitted peaks as a factor of noise on y.
+        min_peak_width  : int, default 8
+            minimum full width of fitted peaks in x-axis steps
+        fit_window  :   int, default 4
+            width parameter of individual fit frames. Actual width is calculated as ``fit_window``\ :math:`\\times` *guessed full width*.
+        max_iterations  : int, default 5
+            maximum fit iterations per window. Each iteration a new peak is added and ``max_iterations``
+        noise   :   float, optional
+            average noise on the spectrum. If no value is given it will be calculated with :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.calculate_noise`
+        inplace :   bool, default True
+            return fitted peaks when False
+        **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+        Other Parameters
+        ----------------
+        y   :   str, Optional
+            name of the spectrum to be treated
+        x_min   :   float or int, optional
+            x-axis lower limit of deconvolved spectrum
+        x_max   :   float or int, optional
+            x-axis upper limit of deconvolved spectrum
+        """
+
+        y = kwargs.get("y", self._spectrumSelect)
+        spectrum = self.signal.get(y)
+        x = self.x
+
+        if noise is None:
+            self.calculate_noise()
+            noise = self.noise
+
+        if x_max := kwargs.get("x_max", None):
+            spectrum = spectrum[x < x_max]
+            x = x[x < x_max]
+        if x_min := kwargs.get("x_min", None):
+            spectrum = spectrum[x > x_min]
+            x = x[x > x_min]
+
+        # clear old peaks
+        if self.peaks is not None:
+            self.peaks = []
+
+        # convert to half width (used by scipy.signal.find_peaks)
+        min_peak_width = min_peak_width / 2
+
+        # smooth_spectrum = sig.savgol_filter(spectrum, window_length=50, polyorder=2)
+        peak_prominence = peak_height + (noise / 2)
+
+        _, centers, widths = cf._find_peak_parameters(
+            x=x,
+            y=spectrum,
+            prominence=peak_prominence,
+            height=peak_height,
+            width=min_peak_width,
+        )
+        ranges = cf._get_peakFit_ranges(
+            centers=centers, half_widths=widths, fit_window=fit_window
+        )
+
+        fitted_parameters = []
+        residual = 0
+        total_length = 0
+        for i, range in enumerate(ranges):
+            xtrim, ytrim = cf._trimxy_ranges(x, spectrum, range)
+            # noise_threshold_local = threshold_scaler(ytrim.max())
+
+            print(f"processing range {i+1:02d}/{len(ranges):02d}\n")
+            try:
+                parameters, residual_local = d.deconvolve_signal(
+                    x=xtrim,
+                    y=ytrim,
+                    # noise_threshold=noise_threshold_local,
+                    residuals_threshold=residuals_threshold,
+                    baseline0=baseline0,
+                    min_peak_width=min_peak_width,
+                    min_amplitude=min_amplitude,
+                    noise=noise,
+                    max_iterations=max_iterations,
+                )
+                fitted_parameters.append(parameters)
+                residual += residual_local * len(xtrim)
+                total_length += len(xtrim)
+            except IndexError:
+                warn(f"range {[int(i) for i in range]}skipped.")
+
+        residual = residual / total_length
+
+        deconvolution_parameters = [np.concatenate(p) for p in zip(*fitted_parameters)]
+        self.signal.add(
+            name="deconvoluted", values=c.sum_GaussLorentz(x, *deconvolution_parameters)
+        )
+        peaks = [
+            {"center": i, "amplitude": j, "width": k, "shape": l, "baselevel": m}
+            for _, (i, j, k, l, m) in enumerate(zip(*deconvolution_parameters))
+        ]
+
+        if not inplace:
+            return peaks
+
+        self.peaks = peaks
```

### Comparing `ramCOH-1.1.0/ramCOH/raman/co2.py` & `ramCOH-1.1.1/ramCOH/raman/CO2.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-"""
-=============
-CO2
-=============
-The CO\ :sub:`2`\  module provides a Raman processing class for for processing CO\ :sub:`2`\ Raman data
-"""
-from typing import Dict, Optional, Tuple
-
-import numpy as np
-import numpy.typing as npt
-
-from ramCOH.raman.baseclass import RamanProcessing
-from ramCOH.raman.baseline_regions import default_birs
-from ramCOH.signal_processing import curves as c
-
-
-class CO2(RamanProcessing):
-    """
-    A subclass of :py:class:`~ramCOH.raman.baseclass.RamanProcessing`, extended with methods for fitting the CO\ :sub:`2` Fermi diad.
-
-    Attributes
-    ----------
-    diad    :   tuple of dictionaries
-        fitted peak parameters of the diad peaks
-    diad_split  :   float
-        splitting of the Fermi diad in cm-1
-
-    """
-
-    diad: Optional[Tuple[Dict, Dict]] = None
-    diad_split: Optional[float] = None
-
-    birs_default = default_birs["CO2"]
-
-    def FermiDiad(
-        self, peak_height=20, fit_window=20, min_peak_width=4, **kwargs
-    ):  # peak_prominence=40
-        """
-        Fit the Fermi diad with mixed Gaussian-Lorentzian curves.
-
-        The spectrum is fitted with peaks with :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve`.
-        The peak with the higest amplitude at wavenumbers <1330cm\ :sup:`-1` is used as the lower diad peak and the peak
-        with the highest amplitude at wavenumbers >1330cm\ :sup:`-1` as the upper diad peak. Diad splitting is calculated as the
-        absolute difference between the fitted centers of the diad peaks.
-
-        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.peaks`, :py:attr:`~ramCOH.raman.CO2.CO2.diad` and :py:attr:`~ramCOH.raman.CO2.CO2.diad_split`.
-
-        Analyses of gas+liquid CO\ :sub:`2` mixtures also result in mixed diad peaks,
-        be careful with interpreting diad splitting if this is the case.
-
-
-        Parameters
-        ----------
-        peak_height :   float or in, default 20
-            minimum absolute height of peaks included in initial guesses, passed to :py:func:`~scipy:scipy.signal.find_peaks`
-        fit_window  :   int, default 20
-            width parameter of the x-axis window within which peaks are fitted. Actual width is calculated as ``fit_window`` :math:`\\times` *guessed width*.
-            passed to :py:meth:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve`
-        min_peak_width  : int, default 4
-            minimum full width of fitted peaks in x-axis steps
-            assed to :py:meth:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve`
-        **kwargs    :   dict, optional
-            Optional keyword arguments, passed to :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve`
-
-        """
-
-        if "baseline_corrected" not in self.signal.names:
-            raise RuntimeError("run baseline correction first")
-
-        self.peaks = self.deconvolve(
-            y="baseline_corrected",
-            peak_height=peak_height,
-            fit_window=fit_window,
-            min_peak_width=min_peak_width,
-            baseline0=True,
-            inplace=False,
-            x_min=1200,
-            x_max=1450,
-            **kwargs
-        )
-
-        lower = [peak for peak in self.peaks if peak["center"] < 1330]
-        upper = [peak for peak in self.peaks if peak["center"] > 1330]
-
-        self.diad = []
-        for region in (lower, upper):
-            amplitude_sort = np.argsort([peak["amplitude"] for peak in region])
-            peaks_sorted = np.array(region)[amplitude_sort]
-            self.diad.append(peaks_sorted[-1])
-
-        self.diad_split = abs(self.diad[0]["center"] - self.diad[1]["center"])
-
-    def diad_curves(self, window=8, stepsize=0.5) -> Tuple[npt.NDArray, npt.NDArray]:
-        """
-        Get diad curves from fitted parameters
-
-        Parameters
-        ----------
-        window  :   int, default 8
-            width parameter of the x-axis window within which curves are calculated. Actual width is calculated as ``window`` :math:`\\times` *peak width*.
-        stepsize    : float
-            x-axis stepsize
-
-        Returns
-        -------
-        npt.NDArray, npt.NDArray
-            (x, 2) shaped arrays with columns x, y for each diad peak.
-
-        """
-
-        if self.diad is None:
-            raise AttributeError("Run 'FermiDiad()' first!")
-
-        results = []
-
-        for peak in self.diad.values():
-            width = peak["width"]
-
-            start = peak["center"] - window * width
-            stop = peak["center"] + window * width
-
-            x = np.arange(start=start, stop=stop, step=stepsize)
-            y = c.GaussLorentz(x=x, **peak)
-
-            results.append(np.vstack([x, y]))
-
-        return results
+"""
+=============
+CO2
+=============
+The CO\ :sub:`2`\  module provides a Raman processing class for for processing CO\ :sub:`2`\ Raman data
+"""
+from typing import Dict, Optional, Tuple
+
+import numpy as np
+import numpy.typing as npt
+
+from ramCOH.raman.baseclass import RamanProcessing
+from ramCOH.raman.baseline_regions import default_birs
+from ramCOH.signal_processing import curves as c
+
+
+class CO2(RamanProcessing):
+    """
+    A subclass of :py:class:`~ramCOH.raman.baseclass.RamanProcessing`, extended with methods for fitting the CO\ :sub:`2` Fermi diad.
+
+    Attributes
+    ----------
+    diad    :   tuple of dictionaries
+        fitted peak parameters of the diad peaks
+    diad_split  :   float
+        splitting of the Fermi diad in cm-1
+
+    """
+
+    diad: Optional[Tuple[Dict, Dict]] = None
+    diad_split: Optional[float] = None
+
+    birs_default = default_birs["CO2"]
+
+    def FermiDiad(
+        self, peak_height=20, fit_window=20, min_peak_width=4, **kwargs
+    ):  # peak_prominence=40
+        """
+        Fit the Fermi diad with mixed Gaussian-Lorentzian curves.
+
+        The spectrum is fitted with peaks with :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve`.
+        The peak with the higest amplitude at wavenumbers <1330cm\ :sup:`-1` is used as the lower diad peak and the peak
+        with the highest amplitude at wavenumbers >1330cm\ :sup:`-1` as the upper diad peak. Diad splitting is calculated as the
+        absolute difference between the fitted centers of the diad peaks.
+
+        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.peaks`, :py:attr:`~ramCOH.raman.CO2.CO2.diad` and :py:attr:`~ramCOH.raman.CO2.CO2.diad_split`.
+
+        Analyses of gas+liquid CO\ :sub:`2` mixtures also result in mixed diad peaks,
+        be careful with interpreting diad splitting if this is the case.
+
+
+        Parameters
+        ----------
+        peak_height :   float or in, default 20
+            minimum absolute height of peaks included in initial guesses, passed to :py:func:`~scipy:scipy.signal.find_peaks`
+        fit_window  :   int, default 20
+            width parameter of the x-axis window within which peaks are fitted. Actual width is calculated as ``fit_window`` :math:`\\times` *guessed width*.
+            passed to :py:meth:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve`
+        min_peak_width  : int, default 4
+            minimum full width of fitted peaks in x-axis steps
+            assed to :py:meth:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve`
+        **kwargs    :   dict, optional
+            Optional keyword arguments, passed to :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.deconvolve`
+
+        """
+
+        if "baseline_corrected" not in self.signal.names:
+            raise RuntimeError("run baseline correction first")
+
+        self.peaks = self.deconvolve(
+            y="baseline_corrected",
+            peak_height=peak_height,
+            fit_window=fit_window,
+            min_peak_width=min_peak_width,
+            baseline0=True,
+            inplace=False,
+            x_min=1200,
+            x_max=1450,
+            **kwargs
+        )
+
+        lower = [peak for peak in self.peaks if peak["center"] < 1330]
+        upper = [peak for peak in self.peaks if peak["center"] > 1330]
+
+        self.diad = []
+        for region in (lower, upper):
+            amplitude_sort = np.argsort([peak["amplitude"] for peak in region])
+            peaks_sorted = np.array(region)[amplitude_sort]
+            self.diad.append(peaks_sorted[-1])
+
+        self.diad_split = abs(self.diad[0]["center"] - self.diad[1]["center"])
+
+    def diad_curves(self, window=8, stepsize=0.5) -> Tuple[npt.NDArray, npt.NDArray]:
+        """
+        Get diad curves from fitted parameters
+
+        Parameters
+        ----------
+        window  :   int, default 8
+            width parameter of the x-axis window within which curves are calculated. Actual width is calculated as ``window`` :math:`\\times` *peak width*.
+        stepsize    : float
+            x-axis stepsize
+
+        Returns
+        -------
+        npt.NDArray, npt.NDArray
+            (x, 2) shaped arrays with columns x, y for each diad peak.
+
+        """
+
+        if self.diad is None:
+            raise AttributeError("Run 'FermiDiad()' first!")
+
+        results = []
+
+        for peak in self.diad.values():
+            width = peak["width"]
+
+            start = peak["center"] - window * width
+            stop = peak["center"] + window * width
+
+            x = np.arange(start=start, stop=stop, step=stepsize)
+            y = c.GaussLorentz(x=x, **peak)
+
+            results.append(np.vstack([x, y]))
+
+        return results
```

### Comparing `ramCOH-1.1.0/ramCOH/raman/glass.py` & `ramCOH-1.1.1/ramCOH/raman/glass.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,305 +1,305 @@
-"""
-======
-Glass
-======
-The glass module provides a Raman processing class for processing spectra of silicate glasses, with tailored algorithms for quantifying their water content.
-"""
-
-from typing import Optional, Tuple, Union
-
-import numpy as np
-import numpy.typing as npt
-import scipy.optimize as opt
-
-from ramCOH.raman.baseclass import RamanProcessing
-from ramCOH.raman.baseline_regions import default_birs
-from ramCOH.signal_processing import functions as f
-
-
-class Glass(RamanProcessing):
-    """
-    A subclass of :py:class:`~ramCOH.raman.baseclass.RamanProcessing`, extended with methods for quantifying water contents of silicate glasses
-
-    Parameters
-    ----------
-    x   :   array
-        1D array with x-axis data
-    y   :   array of float or int
-        1D array with intensity data
-    **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-    Other parameters
-    ----------------
-    laser   :   float, optional
-        laser wavelength in nm
-
-    Attributes
-    ----------
-    birs_default    :   ndarray
-        (n, 2) shaped array with left and right boundaries of default baseline interpolation regions
-    Si_SNR  : float
-        silicate region signal:noise ratio
-    H2O_SNR :   float
-        water region signal:noise ratio
-    SiH2Oareas  : tuple(float, float)
-        Area underneath peaks in the silicate and water regions
-
-    """
-
-    # baseline regions
-    birs_default = default_birs["glass"]
-
-    def __init__(self, x: npt.NDArray, y: npt.NDArray, **kwargs):
-
-        super().__init__(x, y, **kwargs)
-        self._processing.update({"long_corrected": False})
-
-        self.H2O_SNR: Optional[float] = None
-        self.Si_SNR: Optional[float] = None
-
-        self.SiH2Oareas: Optional[Tuple[float, float]] = None
-
-    def longCorrect(
-        self, T_C=23.0, normalisation=False, inplace=True, **kwargs
-    ) -> None:
-        """
-        Long correction of Raman signal intensities
-
-        Correction for temperature and excitation line effects\ [1]_ according to:
-
-        .. math::
-            I = I_{obs} * \left\{ \\nu^{3}_{0} \left[ 1 - exp(-hc\\nu/kT) \\right] \\nu / (\\nu_{0} - \\nu)^{4} \\right\}
-
-        where:
-
-        * :math:`I` = corrected intensity
-        * :math:`I_{obs}` = observed intensity
-        * :math:`\\nu_{0}` = wavenumber of the incident laser (:math:`m^{-1}`)
-        * :math:`\\nu` = measured wavenumber (:math:`m^{-1}`)
-        * :math:`T` = temperature in degrees Kelvin
-
-        with constants:
-
-        * :math:`h` = Planck constant
-        * :math:`k` = Boltzmann constant
-        * :math:`c` = speed of light
-
-        With constant values taken from :py:mod:`scipy:scipy.constants`.
-        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.signal`.
-
-        Parameters
-        ----------
-        T_C :   float, default 23.0
-            temperature during analysis in degrees celsius
-        normalisation   :   bool, default False
-            normalise Long corrected spectrum to total area
-        inplace :   bool, default True
-            return Long corrected spectrum when False
-        **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-        Other parameters
-        ----------------
-        y   :   str, Optional
-            name of the spectrum to be treated
-
-
-        References
-        ----------
-        .. [1] Long, D.A. (1977) Raman Spectroscopy, 276 p. MacGraw-Hill, New York.
-        """
-
-        laser = kwargs.get("laser", self.laser)
-        if not laser:
-            raise ValueError("laser wavelength not set!")
-
-        y = kwargs.get("y", self._spectrumSelect)
-        spectrum = self.signal.get(y)
-
-        long_corrected = f.long_correction(
-            x=self.x,
-            intensities=spectrum,
-            T_C=T_C,
-            laser=laser,
-            normalisation=normalisation,
-        )
-        if inplace:
-            self.signal.add("long_corrected", long_corrected)
-            return
-
-        return long_corrected
-
-    def calculate_SNR(self) -> None:
-        """
-        Calculate signal to noise ratios for silicate and raman peaks
-
-        Noise is calculated with self.calculate_noise and
-        maxima within the silicate and water regions are used as signals.
-
-        silicate and water regions are set with :py:meth:`~ramCOH.raman.water.H2O._get_Si_H2O_regions` and
-        results are stored in :py:attr:`~ramCOH.raman.water.H2O.Si_SNR` and :py:attr:`~ramCOH.raman.water.H2O.H2O_SNR`.
-
-
-        """
-
-        if self.noise is None:
-            self.calculate_noise()
-
-        (Si_left, Si_right), (water_left, water_right) = self._get_Si_H2O_regions()
-        Si_range = (self.x > Si_left) & (self.x < Si_right)
-        water_range = (self.x > water_left) & (self.x < water_right)
-
-        self.Si_SNR = max(self.signal.baseline_corrected[Si_range]) / self.noise
-        self.H2O_SNR = max(self.signal.baseline_corrected[water_range]) / self.noise
-
-    def subtract_interference(
-        self,
-        interference: npt.NDArray,
-        interval: Tuple[Union[float, int], Union[float, int]],
-        smoothing: float,
-        inplace=True,
-        use=False,
-        **kwargs
-    ) -> None:
-        """
-        Subtract interfering signals
-
-        Glass and interfering signal are unmixed by minimising the difference between the unmixed
-        spectrum and an interpolated, ideal spectrum. Interpolated signal is calculated across ``interval``
-        with smoothing splines from :py:func:`csaps:csaps.csaps`,
-        The interpolation region should be a region with intefering peaks bracketed by unaffected signal.
-
-        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.signal`. as *interference_corrected*
-
-
-        Parameters
-        ----------
-        interference    :   array
-            intensities of intefering signal, x-axis must match with original spectrum
-        interval    :   tuple of float
-            lower and upper limit of minimisation interval
-        smoothing   :   float
-            smoothing of interpolation across minimisation interval
-        inplace :   bool, default True
-            return unmixed spectrum if False
-        use :   bool, default False
-            set unmixed spectrum as source for further processing
-        **kwargs    :   dict, optional
-            Optional keyword arguments, see Other parameters
-
-        Other parameters
-        ----------------
-        y   :   str, Optional
-            name of the spectrum to be treated
-
-
-        """
-
-        boundary_left, boundary_right = interval
-        x = self.x
-
-        spectrum = self.signal.get("raw")
-        _, spline_interval, _ = f._interpolate_section(
-            x, spectrum, interpolate=[interval], smooth_factor=smoothing
-        )
-
-        scaling = opt.root(
-            f._root_interference,
-            x0=[0.2, 0],
-            args=(
-                x,
-                interference,
-                spectrum,
-                spline_interval,
-                [boundary_left, boundary_right],
-            ),
-        ).x
-
-        scale, shift = scaling
-        shift = int(shift)
-        interference = f.shift_spectrum(interference, shift)
-        interference = interference * scale
-
-        spectrum_corrected = spectrum - interference
-
-        if inplace:
-            self.signal.add("interference_corrected", spectrum_corrected.copy())
-            if use:
-                # self._spectrumSelect = "interference_corrected"
-                self._processing["interference_corrected"] = True
-            return
-
-        return spectrum_corrected
-
-    def calculate_SiH2Oareas(self) -> Tuple[float, float]:
-        """
-        Calculate areas underneath peaks in the silicate and water regions
-
-        Areas are calculated by trapezoidal integration of regions set by :py:meth:`~ramCOH.raman.water.H2O._get_Si_H2O_regions`
-        Results are stored in :py:attr:`~ramCOH.raman.water.H2O.SiH2Oareas`.
-
-        Returns
-        -------
-        float, float
-            silicate region area, water region area
-
-        """
-
-        if "baseline_corrected" not in self.signal.names:
-            raise RuntimeError("run baseline correction first")
-
-        (Si_left, Si_right), (water_left, water_right) = self._get_Si_H2O_regions()
-        Si_range = (self.x > Si_left) & (self.x < Si_right)
-        water_range = (self.x > water_left) & (self.x < water_right)
-
-        spectrum = self.signal.get("baseline_corrected")
-        SiArea = np.trapz(spectrum[Si_range], self.x[Si_range])
-        H2Oarea = np.trapz(spectrum[water_range], self.x[water_range])
-
-        self.SiH2Oareas = SiArea, H2Oarea
-
-        return self.SiH2Oareas
-
-    def _get_Si_H2O_regions(self) -> Tuple[Tuple[float, float], Tuple[float, float]]:
-        """Limits of the silicate region are calculated from the upper boundary of the lowest wavenumber
-        baseline interpolation region (bir) and the last bir boundary < 1500 cm-1.
-
-        Limits of the water region are calculated from the first bir boundary > 1500 cm-1
-        and the lower limit of the highest wavenumber bir.
-
-        If not enough birs are set, the silicate region is set to 200-1400 cm-1 and the water region to 2000-4000 cm-1
-
-        Returns
-        -------
-        Tuple[float, float], Tuple[float, float]
-            silicate region boundaries, water region boundaries
-
-
-        :meta public:
-        """
-
-        bir_boundaries = self.birs.flatten()
-
-        Si_left = bir_boundaries[1]
-        try:
-            Si_right = bir_boundaries[bir_boundaries < 1500][-1]
-        except IndexError:
-            Si_right = 1400
-
-        try:
-            water_left = bir_boundaries[bir_boundaries > 1500][0]
-        except IndexError:
-            water_left = 2000
-
-        water_right = bir_boundaries[-2]
-
-        Si_range = (self.x > Si_left) & (self.x < Si_right)
-        water_range = (self.x > water_left) & (self.x < water_right)
-
-        if sum(Si_range) == 0:
-            Si_left, Si_right = 200, 1400
-        if sum(water_range) == 0:
-            water_left, water_right = 2000, 4000
-
-        return (Si_left, Si_right), (water_left, water_right)
+"""
+======
+Glass
+======
+The glass module provides a Raman processing class for processing spectra of silicate glasses, with tailored algorithms for quantifying their water content.
+"""
+
+from typing import Optional, Tuple, Union
+
+import numpy as np
+import numpy.typing as npt
+import scipy.optimize as opt
+
+from ramCOH.raman.baseclass import RamanProcessing
+from ramCOH.raman.baseline_regions import default_birs
+from ramCOH.signal_processing import functions as f
+
+
+class Glass(RamanProcessing):
+    """
+    A subclass of :py:class:`~ramCOH.raman.baseclass.RamanProcessing`, extended with methods for quantifying water contents of silicate glasses
+
+    Parameters
+    ----------
+    x   :   array
+        1D array with x-axis data
+    y   :   array of float or int
+        1D array with intensity data
+    **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+    Other parameters
+    ----------------
+    laser   :   float, optional
+        laser wavelength in nm
+
+    Attributes
+    ----------
+    birs_default    :   ndarray
+        (n, 2) shaped array with left and right boundaries of default baseline interpolation regions
+    Si_SNR  : float
+        silicate region signal:noise ratio
+    H2O_SNR :   float
+        water region signal:noise ratio
+    SiH2Oareas  : tuple(float, float)
+        Area underneath peaks in the silicate and water regions
+
+    """
+
+    # baseline regions
+    birs_default = default_birs["glass"]
+
+    def __init__(self, x: npt.NDArray, y: npt.NDArray, **kwargs):
+
+        super().__init__(x, y, **kwargs)
+        self._processing.update({"long_corrected": False})
+
+        self.H2O_SNR: Optional[float] = None
+        self.Si_SNR: Optional[float] = None
+
+        self.SiH2Oareas: Optional[Tuple[float, float]] = None
+
+    def longCorrect(
+        self, T_C=23.0, normalisation=False, inplace=True, **kwargs
+    ) -> None:
+        """
+        Long correction of Raman signal intensities
+
+        Correction for temperature and excitation line effects\ [1]_ according to:
+
+        .. math::
+            I = I_{obs} * \left\{ \\nu^{3}_{0} \left[ 1 - exp(-hc\\nu/kT) \\right] \\nu / (\\nu_{0} - \\nu)^{4} \\right\}
+
+        where:
+
+        * :math:`I` = corrected intensity
+        * :math:`I_{obs}` = observed intensity
+        * :math:`\\nu_{0}` = wavenumber of the incident laser (:math:`m^{-1}`)
+        * :math:`\\nu` = measured wavenumber (:math:`m^{-1}`)
+        * :math:`T` = temperature in degrees Kelvin
+
+        with constants:
+
+        * :math:`h` = Planck constant
+        * :math:`k` = Boltzmann constant
+        * :math:`c` = speed of light
+
+        With constant values taken from :py:mod:`scipy:scipy.constants`.
+        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.signal`.
+
+        Parameters
+        ----------
+        T_C :   float, default 23.0
+            temperature during analysis in degrees celsius
+        normalisation   :   bool, default False
+            normalise Long corrected spectrum to total area
+        inplace :   bool, default True
+            return Long corrected spectrum when False
+        **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+        Other parameters
+        ----------------
+        y   :   str, Optional
+            name of the spectrum to be treated
+
+
+        References
+        ----------
+        .. [1] Long, D.A. (1977) Raman Spectroscopy, 276 p. MacGraw-Hill, New York.
+        """
+
+        laser = kwargs.get("laser", self.laser)
+        if not laser:
+            raise ValueError("laser wavelength not set!")
+
+        y = kwargs.get("y", self._spectrumSelect)
+        spectrum = self.signal.get(y)
+
+        long_corrected = f.long_correction(
+            x=self.x,
+            intensities=spectrum,
+            T_C=T_C,
+            laser=laser,
+            normalisation=normalisation,
+        )
+        if inplace:
+            self.signal.add("long_corrected", long_corrected)
+            return
+
+        return long_corrected
+
+    def calculate_SNR(self) -> None:
+        """
+        Calculate signal to noise ratios for silicate and raman peaks
+
+        Noise is calculated with self.calculate_noise and
+        maxima within the silicate and water regions are used as signals.
+
+        silicate and water regions are set with :py:meth:`~ramCOH.raman.glass.Glass._get_Si_H2O_regions` and
+        results are stored in :py:attr:`~ramCOH.raman.glass.Glass.Si_SNR` and :py:attr:`~ramCOH.raman.glass.Glass.H2O_SNR`.
+
+
+        """
+
+        if self.noise is None:
+            self.calculate_noise()
+
+        (Si_left, Si_right), (water_left, water_right) = self._get_Si_H2O_regions()
+        Si_range = (self.x > Si_left) & (self.x < Si_right)
+        water_range = (self.x > water_left) & (self.x < water_right)
+
+        self.Si_SNR = max(self.signal.baseline_corrected[Si_range]) / self.noise
+        self.H2O_SNR = max(self.signal.baseline_corrected[water_range]) / self.noise
+
+    def subtract_interference(
+        self,
+        interference: npt.NDArray,
+        interval: Tuple[Union[float, int], Union[float, int]],
+        smoothing: float,
+        inplace=True,
+        use=False,
+        **kwargs
+    ) -> None:
+        """
+        Subtract interfering signals
+
+        Glass and interfering signal are unmixed by minimising the difference between the unmixed
+        spectrum and an interpolated, ideal spectrum. Interpolated signal is calculated across ``interval``
+        with smoothing splines from :py:func:`csaps:csaps.csaps`,
+        The interpolation region should be a region with intefering peaks bracketed by unaffected signal.
+
+        Results are stored in :py:attr:`~ramCOH.raman.baseclass.RamanProcessing.signal`. as *interference_corrected*
+
+
+        Parameters
+        ----------
+        interference    :   array
+            intensities of intefering signal, x-axis must match with original spectrum
+        interval    :   tuple of float
+            lower and upper limit of minimisation interval
+        smoothing   :   float
+            smoothing of interpolation across minimisation interval
+        inplace :   bool, default True
+            return unmixed spectrum if False
+        use :   bool, default False
+            set unmixed spectrum as source for further processing
+        **kwargs    :   dict, optional
+            Optional keyword arguments, see Other parameters
+
+        Other parameters
+        ----------------
+        y   :   str, Optional
+            name of the spectrum to be treated
+
+
+        """
+
+        boundary_left, boundary_right = interval
+        x = self.x
+
+        spectrum = self.signal.get("raw")
+        _, spline_interval, _ = f._interpolate_section(
+            x, spectrum, interpolate=[interval], smooth_factor=smoothing
+        )
+
+        scaling = opt.root(
+            f._root_interference,
+            x0=[0.2, 0],
+            args=(
+                x,
+                interference,
+                spectrum,
+                spline_interval,
+                [boundary_left, boundary_right],
+            ),
+        ).x
+
+        scale, shift = scaling
+        shift = int(shift)
+        interference = f.shift_spectrum(interference, shift)
+        interference = interference * scale
+
+        spectrum_corrected = spectrum - interference
+
+        if inplace:
+            self.signal.add("interference_corrected", spectrum_corrected.copy())
+            if use:
+                # self._spectrumSelect = "interference_corrected"
+                self._processing["interference_corrected"] = True
+            return
+
+        return spectrum_corrected
+
+    def calculate_SiH2Oareas(self) -> Tuple[float, float]:
+        """
+        Calculate areas underneath peaks in the silicate and water regions
+
+        Areas are calculated by trapezoidal integration of regions set by :py:meth:`~ramCOH.raman.glass.Glass._get_Si_H2O_regions`
+        Results are stored in :py:attr:`~ramCOH.raman.glass.Glass.SiH2Oareas`.
+
+        Returns
+        -------
+        float, float
+            silicate region area, water region area
+
+        """
+
+        if "baseline_corrected" not in self.signal.names:
+            raise RuntimeError("run baseline correction first")
+
+        (Si_left, Si_right), (water_left, water_right) = self._get_Si_H2O_regions()
+        Si_range = (self.x > Si_left) & (self.x < Si_right)
+        water_range = (self.x > water_left) & (self.x < water_right)
+
+        spectrum = self.signal.get("baseline_corrected")
+        SiArea = np.trapz(spectrum[Si_range], self.x[Si_range])
+        H2Oarea = np.trapz(spectrum[water_range], self.x[water_range])
+
+        self.SiH2Oareas = SiArea, H2Oarea
+
+        return self.SiH2Oareas
+
+    def _get_Si_H2O_regions(self) -> Tuple[Tuple[float, float], Tuple[float, float]]:
+        """Limits of the silicate region are calculated from the upper boundary of the lowest wavenumber
+        baseline interpolation region (bir) and the last bir boundary < 1500 cm-1.
+
+        Limits of the water region are calculated from the first bir boundary > 1500 cm-1
+        and the lower limit of the highest wavenumber bir.
+
+        If not enough birs are set, the silicate region is set to 200-1400 cm-1 and the water region to 2000-4000 cm-1
+
+        Returns
+        -------
+        Tuple[float, float], Tuple[float, float]
+            silicate region boundaries, water region boundaries
+
+
+        :meta public:
+        """
+
+        bir_boundaries = self.birs.flatten()
+
+        Si_left = bir_boundaries[1]
+        try:
+            Si_right = bir_boundaries[bir_boundaries < 1500][-1]
+        except IndexError:
+            Si_right = 1400
+
+        try:
+            water_left = bir_boundaries[bir_boundaries > 1500][0]
+        except IndexError:
+            water_left = 2000
+
+        water_right = bir_boundaries[-2]
+
+        Si_range = (self.x > Si_left) & (self.x < Si_right)
+        water_range = (self.x > water_left) & (self.x < water_right)
+
+        if sum(Si_range) == 0:
+            Si_left, Si_right = 200, 1400
+        if sum(water_range) == 0:
+            water_left, water_right = 2000, 4000
+
+        return (Si_left, Si_right), (water_left, water_right)
```

### Comparing `ramCOH-1.1.0/ramCOH/raman/neon.py` & `ramCOH-1.1.1/ramCOH/raman/neon.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-"""
-======
-Neon
-======
-The neon module provides a Raman processing class for processing neon emission spectra.
-"""
-
-import itertools as it
-from typing import Optional
-
-import numpy as np
-import numpy.typing as npt
-
-from ramCOH.raman.baseclass import RamanProcessing
-from ramCOH.raman.baseline_regions import default_birs
-from ramCOH.signal_processing import functions as f
-
-
-class Neon(RamanProcessing):
-    """
-    A subclass of :py:class:`~ramCOH.raman.baseclass.RamanProcessing`, extended with methods for Raman streching and offset correction.
-
-    Attributes
-    ----------
-    emission_peaks  :   array of float
-        theoretical neon emission lines (cm\ :sup:`-1`)
-    observed_peaks    :   array of float
-        observed neon emission lines (cm\ :sup:`-1`)
-    correction_factor   :   float
-        stretching correction factor (cm\ :sup:`-1`)
-    offset  :   float
-        offset correction factor (cm\ :sup:`-1`)
-    """
-
-    # Baseline regions
-    birs_default = default_birs["neon"]
-
-    emission_peaks: Optional[npt.NDArray] = None
-    observed_peaks: Optional[npt.NDArray] = None
-
-    correction_factor: Optional[float] = None
-    offset: Optional[float] = None
-
-    def __init__(self, x: npt.NDArray, y: npt.NDArray, laser: float):
-
-        super().__init__(x=x, y=y, laser=laser)
-
-    def deconvolve(
-        self,
-        peak_height=2,
-        residuals_theshold=10,
-        min_amplitude=8,
-        min_peak_width=2,
-        fit_window=4,
-        max_iterations=3,
-        noise=None,
-        **kwargs,
-    ):
-        """
-        :meta private:
-        """
-        return super().deconvolve(
-            peak_prominence=peak_height,
-            residuals_threshold=residuals_theshold,
-            baseline0=True,
-            min_amplitude=min_amplitude,
-            min_peak_width=min_peak_width,
-            fit_window=fit_window,
-            noise=noise,
-            max_iterations=max_iterations,
-            **kwargs,
-        )
-
-    def neonCorrection(
-        self, left_nm=565.666, right_nm=574.83, search_window=6, **kwargs
-    ):
-        """
-        Calculate stretching and offset correction factors between observed and theoretical Neon emission lines.
-
-        Compare theoretical neon emission lines near the calibration lines ``left_nm`` and ``right_nm`` with
-        observed peaks. Correction for stretching is calculated as the ratio of the inter calibration line distances of
-        theoretical and observed lines. Offset correction is calculated as the difference between the observed and theoretical position of ``left_nm``.
-
-
-        Results are stored in :py:attr:`~ramCOH.raman.neon.Neon.correction_factor` and :py:attr:`~ramCOH.raman.neon.Neon.offset`.
-
-        Parameters
-        ----------
-        left_nm :   float, default 565.666
-            position of the left calibration line in nm
-        right_nm :   float, default 574.83
-            position of the right calibration line in nm
-        search_window   :   int
-            Half-width (cm\ :sup:`-1`) of the peak search window around theoretical emission lines .
-        """
-        laser = kwargs.get("laser", self.laser)
-
-        if self.peaks is None:
-            raise NameError("peaks not found, run fitPeaks first")
-
-        neon_emission = f.neonEmission(laser=laser)
-        left = np.round(
-            np.float(
-                neon_emission.iloc[:, 4][
-                    np.isclose(left_nm, neon_emission.iloc[:, 1], atol=0.001)
-                ]
-            ),
-            2,
-        )
-        right = np.round(
-            np.float(
-                neon_emission.iloc[:, 4][
-                    np.isclose(right_nm, neon_emission.iloc[:, 1], atol=0.001)
-                ]
-            ),
-            2,
-        )
-
-        # All emission lines within spectrum limits
-        neon_emission_trimmed = np.array(
-            neon_emission.iloc[:, 4][
-                (neon_emission.iloc[:, 4] > self.x.min())
-                & (neon_emission.iloc[:, 4] < self.x.max())
-            ]
-        )
-
-        # theoretical emission line positions with a match found in spectrum
-        self.emission_peaks = np.array([])
-        # measured emission line positions
-        self.observerd_peaks = np.array([])
-
-        for i, j in self.peaks.items():
-            peak = j["center"]
-            emission_check = np.isclose(
-                peak, neon_emission_trimmed, atol=search_window, rtol=0
-            )
-
-            if emission_check.sum() == 1:
-                self.emission_peaks = np.append(
-                    self.emission_peaks, neon_emission_trimmed[emission_check].tolist()
-                )
-                self.observerd_peaks = np.append(self.observerd_peaks, peak)
-            elif emission_check.sum() > 1:
-                raise RuntimeError(
-                    f"multiple emission line fits found at {peak: .2f} cm$^{-1}$"
-                )
-
-        # find correction factor for the calibration lines
-        if not np.isin([left, right], np.round(self.emission_peaks, 2)).sum() == 2:
-            raise RuntimeError("calibration lines not found in spectrum")
-
-        # boolean array for the location of left and right calibration lines
-        calibration_lines = np.array(
-            np.isclose(left, self.emission_peaks, atol=0.001)
-            + np.isclose(right, self.emission_peaks, atol=0.001)
-        )
-        # boolean to index
-        calibration_lines = list(
-            it.compress(range(len(calibration_lines)), calibration_lines)
-        )
-        # indices for differenced array
-        calibration_lines = np.unique(calibration_lines - np.array([0, 1]))
-
-        self.correction_factor = np.float(
-            np.sum(np.diff(self.emission_peaks)[calibration_lines])
-            / np.sum(np.diff(self.observerd_peaks)[calibration_lines])
-        )
-        self.offset = np.float(
-            self.observerd_peaks[np.isclose(left, self.observerd_peaks, atol=10)]
-            - self.emission_peaks[np.isclose(left, self.emission_peaks, atol=0.1)]
-        )
+"""
+======
+Neon
+======
+The neon module provides a Raman processing class for processing neon emission spectra.
+"""
+
+import itertools as it
+from typing import Optional
+
+import numpy as np
+import numpy.typing as npt
+
+from ramCOH.raman.baseclass import RamanProcessing
+from ramCOH.raman.baseline_regions import default_birs
+from ramCOH.signal_processing import functions as f
+
+
+class Neon(RamanProcessing):
+    """
+    A subclass of :py:class:`~ramCOH.raman.baseclass.RamanProcessing`, extended with methods for Raman streching and offset correction.
+
+    Attributes
+    ----------
+    emission_peaks  :   array of float
+        theoretical neon emission lines (cm\ :sup:`-1`)
+    observed_peaks    :   array of float
+        observed neon emission lines (cm\ :sup:`-1`)
+    correction_factor   :   float
+        stretching correction factor (cm\ :sup:`-1`)
+    offset  :   float
+        offset correction factor (cm\ :sup:`-1`)
+    """
+
+    # Baseline regions
+    birs_default = default_birs["neon"]
+
+    emission_peaks: Optional[npt.NDArray] = None
+    observed_peaks: Optional[npt.NDArray] = None
+
+    correction_factor: Optional[float] = None
+    offset: Optional[float] = None
+
+    def __init__(self, x: npt.NDArray, y: npt.NDArray, laser: float):
+
+        super().__init__(x=x, y=y, laser=laser)
+
+    def deconvolve(
+        self,
+        peak_height=2,
+        residuals_theshold=10,
+        min_amplitude=8,
+        min_peak_width=2,
+        fit_window=4,
+        max_iterations=3,
+        noise=None,
+        **kwargs,
+    ):
+        """
+        :meta private:
+        """
+        return super().deconvolve(
+            peak_prominence=peak_height,
+            residuals_threshold=residuals_theshold,
+            baseline0=True,
+            min_amplitude=min_amplitude,
+            min_peak_width=min_peak_width,
+            fit_window=fit_window,
+            noise=noise,
+            max_iterations=max_iterations,
+            **kwargs,
+        )
+
+    def neonCorrection(
+        self, left_nm=565.666, right_nm=574.83, search_window=6, **kwargs
+    ):
+        """
+        Calculate stretching and offset correction factors between observed and theoretical Neon emission lines.
+
+        Compare theoretical neon emission lines near the calibration lines ``left_nm`` and ``right_nm`` with
+        observed peaks. Correction for stretching is calculated as the ratio of the inter calibration line distances of
+        theoretical and observed lines. Offset correction is calculated as the difference between the observed and theoretical position of ``left_nm``.
+
+
+        Results are stored in :py:attr:`~ramCOH.raman.neon.Neon.correction_factor` and :py:attr:`~ramCOH.raman.neon.Neon.offset`.
+
+        Parameters
+        ----------
+        left_nm :   float, default 565.666
+            position of the left calibration line in nm
+        right_nm :   float, default 574.83
+            position of the right calibration line in nm
+        search_window   :   int
+            Half-width (cm\ :sup:`-1`) of the peak search window around theoretical emission lines .
+        """
+        laser = kwargs.get("laser", self.laser)
+
+        if self.peaks is None:
+            raise NameError("peaks not found, run fitPeaks first")
+
+        neon_emission = f.neonEmission(laser=laser)
+        left = np.round(
+            np.float(
+                neon_emission.iloc[:, 4][
+                    np.isclose(left_nm, neon_emission.iloc[:, 1], atol=0.001)
+                ]
+            ),
+            2,
+        )
+        right = np.round(
+            np.float(
+                neon_emission.iloc[:, 4][
+                    np.isclose(right_nm, neon_emission.iloc[:, 1], atol=0.001)
+                ]
+            ),
+            2,
+        )
+
+        # All emission lines within spectrum limits
+        neon_emission_trimmed = np.array(
+            neon_emission.iloc[:, 4][
+                (neon_emission.iloc[:, 4] > self.x.min())
+                & (neon_emission.iloc[:, 4] < self.x.max())
+            ]
+        )
+
+        # theoretical emission line positions with a match found in spectrum
+        self.emission_peaks = np.array([])
+        # measured emission line positions
+        self.observerd_peaks = np.array([])
+
+        for i, j in self.peaks.items():
+            peak = j["center"]
+            emission_check = np.isclose(
+                peak, neon_emission_trimmed, atol=search_window, rtol=0
+            )
+
+            if emission_check.sum() == 1:
+                self.emission_peaks = np.append(
+                    self.emission_peaks, neon_emission_trimmed[emission_check].tolist()
+                )
+                self.observerd_peaks = np.append(self.observerd_peaks, peak)
+            elif emission_check.sum() > 1:
+                raise RuntimeError(
+                    f"multiple emission line fits found at {peak: .2f} cm$^{-1}$"
+                )
+
+        # find correction factor for the calibration lines
+        if not np.isin([left, right], np.round(self.emission_peaks, 2)).sum() == 2:
+            raise RuntimeError("calibration lines not found in spectrum")
+
+        # boolean array for the location of left and right calibration lines
+        calibration_lines = np.array(
+            np.isclose(left, self.emission_peaks, atol=0.001)
+            + np.isclose(right, self.emission_peaks, atol=0.001)
+        )
+        # boolean to index
+        calibration_lines = list(
+            it.compress(range(len(calibration_lines)), calibration_lines)
+        )
+        # indices for differenced array
+        calibration_lines = np.unique(calibration_lines - np.array([0, 1]))
+
+        self.correction_factor = np.float(
+            np.sum(np.diff(self.emission_peaks)[calibration_lines])
+            / np.sum(np.diff(self.observerd_peaks)[calibration_lines])
+        )
+        self.offset = np.float(
+            self.observerd_peaks[np.isclose(left, self.observerd_peaks, atol=10)]
+            - self.emission_peaks[np.isclose(left, self.emission_peaks, atol=0.1)]
+        )
```

### Comparing `ramCOH-1.1.0/ramCOH/signal_processing/curve_fitting.py` & `ramCOH-1.1.1/ramCOH/signal_processing/curve_fitting.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-import warnings
-
-# import csaps as cs
-import numpy as np
-import scipy.optimize as opt
-from scipy import signal
-
-import ramCOH.signal_processing.curves as c
-
-
-def _merge_overlapping_ranges(ranges):
-    """
-    Merge
-
-    Parameters
-    ----------
-    ranges : List[List]
-        list of lists containing start and end for per range
-
-    Returns
-    -------
-    merged ranges : List[List]
-        [xmin, xmax] of merged ranges
-    """
-
-    merged = [False] * len(ranges)
-
-    merged_ranges = []
-
-    for k, (area1, area2) in enumerate(zip(ranges[:-1], ranges[1:])):
-
-        if merged[k]:
-            if (k + 2) == len(ranges):
-                merged_ranges.append(area2)
-            continue
-
-        if np.max(area1) > np.min(area2):
-            merged_ranges.append([np.min(area1 + area2), np.max(area1 + area2)])
-            merged[k + 1] = True
-        else:
-            merged_ranges.append(sorted(area1))
-            if (k + 2) == len(ranges):
-                merged_ranges.append(area2)
-
-    return merged_ranges
-
-
-def _get_peakFit_ranges(centers, half_widths, fit_window=4, merge_overlap=True):
-    """
-    Parameters
-    ----------
-    centers : array-like
-        centers of peaks
-    half_widths : array-like
-        Full width at half maximum of peaks
-    fit_window : int, float
-        ranges are calculated as centers +- (FWHM * fit_window)
-    merge_overlap : bool
-        merge ranges that overlap
-
-    Returns
-    -------
-    ranges : list[list]
-        [xmin, xmax] of ranges around peak centers
-    """
-
-    if isinstance(centers, (int, float)):
-        minimum = centers - fit_window * half_widths
-        maximum = centers + fit_window * half_widths
-
-        return [minimum, maximum]
-
-    sort = np.argsort(centers)
-    centers = centers[sort]
-    half_widths = half_widths[sort]
-
-    ranges = []
-
-    for center, width in zip(centers, half_widths):
-        minimum = center - fit_window * width
-        maximum = center + fit_window * width
-        ranges.append([minimum, maximum])
-
-    if merge_overlap:
-        merged_ranges = _merge_overlapping_ranges(ranges)
-
-        merged = len(centers) - len(merged_ranges)
-
-        while merged > 0:
-
-            old = len(merged_ranges)
-            merged_ranges = _merge_overlapping_ranges(merged_ranges)
-            merged = old - len(merged_ranges)
-            if len(merged_ranges) == 1:
-                break
-
-        ranges = merged_ranges
-
-    return ranges
-
-
-def _trimxy_ranges(x, y, ranges):
-    """ "
-    Parameters
-    ----------
-    x : array-like
-        x
-    y : array-like
-        y
-    ranges : list, list[list]
-        ranges in x as [xmin, xmax] to which y and y will be trimmed
-
-    Returns
-    -------
-    trimmed_xy : list, list[list]
-        x and y trimmed to ranges
-    """
-
-    if not isinstance(ranges[0], list):
-        trim = (x > ranges[0]) & (x < ranges[1])
-        return [x[trim], y[trim]]
-
-    trimmed_xy = []
-
-    for range in ranges:
-        trim = (x > range[0]) & (x < range[1])
-        trimmed_xy.append([x[trim], y[trim]])
-
-    return trimmed_xy
-
-
-def _trim_peakFit_ranges(x, y, centers, half_widths, fit_window=4, merge_overlap=True):
-    """
-    Paramters
-    ---------
-    x : array-like
-        x
-    y : array-like
-        y
-    centers : array-like
-        centers of peaks
-    half-widths : array-like
-        Full width at half maximum (FWHM) for peaks
-    fit_window : int, float
-        ranges are calculated as centers +- FWHM * fit_window
-    merge_overlap : bool
-        merge ranges that overlap
-
-    Returns
-    -------
-    trimmed ranges : list, list[list]
-        x and y trimmed around every peak center
-    """
-    ranges = _get_peakFit_ranges(
-        centers, half_widths, fit_window=fit_window, merge_overlap=merge_overlap
-    )
-
-    return _trimxy_ranges(x, y, ranges)
-
-
-def _find_peak_parameters(x, y, prominence, **kwargs):
-    """
-    Paramters
-    ---------
-    x : array-like
-        x
-    y : array-like
-        y
-    prominence : int, float
-        prominence of peaks, passed to scipy.signal.find_peaks
-    **kwargs
-        passed to scipy.signal.find_peaks
-
-    Returns
-    -------
-    amplitudes : array
-        amplitudes of peaks
-    centers : array
-        centers of peaks
-    widths : array
-        widths of peaks
-    """
-
-    peak_positions, props = signal.find_peaks(y, prominence=prominence, **kwargs)
-    prominence_data = tuple(
-        props[key] for key in ("prominences", "left_bases", "right_bases")
-    )
-
-    amplitudes, centers = y[peak_positions], x[peak_positions]
-    # full width half maximum in x
-    widths = signal.peak_widths(
-        y, peak_positions, rel_height=0.5, prominence_data=prominence_data
-    )[0] * abs(np.diff(x).mean())
-
-    sort = np.argsort(centers)
-
-    amplitudes = amplitudes[sort]
-    centers = centers[sort]
-    widths = widths[sort]
-
-    return amplitudes, centers, widths
-
-
-def diad(x, y, peak_prominence=40, fit_window=8, curve="GL"):
-    """
-    Paramters
-    ---------
-
-    Returns
-    -------
-    """
-    # Fit curves to the two highest peaks in the 1250 - 1450cm-1 window
-
-    # set up the cost function
-    curveDict = {"GL": c.GaussLorentz, "G": c.Gaussian, "L": c.Lorentzian}
-    residuals = lambda params, x, spectrum: curveDict[curve](x, *params) - spectrum
-
-    # check if the diad is within range of the spectrum
-    if (x.min() > 1250) | (x.max() < 1450):
-        raise RuntimeError("spectrum not within 1250 - 1450cm-1")
-
-    y = y[(x > 1250) & (x < 1450)]
-    x = x[(x > 1250) & (x < 1450)]
-
-    # convert peak prominence from relative to absolute
-    peak_prominence = (peak_prominence * 100) / np.max(y)
-    # find initial guesses for peak fitting
-    amplitudes, centers, widths = _find_peak_parameters(
-        x=x, y=y, prominence=peak_prominence
-    )
-
-    if amplitudes.shape[0] < 2:
-        raise RuntimeError("less than two peaks found")
-    if amplitudes.shape[0] > 2:
-        warnings.warn("more than two peaks found")
-
-    # Sort peaks low to high amplitude and select the two highest
-    sort_index = np.argsort(amplitudes)
-    amplitudes = amplitudes[sort_index][-2:]
-    centers = centers[sort_index][-2:]
-    widths = widths[sort_index][-2:]
-    # Gaussian - Lorentzian mixing paramter
-    shape = 0.5
-    # baselevel, should be 0 for baseline corrected spectra
-    baselevel = 0
-
-    # Set bounds for fitting algorithm (amplitude, center, width, baselevel, shape)
-    x_range = x.max() - x.min()
-    if curve == "GL":
-        bounds = (
-            [0, x.min(), 0, -np.inf, 0],
-            [y.max() * 2, x.max(), x_range, y.max(), 1],
-        )
-    else:
-        bounds = (-np.inf, np.inf)
-
-    # Initialise output variables
-    fit_params = []
-    fit_x = []
-    # Fit curves to the two peaks
-    for amplitude, center, width in zip(amplitudes, centers, widths):
-        # Set initial guesses
-        init_values = np.array([amplitude, center, width, baselevel])
-        if curve == "GL":
-            init_values = np.append(init_values, shape)
-
-        x_fit, y_fit = _trim_peakFit_ranges(x, y, center, width, fit_window=fit_window)
-
-        params = opt.least_squares(
-            fun=residuals, x0=init_values, bounds=bounds, args=(x_fit, y_fit)
-        ).x
-        fit_params.append(params)
-        # fit_x.append(x_fit)
-
-    # Unpack output data
-    fit_params1, fit_params2 = fit_params
-    # x1, x2 = fit_x
-
-    # Tidy data
-    labels = ["amplitude", "center", "width", "baselevel"]
-    if curve == "GL":
-        labels.append("shape")
-
-    fit_params1 = {labels[i]: j for i, j in enumerate(fit_params1)}
-    # fit_params1["x"] = x1
-
-    fit_params2 = {labels[i]: j for i, j in enumerate(fit_params2)}
-    # fit_params2["x"] = x2
-
-    return fit_params1, fit_params2
+import warnings
+
+# import csaps as cs
+import numpy as np
+import scipy.optimize as opt
+from scipy import signal
+
+import ramCOH.signal_processing.curves as c
+
+
+def _merge_overlapping_ranges(ranges):
+    """
+    Merge
+
+    Parameters
+    ----------
+    ranges : List[List]
+        list of lists containing start and end for per range
+
+    Returns
+    -------
+    merged ranges : List[List]
+        [xmin, xmax] of merged ranges
+    """
+
+    merged = [False] * len(ranges)
+
+    merged_ranges = []
+
+    for k, (area1, area2) in enumerate(zip(ranges[:-1], ranges[1:])):
+
+        if merged[k]:
+            if (k + 2) == len(ranges):
+                merged_ranges.append(area2)
+            continue
+
+        if np.max(area1) > np.min(area2):
+            merged_ranges.append([np.min(area1 + area2), np.max(area1 + area2)])
+            merged[k + 1] = True
+        else:
+            merged_ranges.append(sorted(area1))
+            if (k + 2) == len(ranges):
+                merged_ranges.append(area2)
+
+    return merged_ranges
+
+
+def _get_peakFit_ranges(centers, half_widths, fit_window=4, merge_overlap=True):
+    """
+    Parameters
+    ----------
+    centers : array-like
+        centers of peaks
+    half_widths : array-like
+        Full width at half maximum of peaks
+    fit_window : int, float
+        ranges are calculated as centers +- (FWHM * fit_window)
+    merge_overlap : bool
+        merge ranges that overlap
+
+    Returns
+    -------
+    ranges : list[list]
+        [xmin, xmax] of ranges around peak centers
+    """
+
+    if isinstance(centers, (int, float)):
+        minimum = centers - fit_window * half_widths
+        maximum = centers + fit_window * half_widths
+
+        return [minimum, maximum]
+
+    sort = np.argsort(centers)
+    centers = centers[sort]
+    half_widths = half_widths[sort]
+
+    ranges = []
+
+    for center, width in zip(centers, half_widths):
+        minimum = center - fit_window * width
+        maximum = center + fit_window * width
+        ranges.append([minimum, maximum])
+
+    if merge_overlap:
+        merged_ranges = _merge_overlapping_ranges(ranges)
+
+        merged = len(centers) - len(merged_ranges)
+
+        while merged > 0:
+
+            old = len(merged_ranges)
+            merged_ranges = _merge_overlapping_ranges(merged_ranges)
+            merged = old - len(merged_ranges)
+            if len(merged_ranges) == 1:
+                break
+
+        ranges = merged_ranges
+
+    return ranges
+
+
+def _trimxy_ranges(x, y, ranges):
+    """ "
+    Parameters
+    ----------
+    x : array-like
+        x
+    y : array-like
+        y
+    ranges : list, list[list]
+        ranges in x as [xmin, xmax] to which y and y will be trimmed
+
+    Returns
+    -------
+    trimmed_xy : list, list[list]
+        x and y trimmed to ranges
+    """
+
+    if not isinstance(ranges[0], list):
+        trim = (x > ranges[0]) & (x < ranges[1])
+        return [x[trim], y[trim]]
+
+    trimmed_xy = []
+
+    for range in ranges:
+        trim = (x > range[0]) & (x < range[1])
+        trimmed_xy.append([x[trim], y[trim]])
+
+    return trimmed_xy
+
+
+def _trim_peakFit_ranges(x, y, centers, half_widths, fit_window=4, merge_overlap=True):
+    """
+    Paramters
+    ---------
+    x : array-like
+        x
+    y : array-like
+        y
+    centers : array-like
+        centers of peaks
+    half-widths : array-like
+        Full width at half maximum (FWHM) for peaks
+    fit_window : int, float
+        ranges are calculated as centers +- FWHM * fit_window
+    merge_overlap : bool
+        merge ranges that overlap
+
+    Returns
+    -------
+    trimmed ranges : list, list[list]
+        x and y trimmed around every peak center
+    """
+    ranges = _get_peakFit_ranges(
+        centers, half_widths, fit_window=fit_window, merge_overlap=merge_overlap
+    )
+
+    return _trimxy_ranges(x, y, ranges)
+
+
+def _find_peak_parameters(x, y, prominence, **kwargs):
+    """
+    Paramters
+    ---------
+    x : array-like
+        x
+    y : array-like
+        y
+    prominence : int, float
+        prominence of peaks, passed to scipy.signal.find_peaks
+    **kwargs
+        passed to scipy.signal.find_peaks
+
+    Returns
+    -------
+    amplitudes : array
+        amplitudes of peaks
+    centers : array
+        centers of peaks
+    widths : array
+        widths of peaks
+    """
+
+    peak_positions, props = signal.find_peaks(y, prominence=prominence, **kwargs)
+    prominence_data = tuple(
+        props[key] for key in ("prominences", "left_bases", "right_bases")
+    )
+
+    amplitudes, centers = y[peak_positions], x[peak_positions]
+    # full width half maximum in x
+    widths = signal.peak_widths(
+        y, peak_positions, rel_height=0.5, prominence_data=prominence_data
+    )[0] * abs(np.diff(x).mean())
+
+    sort = np.argsort(centers)
+
+    amplitudes = amplitudes[sort]
+    centers = centers[sort]
+    widths = widths[sort]
+
+    return amplitudes, centers, widths
+
+
+def diad(x, y, peak_prominence=40, fit_window=8, curve="GL"):
+    """
+    Paramters
+    ---------
+
+    Returns
+    -------
+    """
+    # Fit curves to the two highest peaks in the 1250 - 1450cm-1 window
+
+    # set up the cost function
+    curveDict = {"GL": c.GaussLorentz, "G": c.Gaussian, "L": c.Lorentzian}
+    residuals = lambda params, x, spectrum: curveDict[curve](x, *params) - spectrum
+
+    # check if the diad is within range of the spectrum
+    if (x.min() > 1250) | (x.max() < 1450):
+        raise RuntimeError("spectrum not within 1250 - 1450cm-1")
+
+    y = y[(x > 1250) & (x < 1450)]
+    x = x[(x > 1250) & (x < 1450)]
+
+    # convert peak prominence from relative to absolute
+    peak_prominence = (peak_prominence * 100) / np.max(y)
+    # find initial guesses for peak fitting
+    amplitudes, centers, widths = _find_peak_parameters(
+        x=x, y=y, prominence=peak_prominence
+    )
+
+    if amplitudes.shape[0] < 2:
+        raise RuntimeError("less than two peaks found")
+    if amplitudes.shape[0] > 2:
+        warnings.warn("more than two peaks found")
+
+    # Sort peaks low to high amplitude and select the two highest
+    sort_index = np.argsort(amplitudes)
+    amplitudes = amplitudes[sort_index][-2:]
+    centers = centers[sort_index][-2:]
+    widths = widths[sort_index][-2:]
+    # Gaussian - Lorentzian mixing paramter
+    shape = 0.5
+    # baselevel, should be 0 for baseline corrected spectra
+    baselevel = 0
+
+    # Set bounds for fitting algorithm (amplitude, center, width, baselevel, shape)
+    x_range = x.max() - x.min()
+    if curve == "GL":
+        bounds = (
+            [0, x.min(), 0, -np.inf, 0],
+            [y.max() * 2, x.max(), x_range, y.max(), 1],
+        )
+    else:
+        bounds = (-np.inf, np.inf)
+
+    # Initialise output variables
+    fit_params = []
+    fit_x = []
+    # Fit curves to the two peaks
+    for amplitude, center, width in zip(amplitudes, centers, widths):
+        # Set initial guesses
+        init_values = np.array([amplitude, center, width, baselevel])
+        if curve == "GL":
+            init_values = np.append(init_values, shape)
+
+        x_fit, y_fit = _trim_peakFit_ranges(x, y, center, width, fit_window=fit_window)
+
+        params = opt.least_squares(
+            fun=residuals, x0=init_values, bounds=bounds, args=(x_fit, y_fit)
+        ).x
+        fit_params.append(params)
+        # fit_x.append(x_fit)
+
+    # Unpack output data
+    fit_params1, fit_params2 = fit_params
+    # x1, x2 = fit_x
+
+    # Tidy data
+    labels = ["amplitude", "center", "width", "baselevel"]
+    if curve == "GL":
+        labels.append("shape")
+
+    fit_params1 = {labels[i]: j for i, j in enumerate(fit_params1)}
+    # fit_params1["x"] = x1
+
+    fit_params2 = {labels[i]: j for i, j in enumerate(fit_params2)}
+    # fit_params2["x"] = x2
+
+    return fit_params1, fit_params2
```

### Comparing `ramCOH-1.1.0/ramCOH/signal_processing/curves.py` & `ramCOH-1.1.1/ramCOH/signal_processing/curves.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-"""
-======
-Curves
-======
-Curve shape functions
-
-"""
-
-import numpy as np
-
-
-def Gaussian(x, amplitude, center, width, baselevel=0):
-    """
-    Gaussian curve
-
-    .. math::
-            f(x) = A * exp \left( - \\frac{(x - b)^{2}}{2c^2} \\right) + d
-
-
-    where:
-        * :math:`A` = amplitude
-        * :math:`b` = center
-        * :math:`c` = width (standard deviation)
-        * :math:`d` = baselevel
-
-
-    Parameters
-    ----------
-    x   :   float or array-like
-        x-axis
-    amplitude   :   float
-        maximum peak height
-    center  :   float
-        peak center
-    width   :   float
-        peak width as standard deviation
-    baselevel : float, default 0
-        peak baselevel
-
-
-    Returns
-    -------
-    float, array-like
-        Gaussian curve evaluated at x
-    """
-
-    return amplitude * np.exp(-((x - center) ** 2) / (2 * width**2)) + baselevel
-
-
-def Lorentzian(x, amplitude, center, width, baselevel=0):
-    """
-    Three-parameter Lorentzian curve
-
-    .. math::
-            f(x) = A\left(\\frac{c^2}{(x-b)^2 + c^2}\\right) + d
-
-
-    where:
-        * :math:`A` = amplitude
-        * :math:`b` = center
-        * :math:`c` = width (standard deviation)
-        * :math:`d` = baselevel
-
-    Parameters
-    ----------
-    x   :   float or array-like
-        x-axis
-    amplitude   :   float
-        maximum peak height
-    center  :   float
-        peak center
-    width   :   float
-        peak width as half-width at full maximum
-    baselevel : float, default 0
-        peak baselevel
-
-    Returns
-    -------
-    float, array-like
-        Lorentzian curve evaluated at x
-    """
-
-    return amplitude * width**2 / ((x - center) ** 2 + width**2) + baselevel
-
-
-def GaussLorentz(x, amplitude, center, width, baselevel, shape):
-    """
-    Mixed Gaussian-Lorentzian (Pseudo-Voigt) curve
-
-    .. math::
-            f(x) = Gaussian(x, A * \\alpha, b, c, d) + Lorentzian(x, A * (1 - \\alpha), b, c, d)
-
-    where:
-        * :math:`A` = amplitude
-        * :math:`b` = center
-        * :math:`c` = width (standard deviation)
-        * :math:`d` = baselevel
-        * :math:`\\alpha` = shape
-
-    with parameterisations from :py:func:`~ramCOH.signal_processing.curves.Gaussian` and :py:func:`~ramCOH.signal_processing.curves.Lorentzian`
-
-    Parameters
-    ----------
-    x   :   float or array-like
-        x-axis
-    amplitude   :   float
-        maximum peak height
-    center  :   float
-        peak center
-    width   :   float
-        peak width as half-width at full maximum
-    baselevel : float, default 0
-        peak baselevel
-    shape   :   float
-        mixing parameter between 0 and 1
-
-    Returns
-    -------
-    float, array-like
-        Pseudo-Voigt curve evaluated at x
-
-    """
-
-    return (
-        Gaussian(x, amplitude * (1 - shape), center, width, 0)
-        + Lorentzian(x, amplitude * shape, center, width, 0)
-        + baselevel
-    )
-
-
-def sum_GaussLorentz(x, centers, amplitudes, widths, shapes, baselevels):
-    """
-    add mixed Gauss-Lorentzian curves together
-
-
-    :meta private:
-    """
-
-    peakAmount = len(centers)
-
-    if isinstance(baselevels, (int, float)):
-        baselevels = [baselevels] * peakAmount
-
-    params = [
-        {"center": i, "amplitude": j, "width": k, "baselevel": l, "shape": m}
-        for i, j, k, l, m in zip(centers, amplitudes, widths, baselevels, shapes)
-    ]
-
-    curves = GaussLorentz(x, **params[0])
-
-    for peak in params[1:]:
-        curves = curves + GaussLorentz(x, **peak)
-
-    return curves
+"""
+======
+Curves
+======
+Curve shape functions
+
+"""
+
+import numpy as np
+
+
+def Gaussian(x, amplitude, center, width, baselevel=0):
+    """
+    Gaussian curve
+
+    .. math::
+            f(x) = A * exp \left( - \\frac{(x - b)^{2}}{2c^2} \\right) + d
+
+
+    where:
+        * :math:`A` = amplitude
+        * :math:`b` = center
+        * :math:`c` = width (standard deviation)
+        * :math:`d` = baselevel
+
+
+    Parameters
+    ----------
+    x   :   float or array-like
+        x-axis
+    amplitude   :   float
+        maximum peak height
+    center  :   float
+        peak center
+    width   :   float
+        peak width as standard deviation
+    baselevel : float, default 0
+        peak baselevel
+
+
+    Returns
+    -------
+    float, array-like
+        Gaussian curve evaluated at x
+    """
+
+    return amplitude * np.exp(-((x - center) ** 2) / (2 * width**2)) + baselevel
+
+
+def Lorentzian(x, amplitude, center, width, baselevel=0):
+    """
+    Three-parameter Lorentzian curve
+
+    .. math::
+            f(x) = A\left(\\frac{c^2}{(x-b)^2 + c^2}\\right) + d
+
+
+    where:
+        * :math:`A` = amplitude
+        * :math:`b` = center
+        * :math:`c` = width (standard deviation)
+        * :math:`d` = baselevel
+
+    Parameters
+    ----------
+    x   :   float or array-like
+        x-axis
+    amplitude   :   float
+        maximum peak height
+    center  :   float
+        peak center
+    width   :   float
+        peak width as half-width at full maximum
+    baselevel : float, default 0
+        peak baselevel
+
+    Returns
+    -------
+    float, array-like
+        Lorentzian curve evaluated at x
+    """
+
+    return amplitude * width**2 / ((x - center) ** 2 + width**2) + baselevel
+
+
+def GaussLorentz(x, amplitude, center, width, baselevel, shape):
+    """
+    Mixed Gaussian-Lorentzian (Pseudo-Voigt) curve
+
+    .. math::
+            f(x) = Gaussian(x, A * \\alpha, b, c, d) + Lorentzian(x, A * (1 - \\alpha), b, c, d)
+
+    where:
+        * :math:`A` = amplitude
+        * :math:`b` = center
+        * :math:`c` = width (standard deviation)
+        * :math:`d` = baselevel
+        * :math:`\\alpha` = shape
+
+    with parameterisations from :py:func:`~ramCOH.signal_processing.curves.Gaussian` and :py:func:`~ramCOH.signal_processing.curves.Lorentzian`
+
+    Parameters
+    ----------
+    x   :   float or array-like
+        x-axis
+    amplitude   :   float
+        maximum peak height
+    center  :   float
+        peak center
+    width   :   float
+        peak width as half-width at full maximum
+    baselevel : float, default 0
+        peak baselevel
+    shape   :   float
+        mixing parameter between 0 and 1
+
+    Returns
+    -------
+    float, array-like
+        Pseudo-Voigt curve evaluated at x
+
+    """
+
+    return (
+        Gaussian(x, amplitude * (1 - shape), center, width, 0)
+        + Lorentzian(x, amplitude * shape, center, width, 0)
+        + baselevel
+    )
+
+
+def sum_GaussLorentz(x, centers, amplitudes, widths, shapes, baselevels):
+    """
+    add mixed Gauss-Lorentzian curves together
+
+
+    :meta private:
+    """
+
+    peakAmount = len(centers)
+
+    if isinstance(baselevels, (int, float)):
+        baselevels = [baselevels] * peakAmount
+
+    params = [
+        {"center": i, "amplitude": j, "width": k, "baselevel": l, "shape": m}
+        for i, j, k, l, m in zip(centers, amplitudes, widths, baselevels, shapes)
+    ]
+
+    curves = GaussLorentz(x, **params[0])
+
+    for peak in params[1:]:
+        curves = curves + GaussLorentz(x, **peak)
+
+    return curves
```

### Comparing `ramCOH-1.1.0/ramCOH/signal_processing/deconvolution.py` & `ramCOH-1.1.1/ramCOH/signal_processing/deconvolution.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,194 +1,194 @@
-import warnings
-
-import numpy as np
-import scipy.optimize as opt
-from sklearn.metrics import mean_squared_error
-
-import ramCOH.signal_processing.curve_fitting as cf
-import ramCOH.signal_processing.curves as c
-import ramCOH.signal_processing.functions as f
-
-
-def deconvolve_signal(
-    x,
-    y,
-    min_peak_width=4,
-    min_amplitude=1,
-    residuals_threshold=10,
-    max_iterations=5,
-    baseline0=True,
-    noise=None,
-):
-    """
-    Parameters
-    ----------
-    x : array-like
-        x
-    y : array-like
-        y
-    noise_threshold : float
-        Fit is accepted when the standard deviation of the fit residuals fall below (noise on y) * noise_threshold
-    min_peak_width : int, float
-        minimum width of fitted peaks (full width at half maximum) in x stepsize.
-    min_amplitude : int, float
-        minium amplitude of fitted peaks as a factor of noise on y.
-    baseline0 : bool
-        fix baselevel of fitted curves to 0
-    noise : float, int
-        Absolute noise on y
-    max_iterations : int
-        maximum loop iterations. One new curve is added each loop
-
-    Returns
-    -------
-    fitParams : list[list]
-        fitted parameters for sum_GaussLorentz
-    R2_noise : float
-        R squared of fit result to y, adjusted for noise (on y)
-    fit_noise : float
-        standard deviation on the residuals of y and the fit result
-    """
-
-    # Calculate noise on the total signal
-    # if noise is None:
-    #     noise, _ = f._calculate_noise(x=x, y=y)
-
-    # Set peak prominence to x times noise levels
-    # prominence = ((noise * (min_amplitude-1)) / y.max()) * 100
-
-    # Boundary conditions
-    resolution = abs(np.diff(x).mean())
-    min_width = resolution * min_peak_width  # min_peak_width at FWHM
-    min_amplitude = noise * min_amplitude
-    prominence = min_amplitude + (noise / 2)
-    xlength = x.max() - x.min()
-    # Left and right limits for: center, amplitude, width, shape and baselevel
-    leftBoundSimple = [x.min(), min_amplitude, min_width, 0.0, -5]
-    rightBoundSimple = [x.max(), y.max() * 1.5, xlength, 1.0, y.max()]
-
-    # Initial guesses for peak parameters
-    amplitudes, centers, widths = cf._find_peak_parameters(
-        x, y, prominence, height=noise, width=min_peak_width
-    )
-    # Remove initial guesses that are too narrow or too low amplitude
-    keep = np.where((widths > min_width) & (amplitudes > min_amplitude))
-    amplitudes = amplitudes[keep]
-    centers = centers[keep]
-    widths = widths[keep]
-
-    peakAmount = len(amplitudes)
-    shapes = np.array([1.0] * peakAmount)
-    baselevels = np.array([0.0] * peakAmount)
-
-    initvalues = np.concatenate((centers, amplitudes, widths, shapes, baselevels))
-
-    # Number of fit parameters per curve: 5 for fitted baselevel, 4 for fixed baselevel
-    parameters = 5
-    # Remove bounds if baseline is fixed at 0
-    if baseline0:
-        leftBoundSimple = leftBoundSimple[:-1]
-        rightBoundSimple = rightBoundSimple[:-1]
-        initvalues = initvalues[:-peakAmount]
-        parameters = 4
-
-    def sumGaussLorentz_reshaped(
-        x, params, peakAmount, baseline_fixed=baseline0, baseline=0.0
-    ):
-        "Reshape parameters to use sum_GaussLorentz in least-squares regression"
-
-        if baseline_fixed:
-            baselevels = np.array([baseline] * peakAmount)
-            params = np.concatenate((params, baselevels))
-
-        values = params.reshape((5, peakAmount))
-
-        return c.sum_GaussLorentz(x, *values)
-
-    # Residual on ititial fit
-    residual_old = mean_squared_error(
-        y, sumGaussLorentz_reshaped(x, initvalues, peakAmount), squared=False
-    )  # (y - sumGaussLorentz_reshaped(x, initvalues, peakAmount)).std()
-    # Save the initial values in case the first iteration doesn't give an imporovement
-    fitParams_old = initvalues.reshape((parameters, peakAmount))
-    if baseline0:
-        fitParams_old = np.vstack((fitParams_old, np.array([0.0] * peakAmount)))
-
-    # Cost function to minimise
-    calculate_residuals = (
-        lambda params, x, y, peakAmount: sumGaussLorentz_reshaped(x, params, peakAmount)
-        - y
-    )
-
-    # Flags for stopping the while loop
-    for _ in range(int(max_iterations)):
-
-        # Set up bounds
-        leftBound = np.repeat(leftBoundSimple, peakAmount)
-        rightBound = np.repeat(rightBoundSimple, peakAmount)
-        bounds = (leftBound, rightBound)
-        # Optimise fit parameters
-        LSfit = opt.least_squares(
-            calculate_residuals,
-            x0=initvalues,
-            bounds=bounds,
-            args=(x, y, peakAmount),
-            loss="linear",
-        )
-        # Fitted parameters for sum_GaussLorentz
-        fitParams = LSfit.x.reshape((parameters, peakAmount))
-        if baseline0:
-            fitParams = np.vstack((fitParams, np.array([0.0] * peakAmount)))
-
-        # R squared adjusted for noise
-        R2_noise = (y, c.sum_GaussLorentz(x, *fitParams), noise)
-
-        # RSME on the fit
-        residual = mean_squared_error(
-            y, c.sum_GaussLorentz(x, *fitParams), squared=False
-        )
-        residual_vector = abs(y - c.sum_GaussLorentz(x, *fitParams))
-
-        residuals_increased = residual > residual_old
-        residuals_improvement = (residual_old - residual) * 100 / residual_old
-        # Stop if residuals have increased, or when the residual improvement is below the threshold value
-        if residuals_increased or (residuals_improvement < residuals_threshold):
-            # warnings.warn(f"Noise improved by <{(1 - residuals_threshold):.0%}, using previous result")
-            # Revert back to previous fitted values
-            fitParams = fitParams_old.copy()
-            residual = residual_old
-            break
-
-        # Add new peak
-        peakAmount += 1
-        # Get initial guess for new peak
-        # Y at the highest residual, or mimumum ampltude, whichever one is higher
-        amplitude = np.max(
-            (y[residual_vector == residual_vector.max()][0], min_amplitude)
-        )
-        center = x[residual_vector == residual_vector.max()][0]
-        width = np.max((widths.mean(), min_width))
-
-        amplitudes = np.append(amplitudes, amplitude)
-        centers = np.append(centers, center)
-        widths = np.append(widths, width)
-        shapes = np.append(shapes, 1)
-        baselevels = np.append(baselevels, 0)
-
-        initvalues = np.concatenate((centers, amplitudes, widths, shapes, baselevels))
-
-        if baseline0:
-            initvalues = initvalues[:-peakAmount]
-        # Save old noise and fitted parameters for comparison in next iteration.
-        fitParams_old = fitParams.copy()
-        residual_old = residual.copy()
-
-    return fitParams, residual
-
-
-def _R2_noise(y, y_predict, noise):
-    data_mean = y.mean()
-    residual_vector = y - y_predict
-    residual_sum = sum((residual_vector / noise) ** 2)
-    sum_squares = sum((y - data_mean) ** 2)
-    R2_noise = 1 - (residual_sum / sum_squares)
-    return R2_noise
+import warnings
+
+import numpy as np
+import scipy.optimize as opt
+from sklearn.metrics import mean_squared_error
+
+import ramCOH.signal_processing.curve_fitting as cf
+import ramCOH.signal_processing.curves as c
+import ramCOH.signal_processing.functions as f
+
+
+def deconvolve_signal(
+    x,
+    y,
+    min_peak_width=4,
+    min_amplitude=1,
+    residuals_threshold=10,
+    max_iterations=5,
+    baseline0=True,
+    noise=None,
+):
+    """
+    Parameters
+    ----------
+    x : array-like
+        x
+    y : array-like
+        y
+    noise_threshold : float
+        Fit is accepted when the standard deviation of the fit residuals fall below (noise on y) * noise_threshold
+    min_peak_width : int, float
+        minimum width of fitted peaks (full width at half maximum) in x stepsize.
+    min_amplitude : int, float
+        minium amplitude of fitted peaks as a factor of noise on y.
+    baseline0 : bool
+        fix baselevel of fitted curves to 0
+    noise : float, int
+        Absolute noise on y
+    max_iterations : int
+        maximum loop iterations. One new curve is added each loop
+
+    Returns
+    -------
+    fitParams : list[list]
+        fitted parameters for sum_GaussLorentz
+    R2_noise : float
+        R squared of fit result to y, adjusted for noise (on y)
+    fit_noise : float
+        standard deviation on the residuals of y and the fit result
+    """
+
+    # Calculate noise on the total signal
+    # if noise is None:
+    #     noise, _ = f._calculate_noise(x=x, y=y)
+
+    # Set peak prominence to x times noise levels
+    # prominence = ((noise * (min_amplitude-1)) / y.max()) * 100
+
+    # Boundary conditions
+    resolution = abs(np.diff(x).mean())
+    min_width = resolution * min_peak_width  # min_peak_width at FWHM
+    min_amplitude = noise * min_amplitude
+    prominence = min_amplitude + (noise / 2)
+    xlength = x.max() - x.min()
+    # Left and right limits for: center, amplitude, width, shape and baselevel
+    leftBoundSimple = [x.min(), min_amplitude, min_width, 0.0, -5]
+    rightBoundSimple = [x.max(), y.max() * 1.5, xlength, 1.0, y.max()]
+
+    # Initial guesses for peak parameters
+    amplitudes, centers, widths = cf._find_peak_parameters(
+        x, y, prominence, height=noise, width=min_peak_width
+    )
+    # Remove initial guesses that are too narrow or too low amplitude
+    keep = np.where((widths > min_width) & (amplitudes > min_amplitude))
+    amplitudes = amplitudes[keep]
+    centers = centers[keep]
+    widths = widths[keep]
+
+    peakAmount = len(amplitudes)
+    shapes = np.array([1.0] * peakAmount)
+    baselevels = np.array([0.0] * peakAmount)
+
+    initvalues = np.concatenate((centers, amplitudes, widths, shapes, baselevels))
+
+    # Number of fit parameters per curve: 5 for fitted baselevel, 4 for fixed baselevel
+    parameters = 5
+    # Remove bounds if baseline is fixed at 0
+    if baseline0:
+        leftBoundSimple = leftBoundSimple[:-1]
+        rightBoundSimple = rightBoundSimple[:-1]
+        initvalues = initvalues[:-peakAmount]
+        parameters = 4
+
+    def sumGaussLorentz_reshaped(
+        x, params, peakAmount, baseline_fixed=baseline0, baseline=0.0
+    ):
+        "Reshape parameters to use sum_GaussLorentz in least-squares regression"
+
+        if baseline_fixed:
+            baselevels = np.array([baseline] * peakAmount)
+            params = np.concatenate((params, baselevels))
+
+        values = params.reshape((5, peakAmount))
+
+        return c.sum_GaussLorentz(x, *values)
+
+    # Residual on ititial fit
+    residual_old = mean_squared_error(
+        y, sumGaussLorentz_reshaped(x, initvalues, peakAmount), squared=False
+    )  # (y - sumGaussLorentz_reshaped(x, initvalues, peakAmount)).std()
+    # Save the initial values in case the first iteration doesn't give an imporovement
+    fitParams_old = initvalues.reshape((parameters, peakAmount))
+    if baseline0:
+        fitParams_old = np.vstack((fitParams_old, np.array([0.0] * peakAmount)))
+
+    # Cost function to minimise
+    calculate_residuals = (
+        lambda params, x, y, peakAmount: sumGaussLorentz_reshaped(x, params, peakAmount)
+        - y
+    )
+
+    # Flags for stopping the while loop
+    for _ in range(int(max_iterations)):
+
+        # Set up bounds
+        leftBound = np.repeat(leftBoundSimple, peakAmount)
+        rightBound = np.repeat(rightBoundSimple, peakAmount)
+        bounds = (leftBound, rightBound)
+        # Optimise fit parameters
+        LSfit = opt.least_squares(
+            calculate_residuals,
+            x0=initvalues,
+            bounds=bounds,
+            args=(x, y, peakAmount),
+            loss="linear",
+        )
+        # Fitted parameters for sum_GaussLorentz
+        fitParams = LSfit.x.reshape((parameters, peakAmount))
+        if baseline0:
+            fitParams = np.vstack((fitParams, np.array([0.0] * peakAmount)))
+
+        # R squared adjusted for noise
+        R2_noise = (y, c.sum_GaussLorentz(x, *fitParams), noise)
+
+        # RSME on the fit
+        residual = mean_squared_error(
+            y, c.sum_GaussLorentz(x, *fitParams), squared=False
+        )
+        residual_vector = abs(y - c.sum_GaussLorentz(x, *fitParams))
+
+        residuals_increased = residual > residual_old
+        residuals_improvement = (residual_old - residual) * 100 / residual_old
+        # Stop if residuals have increased, or when the residual improvement is below the threshold value
+        if residuals_increased or (residuals_improvement < residuals_threshold):
+            # warnings.warn(f"Noise improved by <{(1 - residuals_threshold):.0%}, using previous result")
+            # Revert back to previous fitted values
+            fitParams = fitParams_old.copy()
+            residual = residual_old
+            break
+
+        # Add new peak
+        peakAmount += 1
+        # Get initial guess for new peak
+        # Y at the highest residual, or mimumum ampltude, whichever one is higher
+        amplitude = np.max(
+            (y[residual_vector == residual_vector.max()][0], min_amplitude)
+        )
+        center = x[residual_vector == residual_vector.max()][0]
+        width = np.max((widths.mean(), min_width))
+
+        amplitudes = np.append(amplitudes, amplitude)
+        centers = np.append(centers, center)
+        widths = np.append(widths, width)
+        shapes = np.append(shapes, 1)
+        baselevels = np.append(baselevels, 0)
+
+        initvalues = np.concatenate((centers, amplitudes, widths, shapes, baselevels))
+
+        if baseline0:
+            initvalues = initvalues[:-peakAmount]
+        # Save old noise and fitted parameters for comparison in next iteration.
+        fitParams_old = fitParams.copy()
+        residual_old = residual.copy()
+
+    return fitParams, residual
+
+
+def _R2_noise(y, y_predict, noise):
+    data_mean = y.mean()
+    residual_vector = y - y_predict
+    residual_sum = sum((residual_vector / noise) ** 2)
+    sum_squares = sum((y - data_mean) ** 2)
+    R2_noise = 1 - (residual_sum / sum_squares)
+    return R2_noise
```

### Comparing `ramCOH-1.1.0/ramCOH/signal_processing/functions.py` & `ramCOH-1.1.1/ramCOH/signal_processing/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,297 +1,313 @@
-from importlib import resources
-from typing import Tuple, Union
-
-import csaps as cs
-import numpy as np
-import numpy.typing as npt
-import pandas as pd
-
-import ramCOH.signal_processing.curves as c
-
-
-def wavelengthToShift(wavelength, laser=532.18):
-
-    return 1e7 / laser - 1e7 / wavelength
-
-
-def ShiftToWavelength(shift, laser=532.18):
-
-    return 1 / (1 / laser - shift / 1e7)
-
-
-def neonEmission(laser=532.18):
-    "from https://physics.nist.gov/PhysRefData/Handbook/Tables/neontable2.htm"
-
-    with resources.open_text("ramCOH.static", "neon_emissionLines.csv") as df:
-        neon = pd.read_csv(df)
-
-    # neon= pd.read_csv('D:/Dropbox/python/packages/petroPy/neon_emissionLines.csv')
-
-    ramanShift = "RamanShift" + str(int(laser))
-    neon[ramanShift] = wavelengthToShift(neon["wavelength_nm"], laser=laser)
-
-    return neon
-
-
-def trim_sort(x, y, cutoff=0):
-    """
-    Sort and trim x, y data
-
-    Parameters
-    ----------
-    x : array-like
-        x
-    y : array-like
-        y
-
-    Returns
-    -------
-    x, y : x and y sorted by x and trimmed to x > cutoff
-    """
-    x = np.array(x)
-    y = np.array(y)
-    sort = np.argsort(x)
-    y_sort = y[sort]
-    x_sort = x[sort]
-
-    return x_sort[x > cutoff], y_sort[x > cutoff]
-
-
-def shift_spectrum(spectrum: npt.NDArray, shift: int) -> npt.NDArray:
-    if shift == 0:
-        return spectrum
-
-    if shift > 0:
-        spectrum = np.concatenate([spectrum[shift:], [0] * shift])
-    if shift < 0:
-        spectrum = np.concatenate([[0] * abs(shift), spectrum[:shift]])
-
-    return spectrum
-
-
-def smooth(y, type="gaussian", kernel_width=9):
-    """
-    Parameters
-    ----------
-    y : array-like
-        y
-    smoothtype : str
-        'moving_average' or 'gaussian'
-    kernelWidth : int
-        width of smoothing kernel in elements of y
-
-    Returns
-    -------
-    smoothed : array
-        y smoothed by a kernel
-    """
-    kernel_width = int(kernel_width)
-
-    if type not in ("gaussian", "moving_average"):
-        raise ValueError("select smoothtype 'moving_average' or 'gaussian'")
-
-    if type == "moving_average":
-        kernel = np.ones((kernel_width,)) / kernel_width
-    elif type == "gaussian":
-        kernel = np.fromiter(
-            (
-                c.Gaussian(x, 1, 0, kernel_width / 3, 0)
-                for x in range(-(kernel_width - 1) // 2, (kernel_width + 1) // 2, 1)
-            ),
-            np.float,
-        )
-        kernel = kernel / sum(kernel)
-
-    return np.convolve(y, kernel, mode="valid")
-
-
-def long_correction(x, intensities, T_C=25.0, laser=532.18, normalisation=True):
-
-    """
-    Long correction of Raman spectra
-    From Long (1977) and Behrens (2006)
-
-    Parameters
-    ----------
-    x   :   array
-        x-axis in Raman shifts
-    intensities :   array
-        signal intensities
-    T_C :   float
-        temperature of aquisition in degrees celsius
-    laser  :   float
-        laser wavelength in nanometers
-    normalisation   :   bool
-        normalise specturm to the total area
-    """
-    from scipy.constants import c, h, k
-
-    intensities = np.array(intensities)[np.argsort(x)]
-    x = np.array(x)[np.argsort(x)]
-
-    # nu0 laser is in M-1 (wave is in nm)
-    nu0 = 1.0 / laser * 1e9
-    # K temperature
-    T = T_C + 273.15
-
-    # Raman shift from cm-1 to m-1
-    nu = 100.0 * x
-
-    # frequency correction; dimensionless
-    frequency = nu0**3 * nu / ((nu0 - nu) ** 4)
-    # temperature correction with Boltzman distribution; dimensionless
-    boltzman = 1.0 - np.exp(-h * c * nu / (k * T))
-    intensityLong = intensities * frequency * boltzman  # correction
-
-    if normalisation:
-        # normalisation over total area
-        intensityLong = intensityLong / np.trapz(intensityLong, x)
-
-    return intensityLong
-
-
-def H2Oraman(rWS, *, intercept, slope):
-    """Calculate water contents using equation (3) from Le Losq et al. (2012)
-
-    equation:
-    H2O/(100-H2O) = intercept + slope * rWS
-
-    rWS= (Area water peaks / Area silica peaks) of sample raman spectra
-
-    intercept & slope are determined empirically through calibration with standards
-    """
-
-    return (100 * (intercept + slope * rWS)) / (1 + intercept + slope * rWS)
-
-
-def _extractBIR_bool(x, birs):
-    """Extract baseline interpolation regions (birs) from a spectrum
-
-    Parameters
-    ----------
-    x, y : numpy.array
-        1-dimensional array with Raman shift (x) and intensity (y)
-    birs : numpy.array
-        (n,2) shaped array for n baseline interpolation regions (birs). Each row is [lower limit, upper limmit]
-
-    Returns
-    -------
-    birs_x : array
-        values for x within baseline interpolation regions
-    birs_y : array
-        alues for y within baseline interpolation regions
-    """
-
-    selection = (x > birs[0][0]) & (x < birs[0][1])
-
-    for bir in birs[1:]:
-        selection = selection | ((x > bir[0]) & (x < bir[1]))
-
-    return selection
-
-
-def _extractBIR(x, y, birs):
-
-    selection = _extractBIR_bool(x, birs)
-
-    return x[selection], y[selection]
-
-
-def _interpolate_section(x, y, interpolate, smooth_factor):
-
-    smooth = smooth_factor * 1e-5
-
-    interpolate_index = _extractBIR_bool(x, interpolate)
-    spectrum_index = ~interpolate_index
-
-    spline = cs.csaps(x[spectrum_index], y[spectrum_index], smooth=smooth)
-
-    interpolated_x = x[interpolate_index]
-    interpolated_y = spline(interpolated_x)
-
-    return interpolated_x, interpolated_y, spline
-
-
-def _calculate_noise(x, y, smooth_factor=1):
-    """
-    Parameters
-    ----------
-    x : array-like
-        x
-    y : array-like
-        y
-    smooth_factor : int, float
-        scaling factor applied to 'smooth' parameter of csaps
-
-    Returns
-    -------
-    noise : float
-        Noise on y calculated as the standard deviation on the residuals of y and a fitted smoothed spline
-    spline :
-        smoothed spline fitted to y
-    """
-    # Max range in y
-    max_difference = y.max() - y.min()
-    # Emperically found this is gives ok smoothing factors for most spectra
-    smooth = 2e-6 * max_difference * smooth_factor
-    # Fit spline
-    spline = cs.csaps(x, y, smooth=smooth)
-    # Standard deviation on the residuals of y and spline
-    noise_data = y - spline(x)
-    noise = noise_data.std(axis=None) * 2
-
-    return noise, spline
-
-
-def _root_interference(
-    scaling: Tuple[float, int],
-    x,
-    interference: npt.NDArray,
-    spectrum: npt.NDArray,
-    interpolated_interval: npt.NDArray,
-    interval: Tuple[float, float],
-):
-
-    scale, shift = scaling
-    x_min, x_max = interval
-    # Trim glass spectra to length
-    filter_array = (x > x_min) & (x < x_max)
-    spectrum = spectrum[filter_array]
-    # Trim, shift and scale olivine spectrum
-    shifted_array = _shift_window(filter_array=filter_array, shift=shift)
-    interference_scaled = (
-        interference[shifted_array]
-        * scale  # (x > (x_min + shift)) & (x < (x_max + shift))
-    )
-    # Subtract olivine
-    spectrum_corrected = spectrum - interference_scaled
-
-    return [sum(abs(interpolated_interval - spectrum_corrected)), 0]
-
-
-def _shift_window(filter_array: npt.NDArray[np.bool_], shift: Union[float, int]):
-    shift = int(shift)
-    if shift < 0:
-        shifted_array = np.concatenate(
-            [np.repeat(np.array([False]), abs(shift)), filter_array[:-shift]]
-        )
-    elif shift > 0:
-        shifted_array = np.concatenate(
-            [filter_array[shift:], np.repeat(np.array([False]), shift)]
-        )
-    else:
-        return filter_array
-
-    return shifted_array
-
-
-def add_interpolation(
-    spectrum: npt.NDArray,
-    interpolation_indeces: npt.NDArray,
-    interpolated_y: npt.NDArray,
-):
-
-    interpolated_spectrum = spectrum.copy()
-    interpolated_spectrum[interpolation_indeces] = interpolated_y.copy()
-
-    return interpolated_spectrum
+from importlib import resources
+from typing import Tuple, Union
+
+import csaps as cs
+import numpy as np
+import numpy.typing as npt
+import pandas as pd
+from sklearn.metrics import mean_squared_error
+
+import ramCOH.signal_processing.curves as c
+
+
+def wavelengthToShift(wavelength, laser=532.18):
+
+    return 1e7 / laser - 1e7 / wavelength
+
+
+def ShiftToWavelength(shift, laser=532.18):
+
+    return 1 / (1 / laser - shift / 1e7)
+
+
+def neonEmission(laser=532.18):
+    "from https://physics.nist.gov/PhysRefData/Handbook/Tables/neontable2.htm"
+
+    with resources.open_text("ramCOH.static", "neon_emissionLines.csv") as df:
+        neon = pd.read_csv(df)
+
+    # neon= pd.read_csv('D:/Dropbox/python/packages/petroPy/neon_emissionLines.csv')
+
+    ramanShift = "RamanShift" + str(int(laser))
+    neon[ramanShift] = wavelengthToShift(neon["wavelength_nm"], laser=laser)
+
+    return neon
+
+
+def trim_sort(x: npt.NDArray, y: npt.NDArray, cutoff=0):
+    """
+    Sort and trim x, y data
+
+    Parameters
+    ----------
+    x : array-like
+        x
+    y : array-like
+        y
+
+    Returns
+    -------
+    x, y : x and y sorted by x and trimmed to x > cutoff
+    """
+    # x = np.array(x)
+    x = remove_duplicate_x(x)
+    y = np.array(y)
+    sort = np.argsort(x)
+    y_sort = y[sort]
+    x_sort = x[sort]
+
+    return x_sort[x > cutoff], y_sort[x > cutoff]
+
+
+def remove_duplicate_x(x: npt.NDArray):
+    """
+    Shift x-axis values by +1% if they are duplicates.
+    """
+
+    duplicates = np.concatenate([[False], np.diff(x) == 0])
+
+    if not np.any(duplicates):
+        return x
+
+    return np.where(duplicates, x * 1.01, x)
+
+
+def shift_spectrum(spectrum: npt.NDArray, shift: int) -> npt.NDArray:
+    if shift == 0:
+        return spectrum
+
+    if shift > 0:
+        spectrum = np.concatenate([spectrum[shift:], [0] * shift])
+    if shift < 0:
+        spectrum = np.concatenate([[0] * abs(shift), spectrum[:shift]])
+
+    return spectrum
+
+
+def smooth(y, type="gaussian", kernel_width=9):
+    """
+    Parameters
+    ----------
+    y : array-like
+        y
+    smoothtype : str
+        'moving_average' or 'gaussian'
+    kernelWidth : int
+        width of smoothing kernel in elements of y
+
+    Returns
+    -------
+    smoothed : array
+        y smoothed by a kernel
+    """
+    kernel_width = int(kernel_width)
+
+    if type not in ("gaussian", "moving_average"):
+        raise ValueError("select smoothtype 'moving_average' or 'gaussian'")
+
+    if type == "moving_average":
+        kernel = np.ones((kernel_width,)) / kernel_width
+    elif type == "gaussian":
+        kernel = np.fromiter(
+            (
+                c.Gaussian(x, 1, 0, kernel_width / 3, 0)
+                for x in range(-(kernel_width - 1) // 2, (kernel_width + 1) // 2, 1)
+            ),
+            np.float,
+        )
+        kernel = kernel / sum(kernel)
+
+    return np.convolve(y, kernel, mode="valid")
+
+
+def long_correction(x, intensities, T_C=25.0, laser=532.18, normalisation=True):
+
+    """
+    Long correction of Raman spectra
+    From Long (1977) and Behrens (2006)
+
+    Parameters
+    ----------
+    x   :   array
+        x-axis in Raman shifts
+    intensities :   array
+        signal intensities
+    T_C :   float
+        temperature of aquisition in degrees celsius
+    laser  :   float
+        laser wavelength in nanometers
+    normalisation   :   bool
+        normalise specturm to the total area
+    """
+    from scipy.constants import c, h, k
+
+    intensities = np.array(intensities)[np.argsort(x)]
+    x = np.array(x)[np.argsort(x)]
+
+    # nu0 laser is in M-1 (wave is in nm)
+    nu0 = 1.0 / laser * 1e9
+    # K temperature
+    T = T_C + 273.15
+
+    # Raman shift from cm-1 to m-1
+    nu = 100.0 * x
+
+    # frequency correction; dimensionless
+    frequency = nu0**3 * nu / ((nu0 - nu) ** 4)
+    # temperature correction with Boltzman distribution; dimensionless
+    boltzman = 1.0 - np.exp(-h * c * nu / (k * T))
+    intensityLong = intensities * frequency * boltzman  # correction
+
+    if normalisation:
+        # normalisation over total area
+        intensityLong = intensityLong / np.trapz(intensityLong, x)
+
+    return intensityLong
+
+
+def H2Oraman(rWS, *, intercept, slope):
+    """Calculate water contents using equation (3) from Le Losq et al. (2012)
+
+    equation:
+    H2O/(100-H2O) = intercept + slope * rWS
+
+    rWS= (Area water peaks / Area silica peaks) of sample raman spectra
+
+    intercept & slope are determined empirically through calibration with standards
+    """
+
+    return (100 * (intercept + slope * rWS)) / (1 + intercept + slope * rWS)
+
+
+def _extractBIR_bool(x, birs):
+    """Extract baseline interpolation regions (birs) from a spectrum
+
+    Parameters
+    ----------
+    x, y : numpy.array
+        1-dimensional array with Raman shift (x) and intensity (y)
+    birs : numpy.array
+        (n,2) shaped array for n baseline interpolation regions (birs). Each row is [lower limit, upper limmit]
+
+    Returns
+    -------
+    birs_x : array
+        values for x within baseline interpolation regions
+    birs_y : array
+        alues for y within baseline interpolation regions
+    """
+
+    selection = (x > birs[0][0]) & (x < birs[0][1])
+
+    for bir in birs[1:]:
+        selection = selection | ((x > bir[0]) & (x < bir[1]))
+
+    return selection
+
+
+def _extractBIR(x, y, birs):
+
+    selection = _extractBIR_bool(x, birs)
+
+    return x[selection], y[selection]
+
+
+def _interpolate_section(x, y, interpolate, smooth_factor):
+
+    smooth = smooth_factor * 1e-5
+
+    interpolate_index = _extractBIR_bool(x, interpolate)
+    spectrum_index = ~interpolate_index
+
+    spline = cs.csaps(x[spectrum_index], y[spectrum_index], smooth=smooth)
+
+    interpolated_x = x[interpolate_index]
+    interpolated_y = spline(interpolated_x)
+
+    return interpolated_x, interpolated_y, spline
+
+
+def _calculate_noise(x, y, smooth_factor=1):
+    """
+    Parameters
+    ----------
+    x : array-like
+        x
+    y : array-like
+        y
+    smooth_factor : int, float
+        scaling factor applied to 'smooth' parameter of csaps
+
+    Returns
+    -------
+    noise : float
+        Noise on y calculated as the standard deviation on the residuals of y and a fitted smoothed spline
+    spline :
+        smoothed spline fitted to y
+    """
+    # Max range in y
+    max_difference = y.max() - y.min()
+    # Emperically found this is gives ok smoothing factors for most spectra
+    smooth = 2e-6 * max_difference * smooth_factor
+    # Fit spline
+    spline = cs.csaps(x, y, smooth=smooth)
+    # Standard deviation on the residuals of y and spline
+    noise_data = y - spline(x)
+    noise = noise_data.std(axis=None) * 2
+
+    return noise, spline
+
+
+def _root_interference(
+    scaling: Tuple[float, int],
+    x,
+    interference: npt.NDArray,
+    spectrum: npt.NDArray,
+    interpolated_interval: npt.NDArray,
+    interval: Tuple[float, float],
+):
+
+    scale, shift = scaling
+    x_min, x_max = interval
+    # Trim glass spectra to length
+    filter_array = (x > x_min) & (x < x_max)
+    spectrum = spectrum[filter_array]
+    # Trim, shift and scale olivine spectrum
+    shifted_array = _shift_window(filter_array=filter_array, shift=shift)
+    interference_scaled = (
+        interference[shifted_array]
+        * scale  # (x > (x_min + shift)) & (x < (x_max + shift))
+    )
+    # Subtract olivine
+    spectrum_corrected = spectrum - interference_scaled
+    rmse = mean_squared_error(interpolated_interval, spectrum_corrected, squared=False)
+
+    return [rmse, 0]  # sum(abs(interpolated_interval - spectrum_corrected))
+
+
+def _shift_window(filter_array: npt.NDArray[np.bool_], shift: Union[float, int]):
+    shift = int(shift)
+    if shift < 0:
+        shifted_array = np.concatenate(
+            [np.repeat(np.array([False]), abs(shift)), filter_array[:-shift]]
+        )
+    elif shift > 0:
+        shifted_array = np.concatenate(
+            [filter_array[shift:], np.repeat(np.array([False]), shift)]
+        )
+    else:
+        return filter_array
+
+    return shifted_array
+
+
+def add_interpolation(
+    spectrum: npt.NDArray,
+    interpolation_indeces: npt.NDArray,
+    interpolated_y: npt.NDArray,
+):
+
+    interpolated_spectrum = spectrum.copy()
+    interpolated_spectrum[interpolation_indeces] = interpolated_y.copy()
+
+    return interpolated_spectrum
```

### Comparing `ramCOH-1.1.0/ramCOH.egg-info/PKG-INFO` & `ramCOH-1.1.1/ramCOH.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-Metadata-Version: 2.1
-Name: ramCOH
-Version: 1.1.0
-Summary: Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses
-Author: Thomas van Gerve
-License: MIT License
-        
-        Copyright (c) 2022 TDGerve
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/TDGerve/ramCOH
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ramCOH
-
-Library for processing and peak fitting of Raman spectra, targeted at CO<sub>2</sub> fluids and (hydrous) silicate glasses
-
-## Documentation
-Code documentation is available at [ramcoh.readthedocs.io](https://ramcoh.readthedocs.io/en/latest)
-
-## Installation
-
-
+Metadata-Version: 2.1
+Name: ramCOH
+Version: 1.1.1
+Summary: Library for processing and peak fitting of Raman spectra, targeted at CO2 fluids and hydrous silicate glasses
+Author: Thomas van Gerve
+License: MIT License
+        
+        Copyright (c) 2022 TDGerve
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/TDGerve/ramCOH
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Documentation Status](https://readthedocs.org/projects/ramcoh/badge/?version=latest)](https://ramcoh.readthedocs.io/en/latest/?badge=latest)
+# ramCOH
+
+Library for processing and peak fitting of Raman spectra, targeted at CO<sub>2</sub> fluids and (hydrous) silicate glasses
+
+## Documentation
+Code documentation is available at [ramcoh.readthedocs.io](https://ramcoh.readthedocs.io/en/latest)
+
+## Installation
+ramCOH can be installed with pip by running
+
+    pip install ramCOH
+
+in a terminal.
+
+If you would like to install from a specific git branch or release instead run
+
+    pip install git+https://github.com/TDGerve/ramCOH.git@tag
+
+where *tag* should be repleaced by the release tag or branch name (e.g. *v1.0* or *development*)
+
+
```

### Comparing `ramCOH-1.1.0/ramCOH.egg-info/SOURCES.txt` & `ramCOH-1.1.1/ramCOH.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+.gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 ramCOH/__init__.py
 ramCOH.egg-info/PKG-INFO
 ramCOH.egg-info/SOURCES.txt
 ramCOH.egg-info/dependency_links.txt
 ramCOH.egg-info/requires.txt
 ramCOH.egg-info/top_level.txt
+ramCOH/raman/CO2.py
 ramCOH/raman/__init__.py
 ramCOH/raman/baseclass.py
 ramCOH/raman/baseline_regions.py
 ramCOH/raman/co2.py
 ramCOH/raman/glass.py
 ramCOH/raman/neon.py
 ramCOH/signal_processing/__init__.py
```

