# Comparing `tmp/arte-0.5.0.tar.gz` & `tmp/arte-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arte-0.5.0.tar", last modified: Thu Nov 17 12:15:09 2022, max compression
+gzip compressed data, was "arte-0.6.0.tar", last modified: Tue Apr 11 08:04:07 2023, max compression
```

## Comparing `arte-0.5.0.tar` & `arte-0.6.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.753471 arte-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-11-17 12:14:57.000000 arte-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-11-17 12:15:09.753471 arte-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-11-17 12:14:57.000000 arte-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.745471 arte-0.5.0/arte/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 12:14:57.000000 arte-0.5.0/arte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-17 12:14:57.000000 arte-0.5.0/arte/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.745471 arte-0.5.0/arte/atmo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 12:14:57.000000 arte-0.5.0/arte/atmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18486 2022-11-17 12:14:57.000000 arte-0.5.0/arte/atmo/cn2_profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     4099 2022-11-17 12:14:57.000000 arte-0.5.0/arte/atmo/phase_screen_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-11-17 12:14:57.000000 arte-0.5.0/arte/atmo/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    32871 2022-11-17 12:14:57.000000 arte-0.5.0/arte/atmo/von_karman_covariance_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4698 2022-11-17 12:14:57.000000 arte-0.5.0/arte/atmo/von_karman_psd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-11-17 12:14:57.000000 arte-0.5.0/arte/atmo/von_karman_spatial_covariance_calculator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-11-17 12:14:57.000000 arte-0.5.0/arte/code_convention.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.745471 arte-0.5.0/arte/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 12:14:57.000000 arte-0.5.0/arte/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-11-17 12:14:57.000000 arte-0.5.0/arte/contrib/chunk_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8748 2022-11-17 12:14:57.000000 arte-0.5.0/arte/contrib/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-11-17 12:14:57.000000 arte-0.5.0/arte/contrib/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-11-17 12:14:57.000000 arte-0.5.0/arte/contrib/if_.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-11-17 12:14:57.000000 arte-0.5.0/arte/contrib/interpolated_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-11-17 12:14:57.000000 arte-0.5.0/arte/contrib/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-11-17 12:14:57.000000 arte-0.5.0/arte/contrib/yes_no.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.745471 arte-0.5.0/arte/control/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 12:14:57.000000 arte-0.5.0/arte/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7804 2022-11-17 12:14:57.000000 arte-0.5.0/arte/control/transfer_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.745471 arte-0.5.0/arte/math/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 12:14:57.000000 arte-0.5.0/arte/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-11-17 12:14:57.000000 arte-0.5.0/arte/math/factors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6731 2022-11-17 12:14:57.000000 arte-0.5.0/arte/math/make_xy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-11-17 12:14:57.000000 arte-0.5.0/arte/math/masks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-11-17 12:14:57.000000 arte-0.5.0/arte/math/toccd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.745471 arte-0.5.0/arte/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 12:14:57.000000 arte-0.5.0/arte/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9776 2022-11-17 12:14:57.000000 arte-0.5.0/arte/misc/fourier_adaptive_optics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.749471 arte-0.5.0/arte/photometry/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-17 12:14:57.000000 arte-0.5.0/arte/photometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-11-17 12:14:57.000000 arte-0.5.0/arte/photometry/eso_sky_calc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4087 2022-11-17 12:14:57.000000 arte-0.5.0/arte/photometry/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5381 2022-11-17 12:14:57.000000 arte-0.5.0/arte/photometry/mag_estimator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10318 2022-11-17 12:14:57.000000 arte-0.5.0/arte/photometry/n_phot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2243 2022-11-17 12:14:57.000000 arte-0.5.0/arte/photometry/normalized_star_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     4210 2022-11-17 12:14:57.000000 arte-0.5.0/arte/photometry/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     3594 2022-11-17 12:14:57.000000 arte-0.5.0/arte/photometry/spectral_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8596 2022-11-17 12:14:57.000000 arte-0.5.0/arte/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     5455 2022-11-17 12:14:57.000000 arte-0.5.0/arte/sandbox_noise_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.749471 arte-0.5.0/arte/time_series/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-11-17 12:14:57.000000 arte-0.5.0/arte/time_series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3210 2022-11-17 12:14:57.000000 arte-0.5.0/arte/time_series/indexer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3929 2022-11-17 12:14:57.000000 arte-0.5.0/arte/time_series/multi_time_series.py
--rw-r--r--   0 runner    (1001) docker     (121)    12730 2022-11-17 12:14:57.000000 arte-0.5.0/arte/time_series/time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.749471 arte-0.5.0/arte/types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/aperture.py
--rw-r--r--   0 runner    (1001) docker     (121)    10171 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/domainxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/fisba_measure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/guide_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     6995 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/mask.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5221 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/scalar_bidimensional_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/slopes.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/wavefront.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-11-17 12:14:57.000000 arte-0.5.0/arte/types/zernike_coefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.753471 arte-0.5.0/arte/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/capture_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/circular_buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/circular_range.py
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/compareIDL.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     7700 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/discrete_fourier_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     8411 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    11869 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/footprint_geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/generalized_fitting_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     6259 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)     7970 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/help.py
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/image_moments.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/locate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/marechal.py
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/modal_decomposer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/multiton.py
--rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/noise_propagation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4640 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/not_available.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/package_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/quadratic_sum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/radial_profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2990 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/rebin.py
--rw-r--r--   0 runner    (1001) docker     (121)     7726 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/shape_fitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/shared_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     4885 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/tabular_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/timekeepers.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (121)     6856 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/unit_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)    13085 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/zernike_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4006 2022-11-17 12:14:57.000000 arte-0.5.0/arte/utils/zernike_projection_on_subaperture.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.745471 arte-0.5.0/arte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-11-17 12:15:09.000000 arte-0.5.0/arte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-11-17 12:15:09.000000 arte-0.5.0/arte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 12:15:09.000000 arte-0.5.0/arte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-17 12:15:09.000000 arte-0.5.0/arte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-17 12:15:09.000000 arte-0.5.0/arte.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 12:15:09.753471 arte-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2901 2022-11-17 12:14:57.000000 arte-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 12:15:09.753471 arte-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)    16926 2022-11-17 12:14:57.000000 arte-0.5.0/test/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.386244 arte-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-11 08:03:43.000000 arte-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-11 08:04:07.386244 arte-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-11 08:03:43.000000 arte-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.378244 arte-0.6.0/arte/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:03:43.000000 arte-0.6.0/arte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 08:03:43.000000 arte-0.6.0/arte/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.378244 arte-0.6.0/arte/atmo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:43.000000 arte-0.6.0/arte/atmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18467 2023-04-11 08:03:43.000000 arte-0.6.0/arte/atmo/cn2_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-11 08:03:43.000000 arte-0.6.0/arte/atmo/phase_screen_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-11 08:03:43.000000 arte-0.6.0/arte/atmo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32871 2023-04-11 08:03:43.000000 arte-0.6.0/arte/atmo/von_karman_covariance_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-11 08:03:43.000000 arte-0.6.0/arte/atmo/von_karman_psd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-11 08:03:43.000000 arte-0.6.0/arte/atmo/von_karman_spatial_covariance_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-11 08:03:43.000000 arte-0.6.0/arte/code_convention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.378244 arte-0.6.0/arte/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:43.000000 arte-0.6.0/arte/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-11 08:03:43.000000 arte-0.6.0/arte/contrib/chunk_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-04-11 08:03:43.000000 arte-0.6.0/arte/contrib/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-11 08:03:43.000000 arte-0.6.0/arte/contrib/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-11 08:03:43.000000 arte-0.6.0/arte/contrib/if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-11 08:03:43.000000 arte-0.6.0/arte/contrib/interpolated_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 08:03:43.000000 arte-0.6.0/arte/contrib/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 08:03:43.000000 arte-0.6.0/arte/contrib/yes_no.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.378244 arte-0.6.0/arte/control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:43.000000 arte-0.6.0/arte/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-11 08:03:43.000000 arte-0.6.0/arte/control/transfer_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.378244 arte-0.6.0/arte/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:43.000000 arte-0.6.0/arte/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-11 08:03:43.000000 arte-0.6.0/arte/math/factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-11 08:03:43.000000 arte-0.6.0/arte/math/make_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-11 08:03:43.000000 arte-0.6.0/arte/math/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-11 08:03:43.000000 arte-0.6.0/arte/math/toccd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.382244 arte-0.6.0/arte/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:43.000000 arte-0.6.0/arte/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-04-11 08:03:43.000000 arte-0.6.0/arte/misc/fourier_adaptive_optics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.382244 arte-0.6.0/arte/photometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 08:03:43.000000 arte-0.6.0/arte/photometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-11 08:03:43.000000 arte-0.6.0/arte/photometry/eso_sky_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-11 08:03:43.000000 arte-0.6.0/arte/photometry/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-11 08:03:43.000000 arte-0.6.0/arte/photometry/mag_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-11 08:03:43.000000 arte-0.6.0/arte/photometry/n_phot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-11 08:03:43.000000 arte-0.6.0/arte/photometry/normalized_star_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-11 08:03:43.000000 arte-0.6.0/arte/photometry/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-11 08:03:43.000000 arte-0.6.0/arte/photometry/spectral_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-04-11 08:03:43.000000 arte-0.6.0/arte/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-11 08:03:43.000000 arte-0.6.0/arte/sandbox_noise_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.382244 arte-0.6.0/arte/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-11 08:03:43.000000 arte-0.6.0/arte/time_series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-11 08:03:43.000000 arte-0.6.0/arte/time_series/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-11 08:03:43.000000 arte-0.6.0/arte/time_series/multi_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12730 2023-04-11 08:03:43.000000 arte-0.6.0/arte/time_series/time_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.382244 arte-0.6.0/arte/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/domainxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/fisba_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/guide_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/scalar_bidimensional_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/slopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/wavefront.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-11 08:03:43.000000 arte-0.6.0/arte/types/zernike_coefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.386244 arte-0.6.0/arte/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/capture_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/circular_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/circular_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/compareIDL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/discrete_fourier_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11868 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/footprint_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/generalized_fitting_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/image_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/locate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/marechal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/modal_decomposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/multiton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/noise_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/not_available.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/package_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/quadratic_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/radial_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/rebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/shape_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/shared_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/tabular_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/timekeepers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/unit_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/zernike_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-11 08:03:43.000000 arte-0.6.0/arte/utils/zernike_projection_on_subaperture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.378244 arte-0.6.0/arte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-11 08:04:07.000000 arte-0.6.0/arte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-11 08:04:07.000000 arte-0.6.0/arte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:04:07.000000 arte-0.6.0/arte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 08:04:07.000000 arte-0.6.0/arte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 08:04:07.000000 arte-0.6.0/arte.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:04:07.386244 arte-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-11 08:03:43.000000 arte-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:07.386244 arte-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-04-11 08:03:43.000000 arte-0.6.0/test/test_helper.py
```

### Comparing `arte-0.5.0/LICENSE` & `arte-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/PKG-INFO` & `arte-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arte
-Version: 0.5.0
+Version: 0.6.0
 Summary: Arcetri Random sTuff collEction
 Home-page: https://github.com/ArcetriAdaptiveOptics/arte
 Author: Lorenzo Busoni, Alfio Puglisi, INAF Arcetri Adaptive Optics group
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: Adaptive Optics, Astrophysics, INAF, Arcetri
 Classifier: Development Status :: 4 - Beta
