# Comparing `tmp/mzapy-1.5.3.tar.gz` & `tmp/mzapy-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzapy-1.5.3.tar", last modified: Wed Mar 29 17:21:22 2023, max compression
+gzip compressed data, was "mzapy-1.6.3.tar", last modified: Tue Apr 11 18:23:23 2023, max compression
```

## Comparing `mzapy-1.5.3.tar` & `mzapy-1.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ross200  (1223808424) 2016721313        0 2023-03-29 17:21:22.259549 mzapy-1.5.3/
--rw-r--r--   0 ross200  (1223808424) 2016721313      853 2023-03-29 17:21:22.259814 mzapy-1.5.3/PKG-INFO
--rw-r--r--   0 ross200  (1223808424) 2016721313      334 2023-03-29 17:21:07.000000 mzapy-1.5.3/README.md
-drwxr-xr-x   0 ross200  (1223808424) 2016721313        0 2023-03-29 17:21:22.246146 mzapy-1.5.3/mzapy/
--rw-r--r--   0 ross200  (1223808424) 2016721313    43144 2023-03-29 17:21:07.000000 mzapy-1.5.3/mzapy/__init__.py
--rw-r--r--   0 ross200  (1223808424) 2016721313      745 2022-10-14 20:37:15.000000 mzapy-1.5.3/mzapy/_config.py
--rwx------   0 ross200  (1223808424) 2016721313     3113 2022-05-16 18:25:41.000000 mzapy-1.5.3/mzapy/_util.py
--rw-r--r--   0 ross200  (1223808424) 2016721313    11075 2022-09-23 18:33:12.000000 mzapy-1.5.3/mzapy/calibration.py
--rw-r--r--   0 ross200  (1223808424) 2016721313    16968 2022-09-23 18:33:12.000000 mzapy-1.5.3/mzapy/isotopes.py
--rw-r--r--   0 ross200  (1223808424) 2016721313    11743 2023-03-29 17:21:07.000000 mzapy-1.5.3/mzapy/peaks.py
--rwxr-xr-x   0 ross200  (1223808424) 2016721313    18992 2022-10-10 17:48:32.000000 mzapy-1.5.3/mzapy/view.py
-drwxr-xr-x   0 ross200  (1223808424) 2016721313        0 2023-03-29 17:21:22.258430 mzapy-1.5.3/mzapy.egg-info/
--rwx------   0 ross200  (1223808424) 2016721313      853 2023-03-29 17:21:22.000000 mzapy-1.5.3/mzapy.egg-info/PKG-INFO
--rwx------   0 ross200  (1223808424) 2016721313      296 2023-03-29 17:21:22.000000 mzapy-1.5.3/mzapy.egg-info/SOURCES.txt
--rwx------   0 ross200  (1223808424) 2016721313        1 2023-03-29 17:21:22.000000 mzapy-1.5.3/mzapy.egg-info/dependency_links.txt
--rwx------   0 ross200  (1223808424) 2016721313       46 2023-03-29 17:21:22.000000 mzapy-1.5.3/mzapy.egg-info/requires.txt
--rwx------   0 ross200  (1223808424) 2016721313        6 2023-03-29 17:21:22.000000 mzapy-1.5.3/mzapy.egg-info/top_level.txt
--rwx------   0 ross200  (1223808424) 2016721313       80 2022-05-31 15:48:15.000000 mzapy-1.5.3/pyproject.toml
--rw-r--r--   0 ross200  (1223808424) 2016721313      697 2023-03-29 17:21:22.261316 mzapy-1.5.3/setup.cfg
+drwxr-xr-x   0 ross200  (1223808424) 2016721313        0 2023-04-11 18:23:23.657177 mzapy-1.6.3/
+-rw-r--r--   0 ross200  (1223808424) 2016721313      853 2023-04-11 18:23:23.657483 mzapy-1.6.3/PKG-INFO
+-rw-r--r--   0 ross200  (1223808424) 2016721313      334 2023-03-29 17:21:07.000000 mzapy-1.6.3/README.md
+drwxr-xr-x   0 ross200  (1223808424) 2016721313        0 2023-04-11 18:23:23.641873 mzapy-1.6.3/mzapy/
+-rw-r--r--   0 ross200  (1223808424) 2016721313    43144 2023-04-11 18:23:07.000000 mzapy-1.6.3/mzapy/__init__.py
+-rw-r--r--   0 ross200  (1223808424) 2016721313      745 2022-10-14 20:37:15.000000 mzapy-1.6.3/mzapy/_config.py
+-rw-r--r--   0 ross200  (1223808424) 2016721313     3508 2023-04-11 18:23:07.000000 mzapy-1.6.3/mzapy/_util.py
+-rw-r--r--   0 ross200  (1223808424) 2016721313    17045 2023-04-11 18:23:07.000000 mzapy-1.6.3/mzapy/calibration.py
+-rw-r--r--   0 ross200  (1223808424) 2016721313    16968 2022-09-23 18:33:12.000000 mzapy-1.6.3/mzapy/isotopes.py
+-rw-r--r--   0 ross200  (1223808424) 2016721313    11743 2023-03-29 17:21:07.000000 mzapy-1.6.3/mzapy/peaks.py
+-rwxr-xr-x   0 ross200  (1223808424) 2016721313    23029 2023-04-11 18:23:07.000000 mzapy-1.6.3/mzapy/view.py
+drwxr-xr-x   0 ross200  (1223808424) 2016721313        0 2023-04-11 18:23:23.655377 mzapy-1.6.3/mzapy.egg-info/
+-rwx------   0 ross200  (1223808424) 2016721313      853 2023-04-11 18:23:23.000000 mzapy-1.6.3/mzapy.egg-info/PKG-INFO
+-rwx------   0 ross200  (1223808424) 2016721313      296 2023-04-11 18:23:23.000000 mzapy-1.6.3/mzapy.egg-info/SOURCES.txt
+-rwx------   0 ross200  (1223808424) 2016721313        1 2023-04-11 18:23:23.000000 mzapy-1.6.3/mzapy.egg-info/dependency_links.txt
+-rwx------   0 ross200  (1223808424) 2016721313       46 2023-04-11 18:23:23.000000 mzapy-1.6.3/mzapy.egg-info/requires.txt
+-rwx------   0 ross200  (1223808424) 2016721313        6 2023-04-11 18:23:23.000000 mzapy-1.6.3/mzapy.egg-info/top_level.txt
+-rwx------   0 ross200  (1223808424) 2016721313       80 2022-05-31 15:48:15.000000 mzapy-1.6.3/pyproject.toml
+-rw-r--r--   0 ross200  (1223808424) 2016721313      697 2023-04-11 18:23:23.659538 mzapy-1.6.3/setup.cfg
```

### Comparing `mzapy-1.5.3/PKG-INFO` & `mzapy-1.6.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzapy
-Version: 1.5.3
+Version: 1.6.3
 Summary: A Python package that provides an interface to unprocessed MS data in the MZA format.
 Home-page: https://github.com/PNNL-m-q/mzapy
 Author: Dylan Ross
 Author-email: dylan.ross@pnnl.gov
 Project-URL: Bug Tracker, https://github.com/PNNL-m-q/mzapy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `mzapy-1.5.3/mzapy/__init__.py` & `mzapy-1.6.3/mzapy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     The MZA class is defined here. MZA is the main high-level interface for extracting MS data from MZA files
 """
 
 
 # mza_version.major_version.minor_version
 # mza_version is kept in lockstep with release of MZA format
-__version__ = '1.5.3'
+__version__ = '1.6.3'
 
 
 import queue
 import threading
 import time
 import os
 import pickle
```

### Comparing `mzapy-1.5.3/mzapy/_config.py` & `mzapy-1.6.3/mzapy/_config.py`

 * *Files identical despite different names*

### Comparing `mzapy-1.5.3/mzapy/_util.py` & `mzapy-1.6.3/mzapy/_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,14 +24,33 @@
         other value
 
     Returns
     -------
     ppm : float
         ppm error of other relative to reference
     """
