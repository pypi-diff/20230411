# Comparing `tmp/pirt-2.1.0.tar.gz` & `tmp/pirt-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pirt-2.1.0.tar", last modified: Mon Mar 19 13:27:56 2018, max compression
+gzip compressed data, was "pirt-2.1.1.tar", last modified: Tue Apr 11 13:36:59 2023, max compression
```

## Comparing `pirt-2.1.0.tar` & `pirt-2.1.1.tar`

### file list

```diff
@@ -1,100 +1,99 @@
--rw-r--r--   0        0        0      134 2018-03-19 13:27:29.257619 pirt-2.1.0/.hgignore
--rw-r--r--   0        0        0     1581 2017-04-23 21:58:23.158363 pirt-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2172 2017-09-20 12:31:37.830773 pirt-2.1.0/README.md
--rw-r--r--   0        0        0      446 2017-04-23 21:58:23.166369 pirt-2.1.0/RELEASE_NOTES.txt
--rw-r--r--   0        0        0      775 2017-09-20 12:18:20.152104 pirt-2.1.0/bitbucket-pipelines.yml
--rw-r--r--   0        0        0       27 2017-09-20 12:24:18.128650 pirt-2.1.0/docs/.requirements
--rw-r--r--   0        0        0      604 2017-09-19 21:03:06.863374 pirt-2.1.0/docs/Makefile
--rw-r--r--   0        0        0      693 2017-09-20 09:42:39.172998 pirt-2.1.0/docs/aarrays_and_pointset.rst
--rw-r--r--   0        0        0      257 2017-09-19 22:13:30.836189 pirt-2.1.0/docs/apps.rst
--rw-r--r--   0        0        0     5071 2017-12-05 12:07:21.357661 pirt-2.1.0/docs/conf.py
--rw-r--r--   0        0        0      822 2017-09-19 22:27:48.158962 pirt-2.1.0/docs/deform.rst
--rw-r--r--   0        0        0      497 2017-09-19 22:16:28.211117 pirt-2.1.0/docs/gaussfun.rst
--rw-r--r--   0        0        0     1325 2017-09-20 12:43:39.537739 pirt-2.1.0/docs/index.rst
--rw-r--r--   0        0        0      887 2017-09-19 22:27:56.591020 pirt-2.1.0/docs/interp.rst
--rwxr-xr-x   0        0        0      802 2017-09-19 21:03:06.881383 pirt-2.1.0/docs/make.bat
--rw-r--r--   0        0        0     2082 2017-12-05 13:14:37.211936 pirt-2.1.0/docs/reg.rst
--rw-r--r--   0        0        0      379 2017-09-19 22:28:03.825728 pirt-2.1.0/docs/splinegrid.rst
--rw-r--r--   0        0        0      341 2017-09-18 15:13:19.901704 pirt-2.1.0/examples/README.md
--rw-r--r--   0        0        0      831 2017-09-18 15:13:19.912721 pirt-2.1.0/examples/deform_anti_shear.py
--rw-r--r--   0        0        0     2211 2017-09-20 11:03:47.401745 pirt-2.1.0/examples/deform_block.py
--rw-r--r--   0        0        0      286 2017-09-18 15:13:19.917725 pirt-2.1.0/examples/deform_by_hand1.py
--rw-r--r--   0        0        0     1324 2017-09-18 15:13:19.920727 pirt-2.1.0/examples/deform_by_hand2.py
--rw-r--r--   0        0        0     6905 2017-09-18 15:13:19.922728 pirt-2.1.0/examples/deform_forward_vs_backward.py
--rw-r--r--   0        0        0     1634 2017-09-20 11:06:38.544560 pirt-2.1.0/examples/deform_injectivity.py
--rw-r--r--   0        0        0     2339 2017-09-20 11:09:36.371166 pirt-2.1.0/examples/deform_show_edge_freeze.py
--rw-r--r--   0        0        0      644 2017-09-18 15:13:19.933726 pirt-2.1.0/examples/deform_simple.py
--rw-r--r--   0        0        0     3850 2017-09-18 22:54:28.687732 pirt-2.1.0/examples/diffuse_pyramid.py
--rw-r--r--   0        0        0     1331 2017-09-18 15:13:19.942746 pirt-2.1.0/examples/diffuse_scale_steps.py
--rw-r--r--   0        0        0      967 2017-09-20 12:02:38.147444 pirt-2.1.0/examples/fitting_1d_and_2d.py
--rw-r--r--   0        0        0     1440 2017-09-18 15:13:19.950751 pirt-2.1.0/examples/interp_1d.py
--rw-r--r--   0        0        0     1743 2017-09-20 12:03:14.883015 pirt-2.1.0/examples/interp_2x_quadratic_is_cardinal.py
--rw-r--r--   0        0        0      352 2017-12-05 14:30:38.767274 pirt-2.1.0/examples/interp_approx_exp.py
--rw-r--r--   0        0        0     1900 2017-09-18 15:13:19.955754 pirt-2.1.0/examples/interp_bspline_injectivity.py
--rw-r--r--   0        0        0     1395 2017-09-18 22:53:50.805059 pirt-2.1.0/examples/interp_cubic_coefficients.py
--rw-r--r--   0        0        0      782 2017-09-18 22:50:03.870704 pirt-2.1.0/examples/interp_edge_effects.py
--rw-r--r--   0        0        0      941 2017-09-20 12:08:50.782971 pirt-2.1.0/examples/interp_slice_in_volume.py
--rw-r--r--   0        0        0     1739 2017-09-18 22:49:30.435021 pirt-2.1.0/examples/interp_speed_warp.py
--rw-r--r--   0        0        0      659 2017-09-18 15:13:19.981760 pirt-2.1.0/examples/interp_speed_zoom.py
--rw-r--r--   0        0        0     1837 2017-09-20 09:54:08.942722 pirt-2.1.0/examples/reg_gravity_mass_normalization.py
--rw-r--r--   0        0        0     7072 2017-09-20 12:10:13.329451 pirt-2.1.0/examples/reg_groupwise.py
--rw-r--r--   0        0        0     2200 2017-09-20 12:09:47.019994 pirt-2.1.0/examples/reg_pairwise.py
--rw-r--r--   0        0        0      367 2017-09-18 15:13:19.987765 pirt-2.1.0/examples/splinegrid_by_hand.py
--rw-r--r--   0        0        0     1192 2017-09-20 12:12:32.522686 pirt-2.1.0/examples/splinegrid_encode_image1.py
--rw-r--r--   0        0        0     1238 2017-09-19 22:46:58.769692 pirt-2.1.0/examples/splinegrid_encode_image2.py
--rw-r--r--   0        0        0      546 2017-09-11 10:18:24.912426 pirt-2.1.0/flit.ini
--rw-r--r--   0        0        0     1569 2017-09-11 12:42:53.655402 pirt-2.1.0/pirt.proxy.py
--rw-r--r--   0        0        0      381 2017-09-20 09:18:07.261833 pirt-2.1.0/pirt/README.md
--rw-r--r--   0        0        0     1306 2018-03-19 13:25:51.352301 pirt-2.1.0/pirt/__init__.py
--rw-r--r--   0        0        0    16470 2017-09-20 11:24:13.558311 pirt-2.1.0/pirt/_utils.py
--rw-r--r--   0        0        0      179 2017-09-19 22:12:28.083684 pirt-2.1.0/pirt/apps/__init__.py
--rw-r--r--   0        0        0    11907 2017-09-20 11:59:56.090663 pirt-2.1.0/pirt/apps/deform_by_hand.py
--rw-r--r--   0        0        0     7063 2017-09-20 12:12:02.082060 pirt-2.1.0/pirt/apps/spline_by_hand.py
--rw-r--r--   0        0        0      832 2017-09-19 21:32:22.929152 pirt-2.1.0/pirt/deform/__init__.py
--rw-r--r--   0        0        0    21604 2017-09-20 11:36:33.821520 pirt-2.1.0/pirt/deform/_deformbase.py
--rw-r--r--   0        0        0    18176 2017-09-20 11:43:28.538936 pirt-2.1.0/pirt/deform/_deformfield.py
--rw-r--r--   0        0        0    17478 2017-09-20 11:39:18.905507 pirt-2.1.0/pirt/deform/_deformgrid.py
--rw-r--r--   0        0        0     1351 2017-09-18 22:21:09.912240 pirt-2.1.0/pirt/deform/_subs.py
--rw-r--r--   0        0        0    12638 2017-09-20 10:29:32.524959 pirt-2.1.0/pirt/deformvis.py
--rw-r--r--   0        0        0    21696 2017-09-20 09:59:02.063752 pirt-2.1.0/pirt/experiment.py
--rw-r--r--   0        0        0     3639 2017-09-20 12:02:36.745805 pirt-2.1.0/pirt/fitting.py
--rw-r--r--   0        0        0    14558 2017-09-20 10:52:29.142593 pirt-2.1.0/pirt/gaussfun.py
--rw-r--r--   0        0        0      632 2017-09-19 21:29:03.949949 pirt-2.1.0/pirt/interp/__init__.py
--rw-r--r--   0        0        0    22386 2017-09-18 22:47:56.650576 pirt-2.1.0/pirt/interp/_backward.py
--rw-r--r--   0        0        0     5767 2017-09-18 22:47:29.316003 pirt-2.1.0/pirt/interp/_backward_cuda.py
--rw-r--r--   0        0        0    10115 2017-09-11 22:56:19.080398 pirt-2.1.0/pirt/interp/_cubic.py
--rw-r--r--   0        0        0    14501 2017-09-11 22:36:15.439726 pirt-2.1.0/pirt/interp/_forward.py
--rw-r--r--   0        0        0    10416 2017-09-19 21:18:31.456385 pirt-2.1.0/pirt/interp/_func.py
--rw-r--r--   0        0        0     5550 2017-09-11 23:24:58.407845 pirt-2.1.0/pirt/interp/_misc.py
--rw-r--r--   0        0        0     5665 2017-09-20 12:07:24.462404 pirt-2.1.0/pirt/interp/_sliceinvolume.py
--rw-r--r--   0        0        0    19727 2017-09-20 11:51:53.941064 pirt-2.1.0/pirt/new_pointset.py
--rw-r--r--   0        0        0    10299 2017-09-20 10:29:54.564981 pirt-2.1.0/pirt/pyramid.py
--rw-r--r--   0        0        0    10870 2017-09-20 11:10:24.296099 pirt-2.1.0/pirt/randomdeformations.py
--rw-r--r--   0        0        0      470 2017-12-05 13:15:52.928274 pirt-2.1.0/pirt/reg/__init__.py
--rw-r--r--   0        0        0    40248 2017-12-05 14:54:49.282626 pirt-2.1.0/pirt/reg/reg_base.py
--rw-r--r--   0        0        0    14476 2017-12-05 21:22:00.552676 pirt-2.1.0/pirt/reg/reg_demons.py
--rw-r--r--   0        0        0     9761 2017-12-05 13:25:13.360761 pirt-2.1.0/pirt/reg/reg_elastix.py
--rw-r--r--   0        0        0    16940 2017-12-05 21:22:08.952022 pirt-2.1.0/pirt/reg/reg_gravity.py
--rw-r--r--   0        0        0      991 2017-09-19 21:44:36.028153 pirt-2.1.0/pirt/splinegrid/__init__.py
--rw-r--r--   0        0        0    35198 2017-09-20 11:40:02.383776 pirt-2.1.0/pirt/splinegrid/_splinegridclasses.py
--rw-r--r--   0        0        0    28089 2017-09-20 11:40:42.672936 pirt-2.1.0/pirt/splinegrid/_splinegridfuncs.py
--rw-r--r--   0        0        0     2450 2017-09-11 11:38:53.807422 pirt-2.1.0/pirt/testing.py
--rw-r--r--   0        0        0     2848 2017-12-05 13:32:25.518981 pirt-2.1.0/setup.cfg
--rw-r--r--   0        0        0      893 2017-01-08 14:53:05.101999 pirt-2.1.0/tasks/README.md
--rw-r--r--   0        0        0     1340 2017-01-08 14:53:05.108003 pirt-2.1.0/tasks/__init__.py
--rw-r--r--   0        0        0      224 2017-01-08 14:53:05.113007 pirt-2.1.0/tasks/__main__.py
--rw-r--r--   0        0        0      207 2017-09-11 11:11:05.731261 pirt-2.1.0/tasks/_config.py
--rw-r--r--   0        0        0      956 2017-01-08 14:53:05.123014 pirt-2.1.0/tasks/clean.py
--rw-r--r--   0        0        0     1384 2017-01-08 14:53:05.130333 pirt-2.1.0/tasks/copyright.py
--rw-r--r--   0        0        0     1611 2017-01-08 14:53:05.141841 pirt-2.1.0/tasks/docs.py
--rw-r--r--   0        0        0      350 2017-01-08 14:53:05.144842 pirt-2.1.0/tasks/help.py
--rw-r--r--   0        0        0     4017 2017-09-18 13:03:47.099368 pirt-2.1.0/tasks/test.py
--rw-r--r--   0        0        0      243 2017-09-06 22:01:01.317848 pirt-2.1.0/tests/README.md
--rw-r--r--   0        0        0    11801 2017-09-20 11:49:49.981349 pirt-2.1.0/tests/test_deformations.py
--rw-r--r--   0        0        0     1590 2017-09-18 22:43:38.675265 pirt-2.1.0/tests/test_interp_funcs.py
--rw-r--r--   0        0        0     4478 2017-09-18 22:43:44.155265 pirt-2.1.0/tests/test_interp_misc.py
--rw-r--r--   0        0        0    12590 2017-09-18 22:44:02.552979 pirt-2.1.0/tests/test_interp_warp_and_project.py
--rw-r--r--   0        0        0     2585 2017-12-05 14:40:50.958340 pirt-2.1.0/tests/test_reg.py
--rw-r--r--   0        0        0    24280 2017-09-20 11:54:50.683876 pirt-2.1.0/tests/test_splinegrid.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 pirt-2.1.0/setup.py
--rw-r--r--   0        0        0      204 1970-01-01 00:00:00.000000 pirt-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2023-04-11 13:33:39.112924 pirt-2.1.1/.hgignore
+-rw-r--r--   0        0        0     1581 2023-04-11 13:33:39.113027 pirt-2.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2164 2023-04-11 13:34:22.146529 pirt-2.1.1/README.md
+-rw-r--r--   0        0        0      446 2023-04-11 13:33:39.113185 pirt-2.1.1/RELEASE_NOTES.txt
+-rw-r--r--   0        0        0      775 2023-04-11 13:33:39.113270 pirt-2.1.1/bitbucket-pipelines.yml
+-rw-r--r--   0        0        0       27 2023-04-11 13:33:39.113387 pirt-2.1.1/docs/.requirements
+-rw-r--r--   0        0        0      604 2023-04-11 13:33:39.113455 pirt-2.1.1/docs/Makefile
+-rw-r--r--   0        0        0      693 2023-04-11 13:33:39.113528 pirt-2.1.1/docs/aarrays_and_pointset.rst
+-rw-r--r--   0        0        0      257 2023-04-11 13:33:39.113592 pirt-2.1.1/docs/apps.rst
+-rw-r--r--   0        0        0     5071 2023-04-11 13:33:39.113677 pirt-2.1.1/docs/conf.py
+-rw-r--r--   0        0        0      822 2023-04-11 13:33:39.113740 pirt-2.1.1/docs/deform.rst
+-rw-r--r--   0        0        0      497 2023-04-11 13:33:39.113805 pirt-2.1.1/docs/gaussfun.rst
+-rw-r--r--   0        0        0     1314 2023-04-11 13:34:32.697024 pirt-2.1.1/docs/index.rst
+-rw-r--r--   0        0        0      887 2023-04-11 13:33:39.113937 pirt-2.1.1/docs/interp.rst
+-rw-r--r--   0        0        0      802 2023-04-11 13:33:39.114003 pirt-2.1.1/docs/make.bat
+-rw-r--r--   0        0        0     2082 2023-04-11 13:33:39.114071 pirt-2.1.1/docs/reg.rst
+-rw-r--r--   0        0        0      379 2023-04-11 13:33:39.114144 pirt-2.1.1/docs/splinegrid.rst
+-rw-r--r--   0        0        0      341 2023-04-11 13:33:39.114244 pirt-2.1.1/examples/README.md
+-rw-r--r--   0        0        0      831 2023-04-11 13:33:39.114374 pirt-2.1.1/examples/deform_anti_shear.py
+-rw-r--r--   0        0        0     2211 2023-04-11 13:33:39.114483 pirt-2.1.1/examples/deform_block.py
+-rw-r--r--   0        0        0      286 2023-04-11 13:33:39.114564 pirt-2.1.1/examples/deform_by_hand1.py
+-rw-r--r--   0        0        0     1324 2023-04-11 13:33:39.114647 pirt-2.1.1/examples/deform_by_hand2.py
+-rw-r--r--   0        0        0     6905 2023-04-11 13:33:39.114771 pirt-2.1.1/examples/deform_forward_vs_backward.py
+-rw-r--r--   0        0        0     1634 2023-04-11 13:33:39.114846 pirt-2.1.1/examples/deform_injectivity.py
+-rw-r--r--   0        0        0     2339 2023-04-11 13:33:39.114931 pirt-2.1.1/examples/deform_show_edge_freeze.py
+-rw-r--r--   0        0        0      644 2023-04-11 13:33:39.115003 pirt-2.1.1/examples/deform_simple.py
+-rw-r--r--   0        0        0     3850 2023-04-11 13:33:39.115091 pirt-2.1.1/examples/diffuse_pyramid.py
+-rw-r--r--   0        0        0     1331 2023-04-11 13:33:39.115163 pirt-2.1.1/examples/diffuse_scale_steps.py
+-rw-r--r--   0        0        0      967 2023-04-11 13:33:39.115234 pirt-2.1.1/examples/fitting_1d_and_2d.py
+-rw-r--r--   0        0        0     1440 2023-04-11 13:33:39.115349 pirt-2.1.1/examples/interp_1d.py
+-rw-r--r--   0        0        0     1743 2023-04-11 13:33:39.115433 pirt-2.1.1/examples/interp_2x_quadratic_is_cardinal.py
+-rw-r--r--   0        0        0      352 2023-04-11 13:33:39.115527 pirt-2.1.1/examples/interp_approx_exp.py
+-rw-r--r--   0        0        0     1900 2023-04-11 13:33:39.115615 pirt-2.1.1/examples/interp_bspline_injectivity.py
+-rw-r--r--   0        0        0     1395 2023-04-11 13:33:39.115690 pirt-2.1.1/examples/interp_cubic_coefficients.py
+-rw-r--r--   0        0        0      782 2023-04-11 13:33:39.115752 pirt-2.1.1/examples/interp_edge_effects.py
+-rw-r--r--   0        0        0      941 2023-04-11 13:33:39.115821 pirt-2.1.1/examples/interp_slice_in_volume.py
+-rw-r--r--   0        0        0     1739 2023-04-11 13:33:39.115897 pirt-2.1.1/examples/interp_speed_warp.py
+-rw-r--r--   0        0        0      659 2023-04-11 13:33:39.115964 pirt-2.1.1/examples/interp_speed_zoom.py
+-rw-r--r--   0        0        0     1837 2023-04-11 13:33:39.116045 pirt-2.1.1/examples/reg_gravity_mass_normalization.py
+-rw-r--r--   0        0        0     7072 2023-04-11 13:33:39.116144 pirt-2.1.1/examples/reg_groupwise.py
+-rw-r--r--   0        0        0     2200 2023-04-11 13:33:39.116229 pirt-2.1.1/examples/reg_pairwise.py
+-rw-r--r--   0        0        0      367 2023-04-11 13:33:39.116300 pirt-2.1.1/examples/splinegrid_by_hand.py
+-rw-r--r--   0        0        0     1192 2023-04-11 13:33:39.116370 pirt-2.1.1/examples/splinegrid_encode_image1.py
+-rw-r--r--   0        0        0     1238 2023-04-11 13:33:39.116447 pirt-2.1.1/examples/splinegrid_encode_image2.py
+-rw-r--r--   0        0        0     1569 2023-04-11 13:33:39.116597 pirt-2.1.1/pirt.proxy.py
+-rw-r--r--   0        0        0      381 2023-04-11 13:33:39.116699 pirt-2.1.1/pirt/README.md
+-rw-r--r--   0        0        0     1304 2023-04-11 13:35:08.355379 pirt-2.1.1/pirt/__init__.py
+-rw-r--r--   0        0        0    16470 2023-04-11 13:33:39.116915 pirt-2.1.1/pirt/_utils.py
+-rw-r--r--   0        0        0      179 2023-04-11 13:33:39.117037 pirt-2.1.1/pirt/apps/__init__.py
+-rw-r--r--   0        0        0    11907 2023-04-11 13:33:39.117163 pirt-2.1.1/pirt/apps/deform_by_hand.py
+-rw-r--r--   0        0        0     7063 2023-04-11 13:33:39.117243 pirt-2.1.1/pirt/apps/spline_by_hand.py
+-rw-r--r--   0        0        0      832 2023-04-11 13:33:39.117344 pirt-2.1.1/pirt/deform/__init__.py
+-rw-r--r--   0        0        0    21604 2023-04-11 13:33:39.117653 pirt-2.1.1/pirt/deform/_deformbase.py
+-rw-r--r--   0        0        0    18176 2023-04-11 13:33:39.117781 pirt-2.1.1/pirt/deform/_deformfield.py
+-rw-r--r--   0        0        0    17478 2023-04-11 13:33:39.117895 pirt-2.1.1/pirt/deform/_deformgrid.py
+-rw-r--r--   0        0        0     1351 2023-04-11 13:33:39.117973 pirt-2.1.1/pirt/deform/_subs.py
+-rw-r--r--   0        0        0    12638 2023-04-11 13:33:39.118077 pirt-2.1.1/pirt/deformvis.py
+-rw-r--r--   0        0        0    21696 2023-04-11 13:33:39.118212 pirt-2.1.1/pirt/experiment.py
+-rw-r--r--   0        0        0     3639 2023-04-11 13:33:39.118304 pirt-2.1.1/pirt/fitting.py
+-rw-r--r--   0        0        0    14558 2023-04-11 13:33:39.118432 pirt-2.1.1/pirt/gaussfun.py
+-rw-r--r--   0        0        0      632 2023-04-11 13:33:39.118573 pirt-2.1.1/pirt/interp/__init__.py
+-rw-r--r--   0        0        0    22386 2023-04-11 13:33:39.118928 pirt-2.1.1/pirt/interp/_backward.py
+-rw-r--r--   0        0        0     5767 2023-04-11 13:33:39.119015 pirt-2.1.1/pirt/interp/_backward_cuda.py
+-rw-r--r--   0        0        0    10115 2023-04-11 13:33:39.119108 pirt-2.1.1/pirt/interp/_cubic.py
+-rw-r--r--   0        0        0    14501 2023-04-11 13:33:39.119251 pirt-2.1.1/pirt/interp/_forward.py
+-rw-r--r--   0        0        0    10416 2023-04-11 13:33:39.119333 pirt-2.1.1/pirt/interp/_func.py
+-rw-r--r--   0        0        0     5550 2023-04-11 13:33:39.119406 pirt-2.1.1/pirt/interp/_misc.py
+-rw-r--r--   0        0        0     5665 2023-04-11 13:33:39.119481 pirt-2.1.1/pirt/interp/_sliceinvolume.py
+-rw-r--r--   0        0        0    19727 2023-04-11 13:33:39.119602 pirt-2.1.1/pirt/new_pointset.py
+-rw-r--r--   0        0        0    10299 2023-04-11 13:33:39.119705 pirt-2.1.1/pirt/pyramid.py
+-rw-r--r--   0        0        0    10870 2023-04-11 13:33:39.119797 pirt-2.1.1/pirt/randomdeformations.py
+-rw-r--r--   0        0        0      470 2023-04-11 13:33:39.119894 pirt-2.1.1/pirt/reg/__init__.py
+-rw-r--r--   0        0        0    40248 2023-04-11 13:33:39.120102 pirt-2.1.1/pirt/reg/reg_base.py
+-rw-r--r--   0        0        0    14476 2023-04-11 13:33:39.120259 pirt-2.1.1/pirt/reg/reg_demons.py
+-rw-r--r--   0        0        0     9761 2023-04-11 13:33:39.120349 pirt-2.1.1/pirt/reg/reg_elastix.py
+-rw-r--r--   0        0        0    16940 2023-04-11 13:33:39.120411 pirt-2.1.1/pirt/reg/reg_gravity.py
+-rw-r--r--   0        0        0      991 2023-04-11 13:33:39.120529 pirt-2.1.1/pirt/splinegrid/__init__.py
+-rw-r--r--   0        0        0    35198 2023-04-11 13:33:39.120694 pirt-2.1.1/pirt/splinegrid/_splinegridclasses.py
+-rw-r--r--   0        0        0    28089 2023-04-11 13:33:39.120873 pirt-2.1.1/pirt/splinegrid/_splinegridfuncs.py
+-rw-r--r--   0        0        0     2450 2023-04-11 13:33:39.120953 pirt-2.1.1/pirt/testing.py
+-rw-r--r--   0        0        0      696 2023-04-11 13:36:25.533560 pirt-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2848 2023-04-11 13:33:39.121024 pirt-2.1.1/setup.cfg
+-rw-r--r--   0        0        0      893 2023-04-11 13:33:39.121120 pirt-2.1.1/tasks/README.md
+-rw-r--r--   0        0        0     1340 2023-04-11 13:33:39.121183 pirt-2.1.1/tasks/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-11 13:33:39.121236 pirt-2.1.1/tasks/__main__.py
+-rw-r--r--   0        0        0      207 2023-04-11 13:33:39.121290 pirt-2.1.1/tasks/_config.py
+-rw-r--r--   0        0        0      956 2023-04-11 13:33:39.121349 pirt-2.1.1/tasks/clean.py
+-rw-r--r--   0        0        0     1384 2023-04-11 13:33:39.121408 pirt-2.1.1/tasks/copyright.py
+-rw-r--r--   0        0        0     1611 2023-04-11 13:33:39.121469 pirt-2.1.1/tasks/docs.py
+-rw-r--r--   0        0        0      350 2023-04-11 13:33:39.121527 pirt-2.1.1/tasks/help.py
+-rw-r--r--   0        0        0     4017 2023-04-11 13:33:39.121596 pirt-2.1.1/tasks/test.py
+-rw-r--r--   0        0        0      243 2023-04-11 13:33:39.121691 pirt-2.1.1/tests/README.md
+-rw-r--r--   0        0        0    11801 2023-04-11 13:33:39.121780 pirt-2.1.1/tests/test_deformations.py
+-rw-r--r--   0        0        0     1590 2023-04-11 13:33:39.121851 pirt-2.1.1/tests/test_interp_funcs.py
+-rw-r--r--   0        0        0     4478 2023-04-11 13:33:39.121927 pirt-2.1.1/tests/test_interp_misc.py
+-rw-r--r--   0        0        0    12590 2023-04-11 13:33:39.122030 pirt-2.1.1/tests/test_interp_warp_and_project.py
+-rw-r--r--   0        0        0     2585 2023-04-11 13:33:39.122099 pirt-2.1.1/tests/test_reg.py
+-rw-r--r--   0        0        0    24280 2023-04-11 13:33:39.122209 pirt-2.1.1/tests/test_splinegrid.py
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 pirt-2.1.1/PKG-INFO
```

### Comparing `pirt-2.1.0/LICENSE.txt` & `pirt-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/README.md` & `pirt-2.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 PIRT - Python Image Registration Toolkit.
 
 Introduction
 ------------
 
 Pirt is the "Python image registration toolkit". It is a library for
 (elastic, i.e. non-regid) image registration of 2D and 3D images with