```

### Comparing `arte-0.5.0/README.md` & `arte-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/atmo/cn2_profile.py` & `arte-0.6.0/arte/atmo/cn2_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         & = & \big( \sum{0.423 X k^2 J_i} \big)^{-3/5} \\
     \theta_0 & = & \big( 2.914 k^2 X^{8/3} \sum{J_i h_i^{5/3}} \big)^{-3/5} 
    \end{eqnarray}
 
 '''
 import numpy as np
 from astropy.units.quantity import Quantity
-from arte.utils.constants import Constants
+from arte.utils.constants import DEG2RAD, RAD2ARCSEC
 from arte.utils.package_data import dataRootDir
 import os
 from astropy.io import fits
 import astropy.units as u
 from astropy.utils.misc import isiterable
 
 
@@ -225,15 +225,15 @@
 
     @staticmethod
     def zenith_angle_to_airmass(zenithAngleInDeg):
         if isinstance(zenithAngleInDeg, Quantity):
             value = zenithAngleInDeg.to(u.deg).value
         else:
             value = zenithAngleInDeg
-        zenithInRad = value * Constants.DEG2RAD
+        zenithInRad = value * DEG2RAD
         return 1. / np.cos(zenithInRad)
 
     def airmass(self):
         '''
         Returns
         -------
         airmass: float
