# Comparing `tmp/p_winds-1.4.1b0.tar.gz` & `tmp/p_winds-1.4.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p_winds-1.4.1b0.tar", last modified: Thu Nov 17 20:34:43 2022, max compression
+gzip compressed data, was "p_winds-1.4.4b0.tar", last modified: Mon Apr 10 23:40:24 2023, max compression
```

## Comparing `p_winds-1.4.1b0.tar` & `p_winds-1.4.4b0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:34:43.320587 p_winds-1.4.1b0/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-17 20:34:43.320587 p_winds-1.4.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3299 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:34:43.320587 p_winds-1.4.1b0/p_winds/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25087 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/carbon.py
--rw-r--r--   0 runner    (1001) docker     (121)    18033 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/energetics.py
--rw-r--r--   0 runner    (1001) docker     (121)    42366 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/helium.py
--rw-r--r--   0 runner    (1001) docker     (121)    22102 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/hydrogen.py
--rw-r--r--   0 runner    (1001) docker     (121)     4764 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/lines.py
--rw-r--r--   0 runner    (1001) docker     (121)    12662 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/microphysics.py
--rw-r--r--   0 runner    (1001) docker     (121)    18608 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/oxygen.py
--rw-r--r--   0 runner    (1001) docker     (121)    13134 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/parker.py
--rw-r--r--   0 runner    (1001) docker     (121)     7229 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    20828 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/p_winds/transit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 20:34:43.320587 p_winds-1.4.1b0/p_winds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-11-17 20:34:43.000000 p_winds-1.4.1b0/p_winds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-11-17 20:34:43.000000 p_winds-1.4.1b0/p_winds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 20:34:43.000000 p_winds-1.4.1b0/p_winds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-17 20:34:43.000000 p_winds-1.4.1b0/p_winds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-17 20:34:43.000000 p_winds-1.4.1b0/p_winds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 20:34:43.320587 p_winds-1.4.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      905 2022-11-17 20:34:33.000000 p_winds-1.4.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:40:24.298538 p_winds-1.4.4b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-10 23:40:24.298538 p_winds-1.4.4b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:40:24.298538 p_winds-1.4.4b0/p_winds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18412 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/energetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44850 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/helium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23949 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/hydrogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/microphysics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20269 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/oxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/parker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21205 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/p_winds/transit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 23:40:24.298538 p_winds-1.4.4b0/p_winds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-10 23:40:24.000000 p_winds-1.4.4b0/p_winds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 23:40:24.000000 p_winds-1.4.4b0/p_winds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 23:40:24.000000 p_winds-1.4.4b0/p_winds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-10 23:40:24.000000 p_winds-1.4.4b0/p_winds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 23:40:24.000000 p_winds-1.4.4b0/p_winds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 23:40:24.298538 p_winds-1.4.4b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-10 23:40:15.000000 p_winds-1.4.4b0/setup.py
```

### Comparing `p_winds-1.4.1b0/LICENSE` & `p_winds-1.4.4b0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Leonardo A. dos Santos
+Copyright (c) 2023 Leonardo A. dos Santos
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `p_winds-1.4.1b0/README.md` & `p_winds-1.4.4b0/README.md`

 * *Files identical despite different names*

### Comparing `p_winds-1.4.1b0/p_winds/carbon.py` & `p_winds-1.4.4b0/p_winds/oxygen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,579 +1,491 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-This module computes the neutral and ionized populations of C in the upper
+This module computes the neutral and ionized populations of O in the upper
 atmosphere.
 """
 
 from __future__ import (division, print_function, absolute_import,
                         unicode_literals)
 import numpy as np
 import astropy.units as u
 import astropy.constants as c
 from scipy.integrate import simps, solve_ivp, odeint
-from scipy.interpolate import interp1d
-from scipy.special import exp1
 from p_winds import tools, microphysics
 import warnings
 
 
 __all__ = ["radiative_processes", "electron_impact_ionization", "recombination",
            "charge_transfer", "ion_fraction"]
 
 
 # Some hard coding based on the astrophysical literature
-_SOLAR_CARBON_ABUNDANCE_ = 8.43  # Asplund et al. 2009
-_SOLAR_CARBON_FRACTION_ = 10 ** (_SOLAR_CARBON_ABUNDANCE_ - 12.00)
-_SOLAR_SILICON_ABUNDANCE_ = 7.51  # Asplund et al. 2009
-_SOLAR_SILICON_FRACTION_ = 10 ** (_SOLAR_SILICON_ABUNDANCE_ - 12.00)
+_SOLAR_OXYGEN_ABUNDANCE_ = 8.69  # Asplund et al. 2009
+_SOLAR_OXYGEN_FRACTION_ = 10 ** (_SOLAR_OXYGEN_ABUNDANCE_ - 12.00)
 
 
-# Photoionization of C I (neutral) and C II (singly-ionized)
+# Photoionization of O I (neutral)
 def radiative_processes(spectrum_at_planet):
     """
-    Calculate the photoionization rate of carbon at null optical depth based
+    Calculate the photoionization rate of oxygen at null optical depth based
     on the EUV spectrum arriving at the planet.
 
     Parameters
     ----------
-    spectrum_at_planet (``dict``):
+    spectrum_at_planet : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes at
         least up to the wavelength corresponding to the energy to ionize
-        carbon (11.26 eV, or 1101 Angstrom).
+        oxygen (13.62 eV, or 910 Angstrom).
 
     Returns
     -------
-    phi_ci (``float``):
-        Ionization rate of C I at null optical depth in unit of 1 / s.
+    phi_oi : ``float``
+        Ionization rate of O I at null optical depth in unit of 1 / s.
 
-    phi_cii (``float``):
-        Ionization rate of C II at null optical depth in unit of 1 / s.
+    a_oi : ``float``
+        Flux-averaged photoionization cross-section of O I in unit of cm ** 2.
 
-    a_ci (``float``):
-        Flux-averaged photoionization cross-section of C I in unit of cm ** 2.
-
-    a_cii (``float``):
-        Flux-averaged photoionization cross-section of C II in unit of cm ** 2.
-
-    a_h_ci (``float``):
+    a_h_oi : ``float``
         Flux-averaged photoionization cross-section of H I in the range absorbed
-        by C I in unit of cm ** 2.
+        by O I in unit of cm ** 2.
 
-    a_h_cii (``float``):
-        Flux-averaged photoionization cross-section of H I in the range absorbed
-        by C II in unit of cm ** 2.
-
-    a_he (``float``):
+    a_he : ``float``
         Flux-averaged photoionization cross-section of He I in unit of cm ** 2.
     """
     wavelength = (spectrum_at_planet['wavelength'] *
                   spectrum_at_planet['wavelength_unit']).to(u.angstrom).value
     flux_lambda = (spectrum_at_planet['flux_lambda'] * spectrum_at_planet[
         'flux_unit']).to(u.erg / u.s / u.cm ** 2 / u.angstrom).value
     energy = ((c.h * (c.c / wavelength / u.angstrom).to(u.Hz)).to(u.eV)).value
     energy_erg = (energy * u.eV).to(u.erg).value
 
     # Auxiliary definitions
     parameters_dict = microphysics.sigma_properties_v1996()
-    energy_threshold_ci = parameters_dict['C I'][0]  # Ionization threshold in
-    # eV
-    energy_threshold_cii = parameters_dict['C II'][0]  # Ionization threshold in
+
+    energy_threshold_oi = parameters_dict['O I'][0]  # Ionization threshold in
     # eV
-    wl_break_ci = 12398.42 / energy_threshold_ci  # C I ionization threshold in
+    wl_break_oi = 12398.42 / energy_threshold_oi  # O I ionization threshold in
     # angstrom
-    wl_break_cii = 12398.42 / energy_threshold_cii  # C II ionization threshold
-    # in angstrom
     wl_break_he = 504  # He ionization threshold in angstrom
     i0 = tools.nearest_index(wavelength, wl_break_he)
-    i1 = tools.nearest_index(wavelength, wl_break_ci)
-    i2 = tools.nearest_index(wavelength, wl_break_cii)
+    i1 = tools.nearest_index(wavelength, wl_break_oi)
     wavelength_cut_0 = wavelength[:i0]
     flux_lambda_cut_0 = flux_lambda[:i0]
     wavelength_cut_1 = wavelength[:i1]
     flux_lambda_cut_1 = flux_lambda[:i1]
     energy_cut_1 = energy_erg[:i1]
-    wavelength_cut_2 = wavelength[:i2]
-    flux_lambda_cut_2 = flux_lambda[:i2]
-    energy_cut_2 = energy_erg[:i2]
 
     # Calculate the photoionization cross-section
-    a_lambda_ci = microphysics.general_cross_section(wavelength_cut_1,
-                                                     species='C I')
-    a_lambda_cii = microphysics.general_cross_section(wavelength_cut_2,
-                                                      species='C II')
+    a_lambda_oi = microphysics.general_cross_section(wavelength_cut_1,
+                                                     species='O I')
 
-    # The flux-averaged photoionization cross-section of C I and C II
-    a_ci = abs(simps(flux_lambda_cut_1 * a_lambda_ci, wavelength_cut_1) /
+    # The flux-averaged photoionization cross-section of O I
+    a_oi = abs(simps(flux_lambda_cut_1 * a_lambda_oi, wavelength_cut_1) /
                simps(flux_lambda_cut_1, wavelength_cut_1))
-    a_cii = abs(simps(flux_lambda_cut_2 * a_lambda_cii, wavelength_cut_2) /
-                simps(flux_lambda_cut_2, wavelength_cut_2))
 
     # The flux-averaged photoionization cross-section of H is also going to be
-    # needed because it adds to the optical depth that C I and C II see.
-    a_lambda_h_ci = microphysics.hydrogen_cross_section(
+    # needed because it adds to the optical depth that O I see.
+    a_lambda_h_oi = microphysics.hydrogen_cross_section(
         wavelength=wavelength_cut_1)
-    a_h_ci = abs(simps(flux_lambda_cut_1 * a_lambda_h_ci, wavelength_cut_1) /
+    a_h_oi = abs(simps(flux_lambda_cut_1 * a_lambda_h_oi, wavelength_cut_1) /
                  simps(flux_lambda_cut_1, wavelength_cut_1))
-    a_lambda_h_cii = microphysics.hydrogen_cross_section(
-        wavelength=wavelength_cut_2)
-    a_h_cii = abs(simps(flux_lambda_cut_2 * a_lambda_h_cii, wavelength_cut_2) /
-                  simps(flux_lambda_cut_2, wavelength_cut_2))
 
     # Same for the He atoms, but only up to the He ionization threshold
     a_lambda_he = microphysics.helium_total_cross_section(wavelength_cut_0)
     a_he = abs(simps(flux_lambda_cut_0 * a_lambda_he, wavelength_cut_0) /
                simps(flux_lambda_cut_0, wavelength_cut_0))
 
     # Calculate the photoionization rates
-    phi_ci = abs(simps(flux_lambda_cut_1 * a_lambda_ci / energy_cut_1,
-                 wavelength_cut_1))
-    phi_cii = abs(simps(flux_lambda_cut_2 * a_lambda_cii / energy_cut_2,
-                        wavelength_cut_2))
+    phi_oi = abs(simps(flux_lambda_cut_1 * a_lambda_oi / energy_cut_1,
+                       wavelength_cut_1))
 
-    return phi_ci, phi_cii, a_ci, a_cii, a_h_ci, a_h_cii, a_he
+    return phi_oi, a_oi, a_h_oi, a_he
 
 
-# Ionization rate of C by electron impact
+# Ionization rate of O by electron impact
 def electron_impact_ionization(electron_temperature):
     """