-support for groupwise registration. It has support to constrain the 
-deformations to be "diffeomorphic", i.e. without folding or shearing, and 
+support for groupwise registration. It has support to constrain the
+deformations to be "diffeomorphic", i.e. without folding or shearing, and
 thus invertable.
 
 Pirt is written in pure Python and uses Numba for speed. It depends on
 Numpy, Scipy, Numba. It has an optional dependency on Visvis for visualization,
 and on pyelastix for the Elastix registration algorithm.
 
 Pirt implements its own interpolation functions, which, incidentally,
 are faster than the corresponding functions in scipy and scikit-image
 (after Numba's JIT warmup).
 
-Pirt is hosted on [Bitbucket](https://bitbucket.org/almarklein/pirt)
+Pirt is hosted on [Github](https://github.com/almarklein/pirt)
 and has [docs on rtd](http://pirt.readthedocs.io/).
 
 Overview
 --------
 
 Image registration itself requires several image processing techniques
 and data types, which are also included in this package:
```

### Comparing `pirt-2.1.0/bitbucket-pipelines.yml` & `pirt-2.1.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/docs/Makefile` & `pirt-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/docs/aarrays_and_pointset.rst` & `pirt-2.1.1/docs/aarrays_and_pointset.rst`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/docs/conf.py` & `pirt-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/docs/deform.rst` & `pirt-2.1.1/docs/deform.rst`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/docs/index.rst` & `pirt-2.1.1/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Welcome to Pirt's documentation!
 ================================
 
 Pirt is the "Python image registration toolkit". It is a library for
 (elastic, i.e. non-regid) image registration of 2D and 3D images with
-support for groupwise registration. It has support to constrain the 
-deformations to be "diffeomorphic", i.e. without folding or shearing, and 
+support for groupwise registration. It has support to constrain the
+deformations to be "diffeomorphic", i.e. without folding or shearing, and
 thus invertable.
 
 Pirt is written in pure Python and uses Numba for speed. It depends on
 Numpy, Scipy, Numba. It has an optional dependency on Visvis for
 visualization.
 
 Pirt implements its own interpolation functions, which, incidentally,
 are faster than the corresponding functions in scipy and scikit-image
 (after Numba's JIT warmup).
 
 The functionality inside Pirt is implemented over a series of submodules,
 but (almost) all functions and classes are available in the main namespace.
 
-The code lives on `Bitbucket <https://bitbucket.org/almarklein/pirt>`_.
+The code lives on `Github <https://github.com/almarklein/pirt>`_.
 Also check out the `examples <https://bitbucket.org/almarklein/pirt/src/tip/examples/>`_
 or the `docs <http://pirt.readthedocs.io>`_.
 
 .. toctree::
    :maxdepth: 1
    :caption: Reference:
-   
+
    gaussfun
    interp
    deform
    splinegrid
    reg
    aarrays_and_pointset
    apps
```

### Comparing `pirt-2.1.0/docs/interp.rst` & `pirt-2.1.1/docs/interp.rst`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/docs/make.bat` & `pirt-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/docs/reg.rst` & `pirt-2.1.1/docs/reg.rst`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/deform_anti_shear.py` & `pirt-2.1.1/examples/deform_anti_shear.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/deform_block.py` & `pirt-2.1.1/examples/deform_block.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/deform_by_hand2.py` & `pirt-2.1.1/examples/deform_by_hand2.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/deform_forward_vs_backward.py` & `pirt-2.1.1/examples/deform_forward_vs_backward.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/deform_injectivity.py` & `pirt-2.1.1/examples/deform_injectivity.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/deform_show_edge_freeze.py` & `pirt-2.1.1/examples/deform_show_edge_freeze.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/deform_simple.py` & `pirt-2.1.1/examples/deform_simple.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/diffuse_pyramid.py` & `pirt-2.1.1/examples/diffuse_pyramid.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/diffuse_scale_steps.py` & `pirt-2.1.1/examples/diffuse_scale_steps.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/fitting_1d_and_2d.py` & `pirt-2.1.1/examples/fitting_1d_and_2d.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/interp_1d.py` & `pirt-2.1.1/examples/interp_1d.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/interp_2x_quadratic_is_cardinal.py` & `pirt-2.1.1/examples/interp_2x_quadratic_is_cardinal.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/interp_bspline_injectivity.py` & `pirt-2.1.1/examples/interp_bspline_injectivity.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/interp_cubic_coefficients.py` & `pirt-2.1.1/examples/interp_cubic_coefficients.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/interp_edge_effects.py` & `pirt-2.1.1/examples/interp_edge_effects.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/interp_slice_in_volume.py` & `pirt-2.1.1/examples/interp_slice_in_volume.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/interp_speed_warp.py` & `pirt-2.1.1/examples/interp_speed_warp.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/interp_speed_zoom.py` & `pirt-2.1.1/examples/interp_speed_zoom.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/reg_gravity_mass_normalization.py` & `pirt-2.1.1/examples/reg_gravity_mass_normalization.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/reg_groupwise.py` & `pirt-2.1.1/examples/reg_groupwise.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/reg_pairwise.py` & `pirt-2.1.1/examples/reg_pairwise.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/splinegrid_encode_image1.py` & `pirt-2.1.1/examples/splinegrid_encode_image1.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/examples/splinegrid_encode_image2.py` & `pirt-2.1.1/examples/splinegrid_encode_image2.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt.proxy.py` & `pirt-2.1.1/pirt.proxy.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/__init__.py` & `pirt-2.1.1/pirt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # flake8: noqa
 """ Pirt - Python Image Registration Toolkit """
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 # Check compat
 import sys
 if sys.version_info < (3, 4):
     raise RuntimeError('Pirt requires at least Python 3.4')
 
-# Imports 
+# Imports
 
 from ._utils import Aarray, PointSet, Parameters
 
 from .gaussfun import (gaussiankernel, gfilter, gfilter2,
                        diffusionkernel, diffuse, diffuse2)
 
 from .pyramid import ScaleSpacePyramid
@@ -23,15 +23,15 @@
                      deform_backward, deform_forward,
                      resize, imresize, zoom, imzoom,
                      make_samples_absolute,
                      SliceInVolume)
 
 from .splinegrid import GridInterface, SplineGrid, GridContainer, FieldDescription, FD
 
-from .deform import (Deformation, DeformationIdentity, 
+from .deform import (Deformation, DeformationIdentity,
                      DeformationGrid, DeformationField,
                      DeformationGridForward, DeformationFieldForward,
                      DeformationGridBackward, DeformationFieldBackward)
 
 from .reg import *
```

### Comparing `pirt-2.1.0/pirt/_utils.py` & `pirt-2.1.1/pirt/_utils.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/apps/deform_by_hand.py` & `pirt-2.1.1/pirt/apps/deform_by_hand.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/apps/spline_by_hand.py` & `pirt-2.1.1/pirt/apps/spline_by_hand.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/deform/__init__.py` & `pirt-2.1.1/pirt/deform/__init__.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/deform/_deformbase.py` & `pirt-2.1.1/pirt/deform/_deformbase.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/deform/_deformfield.py` & `pirt-2.1.1/pirt/deform/_deformfield.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/deform/_deformgrid.py` & `pirt-2.1.1/pirt/deform/_deformgrid.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/deform/_subs.py` & `pirt-2.1.1/pirt/deform/_subs.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/deformvis.py` & `pirt-2.1.1/pirt/deformvis.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/experiment.py` & `pirt-2.1.1/pirt/experiment.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/fitting.py` & `pirt-2.1.1/pirt/fitting.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/gaussfun.py` & `pirt-2.1.1/pirt/gaussfun.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/interp/__init__.py` & `pirt-2.1.1/pirt/interp/__init__.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/interp/_backward.py` & `pirt-2.1.1/pirt/interp/_backward.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/interp/_backward_cuda.py` & `pirt-2.1.1/pirt/interp/_backward_cuda.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/interp/_cubic.py` & `pirt-2.1.1/pirt/interp/_cubic.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/interp/_forward.py` & `pirt-2.1.1/pirt/interp/_forward.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/interp/_func.py` & `pirt-2.1.1/pirt/interp/_func.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/interp/_misc.py` & `pirt-2.1.1/pirt/interp/_misc.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/interp/_sliceinvolume.py` & `pirt-2.1.1/pirt/interp/_sliceinvolume.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/new_pointset.py` & `pirt-2.1.1/pirt/new_pointset.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/pyramid.py` & `pirt-2.1.1/pirt/pyramid.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/randomdeformations.py` & `pirt-2.1.1/pirt/randomdeformations.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/reg/reg_base.py` & `pirt-2.1.1/pirt/reg/reg_base.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/reg/reg_demons.py` & `pirt-2.1.1/pirt/reg/reg_demons.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/reg/reg_elastix.py` & `pirt-2.1.1/pirt/reg/reg_elastix.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/reg/reg_gravity.py` & `pirt-2.1.1/pirt/reg/reg_gravity.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/splinegrid/__init__.py` & `pirt-2.1.1/pirt/splinegrid/__init__.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/splinegrid/_splinegridclasses.py` & `pirt-2.1.1/pirt/splinegrid/_splinegridclasses.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/splinegrid/_splinegridfuncs.py` & `pirt-2.1.1/pirt/splinegrid/_splinegridfuncs.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/pirt/testing.py` & `pirt-2.1.1/pirt/testing.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/setup.cfg` & `pirt-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tasks/README.md` & `pirt-2.1.1/tasks/README.md`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tasks/__init__.py` & `pirt-2.1.1/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tasks/clean.py` & `pirt-2.1.1/tasks/clean.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tasks/copyright.py` & `pirt-2.1.1/tasks/copyright.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tasks/docs.py` & `pirt-2.1.1/tasks/docs.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tasks/test.py` & `pirt-2.1.1/tasks/test.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tests/test_deformations.py` & `pirt-2.1.1/tests/test_deformations.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tests/test_interp_funcs.py` & `pirt-2.1.1/tests/test_interp_funcs.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tests/test_interp_misc.py` & `pirt-2.1.1/tests/test_interp_misc.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tests/test_interp_warp_and_project.py` & `pirt-2.1.1/tests/test_interp_warp_and_project.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tests/test_reg.py` & `pirt-2.1.1/tests/test_reg.py`

 * *Files identical despite different names*

### Comparing `pirt-2.1.0/tests/test_splinegrid.py` & `pirt-2.1.1/tests/test_splinegrid.py`

 * *Files identical despite different names*