+    return 1e6 * (other - reference) / reference
+
+
+def _abs_ppm_error(reference, other):
+    """
+    compute the absolute error in ppm for a value relative to some reference value
+    
+    Paramters
+    ---------
+    reference : float
+        reference value
+    other : float
+        other value
+
+    Returns
+    -------
+    ppm : float
+        ppm error of other relative to reference
+    """
     return 1e6 * np.abs(other - reference) / reference
 
 
 class _UpdatingProgressBar():
     """ a simple class for reporting progress """
 
     def __init__(self, levels=20, track_time_elapsed=False):
```

### Comparing `mzapy-1.5.3/mzapy/calibration.py` & `mzapy-1.6.3/mzapy/calibration.py`

 * *Files 20% similar despite different names*

```diff
@@ -127,17 +127,184 @@
         if self.opt_params is None:
             msg = ('_CalibrationBase: transform: self.opt_params has not been set, self.fit must be successfully'
                    ' run prior to using this method')
             raise RuntimeError(msg)
         return self.fit_function(X, *self.opt_params)
 
 
-class TWCCSCalibration(_CalibrationBase):
+class MassCalibration(_CalibrationBase):
     """
-    TWIM CCS calibration
+    mass calibration
+
+    Attributes
+    ----------
+    mz_ref : ``numpy.ndarray(float)``
+    mz_obs : ``numpy.ndarray(float)``
+        arrays of reference and observed m/z values
+    fit_func : ``str``
+        function to use for fitting
+    """
+    # map valid fit functions to the actual functions and initial parameters
+    _valid_fit_funcs = {
+        'linear': (lambda X, a, b: a * X + b, (1., 0.)), 
+    }
+
+    def __init__(self, mz_ref, mz_obs, fit_func,
+                 fit=True):
+        """
+        Initialize a new instance of MassCalibration
+
+        Performs fitting at initialization.
+
+        Parameters
+        ----------
+        mz_ref : ``numpy.ndarray(float)``
+        mz_obs : ``numpy.ndarray(float)``
+            arrays of reference and observed m/z values
+        fit_func : ``str``
+            function to use for fitting, valid options are: 'linear'
+        fit : ``bool``, default=True
+            perform fitting at initialization
+        """
+        # validate and store parameters
+        self.mz_ref, self.mz_obs, self.fit_func  =  mz_ref, mz_obs, fit_func
+        if self.fit_func not in self._valid_fit_funcs:
+            msg = 'MassCalibration: __init__: fit_func "{}" invalid, must be one of: {}'
+            valid_func_names = [_ for _ in self._valid_fit_funcs.keys()]
+            raise ValueError(msg.format(self.fit_func, valid_func_names))
+        # set fit_function and init_params based on fit_func
+        self.fit_function, self.init_params = self._valid_fit_funcs[self.fit_func]
+        if fit:
+            # setup values for fitting, make corrections if applicable
+            self._X = self.mz_obs
+            self._y = self.mz_ref
+            # fit calibration curve
+            self._y_fit = self.fit(self._X, self._y)
+
+    def calibrated_mass(self, mz):
+        """
+        returns calibrated masses for a set of uncalibrated masses
+
+        Parameters
+        ----------
+        mz : ``numpy.ndarray(float)`` or ``float``
+            uncalibrated m/z value(s)
+
+        Returns
+        -------
+        mz_cal : ``numpy.ndarray(float)`` or ``float``
+            calibrated m/z value(s)
+        """
+        return self.transform(mz)
+
+
+class CCSCalibrationDTsf(_CalibrationBase):
+    """
+    single-field DT CCS calibration
+
+    Attributes
+    ----------
+    mz : ``numpy.ndarray(float)``
+        calibrant m/z values
+    arrival_time : ``numpy.ndarray(float)``
+        calibrant arrival times
+    ref_ccs : ``numpy.ndarray(float)``
+        calibrant reference CCS values
+    z : ``float``
+        charge state (converted to float)
+    buffer_gas : ``str``
+        buffer gas for IM separation
+    """
+
+    # map valid buffer gasses to their mass
+    _valid_buffer_gasses = {
+        'N2': monoiso_mass({'N': 2}), 
+        'He': monoiso_mass({'He': 1}),
+    }
+
+    def __init__(self, mz, arrival_time, ref_ccs, z,
+                 buffer_gas='N2', fit=True):
+        """
+        Initialize a new instance of CCSCalibrationDTsf 
+
+        Performs fitting at initialization.
+
+        Parameters
+        ----------
+        mz : ``numpy.ndarray(float)``
+            calibrant m/z values
+        arrival_time : ``numpy.ndarray(float)``
+            calibrant arrival times
+        ref_ccs : ``numpy.ndarray(float)``
+            calibrant reference CCS values
+        z : ``int``
+            charge state
+        buffer_gas : ``str``, default='N2'
+            specify buffer gas for IM separation
+        fit : ``bool``, default=True
+            perform fitting at initialization
+        """
+        # validate and store parameters
+        self.mz, self.arrival_time, self.ref_ccs, self.z =  mz, arrival_time, ref_ccs, float(z)
+        # set init_params
+        self.init_params = (0., 1.)  # t_fix = 0 to start, beta = 1 to start
+        self.buffer_gas = buffer_gas
+        if self.buffer_gas not in self._valid_buffer_gasses:
+            msg = 'CCSCalibrationDTsf: __init__: buffer_gas "{}" invalid, must be one of: {}'
+            raise ValueError(msg.format(self.buffer_gas, self._valid_buffer_gasses))
+        self.buffer_gas_mass = self._valid_buffer_gasses[self.buffer_gas]
+        if fit:
+            # setup values for fitting
+            self._X = np.array([self.arrival_time, self.mz])
+            self._y = self.ref_ccs
+            # fit calibration curve
+            self._y_fit = self.fit(self._X, self._y)
+
+    def fit_function(self, X, t_fix, beta):
+        """
+        X should have shape (2, ?) and contain vectors for arrival time and m/z
+        function: CCS = z (arrival_time + t_fix) / (beta * m(mz)) 
+        where t_fix and beta are the fit parameters
+        and m(mz) is the mass term [sqrt(m_i / (m_i + m_b))] that accounts for ion and buffer gas masses
+        """
+        return self.z * (X[0] + t_fix) / (beta * self._mass_term(X[1]))
+
+    def _mass_term(self, mz):
+        """
+        compute sqrt(m_i / (m_i + m_b)) term for m/z of ion and buffer gas
+        """
+        m = mz * self.z  # mass not m/z
+        return np.sqrt(m / (m + self.buffer_gas_mass))
+
+    def calibrated_ccs(self, mz, arrival_time):
+        """
+        returns calibrated CCS values for a set of m/z values and arrival times (also works for single values)
+
+        Parameters
+        ----------
+        mz : ``numpy.ndarray(float)`` or ``float``
+            m/z value(s)
+        arrival_time : ``numpy.ndarray(float)`` or ``float``
+            arrival time(s)
+
+        Returns
+        -------
+        calibrated_ccs : ``numpy.ndarray(float)`` or ``float``
+            calibrated CCS value(s)
+        """
+        if type(mz) == float:
+            X = np.array([[arrival_time], [mz]])
+        else:
+            X = np.array([arrival_time, mz])
+        return self.transform(X)
+
+
+class CCSCalibrationTW(_CalibrationBase):
+    """
+    TWIMS CCS calibration
 
     Attributes
     ----------
     mz : ``numpy.ndarray(float)``
         calibrant m/z values
     arrival_time : ``numpy.ndarray(float)``
         calibrant arrival times
@@ -171,15 +338,15 @@
         'N2': monoiso_mass({'N': 2}), 
         'He': monoiso_mass({'He': 1}),
     }
 
     def __init__(self, mz, arrival_time, ref_ccs, z, fit_func,
                  correct_ccs=True, correct_dt=False, edc=None, buffer_gas='N2', fit=True):
         """