-    Calculates the electron impact ionization rate that consumes neutral C and
-    produces singly-ionized C. Based on the formula of Voronov 1997
+    Calculates the electron impact ionization rate that consumes neutral O and
+    produces singly-ionized O. Based on the formula of Voronov 1997
     (https://ui.adsabs.harvard.edu/abs/1997ADNDT..65....1V/abstract).
 
     Parameters
     ----------
-    electron_temperature (``float``):
+    electron_temperature : ``float``
         Temperature of the plasma where the electrons are embedded in unit of
         Kelvin.
 
     Returns
     -------
-    ionization_rate_ci (``float``):
-        Ionization rate of neutral C into singly-ionized C in unit of
-        cm ** 3 / s.
-
-    ionization_rate_cii (``float``):
-        Ionization rate of singly-ionized C into doubly-ionized C in unit of
+    ionization_rate_oi : ``float``
+        Ionization rate of neutral O into singly-ionized O in unit of
         cm ** 3 / s.
     """
     boltzmann_constant = 8.617333262145179e-05  # eV / K
     electron_energy = boltzmann_constant * electron_temperature
-    energy_ratio_ci = 11.3 / electron_energy
-    energy_ratio_cii = 24.4 / electron_energy
-    ionization_rate_ci = 6.85E-8 * (0.193 + energy_ratio_ci) ** (-1) * \
-        energy_ratio_ci ** 0.25 * np.exp(-energy_ratio_ci)
-    ionization_rate_cii = 1.86E-8 * (0.286 + energy_ratio_cii) ** (-1) * \
-        energy_ratio_cii ** 0.24 * np.exp(-energy_ratio_cii)
-    return ionization_rate_ci, ionization_rate_cii
+    energy_ratio_oi = 11.3 / electron_energy
+    ionization_rate_oi = 3.59E-8 * (0.073 + energy_ratio_oi) ** (-1) * \
+        energy_ratio_oi ** 0.34 * np.exp(-energy_ratio_oi)
+    return ionization_rate_oi
 
 
-# Recombination of singly-ionized C into neutral C
+# Recombination of singly-ionized O into neutral O
 def recombination(electron_temperature):
     """
-    Calculates the rate of recombination of singly-ionized C with an electron to
-    produce a neutral C atom. Based on the formulation of Woodall et al. 2007
-    (https://ui.adsabs.harvard.edu/abs/2007A%26A...466.1197W/abstract). Also
-    calculates the recombination of doubly-ionized C with an electron to produce
-    a singly-ionized C ion. Based on the formulation of Aldrovandi & Péquignot
-    1973 (https://ui.adsabs.harvard.edu/abs/1973A%26A....25..137A/abstract).
+    Calculates the rate of recombination of singly-ionized O with an electron to
+    produce a neutral O atom. Based on the formulation of Woodall et al. 2007
+    (https://ui.adsabs.harvard.edu/abs/2007A%26A...466.1197W/abstract).
 
     Parameters
     ----------
-    electron_temperature (``float``):
+    electron_temperature : ``float``
         Temperature of the plasma where the electrons are embedded in unit of
         Kelvin.
 
     Returns
     -------
-    alpha_rec_ci (``float``):
-        Recombination rate of C II into C I in units of cm ** 3 / s.
-
-    alpha_rec_cii (``float``):
-        Recombination rate of C III into C II in units of cm ** 3 / s.
+    alpha_rec_oi  : ``float``
+        Recombination rate of O II into O I in units of cm ** 3 / s.
     """
-    alpha_rec_ci = 4.67E-12 * (300 / electron_temperature) ** 0.60
-    alpha_rec_cii = 2.3E-12 * (1000 / electron_temperature) ** 0.645
-    return alpha_rec_ci, alpha_rec_cii
+    alpha_rec_oi = 3.25E-12 * (300 / electron_temperature) ** 0.66
+    return alpha_rec_oi
 
 
-# Charge transfer between C and H, He and Si
+# Charge transfer between O and H
 def charge_transfer(temperature):
     """
-    Calculates the charge exchange rates of C with H, He and Si nuclei. Based on
-    the formulation of Stancil et al. 1998
-    (https://ui.adsabs.harvard.edu/abs/1998ApJ...502.1006S/abstract),
-    Woodall et al. 2007
-    (https://ui.adsabs.harvard.edu/abs/2007A%26A...466.1197W/abstract),
-    Glover & Jappsen 2007
-    (https://ui.adsabs.harvard.edu/abs/2007ApJ...666....1G/abstract),
-    Kingdon & Ferland 1996
-    (https://ui.adsabs.harvard.edu/abs/1996ApJS..106..205K/abstract), and
-    Brown 1972 (https://ui.adsabs.harvard.edu/abs/1972ApJ...174..511B/abstract).
+    Calculates the charge exchange rates of O with H nuclei. Based on the
+    formulation of Woodall et al. 2007
+    (https://ui.adsabs.harvard.edu/abs/2007A%26A...466.1197W/abstract).
 
     Parameters
     ----------
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
     Returns
     -------
-    ct_rate_ci_hp (``float``):
-        Charge transfer rate between neutral C and H+ in units of cm ** 3 / s.
-
-    ct_rate_cii_h (``float``):
-        Charge transfer rate between C+ and neutral H in units of cm ** 3 / s.
+    ct_rate_oi_hp : ``float``
+        Charge transfer rate between neutral O and H+ in units of cm ** 3 / s.
 
-    ct_rate_ci_hep (``float``):
-        Charge transfer rate between neutral C and He+ in units of cm ** 3 / s.
-
-    ct_rate_cii_sii (``float``):
-        Charge transfer rate between C+ and neutral Si in units of cm ** 3 / s.
-
-    ct_rate_ciii_h (``float``)
-        Charge transfer rate between C++ and neutral H in units of cm ** 3 / s.
-
-    ct_rate_ciii_he (``float``)
-        Charge transfer rate between C++ and neutral He in units of cm ** 3 / s.
+    ct_rate_oii_h : ``float``
+        Charge transfer rate between O+ and neutral H in units of cm ** 3 / s.
     """
-    # Recombination of C II into C I
-    ct_rate_cii_h = 6.30E-17 * (300 / temperature) ** (-1.96) * \
-        np.exp(-1.7E5 / temperature)
-    ct_rate_cii_sii = 2.1E-9
-
-    # Ionization of C I into C II
-    ct_rate_ci_hp = 1.31E-15 * (300 / temperature) ** (-0.213)
-    ct_rate_ci_hep = 2.5E-15 * (300 / temperature) ** (-1.597)
-
-    # Recombination of C III into C II
-    ct_rate_ciii_h = 1.67E-4 * (temperature / 10000) ** 2.79 * \
-        (1 + 304.72 * np.exp(-4.07 * temperature / 10000))
-    ct_rate_ciii_he = 1.23E-9  # Very approximated from Brown 1972, but should
-    # be good enough for temperatures near 10,000 K
+    # Recombination of O II into O I
+    ct_rate_oii_h = 5.66E-10 * (300 / temperature) ** (-0.36) * \
+        np.exp(8.6 / temperature)
 
-    return ct_rate_ci_hp, ct_rate_cii_h, ct_rate_ci_hep, ct_rate_cii_sii, \
-        ct_rate_ciii_h, ct_rate_ciii_he
+    # Ionization of O I into O II
+    ct_rate_oi_hp = 7.31E-10 * (300 / temperature) ** (-0.23) * \
+        np.exp(-226 / temperature)
 
+    return ct_rate_oi_hp, ct_rate_oii_h
 
-# Calculation the number fractions of C II and C III
+
+# Calculation the number fractions of O II
 def ion_fraction(radius_profile, velocity, density, hydrogen_ion_fraction,
                  helium_ion_fraction, planet_radius, temperature, h_fraction,
                  speed_sonic_point, radius_sonic_point, density_sonic_point,
-                 spectrum_at_planet, c_fraction=_SOLAR_CARBON_FRACTION_,
-                 initial_f_c_ion=np.array([0.0, 0.0]), relax_solution=False,
-                 convergence=0.01, max_n_relax=10, method='odeint',
+                 spectrum_at_planet, o_fraction=_SOLAR_OXYGEN_FRACTION_,
+                 initial_f_o_ion=0.0, relax_solution=False, convergence=0.01,
+                 max_n_relax=10, method='Radau', return_rates=False,
                  **options_solve_ivp):
     """
-    Calculates the fractions of singly- and doubly-ionized carbon in the upper
-    atmosphere in function of the radius in unit of planetary radius.
+    Calculate the fraction of ionized oxygen in the upper atmosphere in function
+    of the radius in unit of planetary radius.
 
     Parameters
     ----------
-    radius_profile (``numpy.ndarray``):
+    radius_profile : ``numpy.ndarray``
         Radius in unit of planetary radii.
 
-    velocity (``numpy.ndarray``):
+    velocity : ``numpy.ndarray``
          Velocities sampled at the values of ``radius_profile`` in units of
          sound speed. Similar to the output of ``parker.structure()``.
 
-    density (``numpy.ndarray``):
+    density : ``numpy.ndarray``
         Densities sampled at the values of ``radius_profile`` in units of
         density at the sonic point. Similar to the output of
         ``parker.structure()``.
 
-    hydrogen_ion_fraction (``numpy.ndarray``):
+    hydrogen_ion_fraction : ``numpy.ndarray``
         Number fraction of H ion over total H in the upper atmosphere in
         function of radius. Similar to the output of
         ``hydrogen.ion_fraction()``.
 
-    helium_ion_fraction (``numpy.ndarray``):
+    helium_ion_fraction : ``numpy.ndarray``
         Number fraction of He ion over total He in the upper atmosphere in
         function of radius. Similar to the output of
         ``helium.population_fraction()``, but should be ``1 - f_1_r - f_3_r``.
 
-    planet_radius (``float``):
+    planet_radius : ``float``
         Planetary radius in unit of Jupiter radius.
 
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
-    h_fraction (``float``):
+    h_fraction : ``float``
         Total (ion + neutral) H number fraction of the atmosphere.
 
-    speed_sonic_point (``float``):
+    speed_sonic_point : ``float``
         Speed of sound in the outflow in units of km / s.
 
-    radius_sonic_point (``float``):
+    radius_sonic_point : ``float``
         Radius of the sonic point in unit of Jupiter radius.
 
-    density_sonic_point (``float``):
+    density_sonic_point : ``float``
         Density at the sonic point in units of g / cm ** 3.
 
-    spectrum_at_planet (``dict``):
+    spectrum_at_planet : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes at
         least up to the wavelength corresponding to the energy to ionize
-        carbon (11.26 eV, or 1101 Angstrom). Can be generated using
+        oxygen (13.62 eV, or 910 Angstrom). Can be generated using
         ``tools.make_spectrum_dict``.
 
-    c_fraction (``float``, optional):
-        Fraction of total carbon in the upper atmosphere. Default value assumes
+    o_fraction : ``float``, optional
+        Fraction of total oxygen in the upper atmosphere. Default value assumes
         solar abundance.
 
-    initial_f_c_ion (``numpy.ndarray``, optional):
-        The initial ion fractions are the `y0` of the differential equation to
-        be solved. This array has two items: the initial fraction of
-        singly-ionized and doubly-ionized carbon in the inner layer of the
-        atmosphere. The default value for this parameter is
-        ``numpy.array([0.0, 0.0])``, i.e., fully neutral at the inner layer.
+    initial_f_o_ion : ``float``, optional
+        The initial oxygen ion fraction at the layer near the surface of the
+        planet. Default is 0.0, i.e., 100% neutral.
 
-    relax_solution (``bool``, optional):
+    relax_solution : ``bool``, optional
         The first solution is calculating by initially assuming the entire
         atmosphere is in neutral state. If ``True``, the solution will be
         re-calculated in a loop until it converges to a delta_f of 1%, or for a
         maximum of 10 loops (default parameters). Default is ``False``.
 
-    convergence (``float``, optional):
+    convergence : ``float``, optional
         Value of delta_f at which to stop the relaxation of the solution for
         ``f_r``. Default is 0.01.
 
-    max_n_relax (``int``, optional):
+    max_n_relax : ``int``, optional
         Maximum number of loops to perform the relaxation of the solution for
         the ion fractions. Default is 10.
 
-    method (``str``, optional):
+    method : ``str``, optional
         If method is ``'odeint'``, then ``scipy.integrate.odeint()`` is used
         instead of ``scipy.integrate.solve_ivp()`` to calculate the steady-state
-        distribution of helium. The first seems to be at least twice faster than
-        the second in some situations. Any other method will fall back to an
-        option of ``solve_ivp()`` methods. For example, if ``method`` is set to
+        distribution of helium. Any other method will fall back to an option of
+        ``solve_ivp()`` methods. For example, if ``method`` is set to
         ``'Radau'``, then use ``solve_ivp(method='Radau')``. Default is
-        ``'odeint'``.
+        ``'Radau'``.
+
+    return_rates : ``bool``, optional
+        If ``True``, then this function also returns a ``dict`` object
+        containing the various reaction rates in function of radius and in units
+        of 1 / s. Default is ``False``.
 
     **options_solve_ivp:
         Options to be passed to the ``scipy.integrate.solve_ivp()`` solver. You
         may want to change the options ``atol`` (absolute tolerance; default is
         1E-6) or ``rtol`` (relative tolerance; default is 1E-3). If you are
         having numerical issues, you may want to decrease the tolerance by a
         factor of 10 or 100, or 1000 in extreme cases.
 
     Returns
     -------
-    f_cii_r (``numpy.ndarray``):
-        Fraction of singly-ionized carbon in function of radius.
+    f_oii_r : ``numpy.ndarray``
+            Fraction of singly-ionized oxygen in function of radius.
 
-    f_ciii_r (``numpy.ndarray``):
-        Fraction of doubly-ionized carbon in function of radius.
+    reaction_rates : ``dict``
+        Dictionary containing the reaction rates in function of radius and in
+        units of 1 / s. Only returned when ``return_rates`` is set to ``True``.
+        Here is a short description of the dict keys:
+
+        * `photoionization`: Photoionization of O I into O II
+        * `recombination`: Recombination of O II into O I
+        * `e_impact_ionization`: Electron impact ionization of O I into O II
+        * `charge_exchange_HII`: Charge exchange between O I and H II
+        * `charge_exchange_HI`: Charge exchange between O II and H I
     """
     vs = speed_sonic_point  # km / s
     rs = radius_sonic_point  # jupiterRad
     rhos = density_sonic_point  # g / cm ** 3
 
     # Recombination rates of C in unit of rs ** 2 * vs
     alpha_rec_unit = ((rs * 7.1492E+09) ** 2 * vs * 1E5)  # cm ** 3 / s
-    alpha_rec_ci, alpha_rec_cii = recombination(temperature)
-    alpha_rec_ci = alpha_rec_ci / alpha_rec_unit
-    alpha_rec_cii = alpha_rec_cii / alpha_rec_unit
+    alpha_rec_oi = recombination(temperature)
+    alpha_rec_oi = alpha_rec_oi / alpha_rec_unit
 
     # Hydrogen mass in unit of rhos * rs ** 3
     m_h_unit = (rhos * (rs * 7.1492E+09) ** 3)  # Converted to g
     m_h = 1.67262192E-24 / m_h_unit
 
     # Photoionization rates at null optical depth at the distance of the planet
     # from the host star, in unit of vs / rs, and the flux-averaged
     # cross-sections in units of rs ** 2
     phi_unit = vs * 1E5 / rs / 7.1492E+09  # 1 / s
-    phi_ci, phi_cii, a_ci, a_cii, a_h_ci, a_h_cii, a_he = radiative_processes(
-        spectrum_at_planet)
-    phi_ci = phi_ci / phi_unit
-    a_ci = a_ci / (rs * 7.1492E+09) ** 2
-    a_h_ci = a_h_ci / (rs * 7.1492E+09) ** 2
+    phi_oi, a_oi, a_h_oi, a_he = radiative_processes(spectrum_at_planet)
+    phi_oi = phi_oi / phi_unit
+    a_oi = a_oi / (rs * 7.1492E+09) ** 2
+    a_h_oi = a_h_oi / (rs * 7.1492E+09) ** 2
     a_he = a_he / (rs * 7.1492E+09) ** 2
 
     # Electron-impact ionization rate for C I in the same unit as the
     # recombination rates
-    ionization_rate_ci, ionization_rate_cii = \
-        electron_impact_ionization(temperature)
-    ionization_rate_ci = ionization_rate_ci / alpha_rec_unit
-    ionization_rate_cii = ionization_rate_cii / alpha_rec_unit
+    ionization_rate_oi = electron_impact_ionization(temperature)
+    ionization_rate_oi = ionization_rate_oi / alpha_rec_unit
 
     # Charge transfer rates in the same unit as the recombination rates
-    ct_rate_ci_hp, ct_rate_cii_h, ct_rate_ci_hep, ct_rate_cii_sii, \
-        ct_rate_ciii_h, ct_rate_ciii_he = charge_transfer(temperature)
-    ct_rate_cii_h = ct_rate_cii_h / alpha_rec_unit
-    ct_rate_ci_hp = ct_rate_ci_hp / alpha_rec_unit
-    ct_rate_ci_hep = ct_rate_ci_hep / alpha_rec_unit
-    ct_rate_ciii_h = ct_rate_ciii_h / alpha_rec_unit
-    ct_rate_ciii_he = ct_rate_ciii_he / alpha_rec_unit
+    ct_rate_oi_hp, ct_rate_oii_h = charge_transfer(temperature)
+    ct_rate_oii_h = ct_rate_oii_h / alpha_rec_unit
+    ct_rate_oi_hp = ct_rate_oi_hp / alpha_rec_unit
 
     # We solve the steady-state ionization balance in a similar way that we do
     # for He
 
     # The radius in unit of radius at the sonic point
     r = radius_profile * planet_radius / rs
     dr = np.diff(r)
-    dr = np.concatenate((dr, np.array([r[-1], ])))
-
-    # Some mock functions that will allow us to parse the values of ion
-    # fraction, velocity and density in function of radius
-    mock_f_h_ion_r = interp1d(r, hydrogen_ion_fraction,
-                              fill_value="extrapolate")
-    mock_f_he_ion_r = interp1d(r, helium_ion_fraction,
-                              fill_value="extrapolate")
-    mock_v_r = interp1d(r, velocity, fill_value="extrapolate")
-    mock_rho_r = interp1d(r, density, fill_value="extrapolate")
+    dr = np.concatenate((dr, np.array([dr[-1], ])))
 
     # With all this setup done, now we need to assume something about the
-    # distribution of neutral C in the atmosphere. Let's assume it based on the
+    # distribution of neutral O in the atmosphere. Let's assume it based on the
     # initial guess input.
     column_density = np.flip(np.cumsum(np.flip(dr * density)))  # Total column
-                                                                # density
+    # density
     column_density_h_0 = np.flip(  # Column density of atomic H only
         np.cumsum(np.flip(dr * density * (1 - hydrogen_ion_fraction))))
     he_fraction = 1 - h_fraction
     column_density_he_0 = np.flip(  # Column density of atomic He only
         np.cumsum(np.flip(dr * density * he_fraction *
                           (1 - helium_ion_fraction))))
-    k1 = h_fraction / (h_fraction + 4 * he_fraction + 6 * c_fraction) / m_h
-    k2 = he_fraction / (h_fraction + 4 * he_fraction + 6 * c_fraction) / m_h
-    k3 = c_fraction / (h_fraction + 4 * he_fraction + 6 * c_fraction) / m_h
-    tau_ci_h = k1 * a_h_ci * column_density_h_0
-    tau_cii_h = k1 * a_h_cii * column_density_h_0
-    tau_c_he = k2 * a_he * column_density_he_0
-    tau_ci_initial = \
-        (1 - initial_f_c_ion[0] - initial_f_c_ion[1]) * k3 * a_ci * \
-        column_density + tau_ci_h + tau_c_he
-    tau_cii_initial = \
-        initial_f_c_ion[0] * k3 * a_cii * column_density + tau_cii_h + tau_c_he
-    # We do a dirty hack to make tau_initial a callable function so it's easily
-    # parsed inside the differential equation solver
-    _tau_ci_fun = interp1d(r, tau_ci_initial, fill_value="extrapolate")
-    _tau_cii_fun = interp1d(r, tau_cii_initial, fill_value="extrapolate")
+    k1 = h_fraction / (h_fraction + 4 * he_fraction + 16 * o_fraction) / m_h
+    k2 = he_fraction / (h_fraction + 4 * he_fraction + 16 * o_fraction) / m_h
+    k3 = o_fraction / (h_fraction + 4 * he_fraction + 16 * o_fraction) / m_h
+    tau_oi_h = k1 * a_h_oi * column_density_h_0
+    tau_o_he = k2 * a_he * column_density_he_0
+    tau_oi = (1 - initial_f_o_ion) * k3 * a_oi * column_density + tau_oi_h + \
+        tau_o_he
 
     # The differential equation
-    def _fun(_r, y):
-        f_cii = y[0]
-        f_ciii = y[1]
-
-        _v = mock_v_r(np.array([_r, ]))[0]
-        _rho = mock_rho_r(np.array([_r, ]))[0]
-        f_h_ion = mock_f_h_ion_r(np.array([_r, ]))[0]  # Fraction of H+
-        f_he_ion = mock_f_he_ion_r(np.array([_r, ]))[0]  # Fraction of He+
+    def _fun(_r, y, rates=False):
+        f_oii = y
+
+        _v = np.interp(_r, r, velocity)
+        _rho = np.interp(_r, r, density)
+        f_h_ion = np.interp(_r, r, hydrogen_ion_fraction)  # Fraction of H+
+        f_he_ion = np.interp(_r, r, helium_ion_fraction)  # Fraction of He+
 
         # Assume the number density of electrons is equal to the number density
         # of H ions + He ions
-        n_e = k1 * _rho * f_h_ion + k2 * _rho * f_he_ion  # Number density of
-        # electrons
-        n_h_plus = k1 * _rho * f_h_ion    # Number density of ionized H
-        n_h0 = k1 * _rho * (1 - f_h_ion)  # Number density of atomic H
-        n_he0 = k2 * _rho * (1 - f_he_ion)  # Number density of atomic He
-        n_he_plus = k2 * _rho * f_he_ion  # Number density of ionized He
-
-        # Terms of dfcii_dr
-        tau_ci = _tau_ci_fun(np.array([_r, ]))[0]
-        term11 = (1 - f_cii - f_ciii) * phi_ci * np.exp(-tau_ci)  # Photo-
+        # Since we may run into loss of numerical precision here (big numbers),
+        # we manipulate the equations to avoid this problem. It looks a bit
+        # messy, but it is necessary
+        log_term_1 = np.log(k1) + np.log(_rho)  # H ions
+        log_term_2 = np.log(k2) + np.log(_rho)  # He ions
+        ionization_rate_oi_n_e = \
+            np.exp(log_term_1 + np.log(ionization_rate_oi)) * f_h_ion + \
+            np.exp(log_term_2 + np.log(ionization_rate_oi)) * f_he_ion
+        ct_rate_oi_hp_n_h_plus = \
+            np.exp(log_term_1 + np.log(ct_rate_oi_hp)) * f_h_ion
+        alpha_rec_oi_n_e = \
+            np.exp(log_term_1 + np.log(alpha_rec_oi)) * f_h_ion + \
+            np.exp(log_term_2 + np.log(alpha_rec_oi)) * f_he_ion
+        ct_rate_oii_h_n_h0 = \
+            np.exp(log_term_1 + np.log(ct_rate_oii_h)) * (1 - f_h_ion)
+
+        # n_e = k1 * _rho * f_h_ion + k2 * _rho * f_he_ion  # Number density of
+        # # electrons
+        # n_h_plus = k1 * _rho * f_h_ion    # Number density of ionized H
+        # n_h0 = k1 * _rho * (1 - f_h_ion)  # Number density of atomic H
+
+        # Terms of dfoii_dr
+        t_oi = np.interp(_r, r, tau_oi)
+        term1 = (1 - f_oii) * phi_oi * np.exp(-t_oi)  # Photoionization
+        term2 = (1 - f_oii) * ionization_rate_oi_n_e  # Electron-impact
         # ionization
-        term12 = (1 - f_cii - f_ciii) * n_e * ionization_rate_ci  # Electron-
-        # impact ionization
-        term13 = (1 - f_cii - f_ciii) * n_h_plus * ct_rate_ci_hp  # Charge
-        # exchange with H+
-        term14 = (1 - f_cii - f_ciii) * n_he_plus * ct_rate_ci_hep  # Charge
-        # exchange with He+
-        term15 = f_cii * n_e * alpha_rec_ci  # Recombination of C II into C I
-        term16 = f_cii * n_h0 * ct_rate_cii_h  # Charge exchange of C II with
-        # neutral H
-        term17 = f_ciii * n_e * alpha_rec_cii  # Recombination of C III into
-        # C II
-        term18 = f_ciii * n_h0 * ct_rate_ciii_h  # Charge exchange of C III with
+        term3 = (1 - f_oii) * ct_rate_oi_hp_n_h_plus  # Charge exchange with
+        # H+
+        term4 = f_oii * alpha_rec_oi_n_e  # Recombination of O II into O I
+        term5 = f_oii * ct_rate_oii_h_n_h0  # Charge exchange of O II with
         # neutral H
-        term19 = f_ciii * n_he0 * ct_rate_ciii_he  # Charge exchange of C III
-        # with neutral He
-        dfcii_dr = (term11 + term12 + term13 + term14 - term15 - term16 +
-                    term17 + term18 + term19) / _v
-
-        # Terms of dfciii_dr
-        tau_cii = _tau_cii_fun(np.array([_r, ]))[0]
-        term21 = f_cii * phi_cii * np.exp(-tau_cii)  # Photoionization
-        term22 = f_cii * n_e * ionization_rate_cii  # Electron-impact ionization
-        dfciii_dr = (term21 + term22 - term17 - term18 - term19) / _v
+        dfoii_dr = (term1 + term2 + term3 - term4 - term5) / _v
 
-        return np.array([dfcii_dr, dfciii_dr])
+        if rates is False:
+            return dfoii_dr
+        else:
+            return np.array([term1, term4, term2, term3, term5]) * phi_unit
 
     if method == 'odeint':
         # Since 'odeint' yields only warnings when precision is lost or when
         # there is a problem, we transform these warnings into an exception
         with warnings.catch_warnings():
             warnings.filterwarnings("error")
             try:
-                sol = odeint(_fun, y0=initial_f_c_ion, t=r, tfirst=True)
+                sol = odeint(_fun, y0=initial_f_o_ion, t=r, tfirst=True)
             except Warning:
                 raise RuntimeError('The solver ``odeint`` failed to obtain a '
                                    'solution.')
-        f_cii_r = np.copy(sol).T[0]
-        f_ciii_r = np.copy(sol).T[1]
+        f_oii_r = np.copy(sol).T[0]
     else:
         # We solve it using `scipy.solve_ivp`
-        sol = solve_ivp(_fun, (r[0], r[-1],), initial_f_c_ion, t_eval=r,
-                        method=method, **options_solve_ivp)
-        f_cii_r = sol['y'][0]
-        f_ciii_r = sol['y'][1]
+        sol = solve_ivp(_fun, (r[0], r[-1],), np.array([initial_f_o_ion, ]),
+                        t_eval=r, method=method, **options_solve_ivp)
+        f_oii_r = sol['y'][0]
         # When `solve_ivp` has problems, it may return an array with different
         # size than `r`. So we raise an exception if this happens
-        if len(f_cii_r) != len(r) or len(f_ciii_r) != len(r):
+        if len(f_oii_r) != len(r):
             raise RuntimeError('The solver ``solve_ivp`` failed to obtain a'
                                ' solution.')
 
+    # High densities can be numerically unstable and produce unphysical values
+    # of `f_r`, so we replace negative values with zero and values above 1.0
+    # with 1.0
+    f_oii_r[f_oii_r < 0] = 1E-15
+    f_oii_r[f_oii_r > 1.0] = 1.0
+
     # For the sake of self-consistency, there is the option of repeating the
     # calculation of f_r by updating the optical depth with the new ion
     # fractions.
     if relax_solution is True:
         for i in range(max_n_relax):
-            previous_f_cii_r = np.copy(f_cii_r)
-            previous_f_ciii_r = np.copy(f_ciii_r)
+            previous_f_oii_r = np.copy(f_oii_r)
 
             # Re-calculate the column densities
-            tau_ci = \
-                k3 * a_ci * np.flip(np.cumsum(
-                    np.flip(dr * density * (1 - f_cii_r - f_ciii_r)))) + \
-                tau_ci_h + tau_c_he
-            tau_cii = k3 * a_cii * np.flip(
-                np.cumsum(np.flip(dr * density * f_cii_r))) + tau_cii_h + \
-                tau_c_he
-            _tau_ci_fun = interp1d(r, tau_ci, fill_value="extrapolate")
-            _tau_cii_fun = interp1d(r, tau_cii, fill_value="extrapolate")
+            tau_oi = \
+                k3 * a_oi * np.flip(np.cumsum(
+                    np.flip(dr * density * (1 - f_oii_r)))) + tau_oi_h + \
+                tau_o_he
 
             # Solve it again
             if method == 'odeint':
-                sol = odeint(_fun, y0=initial_f_c_ion, t=r, tfirst=True)
-                f_cii_r = np.copy(sol).T[0]
-                f_ciii_r = np.copy(sol).T[1]
+                sol = odeint(_fun, y0=initial_f_o_ion, t=r, tfirst=True)
+                f_oii_r = np.copy(sol).T[0]
             else:
-                sol = solve_ivp(_fun, (r[0], r[-1],), initial_f_c_ion,
-                                t_eval=r,
+                sol = solve_ivp(_fun, (r[0], r[-1],),
+                                np.array([initial_f_o_ion, ]), t_eval=r,
                                 method=method, **options_solve_ivp)
-                f_cii_r = sol['y'][0]
-                f_ciii_r = sol['y'][1]
+                f_oii_r = sol['y'][0]
 
             # Replace negative values with zero and values above 1.0 with
             # 1.0
-            f_cii_r[f_cii_r < 0] = 1E-15
-            f_ciii_r[f_ciii_r < 0] = 1E-15
-            f_cii_r[f_cii_r > 1.0] = 1.0
-            f_ciii_r[f_ciii_r > 1.0] = 1.0
+            f_oii_r[f_oii_r < 0] = 1E-15
+            f_oii_r[f_oii_r > 1.0] = 1.0
 
             # Calculate the relative change of f_ion in the outer shell of
             # the atmosphere (where we expect the most important change)
-            relative_delta_f_cii = abs(np.sum(f_cii_r - previous_f_cii_r)) \
-                / np.sum(previous_f_cii_r)
-            relative_delta_f_ciii = \
-                abs(np.sum(f_ciii_r - previous_f_ciii_r)) / \
-                np.sum(previous_f_ciii_r)
+            relative_delta_f_oii = abs(np.sum(f_oii_r - previous_f_oii_r)) \
+                / np.sum(previous_f_oii_r)
 
             # Break the loop if convergence is achieved
-            if relative_delta_f_cii < convergence and \
-                    relative_delta_f_ciii < convergence:
+            if relative_delta_f_oii < convergence:
                 break
             else:
                 pass
     else:
         pass
 
-    return f_cii_r, f_ciii_r
+    if return_rates is False:
+        return f_oii_r
+    else:
+        ionization_rate, recombination_rate, e_impact_ion, ch_exchange_hii,\
+            ch_exchange_hi = _fun(r, f_oii_r, rates=True)
+        reaction_rates = {'photoionization': ionization_rate,
+                          'recombination': recombination_rate,
+                          'e_impact_ionization': e_impact_ion,
+                          'charge_exchange_HII': ch_exchange_hii,
+                          'charge_exchange_HI': ch_exchange_hi}
+        return f_oii_r, reaction_rates
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `p_winds-1.4.1b0/p_winds/energetics.py` & `p_winds-1.4.4b0/p_winds/energetics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,135 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """
 This module is used to compute the wind energetics using the method
 outlined in Vissapragada et al. (2022).
 """
 
+from __future__ import (division, print_function, absolute_import,
+                        unicode_literals)
 import numpy as np
 import astropy.units as u
 import astropy.constants as c
-from scipy.integrate import simpson, cumulative_trapezoid
+from scipy.integrate import simps, cumtrapz
 from scipy.interpolate import interp1d
 
-__all__ = ["calculate_epsilon_max", "calculate_mdot_max", "spec_av_cross",
-    "compute_column_densities", "compute_transmission_coefficient",
-    "calculate_roche_radius", "calculate_f_xuv", "h_photo_cross",
-    "heplus_photo_cross", "helium_photo_cross"]
 
-threshes = {'hydrogen': 13.6*u.eV, 'helium': 24.58*u.eV, 
-    'helium+': 54.4*u.eV}
+__all__ = ["calculate_mdot_max", "calculate_epsilon_max", "spec_av_cross",
+           "compute_column_densities", "compute_transmission_coefficient",
+           "calculate_roche_radius", "calculate_f_xuv", "h_photo_cross",
+           "heplus_photo_cross", "helium_photo_cross"]
+
+threshes = {'hydrogen': 13.6 * u.eV, 'helium': 24.58 * u.eV,
+            'helium+': 54.4 * u.eV}
+
 
 def calculate_mdot_max(R_pl, M_pl, M_star, a, r_grid, spectrum, n_h, n_he, 
-    n_he_plus):
+                       n_he_plus):
     """
     Calculates the maximum mass-loss rate of an outflow given the profiles of
     neutral hydrogen, neutral helium, and ionized helium by Equation (20) of
     Vissapragada et al. (2022).
 
     Parameters
     ----------
-    R_pl (``astropy.Quantity``):
+    R_pl : ``astropy.Quantity``
         The planetary radius. An astropy unit (like u.Rjup) must be specified.
 
-    M_pl (``astropy.Quantity``):
+    M_pl : ``astropy.Quantity``
         The planetary mass. An astropy unit (like u.Mjup) must be specified.
 
-    M_star (``astropy.Quantity``):
+    M_star : ``astropy.Quantity``
         The stellar mass. An astropy unit (like u.Msun) must be specified.
 
-    a (``astropy.Quantity``):
+    a : ``astropy.Quantity``
         The semimajor axis of the planetary orbit. An astropy unit (like u.au)
         must be specified.
 
-    r_grid (``numpy.ndarray``):
+    r_grid : ``numpy.ndarray``
         The radius grid for the calculation. An astropy unit (like u.Rjup) must
         be specified for each value on the grid.
   
-    spectrum (``dict``):
+    spectrum : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes up to
         the wavelength corresponding to the energy to ionize hydrogen (13.6 eV,
         or 911.65 Angstrom). Can be generated using ``tools.make_spectrum_dict``
         or ``tools.generate_muscles_spectrum``. Currently we assume that the
         spectrum does not include lower energies than 13.6 eV.
 
-    n_h (``numpy.ndarray``):
+    n_h : ``numpy.ndarray``
         The neutral hydrogen number density profile for the wind. An astropy
         unit (like u.cm**-3) must be specified for each value on the grid.
  
-    n_he (``numpy.ndarray``):
+    n_he : ``numpy.ndarray``
         The neutral helium number density profile for the wind. An astropy
         unit (like u.cm**-3) must be specified for each value on the grid.
 
-    n_he_plus (``numpy.ndarray``):
+    n_he_plus : ``numpy.ndarray``
         The (singly-)ionized helium number density profile for the wind. An
         astropy unit (like u.cm**-3) must be specified for each value on the
         grid.
 
     Returns
     -------
-    md (``astropy.Quantity``):
+    md : ``astropy.Quantity``
         Maximum mass-loss rate (in g/s) of the wind assuming it is driven only
         by photoionization.
     """
     R_roche = calculate_roche_radius(R_pl, M_pl, M_star, a)
     eps = calculate_epsilon_max(r_grid, spectrum, n_h, n_he, n_he_plus, 
         R_pl, R_roche)
-    K = 1 - 1.5*(R_pl/R_roche) + 0.5*(R_pl/R_roche)**3
+    K = 1 - 1.5 * (R_pl / R_roche) + 0.5 * (R_pl / R_roche) ** 3
     F_XUV = calculate_f_xuv(spectrum)
-    md = 4*eps*np.pi*R_pl.to(u.cm)**3*F_XUV/(K*c.G*M_pl.to(u.g))
+    md = 4 * eps * np.pi * R_pl.to(u.cm) ** 3 * F_XUV / (K * c.G * M_pl.to(u.g))
     return md.to(u.g/u.s)
 
-def calculate_epsilon_max(r_grid, spectrum, n_h, n_he, n_he_plus,
-    R_pl, R_roche):
+
+def calculate_epsilon_max(r_grid, spectrum, n_h, n_he, n_he_plus, R_pl,
+                          R_roche):
     """
     Calculates the maximum mass-loss efficiency of an outflow given the
     profiles of neutral hydrogen, neutral helium, and ionized helium by
     Equation (19) of Vissapragada et al. (2022).
 
     Parameters
     ----------
-    r_grid (``numpy.ndarray``):
+    r_grid : ``numpy.ndarray``
         The radius grid for the calculation. An astropy unit (like u.Rjup) must
         be specified for each value on the grid.
   
-    spectrum (``dict``):
+    spectrum : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes up to
         the wavelength corresponding to the energy to ionize hydrogen (13.6 eV,
         or 911.65 Angstrom). Can be generated using ``tools.make_spectrum_dict``
         or ``tools.generate_muscles_spectrum``. Currently we assume that the
         spectrum does not include lower energies than 13.6 eV.
 
-    n_h (``numpy.ndarray``):
+    n_h : ``numpy.ndarray``
         The neutral hydrogen number density profile for the wind. An astropy
         unit (like u.cm**-3) must be specified for each value on the grid.
  
-    n_he (``numpy.ndarray``):
+    n_he : ``numpy.ndarray``
         The neutral helium number density profile for the wind. An astropy
         unit (like u.cm**-3) must be specified for each value on the grid.
 
-    n_he_plus (``numpy.ndarray``):
+    n_he_plus : ``numpy.ndarray``
         The (singly-)ionized helium number density profile for the wind. An
         astropy unit (like u.cm**-3) must be specified for each value on the
         grid.
 
-    R_pl (``astropy.Quantity``):
+    R_pl : ``astropy.Quantity``
         The planetary radius. An astropy unit (like u.Rjup) must be specified.
 
-    R_roche (``astropy.Quantity``):
+    R_roche : ``astropy.Quantity``
         The Roche radius. An astropy unit (like u.Rjup) must be specified.
 
     Returns
     -------
-    eps (``float``):
+    eps : ``float``
         Maximum mass-loss efficiency of the wind assuming it is driven only
         by photoionization.
     """
     N_h, N_he, N_he_plus = compute_column_densities(r_grid, n_h, n_he, 
         n_he_plus)
     t_coef = compute_transmission_coefficient(spectrum, r_grid,
         N_h, N_he, N_he_plus)
@@ -135,348 +140,359 @@
 
     h_heating_coef = h_av_cross * n_h
     he_heating_coef = he_av_cross * n_he
     he_plus_heating_coef = he_plus_av_cross * n_he_plus
     total_heating_coef = h_heating_coef + he_heating_coef + he_plus_heating_coef
     
     r = r_grid.to(u.cm)
-    integrand = total_heating_coef * r**2
+    integrand = total_heating_coef * r ** 2
     mask = (r >= R_pl) & (r <= R_roche)
-    eps = simpson(integrand[mask], x = r[mask])*u.cm**2/(R_pl.to(u.cm)**2)
+    eps = simps(integrand[mask], x=r[mask]) * u.cm ** 2 / (R_pl.to(u.cm) ** 2)
     return eps
 
+
 def spec_av_cross(r_grid, spectrum, t_coef, species):
     """
     Calculates the heating cross-section for photoionization using Equation (16)
     of Vissapragada et al. (2022).
 
     Parameters
     ----------
-    r_grid (``numpy.ndarray``):
+    r_grid : ``numpy.ndarray``
         The radius grid for the calculation. An astropy unit (like u.Rjup) must
         be specified for each value on the grid.
   
-    spectrum (``dict``):
+    spectrum : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes up to
         the wavelength corresponding to the energy to ionize hydrogen (13.6 eV,
         or 911.65 Angstrom). Can be generated using ``tools.make_spectrum_dict``
         or ``tools.generate_muscles_spectrum``. Currently we assume that the
         spectrum does not include lower energies than 13.6 eV.
 
-    t_coef (``numpy.ndarray``):
+    t_coef : ``numpy.ndarray``
         The transmission coefficient profile for the wind as a function of 
         frequency and altitude. In the optically-thin part of the outflow this
         should be very close to 1.
  
-    species (``str``):
+    species : ``str``
         The photoionzation target for which we are calculating the heating
         cross-section. Must be one of 'hydrogen', 'helium', or 'helium+'.
+
     Returns
     -------
-    cross (``astropy.Quantity``):
-        Heating cross-section in cm**2 for the selected species.
+    cross : ``astropy.Quantity``
+        Heating cross-section in cm ** 2 for the selected species.
     """
-    wav_grid = spectrum['wavelength']*spectrum['wavelength_unit']
-    flux_grid = spectrum['flux_lambda']*spectrum['flux_unit']
-    flux_grid = flux_grid.to(u.erg/u.s/u.cm/u.cm/u.Hz, 
-        equivalencies=u.spectral_density(wav_grid))
-    wavs_hz = wav_grid.to(u.Hz, equivalencies = u.spectral())[::-1]
+    wav_grid = spectrum['wavelength'] * spectrum['wavelength_unit']
+    flux_grid = spectrum['flux_lambda'] * spectrum['flux_unit']
+    flux_grid = flux_grid.to(u.erg / u.s / u.cm / u.cm / u.Hz,
+                             equivalencies=u.spectral_density(wav_grid))
+    wavs_hz = wav_grid.to(u.Hz, equivalencies=u.spectral())[::-1]
     flux_grid = flux_grid[::-1]
     xx, yy = np.meshgrid(wavs_hz, r_grid)
     
     threshold = threshes[species]
     crosses = {'hydrogen': h_photo_cross, 'helium': helium_photo_cross,
-        'helium+': heplus_photo_cross}
+               'helium+': heplus_photo_cross}
     cross = crosses[species]
-    evgrid = xx.to(u.eV, equivalencies = u.spectral())
+    evgrid = xx.to(u.eV, equivalencies=u.spectral())
     eta_grid = 1 - threshold/evgrid
     spec_grid, __ = np.meshgrid(flux_grid, r_grid)
     crossgrid = cross(xx)
-    crossgrid[xx.to(u.eV, equivalencies = u.spectral()) < \
-        threshold] = 0.*u.cm**2
+    crossgrid[xx.to(u.eV, equivalencies=u.spectral()) < threshold] = \
+        0. * u.cm ** 2
 
-    numgrid = eta_grid*spec_grid*crossgrid*t_coef
-    numgrid = numgrid.to(u.erg/u.s/u.Hz)    
-    num = simpson(numgrid, x = wavs_hz, axis = -1)*u.erg/u.s
+    numgrid = eta_grid * spec_grid * crossgrid * t_coef
+    numgrid = numgrid.to(u.erg / u.s / u.Hz)
+    num = simps(numgrid, x=wavs_hz, axis=-1) * u.erg/u.s
 
     F_XUV = calculate_f_xuv(spectrum)
-    cross = num/F_XUV
+    cross = num / F_XUV
     return cross.to(u.cm**2)
 
+
 def compute_column_densities(r_grid, n_h, n_he, n_he_plus):
     """
     Given the density profiles of H, He, and He+, this function calculates the
     column densities.
 
     Parameters
     ----------
-    r_grid (``numpy.ndarray``):
+    r_grid : ``numpy.ndarray``
         The radius grid for the calculation. An astropy unit (like u.Rjup) must
         be specified for each value on the grid.
 
-    n_h (``numpy.ndarray``):
+    n_h : ``numpy.ndarray``
         The neutral hydrogen number density profile for the wind. An astropy
-        unit (like u.cm**-3) must be specified for each value on the grid.
+        unit (like u.cm ** -3) must be specified for each value on the grid.
  
-    n_he (``numpy.ndarray``):
+    n_he : ``numpy.ndarray``
         The neutral helium number density profile for the wind. An astropy
-        unit (like u.cm**-3) must be specified for each value on the grid.
+        unit (like u.cm ** -3) must be specified for each value on the grid.
 
-    n_he_plus (``numpy.ndarray``):
+    n_he_plus : ``numpy.ndarray``
         The (singly-)ionized helium number density profile for the wind. An
-        astropy unit (like u.cm**-3) must be specified for each value on the
+        astropy unit (like u.cm ** -3) must be specified for each value on the
         grid.
+
     Returns
     -------
-    column_h (``numpy.ndarray``):
-        The neutral hydrogen column density profile in u.cm**-2.
+    column_h : ``numpy.ndarray``
+        The neutral hydrogen column density profile in u.cm ** -2.
 
-    column_he (``numpy.ndarray``):
-        The neutral helium column density profile in u.cm**-2.
+    column_he : ``numpy.ndarray``
+        The neutral helium column density profile in u.cm ** -2.
 
-    column_he_plus (``numpy.ndarray``):
-        The ionized helium column density profile in u.cm**-2.
+    column_he_plus : ``numpy.ndarray``
+        The ionized helium column density profile in u.cm ** -2.
     """
-    #flip grid to integrate from infty to r
+    # Flip grid to integrate from infty to r
     r_grid_temp = r_grid.to(u.cm).value[::-1]
     n_h_temp = n_h[::-1]
     n_he_temp = n_he[::-1]
     n_he_plus_temp = n_he_plus[::-1]
     
-    column_h = cumulative_trapezoid(n_h_temp, r_grid_temp,initial=0)*u.cm**-2
-    column_he = cumulative_trapezoid(n_he_temp, r_grid_temp,initial=0)*u.cm**-2
-    column_he_plus = cumulative_trapezoid(n_he_plus_temp,
-        r_grid_temp,initial=0)*u.cm**-2
+    column_h = cumtrapz(n_h_temp, r_grid_temp, initial=0) * u.cm ** -2
+    column_he = cumtrapz(n_he_temp, r_grid_temp, initial=0) * u.cm ** -2
+    column_he_plus = cumtrapz(n_he_plus_temp, r_grid_temp,
+                              initial=0) * u.cm ** -2
     
-    #flip back
+    # Flip back
     column_h = -column_h[::-1]
     column_he = -column_he[::-1]
     column_he_plus = -column_he_plus[::-1]
 
     return column_h, column_he, column_he_plus
 
+
 def compute_transmission_coefficient(spectrum, r_grid, N_h, N_he, N_he_plus):
     """
     Given the column density profiles of H, He, and He+, this function 
     calculates the transmission coefficient (negative exponential of the optical
     depth) as a function of altitude and frequency. 
 
     Parameters
     ----------
-    r_grid (``numpy.ndarray``):
+    r_grid : ``numpy.ndarray``
         The radius grid for the calculation. An astropy unit (like u.Rjup) must
         be specified for each value on the grid.
 
-    spectrum (``dict``):
+    spectrum : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes up to
         the wavelength corresponding to the energy to ionize hydrogen (13.6 eV,
         or 911.65 Angstrom). Can be generated using ``tools.make_spectrum_dict``
         or ``tools.generate_muscles_spectrum``. Currently we assume that the
         spectrum does not include lower energies than 13.6 eV.
 
-    N_h (``numpy.ndarray``):
+    N_h : ``numpy.ndarray``
         The neutral hydrogen column density profile. An astropy unit (like
-        u.cm**-2) must be specified for each value on the grid.
+        u.cm ** -2) must be specified for each value on the grid.
 
-    N_he (``numpy.ndarray``):
+    N_he : ``numpy.ndarray``
         The neutral helium column density profile. An astropy unit (like
-        u.cm**-2) must be specified for each value on the grid.
+        u.cm ** -2) must be specified for each value on the grid.
 
-    N_he_plus (``numpy.ndarray``):
+    N_he_plus : ``numpy.ndarray``
         The ionized helium column density profile. An astropy unit (like
-        u.cm**-2) must be specified for each value on the grid.
+        u.cm ** -2) must be specified for each value on the grid.
+
     Returns
     -------
-    t_coef (``numpy.ndarray``):
+    t_coef : ``numpy.ndarray``
         The transmission coefficient profile for the wind as a function of 
         frequency and altitude.
     """
-    wavs = spectrum['wavelength']*spectrum['wavelength_unit']
-    wavs_hz = wavs.to(u.Hz, equivalencies = u.spectral())[::-1]
+    wavs = spectrum['wavelength'] * spectrum['wavelength_unit']
+    wavs_hz = wavs.to(u.Hz, equivalencies=u.spectral())[::-1]
 
-    cd_h = interp1d(r_grid.to(u.cm).value, N_h.to(u.cm**-2).value,
-        kind = 'cubic')
-    cd_he = interp1d(r_grid.to(u.cm).value, N_he.to(u.cm**-2).value,
-        kind = 'cubic')
-    cd_he_plus = interp1d(r_grid.to(u.cm).value, N_he_plus.to(u.cm**-2).value, 
-        kind = 'cubic')
+    cd_h = interp1d(r_grid.to(u.cm).value, N_h.to(u.cm ** -2).value,
+                    kind='cubic')
+    cd_he = interp1d(r_grid.to(u.cm).value, N_he.to(u.cm ** -2).value,
+                     kind='cubic')
+    cd_he_plus = interp1d(r_grid.to(u.cm).value, N_he_plus.to(u.cm**-2).value,
+                          kind='cubic')
 
     xx, yy = np.meshgrid(wavs_hz, r_grid)    
     h_cross = h_photo_cross(xx)
     he_cross = helium_photo_cross(xx) 
     he_plus_cross = heplus_photo_cross(xx)
 
-    h_cross[xx.to(u.eV, equivalencies = u.spectral()) < \
-        threshes['hydrogen']] = 0.*u.cm**2
-    he_cross[xx.to(u.eV, equivalencies = u.spectral()) < \
-        threshes['helium']] = 0.*u.cm**2
-    he_plus_cross[xx.to(u.eV, equivalencies = u.spectral()) < \
-        threshes['helium+']] = 0.*u.cm**2
-
-    h_column = cd_h(yy.to(u.cm).value)*u.cm**-2
-    he_column = cd_he(yy.to(u.cm).value)*u.cm**-2
-    he_plus_column = cd_he_plus(yy.to(u.cm).value)*u.cm**-2
+    h_cross[xx.to(u.eV, equivalencies=u.spectral()) < threshes['hydrogen']] = \
+        0. * u.cm ** 2
+    he_cross[xx.to(u.eV, equivalencies=u.spectral()) < threshes['helium']] = \
+        0. * u.cm ** 2
+    he_plus_cross[xx.to(u.eV, equivalencies=u.spectral()) <
+                  threshes['helium+']] = 0. * u.cm ** 2
+
+    h_column = cd_h(yy.to(u.cm).value) * u.cm ** -2
+    he_column = cd_he(yy.to(u.cm).value) * u.cm ** -2
+    he_plus_column = cd_he_plus(yy.to(u.cm).value) * u.cm ** -2
 
     tau_h = h_cross * h_column
     tau_he = he_cross * he_column
-    tau_he_plus = he_plus_cross * he_column
+    tau_he_plus = he_plus_cross * he_plus_column
 
     tau_tot = tau_h + tau_he + tau_he_plus
     transmission_coef = np.exp(-tau_tot)
     
     return transmission_coef
 
+
 def calculate_roche_radius(R_pl, M_pl, M_star, a):
     """
     Calculates the Roche radius for the planet.
 
     Parameters
     ----------
-    R_pl (``astropy.Quantity``):
+    R_pl : ``astropy.Quantity``
         The planetary radius. An astropy unit (like u.Rjup) must be specified.
 
-    M_pl (``astropy.Quantity``):
+    M_pl : ``astropy.Quantity``
         The planetary mass. An astropy unit (like u.Mjup) must be specified.
 
-    M_star (``astropy.Quantity``):
+    M_star : ``astropy.Quantity``
         The stellar mass. An astropy unit (like u.Msun) must be specified.
 
-    a (``astropy.Quantity``):
+    a : ``astropy.Quantity``
         The semimajor axis of the planetary orbit. An astropy unit (like u.au)
         must be specified.
  
     Returns
     -------
-    R_roche (``astropy.Quantity``):
+    R_roche : ``astropy.Quantity``
         The Roche radius.
     """
-    return (a*(M_pl/(3*M_star))**(1/3)).to(u.Rjup)
+    return (a * (M_pl / (3 * M_star)) ** (1 / 3)).to(u.Rjup)
+
 
 def calculate_f_xuv(spectrum):
     """
     Calculates the total XUV flux given the spectrum at the planet (Equation
     14 of Vissapragada et al. 2022, where the minimum threshold is 13.6 eV. This
     function currently assumes the spectrum is truncated at 13.6 eV and does not
     include lower energies. 
 
     Parameters
     ----------
-    spectrum (``dict``):
+    spectrum : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes up to
         the wavelength corresponding to the energy to ionize hydrogen (13.6 eV,
         or 911.65 Angstrom). Can be generated using ``tools.make_spectrum_dict``
         or ``tools.generate_muscles_spectrum``. Currently we assume that the
         spectrum does not include lower energies than 13.6 eV.
+
     Returns
     -------
-    f_xuv (``astropy.Quantity``):
+    f_xuv : ``astropy.Quantity``
         The integrated XUV flux.
     """
-    wav_grid = spectrum['wavelength']*spectrum['wavelength_unit']
-    flux_grid = spectrum['flux_lambda']*spectrum['flux_unit']
-    flux_grid = flux_grid.to(u.erg/u.s/u.cm/u.cm/u.Hz, 
-        equivalencies=u.spectral_density(wav_grid))
-    wavs_hz = wav_grid.to(u.Hz, equivalencies = u.spectral())[::-1]
+    wav_grid = spectrum['wavelength'] * spectrum['wavelength_unit']
+    flux_grid = spectrum['flux_lambda'] * spectrum['flux_unit']
+    flux_grid = flux_grid.to(u.erg / u.s / u.cm / u.cm / u.Hz,
+                             equivalencies=u.spectral_density(wav_grid))
+    wavs_hz = wav_grid.to(u.Hz, equivalencies=u.spectral())[::-1]
     flux_grid = flux_grid[::-1]
-    f_xuv = simpson(flux_grid, x = wavs_hz)*u.erg/u.s/u.cm**2
+    f_xuv = simps(flux_grid, x=wavs_hz) * u.erg / u.s / u.cm ** 2
     return f_xuv
 
+
 def h_photo_cross(nu_init):
     """
     Calculates the photoionization cross-section of hydrogen (Equation 17 from
     Vissapragada et al. 2022). Note: potential overlap with 
     ``microphysics.hydrogen_cross_section``.
 
     Parameters
     ----------
-    nu_init (``numpy.ndarray``):
+    nu_init : ``numpy.ndarray``
         Frequencies at which to compute the cross-section. An astropy unit
         (like u.Hz) must be specified for each value in the array.
 
     Returns
     -------
-    out (``numpy.ndarray``):
-        The cross-section in cm**2. 
+    out : ``numpy.ndarray``
+        The cross-section in cm ** 2.
     """
     "nu in Hz -> cross section in units cm^2"
     threshold_energy = threshes['hydrogen']
     threshold_cross = 6.3e-18 * u.cm * u.cm
     
-    nu = nu_init.to(u.eV, equivalencies = u.spectral())
+    nu = nu_init.to(u.eV, equivalencies=u.spectral())
     
-    eps = np.sqrt(nu/threshold_energy - 1)
-    arg1 = threshold_cross*np.exp(4 - 4*np.arctan(eps)/eps/u.rad)
-    arg2 = (1 - np.exp(-2*np.pi/eps))
-    arg3 = (threshold_energy/nu)**4
+    eps = np.sqrt(nu / threshold_energy - 1)
+    arg1 = threshold_cross*np.exp(4 - 4 * np.arctan(eps) / eps / u.rad)
+    arg2 = (1 - np.exp(-2 * np.pi / eps))
+    arg3 = (threshold_energy / nu) **4
     
-    out =  arg1 / arg2 * arg3
+    out = arg1 / arg2 * arg3
     return out
 
+
 def heplus_photo_cross(nu_init):
     """
     Calculates the photoionization cross-section of ionized helium (Equation 17
     from Vissapragada et al. 2022).
 
     Parameters
     ----------
-    nu_init (``numpy.ndarray``):
+    nu_init : ``numpy.ndarray``
         Frequencies at which to compute the cross-section. An astropy unit
         (like u.Hz) must be specified for each value in the array.
 
     Returns
     -------
-    out (``numpy.ndarray``):
+    out : ``numpy.ndarray``
         The cross-section in cm**2. 
     """
     "nu in Hz -> cross section in units cm^2"
     threshold_energy = threshes['helium+']
-    threshold_cross = 6.3e-18/4 * u.cm * u.cm
+    threshold_cross = 6.3e-18 / 4 * u.cm * u.cm
     
-    nu = nu_init.to(u.eV, equivalencies = u.spectral())
+    nu = nu_init.to(u.eV, equivalencies=u.spectral())
     
     eps = np.sqrt(nu/threshold_energy - 1)
-    arg1 = threshold_cross*np.exp(4 - 4*np.arctan(eps)/eps/u.rad)
-    arg2 = (1 - np.exp(-2*np.pi/eps))
-    arg3 = (threshold_energy/nu)**4
+    arg1 = threshold_cross * np.exp(4 - 4 * np.arctan(eps) / eps / u.rad)
+    arg2 = (1 - np.exp(-2 * np.pi / eps))
+    arg3 = (threshold_energy / nu) **4
     
-    out =  arg1 / arg2 * arg3
+    out = arg1 / arg2 * arg3
     return out
 
+
 def helium_photo_cross(nu_init):
     """
     Calculates the photoionization cross-section of neutral helium. This is 
     Equation 18 from Vissapragada et al. 2022, which itself is from Yan, 
     Sadeghpour, & Dalgarno (1998, ApJ). Note that this does not overlap with
     the state-resolved cross-sections from the ``microphysics`` module as this
     is a total photoionization cross-section across all states. 
 
     Parameters
     ----------
-    nu_init (``numpy.ndarray``):
+    nu_init : ``numpy.ndarray``
         Frequencies at which to compute the cross-section. An astropy unit
         (like u.Hz) must be specified for each value in the array.
 
     Returns
     -------
-    out (``numpy.ndarray``):
+    out : ``numpy.ndarray``
         The cross-section in cm**2. 
     """
-    "nu in Hz -> cross section in units cm^2"
-    "Source: Yan, Sadeghpour, & Dalgarno (1998, ApJ)"
+    # nu in Hz -> cross section in units cm^2
+    # Source: Yan, Sadeghpour, & Dalgarno (1998, ApJ)
     threshold_energy = threshes['helium']
     
-    nu = nu_init.to(u.eV, equivalencies = u.spectral())
+    nu = nu_init.to(u.eV, equivalencies=u.spectral())
     
     nu_masked = nu
     x = nu_masked / threshold_energy
-    e_term = (nu_masked / u.eV / 1000.)**(7/2)
+    e_term = (nu_masked / u.eV / 1000.)**(7 / 2)
     
     coefs = [-4.7416, 14.8200, -30.8678, 37.3584, -23.4585, 5.9133]
     sum_term = 0.
     for i, coef in enumerate(coefs):
-        sum_term += coef / x**((i+1)/2)
+        sum_term += coef / x ** ((i + 1) / 2)
     
     num = 733 * u.barn
     out = num.to(u.cm * u.cm)/e_term * (1 + sum_term)
 
     return out
-
```

### Comparing `p_winds-1.4.1b0/p_winds/helium.py` & `p_winds-1.4.4b0/p_winds/helium.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from __future__ import (division, print_function, absolute_import,
                         unicode_literals)
 import numpy as np
 import astropy.units as u
 import astropy.constants as c
 from scipy.integrate import simps, solve_ivp, odeint
-from scipy.interpolate import interp1d
 from p_winds import tools, microphysics
 import warnings
 
 
 __all__ = ["radiative_processes", "radiative_processes_mono", "recombination",
            "recombination_all", "collision", "charge_transfer",
            "population_fraction", "ion_fraction"]
@@ -25,59 +24,59 @@
 def radiative_processes(spectrum_at_planet, combined_ionization=False):
     """
     Calculate the photoionization rate of helium at null optical depth based
     on the EUV spectrum arriving at the planet.
 
     Parameters
     ----------
-    spectrum_at_planet (``dict``):
+    spectrum_at_planet : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes at
         least up to the wavelength corresponding to the energy to ionize
         helium (4.8 eV, or 2593 Angstrom).
 
     Returns
     -------
-    phi_1 (``float``):
+    phi_1 : ``float``
         Ionization rate of helium singlet at null optical depth in unit of
         1 / s. This is returned if ``combined_ionization`` is set to ``False``.
 
-    phi_3 (``float``):
+    phi_3 : ``float``
         Ionization rate of helium triplet at null optical depth in unit of
         1 / s. This is returned if ``combined_ionization`` is set to ``False``.
 
-    a_1 (``float``):
+    a_1 : ``float``
         Flux-averaged photoionization cross-section of helium singlet in unit of
         cm ** 2. This is returned if ``combined_ionization`` is set to
         ``False``.
 
-    a_3 (``float``):
+    a_3 : ``float``
         Flux-averaged photoionization cross-section of helium triplet in unit of
         cm ** 2. This is returned if ``combined_ionization`` is set to
         ``False``.
 
-    a_h_1 (``float``):
+    a_h_1 : ``float``
         Flux-averaged photoionization cross-section of hydrogen in the range
         absorbed by helium singlet in unit of cm ** 2. This is returned if
         ``combined_ionization`` is set to ``False``.
 
-    a_h_3 (``float``):
+    a_h_3 : ``float``
         Flux-averaged photoionization cross-section of hydrogen in the range
         absorbed by helium triplet in unit of cm ** 2. This is returned if
         ``combined_ionization`` is set to ``False``.
 
-    phi (``float``):
+    phi : ``float``
         Ionization rate of helium at null optical depth in unit of 1 / s. This
         is returned if ``combined_ionization`` is set to ``True``.
 
-    a_he (``float``):
+    a_he : ``float``
         Flux-averaged photoionization cross-section of helium in unit of
         cm ** 2. This is returned if ``combined_ionization`` is set to
         ``True``.
 
-    a_h (``float``):
+    a_h : ``float``
         Flux-averaged photoionization cross-section of hydrogen in the range
         absorbed by helium atoms in unit of cm ** 2. This is returned if
         ``combined_ionization`` is set to ``True``.
     """
     wavelength = (spectrum_at_planet['wavelength'] *
                   spectrum_at_planet['wavelength_unit']).to(u.angstrom).value
     flux_lambda = (spectrum_at_planet['flux_lambda'] * spectrum_at_planet[
@@ -179,59 +178,59 @@
                              average_fuv_photon_wavelength=2348.0):
     """
     Calculate the photoionization rate of helium at null optical depth based
     on the EUV spectrum arriving at the planet.
 
     Parameters
     ----------
-    flux_euv (``float``):
+    flux_euv : ``float``
         Monochromatic extreme-ultraviolet (0 - 504 Angstrom) flux arriving at
         the planet in units of erg / s / cm ** 2. Attention: notice that this
         ``flux_euv`` is different from the one used for hydrogen, since helium
         ionization happens at a shorter wavelength.
 
-    flux_fuv (``float``):
+    flux_fuv : ``float``
         Monochromatic far- to middle-ultraviolet (911 - 2593 Angstrom) flux
         arriving at the planet in units of erg / s / cm ** 2.
 
-    average_euv_photon_wavelength (``float``):
+    average_euv_photon_wavelength : ``float``
         Average wavelength of EUV photons ionizing the He singlet state, in unit
         of Angstrom. Default value is 242 Angstrom. The default value is based
         on a flux-weighted average of the solar spectrum between 0 and 504
         Angstrom.
 
-    average_fuv_photon_wavelength (``float``):
+    average_fuv_photon_wavelength : ``float``
         Average wavelength of FUV-NUV photons ionizing the He triplet state, in
         unit of Angstrom. Default value is 2348 Angstrom. The default value is
         based on a flux-weighted average of the solar spectrum between 911 and
         2593 Angstrom.
 
     Returns
     -------
-    phi_1 (``float``):
+    phi_1 : ``float``
         Ionization rate of helium singlet at null optical depth in unit of
         1 / s.
 
-    phi_3 (``float``):
+    phi_3 : ``float``
         Ionization rate of helium triplet at null optical depth in unit of
         1 / s.
 
-    a_1 (``float``):
+    a_1 : ``float``
         Flux-averaged photoionization cross-section of helium singlet in unit of
         cm ** 2.
 
-    a_3 (``float``):
+    a_3 : ``float``
         Flux-averaged photoionization cross-section of helium triplet in unit of
         cm ** 2.
 
-    a_h_1 (``float``):
+    a_h_1 : ``float``
         Flux-averaged photoionization cross-section of hydrogen in the range
         absorbed by helium singlet in unit of cm ** 2.
 
-    a_h_3 (``float``):
+    a_h_3 : ``float``
         Flux-averaged photoionization cross-section of hydrogen in the range
         absorbed by helium triplet in unit of cm ** 2.
     """
     # Average cross-section to ionize helium singlet
     a_1 = microphysics.helium_singlet_cross_section(average_euv_photon_wavelength)
 
     # The photoionization cross-section of He triplet
@@ -265,23 +264,23 @@
 def recombination(temperature):
     """
     Calculates the helium singlet and triplet recombination rates for a gas at
     a certain temperature.
 
     Parameters
     ----------
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
     Returns
     -------
-    alpha_rec_1 (``float``):
+    alpha_rec_1 : ``float``
         Recombination rate of helium singlet in units of cm ** 3 / s.
 
-    alpha_rec_3 (``float``):
+    alpha_rec_3 : ``float``
         Recombination rate of helium triplet in units of cm ** 3 / s.
     """
     # The recombination rates come from Benjamin et al. (1999,
     # ADS:1999ApJ...514..307B)
     alpha_rec_1 = 1.54E-13 * (temperature / 1E4) ** (-0.486)
     alpha_rec_3 = 2.10E-13 * (temperature / 1E4) ** (-0.778)
     return alpha_rec_1, alpha_rec_3
@@ -291,20 +290,20 @@
 def recombination_all(temperature):
     """
     Calculates the helium recombination rates for a gas at a certain
     temperature, with no distinction between singlet and triplet states.
 
     Parameters
     ----------
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
     Returns
     -------
-    alpha_rec (``float``):
+    alpha_rec : ``float``
         Recombination rate of helium in units of cm ** 3 / s.
     """
     # The recombination rates come from Storey & Hummer 1995
     alpha_rec = 4.6E-12 * (temperature / 300) ** (-0.64)
     return alpha_rec
 
 
@@ -312,36 +311,36 @@
 def collision(temperature):
     """
     Calculates the helium singlet and triplet collisional population rates for
     a gas at a certain temperature.
 
     Parameters
     ----------
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
     Returns
     -------
-    q_13 (``float``):
+    q_13 : ``float``
         Rate of helium transition from singlet (1^1S) to triplet (2^3S) due to
         collisions with free electrons in units of cm ** 3 / s.
 
-    q_31a (``float``):
+    q_31a : ``float``
         Rate of helium transition from triplet (2^3S) to 2^1S due to collisions
         with free electrons in units of cm ** 3 / s.
 
-    q_31b (``float``):
+    q_31b : ``float``
         Rate of helium transition from triplet (2^3S) to 2^1P due to collisions
         with free electrons in units of cm ** 3 / s.
 
-    big_q_he (``float``):
+    big_q_he : ``float``
         Rate of charge exchange between helium singlet and ionized hydrogen in
         units of cm ** 3 / s.
 
-    big_q_he_plus (``float``):
+    big_q_he_plus : ``float``
         Rate of charge exchange between ionized helium and atomic hydrogen in
         units of cm ** 3 / s.
     """
     # The effective collision strengths are hard-coded from the values provided
     # by Bray et al. (2000, ADS:2000A&AS..146..481B), which are binned to
     # specific temperatures. Thus, we need to interpolate to the specific
     # temperature of our gas. First we parse the tabulated data
@@ -379,23 +378,23 @@
 def charge_transfer(temperature):
     """
     Calculates the charge exchange rates of He with H nuclei. Based on the
     formulation of Glover & Jappsen et al. 2007.
 
     Parameters
     ----------
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
     Returns
     -------
-    ct_rate_he_hp (``float``):
+    ct_rate_he_hp : ``float``
         Charge transfer rate between neutral He and H+ in units of cm ** 3 / s.
 
-    ct_rate_hep_h (``float``):
+    ct_rate_hep_h : ``float``
         Charge transfer rate between He+ and neutral H in units of cm ** 3 / s.
     """
     # Recombination of He II into He I
     ct_rate_hep_h = 1.25E-15 * (300 / temperature) ** (-0.25)
 
     # Ionization of He I into He II
     ct_rate_he_hp = 1.75E-11 * (300 / temperature) ** 0.75 * \
@@ -408,118 +407,141 @@
 def population_fraction(radius_profile, velocity, density,
                         hydrogen_ion_fraction, planet_radius, temperature,
                         h_fraction, speed_sonic_point, radius_sonic_point,
                         density_sonic_point, spectrum_at_planet=None,
                         flux_euv=None, flux_fuv=None,
                         initial_state=np.array([0.5, 0.5]),
                         relax_solution=False, convergence=0.01, max_n_relax=10,
-                        method='odeint', **options_solve_ivp):
+                        method='odeint', return_rates=False,
+                        **options_solve_ivp):
     """
     Calculate the fraction of helium in singlet and triplet state in the upper
     atmosphere in function of the radius in unit of planetary radius.
 
     Parameters
     ----------
-    radius_profile (``numpy.ndarray``):
+    radius_profile : ``numpy.ndarray``
         Radius in unit of planetary radii.
 
-    velocity (``numpy.ndarray``):
+    velocity : ``numpy.ndarray``
          Velocities sampled at the values of ``radius_profile`` in units of
          sound speed. Similar to the output of ``parker.structure()``.
 
-    density (``numpy.ndarray``):
+    density : ``numpy.ndarray``
         Densities sampled at the values of ``radius_profile`` in units of
         density at the sonic point. Similar to the output of
         ``parker.structure()``.
 
-    hydrogen_ion_fraction (``numpy.ndarray``):
+    hydrogen_ion_fraction : ``numpy.ndarray``
         Number fraction of H ion over total H in the upper atmosphere in
         function of radius. Similar to the output of
         ``hydrogen.ion_fraction()``.
 
-    planet_radius (``float``):
+    planet_radius : ``float``
         Planetary radius in unit of Jupiter radius.
 
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
-    h_fraction (``float``):
+    h_fraction : ``float``
         Total (ion + neutral) H number fraction of the atmosphere.
 
-    speed_sonic_point (``float``):
+    speed_sonic_point : ``float``
         Speed of sound in the outflow in units of km / s.
 
-    radius_sonic_point (``float``):
+    radius_sonic_point : ``float``
         Radius of the sonic point in unit of Jupiter radius.
 
-    density_sonic_point (``float``):
+    density_sonic_point : ``float``
         Density at the sonic point in units of g / cm ** 3.
 
-    spectrum_at_planet (``dict``, optional):
+    spectrum_at_planet : ``dict``, optional
         Spectrum of the host star arriving at the planet covering fluxes at
         least up to the wavelength corresponding to the energy to populate the
         helium states (4.8 eV, or 2593 Angstrom). Can be generated using
         ``tools.make_spectrum_dict``. If ``None``, then ``flux_euv`` and
         ``flux_fuv`` must be provided instead. Default is ``None``.
 
-    flux_euv (``float``, optional):
+    flux_euv : ``float``, optional
         Monochromatic extreme-ultraviolet (0 - 1200 Angstrom) flux arriving at
         the planet in units of erg / s / cm ** 2. If ``None``, then
         ``spectrum_at_planet`` must be provided instead. Default is ``None``.
 
-    flux_fuv (``float``, optional):
+    flux_fuv : ``float``, optional
         Monochromatic far- to middle-ultraviolet (1200 - 2600 Angstrom) flux
         arriving at the planet in units of erg / s / cm ** 2. If ``None``, then
         ``spectrum_at_planet`` must be provided instead. Default is ``None``.
 
-    initial_state (``numpy.ndarray``, optional):
+    initial_state : ``numpy.ndarray``, optional
         The initial state is the `y0` of the differential equation to be solved.
         This array has two items: the initial value of the fractions of singlet
         and triplet state in the inner layer of the atmosphere. The default
         value for this parameter is ``numpy.array([0.5, 0.5])``, i.e., fully
         neutral at the inner layer with 50% in singlet and 50% in triplet
         states.
 
-    relax_solution (``bool``, optional):
+    relax_solution : ``bool``, optional
         The first solution is calculating by initially assuming the entire
         atmosphere is in neutral state. If ``True``, the solution will be
         re-calculated in a loop until it converges to a delta_f of 1%, or for a
         maximum of 10 loops (default parameters). Default is ``False``.
 
-    convergence (``float``, optional):
+    convergence : ``float``, optional
         Value of delta_f at which to stop the relaxation of the solution for
         ``f_r``. Default is 0.01.
 
-    max_n_relax (``int``, optional):
+    max_n_relax : ``int``, optional
         Maximum number of loops to perform the relaxation of the solution for
         ``f_r``. Default is 10.
 
-    method (``str``, optional):
+    method : ``str``, optional
         If method is ``'odeint'``, then ``scipy.integrate.odeint()`` is used
         instead of ``scipy.integrate.solve_ivp()`` to calculate the steady-state
         distribution of helium. The first seems to be at least twice faster than
         the second in some situations. Any other method will fall back to an
         option of ``solve_ivp()`` methods. For example, if ``method`` is set to
         ``'Radau'``, then use ``solve_ivp(method='Radau')``. Default is
         ``'odeint'``.
 
+    return_rates : ``bool``, optional
+        If ``True``, then this function also returns a ``dict`` object
+        containing the various reaction rates in function of radius and in units
+        of 1 / s. Default is ``False``.
+
     **options_solve_ivp:
         Options to be passed to the ``scipy.integrate.solve_ivp()`` solver. You
         may want to change the options ``atol`` (absolute tolerance; default is
         1E-6) or ``rtol`` (relative tolerance; default is 1E-3). If you are
         having numerical issues, you may want to decrease the tolerance by a
         factor of 10 or 100, or 1000 in extreme cases.
 
     Returns
     -------
-    f_1_r (``numpy.ndarray``):
+    f_1_r : ``numpy.ndarray``
         Fraction of helium in singlet state in function of radius.
 
-    f_3_r (``numpy.ndarray``):
+    f_3_r : ``numpy.ndarray``
         Fraction of helium in triplet state in function of radius.
+
+    reaction_rates : ``dict``
+        Dictionary containing the reaction rates in function of radius and in
+        units of 1 / s. Only returned when ``return_rates`` is set to ``True``.
+        Here is a short description of the dict keys:
+
+        * `ionization_1`: Photoionization of He singlet atoms
+        * `ionization_3`: Photoionization of He triplet atoms
+        * `recombination_1`: Recombination of He ions into He singlet
+        * `recombination_3`: Recombination of He ions into He triplet
+        * `radiative_transition`: Radiative transition of He triplet into singlet
+        * `transition_1_to_3`: Transition of He singlet to triplet due to collisions with electrons
+        * `transition_3_to_21s`: Transition of He triplet to 2$^1$S due to collisions with electrons
+        * `transition_3_to_21p`: Transition of He triplet to 2$^1$P due to collisions with electrons
+        * `other_ionization`: Combined rate of associative ionization and Penning ionization
+        * `charge_exchange_1`: Charge exchange between helium singlet and ionized hydrogen
+        * `charge_exchange_he_ion`: Charge exchange between ionized helium and atomic hydrogen
     """
     vs = speed_sonic_point  # km / s
     rs = radius_sonic_point  # jupiterRad
     rhos = density_sonic_point  # g / cm ** 3
 
     # Recombination rates of helium singlet and triplet in unit of rs ** 2 * vs
     alpha_rec_unit = ((rs * 7.1492E+09) ** 2 * vs * 1E5)  # cm ** 3 / s
@@ -571,88 +593,95 @@
     big_a_31 = 1.272E-4 / phi_unit
 
     # Now let's solve the differential eq. 15 of Oklopcic & Hirata 2018
 
     # The radius in unit of radius at the sonic point
     r = radius_profile * planet_radius / rs
     dr = np.diff(r)
-    dr = np.concatenate((dr, np.array([r[-1], ])))
-
-    # The way we solve the differential equation requires us to pass the H ion
-    # fraction, densities and velocities at specific values of r, and it can be
-    # cumbersome to parse this inside the callable function _fun(). Instead,
-    # let's create a "mock function" that returns the value of v, rho, and
-    # f_H_ion in function of r (essentially a scipy.interp1d function)
-    mock_f_h_ion_r = interp1d(r, hydrogen_ion_fraction,
-                              fill_value="extrapolate")
-    mock_v_r = interp1d(r, velocity, fill_value="extrapolate")
-    mock_rho_r = interp1d(r, density, fill_value="extrapolate")
+    dr = np.concatenate((dr, np.array([dr[-1], ])))
 
     # With all this setup done, now we need to assume something about the
     # distribution of singlet and triplet helium in the atmosphere. Let's assume
     # it based on the initial guess input.
     column_density = np.flip(np.cumsum(np.flip(dr * density)))  # Total column
                                                                 # density
     column_density_h_0 = np.flip(  # Column density of H only
         np.cumsum(np.flip(dr * density * (1 - hydrogen_ion_fraction))))
     he_fraction = 1 - h_fraction
     k1 = h_fraction / (h_fraction + 4 * he_fraction) / m_h
     k2 = he_fraction / (h_fraction + 4 * he_fraction) / m_h
     tau_1_h = k1 * a_h_1 * column_density_h_0
     tau_3_h = k1 * a_h_3 * column_density_h_0
-    tau_1_initial = (initial_state[0] * k2 * a_1 * column_density + tau_1_h)
-    tau_3_initial = (initial_state[1] * k2 * a_3 * column_density + tau_3_h)
-    # We do a dirty hack to make tau_initial a callable function so it's easily
-    # parsed inside the differential equation solver
-    _tau_1_fun = interp1d(r, tau_1_initial, fill_value="extrapolate")
-    _tau_3_fun = interp1d(r, tau_3_initial, fill_value="extrapolate")
+    tau_1 = (initial_state[0] * k2 * a_1 * column_density + tau_1_h)
+    tau_3 = (initial_state[1] * k2 * a_3 * column_density + tau_3_h)
 
     # The differential equation
-    def _fun(_r, y):
+    def _fun(_r, y, rates=False):
         f_1 = y[0]  # Fraction of helium in singlet
         f_3 = y[1]  # Fraction of helium in triplet
 
-        _v = mock_v_r(np.array([_r, ]))[0]
-        _rho = mock_rho_r(np.array([_r, ]))[0]
-        f_h_ion = mock_f_h_ion_r(np.array([_r, ]))[0]  # Fraction of H+
+        _v = np.interp(_r, r, velocity)
+        _rho = np.interp(_r, r, density)
+        f_h_ion = np.interp(_r, r, hydrogen_ion_fraction)  # Fraction of H+
 
         # Assume the number density of electrons is equal to the number density
         # of H ions
-        n_e = k1 * _rho * f_h_ion         # Number density of electrons
-        n_h_plus = k1 * _rho * f_h_ion    # Number density of ionized H
-        n_h0 = k1 * _rho * (1 - f_h_ion)  # Number density of atomic H
+        # Since we may run into loss of numerical precision here (big numbers),
+        # we manipulate the equations to avoid this problem. It looks a bit
+        # messy, but it is necessary
+        alpha_rec_1_n_e = np.exp(
+            np.log(k1) + np.log(_rho) + np.log(alpha_rec_1)) * f_h_ion
+        alpha_rec_3_n_e = np.exp(
+            np.log(k1) + np.log(_rho) + np.log(alpha_rec_3)) * f_h_ion
+        q_13_n_e = np.exp(
+            np.log(k1) + np.log(_rho) + np.log(q_13)) * f_h_ion
+        q_31a_n_e = np.exp(
+            np.log(k1) + np.log(_rho) + np.log(q_31a)) * f_h_ion
+        q_31b_n_e = np.exp(
+            np.log(k1) + np.log(_rho) + np.log(q_31b)) * f_h_ion
+        big_q_31_n_h0 = np.exp(
+            np.log(k1) + np.log(_rho) + np.log(big_q_31)) * (1 - f_h_ion)
+        big_q_he_n_h_plus = np.exp(
+            np.log(k1) + np.log(_rho) + np.log(big_q_he)) * f_h_ion
+        big_q_he_plus_n_h0 = np.exp(
+            np.log(k1) + np.log(_rho) + np.log(big_q_he_plus)) * (1 - f_h_ion)
 
         # Terms of df1_dr
-        term_11 = (1 - f_1 - f_3) * n_e * alpha_rec_1  # Recombination
+        term_11 = (1 - f_1 - f_3) * alpha_rec_1_n_e  # Recombination
         term_12 = f_3 * big_a_31  # Radiative transition rate
-        t_1 = _tau_1_fun(np.array([_r, ]))[0]
-        t_3 = _tau_3_fun(np.array([_r, ]))[0]
+        t_1 = np.interp(_r, r, tau_1)
+        t_3 = np.interp(_r, r, tau_3)
         term_13 = f_1 * phi_1 * np.exp(-t_1)  # Photoionization
-        term_14 = f_1 * n_e * q_13  # Transition rate due to collision with e
-        term_15 = f_3 * n_e * q_31a  # Transition rate due to collision with e
-        term_16 = f_3 * n_e * q_31b  # Transition rate due to collision with e
-        term_17 = f_3 * n_h0 * big_q_31  # Combined rate of associative
+        term_14 = f_1 * q_13_n_e  # Transition rate due to collision with e
+        term_15 = f_3 * q_31a_n_e  # Transition rate due to collision with e
+        term_16 = f_3 * q_31b_n_e  # Transition rate due to collision with e
+        term_17 = f_3 * big_q_31_n_h0  # Combined rate of associative
                                          # ionization and Penning ionization
-        term_18 = f_1 * n_h_plus * big_q_he  # Charge exchange consuming He
+        term_18 = f_1 * big_q_he_n_h_plus  # Charge exchange consuming He
                                              # singlet
-        term_19 = (1 - f_1 - f_3) * n_h0 * big_q_he_plus  # Charge exchange
+        term_19 = (1 - f_1 - f_3) * big_q_he_plus_n_h0  # Charge exchange
                                                           # producing He
                                                           # singlet
 
         # Terms of df3_dr
-        term_31 = (1 - f_1 - f_3) * n_e * alpha_rec_3  # Recombination
+        term_31 = (1 - f_1 - f_3) * alpha_rec_3_n_e  # Recombination
         term_33 = f_3 * phi_3 * np.exp(-t_3)  # Photoionization
 
         # Finally assemble the equations for df3_dr and df3_dr
         df1_dr = (term_11 + term_12 - term_13 - term_14 + term_15 + term_16
                   + term_17 - term_18 + term_19) / _v
         df3_dr = (term_31 - term_12 - term_33 + term_14 - term_15 - term_16
                   - term_17) / _v
 
-        return np.array([df1_dr, df3_dr])
+        if rates is False:
+            return np.array([df1_dr, df3_dr])
+        else:
+            return np.array([term_13, term_33, term_11, term_31, term_12,
+                             term_14, term_15, term_16, term_17, term_18,
+                             term_19]) * phi_unit
 
     if method == 'odeint':
         # Since 'odeint' yields only warnings when precision is lost or when
         # there is a problem, we transform these warnings into an exception
         with warnings.catch_warnings():
             warnings.filterwarnings("error")
             try:
@@ -691,16 +720,14 @@
             previous_f_3_r = np.copy(f_3_r)
 
             # Re-calculate the column densities
             tau_1 = k2 * a_1 * np.flip(
                 np.cumsum(np.flip(dr * density * f_1_r))) + tau_1_h
             tau_3 = k2 * a_3 * np.flip(
                 np.cumsum(np.flip(dr * density * f_3_r))) + tau_3_h
-            _tau_1_fun = interp1d(r, tau_1, fill_value="extrapolate")
-            _tau_3_fun = interp1d(r, tau_3, fill_value="extrapolate")
 
             # Solve it again
             if method == 'odeint':
                 sol = odeint(_fun, y0=initial_state, t=r, tfirst=True)
                 f_1_r = np.copy(sol).T[0]
                 f_3_r = np.copy(sol).T[1]
             else:
@@ -727,15 +754,33 @@
                     relative_delta_f_3 < convergence:
                 break
             else:
                 pass
     else:
         pass
 
-    return f_1_r, f_3_r
+    if return_rates is False:
+        return f_1_r, f_3_r
+    else:
+        ion_rate_1, ion_rate_3, recomb_rate_1, recomb_rate_3, rad_trans_rate, \
+            transition_rate_q13, transition_rate_q31a, transition_rate_q31b, \
+            other_ionz_rate, ch_exchange_he1, ch_exchange_hep = \
+            _fun(r, [f_1_r, f_3_r], rates=True)
+        reaction_rates = {'ionization_1': ion_rate_1,
+                          'ionization_3': ion_rate_3,
+                          'recombination_1': recomb_rate_1,
+                          'recombination_3': recomb_rate_3,
+                          'radiative_transition': rad_trans_rate,
+                          'transition_1_to_3': transition_rate_q13,
+                          'transition_3_to_21s': transition_rate_q31a,
+                          'transition_3_to_21p': transition_rate_q31b,
+                          'other_ionization': other_ionz_rate,
+                          'charge_exchange_1': ch_exchange_he1,
+                          'charge_exchange_he_ion': ch_exchange_hep}
+        return f_1_r, f_3_r, reaction_rates
 
 
 # Calculate the ion fraction of He
 def ion_fraction(radius_profile, velocity, density, hydrogen_ion_fraction,
                  planet_radius, temperature, h_fraction, speed_sonic_point,
                  radius_sonic_point, density_sonic_point, spectrum_at_planet,
                  initial_f_he_ion=0.0, relax_solution=False, convergence=0.01,
@@ -744,74 +789,74 @@
     Sometimes we need to calculate only the fraction of ionized helium and not
     necessarily the triplet and singlet fractions. This function does that,
     which is faster than ``population_fraction()``. The result is in function of
     the radius in unit of planetary radius.
 
     Parameters
     ----------
-    radius_profile (``numpy.ndarray``):
+    radius_profile : ``numpy.ndarray``
         Radius in unit of planetary radii.
 
-    velocity (``numpy.ndarray``):
+    velocity : ``numpy.ndarray``
          Velocities sampled at the values of ``radius_profile`` in units of
          sound speed. Similar to the output of ``parker.structure()``.
 
-    density (``numpy.ndarray``):
+    density : ``numpy.ndarray``
         Densities sampled at the values of ``radius_profile`` in units of
         density at the sonic point. Similar to the output of
         ``parker.structure()``.
 
-    hydrogen_ion_fraction (``numpy.ndarray``):
+    hydrogen_ion_fraction : ``numpy.ndarray``
         Number fraction of H ion over total H in the upper atmosphere in
         function of radius. Similar to the output of
         ``hydrogen.ion_fraction()``.
 
-    planet_radius (``float``):
+    planet_radius : ``float``
         Planetary radius in unit of Jupiter radius.
 
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
-    h_fraction (``float``):
+    h_fraction : ``float``
         Total (ion + neutral) H number fraction of the atmosphere.
 
-    speed_sonic_point (``float``):
+    speed_sonic_point : ``float``
         Speed of sound in the outflow in units of km / s.
 
-    radius_sonic_point (``float``):
+    radius_sonic_point : ``float``
         Radius of the sonic point in unit of Jupiter radius.
 
-    density_sonic_point (``float``):
+    density_sonic_point : ``float``
         Density at the sonic point in units of g / cm ** 3.
 
-    spectrum_at_planet (``dict``):
+    spectrum_at_planet : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes at
         least up to the wavelength corresponding to the energy to ionize helium
         (4.8 eV, or 2593 Angstrom). Can be generated using
         ``tools.make_spectrum_dict``.
 
-    initial_f_he_ion (``numpy.ndarray``, optional):
+    initial_f_he_ion : ``numpy.ndarray``, optional
         The initial helium ion fraction at the layer near the surface of the
         planet. Default is 0.0, i.e., 100% neutral.
 
-    relax_solution (``bool``, optional):
+    relax_solution : ``bool``, optional
         The first solution is calculating by initially assuming the entire
         atmosphere is in neutral state. If ``True``, the solution will be
         re-calculated in a loop until it converges to a delta_f of 1%, or for a
         maximum of 10 loops (default parameters). Default is ``False``.
 
-    convergence (``float``, optional):
+    convergence : ``float``, optional
         Value of delta_f at which to stop the relaxation of the solution for
         ``f_r``. Default is 0.01.
 
-    max_n_relax (``int``, optional):
+    max_n_relax : ``int``, optional
         Maximum number of loops to perform the relaxation of the solution for
         ``f_r``. Default is 10.
 
-    method (``str``, optional):
+    method : ``str``, optional
         If method is ``'odeint'``, then ``scipy.integrate.odeint()`` is used
         instead of ``scipy.integrate.solve_ivp()`` to calculate the steady-state
         distribution of helium. The first seems to be at least twice faster than
         the second in some situations. Any other method will fall back to an
         option of ``solve_ivp()`` methods. For example, if ``method`` is set to
         ``'Radau'``, then use ``solve_ivp(method='Radau')``. Default is
         ``'Radau'``.
@@ -821,15 +866,15 @@
         may want to change the options ``atol`` (absolute tolerance; default is
         1E-6) or ``rtol`` (relative tolerance; default is 1E-3). If you are
         having numerical issues, you may want to decrease the tolerance by a
         factor of 10 or 100, or 1000 in extreme cases.
 
     Returns
     -------
-    f_r (``numpy.ndarray``):
+    f_r : ``numpy.ndarray``
         Fraction of ionized helium in function of radius.
     """
     vs = speed_sonic_point  # km / s
     rs = radius_sonic_point  # jupiterRad
     rhos = density_sonic_point  # g / cm ** 3
 
     # Recombination rates of C in unit of rs ** 2 * vs
@@ -857,59 +902,64 @@
     ct_rate_he_hp = ct_rate_he_hp / alpha_rec_unit
 
     # We solve the steady-state ionization balance
 
     # The radius in unit of radius at the sonic point
     r = radius_profile * planet_radius / rs
     dr = np.diff(r)
-    dr = np.concatenate((dr, np.array([r[-1], ])))
-
-    # Some mock functions that will allow us to parse the values of ion
-    # fraction, velocity and density in function of radius
-    mock_f_h_ion_r = interp1d(r, hydrogen_ion_fraction,
-                              fill_value="extrapolate")
-    mock_v_r = interp1d(r, velocity, fill_value="extrapolate")
-    mock_rho_r = interp1d(r, density, fill_value="extrapolate")
+    dr = np.concatenate((dr, np.array([dr[-1], ])))
 
     # With all this setup done, now we need to assume something about the
     # distribution of singlet and triplet helium in the atmosphere. Let's assume
     # it based on the initial guess input.
     column_density = np.flip(np.cumsum(np.flip(dr * density)))  # Total column
                                                                 # density
     column_density_h_0 = np.flip(  # Column density of H only
         np.cumsum(np.flip(dr * density * (1 - hydrogen_ion_fraction))))
     he_fraction = 1 - h_fraction
     k1 = h_fraction / (h_fraction + 4 * he_fraction) / m_h
     k2 = he_fraction / (h_fraction + 4 * he_fraction) / m_h
     tau_h = k1 * a_h * column_density_h_0
-    tau_he_initial = (initial_f_he_ion * k2 * a_he * column_density + tau_h)
-    _tau_he_fun = interp1d(r, tau_he_initial, fill_value="extrapolate")
+    tau_he = (initial_f_he_ion * k2 * a_he * column_density + tau_h)
 
     # The differential equation
     def _fun(_r, y):
         f_he_ion = y
 
-        _v = mock_v_r(np.array([_r, ]))[0]
-        _rho = mock_rho_r(np.array([_r, ]))[0]
-        f_h_ion = mock_f_h_ion_r(np.array([_r, ]))[0]  # Fraction of H+
+        _v = np.interp(_r, r, velocity)
+        _rho = np.interp(_r, r, density)
+        f_h_ion = np.interp(_r, r, hydrogen_ion_fraction)  # Fraction of H+
 
         # Assume the number density of electrons is equal to the number density
         # of H ions + He ions
-        n_e = k1 * _rho * f_h_ion + k2 * _rho * f_he_ion  # Number density of
-        # electrons
-        n_h_plus = k1 * _rho * f_h_ion    # Number density of ionized H
-        n_h0 = k1 * _rho * (1 - f_h_ion)  # Number density of atomic H
+        # Since we may run into loss of numerical precision here (big numbers),
+        # we manipulate the equations to avoid this problem. It looks a bit
+        # messy, but it is necessary
+        log_term_1 = np.log(k1) + np.log(_rho)  # H ions
+        log_term_2 = np.log(k2) + np.log(_rho)  # He ions
+        ct_rate_he_hp_n_h_plus = \
+            np.exp(log_term_1 + np.log(ct_rate_he_hp)) * f_h_ion
+        alpha_rec_n_e = \
+            np.exp(log_term_1 + np.log(alpha_rec)) * f_h_ion + \
+            np.exp(log_term_2 + np.log(alpha_rec)) * f_he_ion
+        ct_rate_hep_h_n_h0 = \
+            np.exp(log_term_1 + np.log(ct_rate_hep_h)) * (1 - f_h_ion)
+
+        # n_e = k1 * _rho * f_h_ion + k2 * _rho * f_he_ion  # Number density of
+        # # electrons
+        # n_h_plus = k1 * _rho * f_h_ion    # Number density of ionized H
+        # n_h0 = k1 * _rho * (1 - f_h_ion)  # Number density of atomic H
 
         # Terms of df_dr
-        tau_he = _tau_he_fun(np.array([_r, ]))[0]
-        term1 = (1 - f_he_ion) * phi_he * np.exp(-tau_he)  # Photoionization
-        term2 = (1 - f_he_ion) * n_h_plus * ct_rate_he_hp  # Charge exchange
+        t_he = np.interp(_r, r, tau_he)
+        term1 = (1 - f_he_ion) * phi_he * np.exp(-t_he)  # Photoionization
+        term2 = (1 - f_he_ion) * ct_rate_he_hp_n_h_plus  # Charge exchange
         # with H+
-        term3 = f_he_ion * n_e * alpha_rec  # Recombination of He II into He I
-        term4 = f_he_ion * n_h0 * ct_rate_hep_h  # Charge exchange of He II with
+        term3 = f_he_ion * alpha_rec_n_e  # Recombination of He II into He I
+        term4 = f_he_ion * ct_rate_hep_h_n_h0  # Charge exchange of He II with
         # neutral H
         df_dr = (term1 + term2 - term3 - term4) / _v
 
         return df_dr
 
     if method == 'odeint':
         # Since 'odeint' yields only warnings when precision is lost or when
@@ -940,15 +990,14 @@
         for i in range(max_n_relax):
             previous_f_r = np.copy(f_r)
 
             # Re-calculate the column densities
             tau_he = \
                 k2 * a_he * np.flip(np.cumsum(
                     np.flip(dr * density * (1 - f_r)))) + tau_h
-            _tau_he_fun = interp1d(r, tau_he, fill_value="extrapolate")
 
             # Solve it again
             if method == 'odeint':
                 sol = odeint(_fun, y0=initial_f_he_ion, t=r, tfirst=True)
                 f_r = np.copy(sol).T[0]
             else:
                 sol = solve_ivp(_fun, (r[0], r[-1],),
```

### Comparing `p_winds-1.4.1b0/p_winds/hydrogen.py` & `p_winds-1.4.4b0/p_winds/hydrogen.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from __future__ import (division, print_function, absolute_import,
                         unicode_literals)
 import numpy as np
 import astropy.units as u
 import astropy.constants as c
 from scipy.integrate import simps, solve_ivp, cumtrapz
-from scipy.interpolate import interp1d
 from p_winds import parker, tools, microphysics
 
 
 __all__ = ["radiative_processes_exact", "radiative_processes",
            "radiative_processes_mono", "recombination", "ion_fraction"]
 
 
@@ -25,38 +24,38 @@
     """
     Calculate the photoionization rate of hydrogen as a function of radius based
     on the EUV spectrum arriving at the planet and the neutral H density
     profile.
 
     Parameters
     ----------
-    spectrum_at_planet (``dict``):
+    spectrum_at_planet : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes at
         least up to the wavelength corresponding to the energy to ionize
         hydrogen (13.6 eV, or 911.65 Angstrom).
     
-    r_grid (``numpy.ndarray``):
+    r_grid : ``numpy.ndarray``
         Radius grid for the calculation, in units of cm.
 
-    density (``numpy.ndarray``):
-        Number density profile for the atmosphere, in units of 1 / cm ** 3.
+    density : ``numpy.ndarray``
+        Total density profile for the atmosphere, in units of g / cm ** 3.
 
-    f_h_r (``numpy.ndarray`` or ``float``):
+    f_h_r : ``numpy.ndarray`` or ``float``
         H ion fraction profile for the atmosphere.
 
-    h_fraction (``float``):
+    h_fraction : ``float``
         Hydrogen number fraction of the outflow.
 
-    f_he_r (``numpy.ndarray`` or ``float`` or ``None``):
+    f_he_r : ``numpy.ndarray`` or ``float`` or ``None``
         He ion fraction profile for the atmosphere. If ``None``, then assume
         that the profile is the same as ``f_h_r``.
 
     Returns
     -------
-    phi_prime (``float``):
+    phi_prime : ``float``
         Ionization rate of hydrogen for each point on r_grid in unit of 1 / s.
     """
     wavelength = (spectrum_at_planet['wavelength'] *
                   spectrum_at_planet['wavelength_unit']).to(u.angstrom).value
     flux_lambda = (spectrum_at_planet['flux_lambda'] * spectrum_at_planet[
         'flux_unit']).to(u.erg / u.s / u.cm ** 2 / u.angstrom).value
     energy = (c.h * c.c).to(u.erg * u.angstrom).value / wavelength
@@ -74,15 +73,15 @@
 
     # 2d grid of radius and wavelength
     xx, yy = np.meshgrid(wavelength_cut, r_grid)
     # Photoionization cross-section in function of wavelength
     a_lambda = microphysics.hydrogen_cross_section(wavelength=xx)
 
     # Optical depth to hydrogen photoionization
-    m_h = 1.67262192E-24  # Proton mass in unit of kg
+    m_h = 1.67262192E-24  # Proton mass in unit of g
     r_grid_temp = r_grid[::-1]
     # We assume that the atmosphere is made of only H + He
     he_fraction = 1 - h_fraction
     f_he_to_h = he_fraction / h_fraction
     mu = (1 + 4 * f_he_to_h) / (1 + f_h_r + f_he_to_h)
 
     n_tot = density / mu / m_h
@@ -119,25 +118,25 @@
 def radiative_processes(spectrum_at_planet):
     """
     Calculate the photoionization rate of hydrogen at null optical depth based
     on the EUV spectrum arriving at the planet.
 
     Parameters
     ----------
-    spectrum_at_planet (``dict``):
+    spectrum_at_planet : ``dict``
         Spectrum of the host star arriving at the planet covering fluxes at
         least up to the wavelength corresponding to the energy to ionize
         hydrogen (13.6 eV, or 911.65 Angstrom).
 
     Returns
     -------
-    phi (``float``):
+    phi : ``float``
         Ionization rate of hydrogen at null optical depth in unit of 1 / s.
 
-    a_0 (``float``):
+    a_0 : ``float``
         Flux-averaged photoionization cross-section of hydrogen in unit of
         cm ** 2.
     """
     wavelength = (spectrum_at_planet['wavelength'] *
                   spectrum_at_planet['wavelength_unit']).to(u.angstrom).value
     flux_lambda = (spectrum_at_planet['flux_lambda'] * spectrum_at_planet[
         'flux_unit']).to(u.erg / u.s / u.cm ** 2 / u.angstrom).value
@@ -173,28 +172,28 @@
 def radiative_processes_mono(flux_euv, average_photon_energy=20.):
     """
     Calculate the photoionization rate of hydrogen at null optical depth based
     on the monochromatic EUV flux arriving at the planet.
 
     Parameters
     ----------
-    flux_euv (``float``):
+    flux_euv : ``float``
         Monochromatic extreme-ultraviolet (0 - 912 Angstrom) flux arriving at
         the planet in unit of erg / s / cm ** 2.
 
-    average_photon_energy (``float``, optional):
+    average_photon_energy : ``float``, optional
         Average energy of the photons ionizing H in unit of eV. Default is 20 eV
         (as in Murray-Clay et al 2009, Allan & Vidotto 2019).
 
     Returns
     -------
-    phi (``float``):
+    phi : ``float``
         Ionization rate of hydrogen at null optical depth in unit of 1 / s.
 
-    a_0 (``float``):
+    a_0 : ``float``
         Flux-averaged photoionization cross-section of hydrogen in unit of
         cm ** 2.
     """
     # Average cross-section
     a_0 = 6.3E-18 * (average_photon_energy / 13.6) ** (-3)  # Unit 1 / cm ** 2.
 
     # Monochromatic ionization rate
@@ -207,139 +206,156 @@
 def recombination(temperature):
     """
     Calculates the case-B hydrogen recombination rate for a gas at a certain
     temperature.
 
     Parameters
     ----------
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
     Returns
     -------
-    alpha_rec (``float``):
+    alpha_rec : ``float``
         Recombination rate of hydrogen in units of cm ** 3 / s.
     """
     alpha_rec = 2.59E-13 * (temperature / 1E4) ** (-0.7)
     return alpha_rec
 
 
 # Fraction of ionized hydrogen vs. radius profile
 def ion_fraction(radius_profile, planet_radius, temperature, h_fraction,
                  mass_loss_rate, planet_mass, mean_molecular_weight_0=1.0,
                  star_mass = 1.0, semimajor_axis = 1.0,
                  spectrum_at_planet=None, flux_euv=None, initial_f_ion=0.0,
                  relax_solution=False, convergence=0.01, max_n_relax=10,
-                 exact_phi=False, return_mu=False, **options_solve_ivp):
+                 exact_phi=False, return_mu=False, return_rates=False,
+                 **options_solve_ivp):
     """
     Calculate the fraction of ionized hydrogen in the upper atmosphere in
     function of the radius in unit of planetary radius.
 
     Parameters
     ----------
-    radius_profile (``numpy.ndarray``):
+    radius_profile : ``numpy.ndarray``
         Radius in unit of planetary radii.
 
-    planet_radius (``float``):
+    planet_radius : ``float``
         Planetary radius in unit of Jupiter radius.
 
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the upper atmosphere in unit of Kelvin.
 
-    h_fraction (``float``):
+    h_fraction : ``float``
         Total (ion + neutral) H number fraction of the atmosphere.
 
-    mass_loss_rate (``float``):
+    mass_loss_rate : ``float``
         Mass loss rate of the planet in units of g / s.
 
-    planet_mass (``float``):
+    planet_mass : ``float``
         Planetary mass in unit of Jupiter mass.
 
-    mean_molecular_weight_0 (``float``):
+    mean_molecular_weight_0 : ``float``
         Initial mean molecular weight of the atmosphere in unit of proton mass.
         Default value is 1.0 (100% neutral H). Since its final value depend on
         the H ion fraction itself, the mean molecular weight can be
         self-consistently calculated by setting `relax_solution` to `True`.
 
-    star_mass (``float``, optional):
+    star_mass : ``float``, optional
         Stellar mass in units of M_sun, needed for the tidal gravity
         calculation. Default is 1.
 
-    semimajor_axis (``float``, optional):
+    semimajor_axis : ``float``, optional
         Planetary semimajor axis in units of au, needed for the tidal gravity
         calculation. Default is 1 (so the tidal gravity correction is minimal by
         default).
 
-    spectrum_at_planet (``dict``, optional):
+    spectrum_at_planet : ``dict``, optional
         Spectrum of the host star arriving at the planet covering fluxes at
         least up to the wavelength corresponding to the energy to ionize
         hydrogen (13.6 eV, or 911.65 Angstrom). Can be generated using
         ``tools.make_spectrum_dict``. If ``None``, then ``flux_euv`` must be
         provided instead. Default is ``None``.
 
-    flux_euv (``float``, optional):
+    flux_euv : ``float``, optional
         Extreme-ultraviolet (0-911.65 Angstrom) flux arriving at the planet in
         units of erg / s / cm ** 2. If ``None``, then ``spectrum_at_planet``
         must be provided instead. Default is ``None``.
 
-    initial_f_ion (``float``, optional):
+    initial_f_ion : ``float``, optional
         The initial ionization fraction at the layer near the surface of the
         planet. Default is 0.0, i.e., 100% neutral.
 
-    relax_solution (``bool``, optional):
+    relax_solution : ``bool``, optional
         The first solution is calculating by initially assuming the entire
         atmosphere is in neutral state. If ``True``, the solution will be
         re-calculated in a loop until it converges to a delta_f of 1%, or for a
         maximum of 10 loops (default parameters). Default is ``False``.
 
-    convergence (``float``, optional):
+    convergence : ``float``, optional
         Value of delta_f at which to stop the relaxation of the solution for
         ``f_r``. Default is 0.01.
 
-    max_n_relax (``int``, optional):
+    max_n_relax : ``int``, optional
         Maximum number of loops to perform the relaxation of the solution for
         ``f_r``. Default is 10.
 
-    return_mu (``bool``, optional):
+    exact_phi : ``bool``, optional
+        If set to ``True``, the H photoionization is calculated exactly (using
+        the ``radiative_processes_exact()`` function). If set to ``False``, then
+        calculate it using an approximation with ``radiative_processes()``.
+        Default value is ``False``.
+
+    return_mu : ``bool``, optional
         If ``True``, then this function returns a second variable ``mu_bar``,
         which is the self-consistent, density-averaged mean molecular weight of
         the atmosphere. Equivalent to the ``mu_bar`` of Eq. A.3 in Lampón et
         al. 2020.
 
+    return_rates : ``bool``, optional
+        If ``True``, then this function also returns a ``dict`` object
+        containing the rates of photoionization and recombination in function of
+        radius and in units of 1 / s. Default is ``False``.
+
     **options_solve_ivp:
         Options to be passed to the ``scipy.integrate.solve_ivp()`` solver. You
         may want to change the options ``method`` (integration method; default
         is ``'RK45'``), ``atol`` (absolute tolerance; default is 1E-6) or
         ``rtol`` (relative tolerance; default is 1E-3). If you are having
         numerical issues, you may want to decrease the tolerance by a factor of
         10 or 100, or 1000 in extreme cases.
 
     Returns
     -------
-    f_r (``numpy.ndarray``):
+    f_r : ``numpy.ndarray``
         Values of the fraction of ionized hydrogen in function of the radius.
 
-    mu_bar (``float``):
+    mu_bar : ``float``
         Mean molecular weight of the atmosphere, in unit of proton mass,
         averaged across the radial distance using according to the function
         `average_molecular_weight` in the `parker` module. Only returned when
         ``return_mu`` is set to ``True``.
+
+    rates : ``dict``
+        Dictionary containing the rates of photoionization and recombination in
+        function of radius and in units of 1 / s. Only returned when
+        ``return_rates`` is set to ``True``.
     """
     # Hydrogen recombination rate
     alpha_rec = recombination(temperature)
 
     # Hydrogen mass in g
     m_h = 1.67262192E-24
 
     # Photoionization rate at null optical depth at the distance of the planet
     # from the host star, in unit of 1 / s.
+    vs = parker.sound_speed(temperature, mean_molecular_weight_0)
+    rs = parker.radius_sonic_point_tidal(planet_mass, vs, star_mass,
+                                            semimajor_axis)
     if exact_phi and spectrum_at_planet is not None:
-        vs = parker.sound_speed(temperature, mean_molecular_weight_0)
-        rs = parker.radius_sonic_point_tidal(planet_mass, vs, star_mass,
-                                             semimajor_axis)
         rhos = parker.density_sonic_point(mass_loss_rate, rs, vs)
         _, rho_norm = parker.structure_tidal(
             radius_profile * planet_radius / rs, vs, rs, planet_mass,
             star_mass, semimajor_axis)
         f_outer = 0.0  # Assume completely ionized at the top of atmosphere
         phi_abs = radiative_processes_exact(
             spectrum_at_planet,
@@ -394,46 +410,39 @@
                                                   star_mass, semimajor_axis)
 
         return phi_norm, k1_norm, k2_norm, r_norm, dr_norm, v_norm, rho_norm
 
     phi, k1, k2, r, dr, velocity, density = _normalize(
         phi_abs, k1_abs, k2_abs, radius_profile, mean_molecular_weight_0)
 
-    if exact_phi:
-        _phi_prime_fun = interp1d(r, phi, fill_value="extrapolate")
-    else:
+    if exact_phi is False:
         # To start the calculations we need the optical depth, but technically
         # we don't know it yet, because it depends on the ion fraction in the
         # atmosphere, which is what we want to obtain. However, the optical
         # depth depends more strongly on the densities of H than the ion
         # fraction, so a good first approximation is to assume the whole
         # atmosphere is neutral at first.
         column_density = np.flip(np.cumsum(np.flip(dr * density)))
-        tau_initial = k1 * column_density
-        # We do a dirty hack to make tau_initial and velocity a callable
-        # function so it's easily parsed inside the differential equation solver
-        _tau_fun = interp1d(r, tau_initial, fill_value="extrapolate")
-    _v_fun = interp1d(r, velocity, fill_value="extrapolate")
-
-    _v_fun = interp1d(r, velocity, fill_value="extrapolate")
-    _rho_fun = interp1d(r, density, fill_value="extrapolate")
+        tau = k1 * column_density
+    else:
+        pass
 
     # Now let's solve the differential eq. 13 of Oklopcic & Hirata 2018
     # The differential equation in function of r
     def _fun(_r, _f, _phi, _k2):
         if exact_phi:
-            _phi_prime = _phi_prime_fun(np.array([_r, ]))[0]
+            _phi_prime = np.interp(_r, r, phi)
         else:
-            _t = _tau_fun(np.array([_r, ]))[0]
-            _phi_prime = np.exp(-_t)*_phi
+            _t = np.interp(_r, r, tau)
+            _phi_prime = np.exp(-_t) * _phi
 
         # The next two lines may need to be substituted by `structure_tidal()`
         # instead of interpolated
-        _v = _v_fun(_r)
-        _rho = _rho_fun(_r)
+        _v = np.interp(_r, r, velocity)
+        _rho = np.interp(_r, r, density)
 
         # In terms 1 and 2 we use the values of k2 and phi from above
         term1 = (1. - _f) / _v * _phi_prime
         term2 = _k2 * _rho * _f ** 2 / _v
         df_dr = term1 - term2
 
         return df_dr
@@ -448,15 +457,17 @@
     # size than `r`. So we raise an exception if this happens
     if len(f_r) != len(r):
         raise RuntimeError('The solver ``solve_ivp`` failed to obtain a'
                            ' solution.')
 
     # Calculate the average mean molecular weight using Eq. A.3 from Lampón et
     # al. 2020
-    mu_bar = parker.average_molecular_weight(f_r, radius_profile, velocity,
+    mu_bar = parker.average_molecular_weight(f_r,
+                                             radius_profile * planet_radius,
+                                             velocity * vs,
                                              planet_mass, temperature,
                                              he_h_fraction)
 
     # For the sake of self-consistency, there is the option of repeating the
     # calculation of f_r by updating the optical depth with the new ion
     # fractions.
     if relax_solution is True:
@@ -479,41 +490,37 @@
                     rho_norm * rhos, f_r, h_fraction)
 
             # We re-normalize key parameters because the newly-calculated f_ion
             # changes the value of the mean molecular weight of the atmosphere
             phi, k1, k2, r, dr, velocity, density = _normalize(
                 phi_abs, k1_abs, k2_abs, radius_profile, mu_bar)
 
-            if exact_phi:
-                _phi_prime_fun = interp1d(r, phi, fill_value="extrapolate")
-            else:
+            if exact_phi is False:
                 # Re-calculate the column densities
                 column_density = np.flip(np.cumsum(np.flip(dr * density *
                                                            (1 - f_r))))
                 tau = k1 * column_density
-                _tau_fun = interp1d(r, tau, fill_value="extrapolate")
-            _v_fun = interp1d(r, velocity, fill_value="extrapolate")
             
             # And solve it again
             sol = solve_ivp(_fun, (r[0], r[-1],), np.array([initial_f_ion, ]),
                             t_eval=r, args=(phi, k2,), 
                             **options_solve_ivp)
             f_r = sol['y'][0]
 
             # Raise an error if the length of `f_r` is different from the length
             # of `r`
             if len(f_r) != len(r):
                 raise RuntimeError('The solver ``solve_ivp`` failed to obtain a'
                                    ' solution.')
 
             # Here we update the average mean molecular weight
-            mu_bar = parker.average_molecular_weight(f_r, radius_profile,
-                                                     velocity,
-                                                     planet_mass, temperature,
-                                                     he_h_fraction)
+            mu_bar = parker.average_molecular_weight(
+                f_r, radius_profile * planet_radius, velocity * vs, planet_mass,
+                temperature, he_h_fraction
+            )
 
             # Calculate the relative change of f_ion in the outer shell of the
             # atmosphere (where we expect the most important change)
             # relative_delta_f = abs(f_r[-1] - previous_f_r_outer_layer) \
             #     / previous_f_r_outer_layer
             relative_delta_f = abs(
                 np.sum(f_r - previous_f_r) / np.sum(previous_f_r))
@@ -522,11 +529,46 @@
             if relative_delta_f < convergence:
                 break
             else:
                 pass
     else:
         pass
 
-    if return_mu is False:
-        return f_r
+    # Calculate the final structure and rates of photoionization and
+    # recombination in function of radius
+    if return_rates is True:
+        # Final photoionization rate in unit of 1 / s
+        final_phi_prime = radiative_processes_exact(
+            spectrum_at_planet,
+            (radius_profile * planet_radius * u.Rjup).to(u.cm).value,
+            rho_norm * rhos, f_r, h_fraction) * (1 - f_r)
+        # Final sound speed in km / s
+        final_vs = parker.sound_speed(temperature, mu_bar)
+        # Final radius at the sonic point in units of Jupiter radii
+        final_rs = parker.radius_sonic_point_tidal(planet_mass, final_vs,
+                                                   star_mass, semimajor_axis)
+        # Final density at the sonic point in unit of g / cm ** 3
+        final_rhos = parker.density_sonic_point(mass_loss_rate, final_rs,
+                                                final_vs)
+        # Final velocity and density profiles in units of sonic point
+        final_r_norm = (radius_profile * planet_radius / final_rs)
+        final_v_norm, final_rho_norm = parker.structure_tidal(
+            final_r_norm, final_vs, final_rs, planet_mass, star_mass,
+            semimajor_axis)
+        # Final density profile in g / cm ** 3
+        final_rho = final_rho_norm * final_rhos
+        # Final recombination rate in 1 / s
+        final_alpha_rec = recombination(temperature) * k2_abs * final_rho * \
+            f_r ** 2
+        rates = {'photoionization': final_phi_prime,
+                 'recombination': final_alpha_rec}
     else:
+        pass
+
+    if return_mu is True and return_rates is False:
         return f_r, mu_bar
+    elif return_mu is False and return_rates is True:
+        return f_r, rates
+    elif return_mu is True and return_rates is True:
+        return f_r, mu_bar, rates
+    else:
+        return f_r
```

### Comparing `p_winds-1.4.1b0/p_winds/lines.py` & `p_winds-1.4.4b0/p_winds/lines.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,33 +16,33 @@
     Returns the central wavelengths in air, oscillator strengths and the
     Einstein coefficient of the helium triplet in 1.083 microns. The values
     were taken from the NIST database:
     https://www.nist.gov/pml/atomic-spectra-database
 
     Returns
     -------
-    lambda_0 (``float``):
+    lambda_0 : ``float``
         Central wavelength in air of line 0 in unit of m.
 
-    lambda_1 (``float``):
+    lambda_1 : ``float``
         Central wavelength in air of line 1 in unit of m.
 
-    lambda_2 (``float``):
+    lambda_2 : ``float``
         Central wavelength in air of line 2 in unit of m.
 
-    f_0 (``float``):
+    f_0 : ``float``
         Oscillator strength of line 0 (unitless).
 
-    f_1 (``float``):
+    f_1 : ``float``
         Oscillator strength of line 1 (unitless).
 
-    f_2 (``float``):
+    f_2 : ``float``
         Oscillator strength of line 2 (unitless).
 
-    a_ij (``float``):
+    a_ij : ``float``
         Einstein coefficient of the whole triplet in unit of 1 / s.
     """
     # Central wavelengths in units of m
     lambda_0 = 1.082909114 * 1E-6
     lambda_1 = 1.083025010 * 1E-6
     lambda_2 = 1.083033977 * 1E-6
     # Oscillator strengths
@@ -62,39 +62,39 @@
     Returns the central wavelengths in air, oscillator strengths and the
     Einstein coefficient of the C II lines in the STIS FUV wavelength range. The
     values were taken from the NIST database:
     https://www.nist.gov/pml/atomic-spectra-database
 
     Returns
     -------
-    lambda_0 (``float``):
+    lambda_0 : ``float``
         Central wavelength in air of line 0 in unit of m.
 
-    lambda_1 (``float``):
+    lambda_1 : ``float``
         Central wavelength in air of line 1 in unit of m.
 
-    lambda_2 (``float``):
+    lambda_2 : ``float``
         Central wavelength in air of line 2 in unit of m.
 
-    f_0 (``float``):
+    f_0 : ``float``
         Oscillator strength of line 0 (unitless).
 
-    f_1 (``float``):
+    f_1 : ``float``
         Oscillator strength of line 1 (unitless).
 
-    f_2 (``float``):
+    f_2 : ``float``
         Oscillator strength of line 2 (unitless).
 
-    a_ij_0 (``float``):
+    a_ij_0 : ``float``
         Einstein coefficient of line 0 in unit of 1 / s.
 
-    a_ij_1 (``float``):
+    a_ij_1 : ``float``
         Einstein coefficient of line 1 in unit of 1 / s.
 
-    a_ij_2 (``float``):
+    a_ij_2 : ``float``
         Einstein coefficient of line 2 in unit of 1 / s.
     """
     # Central wavelengths in units of m
     lambda_0 = 1334.5323 * 1E-10
     lambda_1 = 1335.6628 * 1E-10
     lambda_2 = 1335.7079 * 1E-10
     # Oscillator strengths
@@ -116,39 +116,39 @@
     Returns the central wavelengths in air, oscillator strengths and the
     Einstein coefficient of the O I lines in the STIS FUV wavelength range. The
     values were taken from the NIST database:
     https://www.nist.gov/pml/atomic-spectra-database
 
     Returns
     -------
-    lambda_0 (``float``):
+    lambda_0 : ``float``
         Central wavelength in air of line 0 in unit of m.
 
-    lambda_1 (``float``):
+    lambda_1 : ``float``
         Central wavelength in air of line 1 in unit of m.
 
-    lambda_2 (``float``):
+    lambda_2 : ``float``
         Central wavelength in air of line 2 in unit of m.
 
-    f_0 (``float``):
+    f_0 : ``float``
         Oscillator strength of line 0 (unitless).
 
-    f_1 (``float``):
+    f_1 : ``float``
         Oscillator strength of line 1 (unitless).
 
-    f_2 (``float``):
+    f_2 : ``float``
         Oscillator strength of line 2 (unitless).
 
-    a_ij_0 (``float``):
+    a_ij_0 : ``float``
         Einstein coefficient of line 0 in unit of 1 / s.
 
-    a_ij_1 (``float``):
+    a_ij_1 : ``float``
         Einstein coefficient of line 1 in unit of 1 / s.
 
-    a_ij_2 (``float``):
+    a_ij_2 : ``float``
         Einstein coefficient of line 2 in unit of 1 / s.
     """
     # Central wavelengths in units of m
     lambda_0 = 1302.168 * 1E-10
     lambda_1 = 1304.858 * 1E-10
     lambda_2 = 1306.029 * 1E-10
     # Oscillator strengths
```

### Comparing `p_winds-1.4.1b0/p_winds/microphysics.py` & `p_winds-1.4.4b0/p_winds/microphysics.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 """
 
 from __future__ import (division, print_function, absolute_import,
                         unicode_literals)
 import numpy as np
 import astropy.units as u
 import astropy.constants as c
-from warnings import warn
+from warnings import warn, filterwarnings
+
+# Ignore some annoying warnings that are not a problem when using the MUSCLES
+# spectra
+filterwarnings(action='ignore', category=RuntimeWarning)
 
 
 __all__ = ["hydrogen_cross_section", "helium_total_cross_section",
            "helium_singlet_cross_section", "helium_triplet_cross_section",
            "he_collisional_strength", "general_cross_section",
            "sigma_properties_v1996", "collisional_excitation"]
 
@@ -23,29 +27,29 @@
 def hydrogen_cross_section(wavelength=None, energy=None):
     """
     Compute the photoionization cross-section of hydrogen in function of
     wavelength or energy.
 
     Parameters
     ----------
-    wavelength (``float`` or ``numpy.ndarray``, optional):
+    wavelength : ``float`` or ``numpy.ndarray``, optional
         Wavelength in unit of angstrom. Default is ``None``. If ``None``,
         ``energy`` cannot be ``None``.
 
-    energy (``float`` or ``numpy.ndarray``, optional):
+    energy : ``float`` or ``numpy.ndarray``, optional
         Energy in unit of electron-volt. Default is ``None``. If ``None``,
         ``wavelength`` cannot be ``None``.
 
     Returns
     -------
-    a_lambda (``float`` or ``numpy.ndarray``):
+    a_lambda : ``float`` or ``numpy.ndarray``
         Cross-section in function of wavelength and in unit of cm ** 2. Only
         returned if wavelength was input.
 
-    a_nu (``float`` or ``numpy.ndarray``):
+    a_nu : ``float`` or ``numpy.ndarray``
         Cross-section in function of energy and in unit of cm ** 2. Only
         returned if energy was input.
     """
 
     if wavelength is not None:
         epsilon = (911.65 / wavelength - 1) ** 0.5
         # Photoionization cross-section in function of wavelength
@@ -76,20 +80,20 @@
     Compute the total photoionization cross-section of helium in function of
     wavelength.
 
     Source: Yan, Sadeghpour, & Dalgarno (1998, ApJ)
 
     Parameters
     ----------
-    wavelength (``numpy.ndarray``):
+    wavelength : ``numpy.ndarray``
         Wavelength in unit of angstrom.
 
     Returns
     -------
-    a_lambda_1 (``numpy.ndarray``):
+    a_lambda_1 : ``numpy.ndarray``
         Cross-section in function of wavelength and in unit of cm ** 2.
     """
     nu_init = (wavelength * u.AA).to(u.Hz, equivalencies=u.spectral())
     threshold_energy = 24.58 * u.eV
     nu = nu_init.to(u.eV, equivalencies=u.spectral())
     x = nu / threshold_energy
     e_term = (nu / u.eV / 1000.) ** (7 / 2)
@@ -110,20 +114,20 @@
 def helium_singlet_cross_section(wavelength):
     """
     Compute the photoionization cross-section of helium singlet in function of
     wavelength.
 
     Parameters
     ----------
-    wavelength (``float`` or ``numpy.ndarray``):
+    wavelength : ``float`` or ``numpy.ndarray``
         Wavelength in unit of angstrom.
 
     Returns
     -------
-    a_lambda_1 (``float`` or ``numpy.ndarray``):
+    a_lambda_1 : ``float`` or ``numpy.ndarray``
         Cross-section in function of wavelength and in unit of cm ** 2.
     """
     energy = 12398.41984332 / wavelength  # Energy in unit of eV
 
     # The cross-sections for helium are partially hard-coded and based on those
     # of hydrogen
     a_lambda_h = hydrogen_cross_section(wavelength=wavelength)
@@ -143,18 +147,18 @@
 def helium_triplet_cross_section():
     """
     Compute the photoionization cross-section of helium triplet in function of
     wavelength.
 
     Returns
     -------
-    wavelength (``numpy.ndarray``):
+    wavelength : ``numpy.ndarray``
         Wavelength in which the cross-section was sampled in Norcross (1971).
 
-    a_lambda_3 (``numpy.ndarray``):
+    a_lambda_3 : ``numpy.ndarray``
         Cross-section in function of wavelength and in unit of cm ** 2.
     """
     # The photoionization cross-section of He triplet is hard-coded with the
     # values calculated by Norcross 1971 (ADS:1971JPhB....4..652N). The
     # differential oscillator strength is calculated for bins of wavelength that
     # are not necessarily the same as the stellar spectrum wavelength bins.
 
@@ -193,15 +197,15 @@
 def he_collisional_strength():
     """
     Returns a hard-coded array containing the helium collisional strengths in
     function of temperature.
 
     Returns
     -------
-    array (``numpy.ndarray``):
+    array : ``numpy.ndarray``
         Collisional strengths array. Columns: 0 = temperature, 1 = gamma_13,
         2 = gamma_31a, 3 = gamma_31b.
     """
     # log(T) [K]    gamma_13    gamma_31a   gamma_31b
     array = np.array([
         [3.75,            6.198E-2,    2.389,       7.965E-1],
         [4.00,            6.458E-2,    2.456,       9.579E-1],
@@ -221,25 +225,25 @@
     """
     Calculates the photoionization cross-section of an atomic or ion species
     using the parametrization of Verner et al. (1996)
     [https://ui.adsabs.harvard.edu/abs/1996ApJ...465..487V/abstract].
 
     Parameters
     ----------
-    wavelength (``float`` or ``numpy.ndarray``)
+    wavelength : ``float`` or ``numpy.ndarray``
         Photon wavelength in angstrom.
 
-    species (``str``):
+    species : ``str``
         String containing the species for which you request the cross-section in
         the format ``'X N'`` where ``X`` is the element and ``N`` is the
         ionization number. Example: ``'C II'``.
 
     Returns
     -------
-    cross_section (``float`` or ``numpy.ndarray``):
+    cross_section : ``float`` or ``numpy.ndarray``
         Cross-section in unit of cm ** (-2)
     """
     # Convert wavelength to energy
     energy = (c.h * c.c / wavelength / u.angstrom).to(u.eV).value
 
     parameters_dict = sigma_properties_v1996()
     energy_threshold, energy_max, energy_0, sigma_0, y_a, p, y_w, y_0, y_1 = \
@@ -282,15 +286,15 @@
 def sigma_properties_v1996():
     """
     Function that hard-codes the cross-section parameters from Verner et al.
     (1996). We include only the species important for exoplanetary atmospheres.
 
     Returns
     -------
-    parameters_dict (``dict``):
+    parameters_dict : ``dict``
         Dictionary containing the parameters.
     """
     parameters_dict = {
         #         E_thresold, E_max, energy_0, sigma_0, y_a, p,
         #         y_w, y_0, y_1
         'C I':    [1.126E1, 2.910E2, 2.144E0, 5.027E2, 6.126E1, 5.101E0,
                    9.157E-2, 1.133E0, 1.607E0],
```

### Comparing `p_winds-1.4.1b0/p_winds/parker.py` & `p_winds-1.4.4b0/p_winds/parker.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 
 from __future__ import (division, print_function, absolute_import,
                         unicode_literals)
 import numpy as np
 import scipy.optimize as so
 from scipy.integrate import simps, trapz
-from p_winds import tools
 from astropy import units as u, constants as c
 
 __all__ = ["average_molecular_weight", "sound_speed", "radius_sonic_point",
            "density_sonic_point", "structure", "radius_sonic_point_tidal",
            "structure_tidal"]
 
 
@@ -22,37 +21,37 @@
                              planet_mass, temperature, he_h_fraction=0.1 / 0.9):
     """
     Calculates the "average" mean molecular weight of the upper atmosphere
     following Eq. A.3 in Lampón et al. 2020, in unit of proton mass.
 
     Parameters
     ----------
-    ion_fraction_profile (``numpy.ndarray``):
+    ion_fraction_profile : ``numpy.ndarray``
         Hydrogen ion fraction in function of radial distance.
 
-    r_profile (``numpy.ndarray``):
+    r_profile : ``numpy.ndarray``
         Radial distance profile in unit of Jupiter radii. This is the
         independent variable over which the profiles are described.
 
-    v_profile (``numpy.ndarray``):
+    v_profile : ``numpy.ndarray``
         Velocity profile in units of km / s in function of radial distance.
 
-    planet_mass (``float``):
+    planet_mass : ``float``
         Planetary mass in unit of Jupiter mass.
 
-    temperature (``float``):
+    temperature : ``float``
         Isothermal temperature of the outflow in unit of K.
 
-    he_h_fraction (``float``, optional):
+    he_h_fraction : ``float``, optional
         Number fraction of He particles in relation to H particles. Default is
         0.1 / 0.9.
 
     Returns
     -------
-    mu_bar (``float``):
+    mu_bar : ``float``
         "Average" mean molecular weight as defined by Eq. A.3 of Lampón et al.
         2020, in unit of proton mass.
     """
     # Converting units
     m_planet = planet_mass * 1.8981246e+27  # Planet mass in kg
     r = r_profile * 71492000.0  # Radius profile in m
     v_r = v_profile * 1000  # Velocity profile in unit of m / s
@@ -83,26 +82,26 @@
 # Speed of sound
 def sound_speed(temperature, mean_molecular_weight=1.0):
     """
     Speed of sound in an isothermal ideal gas.
 
     Parameters
     ----------
-    temperature (``float``):
+    temperature : ``float``
         Constant temperature of the gas in Kelvin. Assumed to be close to the
         maximum thermospheric temperature (see Oklopčić & Hirata 2018 and
         Lampón et al. 2020 for more details).
 
-    mean_molecular_weight (``float``):
+    mean_molecular_weight : ``float``
         Mean molecular weight of the atmosphere in unit of proton mass. Default
         value is 1.0 (100% neutral H).
 
     Returns
     -------
-    cs (``float``):
+    cs : ``float``
         Sound speed in the gas in unit of km / s.
     """
     m_h = 1.67262192369e-27  # Hydrogen mass in kg
     k_b = 1.380649e-29  # Boltzmann constant in km ** 2 / s ** 2 * kg / K
     cs = (k_b * temperature / mean_molecular_weight / m_h) ** 0.5
     return cs
 
@@ -111,23 +110,23 @@
 def radius_sonic_point(planet_mass, sound_speed_0):
     """
     Radius of the sonic point, i.e., where the wind speed matches the speed of
     sound.
 
     Parameters
     ----------
-    planet_mass (``float``):
+    planet_mass : ``float``
         Planetary mass in unit of Jupiter mass.
 
-    sound_speed_0 (``float``):
+    sound_speed_0 : ``float``
         Constant speed of sound in unit of km / s.
 
     Returns
     -------
-    radius_sonic_point (``float``):
+    radius_sonic_point : ``float``
         Radius of the sonic point in unit of Jupiter radius.
     """
     grav = 1772.0378503888546  # Gravitational constant in unit of
     # jupiterRad * km ** 2 / s ** 2 / jupiterMass
     radius_sonic_point = grav * planet_mass / 2 / sound_speed_0 ** 2
     return radius_sonic_point
 
@@ -136,26 +135,26 @@
 def density_sonic_point(mass_loss_rate, radius_sp, sound_speed_0):
     """
     Density at the sonic point, where the wind speed matches the speed of
     sound. The input values must be `astropy.Quantity`.
 
     Parameters
     ----------
-    mass_loss_rate (``float``):
+    mass_loss_rate : ``float``
         Total mass loss rate of the planet in units of g / s.
 
-    radius_sp (``float``):
+    radius_sp : ``float``
         Radius at the sonic point in unit of Jupiter radius.
 
-    sound_speed_0 (``float``):
+    sound_speed_0 : ``float``
         Speed of sound, assumed to be constant, in units of km / s.
 
     Returns
     -------
-    rho_sp (``float``):
+    rho_sp : ``float``
         Density at the sonic point in units of g / cm ** 3.
     """
     vs = sound_speed_0 * 1E5  # Convert sound speed to cm / s
     rs = radius_sp * 7.1492E+09  # Convert radius to cm
     rho_sp = mass_loss_rate / 4 / np.pi / rs ** 2 / vs
     return rho_sp
 
@@ -165,31 +164,31 @@
     """
     Calculate the velocity and density of the atmosphere in function of radius
     at the sonic point, and in units of sound speed and density at the sonic
     point, respectively.
 
     Parameters
     ----------
-    r (``numpy.ndarray`` or ``float``):
+    r : ``numpy.ndarray`` or ``float``
         Radius at which to sample the velocity in unit of radius at the sonic
         point.
         
-    v_guess (``numpy.ndarray`` or ``float``, optional):
+    v_guess : ``numpy.ndarray`` or ``float``, optional
         Guessed value(s) of velocity, in unit of sound speed, corresponding to 
         the radius(ii) ``r``. If ``None``, then the code assumes a standard 
         guess for the velocity. If not ``None``, ``v_guess`` must have the same
         shape as ``r``. Default is ``None``.
 
     Returns
     -------
-    velocity_r (``numpy.ndarray`` or ``float``):
+    velocity_r : ``numpy.ndarray`` or ``float``
         `numpy` array or a single value of velocity at the given radius or radii
         in unit of sound speed.
 
-    density_r (``numpy.ndarray`` or ``float``):
+    density_r : ``numpy.ndarray`` or ``float``
         Density sampled at the radius or radii `r` and in unit of density at the
         sonic point.
     """
     def _eq_to_solve(v, r_k):
         eq = v * np.exp(-0.5 * v ** 2) - (1 / r_k) ** 2 * np.exp(
             -2 * 1 / r_k + 3 / 2)
         return eq
@@ -204,20 +203,18 @@
         velocity_r = so.newton(_eq_to_solve, x0=v_guess, args=(r,))
 
     # Otherwise, we set it automatically: If the radius is below the sonic
     # radius, the first guess is 0.1. If the radius is above, the first
     # guess is 2.0. This is a hacky solution, but it seems to work well.
     elif isinstance(r, np.ndarray):
         # If r is a ``numpy.ndarray``, we do a dirty little hack to setup an
-        # array of first guesses `x0` whose values are 0.1 for r <= 1, and 2 if
-        # r > 1.
-        ind = tools.nearest_index(r, 1.0)  # Find the index where r == 1.0
-        x0_array = np.ones_like(r) * 0.1   # Setup the array of first guesses
-        x0_array[ind:] *= 20.0
-        velocity_r = so.newton(_eq_to_solve, x0=x0_array, args=(r,))
+        # array of first guesses `x0` whose values are 0.1 for r <= 1, and 2.1
+        # if r > 1.
+        v_init = np.array(r > 1, dtype=int) * 2 + 0.1
+        velocity_r = so.newton(_eq_to_solve, x0=v_init, args=(r,))
     # If r is float, just do a simple if statement
     else:
         if r <= 1.0:
             velocity_r = so.newton(_eq_to_solve, x0=1E-1, args=(r,))
         else:
             velocity_r = so.newton(_eq_to_solve, x0=2.0, args=(r,))
 
@@ -229,29 +226,29 @@
                              semi_major_axis):
     """
     Radius of the sonic point, i.e., where the wind speed matches the speed of
     sound, accounting for the tidal gravity of the host star.
 
     Parameters
     ----------
-    planet_mass (``float``):
+    planet_mass : ``float``
         Planetary mass in unit of Jupiter mass.
 
-    sound_speed_0 (``float``):
+    sound_speed_0 : ``float``
         Constant speed of sound in unit of km / s.
 
-    star_mass (``float``):
+    star_mass : ``float``
         Stellar mass in unit of solar mass.
 
-    semi_major_axis (``float``):
+    semi_major_axis : ``float``
         Planetary semimajor axis in unit of AU.
 
     Returns
     -------
-    radius_sonic_point (``float``):
+    radius_sonic_point : ``float``
         Radius of the sonic point in units of Jupiter radius.
     """
     grav = 1772.0378503888546  # Gravitational constant in unit of
     # jupiterRad * km ** 2 / s ** 2 / jupiterMass
 
     # Convert stellar mass unit to Jupiter mass and semi_major_axis unit to
     # Jupiter radius
@@ -274,41 +271,41 @@
     Calculate the velocity and density of the atmosphere in function of radius
     at the sonic point, and in units of sound speed and density at the sonic
     point, respectively. This version accounts for the tidal gravity of the host
     star.
 
     Parameters
     ----------
-    r (``numpy.ndarray`` or ``float``):
+    r : ``numpy.ndarray`` or ``float``
         Radius at which to sample the velocity in unit of radius at the sonic
         point.
 
-    sound_speed_0 (``float``):
+    sound_speed_0 : ``float``
         Constant speed of sound in unit of km / s.
 
-    radius_sonic_point (``float``):
+    radius_sonic_point : ``float``
         Sonic radius in unit of Jupiter radius. Note: ensure that this is
         computed with ``radius_sonic_point_tidal``.
 
-    planet_mass (``float``):
+    planet_mass : ``float``
         Planetary mass in unit of Jupiter mass.
 
-    star_mass (``float``):
+    star_mass : ``float``
         Stellar mass in unit of solar mass.
 
-    semi_major_axis (``float``):
+    semi_major_axis : ``float``
         Planetary semimajor axis in unit of AU.
 
     Returns
     -------
-    velocity_r (``numpy.ndarray`` or ``float``):
+    velocity_r : ``numpy.ndarray`` or ``float``
         `numpy` array or a single value of velocity at the given radius or radii
         in unit of sound speed.
 
-    density_r (``numpy.ndarray`` or ``float``):
+    density_r : ``numpy.ndarray`` or ``float``
         Density sampled at the radius or radii `r` and in unit of density at the
         sonic point.
     """
 
     # First make all quantities cgs, then work with values only
     sound_speed_0 = 100000. * sound_speed_0
     radius_sonic_point = 7.1492e+09 * radius_sonic_point
@@ -323,36 +320,36 @@
             - grav * M_p / (c_s ** 2 * (r * r_s)) + grav * M_p / (c_s ** 2 * r_s) \
             - 3 * grav * M_star * (r * r_s) ** 2 / (2 * a ** 3 * c_s ** 2) \
             + 3 * grav * M_star * r_s ** 2 / (2 * a ** 3 * c_s ** 2) - 0.5
         )
         return eq
 
     if isinstance(r, np.ndarray):
-        # One line verison of Leo's initial value hack gives 0.1 below sonic
+        # One line version of Leo's initial value hack gives 0.1 below sonic
         # point and 2 above
         v_init = (np.array(r > 1, dtype=int) * 2 + 0.1)
 
         # Compute velocity profile
-        velocity_r = np.array([so.newton(_eq_to_solve, x0=v_init[k],
-            args=(r[k], sound_speed_0, radius_sonic_point, planet_mass,
-                  star_mass, semi_major_axis),
-            maxiter = 1000) for k in range(len(r))])    
+        velocity_r = so.newton(_eq_to_solve, x0=v_init,
+            args=(r, sound_speed_0, radius_sonic_point, planet_mass,
+                  star_mass, semi_major_axis), maxiter=1000)
     elif r <= 1.0:
         velocity_r = so.newton(_eq_to_solve, x0=1E-1,
                                args=(r, sound_speed_0, radius_sonic_point,
                                      planet_mass, star_mass, semi_major_axis))
     else:
         velocity_r = so.newton(_eq_to_solve, x0=2.0,
                                args=(r, sound_speed_0, radius_sonic_point,
                                      planet_mass, star_mass, semi_major_axis))
 
     # Some useful definitions to make the code cleaner
     k1 = sound_speed_0 ** 2 * (r * radius_sonic_point)
-    k2 = 2 * semi_major_axis ** 3 * sound_speed_0 ** 2
-    density_r = np.exp(grav * planet_mass / k1 - grav * planet_mass / k1 \
-        + 3 * grav * star_mass * (r * radius_sonic_point) ** 2 / k2 \
-        - 3 * grav * star_mass * radius_sonic_point ** 2 / k2 + 0.5 - \
+    k2 = sound_speed_0 ** 2 * radius_sonic_point
+    k3 = 2 * semi_major_axis ** 3 * sound_speed_0 ** 2
+    density_r = np.exp(grav * planet_mass / k1 - grav * planet_mass / k2 \
+        + 3 * grav * star_mass * (r * radius_sonic_point) ** 2 / k3 \
+        - 3 * grav * star_mass * radius_sonic_point ** 2 / k3 + 0.5 - \
         np.array(velocity_r) ** 2 / 2)
 
     return velocity_r, density_r
```

### Comparing `p_winds-1.4.1b0/p_winds/tools.py` & `p_winds-1.4.4b0/p_winds/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 
 def nearest_index(array, target_value):
     """
     Finds the index of a value in ``array`` that is closest to ``target_value``.
 
     Parameters
     ----------
-    array (``numpy.array``):
+    array : ``numpy.array``
         Target array.
-    target_value (``float``):
+    target_value : ``float``
         Target value.
 
     Returns
     -------
-    index (``int``):
+    index : ``int``
         Index of the value in ``array`` that is closest to ``target_value``.
     """
     index = array.searchsorted(target_value)
     index = np.clip(index, 1, len(array) - 1)
     left = array[index - 1]
     right = array[index]
     index -= target_value - left < right - target_value
@@ -47,47 +47,47 @@
     Construct a dictionary containing an input spectrum from a MUSCLES spectrum.
     MUSCLES reports spectra as observed at Earth, the code scales this to the
     spectrum received at your planet provided a value for the scaled semi-major
     axis a_rs.
 
     Parameters
     ----------
-    host_star_name (``str``):
+    host_star_name : ``str``
         Name of the MUSCLES stellar spectrum you want to use. Must be one of:
         ['gj176', 'gj436', 'gj551', 'gj581', 'gj667c', 'gj832', 'gj876',
         'gj1214', 'hd40307', 'hd85512', 'hd97658', 'v-eps-eri'].
 
-    muscles_dir (``str``):
+    muscles_dir : ``str``
         Path to the directory with the MUSCLES data.
 
-    semi_major_axis (``float``):
+    semi_major_axis : ``float``
         Semi-major axis of the planet in units of stellar radii. The code first
         converts the MUSCLES spectrum to what it would be at R_star;
         ``semi_major_axis`` is needed to get the spectrum at the planet.
 
-    stellar_radius (``float``, optional):
+    stellar_radius : ``float``, optional
         Stellar radius in unit of solar radii. Setting a value for this
         parameter allows the spectrum to be scaled to an arbitrary stellar
         radius instead of the radius of the MUSCLES star. If ``None``, then the
         scaling is performed using the radius of the MUSCLES star. Default is
         ``None``.
 
-    truncate_wavelength_grid (``bool``, optional):
+    truncate_wavelength_grid : ``bool``, optional
         If ``True``, will only return the spectrum with energy > 13.6 eV. This
         may be useful for computational expediency. If False, returns the whole
         spectrum. Default is ``False``.
 
-    cutoff_thresh (`float`, optional):
+    cutoff_thresh : ``float``, optional
         If ``truncate_wavelength_grid`` is set to ``True``, then the truncation
         happens for energies whose value in eV is above this threshold, also in
         eV. Default is ``13.6``.
 
     Returns
     -------
-    spectrum (``dict``):
+    spectrum : ``dict``
         Spectrum dictionary with entries for the wavelength and flux, and their
         units.
     """
     # Hard coding some values
     # The stellar radii and distances are taken from NASA Exoplanet Archive.
 
     thresh = cutoff_thresh * u.eV
@@ -130,46 +130,62 @@
                 semi_major_axis ** (-2),
                 'wavelength_unit': u.AA,
                 'flux_unit': u.erg / u.s / u.cm / u.cm / u.AA}
     return spectrum
 
 
 def make_spectrum_from_file(filename, units, path='', skiprows=0,
-                            scale_flux=1.0):
+                            scale_flux=1.0, star_distance=None,
+                            semi_major_axis=None):
     """
     Construct a dictionary containing an input spectrum from a text file. The
     input file must have two or more columns, in which the first is the
     wavelength or frequency bin center and the second is the flux per bin of
     wavelength or frequency. The code automatically figures out if the input
     spectra are binned in wavelength or frequency based on the units the user
     passes.
 
     Parameters
     ----------
-    filename (``str``):
+    filename : ``str``
         Name of the file containing the spectrum data.
 
-    units (``dict``):
+    units : ``dict``
         Units of the spectrum. This dictionary must have the entries
         ``'wavelength'`` and ``'flux'``, or ``'frequency'`` and ``'flux'``.
         The units must be set in ``astropy.units``.
 
-    path (``str``, optional):
+    path : ``str``, optional
         Path to the spectrum data file.
 
-    skiprows (``int``, optional):
+    skiprows : ``int``, optional
         Number of rows to skip corresponding to the header of the input text
         file.
 
-    scale_flux (``float``, optional):
+    scale_flux : ``float``, optional
         Scaling factor for flux. Default value is 1.0 (no scaling).
 
+    star_distance : ``float`` or ``None``, optional
+        Distance to star in unit of parsec. This is used to scale the flux as
+        observed from Earth to the semi-major axis of the planet. If ``None``,
+        no scaling is applied. If not ``None``, then a value``semi_major_axis``
+        must be provided as well. Default is ``None``.
+
+    semi_major_axis : ``float`` or ``None``, optional
+        Semi-major axis of the planet in unit of au. This is used to scale the
+        flux as observed from Earth to the semi-major axis of the planet. Notice
+        that this parameter is different from the
+        ``generate_muscles_spectrum()``  function, which uses the semi-major
+        axis in unit of stellar radii. If ``None``, no scaling is applied. If
+        not ``None``, then a value``star_distance`` must be provided as well.
+        Default is ``None``.
+
     Returns
     -------
-    spectrum (``dict``):
+    spectrum : ``dict``
         Spectrum dictionary with entries for the wavelength and flux, and their
         units.
 
     """
     spectrum_table = np.loadtxt(path + filename, usecols=(0, 1),
                                 skiprows=skiprows, dtype=float)
 
@@ -179,12 +195,19 @@
         y_axis = 'flux_lambda'
     except KeyError:
         x_axis = 'frequency'
         x_axis_unit = units.pop(x_axis)
         y_axis = 'flux_nu'
     y_axis_unit = units.pop('flux')
 
+    conv_pc_to_au = 206264.8062471  # Conversion from pc to au
+    if star_distance is not None and semi_major_axis is not None:
+        scale_to_planet = \
+            (star_distance * conv_pc_to_au / semi_major_axis) ** (-2)
+    else:
+        scale_to_planet = 1.0
+
     spectrum = {x_axis: spectrum_table[:, 0],
-                y_axis: spectrum_table[:, 1] * scale_flux,
+                y_axis: spectrum_table[:, 1] * scale_flux * scale_to_planet,
                 '{}_unit'.format(x_axis): x_axis_unit,
                 'flux_unit': y_axis_unit}
     return spectrum
```

### Comparing `p_winds-1.4.1b0/p_winds/transit.py` & `p_winds-1.4.4b0/p_winds/transit.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This module is used to compute a grid containing drawing of disks of stars,
 planets and atmospheres.
 """
 
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.special import voigt_profile
-from scipy.integrate import simps
+from scipy.integrate import trapz
 from flatstar import draw, utils
 
 
 __all__ = ["draw_transit", "radiative_transfer_2d", "profile_los",
            "optical_depth_2d"]
 
 
@@ -23,68 +23,68 @@
                  limb_darkening_law=None, ld_coefficient=None):
     """
     Calculate a normalized transit map. Additionally, calculate two-dimensional
     arrays of density and line-of-sight radial velocities around the planet.
 
     Parameters
     ----------
-    planet_to_star_ratio (``float``):
+    planet_to_star_ratio : ``float``
         Ratio between the radii of the planet and the star.
 
-    planet_physical_radius (``float``):
+    planet_physical_radius : ``float``
         Physical radius of the planet in whatever unit you want to work with.
 
-    impact_parameter (``float``, optional):
+    impact_parameter : ``float``, optional
         Transit impact parameter of the planet (not the atmosphere). Default is
         0.0.
 
-    phase (``float``, optional):
+    phase : ``float``, optional
         Phase of the transit. -0.5, 0.0, and +0.5 correspond to the center of
         planet being located at, respectively, the left limb of the star, the
         center, and the right limb. Default is 0.0.
 
-    grid_size (``int``, optional):
+    grid_size : ``int``, optional
         Size of the transit grid. Default is 100.
 
-    supersampling (``float`` or ``None``, optional):
+    supersampling : ``float`` or ``None``, optional
         In order to avoid pixels with hard edges, it is useful to first compute
         the transit grid at a high resolution and then downscale it to a
         manageable grid size. Supersampling is the factor by which to increase
         the grid size at first and then downscale to the requested grid size. If
         ``None``, no supersampling is applied. Default is ``None``.
 
-    resample_method (``str`` or ``None``, optional):
+    resample_method : ``str`` or ``None``, optional
         Method by which to resample the image if supersampling is used. If
         ``None``, then fallback to a "box" method. Available methods are
         ``"nearest"``, ``"box"``, ``"bilinear"``, ``"hamming"`` and
         ``"lanczos"`` (the last two are not recommended for research-grade
         results. Default is ``None``.
 
-    limb_darkening_law (``None`` or ``str``, optional):
+    limb_darkening_law : ``None`` or ``str``, optional
         String with the name of the limb-darkening law. The options are the same
         currently implemented in the code ``flatstar``: ``'linear'``,
         ``'quadratic'``, ``'square-root'``, ``'log'``, ``'exp'``, ``'s3'``,
         ``'c4'``, or ``None`` (no limb-darkening). Default is ``None``.
 
-    ld_coefficient (``float`` or ``array-like``):
+    ld_coefficient : ``float`` or ``array-like``
         In case of a linear limb-darkening law, the value of the coefficient
         should be a float. In all other options it should be array-like. Default
         is ``None``.
 
     Returns
     -------
-    normalized_intensity_map (``numpy.ndarray``):
+    normalized_intensity_map : ``numpy.ndarray``
         2-D map of intensity normalized in such a way that the sum of the array
         will be 1.0 if the planet is not transiting.
 
-    transit_depth (``float``):
+    transit_depth : ``float``
         Absorption caused by the opaque disk of the planet in the specified
         transit configuration.
 
-    r_from_planet (``numpy.ndarray``):
+    r_from_planet : ``numpy.ndarray``
         2-D map of radial distances of each pixel from the center of the planet
         in the same unit as ``planet_physical_radius``.
     """
     if supersampling is not None:
         effective_grid_size = int(round(grid_size * supersampling))
         rescaling = 1 / supersampling
     else:
@@ -118,100 +118,105 @@
 
 # Calculate the radiative transfer
 def radiative_transfer_2d(intensity_0, r_from_planet, radius_profile,
                           density_profile, velocity_profile, central_wavelength,
                           oscillator_strength, einstein_coefficient,
                           wavelength_grid, gas_temperature, particle_mass,
                           bulk_los_velocity=0.0, planet_radial_velocity=0.0,
-                          wind_broadening_method='average',
+                          wind_broadening_method='average', z_grid_size=200,
                           turbulence_broadening=False):
     """
     Calculate the absorbed intensity profile in a wavelength grid.
 
     Parameters
     ----------
-    intensity_0 (``float`` or ``numpy.ndarray``):
+    intensity_0 : ``float`` or ``numpy.ndarray``
         Original flux intensity originating from a background illuminating
         source. If ``numpy.ndarray``, must have the same shape as
         ``r_from_planet``.
 
-    r_from_planet (``numpy.ndarray``):
+    r_from_planet : ``numpy.ndarray``
         2-D map of radial distances of each pixel from the center of the planet.
         The unit has to be consistent with the other input parameters. E.g., if
         you use unit of meters, all other input parameters with length in the
         unit also have to be in meters.
 
-    radius_profile (``numpy.ndarray``):
+    radius_profile : ``numpy.ndarray``
         1-D profile of radii in which the densities are sampled. Unit has to be
         the same as ``r_from_planet``.
 
-    density_profile (``numpy.ndarray``):
+    density_profile : ``numpy.ndarray``
         1-D profile of volumetric number densities in function of radius. Unit
         has to be 1 / length ** 3, where length is the same unit as
         ``r_from_planet``.
 
-    velocity_profile (``numpy.ndarray``):
+    velocity_profile : ``numpy.ndarray``
         1-D profile of velocities in function of radius. Unit has to be
         m / s.
 
-    central_wavelength (``float`` or ``array_like``):
+    central_wavelength : ``float`` or ``array_like``
         Central wavelength of the transition in unit of m. If more than one line
         is to be calculated, then input this parameter as an array-like object.
 
-    oscillator_strength (``float``):
+    oscillator_strength : ``float``
         Oscillator strength of the transition. The format or shape of this input
         parameter needs to be consistent with that of ``central_wavelength``.
 
-    einstein_coefficient (``float``):
+    einstein_coefficient : ``float``
         Einstein coefficient of the transition in 1 / s. The format or shape of
         this input parameter needs to be consistent with that of
         ``central_wavelength``.
 
-    wavelength_grid (``numpy.ndarray``):
+    wavelength_grid : ``numpy.ndarray``
         Wavelengths to calculate the profile in unit of m.
 
-    gas_temperature (``float``):
+    gas_temperature : ``float``
         Gas temperature in K.
 
-    particle_mass (``float``):
+    particle_mass : ``float``
         Mass of the particle corresponding to the transition in unit of kg.
 
-    bulk_los_velocity (``float``, optional):
+    bulk_los_velocity : ``float``, optional
         Bulk velocity of the gas cell in the line of sight in unit of m / s.
         Default is 0.0.
 
-    planet_radial_velocity (``float``, optional):
+    planet_radial_velocity : ``float``, optional
         Radial velocity (i.e., the component in the line of sight) of the planet
         in relation to the rest frame of the host star and in unit of m / s.
         Default is 0.0.
 
-    wind_broadening_method (``str``, optional):
+    wind_broadening_method : ``str``, optional
         Method of calculation for the wind broadening. There are two options:
         1) ``'formal'``: the formal definition of radiative transfer taking into
         account the full dimensionality of the wind (slower);
         2) ``'average'``: assumes the Parker wind broadening contributes to the
         Gaussian term of the Voigt profile with an additive factor proportional
         to the square of the density-averaged, line-of-sight velocity (faster).
 
-    turbulence_broadening (``bool``, optional):
+    z_grid_size : ``int``, optional
+        Grid size for the line of sight direction. This is used only if
+        ``wind_broadening_method`` is set to ``'formal'``. Default is 200.
+
+    turbulence_broadening : ``bool``, optional
         If ``True``, adds a turbulence broadening, defined as in Lampón et al.
         2020, to the Gaussian term of the Voigt profile. Default is ``False``.
 
     Returns
     -------
-    intensity (``numpy.ndarray``):
+    intensity : ``numpy.ndarray``
         Absorbed intensity profile in function of ``wavelength_grid``.
     """
     # First, calculate the optical depth in function of radial distance from the
     # planet and the wavelength
     optical_depth_profile = optical_depth_2d(
         radius_profile, density_profile, velocity_profile, central_wavelength,
         oscillator_strength, einstein_coefficient, wavelength_grid,
-        gas_temperature, particle_mass, bulk_los_velocity,
-        planet_radial_velocity, wind_broadening_method, turbulence_broadening
+        gas_temperature, particle_mass, z_grid_size, bulk_los_velocity,
+        planet_radial_velocity, wind_broadening_method,
+        turbulence_broadening
     )
 
     # Now we interpolate the optical depths to each radius from the planet
     f = interp1d(radius_profile, optical_depth_profile, axis=0,
                  bounds_error=False, fill_value=0.0)
     optical_depth_array = f(r_from_planet)
 
@@ -221,42 +226,44 @@
     # Finally calculate the radiative transfer
     intensity = np.sum(intensity_0 * np.exp(-optical_depth_array), axis=(0, 1))
 
     return intensity
 
 
 # Density and velocity profiles in the line of sight
-def profile_los(radius_profile, density_profile, velocity_profile,
-                z_grid_size=200):
+def profile_los(radius_profile, density_profile, velocity_profile, z_grid_size):
     """
     Calculate the profiles of radius and line-of-sight velocities in function of
     sky-projected radial distance from the planet (axis 0) and the line of sight
     direction (axis 1).
 
     Parameters
     ----------
-    radius_profile (``numpy.ndarray``):
+    radius_profile : ``numpy.ndarray``
         1-D profile of radii in which the densities are sampled, in whatever
         unit you want to work with.
 
-    density_profile (``numpy.ndarray``):
+    density_profile : ``numpy.ndarray``
         1-D profile of volumetric number densities in function of radius, in
         whatever unit you want to work with.
 
-    velocity_profile (``numpy.ndarray``):
+    velocity_profile : ``numpy.ndarray``
         1-D profile of velocities in function of radius, in whatever unit you
         want to work with.
 
+    z_grid_size : ``int``, optional
+        Grid size for the line of sight direction.
+
     Returns
     -------
-    los_density_r_z (``numpy.ndarray``):
+    los_density_r_z : ``numpy.ndarray``
         2-D map of densities in the x- and z-axis distances from the center of
         the planet.
 
-    los_velocity_r_z (``numpy.ndarray``):
+    los_velocity_r_z : ``numpy.ndarray``
         2-D map of line-of-sight velocities in the x- and z-axis distances from
         the center of the planet.
     """
     # Create a two-dimensional array that measures the distance from the planet
     # The second dimension is the line-of-sight direction.
     r_top_atm = radius_profile[-1]
     los_z = np.linspace(-r_top_atm, r_top_atm, z_grid_size)
@@ -285,91 +292,95 @@
 
 
 # Optical depth in function of cylindrical radius from the planet and
 # wavelength. Hold on to your hat because this code is very complex.
 def optical_depth_2d(radius_profile, density_profile, velocity_profile,
                      central_wavelength, oscillator_strength,
                      einstein_coefficient, wavelength_grid, gas_temperature,
-                     particle_mass, bulk_los_velocity=0.0,
+                     particle_mass, z_grid_size, bulk_los_velocity=0.0,
                      planet_radial_velocity=0.0,
                      wind_broadening_method='average',
                      turbulence_broadening=False):
     """
     Calculate the optical depth in function of cylindrical radius from the
     planet and the wavelength.
 
     Parameters
     ----------
-    radius_profile (``numpy.ndarray``):
+    radius_profile : ``numpy.ndarray``
         1-D profile of radii in which the densities are sampled. Unit has to be
         consistent with the other input parameters involving lenghts and
         densities.
 
-    density_profile (``numpy.ndarray``):
+    density_profile : ``numpy.ndarray``
         1-D profile of volumetric number densities in function of radius. Unit
         has to be 1 / length ** 3, where length is the same unit as
         ``radius_profile``.
 
-    velocity_profile (``numpy.ndarray``):
+    velocity_profile : ``numpy.ndarray``
         1-D profile of velocities in function of radius. Unit has to be
         m / s.
 
-    central_wavelength (``float`` or ``array_like``):
+    central_wavelength : ``float`` or ``array_like``
         Central wavelength of the transition in unit of m. If more than one line
         is to be calculated, then input this parameter as an array-like object.
 
-    oscillator_strength (``float``):
+    oscillator_strength : ``float``
         Oscillator strength of the transition. The format or shape of this input
         parameter needs to be consistent with that of ``central_wavelength``.
 
-    einstein_coefficient (``float``):
+    einstein_coefficient : ``float``
         Einstein coefficient of the transition in 1 / s. The format or shape of
         this input parameter needs to be consistent with that of
         ``central_wavelength``.
 
-    wavelength_grid (``numpy.ndarray``):
+    wavelength_grid : ``numpy.ndarray``
         Wavelengths to calculate the profile in unit of m.
 
-    gas_temperature (``float``):
+    gas_temperature : ``float``
         Gas temperature in K.
 
-    particle_mass (``float``):
+    particle_mass : ``float``
         Mass of the particle corresponding to the transition in unit of kg.
 
-    bulk_los_velocity (``float``, optional):
+    z_grid_size : ``int``, optional
+        Grid size for the line of sight direction.
+
+    bulk_los_velocity : ``float``, optional
         Bulk velocity of the gas cell in the line of sight in unit of m / s.
         Default is 0.0.
 
-    planet_radial_velocity (``float``, optional):
+    planet_radial_velocity : ``float``, optional
         Radial velocity (i.e., the component in the line of sight) of the planet
         in relation to the rest frame of the host star and in unit of m / s.
         Default is 0.0.
 
-    wind_broadening_method (``str``, optional):
+    wind_broadening_method : ``str``, optional
         Method of calculation for the wind broadening. There are two options:
         1) ``'formal'``: the formal definition of radiative transfer taking into
         account the full dimensionality of the wind (slower);
         2) ``'average'``: assumes the Parker wind broadening contributes to the
         Gaussian term of the Voigt profile with an additive factor proportional
         to the square of the density-averaged, line-of-sight velocity (faster).
 
-    turbulence_broadening (``bool``, optional):
+    turbulence_broadening : ``bool``, optional
         If ``True``, adds a turbulence broadening, defined as in Lampón et al.
         2020, to the Gaussian term of the Voigt profile. Only used if
         ``wind_broadening_method`` is set to ``'average'``. Default is ``False``.
 
     Returns
     -------
-    optical_depth_array (``numpy.ndarray``):
+    optical_depth_array : ``numpy.ndarray``
         Optical depth in function of radial distance from the center of the
         planet (axis 0) and in function of wavelength (axis 1).
     """
     # Calculate density and velocity profiles in the line of sight
     density_los, velocity_los, z_los = \
-        profile_los(radius_profile, density_profile, velocity_profile)
+        profile_los(radius_profile, density_profile, velocity_profile,
+                    z_grid_size)
     spatial_shape = np.shape(density_los)
 
     # Spectral line properties
     w0 = central_wavelength  # Reference wavelength in m
     f = oscillator_strength  # Unit-less
     a_ij = einstein_coefficient  # In unit of 1 / s
 
@@ -465,15 +476,15 @@
         # Finally calculate the Voigt profiles
         profiles = voigt_profile(delta_nu_grid + delta_nu_add, alpha_nu,
                                  gamma)
 
         # Calculate the optical depths divided by the cross section
         density_expanded = np.expand_dims(density_los, axis=-1)
         opt_depth_over_cross_section_r_nu = \
-            simps(profiles * density_expanded, z_los, axis=0)
+            trapz(profiles * density_expanded, z_los, axis=0)
 
         return opt_depth_over_cross_section_r_nu
 
     # Calculate the optical depth for each line
     optical_depth_list = []
     for i in range(n_lines):
         norm_opt_depth = _normalized_optical_depth(
```

### Comparing `p_winds-1.4.1b0/setup.py` & `p_winds-1.4.4b0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist upload")
     sys.exit()
 
 setup(
     name="p_winds",
-    version="1.4.1b",
+    version="1.4.4b",
     author="Leonardo dos Santos",
     author_email="ldsantos@stsci.edu",
     packages=["p_winds"],
     url="https://github.com/ladsantos/p-winds",
     license="MIT",
     description="Parker wind models for planetary atmospheres",
     install_requires=[line.strip() for line in
```