@@ -305,15 +305,15 @@
         """
         Returns
         -------
         seeing: :class:`~astropy:astropy.units.quantity.Quantity` equivalent to arcsec
             seeing value at specified lambda and zenith angle
             defined as 0.98 * lambda / r0
         """
-        return 0.98 * self.wavelength() / self.r0() * Constants.RAD2ARCSEC * \
+        return 0.98 * self.wavelength() / self.r0() * RAD2ARCSEC * \
             u.arcsec
 
     def r0(self):
         '''
         Returns
         -------
         r0: :class:`~astropy:astropy.units.quantity.Quantity` equivalent to meters
@@ -340,15 +340,15 @@
             theta0 (float): isoplanatic angle at specified lambda and zenith
                 angle [arcsec]
         '''
         return (2.914 * self._airmass ** (8. / 3) *
                 (2 * np.pi / self._lambda) ** 2 *
                 np.sum(self._layersJs *
                        self._layersAltitudeInMeterAtZenith ** (5. / 3))
-                ) ** (-3. / 5) * Constants.RAD2ARCSEC * u.arcsec
+                ) ** (-3. / 5) * RAD2ARCSEC * u.arcsec
 
     def tau0(self):
         '''
         Returns:
             tau0 (float): tau0 at specified lambda and zenith angle [sec]
         '''
         return (2.914 * self._airmass *
@@ -544,8 +544,8 @@
         hs = np.array([0.03, 0.140, 0.281, 0.562, 1.125, 2.250, 4.500,
                        7.750, 11.000, 14.000]) * 1000
         js = [0.59, 0.02, 0.04, 0.06, 0.01, 0.05, 0.09, 0.04, 0.05, 0.05]
         windSpeed = [6.6, 5.9, 5.1, 4.5, 5.1, 8.3, 16.3, 30.2, 34.3, 17.5]
         windDirection = np.linspace(0, 360, len(js))
         L0s = np.ones(len(js)) * 22.
         return Cn2Profile.from_fractional_j(
-            r0, js, L0s, hs, windSpeed, windDirection)
+            r0, js, L0s, hs, windSpeed, windDirection)
```

### Comparing `arte-0.5.0/arte/atmo/phase_screen_generator.py` & `arte-0.6.0/arte/atmo/phase_screen_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             -11. / 12)
         mappa[0, 0] = 0
         return mappa
 
     def _generate_sub_harmonics(self, numberOfSubHarmonics):
         nSub = 3
         lowFreqScreen = np.zeros((self._screenSzInPx, self._screenSzInPx),
-                                 dtype=np.complex)
+                                 dtype=np.complex128)
         freqX = bfft.frequencies_x_map(nSub, 1. / nSub)
         freqY = bfft.frequencies_y_map(nSub, 1. / nSub)
         freqMod = bfft.frequencies_norm_map(nSub, 1. / nSub)
         vv = np.arange(self._screenSzInPx) / self._screenSzInPx
         xx = np.tile(vv, (self._screenSzInPx, 1))
         yy = xx.T
         depth = 0