-        Initialize a new instance of TWCCSCalibration using 
+        Initialize a new instance of CCSCalibrationTW 
 
         Performs fitting at initialization.
 
         Parameters
         ----------
         mz : ``numpy.ndarray(float)``
             calibrant m/z values
@@ -205,26 +372,27 @@
             specify buffer gas for IM separation
         fit : ``bool``, default=True
             perform fitting at initialization
         """
         # validate and store parameters
         self.mz, self.arrival_time, self.ref_ccs, self.z, self.fit_func =  mz, arrival_time, ref_ccs, float(z), fit_func
         if self.fit_func not in self._valid_fit_funcs:
-            msg = 'TWCCSCalibration: __init__: fit_func "{}" invalid, must be one of: {}'
-            raise ValueError(msg.format(self.fit_func, self._valid_fit_funcs))
+            msg = 'CCSCalibrationTW: __init__: fit_func "{}" invalid, must be one of: {}'
+            valid_func_names = [_ for _ in self._valid_fit_funcs.keys()]
+            raise ValueError(msg.format(self.fit_func, valid_func_names))
         # set fit_function and init_params based on fit_func
         self.fit_function, self.init_params = self._valid_fit_funcs[self.fit_func]
         self.correct_ccs, self.correct_dt, self.edc = correct_ccs, correct_dt, edc
         if self.correct_dt and self.edc is None:
-            msg = 'TWCCSCalibration: __init__: correct_dt was set but no edc was provided'
+            msg = 'CCSCalibrationTW: __init__: correct_dt was set but no edc was provided'
             raise ValueError(msg)
         self.buffer_gas = buffer_gas
         if self.buffer_gas not in self._valid_buffer_gasses:
-            msg = 'TWCCSCalibration: __init__: buffer_gas "{}" invalid, must be one of: {}'
-            raise ValueError(msg.format(self.fit_func, self._valid_buffer_gasses))
+            msg = 'CCSCalibrationTW: __init__: buffer_gas "{}" invalid, must be one of: {}'
+            raise ValueError(msg.format(self.buffer_gas, self._valid_buffer_gasses))
         self.buffer_gas_mass = self._valid_buffer_gasses[self.buffer_gas]
         if fit:
             # setup values for fitting, make corrections if applicable
             self._X = self._correct_dt(self.arrival_time, self.mz) if self.correct_dt else self.arrival_time
             self._y = self._correct_ccs(self.ref_ccs, self.mz) if self.correct_ccs else self.ref_ccs
             # fit calibration curve
             self._y_fit = self.fit(self._X, self._y)
@@ -260,10 +428,15 @@
 
         Parameters
         ----------
         mz : ``numpy.ndarray(float)`` or ``float``
             m/z value(s)
         arrival_time : ``numpy.ndarray(float)`` or ``float``
             arrival time(s)
+
+        Returns
+        -------
+        calibrated_ccs : ``numpy.ndarray(float)`` or ``float``
+            calibrated CCS value(s)
         """
         ccs = self.transform(self._correct_dt(arrival_time, mz) if self.correct_dt else arrival_time)
         return self._inverse_correct_ccs(ccs, mz) if self.correct_ccs else ccs