```

### Comparing `arte-0.5.0/arte/atmo/von_karman_covariance_calculator.py` & `arte-0.6.0/arte/atmo/von_karman_covariance_calculator.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/atmo/von_karman_psd.py` & `arte-0.6.0/arte/atmo/von_karman_psd.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/atmo/von_karman_spatial_covariance_calculator.py` & `arte-0.6.0/arte/atmo/von_karman_spatial_covariance_calculator.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/code_convention.py` & `arte-0.6.0/arte/code_convention.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/contrib/chunk_iterator.py` & `arte-0.6.0/arte/contrib/chunk_iterator.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/contrib/daemonize.py` & `arte-0.6.0/arte/contrib/daemonize.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/contrib/debug.py` & `arte-0.6.0/arte/contrib/debug.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/contrib/if_.py` & `arte-0.6.0/arte/contrib/if_.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/contrib/interpolated_array.py` & `arte-0.6.0/arte/contrib/interpolated_array.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/contrib/timer.py` & `arte-0.6.0/arte/contrib/timer.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/contrib/yes_no.py` & `arte-0.6.0/arte/contrib/yes_no.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/control/transfer_function.py` & `arte-0.6.0/arte/control/transfer_function.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/math/make_xy.py` & `arte-0.6.0/arte/math/make_xy.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/math/masks.py` & `arte-0.6.0/arte/math/masks.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/math/toccd.py` & `arte-0.6.0/arte/math/toccd.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/misc/fourier_adaptive_optics.py` & `arte-0.6.0/arte/misc/fourier_adaptive_optics.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,28 +215,28 @@
                          ac.ymap)
 
     def _autoCorrelate(self, scalar2dfunct):
         functFT = bfft.direct(scalar2dfunct)
         aa = S2DF(np.abs(functFT.values ** 2),
                   functFT.xmap,
                   functFT.ymap)
-        return bfft.inverse(aa)
+        return bfft.reverse(aa)
 
     def _createPsf(self):
-        psf = bfft.inverse(self.otf())
+        psf = bfft.reverse(self.otf())
         rescaleCoordFact = 1 / self._focalLength
         self._psf = S2DF(np.abs(psf.values),
                          psf.xmap * rescaleCoordFact,
                          psf.ymap * rescaleCoordFact)
 
     def _createStructureFunction(self):
         extFieldMap = self._extendFieldMap(self.field(),
                                            self._resolutionFactor)
         ac = self._autoCorrelate(extFieldMap)
-        cc = (np.asarray(ac.shape) / 2).astype(np.int)
+        cc = (np.asarray(ac.shape) / 2).astype(np.int64)
         self._stf = 2 * (ac[cc[0], cc[1]] - ac)
 
     def _createFocalPlaneCoordinatesInArcSec(self):
         return bfft.distances_x_map(
             self.focalPlaneSizeInPixels(),
             self.focalPlanePixelSizeInArcsec())
```

### Comparing `arte-0.5.0/arte/photometry/eso_sky_calc.py` & `arte-0.6.0/arte/photometry/eso_sky_calc.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/photometry/filters.py` & `arte-0.6.0/arte/photometry/filters.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/photometry/mag_estimator.py` & `arte-0.6.0/arte/photometry/mag_estimator.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/photometry/n_phot.py` & `arte-0.6.0/arte/photometry/n_phot.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/photometry/normalized_star_spectrum.py` & `arte-0.6.0/arte/photometry/normalized_star_spectrum.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/photometry/sandbox.py` & `arte-0.6.0/arte/photometry/sandbox.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/photometry/spectral_types.py` & `arte-0.6.0/arte/photometry/spectral_types.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/sandbox.py` & `arte-0.6.0/arte/sandbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -221,7 +221,18 @@
 #         vCoord2 = self._getCleverVersorCoords(self._source2Coords)
 #         sep = self._layerAlt * vCoord2 / vCoord2[2] - \
 #             self._layerAlt * vCoord1 / vCoord1[2]
 #         return sep
 #
 #     def _getPhaseOfDMUntilStepN(self, ):
 #         pass
+
+
+
+    
+    
+    # Parsevals theorem with proper sample points
+    
+    #energy_t = np.sum(abs(f)**2, x=t)
+    #energy_f = np.trapz(abs(FFT)**2, x=frq) / N
+    
+    #print('Parsevals theorem NOT fulfilled: ' + str(energy_t - energy_f))
```

### Comparing `arte-0.5.0/arte/time_series/indexer.py` & `arte-0.6.0/arte/time_series/indexer.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/time_series/multi_time_series.py` & `arte-0.6.0/arte/time_series/multi_time_series.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/time_series/time_series.py` & `arte-0.6.0/arte/time_series/time_series.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/aperture.py` & `arte-0.6.0/arte/types/aperture.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/domainxy.py` & `arte-0.6.0/arte/types/domainxy.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/fisba_measure.py` & `arte-0.6.0/arte/types/fisba_measure.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/guide_source.py` & `arte-0.6.0/arte/types/guide_source.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/mask.py` & `arte-0.6.0/arte/types/mask.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/region_of_interest.py` & `arte-0.6.0/arte/types/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/scalar_bidimensional_function.py` & `arte-0.6.0/arte/types/scalar_bidimensional_function.py`

 * *Files 13% similar despite different names*

```diff
@@ -87,16 +87,39 @@
 
     @property
     def shape(self):
         '''(y,x) function shape'''
         return self._values.shape
 
     def interpolate_in_xy(self, x, y, span=3):
-        '''Interpolate the function value at x,y'''
-        return self._my_interp(x, y, span=3)
+        '''
+        Interpolate the function at points x,y
+
+        Returns an array of z[i] corresponding to the values interpolated
+        at points x[i], y[i]
+
+        The interpolation algorithm is linear and uses a box of 3x3 points
+        centered on the closest point to the interpolation coordinate
+
+
+        Parameters
+        ----------
+        x: numpy.ndarray or tuple with size N
+            1D array of the x coordinates of the sampling points
+
+        y: numpy.ndarray or tuple with size N
+            1D array of the y coordinates of the sampling points
+
+        Returns
+        -------
+        z: numpy.ndarray
+            array of shape (N,) of the sampled values. z[i] = interp(f, x[i], y[i]) 
+
+        '''
+        return self._my_interp(x, y, span=span)
 
     def get_radial_profile(self):
         '''Get the radial profile around the domain origin.
 
         Assumes that the domain sampling is the same in the X and Y
         directions
         '''
@@ -107,15 +130,15 @@
     def plot_radial_profile(self):
         import matplotlib.pyplot as plt
         y, x = self.get_radial_profile()
         plt.plot(x, y)
         plt.show()
 
     def _my_interp(self, x, y, span=3):