```

### Comparing `mzapy-1.5.3/mzapy/isotopes.py` & `mzapy-1.6.3/mzapy/isotopes.py`

 * *Files identical despite different names*

### Comparing `mzapy-1.5.3/mzapy/peaks.py` & `mzapy-1.6.3/mzapy/peaks.py`

 * *Files identical despite different names*

### Comparing `mzapy-1.5.3/mzapy/view.py` & `mzapy-1.6.3/mzapy/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 """
 
 
 from functools import wraps
 
 from matplotlib import pyplot as plt, rcParams
 
+from mzapy._util import _ppm_error
+
 
 # always set font size to 6 on import
 rcParams['font.size'] = 6
 
 
 def _setup_and_save_or_show_plot(label, ax, figname, figsize, ign_newax):
     """
@@ -352,22 +354,117 @@
                 ls='-', c=c, lw=1)
         if add_text_lbl:
             s = '{:.1e} +/- {:.1e} {}\n{:.1e}'.format(pk_mean, pk_width, x_units, pk_height)
             # add some text with the peak info
             ax.text(pk_mean + pk_width / 2, 0.75 * pk_height, s, size=fontsize, c=c)
 
 
+def plot_mass_calibration(calibration, figname=None):
+    """
+    Generates a plot of a mass calibration from a fitted instance of ``mzapy.calibration.MassCalibration``
+
+    Parameters
+    ----------
+    calibration : ``mzapy.calibration.MassCalibration``
+        fitted mass calibration instance
+    figname : ``str``, optional
+        if not provided, do not save the figure or display it for interactive viewing. if figname is "show" then
+        display the figure for interactive viewing, and if figname is a path to an image file then save the image to
+        that path
+    """
+    # ensure that the calibration has been fitted
+    if calibration.opt_params is None:
+        msg = 'plot_mass_calibration: calibration has not been fit yet (calibration.opt_params is None)'
+        raise RuntimeError(msg)
+    # get reference and fitted values
+    X, y, y_fit = calibration._X, calibration._y, calibration._y_fit
+    ppms = _ppm_error(y, y_fit)
+    # get a text description of the fit parameters
+    text_format = {
+        'linear': "Y = {:.6f} * X {:+.6f}",
+    }
+    param_text = text_format[calibration.fit_func].format(*calibration.opt_params)
+    fig, axs = plt.subplots(nrows=2, figsize=(3.33, 4), gridspec_kw={'height_ratios': [2.5, 1]})
+    xlab = 'm/z (obs.)'
+    axs[0].plot(X, y, 'b.', ms=5)
+    axs[0].plot(X, y_fit, 'b--', lw=0.75)
+    axs[0].set_ylabel('m/z (ref.)')
+    axs[0].text(0.05, 1., param_text, color='b', transform=axs[0].transAxes)
+    axs[1].plot(X, ppms, 'b.', ms=5)
+    axs[1].axhline(0, ls='--', lw=0.5, color='k')
+    axs[1].set_xlabel(xlab)
+    axs[1].set_ylabel('ppm error')
+    for ax in axs:
+        for d in ['top', 'right']:
+            ax.spines[d].set_visible(False)
+    if figname is not None:
+        plt.tight_layout()
+        if figname == 'show':
+            plt.show()
+        else:
+            plt.savefig(figname, dpi=350, bbox_inches='tight')
+
+
+def plot_dtsf_ccs_calibration(calibration, figname=None):
+    """
+    Generates a plot of a single-filed DTIMS CCS calibration from a fitted 
+    instance of ``mzapy.calibration.CCSCalibrationDTsf``
+
+    Parameters
+    ----------
+    calibration : ``mzapy.calibration.CCSCalibrationDTsf``
+        fitted single-field DTIMS CCS calibration instance
+    figname : ``str``, optional
+        if not provided, do not save the figure or display it for interactive viewing. if figname is "show" then
+        display the figure for interactive viewing, and if figname is a path to an image file then save the image to
+        that path
+    """
+    # ensure that the calibration has been fitted
+    if calibration.opt_params is None:
+        msg = 'plot_dtsf_ccs_calibration: calibration has not been fit yet (calibration.opt_params is None)'
+        raise RuntimeError(msg)
+    # get reference and fitted values
+    y, y_fit = calibration._y, calibration._y_fit
+    dt = calibration.arrival_time
+    ccs_ref = calibration.ref_ccs
+    ccs_cal = calibration.calibrated_ccs(calibration.mz, calibration.arrival_time)
+    percent_error = 100. * (ccs_cal - ccs_ref) / ccs_ref
+    # get a text description of the fit parameters
+    text_format = 't_fix = {:+.4f}\nbeta = {:.4f}' 
+    param_text = text_format.format(*calibration.opt_params)
+    fig, axs = plt.subplots(nrows=2, figsize=(3.33, 4), gridspec_kw={'height_ratios': [2.5, 1]})
+    xlab = 'arrival time (ms)'
+    axs[0].plot(dt, y, 'b.', ms=5)
+    axs[0].plot(dt, y_fit, 'b--', lw=0.75)
+    axs[0].set_ylabel('CCS (Ang^2)')
+    axs[0].text(0.05, 1., param_text, color='b', transform=axs[0].transAxes)
+    axs[1].plot(dt, percent_error, 'b.', ms=5)
+    axs[1].axhline(0, ls='--', lw=0.5, color='k')
+    axs[1].set_xlabel(xlab)
+    axs[1].set_ylabel('CCS % error')
+    for ax in axs:
+        for d in ['top', 'right']:
+            ax.spines[d].set_visible(False)
+    if figname is not None:
+        plt.tight_layout()
+        if figname == 'show':
+            plt.show()
+        else:
+            plt.savefig(figname, dpi=350, bbox_inches='tight')
+
+
 def plot_tw_ccs_calibration(calibration, figname=None):
     """
-    Generates a plot of a TW CCS calibration from a fitted instance of ``mzapy.calibration.TWCCSCalibration``
+    Generates a plot of a TWIMS CCS calibration from a fitted 
+    instance of ``mzapy.calibration.CCSCalibrationTW``
 
     Parameters
     ----------
-    calibration : ``mzapy.calibration.TWCCSCalibration``
-        fitted TW CCS calibration instance
+    calibration : ``mzapy.calibration.CCSCalibrationTW``
+        fitted TWIMS CCS calibration instance
     figname : ``str``, optional
         if not provided, do not save the figure or display it for interactive viewing. if figname is "show" then
         display the figure for interactive viewing, and if figname is a path to an image file then save the image to
         that path
     """
     # ensure that the calibration has been fitted
     if calibration.opt_params is None:
@@ -376,17 +473,17 @@
     # get reference and fitted values
     X, y, y_fit = calibration._X, calibration._y, calibration._y_fit
     ccs_ref = calibration.ref_ccs
     ccs_cal = calibration.calibrated_ccs(calibration.mz, calibration.arrival_time)
     percent_error = 100. * (ccs_cal - ccs_ref) / ccs_ref
     # get a text description of the fit parameters
     text_format = {
-        'linear': "Y = {:.2e} * X + {:.2e}",
-        'quadratic': "Y = {:.2e} * X^2 + {:.2e} * X + {:.2e}",
-        'power1': "Y = {:.2e} + {:.2e} * X^{:.3f}",
+        'linear': "Y = {:.2e} * X {:+.2e}",
+        'quadratic': "Y = {:.2e} * X^2 {:+.2e} * X {:+.2e}",
+        'power1': "Y = {:.2e} {:+.2e} * X^{:.3f}",
         'power2': "Y = {:.2e} * (X {:+5.2e})^{:.3f}",
     }
     param_text = text_format[calibration.fit_func].format(*calibration.opt_params)
     fig, axs = plt.subplots(nrows=2, figsize=(3.33, 4), gridspec_kw={'height_ratios': [2.5, 1]})
     xlab = 'arrival time (corrected)' if calibration.correct_dt else 'arrival time'
     axs[0].plot(X, y, 'b.', ms=5)
     axs[0].plot(X, y_fit, 'b--', lw=0.75)
@@ -401,7 +498,9 @@
             ax.spines[d].set_visible(False)
     if figname is not None:
         plt.tight_layout()
         if figname == 'show':
             plt.show()
         else:
             plt.savefig(figname, dpi=350, bbox_inches='tight')
+
+
```

### Comparing `mzapy-1.5.3/mzapy.egg-info/PKG-INFO` & `mzapy-1.6.3/mzapy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzapy
-Version: 1.5.3
+Version: 1.6.3
 Summary: A Python package that provides an interface to unprocessed MS data in the MZA format.
 Home-page: https://github.com/PNNL-m-q/mzapy
 Author: Dylan Ross
 Author-email: dylan.ross@pnnl.gov
 Project-URL: Bug Tracker, https://github.com/PNNL-m-q/mzapy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `mzapy-1.5.3/setup.cfg` & `mzapy-1.6.3/setup.cfg`

 * *Files identical despite different names*