-        xs, ys = map(np.array, (x, y))
+        xs, ys = map(np.array, (np.atleast_1d(x), np.atleast_1d(y)))
         z = np.zeros(xs.shape)
         for i, (x, y) in enumerate(zip(xs, ys)):
             # get the indices of the nearest x,y
             box = self._domain.get_boundingbox_slice(x, y, span=span)
 
             # make slices of X,Y,Z that are only a few items wide
             nX = self._domain.xmap[box]
@@ -125,25 +148,24 @@
             if np.iscomplexobj(nZ):
                 z[i] = self._interp_complex(nX, nY, nZ, x, y)
             else:
                 z[i] = self._interp_real(nX, nY, nZ, x, y)
         return z
 
     def _interp_real(self, nX, nY, nZ, x, y):
-        # beware of https://github.com/scipy/scipy/issues/10268 !!! 
+        # beware of https://github.com/scipy/scipy/issues/10268 !!!
         # use 1D (nX[0] and nY[:,0]) instead of 2D nX and nY
-        intp = interpolate.interp2d(nX[0], nY[:,0], nZ, kind='linear')
+        intp = interpolate.interp2d(nX[0], nY[:, 0], nZ, kind='linear')
         return intp(x, y)[0]
 
     def _interp_complex(self, nX, nY, nZ, x, y):
-        intpr = interpolate.interp2d(nX[0], nY[:,0], nZ.real, kind='linear')
-        intpi = interpolate.interp2d(nX[0], nY[:,0], nZ.imag, kind='linear')
+        intpr = interpolate.interp2d(nX[0], nY[:, 0], nZ.real, kind='linear')
+        intpi = interpolate.interp2d(nX[0], nY[:, 0], nZ.imag, kind='linear')
         return intpr(x, y)[0] + 1j * intpi(x, y)[0]
 
     def get_roi(self, xmin, xmax, ymin, ymax):
 
         box = self._domain.get_crop_slice(xmin, xmax, ymin, ymax)
         cropped_values = self.values[box]
         cropped_domain = self._domain[box]
         return ScalarBidimensionalFunction(cropped_values,
                                            domain=cropped_domain)
-
```

### Comparing `arte-0.5.0/arte/types/slopes.py` & `arte-0.6.0/arte/types/slopes.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/wavefront.py` & `arte-0.6.0/arte/types/wavefront.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/types/zernike_coefficients.py` & `arte-0.6.0/arte/types/zernike_coefficients.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/capture_output.py` & `arte-0.6.0/arte/utils/capture_output.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/circular_buffer.py` & `arte-0.6.0/arte/utils/circular_buffer.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/compareIDL.py` & `arte-0.6.0/arte/utils/compareIDL.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/decorator.py` & `arte-0.6.0/arte/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/discrete_fourier_transform.py` & `arte-0.6.0/arte/utils/discrete_fourier_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             xmap=BidimensionalFourierTransform.frequencies_x_map(
                 sizeX, pxSizeX),
             ymap=BidimensionalFourierTransform.frequencies_y_map(
                 sizeY, pxSizeY)
         )
 
     @staticmethod
-    def inverse(xyFunct):
+    def reverse(xyFunct):
         sizeY, sizeX = xyFunct.values.shape
         pxSizeX, pxSizeY = xyFunct.domain.step
         return ScalarBidimensionalFunction(
             BidimensionalFourierTransform.inverse_transform(
                 xyFunct.values),
             xmap=BidimensionalFourierTransform.frequencies_x_map(
                 sizeX, pxSizeX),
```

### Comparing `arte-0.5.0/arte/utils/executor.py` & `arte-0.6.0/arte/utils/executor.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/footprint_geometry.py` & `arte-0.6.0/arte/utils/footprint_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,16 +129,14 @@
 #                 ll = self._polToRect(l['lRo'], l['lAz'])
 #                 cc = self._centerOffset(l['skyTheta'], l['skyAz'],
 #                                         self._layerAltitudeInMeter)
 #                 ra = self._lgsRadius()
 #                 self._dmsL.append(FootprintXYRadius(
 #                     ll[0] + cc[0], ll[1] + cc[1], ra))
 
-        self._computePatches()
-
     def getNgsFootprint(self):
         return self._ngsL
 
     def getLgsFootprint(self):
         return self._lgsL
 
     def getTargetFootprint(self):
@@ -166,15 +164,15 @@
                 l[0], l[1], l[2], 0.99 * l[2],
                 theta1=l[3] - 10, theta2=l[3] + 10, color='b')
         if self._drawMetapupil:
             for l in self._metapupilL:
                 self._addAnnularFootprint(
                     l.x, l.y, l.r, 0.99 * l.r, color='k')
         for l in self._dmsL:
-            self._addDmFootprint(l, color='k', alpha=0.1)
+            self._addDmFootprint(l, color='k', alpha=0.3)
 
     def scienceFieldRadius(self, rTel, fovInArcsec, hInMeter):
         return rTel + fovInArcsec / 2 * 4.848e-6 * hInMeter
 
     def _polToRect(self, ro, azInDeg):
         azInRad = azInDeg * np.pi / 180
         return ro * np.array(
@@ -238,14 +236,15 @@
             Polygon(vertexes, closed=True, color=color, alpha=alpha))
         self._xlim = np.maximum(
             self._xlim,
             np.linalg.norm(np.array([centerX, centerY])) +
             0.5 * np.linalg.norm(np.array([sideX, sideY])))
 
     def plot(self):
+        self._computePatches()
         fig, ax = plt.subplots()
         ax.set_aspect('equal')
         ax.set_xlim(-self._xlim, self._xlim)
         ax.set_ylim(-self._xlim, self._xlim)
         p = PatchCollection(self._patches, match_original=True)
         ax.add_collection(p)
         ax.set_title('Footprints @ %g km, zenith= %7.3f°' % (
```

### Comparing `arte-0.5.0/arte/utils/gpu.py` & `arte-0.6.0/arte/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/help.py` & `arte-0.6.0/arte/utils/help.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/image_moments.py` & `arte-0.6.0/arte/utils/image_moments.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
     def rawMoment(self, iord, jord):
         data = self._image * self.x**iord * self.y**jord
         return data.sum()
 
 
     def centralNormalizedMoment(self, iord, jord):
-        return self.centralMoment(iord, jord) / self._m00
+        return self.central_moment(iord, jord) / self._m00
 
 
     # TODO: (lb) 20160104 make it faster if needed, it is easy!
-    def centralMoment(self, iord, jord):
+    def central_moment(self, iord, jord):
         if iord == 0 and jord == 0:
             return self._m00
         if (iord == 0 and jord == 1) or (iord == 1 and jord == 0):
             return 0.
         moment=0.
         x_bar= self.xBar()
         y_bar= self.yBar()
```

### Comparing `arte-0.5.0/arte/utils/iterators.py` & `arte-0.6.0/arte/utils/iterators.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/locate.py` & `arte-0.6.0/arte/utils/locate.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/logger.py` & `arte-0.6.0/arte/utils/logger.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/marechal.py` & `arte-0.6.0/arte/utils/marechal.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/math.py` & `arte-0.6.0/arte/utils/math.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/modal_decomposer.py` & `arte-0.6.0/arte/utils/modal_decomposer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from scipy.linalg.basic import pinv
+from scipy.linalg import pinv
 from arte.utils.decorator import cacheResult, returns
 from arte.utils.zernike_generator import ZernikeGenerator
 from arte.types.zernike_coefficients import ZernikeCoefficients
 from arte.types.mask import CircularMask
 from arte.types.wavefront import Wavefront
 from arte.types.slopes import Slopes
```

### Comparing `arte-0.5.0/arte/utils/multiton.py` & `arte-0.6.0/arte/utils/multiton.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/not_available.py` & `arte-0.6.0/arte/utils/not_available.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/radial_profile.py` & `arte-0.6.0/arte/utils/radial_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     yCoord, xCoord= np.indices(image.shape)
     yCoord= (yCoord - centerInPxY)
     xCoord= (xCoord - centerInPxX)
     rCoord=np.sqrt(xCoord**2 + yCoord**2)
     indexR= np.argsort(rCoord.flat)
     radialDistancesSorted= rCoord.flat[indexR]
     imageValuesSortedByRadialDistance= image.flat[indexR]
-    integerPartOfRadialDistances= radialDistancesSorted.astype(np.int)
+    integerPartOfRadialDistances= radialDistancesSorted.astype(np.int64)
     deltaRadialDistance= integerPartOfRadialDistances[1:] - \
         integerPartOfRadialDistances[:-1]
     radialDistanceChanges= np.where(deltaRadialDistance)[0]
     nPxInBinZero= radialDistanceChanges[0]+ 1
     nPxInRadialBin= radialDistanceChanges[1:] - \
         radialDistanceChanges[:-1]
     imageRadialCumSum= np.cumsum(imageValuesSortedByRadialDistance,
```

### Comparing `arte-0.5.0/arte/utils/rebin.py` & `arte-0.6.0/arte/utils/rebin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 '''
 
 # who       when        what
 # -------  ----------  ---------------------------------
-#           2012-11-20  Created from git://gist.github.com/1348792.git
+# apuglisi  2022-02-30  Fixed bug in detecting downsampling
+#                       on just one axis
 # apuglisi  2020-04-15  Added sample option, added exceptions,
 #                       allow any kind of sequence for new_shape
+#           2012-11-20  Created from git://gist.github.com/1348792.git
 '''
 import numpy as np
 
 
 def rebin(a, new_shape, sample=False):
     """
     Replacement of IDL's rebin() function for 2d arrays.
@@ -67,15 +69,15 @@
     m, n = map(int, new_shape)
 
     if a.shape == (m, n):
         return a
 
     M, N = a.shape
 
-    if m <= M and n <= M:
+    if m <= M and n <= N:
         if (M//m != M/m) or (N//n != N/n):
             raise ValueError('Cannot downsample by non-integer factors')
 
     elif M <= m and M <= m:
         if (m//M != m/M) or (n//N != n/N):
             raise ValueError('Cannot upsample by non-integer factors')
```

### Comparing `arte-0.5.0/arte/utils/shape_fitter.py` & `arte-0.6.0/arte/utils/shape_fitter.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/shared_array.py` & `arte-0.6.0/arte/utils/shared_array.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/tabular_report.py` & `arte-0.6.0/arte/utils/tabular_report.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/timekeepers.py` & `arte-0.6.0/arte/utils/timekeepers.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/timestamp.py` & `arte-0.6.0/arte/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/unit_checker.py` & `arte-0.6.0/arte/utils/unit_checker.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/zernike_generator.py` & `arte-0.6.0/arte/utils/zernike_generator.py`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/arte/utils/zernike_projection_on_subaperture.py` & `arte-0.6.0/arte/utils/zernike_projection_on_subaperture.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 
 BUG: something wrong in computed values z2,z3 when z7 is not null in the full
 pupil
 """
 
 
 class ZernikeProjectionOnSubaperture(object):
+    
+    N_MODES = 10
 
     def __init__(self,
                  pupilRadiusInMeter,
                  subapsRadiusInMeter,
                  subapOffAxisRadiusInMeter,
                  subapOffAxisAzimuthInDegrees):
         self._R = pupilRadiusInMeter
         self._r = subapsRadiusInMeter
         self._h = subapOffAxisRadiusInMeter
         self._a = subapOffAxisAzimuthInDegrees
         self._S = self._computeMatrix()
 
-    def computeZernikeDecomponsitionOnSubap(self, zernikeCoeffFrom2To11):
+    def compute_zernike_decomposition_on_subap(self, zernikeCoeffFrom2To11):
         return np.dot(zernikeCoeffFrom2To11, self._S)
 
-    def getProjectionMatrix(self):
+    def get_projection_matrix(self):
         return self._S
+    
 
     def _computeMatrix(self):
         roR = self._r / self._R
         hoR = self._h / self._R
         ca = np.cos(self._a * np.pi / 180)
         sa = np.sin(self._a * np.pi / 180)
         c2a = np.cos(2 * self._a * np.pi / 180)
```

### Comparing `arte-0.5.0/arte.egg-info/PKG-INFO` & `arte-0.6.0/arte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arte
-Version: 0.5.0
+Version: 0.6.0
 Summary: Arcetri Random sTuff collEction
 Home-page: https://github.com/ArcetriAdaptiveOptics/arte
 Author: Lorenzo Busoni, Alfio Puglisi, INAF Arcetri Adaptive Optics group
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: Adaptive Optics, Astrophysics, INAF, Arcetri
 Classifier: Development Status :: 4 - Beta
```

### Comparing `arte-0.5.0/arte.egg-info/SOURCES.txt` & `arte-0.6.0/arte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arte-0.5.0/setup.py` & `arte-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
       install_requires=["numpy>1.17",
                         "scipy",
                         "matplotlib",
                         "astropy",
                         "synphot",
                         "pytest",
                         "skycalc-cli",
-                        "scikit-image",
+                        "scikit-image>=0.17",
                         "scipy",
                         "mpmath"
                         ],
       include_package_data=True,
       test_suite='test',
       cmdclass={'upload': UploadCommand, },
       )
```

### Comparing `arte-0.5.0/test/test_helper.py` & `arte-0.6.0/test/test_helper.py`

 * *Files identical despite different names*

