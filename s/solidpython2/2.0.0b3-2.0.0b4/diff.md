# Comparing `tmp/solidpython2-2.0.0b3.tar.gz` & `tmp/solidpython2-2.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidpython2-2.0.0b3.tar", max compression
+gzip compressed data, was "solidpython2-2.0.0b4.tar", max compression
```

## Comparing `solidpython2-2.0.0b3.tar` & `solidpython2-2.0.0b4.tar`

### file list

```diff
@@ -1,184 +1,325 @@
--rw-r--r--   0        0        0    22930 2023-03-15 13:23:46.110122 solidpython2-2.0.0b3/README.rst
--rw-r--r--   0        0        0     1124 2023-03-18 13:03:21.802968 solidpython2-2.0.0b3/pyproject.toml
--rw-r--r--   0        0        0      108 2023-03-16 11:22:53.244444 solidpython2-2.0.0b3/solid2/__init__.py
--rw-r--r--   0        0        0     1863 2022-12-02 15:01:31.860410 solidpython2-2.0.0b3/solid2/config.py
--rw-r--r--   0        0        0      381 2023-03-15 13:33:52.945033 solidpython2-2.0.0b3/solid2/core/__init__.py
--rw-r--r--   0        0        0     3488 2023-03-16 11:22:53.244444 solidpython2-2.0.0b3/solid2/core/accessSyntaxBase.py
--rw-r--r--   0        0        0    25482 2023-03-16 11:22:40.768430 solidpython2-2.0.0b3/solid2/core/builtin_primitives.py
--rw-r--r--   0        0        0     1040 2022-08-12 15:59:10.179877 solidpython2-2.0.0b3/solid2/core/builtins.implicit
--rw-r--r--   0        0        0     1989 2022-08-12 15:59:10.179877 solidpython2-2.0.0b3/solid2/core/builtins.openscad
--rw-r--r--   0        0        0     4221 2023-03-16 11:22:53.244444 solidpython2-2.0.0b3/solid2/core/builtins.py
--rw-r--r--   0        0        0      938 2022-09-03 20:01:15.234639 solidpython2-2.0.0b3/solid2/core/extension_manager.py
--rw-r--r--   0        0        0     6808 2023-03-16 11:22:53.244444 solidpython2-2.0.0b3/solid2/core/object_base.py
--rw-r--r--   0        0        0     3994 2022-08-12 15:59:10.183877 solidpython2-2.0.0b3/solid2/core/object_factory.py
--rw-r--r--   0        0        0     1965 2023-03-16 11:22:53.244444 solidpython2-2.0.0b3/solid2/core/operatorBase.py
--rw-r--r--   0        0        0     3411 2023-03-17 14:12:24.555480 solidpython2-2.0.0b3/solid2/core/parse_scad.py
--rw-r--r--   0        0        0     5485 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/core/scad_import.py
--rw-r--r--   0        0        0     3049 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/core/scad_render.py
--rw-r--r--   0        0        0     2152 2022-08-12 15:59:10.183877 solidpython2-2.0.0b3/solid2/core/utils.py
--rwxr-xr-x   0        0        0      559 2023-03-15 22:53:12.381332 solidpython2-2.0.0b3/solid2/examples/01-basics.py
--rwxr-xr-x   0        0        0      846 2023-03-15 22:55:23.517187 solidpython2-2.0.0b3/solid2/examples/02-vars-and-operators.py
--rwxr-xr-x   0        0        0      647 2022-08-12 15:59:10.183877 solidpython2-2.0.0b3/solid2/examples/03-debug-background.py
--rwxr-xr-x   0        0        0     1272 2022-08-12 15:59:10.183877 solidpython2-2.0.0b3/solid2/examples/04-convenience.py
--rwxr-xr-x   0        0        0      934 2022-08-12 15:59:10.183877 solidpython2-2.0.0b3/solid2/examples/05-access-style-syntax.py
--rwxr-xr-x   0        0        0     1182 2023-03-15 22:58:40.236989 solidpython2-2.0.0b3/solid2/examples/06-functions.py
--rwxr-xr-x   0        0        0      527 2023-03-17 19:41:23.878938 solidpython2-2.0.0b3/solid2/examples/07-libs-bosl2-attachable.py
--rwxr-xr-x   0        0        0     1793 2023-03-17 19:29:48.250404 solidpython2-2.0.0b3/solid2/examples/07-libs-bosl2.py
--rwxr-xr-x   0        0        0      620 2022-08-12 15:59:10.183877 solidpython2-2.0.0b3/solid2/examples/07-libs.py
--rwxr-xr-x   0        0        0     2821 2023-03-15 22:56:54.837095 solidpython2-2.0.0b3/solid2/examples/08-extensions.py
--rwxr-xr-x   0        0        0     1675 2022-12-15 10:19:43.476714 solidpython2-2.0.0b3/solid2/examples/09-code-attach-extension.py
--rwxr-xr-x   0        0        0      884 2023-03-15 13:23:46.114122 solidpython2-2.0.0b3/solid2/examples/10-customizer.py
--rw-r--r--   0        0        0      158 2022-08-12 15:59:10.183877 solidpython2-2.0.0b3/solid2/examples/11-font/LICENSE_README
--rw-r--r--   0        0        0    47404 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/examples/11-font/RichEatin.otf
--rwxr-xr-x   0        0        0      192 2023-03-15 13:23:46.114122 solidpython2-2.0.0b3/solid2/examples/11-fonts.py
--rwxr-xr-x   0        0        0      335 2023-03-15 13:23:46.114122 solidpython2-2.0.0b3/solid2/examples/12-animation.py
--rwxr-xr-x   0        0        0     2026 2023-03-15 13:23:46.114122 solidpython2-2.0.0b3/solid2/examples/13-animated-bouncing-ball.py
--rwxr-xr-x   0        0        0     1381 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/examples/14-implicitCAD.py
--rwxr-xr-x   0        0        0     1794 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/examples/15-implicitCAD2.py
--rwxr-xr-x   0        0        0     1102 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/examples/16-mazebox-bosl2.py
--rwxr-xr-x   0        0        0     2243 2023-03-15 13:23:46.114122 solidpython2-2.0.0b3/solid2/examples/17-greedy-scad-interface.py
--rw-r--r--   0        0        0     1196 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/examples/maze7.png
--rwxr-xr-x   0        0        0      293 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/examples/run_all_examples.py
--rw-r--r--   0        0        0        1 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/extensions/__init__.py
--rw-r--r--   0        0        0      961 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/__init__.py
--rw-r--r--   0        0        0     3308 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/affine.py
--rw-r--r--   0        0        0     1185 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/all.py
--rw-r--r--   0        0        0    12608 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/attachments.py
--rw-r--r--   0        0        0     7614 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/beziers.py
--rw-r--r--   0        0        0    10520 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/bottlecaps.py
--rw-r--r--   0        0        0     1482 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/color.py
--rw-r--r--   0        0        0     6440 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/comparisons.py
--rw-r--r--   0        0        0     1036 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/constants.py
--rw-r--r--   0        0        0     2988 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/coords.py
--rw-r--r--   0        0        0     3563 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/cubetruss.py
--rw-r--r--   0        0        0     5270 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/distributors.py
--rw-r--r--   0        0        0     7926 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/drawing.py
--rw-r--r--   0        0        0    12920 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/fnliterals.py
--rw-r--r--   0        0        0    12680 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/gears.py
--rw-r--r--   0        0        0    19564 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/geometry.py
--rw-r--r--   0        0        0     2016 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/hingesnaps.py
--rw-r--r--   0        0        0     9439 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/joiners.py
--rw-r--r--   0        0        0     5668 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/linalg.py
--rw-r--r--   0        0        0     1413 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/linear_bearings.py
--rw-r--r--   0        0        0     7016 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/lists.py
--rw-r--r--   0        0        0     4315 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/masks2d.py
--rw-r--r--   0        0        0     7013 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/masks3d.py
--rw-r--r--   0        0        0    12453 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/math.py
--rw-r--r--   0        0        0     3755 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/metric_screws.py
--rw-r--r--   0        0        0     1280 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/modular_hose.py
--rw-r--r--   0        0        0     2283 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/mutators.py
--rw-r--r--   0        0        0     4441 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/nema_steppers.py
--rw-r--r--   0        0        0     4045 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/partitions.py
--rw-r--r--   0        0        0     8347 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/paths.py
--rw-r--r--   0        0        0     3338 2023-03-18 13:02:00.366959 solidpython2-2.0.0b3/solid2/extensions/bosl2/polyhedra.py
--rw-r--r--   0        0        0     7796 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/regions.py
--rw-r--r--   0        0        0    20712 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/rounding.py
--rw-r--r--   0        0        0     2678 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/screw_drive.py
--rw-r--r--   0        0        0     5814 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/screws.py
--rw-r--r--   0        0        0    13556 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/shapes2d.py
--rw-r--r--   0        0        0    19583 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/shapes3d.py
--rw-r--r--   0        0        0    15415 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/skin.py
--rw-r--r--   0        0        0     1525 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/sliders.py
--rw-r--r--   0        0        0     7307 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/strings.py
--rw-r--r--   0        0        0     1666 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/structs.py
--rw-r--r--   0        0        0    18158 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/threading.py
--rw-r--r--   0        0        0     8396 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/transforms.py
--rw-r--r--   0        0        0     4802 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/trigonometry.py
--rw-r--r--   0        0        0      527 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/tripod_mounts.py
--rw-r--r--   0        0        0     3020 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/turtle3d.py
--rw-r--r--   0        0        0     7911 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/utility.py
--rw-r--r--   0        0        0     4400 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/vectors.py
--rw-r--r--   0        0        0     1719 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/version.py
--rw-r--r--   0        0        0     9126 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/vnf.py
--rw-r--r--   0        0        0     2097 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/walls.py
--rw-r--r--   0        0        0      969 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2/wiring.py
--rwxr-xr-x   0        0        0     1236 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/bosl2_stub_generator.py
--rw-r--r--   0        0        0      264 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/extensions/greedy_scad_interface/__init__.py
--rw-r--r--   0        0        0     1625 2023-03-15 13:23:46.114122 solidpython2-2.0.0b3/solid2/extensions/greedy_scad_interface/customizer_widgets.py
--rw-r--r--   0        0        0      871 2023-03-15 13:23:46.114122 solidpython2-2.0.0b3/solid2/extensions/greedy_scad_interface/scad_interface.py
--rw-r--r--   0        0        0     1034 2023-03-15 13:33:52.945033 solidpython2-2.0.0b3/solid2/extensions/greedy_scad_interface/scad_variable.py
--rwxr-xr-x   0        0        0     3227 2023-03-18 13:02:00.370959 solidpython2-2.0.0b3/solid2/extensions/openscad_extension_generator.py
--rw-r--r--   0        0        0     2142 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/libs/BOSL2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1323 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/libs/BOSL2/LICENSE
--rw-r--r--   0        0        0     2895 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/libs/BOSL2/README.md
--rw-r--r--   0        0        0    37745 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/libs/BOSL2/WRITING_DOCS.md
--rw-r--r--   0        0        0    16829 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/libs/BOSL2/affine.scad
--rw-r--r--   0        0        0   136954 2022-08-12 15:59:10.187877 solidpython2-2.0.0b3/solid2/libs/BOSL2/attachments.scad
--rw-r--r--   0        0        0    73284 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/beziers.scad
--rw-r--r--   0        0        0     3677 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/bosl1compat.scad
--rw-r--r--   0        0        0    46336 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/bottlecaps.scad
--rw-r--r--   0        0        0     1257 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/builtins.scad
--rw-r--r--   0        0        0     7630 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/color.scad
--rw-r--r--   0        0        0    33970 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/comparisons.scad
--rw-r--r--   0        0        0     8574 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/constants.scad
--rw-r--r--   0        0        0    18570 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/coords.scad
--rw-r--r--   0        0        0    26314 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/cubetruss.scad
--rw-r--r--   0        0        0    53512 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/distributors.scad
--rw-r--r--   0        0        0    59181 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/drawing.scad
--rw-r--r--   0        0        0    56993 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/fnliterals.scad
--rw-r--r--   0        0        0    62445 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/gears.scad
--rw-r--r--   0        0        0   125013 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/geometry.scad
--rw-r--r--   0        0        0     8985 2022-08-12 15:59:10.191877 solidpython2-2.0.0b3/solid2/libs/BOSL2/hingesnaps.scad
--rw-r--r--   0        0        0   117043 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/images/BOSL2logo.png
--rw-r--r--   0        0        0    55357 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/joiners.scad
--rw-r--r--   0        0        0    30685 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/linalg.scad
--rw-r--r--   0        0        0     5326 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/linear_bearings.scad
--rw-r--r--   0        0        0    45059 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/lists.scad
--rw-r--r--   0        0        0    21402 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/masks2d.scad
--rw-r--r--   0        0        0    21715 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/masks3d.scad
--rw-r--r--   0        0        0    54660 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/math.scad
--rw-r--r--   0        0        0    23837 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/metric_screws.scad
--rw-r--r--   0        0        0     8826 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/modular_hose.scad
--rw-r--r--   0        0        0    19913 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/mutators.scad
--rw-r--r--   0        0        0    28200 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/nema_steppers.scad
--rw-r--r--   0        0        0    23428 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/partitions.scad
--rw-r--r--   0        0        0    53553 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/paths.scad
--rw-r--r--   0        0        0    44043 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/polyhedra.scad
--rw-r--r--   0        0        0    60064 2022-08-12 15:59:10.195877 solidpython2-2.0.0b3/solid2/libs/BOSL2/regions.scad
--rw-r--r--   0        0        0   217671 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/rounding.scad
--rw-r--r--   0        0        0    11432 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/screw_drive.scad
--rw-r--r--   0        0        0    79822 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/screws.scad
--rwxr-xr-x   0        0        0      115 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/check_for_tabs.sh
--rwxr-xr-x   0        0        0     2784 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/func_coverage.py
--rwxr-xr-x   0        0        0     2345 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/img2scad.py
--rwxr-xr-x   0        0        0      545 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/increment_version.sh
--rwxr-xr-x   0        0        0      511 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/linecount.sh
--rwxr-xr-x   0        0        0      368 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/purge_wiki_history.sh
--rwxr-xr-x   0        0        0      790 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/run_tests.sh
--rw-r--r--   0        0        0    79782 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/shapes2d.scad
--rw-r--r--   0        0        0   148367 2022-08-12 15:59:10.199877 solidpython2-2.0.0b3/solid2/libs/BOSL2/shapes3d.scad
--rw-r--r--   0        0        0   161752 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/skin.scad
--rw-r--r--   0        0        0     6613 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/sliders.scad
--rw-r--r--   0        0        0     1071 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/std.scad
--rw-r--r--   0        0        0    33384 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/strings.scad
--rw-r--r--   0        0        0     5016 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/structs.scad
--rw-r--r--   0        0        0      186 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tests/README.txt
--rw-r--r--   0        0        0    61268 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/threading.scad
--rw-r--r--   0        0        0    59856 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/transforms.scad
--rw-r--r--   0        0        0    15311 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/trigonometry.scad
--rw-r--r--   0        0        0     4151 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tripod_mounts.scad
--rw-r--r--   0        0        0    47847 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/turtle3d.scad
--rw-r--r--   0        0        0    34615 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Attachments.md
--rw-r--r--   0        0        0     6240 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Distributors.md
--rw-r--r--   0        0        0     3329 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/FractalTree.md
--rw-r--r--   0        0        0     7580 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Mutators.md
--rw-r--r--   0        0        0    14849 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Paths.md
--rw-r--r--   0        0        0    19937 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Shapes2d.md
--rw-r--r--   0        0        0     9378 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Shapes3d.md
--rw-r--r--   0        0        0     6679 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Transforms.md
--rw-r--r--   0        0        0     7054 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/VNF.md
--rw-r--r--   0        0        0    37101 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/utility.scad
--rw-r--r--   0        0        0    25139 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/vectors.scad
--rw-r--r--   0        0        0     6047 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/version.scad
--rw-r--r--   0        0        0    73918 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/vnf.scad
--rw-r--r--   0        0        0    15623 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/walls.scad
--rw-r--r--   0        0        0     3421 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/BOSL2/wiring.scad
--rw-r--r--   0        0        0        0 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/__init__.py
--rw-r--r--   0        0        0     7048 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/py_scadparser/LICENSE
--rw-r--r--   0        0        0      640 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/py_scadparser/README.md
--rw-r--r--   0        0        0    48312 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/py_scadparser/parsetab.py
--rw-r--r--   0        0        0     1229 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/py_scadparser/scad_ast.py
--rw-r--r--   0        0        0     8328 2022-08-12 15:59:10.203877 solidpython2-2.0.0b3/solid2/libs/py_scadparser/scad_parser.py
--rw-r--r--   0        0        0     2745 2023-03-18 12:56:04.182911 solidpython2-2.0.0b3/solid2/libs/py_scadparser/scad_tokens.py
--rw-r--r--   0        0        0    24591 1970-01-01 00:00:00.000000 solidpython2-2.0.0b3/setup.py
--rw-r--r--   0        0        0    24248 1970-01-01 00:00:00.000000 solidpython2-2.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0    22930 2023-03-15 13:23:46.110122 solidpython2-2.0.0b4/README.rst
+-rw-r--r--   0        0        0     1124 2023-03-23 17:50:13.249468 solidpython2-2.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-03-16 11:22:53.244444 solidpython2-2.0.0b4/solid2/__init__.py
+-rw-r--r--   0        0        0     1687 2023-03-20 22:35:21.713279 solidpython2-2.0.0b4/solid2/config.py
+-rw-r--r--   0        0        0      381 2023-03-15 13:33:52.945033 solidpython2-2.0.0b4/solid2/core/__init__.py
+-rw-r--r--   0        0        0      554 2023-03-15 13:35:20.520880 solidpython2-2.0.0b4/solid2/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      423 2022-08-12 15:59:23.591930 solidpython2-2.0.0b4/solid2/core/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6380 2023-03-16 18:55:30.044594 solidpython2-2.0.0b4/solid2/core/__pycache__/accessSyntaxBase.cpython-310.pyc
+-rw-r--r--   0        0        0     6918 2022-09-07 12:28:16.184411 solidpython2-2.0.0b4/solid2/core/__pycache__/accessSyntaxBase.cpython-38.pyc
+-rw-r--r--   0        0        0    28847 2023-03-19 13:06:07.912877 solidpython2-2.0.0b4/solid2/core/__pycache__/builtin_primitives.cpython-310.pyc
+-rw-r--r--   0        0        0    29566 2022-09-01 10:40:49.372983 solidpython2-2.0.0b4/solid2/core/__pycache__/builtin_primitives.cpython-38.pyc
+-rw-r--r--   0        0        0     5278 2023-03-16 18:55:29.980594 solidpython2-2.0.0b4/solid2/core/__pycache__/builtins.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2022-11-04 17:06:42.583231 solidpython2-2.0.0b4/solid2/core/__pycache__/builtins.cpython-38.pyc
+-rw-r--r--   0        0        0    29570 2022-09-01 10:26:41.748636 solidpython2-2.0.0b4/solid2/core/__pycache__/explicit_builtins.cpython-38.pyc
+-rw-r--r--   0        0        0     1599 2022-12-15 09:17:23.706920 solidpython2-2.0.0b4/solid2/core/__pycache__/extension_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     1659 2022-09-04 08:54:20.584363 solidpython2-2.0.0b4/solid2/core/__pycache__/extension_manager.cpython-38.pyc
+-rw-r--r--   0        0        0     9562 2023-03-16 18:55:30.036594 solidpython2-2.0.0b4/solid2/core/__pycache__/object_base.cpython-310.pyc
+-rw-r--r--   0        0        0     4712 2022-11-04 17:06:42.599231 solidpython2-2.0.0b4/solid2/core/__pycache__/object_base.cpython-38.pyc
+-rw-r--r--   0        0        0     2902 2022-12-15 09:17:23.690920 solidpython2-2.0.0b4/solid2/core/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     2906 2022-08-12 15:59:23.619930 solidpython2-2.0.0b4/solid2/core/__pycache__/object_factory.cpython-38.pyc
+-rw-r--r--   0        0        0     2402 2023-03-16 18:55:30.044594 solidpython2-2.0.0b4/solid2/core/__pycache__/operatorBase.cpython-310.pyc
+-rw-r--r--   0        0        0     2420 2022-09-04 09:09:46.976401 solidpython2-2.0.0b4/solid2/core/__pycache__/operatorBase.cpython-38.pyc
+-rw-r--r--   0        0        0     2616 2023-03-19 17:50:38.095079 solidpython2-2.0.0b4/solid2/core/__pycache__/parse_scad.cpython-310.pyc
+-rw-r--r--   0        0        0     2548 2022-08-12 15:59:23.611930 solidpython2-2.0.0b4/solid2/core/__pycache__/parse_scad.cpython-38.pyc
+-rw-r--r--   0        0        0     3817 2023-03-19 17:50:38.075079 solidpython2-2.0.0b4/solid2/core/__pycache__/scad_import.cpython-310.pyc
+-rw-r--r--   0        0        0     3662 2022-08-12 15:59:23.595930 solidpython2-2.0.0b4/solid2/core/__pycache__/scad_import.cpython-38.pyc
+-rw-r--r--   0        0        0     2296 2023-03-21 15:30:12.280767 solidpython2-2.0.0b4/solid2/core/__pycache__/scad_render.cpython-310.pyc
+-rw-r--r--   0        0        0     2185 2022-08-12 15:59:23.619930 solidpython2-2.0.0b4/solid2/core/__pycache__/scad_render.cpython-38.pyc
+-rw-r--r--   0        0        0     2079 2022-12-15 09:17:23.674920 solidpython2-2.0.0b4/solid2/core/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2063 2022-08-12 15:59:23.599930 solidpython2-2.0.0b4/solid2/core/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0       53 2023-03-20 22:35:21.713279 solidpython2-2.0.0b4/solid2/core/builtins/__init__.py
+-rw-r--r--   0        0        0      215 2023-03-21 15:30:12.248767 solidpython2-2.0.0b4/solid2/core/builtins/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    28807 2023-03-19 17:50:38.111079 solidpython2-2.0.0b4/solid2/core/builtins/__pycache__/builtin_primitives.cpython-310.pyc
+-rw-r--r--   0        0        0      364 2023-03-19 13:10:55.672767 solidpython2-2.0.0b4/solid2/core/builtins/__pycache__/builtins.cpython-310.pyc
+-rw-r--r--   0        0        0      170 2023-03-20 21:07:38.219931 solidpython2-2.0.0b4/solid2/core/builtins/__pycache__/builtins_impl.cpython-310.pyc
+-rw-r--r--   0        0        0     5188 2023-03-21 15:30:12.276767 solidpython2-2.0.0b4/solid2/core/builtins/__pycache__/convenience.cpython-310.pyc
+-rw-r--r--   0        0        0    28808 2023-03-21 15:30:12.272767 solidpython2-2.0.0b4/solid2/core/builtins/__pycache__/openscad_primitives.cpython-310.pyc
+-rw-r--r--   0        0        0      458 2023-03-21 15:30:12.252767 solidpython2-2.0.0b4/solid2/core/builtins/__pycache__/primitives.cpython-310.pyc
+-rw-r--r--   0        0        0     3633 2023-03-20 22:35:21.713279 solidpython2-2.0.0b4/solid2/core/builtins/convenience.py
+-rw-r--r--   0        0        0     1040 2023-03-20 22:35:21.713279 solidpython2-2.0.0b4/solid2/core/builtins/implicit.primitives
+-rw-r--r--   0        0        0      754 2023-03-20 22:35:21.713279 solidpython2-2.0.0b4/solid2/core/builtins/openscad.mutators
+-rw-r--r--   0        0        0     1968 2023-03-20 22:35:21.713279 solidpython2-2.0.0b4/solid2/core/builtins/openscad.primitives
+-rw-r--r--   0        0        0    25400 2023-03-20 22:35:21.713279 solidpython2-2.0.0b4/solid2/core/builtins/openscad_primitives.py
+-rw-r--r--   0        0        0      367 2023-03-20 22:35:21.713279 solidpython2-2.0.0b4/solid2/core/builtins/primitives.py
+-rw-r--r--   0        0        0      938 2022-09-03 20:01:15.234639 solidpython2-2.0.0b4/solid2/core/extension_manager.py
+-rw-r--r--   0        0        0       32 2023-03-19 13:30:20.199884 solidpython2-2.0.0b4/solid2/core/object_base/__init__.py
+-rw-r--r--   0        0        0      201 2023-03-19 17:50:38.103079 solidpython2-2.0.0b4/solid2/core/object_base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6414 2023-03-20 15:40:54.295908 solidpython2-2.0.0b4/solid2/core/object_base/__pycache__/access_syntax_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0     9417 2023-03-19 13:06:07.904877 solidpython2-2.0.0b4/solid2/core/object_base/__pycache__/object_base.cpython-310.pyc
+-rw-r--r--   0        0        0     9636 2023-03-21 15:30:12.268767 solidpython2-2.0.0b4/solid2/core/object_base/__pycache__/object_base_impl.cpython-310.pyc
+-rw-r--r--   0        0        0     2465 2023-03-20 15:40:54.295908 solidpython2-2.0.0b4/solid2/core/object_base/__pycache__/operator_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0     3522 2023-03-20 14:58:07.769013 solidpython2-2.0.0b4/solid2/core/object_base/access_syntax_mixin.py
+-rw-r--r--   0        0        0     6839 2023-03-23 17:47:21.609266 solidpython2-2.0.0b4/solid2/core/object_base/object_base_impl.py
+-rw-r--r--   0        0        0     2253 2023-03-20 14:58:07.769013 solidpython2-2.0.0b4/solid2/core/object_base/operator_mixin.py
+-rw-r--r--   0        0        0     3994 2022-08-12 15:59:10.183877 solidpython2-2.0.0b4/solid2/core/object_factory.py
+-rw-r--r--   0        0        0     3469 2023-03-21 17:35:24.083900 solidpython2-2.0.0b4/solid2/core/parse_scad.py
+-rw-r--r--   0        0        0     5493 2023-03-19 13:30:20.199884 solidpython2-2.0.0b4/solid2/core/scad_import.py
+-rw-r--r--   0        0        0     3049 2023-03-23 17:47:21.609266 solidpython2-2.0.0b4/solid2/core/scad_render.py
+-rw-r--r--   0        0        0     2152 2022-08-12 15:59:10.183877 solidpython2-2.0.0b4/solid2/core/utils.py
+-rwxr-xr-x   0        0        0      559 2023-03-15 22:53:12.381332 solidpython2-2.0.0b4/solid2/examples/01-basics.py
+-rw-r--r--   0        0        0       75 2023-03-20 22:32:59.744979 solidpython2-2.0.0b4/solid2/examples/01-basics.scad
+-rwxr-xr-x   0        0        0      846 2023-03-15 22:55:23.517187 solidpython2-2.0.0b4/solid2/examples/02-vars-and-operators.py
+-rw-r--r--   0        0        0       66 2023-03-20 22:32:59.800979 solidpython2-2.0.0b4/solid2/examples/02-vars-and-operators.scad
+-rwxr-xr-x   0        0        0      647 2022-08-12 15:59:10.183877 solidpython2-2.0.0b4/solid2/examples/03-debug-background.py
+-rw-r--r--   0        0        0      110 2023-03-20 22:32:59.860980 solidpython2-2.0.0b4/solid2/examples/03-debug-background.scad
+-rwxr-xr-x   0        0        0     1272 2022-08-12 15:59:10.183877 solidpython2-2.0.0b4/solid2/examples/04-convenience.py
+-rw-r--r--   0        0        0      166 2023-03-20 22:32:59.916980 solidpython2-2.0.0b4/solid2/examples/04-convenience.scad
+-rwxr-xr-x   0        0        0      934 2022-08-12 15:59:10.183877 solidpython2-2.0.0b4/solid2/examples/05-access-style-syntax.py
+-rw-r--r--   0        0        0      166 2023-03-20 22:32:59.972980 solidpython2-2.0.0b4/solid2/examples/05-access-style-syntax.scad
+-rwxr-xr-x   0        0        0     1182 2023-03-15 22:58:40.236989 solidpython2-2.0.0b4/solid2/examples/06-functions.py
+-rw-r--r--   0        0        0     1268 2023-03-20 22:33:00.032980 solidpython2-2.0.0b4/solid2/examples/06-functions.scad
+-rwxr-xr-x   0        0        0      527 2023-03-19 11:58:59.349891 solidpython2-2.0.0b4/solid2/examples/07-libs-bosl2-attachable.py
+-rw-r--r--   0        0        0     3047 2023-03-20 22:33:00.172980 solidpython2-2.0.0b4/solid2/examples/07-libs-bosl2-attachable.scad
+-rw-r--r--   0        0        0     3342 2023-03-20 14:58:07.769013 solidpython2-2.0.0b4/solid2/examples/07-libs-bosl2-logo.py
+-rw-r--r--   0        0        0     4669 2023-03-20 22:33:00.268980 solidpython2-2.0.0b4/solid2/examples/07-libs-bosl2-logo.scad
+-rwxr-xr-x   0        0        0     1762 2023-03-20 14:58:07.769013 solidpython2-2.0.0b4/solid2/examples/07-libs-bosl2.py
+-rw-r--r--   0        0        0    39897 2023-03-20 22:33:00.360981 solidpython2-2.0.0b4/solid2/examples/07-libs-bosl2.scad
+-rwxr-xr-x   0        0        0      620 2022-08-12 15:59:10.183877 solidpython2-2.0.0b4/solid2/examples/07-libs.py
+-rw-r--r--   0        0        0      128 2023-03-20 22:33:00.420981 solidpython2-2.0.0b4/solid2/examples/07-libs.scad
+-rwxr-xr-x   0        0        0     2448 2023-03-20 14:58:07.769013 solidpython2-2.0.0b4/solid2/examples/08-extensions.py
+-rw-r--r--   0        0        0      200 2023-03-20 22:33:00.476981 solidpython2-2.0.0b4/solid2/examples/08-extensions.scad
+-rwxr-xr-x   0        0        0     1675 2022-12-15 10:19:43.476714 solidpython2-2.0.0b4/solid2/examples/09-code-attach-extension.py
+-rw-r--r--   0        0        0     1753 2023-03-20 22:33:00.532981 solidpython2-2.0.0b4/solid2/examples/09-code-attach-extension.scad
+-rwxr-xr-x   0        0        0      889 2023-03-19 12:43:05.625475 solidpython2-2.0.0b4/solid2/examples/10-customizer.py
+-rw-r--r--   0        0        0      755 2023-03-20 22:33:00.588981 solidpython2-2.0.0b4/solid2/examples/10-customizer.scad
+-rw-r--r--   0        0        0      158 2022-08-12 15:59:10.183877 solidpython2-2.0.0b4/solid2/examples/11-font/LICENSE_README
+-rw-r--r--   0        0        0    47404 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/examples/11-font/RichEatin.otf
+-rwxr-xr-x   0        0        0      192 2023-03-15 13:23:46.114122 solidpython2-2.0.0b4/solid2/examples/11-fonts.py
+-rw-r--r--   0        0        0      100 2023-03-20 22:33:00.648981 solidpython2-2.0.0b4/solid2/examples/11-fonts.scad
+-rwxr-xr-x   0        0        0      335 2023-03-15 13:23:46.114122 solidpython2-2.0.0b4/solid2/examples/12-animation.py
+-rw-r--r--   0        0        0      141 2023-03-20 22:33:00.700981 solidpython2-2.0.0b4/solid2/examples/12-animation.scad
+-rwxr-xr-x   0        0        0     2032 2023-03-19 12:43:05.625475 solidpython2-2.0.0b4/solid2/examples/13-animated-bouncing-ball.py
+-rw-r--r--   0        0        0    43939 2023-03-20 22:33:00.764981 solidpython2-2.0.0b4/solid2/examples/13-animated-bouncing-ball.scad
+-rw-r--r--   0        0        0     1353 2023-03-20 22:33:00.820982 solidpython2-2.0.0b4/solid2/examples/14-implicitCAD.escad
+-rwxr-xr-x   0        0        0     1381 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/examples/14-implicitCAD.py
+-rw-r--r--   0        0        0     1177 2023-03-20 22:33:00.872982 solidpython2-2.0.0b4/solid2/examples/15-implicitCAD2.escad
+-rwxr-xr-x   0        0        0     1794 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/examples/15-implicitCAD2.py
+-rwxr-xr-x   0        0        0     1102 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/examples/16-mazebox-bosl2.py
+-rw-r--r--   0        0        0    10656 2023-03-20 22:33:00.952982 solidpython2-2.0.0b4/solid2/examples/16-mazebox-bosl2.scad
+-rwxr-xr-x   0        0        0     2243 2023-03-15 13:23:46.114122 solidpython2-2.0.0b4/solid2/examples/17-greedy-scad-interface.py
+-rw-r--r--   0        0        0      541 2023-03-20 22:33:01.012982 solidpython2-2.0.0b4/solid2/examples/17-greedy-scad-interface.scad
+-rw-r--r--   0        0        0     1196 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/examples/maze7.png
+-rwxr-xr-x   0        0        0      293 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/examples/run_all_examples.py
+-rw-r--r--   0        0        0        1 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/extensions/__init__.py
+-rw-r--r--   0        0        0     2480 2023-03-17 15:24:05.098592 solidpython2-2.0.0b4/solid2/extensions/__pycache__/___bosl2_stub_generator.cpython-310.pyc
+-rw-r--r--   0        0        0      162 2022-12-15 09:17:23.698920 solidpython2-2.0.0b4/solid2/extensions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      148 2022-08-12 15:59:23.623930 solidpython2-2.0.0b4/solid2/extensions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4377 2022-12-15 09:17:23.702920 solidpython2-2.0.0b4/solid2/extensions/__pycache__/access_syntax.cpython-310.pyc
+-rw-r--r--   0        0        0     4759 2022-11-04 17:06:42.607231 solidpython2-2.0.0b4/solid2/extensions/__pycache__/access_syntax.cpython-38.pyc
+-rw-r--r--   0        0        0     2462 2023-03-17 15:22:25.114628 solidpython2-2.0.0b4/solid2/extensions/__pycache__/bosl2.cpython-310.pyc
+-rw-r--r--   0        0        0     1582 2022-08-12 15:59:23.631930 solidpython2-2.0.0b4/solid2/extensions/__pycache__/bosl2.cpython-38.pyc
+-rw-r--r--   0        0        0     2477 2023-03-17 15:23:27.666606 solidpython2-2.0.0b4/solid2/extensions/__pycache__/bosl2_stub_generator.cpython-310.pyc
+-rw-r--r--   0        0        0     3742 2023-01-29 10:37:12.813201 solidpython2-2.0.0b4/solid2/extensions/__pycache__/convenience.cpython-310.pyc
+-rw-r--r--   0        0        0     4010 2022-11-04 17:09:30.895053 solidpython2-2.0.0b4/solid2/extensions/__pycache__/convenience.cpython-38.pyc
+-rw-r--r--   0        0        0    29576 2022-08-12 15:59:23.627930 solidpython2-2.0.0b4/solid2/extensions/__pycache__/explicit_builtins.cpython-38.pyc
+-rw-r--r--   0        0        0     2358 2022-07-17 22:37:30.559456 solidpython2-2.0.0b4/solid2/extensions/__pycache__/exportResultAsModule.cpython-38.pyc
+-rw-r--r--   0        0        0     3844 2023-03-21 16:33:13.384780 solidpython2-2.0.0b4/solid2/extensions/__pycache__/openscad_extension_generator.cpython-310.pyc
+-rw-r--r--   0        0        0     1511 2022-12-15 09:17:23.698920 solidpython2-2.0.0b4/solid2/extensions/__pycache__/operators.cpython-310.pyc
+-rw-r--r--   0        0        0     1489 2022-11-04 17:06:42.603231 solidpython2-2.0.0b4/solid2/extensions/__pycache__/operators.cpython-38.pyc
+-rw-r--r--   0        0        0     1954 2022-06-21 12:18:20.283311 solidpython2-2.0.0b4/solid2/extensions/__pycache__/scad_interface.cpython-38.pyc
+-rw-r--r--   0        0        0      210 2023-03-20 21:53:25.648477 solidpython2-2.0.0b4/solid2/extensions/bosl2/__init__.py
+-rw-r--r--   0        0        0      393 2023-03-20 21:54:51.820644 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5373 2023-03-20 22:33:00.144980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/affine.cpython-310.pyc
+-rw-r--r--   0        0        0    16062 2023-03-20 22:33:00.108980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/attachments.cpython-310.pyc
+-rw-r--r--   0        0        0     9635 2023-03-20 22:33:00.260980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/beziers.cpython-310.pyc
+-rw-r--r--   0        0        0    18026 2023-03-21 15:59:20.551984 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/bosl2_access_syntax_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0     1638 2023-03-20 15:40:54.307908 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/bosl2_base.cpython-310.pyc
+-rw-r--r--   0        0        0    14715 2023-03-20 11:25:53.399813 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/bosl2_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0      961 2023-03-20 12:13:36.942901 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/bosl2_operator_mixin.cpython-310.pyc
+-rw-r--r--   0        0        0      555 2023-03-20 15:40:54.391908 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/bosl2_patches.cpython-310.pyc
+-rw-r--r--   0        0        0     2316 2023-03-20 22:33:00.104980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/color.cpython-310.pyc
+-rw-r--r--   0        0        0     9435 2023-03-20 22:33:00.136980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/comparisons.cpython-310.pyc
+-rw-r--r--   0        0        0     1316 2023-03-20 22:33:00.096980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     4550 2023-03-20 22:33:00.148980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/coords.cpython-310.pyc
+-rw-r--r--   0        0        0     3773 2023-03-20 22:33:00.264980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/cubetruss.cpython-310.pyc
+-rw-r--r--   0        0        0     6555 2023-03-20 22:33:00.100980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/distributors.cpython-310.pyc
+-rw-r--r--   0        0        0     6069 2023-03-20 22:33:00.120980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/drawing.cpython-310.pyc
+-rw-r--r--   0        0        0    10428 2023-03-20 22:33:00.260980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/gears.cpython-310.pyc
+-rw-r--r--   0        0        0    25233 2023-03-20 22:33:00.152980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/geometry.cpython-310.pyc
+-rw-r--r--   0        0        0     8569 2023-03-20 22:33:00.140980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/linalg.cpython-310.pyc
+-rw-r--r--   0        0        0    10183 2023-03-20 22:33:00.136980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/lists.cpython-310.pyc
+-rw-r--r--   0        0        0     4069 2023-03-20 22:33:00.124980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/masks2d.cpython-310.pyc
+-rw-r--r--   0        0        0     6409 2023-03-20 22:33:00.120980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/masks3d.cpython-310.pyc
+-rw-r--r--   0        0        0    18287 2023-03-20 22:33:00.128980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/math.cpython-310.pyc
+-rw-r--r--   0        0        0     4984 2023-03-20 22:33:00.352981 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/metric_screws.cpython-310.pyc
+-rw-r--r--   0        0        0     3361 2023-03-20 22:33:00.100980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/mutators.cpython-310.pyc
+-rw-r--r--   0        0        0     8511 2023-03-21 15:59:20.547984 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/openscad.cpython-310.pyc
+-rw-r--r--   0        0        0     5514 2023-03-20 22:33:00.172980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/partitions.cpython-310.pyc
+-rw-r--r--   0        0        0    10384 2023-03-20 22:33:00.132980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/paths.cpython-310.pyc
+-rw-r--r--   0        0        0     9518 2023-03-20 22:33:00.156980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/regions.cpython-310.pyc
+-rw-r--r--   0        0        0     6037 2023-03-20 22:33:00.264980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/screws.cpython-310.pyc
+-rw-r--r--   0        0        0    11568 2023-03-20 22:33:00.116980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/shapes2d.cpython-310.pyc
+-rw-r--r--   0        0        0    14561 2023-03-20 22:33:00.112980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/shapes3d.cpython-310.pyc
+-rw-r--r--   0        0        0    13993 2023-03-20 22:33:00.164980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/skin.cpython-310.pyc
+-rw-r--r--   0        0        0      731 2023-03-21 15:59:20.543984 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/std.cpython-310.pyc
+-rw-r--r--   0        0        0    10226 2023-03-20 22:33:00.160980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/strings.cpython-310.pyc
+-rw-r--r--   0        0        0    11425 2023-03-20 22:33:00.100980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/transforms.cpython-310.pyc
+-rw-r--r--   0        0        0     7010 2023-03-20 22:33:00.140980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/trigonometry.cpython-310.pyc
+-rw-r--r--   0        0        0    11940 2023-03-20 22:33:00.168980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/utility.cpython-310.pyc
+-rw-r--r--   0        0        0     6439 2023-03-20 22:33:00.144980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/vectors.cpython-310.pyc
+-rw-r--r--   0        0        0     2934 2023-03-20 22:33:00.096980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/version.cpython-310.pyc
+-rw-r--r--   0        0        0    11953 2023-03-20 22:33:00.164980 solidpython2-2.0.0b4/solid2/extensions/bosl2/__pycache__/vnf.cpython-310.pyc
+-rw-r--r--   0        0        0     3320 2023-03-21 16:33:13.784774 solidpython2-2.0.0b4/solid2/extensions/bosl2/affine.py
+-rw-r--r--   0        0        0    12499 2023-03-21 16:33:15.172751 solidpython2-2.0.0b4/solid2/extensions/bosl2/attachments.py
+-rw-r--r--   0        0        0     7575 2023-03-21 16:33:13.956771 solidpython2-2.0.0b4/solid2/extensions/bosl2/beziers.py
+-rw-r--r--   0        0        0    15725 2023-03-21 16:33:13.744774 solidpython2-2.0.0b4/solid2/extensions/bosl2/bosl2_access_syntax_mixin.py
+-rw-r--r--   0        0        0     1002 2023-03-20 14:58:07.773012 solidpython2-2.0.0b4/solid2/extensions/bosl2/bosl2_base.py
+-rw-r--r--   0        0        0      611 2023-03-20 14:58:07.773012 solidpython2-2.0.0b4/solid2/extensions/bosl2/bosl2_patches.py
+-rw-r--r--   0        0        0    10523 2023-03-21 16:33:13.876772 solidpython2-2.0.0b4/solid2/extensions/bosl2/bottlecaps.py
+-rw-r--r--   0        0        0     1542 2023-03-21 16:33:14.132768 solidpython2-2.0.0b4/solid2/extensions/bosl2/color.py
+-rw-r--r--   0        0        0     6384 2023-03-21 16:33:13.768774 solidpython2-2.0.0b4/solid2/extensions/bosl2/comparisons.py
+-rw-r--r--   0        0        0     1140 2023-03-21 16:33:14.068769 solidpython2-2.0.0b4/solid2/extensions/bosl2/constants.py
+-rw-r--r--   0        0        0     3012 2023-03-21 16:33:15.008753 solidpython2-2.0.0b4/solid2/extensions/bosl2/coords.py
+-rw-r--r--   0        0        0     3619 2023-03-21 16:33:15.196750 solidpython2-2.0.0b4/solid2/extensions/bosl2/cubetruss.py
+-rw-r--r--   0        0        0     5270 2023-03-21 16:33:13.984770 solidpython2-2.0.0b4/solid2/extensions/bosl2/distributors.py
+-rw-r--r--   0        0        0     7950 2023-03-21 16:33:14.784757 solidpython2-2.0.0b4/solid2/extensions/bosl2/drawing.py
+-rw-r--r--   0        0        0    12656 2023-03-21 16:33:13.912772 solidpython2-2.0.0b4/solid2/extensions/bosl2/fnliterals.py
+-rw-r--r--   0        0        0    12640 2023-03-21 16:33:14.224766 solidpython2-2.0.0b4/solid2/extensions/bosl2/gears.py
+-rw-r--r--   0        0        0    19280 2023-03-21 16:33:14.296765 solidpython2-2.0.0b4/solid2/extensions/bosl2/geometry.py
+-rw-r--r--   0        0        0     2088 2023-03-21 16:33:14.620760 solidpython2-2.0.0b4/solid2/extensions/bosl2/hingesnaps.py
+-rw-r--r--   0        0        0     9439 2023-03-21 16:33:15.100752 solidpython2-2.0.0b4/solid2/extensions/bosl2/joiners.py
+-rw-r--r--   0        0        0     5628 2023-03-21 16:33:14.092769 solidpython2-2.0.0b4/solid2/extensions/bosl2/linalg.py
+-rw-r--r--   0        0        0     1485 2023-03-21 16:33:13.832773 solidpython2-2.0.0b4/solid2/extensions/bosl2/linear_bearings.py
+-rw-r--r--   0        0        0     6948 2023-03-21 16:33:13.808773 solidpython2-2.0.0b4/solid2/extensions/bosl2/lists.py
+-rw-r--r--   0        0        0     4347 2023-03-21 16:33:14.972754 solidpython2-2.0.0b4/solid2/extensions/bosl2/masks2d.py
+-rw-r--r--   0        0        0     7013 2023-03-21 16:33:14.736758 solidpython2-2.0.0b4/solid2/extensions/bosl2/masks3d.py
+-rw-r--r--   0        0        0    12249 2023-03-21 16:33:14.916755 solidpython2-2.0.0b4/solid2/extensions/bosl2/math.py
+-rw-r--r--   0        0        0     3783 2023-03-21 16:33:15.232750 solidpython2-2.0.0b4/solid2/extensions/bosl2/metric_screws.py
+-rw-r--r--   0        0        0     1359 2023-03-21 16:33:15.204750 solidpython2-2.0.0b4/solid2/extensions/bosl2/modular_hose.py
+-rw-r--r--   0        0        0     2335 2023-03-21 16:33:14.872756 solidpython2-2.0.0b4/solid2/extensions/bosl2/mutators.py
+-rw-r--r--   0        0        0     4461 2023-03-21 16:33:15.028753 solidpython2-2.0.0b4/solid2/extensions/bosl2/nema_steppers.py
+-rw-r--r--   0        0        0     6047 2023-03-21 16:33:15.268749 solidpython2-2.0.0b4/solid2/extensions/bosl2/openscad.py
+-rw-r--r--   0        0        0     4057 2023-03-21 16:33:13.824773 solidpython2-2.0.0b4/solid2/extensions/bosl2/partitions.py
+-rw-r--r--   0        0        0     8291 2023-03-21 16:33:14.616760 solidpython2-2.0.0b4/solid2/extensions/bosl2/paths.py
+-rw-r--r--   0        0        0     3389 2023-03-21 16:33:14.128768 solidpython2-2.0.0b4/solid2/extensions/bosl2/polyhedra.py
+-rw-r--r--   0        0        0     7756 2023-03-21 16:33:15.264749 solidpython2-2.0.0b4/solid2/extensions/bosl2/regions.py
+-rw-r--r--   0        0        0    20576 2023-03-21 16:33:14.400763 solidpython2-2.0.0b4/solid2/extensions/bosl2/rounding.py
+-rw-r--r--   0        0        0     2710 2023-03-21 16:33:14.956754 solidpython2-2.0.0b4/solid2/extensions/bosl2/screw_drive.py
+-rw-r--r--   0        0        0     5826 2023-03-21 16:33:14.064769 solidpython2-2.0.0b4/solid2/extensions/bosl2/screws.py
+-rw-r--r--   0        0        0    13484 2023-03-21 16:33:14.184767 solidpython2-2.0.0b4/solid2/extensions/bosl2/shapes2d.py
+-rw-r--r--   0        0        0    19503 2023-03-21 16:33:14.552761 solidpython2-2.0.0b4/solid2/extensions/bosl2/shapes3d.py
+-rw-r--r--   0        0        0    15362 2023-03-21 16:33:14.860756 solidpython2-2.0.0b4/solid2/extensions/bosl2/skin.py
+-rw-r--r--   0        0        0     1597 2023-03-21 16:33:14.944754 solidpython2-2.0.0b4/solid2/extensions/bosl2/sliders.py
+-rw-r--r--   0        0        0      679 2023-03-21 16:33:13.384780 solidpython2-2.0.0b4/solid2/extensions/bosl2/std.py
+-rw-r--r--   0        0        0     7243 2023-03-21 16:33:14.996754 solidpython2-2.0.0b4/solid2/extensions/bosl2/strings.py
+-rw-r--r--   0        0        0     1722 2023-03-21 16:33:14.584760 solidpython2-2.0.0b4/solid2/extensions/bosl2/structs.py
+-rw-r--r--   0        0        0    18126 2023-03-21 16:33:14.660759 solidpython2-2.0.0b4/solid2/extensions/bosl2/threading.py
+-rw-r--r--   0        0        0     8285 2023-03-21 16:33:14.432763 solidpython2-2.0.0b4/solid2/extensions/bosl2/transforms.py
+-rw-r--r--   0        0        0     4786 2023-03-21 16:33:14.408763 solidpython2-2.0.0b4/solid2/extensions/bosl2/trigonometry.py
+-rw-r--r--   0        0        0      611 2023-03-21 16:33:14.936754 solidpython2-2.0.0b4/solid2/extensions/bosl2/tripod_mounts.py
+-rw-r--r--   0        0        0     3060 2023-03-21 16:33:14.580760 solidpython2-2.0.0b4/solid2/extensions/bosl2/turtle3d.py
+-rw-r--r--   0        0        0     7807 2023-03-21 16:33:14.932755 solidpython2-2.0.0b4/solid2/extensions/bosl2/utility.py
+-rw-r--r--   0        0        0     4396 2023-03-21 16:33:13.892772 solidpython2-2.0.0b4/solid2/extensions/bosl2/vectors.py
+-rw-r--r--   0        0        0     1772 2023-03-21 16:33:14.724758 solidpython2-2.0.0b4/solid2/extensions/bosl2/version.py
+-rw-r--r--   0        0        0     9048 2023-03-21 16:33:14.720758 solidpython2-2.0.0b4/solid2/extensions/bosl2/vnf.py
+-rw-r--r--   0        0        0     2165 2023-03-21 16:33:15.044753 solidpython2-2.0.0b4/solid2/extensions/bosl2/walls.py
+-rw-r--r--   0        0        0     1045 2023-03-21 16:33:13.772774 solidpython2-2.0.0b4/solid2/extensions/bosl2/wiring.py
+-rwxr-xr-x   0        0        0     3830 2023-03-21 16:33:00.588994 solidpython2-2.0.0b4/solid2/extensions/bosl2_generator.py
+-rw-r--r--   0        0        0      264 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__init__.py
+-rw-r--r--   0        0        0      491 2022-12-15 09:17:23.702920 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      475 2022-08-12 15:59:23.623930 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2472 2023-03-19 13:06:07.916877 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__pycache__/customizer_widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2602 2022-11-04 17:06:42.607231 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__pycache__/customizer_widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     1865 2023-03-15 13:31:51.797247 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__pycache__/scad_interface.cpython-310.pyc
+-rw-r--r--   0        0        0     2010 2022-08-12 15:59:23.627930 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__pycache__/scad_interface.cpython-38.pyc
+-rw-r--r--   0        0        0     1388 2023-03-19 10:51:20.593500 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__pycache__/scad_variable.cpython-310.pyc
+-rw-r--r--   0        0        0     6322 2022-11-04 17:06:42.611231 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/__pycache__/scad_variable.cpython-38.pyc
+-rw-r--r--   0        0        0     1647 2023-03-19 12:43:05.633475 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/customizer_widgets.py
+-rw-r--r--   0        0        0      871 2023-03-15 13:23:46.114122 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/scad_interface.py
+-rw-r--r--   0        0        0     1034 2023-03-19 03:02:37.644529 solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/scad_variable.py
+-rwxr-xr-x   0        0        0     3570 2023-03-22 15:09:19.365226 solidpython2-2.0.0b4/solid2/extensions/openscad_extension_generator.py
+-rw-r--r--   0        0        0     2142 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/libs/BOSL2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1323 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/libs/BOSL2/LICENSE
+-rw-r--r--   0        0        0     2895 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/libs/BOSL2/README.md
+-rw-r--r--   0        0        0    37745 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/libs/BOSL2/WRITING_DOCS.md
+-rw-r--r--   0        0        0    16829 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/libs/BOSL2/affine.scad
+-rw-r--r--   0        0        0   136954 2022-08-12 15:59:10.187877 solidpython2-2.0.0b4/solid2/libs/BOSL2/attachments.scad
+-rw-r--r--   0        0        0    73284 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/beziers.scad
+-rw-r--r--   0        0        0     3677 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/bosl1compat.scad
+-rw-r--r--   0        0        0    46336 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/bottlecaps.scad
+-rw-r--r--   0        0        0     1257 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/builtins.scad
+-rw-r--r--   0        0        0     7630 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/color.scad
+-rw-r--r--   0        0        0    33970 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/comparisons.scad
+-rw-r--r--   0        0        0     8574 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/constants.scad
+-rw-r--r--   0        0        0    18570 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/coords.scad
+-rw-r--r--   0        0        0    26314 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/cubetruss.scad
+-rw-r--r--   0        0        0    53512 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/distributors.scad
+-rw-r--r--   0        0        0    59181 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/drawing.scad
+-rw-r--r--   0        0        0    56993 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/fnliterals.scad
+-rw-r--r--   0        0        0    62445 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/gears.scad
+-rw-r--r--   0        0        0   125013 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/geometry.scad
+-rw-r--r--   0        0        0     8985 2022-08-12 15:59:10.191877 solidpython2-2.0.0b4/solid2/libs/BOSL2/hingesnaps.scad
+-rw-r--r--   0        0        0   117043 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/images/BOSL2logo.png
+-rw-r--r--   0        0        0    55357 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/joiners.scad
+-rw-r--r--   0        0        0    30685 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/linalg.scad
+-rw-r--r--   0        0        0     5326 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/linear_bearings.scad
+-rw-r--r--   0        0        0    45059 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/lists.scad
+-rw-r--r--   0        0        0    21402 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/masks2d.scad
+-rw-r--r--   0        0        0    21715 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/masks3d.scad
+-rw-r--r--   0        0        0    54660 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/math.scad
+-rw-r--r--   0        0        0    23837 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/metric_screws.scad
+-rw-r--r--   0        0        0     8826 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/modular_hose.scad
+-rw-r--r--   0        0        0    19913 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/mutators.scad
+-rw-r--r--   0        0        0    28200 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/nema_steppers.scad
+-rw-r--r--   0        0        0    23428 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/partitions.scad
+-rw-r--r--   0        0        0    53553 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/paths.scad
+-rw-r--r--   0        0        0    44043 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/polyhedra.scad
+-rw-r--r--   0        0        0    60064 2022-08-12 15:59:10.195877 solidpython2-2.0.0b4/solid2/libs/BOSL2/regions.scad
+-rw-r--r--   0        0        0   217671 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/rounding.scad
+-rw-r--r--   0        0        0    11432 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/screw_drive.scad
+-rw-r--r--   0        0        0    79822 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/screws.scad
+-rwxr-xr-x   0        0        0      115 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/check_for_tabs.sh
+-rwxr-xr-x   0        0        0     2784 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/func_coverage.py
+-rwxr-xr-x   0        0        0     2345 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/img2scad.py
+-rwxr-xr-x   0        0        0      545 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/increment_version.sh
+-rwxr-xr-x   0        0        0      511 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/linecount.sh
+-rwxr-xr-x   0        0        0      368 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/purge_wiki_history.sh
+-rwxr-xr-x   0        0        0      790 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/run_tests.sh
+-rw-r--r--   0        0        0    79782 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/shapes2d.scad
+-rw-r--r--   0        0        0   148367 2022-08-12 15:59:10.199877 solidpython2-2.0.0b4/solid2/libs/BOSL2/shapes3d.scad
+-rw-r--r--   0        0        0   161752 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/skin.scad
+-rw-r--r--   0        0        0     6613 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/sliders.scad
+-rw-r--r--   0        0        0     1071 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/std.scad
+-rw-r--r--   0        0        0    33384 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/strings.scad
+-rw-r--r--   0        0        0     5016 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/structs.scad
+-rw-r--r--   0        0        0      186 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tests/README.txt
+-rw-r--r--   0        0        0    61268 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/threading.scad
+-rw-r--r--   0        0        0    59856 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/transforms.scad
+-rw-r--r--   0        0        0    15311 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/trigonometry.scad
+-rw-r--r--   0        0        0     4151 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tripod_mounts.scad
+-rw-r--r--   0        0        0    47847 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/turtle3d.scad
+-rw-r--r--   0        0        0    34615 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Attachments.md
+-rw-r--r--   0        0        0     6240 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Distributors.md
+-rw-r--r--   0        0        0     3329 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/FractalTree.md
+-rw-r--r--   0        0        0     7580 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Mutators.md
+-rw-r--r--   0        0        0    14849 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Paths.md
+-rw-r--r--   0        0        0    19937 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Shapes2d.md
+-rw-r--r--   0        0        0     9378 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Shapes3d.md
+-rw-r--r--   0        0        0     6679 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Transforms.md
+-rw-r--r--   0        0        0     7054 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/VNF.md
+-rw-r--r--   0        0        0    37101 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/utility.scad
+-rw-r--r--   0        0        0    25139 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/vectors.scad
+-rw-r--r--   0        0        0     6047 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/version.scad
+-rw-r--r--   0        0        0    73918 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/vnf.scad
+-rw-r--r--   0        0        0    15623 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/walls.scad
+-rw-r--r--   0        0        0     3421 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/BOSL2/wiring.scad
+-rw-r--r--   0        0        0        0 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/__init__.py
+-rw-r--r--   0        0        0      156 2022-12-15 10:15:59.164791 solidpython2-2.0.0b4/solid2/libs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      142 2022-08-12 15:59:23.631930 solidpython2-2.0.0b4/solid2/libs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7048 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/py_scadparser/LICENSE
+-rw-r--r--   0        0        0      640 2022-08-12 15:59:10.203877 solidpython2-2.0.0b4/solid2/libs/py_scadparser/README.md
+-rw-r--r--   0        0        0    44957 2023-03-21 17:34:01.432396 solidpython2-2.0.0b4/solid2/libs/py_scadparser/__pycache__/parsetab.cpython-310.pyc
+-rw-r--r--   0        0        0    34111 2022-08-12 15:50:00.790398 solidpython2-2.0.0b4/solid2/libs/py_scadparser/__pycache__/parsetab.cpython-38.pyc
+-rw-r--r--   0        0        0     3335 2023-03-21 17:34:01.396396 solidpython2-2.0.0b4/solid2/libs/py_scadparser/__pycache__/scad_ast.cpython-310.pyc
+-rw-r--r--   0        0        0     2735 2022-08-12 15:59:23.635930 solidpython2-2.0.0b4/solid2/libs/py_scadparser/__pycache__/scad_ast.cpython-38.pyc
+-rw-r--r--   0        0        0    10330 2023-03-21 16:33:13.380780 solidpython2-2.0.0b4/solid2/libs/py_scadparser/__pycache__/scad_parser.cpython-310.pyc
+-rw-r--r--   0        0        0    10490 2022-08-12 15:49:20.526338 solidpython2-2.0.0b4/solid2/libs/py_scadparser/__pycache__/scad_parser.cpython-38.pyc
+-rw-r--r--   0        0        0     2848 2023-03-21 16:33:13.384780 solidpython2-2.0.0b4/solid2/libs/py_scadparser/__pycache__/scad_tokens.cpython-310.pyc
+-rw-r--r--   0        0        0     2977 2022-08-12 15:50:00.766398 solidpython2-2.0.0b4/solid2/libs/py_scadparser/__pycache__/scad_tokens.cpython-38.pyc
+-rw-r--r--   0        0        0    48312 2023-03-23 17:47:21.609266 solidpython2-2.0.0b4/solid2/libs/py_scadparser/parsetab.py
+-rw-r--r--   0        0        0     1229 2023-03-23 17:47:21.609266 solidpython2-2.0.0b4/solid2/libs/py_scadparser/scad_ast.py
+-rw-r--r--   0        0        0     8328 2023-03-23 17:47:21.609266 solidpython2-2.0.0b4/solid2/libs/py_scadparser/scad_parser.py
+-rw-r--r--   0        0        0     2745 2023-03-21 16:32:26.613592 solidpython2-2.0.0b4/solid2/libs/py_scadparser/scad_tokens.py
+-rw-r--r--   0        0        0    24644 1970-01-01 00:00:00.000000 solidpython2-2.0.0b4/setup.py
+-rw-r--r--   0        0        0    24248 1970-01-01 00:00:00.000000 solidpython2-2.0.0b4/PKG-INFO
```

### Comparing `solidpython2-2.0.0b3/README.rst` & `solidpython2-2.0.0b4/README.rst`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/pyproject.toml` & `solidpython2-2.0.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solidpython2"
-version = "2.0.0-beta-03"
+version = "2.0.0-beta-04"
 description = "Python interface to the OpenSCAD declarative geometry language"
 authors = ["jeff"]
 homepage = "https://github.com/jeff-dh/SolidPython"
 repository = "https://github.com/jeff-dh/SolidPython"
 license = "LGPL-2.1"
 readme = "README.rst"
 keywords = [
```

### Comparing `solidpython2-2.0.0b3/solid2/config.py` & `solidpython2-2.0.0b4/solid2/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,23 +5,20 @@
 import sys
 import re
 
 class Config:
     def __init__(self):
         self.use_implicit_builtins = "--implicit" in sys.argv
 
-        builtins_suffix = ".openscad" if not self.use_implicit_builtins else ".implicit"
-        self.builtins_file = Path(__file__).absolute().parent / ("core/builtins" + builtins_suffix)
-
         self.enable_pickle_cache = True
         self.pickle_cache_dir = self.get_pickle_cache_dir()
 
-        self.openscad_library_paths = self.openscad_library_paths()
+        self.openscad_library_paths = self.get_openscad_library_paths()
 
-    def openscad_library_paths(self):
+    def get_openscad_library_paths(self):
         """
         Return system-dependent OpenSCAD library paths or paths defined in
         os.environ['OPENSCADPATH'] """
         paths = [Path('.')]
 
         user_path = os.environ.get('OPENSCADPATH')
         if user_path:
@@ -36,15 +33,15 @@
         }
 
         paths.append(default_paths[platform.system()])
 
         #system wide paths
         if platform.system() == 'Linux':
             #sorry, but I've no clue what the paths are on other operating systems
-            paths.append("/usr/share/openscad/libraries")
+            paths.append(Path("/usr/share/openscad/libraries"))
 
         return paths
 
     def get_pickle_cache_dir(self):
         default_paths = {
             'Linux':   Path.home() / '.local/share/expSolidPython/pickle_cache',
             'Darwin':  Path.home() / 'Documents/expSolidPython/pickle_cache',
```

### Comparing `solidpython2-2.0.0b3/solid2/core/accessSyntaxBase.py` & `solidpython2-2.0.0b4/solid2/core/object_base/access_syntax_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-from ..config import config
+from ...config import config
 
 def builtins():
-    from . import builtins
+    from .. import builtins
     return builtins
 
-class AccessSyntaxBase:
+class AccessSyntaxMixin:
     if not config.use_implicit_builtins:
         def intersection_for(self, n):     return builtins().intersection_for(n)(self)
         def color(self, color, alpha=1.0): return builtins().color(color, alpha)(self)
         def hull(self):                    return builtins().hull()(self)
         def render(self, convexity=None):  return builtins().render(convexity)(self)
-        def projection(self, cut=None):    return builtins().projection(cut=None)(self)
+        def projection(self, cut=None):    return builtins().projection(cut)(self)
 
         def surface(self, file, center=None, convexity=None, invert=None):
             return builtins().surface(file, center, convexity, invert)(self)
         def offset(self, r=None, delta=None, chamfer=None, _fn=None):
             return builtins().offset(r, delta, chamfer, _fn)(self)
 
         def mirror(self, *args, **kwargs): return builtins().mirror(*args, **kwargs)(self)
         def resize(self, *args, **kwargs): return builtins().resize(*args, **kwargs)(self)
 
-        def mirrorX(self, x): return builtins().mirrorX(x)(self)
-        def mirrorY(self, y): return builtins().mirrorY(y)(self)
-        def mirrorZ(self, z): return builtins().mirrorZ(z)(self)
+        def mirrorX(self): return builtins().mirrorX()(self)
+        def mirrorY(self): return builtins().mirrorY()(self)
+        def mirrorZ(self): return builtins().mirrorZ()(self)
 
         def resizeX(self, x): return builtins().resizeX(x)(self)
         def resizeY(self, y): return builtins().resizeY(y)(self)
         def resizeZ(self, z): return builtins().resizeZ(z)(self)
 
     def union(self):          return builtins().union()(self)
     def difference(self):     return builtins().difference()(self)
     def intersection(self):   return builtins().intersection()(self)
 
 
     def rotate_extrude(self, angle=None, convexity=None, _fn=None):
-        return builtins().rotate_extrude(*args, **kwargs)(self)
+        return builtins().rotate_extrude(angle, convexity, _fn)(self)
+
     def linear_extrude(self, height=None, center=None, convexity=None, \
                        twist=None, slices=None, scale=None):
-        return builtins().linear_extrude(height, center, convexity, twist, slices, scale)(self)
+        return builtins().linear_extrude(height, center, convexity, twist,
+                                         slices, scale)(self)
 
     def translate(self, *args, **kwargs): return builtins().translate(*args, **kwargs)(self)
     def scale(self, *args, **kwargs):     return builtins().scale(*args, **kwargs)(self)
     def rotate(self, *args, **kwargs):    return builtins().rotate(*args, **kwargs)(self)
 
     def down(self, z):    return builtins().down(z)(self)
     def up(self, z):      return builtins().up(z)(self)
```

### Comparing `solidpython2-2.0.0b3/solid2/core/builtin_primitives.py` & `solidpython2-2.0.0b4/solid2/core/builtins/openscad_primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .object_base import OpenSCADObject
+from ..object_base import OpenSCADObject
 
 from pathlib import Path
-from typing import Dict, Optional, Sequence, Tuple, Union, List
+from typing import Sequence, Tuple, Union
 
 PathStr = Union[Path, str]
 
 P2 = Tuple[float, float]
 P3 = Tuple[float, float, float]
 P4 = Tuple[float, float, float, float]
 Vec3 = P3
@@ -21,19 +21,19 @@
 class polygon(OpenSCADObject):
     """
     Create a polygon with the specified points and paths.
 
     :param points: the list of points of the polygon
     :type points: sequence of 2 element sequences
 
-    :param paths: Either a single vector, enumerating the point list, ie. the 
-    order to traverse the points, or, a vector of vectors, ie a list of point 
-    lists for each separate curve of the polygon. The latter is required if the 
-    polygon has holes. The parameter is optional and if omitted the points are 
-    assumed in order. (The 'pN' components of the *paths* vector are 0-indexed 
+    :param paths: Either a single vector, enumerating the point list, ie. the
+    order to traverse the points, or, a vector of vectors, ie a list of point
+    lists for each separate curve of the polygon. The latter is required if the
+    polygon has holes. The parameter is optional and if omitted the points are
+    assumed in order. (The 'pN' components of the *paths* vector are 0-indexed
     references to the elements of the *points* vector.)
 
     :param convexity: OpenSCAD's convexity... yadda yadda
 
     NOTE: OpenSCAD accepts only 2D points for `polygon()`. Convert any 3D points
     to 2D before compiling
     """
@@ -75,21 +75,21 @@
 class square(OpenSCADObject):
     """
     Creates a square at the origin of the coordinate system. When center is
     True the square will be centered on the origin, otherwise it is created
     in the first quadrant. The argument names are optional if the arguments
     are given in the same order as specified in the parameters
 
-    :param size: If a single number is given, the result will be a square with 
-    sides of that length. If a 2 value sequence is given, then the values will 
+    :param size: If a single number is given, the result will be a square with
+    sides of that length. If a 2 value sequence is given, then the values will
     correspond to the lengths of the X and Y sides.  Default value is 1.
     :type size: number or 2 value sequence
 
-    :param center: This determines the positioning of the object. If True, 
-    object is centered at (0,0). Otherwise, the square is placed in the positive 
+    :param center: This determines the positioning of the object. If True,
+    object is centered at (0,0). Otherwise, the square is placed in the positive
     quadrant with one corner at (0,0). Defaults to False.
     :type center: boolean
     """
 
     def __init__(self, size: ScadSize = None, center: bool = None) -> None:
         super().__init__('square',
                          {'size': size, 'center': center})
@@ -118,21 +118,21 @@
 class cube(OpenSCADObject):
     """
     Creates a cube at the origin of the coordinate system. When center is
     True the cube will be centered on the origin, otherwise it is created in
     the first octant. The argument names are optional if the arguments are
     given in the same order as specified in the parameters
 
-    :param size: If a single number is given, the result will be a cube with 
-    sides of that length. If a 3 value sequence is given, then the values will 
+    :param size: If a single number is given, the result will be a cube with
+    sides of that length. If a 3 value sequence is given, then the values will
     correspond to the lengths of the X, Y, and Z sides. Default value is 1.
     :type size: number or 3 value sequence
 
-    :param center: This determines the positioning of the object. If True, 
-    object is centered at (0,0,0). Otherwise, the cube is placed in the positive 
+    :param center: This determines the positioning of the object. If True,
+    object is centered at (0,0,0). Otherwise, the cube is placed in the positive
     quadrant with one corner at (0,0,0). Defaults to False
     :type center: boolean
     """
 
     def __init__(self, size: ScadSize = None, center: bool = None) -> None:
         super().__init__('cube',
                          {'size': size, 'center': center})
@@ -143,15 +143,15 @@
     Creates a cylinder or cone at the origin of the coordinate system. A
     single radius (r) makes a cylinder, two different radii (r1, r2) make a
     cone.
 
     :param h: This is the height of the cylinder. Default value is 1.
     :type h: number
 
-    :param r: The radius of both top and bottom ends of the cylinder. Use this 
+    :param r: The radius of both top and bottom ends of the cylinder. Use this
     parameter if you want plain cylinder. Default value is 1.
     :type r: number
 
     :param r1: This is the radius of the cone on bottom end. Default value is 1.
     :type r1: number
 
     :param r2: This is the radius of the cone on top end. Default value is 1.
@@ -163,16 +163,16 @@
 
     :param d1: This is the diameter of the cone on bottom end. Default value is 1.
     :type d1: number
 
     :param d2: This is the diameter of the cone on top end. Default value is 1.
     :type d2: number
 
-    :param center: If True will center the height of the cone/cylinder around 
-    the origin. Default is False, placing the base of the cylinder or r1 radius 
+    :param center: If True will center the height of the cone/cylinder around
+    the origin. Default is False, placing the base of the cylinder or r1 radius
     of cone at the origin.
     :type center: boolean
 
     :param _fn: Number of fragments in 360 degrees.
     :type _fn: int
     """
 
@@ -192,27 +192,27 @@
     relate to the surfaces of the polyhedron.
 
     *note: if your version of OpenSCAD is lower than 2014.03 replace "faces"
     with "triangles" in the below examples*
 
     :param points: sequence of points or vertices (each a 3 number sequence).
 
-    :param triangles: (*deprecated in version 2014.03, use faces*) vector of 
-    point triplets (each a 3 number sequence). Each number is the 0-indexed point 
+    :param triangles: (*deprecated in version 2014.03, use faces*) vector of
+    point triplets (each a 3 number sequence). Each number is the 0-indexed point
     number from the point vector.
 
-    :param faces: (*introduced in version 2014.03*) vector of point n-tuples 
-    with n >= 3. Each number is the 0-indexed point number from the point vector.  
-    That is, faces=[[0,1,4]] specifies a triangle made from the first, second, 
-    and fifth point listed in points. When referencing more than 3 points in a 
+    :param faces: (*introduced in version 2014.03*) vector of point n-tuples
+    with n >= 3. Each number is the 0-indexed point number from the point vector.
+    That is, faces=[[0,1,4]] specifies a triangle made from the first, second,
+    and fifth point listed in points. When referencing more than 3 points in a
     single tuple, the points must all be on the same plane.
 
-    :param convexity: The convexity parameter specifies the maximum number of 
-    front sides (back sides) a ray intersecting the object might penetrate. This 
-    parameter is only needed for correctly displaying the object in OpenCSG 
+    :param convexity: The convexity parameter specifies the maximum number of
+    front sides (back sides) a ray intersecting the object might penetrate. This
+    parameter is only needed for correctly displaying the object in OpenCSG
     preview mode and has no effect on the polyhedron rendering.
     :type convexity: int
     """
 
     def __init__(self, points: P3s, faces: Indexes, convexity: int = None, triangles: Indexes = None) -> None:
         super().__init__('polyhedron',
                          {'points': points, 'faces': faces,
@@ -304,15 +304,15 @@
 
 class resize(OpenSCADObject):
     """
     Modify the size of the child object to match the given new size.
 
     :param newsize: X, Y and Z values
     :type newsize: 3 value sequence
-    
+
     :param auto: 3-tuple of booleans to specify which axes should be scaled
     :type auto: 3 boolean sequence
     """
 
     def __init__(self, newsize: Vec3, auto: Tuple[bool, bool, bool] = None) -> None:
         super().__init__('resize', {'newsize': newsize, 'auto': auto})
 
@@ -337,15 +337,15 @@
     currently support color. The alpha value will default to 1.0 (opaque) if
     not specified.
 
     :param c: RGB color + alpha value.
     :type c: sequence of 3 or 4 numbers between 0 and 1, OR 3-, 4-, 6-, or 8-digit RGB/A hex code, OR string color name as described at https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Transformations#color
 
     :param alpha: Alpha value from 0 to 1
-    :type alpha: float 
+    :type alpha: float
     """
 
     def __init__(self, c: Union[Vec34, str], alpha: float = 1.0) -> None:
         super().__init__('color', {'c': c, 'alpha': alpha})
 
 
 class minkowski(OpenSCADObject):
@@ -357,27 +357,27 @@
 
     def __init__(self) -> None:
         super().__init__('minkowski', {})
 
 
 class offset(OpenSCADObject):
     """
-    
-    :param r: Amount to offset the polygon (rounded corners). When negative, 
-        the polygon is offset inwards. The parameter r specifies the radius 
+
+    :param r: Amount to offset the polygon (rounded corners). When negative,
+        the polygon is offset inwards. The parameter r specifies the radius
         that is used to generate rounded corners, using delta gives straight edges.
     :type r: number
-    
-    :param delta: Amount to offset the polygon (sharp corners). When negative, 
-        the polygon is offset inwards. The parameter r specifies the radius 
+
+    :param delta: Amount to offset the polygon (sharp corners). When negative,
+        the polygon is offset inwards. The parameter r specifies the radius
         that is used to generate rounded corners, using delta gives straight edges.
     :type delta: number
-    
-    :param chamfer: When using the delta parameter, this flag defines if edges 
-        should be chamfered (cut off with a straight line) or not (extended to 
+
+    :param chamfer: When using the delta parameter, this flag defines if edges
+        should be chamfered (cut off with a straight line) or not (extended to
         their intersection).
     :type chamfer: bool
 
     :param _fn: Resolution of any radial curves
     :type _fn: int
     """
 
@@ -426,22 +426,22 @@
 
     :param height: the extrusion height.
     :type height: number
 
     :param center: determines if the object is centered on the Z-axis after extrusion.
     :type center: boolean
 
-    :param convexity: The convexity parameter specifies the maximum number of 
-    front sides (back sides) a ray intersecting the object might penetrate. This 
-    parameter is only needed for correctly displaying the object in OpenCSG 
+    :param convexity: The convexity parameter specifies the maximum number of
+    front sides (back sides) a ray intersecting the object might penetrate. This
+    parameter is only needed for correctly displaying the object in OpenCSG
     preview mode and has no effect on the polyhedron rendering.
     :type convexity: int
 
-    :param twist: Twist is the number of degrees of through which the shape is 
-    extruded.  Setting to 360 will extrude through one revolution.  The twist 
+    :param twist: Twist is the number of degrees of through which the shape is
+    extruded.  Setting to 360 will extrude through one revolution.  The twist
     direction follows the left hand rule.
     :type twist: number
 
     :param slices: number of slices to extrude. Can be used to improve the output.
     :type slices: int
 
     :param scale: relative size of the top of the extrusion compared to the start
@@ -467,25 +467,25 @@
     The 2D shape needs to be either completely on the positive, or negative
     side (not recommended), of the X axis. It can touch the axis, i.e. zero,
     however if the shape crosses the X axis a warning will be shown in the
     console windows and the rotate/_extrude() will be ignored. If the shape
     is in the negative axis the faces will be inside-out, you probably don't
     want to do that; it may be fixed in the future.
 
-    :param angle: Defaults to 360. Specifies the number of degrees to sweep, 
-    starting at the positive X axis. The direction of the sweep follows the 
+    :param angle: Defaults to 360. Specifies the number of degrees to sweep,
+    starting at the positive X axis. The direction of the sweep follows the
     Right Hand Rule, hence a negative angle will sweep clockwise.
     :type angle: number
-    
+
     :param _fn: Number of fragments in 360 degrees.
     :type _fn: int
 
-    :param convexity: The convexity parameter specifies the maximum number of 
-    front sides (back sides) a ray intersecting the object might penetrate. This 
-    parameter is only needed for correctly displaying the object in OpenCSG 
+    :param convexity: The convexity parameter specifies the maximum number of
+    front sides (back sides) a ray intersecting the object might penetrate. This
+    parameter is only needed for correctly displaying the object in OpenCSG
     preview mode and has no effect on the polyhedron rendering.
     :type convexity: int
 
     """
 
     def __init__(self, angle: float = 360, convexity: int = None, _fn: int = None) -> None:
         super().__init__('rotate_extrude',
@@ -505,16 +505,16 @@
 
 
 class projection(OpenSCADObject):
     """
     Creates 2d shapes from 3d models, and export them to the dxf format.
     It works by projecting a 3D model to the (x,y) plane, with z at 0.
 
-    :param cut: when True only points with z=0 will be considered (effectively 
-    cutting the object) When False points above and below the plane will be 
+    :param cut: when True only points with z=0 will be considered (effectively
+    cutting the object) When False points above and below the plane will be
     considered as well (creating a proper projection).
     :type cut: boolean
     """
 
     def __init__(self, cut: bool = None) -> None:
         super().__init__('projection', {'cut': cut})
 
@@ -522,82 +522,82 @@
 class surface(OpenSCADObject):
     """
     Surface reads information from text or image files.
 
     :param file: The path to the file containing the heightmap data.
     :type file: PathStr
 
-    :param center: This determines the positioning of the generated object. If 
-    True, object is centered in X- and Y-axis. Otherwise, the object is placed 
+    :param center: This determines the positioning of the generated object. If
+    True, object is centered in X- and Y-axis. Otherwise, the object is placed
     in the positive quadrant. Defaults to False.
     :type center: boolean
 
-    :param invert: Inverts how the color values of imported images are translated 
-    into height values. This has no effect when importing text data files. 
+    :param invert: Inverts how the color values of imported images are translated
+    into height values. This has no effect when importing text data files.
     Defaults to False.
     :type invert: boolean
 
-    :param convexity: The convexity parameter specifies the maximum number of 
-    front sides (back sides) a ray intersecting the object might penetrate. 
-    This parameter is only needed for correctly displaying the object in OpenCSG 
+    :param convexity: The convexity parameter specifies the maximum number of
+    front sides (back sides) a ray intersecting the object might penetrate.
+    This parameter is only needed for correctly displaying the object in OpenCSG
     preview mode and has no effect on the polyhedron rendering.
     :type convexity: int
     """
 
     def __init__(self, file, center: bool = None, convexity: int = None, invert=None) -> None:
         super().__init__('surface',
                          {'file': file, 'center': center,
                           'convexity': convexity, 'invert': invert})
 
 
 class text(OpenSCADObject):
     """
-    Create text using fonts installed on the local system or provided as separate 
+    Create text using fonts installed on the local system or provided as separate
     font file.
 
     :param text: The text to generate.
     :type text: string
 
-    :param size: The generated text will have approximately an ascent of the given 
-    value (height above the baseline). Default is 10.  Note that specific fonts 
-    will vary somewhat and may not fill the size specified exactly, usually 
+    :param size: The generated text will have approximately an ascent of the given
+    value (height above the baseline). Default is 10.  Note that specific fonts
+    will vary somewhat and may not fill the size specified exactly, usually
     slightly smaller.
     :type size: number
 
-    :param font: The name of the font that should be used. This is not the name 
-    of the font file, but the logical font name (internally handled by the 
-    fontconfig library). A list of installed fonts can be obtained using the 
+    :param font: The name of the font that should be used. This is not the name
+    of the font file, but the logical font name (internally handled by the
+    fontconfig library). A list of installed fonts can be obtained using the
     font list dialog (Help -> Font List).
     :type font: string
 
-    :param halign: The horizontal alignment for the text. Possible values are 
+    :param halign: The horizontal alignment for the text. Possible values are
     "left", "center" and "right". Default is "left".
     :type halign: string
 
-    :param valign: The vertical alignment for the text. Possible values are 
+    :param valign: The vertical alignment for the text. Possible values are
     "top", "center", "baseline" and "bottom". Default is "baseline".
     :type valign: string
 
-    :param spacing: Factor to increase/decrease the character spacing.  The 
-    default value of 1 will result in the normal spacing for the font, giving 
+    :param spacing: Factor to increase/decrease the character spacing.  The
+    default value of 1 will result in the normal spacing for the font, giving
     a value greater than 1 will cause the letters to be spaced further apart.
     :type spacing: number
 
-    :param direction: Direction of the text flow. Possible values are "ltr" 
-    (left-to-right), "rtl" (right-to-left), "ttb" (top-to-bottom) and "btt" 
+    :param direction: Direction of the text flow. Possible values are "ltr"
+    (left-to-right), "rtl" (right-to-left), "ttb" (top-to-bottom) and "btt"
     (bottom-to-top). Default is "ltr".
     :type direction: string
 
     :param language: The language of the text. Default is "en".
     :type language: string
 
     :param script: The script of the text. Default is "latin".
     :type script: string
 
-    :param _fn: used for subdividing the curved path _fn provided by 
+    :param _fn: used for subdividing the curved path _fn provided by
     freetype
     :type _fn: int
     """
 
     def __init__(self, text: str, size: float = None, font: str = None, halign: str = None,
                  valign: str = None, spacing: float = None, direction: str = None,
                  language: str = None, script: str = None, _fn: int = None) -> None:
@@ -618,19 +618,19 @@
 
 class children(OpenSCADObject):
     """
     The child nodes of the module instantiation can be accessed using the
     children() statement within the module. The number of module children
     can be accessed using the $children variable.
 
-    :param index: select one child, at index value. Index start at 0 and should 
+    :param index: select one child, at index value. Index start at 0 and should
     be less than or equal to $children-1.
     :type index: int
 
-    :param vector: select children with index in vector. Index should be between 
+    :param vector: select children with index in vector. Index should be between
     0 and $children-1.
     :type vector: sequence of int
 
     :param range: [:] or [::]. select children between to , incremented by (default 1).
     """
 
     def __init__(self, index: int = None, vector: float = None, range: P23 = None) -> None:
@@ -657,26 +657,28 @@
     """
     Imports a file for use in the current OpenSCAD model. OpenSCAD currently
     supports import of DXF and STL (both ASCII and Binary) files.
 
     :param file: path to the STL or DXF file.
     :type file: PathStr
 
-    :param convexity: The convexity parameter specifies the maximum number of 
-    front sides (back sides) a ray intersecting the object might penetrate. This 
-    parameter is only needed for correctly displaying the object in OpenCSG 
+    :param convexity: The convexity parameter specifies the maximum number of
+    front sides (back sides) a ray intersecting the object might penetrate. This
+    parameter is only needed for correctly displaying the object in OpenCSG
     preview mode and has no effect on the polyhedron rendering.
     :type convexity: int
     """
 
     def __init__(self, file: PathStr, origin: P2 = (0, 0), convexity: int = None, layer: int = None) -> None:
         super().__init__('import',
                          {'file': Path(file).as_posix(), 'origin': origin,
                           'convexity': convexity, 'layer': layer})
 
+class _import(import_): pass
+
 
 class intersection_for(OpenSCADObject):
     """
     Iterate over the values in a vector or range and take an
     intersection of the contents.
     """
```

### Comparing `solidpython2-2.0.0b3/solid2/core/builtins.implicit` & `solidpython2-2.0.0b4/solid2/core/builtins/implicit.primitives`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/core/builtins.openscad` & `solidpython2-2.0.0b4/solid2/core/builtins/openscad.primitives`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 module import_stl(file, origin=default, convexity=default, layer=default);
 module import_dxf(file, origin=default, convexity=default, layer=default);
 module import(file, origin=default, convexity=default, layer=default);
 
 module assign();
 module multmatrix(m=default);
 
-//builtin primitives
 module polygon(points, paths=default, convexity=default);
 module circle(r=default, d=default, $fn=default);
 module square(size=default, center=default);
 module sphere(r=default, d=default, $fn=default);
 module cube(size=default, center=default);
 module cylinder(r=default, h=default, r1=default, r2=default,
                 d=default, d1=default, d2=default, center=default, $fn=default);
```

### Comparing `solidpython2-2.0.0b3/solid2/core/builtins.py` & `solidpython2-2.0.0b4/solid2/core/builtins/convenience.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-from .scad_import import use
-from .object_base import ObjectBase
-from ..config import config
-
-# ====================
-# = dynamic builtins =
-# ====================
-"""
-    This loads all the built in OpenSCAD functions (like circle, square, color,
-    translate.....) from builtins.openscad file.
-    I intentionally didn't use a *.scad file because it would be ignore through
-    .gitignore und would be a pain to maintain (unless we remove *.scad from
-    .gitignore, but that would cause a lot of generated files to show up while
-    developing...).
-"""
-if config.use_implicit_builtins:
-    use(config.builtins_file, skip_render=True)
-else:
-    from .builtin_primitives import *
+from ...config import config
+from ..object_base import ObjectBase
+from .primitives import *
 
 # =============
 # = modifiers =
 # =============
 class ModifierBase(ObjectBase):
     def __init__(self, child=None):
         super().__init__()
         if child:
-            self.children += [child]
+            self._children += [child]
 
 class debug(ModifierBase):
     def _render(self):
         return "#" + super()._render()
 
 class background(ModifierBase):
     def _render(self):
```

### Comparing `solidpython2-2.0.0b3/solid2/core/extension_manager.py` & `solidpython2-2.0.0b4/solid2/core/extension_manager.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/core/object_base.py` & `solidpython2-2.0.0b4/solid2/core/object_base/object_base_impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,123 @@
-from .accessSyntaxBase import AccessSyntaxBase
-from .operatorBase import OperatorBase
+from .access_syntax_mixin import AccessSyntaxMixin
+from .operator_mixin import OperatorMixin
 
 #don't do relative imports on the global scope to be able to import this file
 #from "everywhere"
 
-class ObjectBaseInterface(AccessSyntaxBase, OperatorBase):
-    def _render(self):
-        return ""
-
+class RenderMixin:
     def __repr__(self):
         return self.as_scad()
 
     def as_scad(self):
-        from .scad_render import scad_render
+        from ..scad_render import scad_render
         return scad_render(self)[:-1]
 
     def save_as_scad(self, filename='', outdir=''):
-        from .scad_render import scad_render_to_file
+        from ..scad_render import scad_render_to_file
         return scad_render_to_file(self, filename, outdir)
 
     def save_as_stl(self, filename='', outdir=''):
-        from .scad_render import render_to_stl_file
+        from ..scad_render import render_to_stl_file
         return render_to_stl_file(self, filename)
 
-class ObjectBase(ObjectBaseInterface):
+class ObjectBase(RenderMixin):
     def __init__(self):
-        self.children = []
+        self._children = []
 
     def add(self, c):
         def _add(c):
             assert(hasattr(c, "_render"))
-            self.children += [c]
+            self._children += [c]
 
         if isinstance(c, list):
             for cc in c:
                 _add(cc)
         else:
             _add(c)
 
         return self
 
     def _render(self):
         s = ''
-        for c in self.children:
+        for c in self._children:
             s += c._render()
         return s
 
     def __call__(self, *args):
         #translate(...)(cube())
-        #this adds cube() to translate.children
+        #this adds cube() to translate._children
         for a in args:
             self.add(a)
         return self
 
-class OpenSCADObject(ObjectBase):
+
+class BareOpenSCADObject(ObjectBase):
     def __init__(self, name, params):
         super().__init__()
-        self.name = name
-        self.params = params
+        self._name = name
+        self._params = params
 
     def _render(self):
         """
             returns the scad code for a given node tuple consiting of name,
             params and children list.
 
             -> translate(v = [1, 2, 3]) {children[0]; children[1]; ...};\n
         """
-        from .utils import indent
-        s = self.generate_scad_head()
+        from ..utils import indent
+        s = self._generate_scad_head()
 
-        if self.children:
+        if self._children:
             s += " {\n"
-            for child in self.children:
+            for child in self._children:
                 s += indent(child._render())
             s += "}"
         else:
             s += ";"
 
         return s + "\n"
 
-    def generate_scad_head(self):
+    def _generate_scad_head(self):
         """
             for a given function name and dict of params it returns:
                 {name}(p1=v1, p2=v2,...)
                 -> translate(v = [1, 2, 3])
         """
-        from .utils import unescape_openscad_identifier, py2openscad
-        from ..config import config
+        from ..utils import unescape_openscad_identifier, py2openscad
+        from ...config import config
 
         param_strings = []
-        for p in sorted(self.params.keys()):
-            if self.params[p] is None:
+        for p in sorted(self._params.keys()):
+            if self._params[p] is None:
                 continue
 
             if config.use_implicit_builtins and \
-                        isinstance(self.params[p], OpenSCADParameterFunction):
+                        isinstance(self._params[p], OpenSCADParameterFunction):
 
-                param_strings.append(self.params[p]._render())
+                param_strings.append(self._params[p]._render())
             else:
-                scad_value = py2openscad(self.params[p])
+                scad_value = py2openscad(self._params[p])
                 scad_identifier = unescape_openscad_identifier(p)
 
                 param_strings.append(f'{scad_identifier} = {scad_value}')
 
-        scad_identifier = unescape_openscad_identifier(self.name)
+        scad_identifier = unescape_openscad_identifier(self._name)
         param_str = ", ".join(param_strings)
 
         return f'{scad_identifier}({param_str})'
 
+class OpenSCADObject(AccessSyntaxMixin, OperatorMixin, BareOpenSCADObject):
+    pass
+
 class OpenSCADConstant:
     def __init__(self, value):
         self.value = value
 
-        from .utils import escape_openscad_identifier
+        from ..utils import escape_openscad_identifier
         self.__doc__ = escape_openscad_identifier(value)
 
     def __repr__(self):
         return f'{self.value}'
 
     def __operator_base__(self, op, other):
         return OpenSCADConstant(f'({self} {op} {other})')
```

### Comparing `solidpython2-2.0.0b3/solid2/core/object_factory.py` & `solidpython2-2.0.0b4/solid2/core/object_factory.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/core/operatorBase.py` & `solidpython2-2.0.0b4/solid2/core/object_base/operator_mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 
-class OperatorBase:
-    def union_op(self, x):
+class OperatorMixin:
+    def _union_op(self, x, unionType):
         """
         This makes u = a+b identical to:
         u = union()(a, b )
         """
-        from . import builtins
-        res = builtins.union()
+        res = unionType()
 
         #add self or all its children to res
-        if isinstance(self, builtins.union):
-            for c in self.children:
+        if isinstance(self, unionType):
+            for c in self._children:
                 res.add(c)
         else:
             res.add(self)
 
         #add x or all its children to res
-        if isinstance(x, builtins.union):
-            for c in x.children:
+        if isinstance(x, unionType):
+            for c in x._children:
                 res.add(c)
         else:
             res.add(x)
 
         return res
 
-    def difference_op(self, x):
+    def _difference_op(self, x, differenceType):
         """
         This makes u = a - b identical to:
         u = difference()(a, b )
         """
-        from . import builtins
-        res = builtins.difference()
+        res = differenceType()
 
-        if isinstance(self, builtins.difference) and len(self.children):
-            for c in self.children:
+        if isinstance(self, differenceType) and len(self._children):
+            for c in self._children:
                 res.add(c)
         else:
             res.add(self)
 
         res.add(x)
         return res
 
-    def intersection_op(self, x):
+    def _intersection_op(self, x, intersectionType):
         """
         This makes u = a * b identical to:
         u = intersection()(a, b )
         """
-        from . import builtins
-        res = builtins.intersection()
+        res = intersectionType()
 
-        if isinstance(self, builtins.intersection) and len(self.children):
-            for c in self.children:
+        if isinstance(self, intersectionType) and len(self._children):
+            for c in self._children:
                 res.add(c)
         else:
             res.add(self)
 
-        if isinstance(x, builtins.intersection):
-            for c in x.children:
+        if isinstance(x, intersectionType):
+            for c in x._children:
                 res.add(c)
         else:
             res.add(x)
 
         return res
 
-    def __add__(self, x): return self.union_op(x)
-    def __or__(self, x): return self.union_op(x)
-    def __radd__(self, x): return self.union_op(x)
-    def __sub__(self, x): return self.difference_op(x)
-    def __mul__(self, x): return self.intersection_op(x)
-    def __and__(self, x): return self.intersection_op(x)
-    def __invert__(self): from . import builtins; return builtins.debug()(self)
+    def __add__(self, x):
+        from ..builtins import union
+        return self._union_op(x, union)
+    def __or__(self, x):
+        from ..builtins import union
+        return self._union_op(x, union)
+    def __radd__(self, x):
+        from ..builtins import union
+        return self._union_op(x, union)
+    def __sub__(self, x):
+        from ..builtins import difference
+        return self._difference_op(x, difference)
+    def __mul__(self, x):
+        from ..builtins import intersection
+        return self._intersection_op(x, intersection)
+    def __and__(self, x):
+        from ..builtins import intersection
+        return self._intersection_op(x, intersection)
+    def __invert__(self):
+        from .. import builtins; return builtins.debug()(self)
```

### Comparing `solidpython2-2.0.0b3/solid2/core/parse_scad.py` & `solidpython2-2.0.0b4/solid2/core/parse_scad.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,19 @@
             callables.append(callables_entry(c.name, [], kwargs))
 
         #write the read version to disk so we can probably use it the next time
         update_pickle_cache(filename, callables, global_vars)
 
     #create a wrapper for each callable and add it to the dict
     new_namespace_dict = {}
-    for c in callables:
-        wrapper = create_openscad_wrapper_from_symbols(c.name, [], c.kwargs)
-        new_namespace_dict[escape_openscad_identifier(c.name)] = wrapper
+    if callables:
+        for c in callables:
+            wrapper = create_openscad_wrapper_from_symbols(c.name, [], c.kwargs)
+            new_namespace_dict[escape_openscad_identifier(c.name)] = wrapper
 
-    for c in global_vars:
-        new_namespace_dict[escape_openscad_identifier(c.name)] = \
+    if global_vars:
+        for c in global_vars:
+            new_namespace_dict[escape_openscad_identifier(c.name)] = \
                                                         OpenSCADConstant(c.name)
 
     return new_namespace_dict
```

### Comparing `solidpython2-2.0.0b3/solid2/core/scad_import.py` & `solidpython2-2.0.0b4/solid2/core/scad_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,26 +84,26 @@
 # use() & include() mimic OpenSCAD's use/include mechanics.
 # -- use() makes methods in scad_file_path.scad available to be called.
 # -- include() makes those methods available AND executes all code in
 #    scad_file_path.scad, which may have side effects.
 #    Unless you have a specific need, call use().
 def get_callers_namespace_dict(depth=2):
     frame = inspect.currentframe()
-    for i in range(depth):
+    for _ in range(depth):
+        assert(frame)
         frame = frame.f_back
 
+    assert(frame)
     if frame.f_code.co_name == "<module>":
         return frame.f_locals
     else:
         raise Exception("use & include can not be used inside a function!\n" +\
               "they would polute the modules namespace and only if executed. This\n" +\
               "has strange side effects! Use them on module level.\n")
 
-        return frame.f_globals
-
 def use(filename, skip_render=False):
     load_scad_file_or_dir_into_dict(filename, get_callers_namespace_dict(), True, skip_render)
 
 def include(filename, skip_render=False):
     load_scad_file_or_dir_into_dict(filename, get_callers_namespace_dict(), False, skip_render)
 
 def import_scad(filename, dest_namespace=None, use_not_include=True, skip_render=False):
```

### Comparing `solidpython2-2.0.0b3/solid2/core/scad_render.py` & `solidpython2-2.0.0b4/solid2/core/scad_render.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/core/utils.py` & `solidpython2-2.0.0b4/solid2/core/utils.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/01-basics.py` & `solidpython2-2.0.0b4/solid2/examples/01-basics.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/02-vars-and-operators.py` & `solidpython2-2.0.0b4/solid2/examples/02-vars-and-operators.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/03-debug-background.py` & `solidpython2-2.0.0b4/solid2/examples/03-debug-background.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/04-convenience.py` & `solidpython2-2.0.0b4/solid2/examples/04-convenience.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/05-access-style-syntax.py` & `solidpython2-2.0.0b4/solid2/examples/05-access-style-syntax.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/06-functions.py` & `solidpython2-2.0.0b4/solid2/examples/06-functions.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/07-libs-bosl2-attachable.py` & `solidpython2-2.0.0b4/solid2/examples/07-libs-bosl2-attachable.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/07-libs-bosl2.py` & `solidpython2-2.0.0b4/solid2/examples/07-libs-bosl2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #! /usr/bin/env python
 
 from solid2.extensions.bosl2 import *
+from solid2.extensions.bosl2 import metric_screws
 
 #basic stuff
 def bolt():
     return metric_screws.metric_bolt(size=20, headtype='hex', l=40)
 
-def bounding_box_wrapper(obj):
-    return ~bounding_box()(obj)
-
 def extrude_along_path():
     path = [ [0, 0, 0], [33, 33, 33], [66, 33, 40], [100, 0, 0], [150,0,0] ]
-    return path_extrude(path)(circle(r=10, _fn=6))
+    return circle(r=10, _fn=6).path_extrude(path)
 
 def heightfield_test():
     def get_data():
         from math import sqrt,sin
         data = []
         for y in range(50):
             yrow = []
@@ -47,22 +45,20 @@
     #openscad example from bosl2 wiki:
     #diff()
     #    cuboid(50) {
     #        tag("remove") attach(TOP) sphere(d=40);
     #        tag("keep") attach(CTR) cylinder(h=40, d=10);
     #    }
     return \
-    diff() (
         cuboid(50) (
             sphere(d=40).attach(TOP).tag("remove"),
             cylinder(h=40, d=10).attach(CTR).tag("keep")
-        )
-    )
+        ).diff()
 
-assembly = bounding_box_wrapper(extrude_along_path()) +\
-           extrude_along_path().color("purple") +\
+assembly = ~extrude_along_path().bounding_box() +\
+           extrude_along_path().recolor("purple") +\
            bosl_diff2().back(100) +\
            bolt().left(100) +\
            heightfield_test().fwd(100)
 
 assembly.save_as_scad()
```

### Comparing `solidpython2-2.0.0b3/solid2/examples/07-libs.py` & `solidpython2-2.0.0b4/solid2/examples/07-libs.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/08-extensions.py` & `solidpython2-2.0.0b4/solid2/examples/08-extensions.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 # some usage of it.
 
 # create a custom OpenSCADObject that maps to color(c="red")
 class red(OpenSCADObject):
     def __init__(self):
         super().__init__(name="color", params={"c" : "red"})
 
-# monkey patch it onto ObjectBase to allow "access-style" syntax
-ObjectBase.red = lambda self: red()(self)
-
 # a non sense object that's not an OpenSCADObject. You can use this to get
 # "low-level" access if you don't want the typical OpenSCAD
 # call(params)(children) syntax. For example the debug,background,.... modifiers
 # are implemented like this (see core/builtins.py)
 class non_sense_comment(ObjectBase):
     def _render(self):
         return "//non sense comment\n" + super()._render()
@@ -32,15 +29,15 @@
 def non_sense_pre_render(root):
 
     def count_nense_recursive(node):
         count = 0
         if isinstance(node, non_sense_comment):
             count += 1
 
-        for c in node.children:
+        for c in node._children:
             count += count_nense_recursive(c)
 
         return count
 
     count = count_nense_recursive(root)
     return f"//the root tree contains {count} non sense comment(s)\n"
 
@@ -60,33 +57,26 @@
 red_commented_cube1 = red()(
                           commented_cube1
                       )
 
 commented_cube2 = non_sense_comment()(
                         cube2
                     )
-# access-style syntax:
-red_commented_cube2 = commented_cube2.\
-                          red()
 
-scene = red_commented_cube1 + red_commented_cube2
+scene = red_commented_cube1 + commented_cube2
 scene.save_as_scad()
 
 # This generates the following output:
 #
-#     // Generated by ExpSolidPython
 #
 #     //the root tree contains 2 non sense comment(s)
 #
 #     union() {
-#             color(c = "red") {
-#                     //non sense comment
-#                     cube(size = 10);
-#             };
-#             color(c = "red") {
-#                     //non sense comment
-#                     translate(v = [-20, 0, 0]) {
-#                             cube(size = 5);
-#                     };
-#             };
-#     };
-
+#         color(c = "red") {
+#             //non sense comment
+#             cube(size = 10);
+#         }
+#         //non sense comment
+#         translate(v = [-20, 0, 0]) {
+#             cube(size = 5);
+#         }
+#     }
```

### Comparing `solidpython2-2.0.0b3/solid2/examples/09-code-attach-extension.py` & `solidpython2-2.0.0b4/solid2/examples/09-code-attach-extension.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/10-customizer.py` & `solidpython2-2.0.0b4/solid2/examples/10-customizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,11 +19,11 @@
                     }
                     """)
 
 scene += translate(cube_pos) (
             cube(cube_size * 2))
 
 scene += translate([0, -20, 0]) (
-            text(customizedText))
+            text(str(customizedText)))
 
 scad_render_to_file(scene)
```

### Comparing `solidpython2-2.0.0b3/solid2/examples/11-font/RichEatin.otf` & `solidpython2-2.0.0b4/solid2/examples/11-font/RichEatin.otf`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/13-animated-bouncing-ball.py` & `solidpython2-2.0.0b4/solid2/examples/13-animated-bouncing-ball.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from solid2 import *
 
 #set steps in OpenSCAD to 1000
 
 ball_radius = 100
 
 class Vector3:
-    def __init__(self, x=0, y=0, z=0):
+    def __init__(self, x=0.0, y=0.0, z=0.0):
         self.x = x
         self.y = y
         self.z = z
 
     def __add__(self, other):
         return Vector3(self.x + other.x,
                        self.y + other.y,
@@ -25,15 +25,15 @@
     def tolist(self):
         return [self.x, self.y, self.z]
 
 #this is our little physics engine
 def get_bouncing_ball_data(pos=Vector3(), vel=Vector3(5.0, 5.0, 200.0)):
     data = []
     gravity = Vector3(0.0, 0.0, -8.0)
-    for t in range(1000):
+    for _ in range(1000):
         vel = (vel + gravity) * 0.995
         pos += vel
         if pos.z < ball_radius:
             vel.z = vel.z * -1
             pos.z = ball_radius
 
         data.append(pos.tolist())
```

### Comparing `solidpython2-2.0.0b3/solid2/examples/14-implicitCAD.py` & `solidpython2-2.0.0b4/solid2/examples/14-implicitCAD.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/15-implicitCAD2.py` & `solidpython2-2.0.0b4/solid2/examples/15-implicitCAD2.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/16-mazebox-bosl2.py` & `solidpython2-2.0.0b4/solid2/examples/16-mazebox-bosl2.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/17-greedy-scad-interface.py` & `solidpython2-2.0.0b4/solid2/examples/17-greedy-scad-interface.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/examples/maze7.png` & `solidpython2-2.0.0b4/solid2/examples/maze7.png`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/affine.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/affine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/affine.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class affine2d_identity(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/affine.scad'}", use_not_include=False)
+
+class affine2d_identity(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("affine2d_identity", {**kwargs})
 
-class affine2d_translate(OpenSCADObject):
+class affine2d_translate(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("affine2d_translate", {"v" : v, **kwargs})
 
-class affine2d_scale(OpenSCADObject):
+class affine2d_scale(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("affine2d_scale", {"v" : v, **kwargs})
 
-class affine2d_zrot(OpenSCADObject):
+class affine2d_zrot(_Bosl2Base):
     def __init__(self, ang=None, **kwargs):
        super().__init__("affine2d_zrot", {"ang" : ang, **kwargs})
 
-class affine2d_mirror(OpenSCADObject):
+class affine2d_mirror(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("affine2d_mirror", {"v" : v, **kwargs})
 
-class affine2d_skew(OpenSCADObject):
+class affine2d_skew(_Bosl2Base):
     def __init__(self, xa=None, ya=None, **kwargs):
        super().__init__("affine2d_skew", {"xa" : xa, "ya" : ya, **kwargs})
 
-class affine3d_identity(OpenSCADObject):
+class affine3d_identity(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("affine3d_identity", {**kwargs})
 
-class affine3d_translate(OpenSCADObject):
+class affine3d_translate(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("affine3d_translate", {"v" : v, **kwargs})
 
-class affine3d_scale(OpenSCADObject):
+class affine3d_scale(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("affine3d_scale", {"v" : v, **kwargs})
 
-class affine3d_xrot(OpenSCADObject):
+class affine3d_xrot(_Bosl2Base):
     def __init__(self, ang=None, **kwargs):
        super().__init__("affine3d_xrot", {"ang" : ang, **kwargs})
 
-class affine3d_yrot(OpenSCADObject):
+class affine3d_yrot(_Bosl2Base):
     def __init__(self, ang=None, **kwargs):
        super().__init__("affine3d_yrot", {"ang" : ang, **kwargs})
 
-class affine3d_zrot(OpenSCADObject):
+class affine3d_zrot(_Bosl2Base):
     def __init__(self, ang=None, **kwargs):
        super().__init__("affine3d_zrot", {"ang" : ang, **kwargs})
 
-class affine3d_rot_by_axis(OpenSCADObject):
+class affine3d_rot_by_axis(_Bosl2Base):
     def __init__(self, u=None, ang=None, **kwargs):
        super().__init__("affine3d_rot_by_axis", {"u" : u, "ang" : ang, **kwargs})
 
-class affine3d_rot_from_to(OpenSCADObject):
+class affine3d_rot_from_to(_Bosl2Base):
     def __init__(self, _from=None, to=None, **kwargs):
        super().__init__("affine3d_rot_from_to", {"_from" : _from, "to" : to, **kwargs})
 
-class affine3d_mirror(OpenSCADObject):
+class affine3d_mirror(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("affine3d_mirror", {"v" : v, **kwargs})
 
-class affine3d_skew(OpenSCADObject):
+class affine3d_skew(_Bosl2Base):
     def __init__(self, sxy=None, sxz=None, syx=None, syz=None, szx=None, szy=None, **kwargs):
        super().__init__("affine3d_skew", {"sxy" : sxy, "sxz" : sxz, "syx" : syx, "syz" : syz, "szx" : szx, "szy" : szy, **kwargs})
 
-class affine3d_skew_xy(OpenSCADObject):
+class affine3d_skew_xy(_Bosl2Base):
     def __init__(self, xa=None, ya=None, **kwargs):
        super().__init__("affine3d_skew_xy", {"xa" : xa, "ya" : ya, **kwargs})
 
-class affine3d_skew_xz(OpenSCADObject):
+class affine3d_skew_xz(_Bosl2Base):
     def __init__(self, xa=None, za=None, **kwargs):
        super().__init__("affine3d_skew_xz", {"xa" : xa, "za" : za, **kwargs})
 
-class affine3d_skew_yz(OpenSCADObject):
+class affine3d_skew_yz(_Bosl2Base):
     def __init__(self, ya=None, za=None, **kwargs):
        super().__init__("affine3d_skew_yz", {"ya" : ya, "za" : za, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/attachments.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/attachments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,249 +1,251 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/attachments.scad'}", use_not_include=False)
-
-_tags = OpenSCADConstant('_tags')
-_tag = OpenSCADConstant('_tag')
-_tag_prefix = OpenSCADConstant('_tag_prefix')
-_overlap = OpenSCADConstant('_overlap')
-_color = OpenSCADConstant('_color')
-_save_color = OpenSCADConstant('_save_color')
-_attach_to = OpenSCADConstant('_attach_to')
-_attach_anchor = OpenSCADConstant('_attach_anchor')
-_attach_norot = OpenSCADConstant('_attach_norot')
-_parent_anchor = OpenSCADConstant('_parent_anchor')
-_parent_spin = OpenSCADConstant('_parent_spin')
-_parent_orient = OpenSCADConstant('_parent_orient')
-_parent_size = OpenSCADConstant('_parent_size')
-_parent_geom = OpenSCADConstant('_parent_geom')
-_tags_shown = OpenSCADConstant('_tags_shown')
-_tags_hidden = OpenSCADConstant('_tags_hidden')
-_ANCHOR_TYPES = OpenSCADConstant('_ANCHOR_TYPES')
-EDGES_NONE = OpenSCADConstant('EDGES_NONE')
-EDGES_ALL = OpenSCADConstant('EDGES_ALL')
-EDGE_OFFSETS = OpenSCADConstant('EDGE_OFFSETS')
-CORNERS_NONE = OpenSCADConstant('CORNERS_NONE')
-CORNERS_ALL = OpenSCADConstant('CORNERS_ALL')
-CORNER_OFFSETS = OpenSCADConstant('CORNER_OFFSETS')
-class position(OpenSCADObject):
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
+
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/attachments.scad'}", use_not_include=False)
+
+_tags = _OpenSCADConstant('_tags')
+_tag = _OpenSCADConstant('_tag')
+_tag_prefix = _OpenSCADConstant('_tag_prefix')
+_overlap = _OpenSCADConstant('_overlap')
+_color = _OpenSCADConstant('_color')
+_save_color = _OpenSCADConstant('_save_color')
+_attach_to = _OpenSCADConstant('_attach_to')
+_attach_anchor = _OpenSCADConstant('_attach_anchor')
+_attach_norot = _OpenSCADConstant('_attach_norot')
+_parent_anchor = _OpenSCADConstant('_parent_anchor')
+_parent_spin = _OpenSCADConstant('_parent_spin')
+_parent_orient = _OpenSCADConstant('_parent_orient')
+_parent_size = _OpenSCADConstant('_parent_size')
+_parent_geom = _OpenSCADConstant('_parent_geom')
+_tags_shown = _OpenSCADConstant('_tags_shown')
+_tags_hidden = _OpenSCADConstant('_tags_hidden')
+_ANCHOR_TYPES = _OpenSCADConstant('_ANCHOR_TYPES')
+EDGES_NONE = _OpenSCADConstant('EDGES_NONE')
+EDGES_ALL = _OpenSCADConstant('EDGES_ALL')
+EDGE_OFFSETS = _OpenSCADConstant('EDGE_OFFSETS')
+CORNERS_NONE = _OpenSCADConstant('CORNERS_NONE')
+CORNERS_ALL = _OpenSCADConstant('CORNERS_ALL')
+CORNER_OFFSETS = _OpenSCADConstant('CORNER_OFFSETS')
+class reorient(_Bosl2Base):
+    def __init__(self, anchor=None, spin=None, orient=None, size=None, size2=None, shift=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, l=None, h=None, vnf=None, path=None, region=None, extent=None, offset=None, cp=None, anchors=None, two_d=None, axis=None, geom=None, p=None, **kwargs):
+       super().__init__("reorient", {"anchor" : anchor, "spin" : spin, "orient" : orient, "size" : size, "size2" : size2, "shift" : shift, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "l" : l, "h" : h, "vnf" : vnf, "path" : path, "region" : region, "extent" : extent, "offset" : offset, "cp" : cp, "anchors" : anchors, "two_d" : two_d, "axis" : axis, "geom" : geom, "p" : p, **kwargs})
+
+class named_anchor(_Bosl2Base):
+    def __init__(self, name=None, pos=None, orient=None, spin=None, **kwargs):
+       super().__init__("named_anchor", {"name" : name, "pos" : pos, "orient" : orient, "spin" : spin, **kwargs})
+
+class attach_geom(_Bosl2Base):
+    def __init__(self, size=None, size2=None, shift=None, scale=None, twist=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, l=None, h=None, vnf=None, region=None, extent=None, cp=None, offset=None, anchors=None, two_d=None, axis=None, **kwargs):
+       super().__init__("attach_geom", {"size" : size, "size2" : size2, "shift" : shift, "scale" : scale, "twist" : twist, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "l" : l, "h" : h, "vnf" : vnf, "region" : region, "extent" : extent, "cp" : cp, "offset" : offset, "anchors" : anchors, "two_d" : two_d, "axis" : axis, **kwargs})
+
+class _attach_geom_2d(_Bosl2Base):
+    def __init__(self, geom=None, **kwargs):
+       super().__init__("_attach_geom_2d", {"geom" : geom, **kwargs})
+
+class _attach_geom_size(_Bosl2Base):
+    def __init__(self, geom=None, **kwargs):
+       super().__init__("_attach_geom_size", {"geom" : geom, **kwargs})
+
+class _attach_transform(_Bosl2Base):
+    def __init__(self, anchor=None, spin=None, orient=None, geom=None, p=None, **kwargs):
+       super().__init__("_attach_transform", {"anchor" : anchor, "spin" : spin, "orient" : orient, "geom" : geom, "p" : p, **kwargs})
+
+class _get_cp(_Bosl2Base):
+    def __init__(self, geom=None, **kwargs):
+       super().__init__("_get_cp", {"geom" : geom, **kwargs})
+
+class _force_anchor_2d(_Bosl2Base):
+    def __init__(self, anchor=None, **kwargs):
+       super().__init__("_force_anchor_2d", {"anchor" : anchor, **kwargs})
+
+class _find_anchor(_Bosl2Base):
+    def __init__(self, anchor=None, geom=None, **kwargs):
+       super().__init__("_find_anchor", {"anchor" : anchor, "geom" : geom, **kwargs})
+
+class _is_shown(_Bosl2Base):
+    def __init__(self, **kwargs):
+       super().__init__("_is_shown", {**kwargs})
+
+class _standard_anchors(_Bosl2Base):
+    def __init__(self, two_d=None, **kwargs):
+       super().__init__("_standard_anchors", {"two_d" : two_d, **kwargs})
+
+class _edges_vec_txt(_Bosl2Base):
+    def __init__(self, x=None, **kwargs):
+       super().__init__("_edges_vec_txt", {"x" : x, **kwargs})
+
+class _edges_text(_Bosl2Base):
+    def __init__(self, edges=None, **kwargs):
+       super().__init__("_edges_text", {"edges" : edges, **kwargs})
+
+class _is_edge_array(_Bosl2Base):
+    def __init__(self, x=None, **kwargs):
+       super().__init__("_is_edge_array", {"x" : x, **kwargs})
+
+class _edge_set(_Bosl2Base):
+    def __init__(self, v=None, **kwargs):
+       super().__init__("_edge_set", {"v" : v, **kwargs})
+
+class _normalize_edges(_Bosl2Base):
+    def __init__(self, v=None, **kwargs):
+       super().__init__("_normalize_edges", {"v" : v, **kwargs})
+
+class _edges(_Bosl2Base):
+    def __init__(self, v=None, _except=None, **kwargs):
+       super().__init__("_edges", {"v" : v, "_except" : _except, **kwargs})
+
+class _is_corner_array(_Bosl2Base):
+    def __init__(self, x=None, **kwargs):
+       super().__init__("_is_corner_array", {"x" : x, **kwargs})
+
+class _normalize_corners(_Bosl2Base):
+    def __init__(self, v=None, **kwargs):
+       super().__init__("_normalize_corners", {"v" : v, **kwargs})
+
+class _corner_set(_Bosl2Base):
+    def __init__(self, v=None, **kwargs):
+       super().__init__("_corner_set", {"v" : v, **kwargs})
+
+class _corners(_Bosl2Base):
+    def __init__(self, v=None, _except=None, **kwargs):
+       super().__init__("_corners", {"v" : v, "_except" : _except, **kwargs})
+
+class _corner_edges(_Bosl2Base):
+    def __init__(self, edges=None, v=None, **kwargs):
+       super().__init__("_corner_edges", {"edges" : edges, "v" : v, **kwargs})
+
+class _corner_edge_count(_Bosl2Base):
+    def __init__(self, edges=None, v=None, **kwargs):
+       super().__init__("_corner_edge_count", {"edges" : edges, "v" : v, **kwargs})
+
+class _corners_text(_Bosl2Base):
+    def __init__(self, corners=None, **kwargs):
+       super().__init__("_corners_text", {"corners" : corners, **kwargs})
+
+class position(_Bosl2Base):
     def __init__(self, _from=None, **kwargs):
        super().__init__("position", {"_from" : _from, **kwargs})
 
-class orient(OpenSCADObject):
+class orient(_Bosl2Base):
     def __init__(self, dir=None, anchor=None, spin=None, **kwargs):
        super().__init__("orient", {"dir" : dir, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class attach(OpenSCADObject):
+class attach(_Bosl2Base):
     def __init__(self, _from=None, to=None, overlap=None, norot=None, **kwargs):
        super().__init__("attach", {"_from" : _from, "to" : to, "overlap" : overlap, "norot" : norot, **kwargs})
 
-class tag(OpenSCADObject):
+class tag(_Bosl2Base):
     def __init__(self, tag=None, **kwargs):
        super().__init__("tag", {"tag" : tag, **kwargs})
 
-class force_tag(OpenSCADObject):
+class force_tag(_Bosl2Base):
     def __init__(self, tag=None, **kwargs):
        super().__init__("force_tag", {"tag" : tag, **kwargs})
 
-class tag_scope(OpenSCADObject):
+class tag_scope(_Bosl2Base):
     def __init__(self, scope=None, **kwargs):
        super().__init__("tag_scope", {"scope" : scope, **kwargs})
 
-class diff(OpenSCADObject):
+class diff(_Bosl2Base):
     def __init__(self, remove=None, keep=None, **kwargs):
        super().__init__("diff", {"remove" : remove, "keep" : keep, **kwargs})
 
-class tag_diff(OpenSCADObject):
+class tag_diff(_Bosl2Base):
     def __init__(self, tag=None, remove=None, keep=None, **kwargs):
        super().__init__("tag_diff", {"tag" : tag, "remove" : remove, "keep" : keep, **kwargs})
 
-class intersect(OpenSCADObject):
+class intersect(_Bosl2Base):
     def __init__(self, intersect=None, keep=None, **kwargs):
        super().__init__("intersect", {"intersect" : intersect, "keep" : keep, **kwargs})
 
-class tag_intersect(OpenSCADObject):
+class tag_intersect(_Bosl2Base):
     def __init__(self, tag=None, intersect=None, keep=None, **kwargs):
        super().__init__("tag_intersect", {"tag" : tag, "intersect" : intersect, "keep" : keep, **kwargs})
 
-class conv_hull(OpenSCADObject):
+class conv_hull(_Bosl2Base):
     def __init__(self, keep=None, **kwargs):
        super().__init__("conv_hull", {"keep" : keep, **kwargs})
 
-class tag_conv_hull(OpenSCADObject):
+class tag_conv_hull(_Bosl2Base):
     def __init__(self, tag=None, keep=None, **kwargs):
        super().__init__("tag_conv_hull", {"tag" : tag, "keep" : keep, **kwargs})
 
-class hide(OpenSCADObject):
+class hide(_Bosl2Base):
     def __init__(self, tags=None, **kwargs):
        super().__init__("hide", {"tags" : tags, **kwargs})
 
-class show_only(OpenSCADObject):
+class show_only(_Bosl2Base):
     def __init__(self, tags=None, **kwargs):
        super().__init__("show_only", {"tags" : tags, **kwargs})
 
-class show_all(OpenSCADObject):
+class show_all(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("show_all", {**kwargs})
 
-class show_int(OpenSCADObject):
+class show_int(_Bosl2Base):
     def __init__(self, tags=None, **kwargs):
        super().__init__("show_int", {"tags" : tags, **kwargs})
 
-class edge_mask(OpenSCADObject):
+class edge_mask(_Bosl2Base):
     def __init__(self, edges=None, _except=None, **kwargs):
        super().__init__("edge_mask", {"edges" : edges, "_except" : _except, **kwargs})
 
-class corner_mask(OpenSCADObject):
+class corner_mask(_Bosl2Base):
     def __init__(self, corners=None, _except=None, **kwargs):
        super().__init__("corner_mask", {"corners" : corners, "_except" : _except, **kwargs})
 
-class face_profile(OpenSCADObject):
+class face_profile(_Bosl2Base):
     def __init__(self, faces=None, r=None, d=None, convexity=None, **kwargs):
        super().__init__("face_profile", {"faces" : faces, "r" : r, "d" : d, "convexity" : convexity, **kwargs})
 
-class edge_profile(OpenSCADObject):
+class edge_profile(_Bosl2Base):
     def __init__(self, edges=None, _except=None, convexity=None, **kwargs):
        super().__init__("edge_profile", {"edges" : edges, "_except" : _except, "convexity" : convexity, **kwargs})
 
-class corner_profile(OpenSCADObject):
+class corner_profile(_Bosl2Base):
     def __init__(self, corners=None, _except=None, r=None, d=None, convexity=None, **kwargs):
        super().__init__("corner_profile", {"corners" : corners, "_except" : _except, "r" : r, "d" : d, "convexity" : convexity, **kwargs})
 
-class attachable(OpenSCADObject):
+class attachable(_Bosl2Base):
     def __init__(self, anchor=None, spin=None, orient=None, size=None, size2=None, shift=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, l=None, h=None, vnf=None, path=None, region=None, extent=None, cp=None, offset=None, anchors=None, two_d=None, axis=None, geom=None, **kwargs):
        super().__init__("attachable", {"anchor" : anchor, "spin" : spin, "orient" : orient, "size" : size, "size2" : size2, "shift" : shift, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "l" : l, "h" : h, "vnf" : vnf, "path" : path, "region" : region, "extent" : extent, "cp" : cp, "offset" : offset, "anchors" : anchors, "two_d" : two_d, "axis" : axis, "geom" : geom, **kwargs})
 
-class show_anchors(OpenSCADObject):
+class show_anchors(_Bosl2Base):
     def __init__(self, s=None, std=None, custom=None, **kwargs):
        super().__init__("show_anchors", {"s" : s, "std" : std, "custom" : custom, **kwargs})
 
-class anchor_arrow(OpenSCADObject):
+class anchor_arrow(_Bosl2Base):
     def __init__(self, s=None, color=None, flag=None, _tag=None, **kwargs):
        super().__init__("anchor_arrow", {"s" : s, "color" : color, "flag" : flag, "_tag" : _tag, **kwargs})
 
-class anchor_arrow2d(OpenSCADObject):
+class anchor_arrow2d(_Bosl2Base):
     def __init__(self, s=None, color=None, _tag=None, **kwargs):
        super().__init__("anchor_arrow2d", {"s" : s, "color" : color, "_tag" : _tag, **kwargs})
 
-class expose_anchors(OpenSCADObject):
+class expose_anchors(_Bosl2Base):
     def __init__(self, opacity=None, **kwargs):
        super().__init__("expose_anchors", {"opacity" : opacity, **kwargs})
 
-class frame_ref(OpenSCADObject):
+class frame_ref(_Bosl2Base):
     def __init__(self, s=None, opacity=None, **kwargs):
        super().__init__("frame_ref", {"s" : s, "opacity" : opacity, **kwargs})
 
-class _edges_text3d(OpenSCADObject):
+class _edges_text3d(_Bosl2Base):
     def __init__(self, txt=None, size=None, **kwargs):
        super().__init__("_edges_text3d", {"txt" : txt, "size" : size, **kwargs})
 
-class _show_edges(OpenSCADObject):
+class _show_edges(_Bosl2Base):
     def __init__(self, edges=None, size=None, text=None, txtsize=None, toplabel=None, **kwargs):
        super().__init__("_show_edges", {"edges" : edges, "size" : size, "text" : text, "txtsize" : txtsize, "toplabel" : toplabel, **kwargs})
 
-class _show_corners(OpenSCADObject):
+class _show_corners(_Bosl2Base):
     def __init__(self, corners=None, size=None, text=None, txtsize=None, toplabel=None, **kwargs):
        super().__init__("_show_corners", {"corners" : corners, "size" : size, "text" : text, "txtsize" : txtsize, "toplabel" : toplabel, **kwargs})
 
-class _show_cube_faces(OpenSCADObject):
+class _show_cube_faces(_Bosl2Base):
     def __init__(self, faces=None, size=None, toplabel=None, botlabel=None, **kwargs):
        super().__init__("_show_cube_faces", {"faces" : faces, "size" : size, "toplabel" : toplabel, "botlabel" : botlabel, **kwargs})
 
-class reorient(OpenSCADObject):
-    def __init__(self, anchor=None, spin=None, orient=None, size=None, size2=None, shift=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, l=None, h=None, vnf=None, path=None, region=None, extent=None, offset=None, cp=None, anchors=None, two_d=None, axis=None, geom=None, p=None, **kwargs):
-       super().__init__("reorient", {"anchor" : anchor, "spin" : spin, "orient" : orient, "size" : size, "size2" : size2, "shift" : shift, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "l" : l, "h" : h, "vnf" : vnf, "path" : path, "region" : region, "extent" : extent, "offset" : offset, "cp" : cp, "anchors" : anchors, "two_d" : two_d, "axis" : axis, "geom" : geom, "p" : p, **kwargs})
-
-class named_anchor(OpenSCADObject):
-    def __init__(self, name=None, pos=None, orient=None, spin=None, **kwargs):
-       super().__init__("named_anchor", {"name" : name, "pos" : pos, "orient" : orient, "spin" : spin, **kwargs})
-
-class attach_geom(OpenSCADObject):
-    def __init__(self, size=None, size2=None, shift=None, scale=None, twist=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, l=None, h=None, vnf=None, region=None, extent=None, cp=None, offset=None, anchors=None, two_d=None, axis=None, **kwargs):
-       super().__init__("attach_geom", {"size" : size, "size2" : size2, "shift" : shift, "scale" : scale, "twist" : twist, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "l" : l, "h" : h, "vnf" : vnf, "region" : region, "extent" : extent, "cp" : cp, "offset" : offset, "anchors" : anchors, "two_d" : two_d, "axis" : axis, **kwargs})
-
-class _attach_geom_2d(OpenSCADObject):
-    def __init__(self, geom=None, **kwargs):
-       super().__init__("_attach_geom_2d", {"geom" : geom, **kwargs})
-
-class _attach_geom_size(OpenSCADObject):
-    def __init__(self, geom=None, **kwargs):
-       super().__init__("_attach_geom_size", {"geom" : geom, **kwargs})
-
-class _attach_transform(OpenSCADObject):
-    def __init__(self, anchor=None, spin=None, orient=None, geom=None, p=None, **kwargs):
-       super().__init__("_attach_transform", {"anchor" : anchor, "spin" : spin, "orient" : orient, "geom" : geom, "p" : p, **kwargs})
-
-class _get_cp(OpenSCADObject):
-    def __init__(self, geom=None, **kwargs):
-       super().__init__("_get_cp", {"geom" : geom, **kwargs})
-
-class _force_anchor_2d(OpenSCADObject):
-    def __init__(self, anchor=None, **kwargs):
-       super().__init__("_force_anchor_2d", {"anchor" : anchor, **kwargs})
-
-class _find_anchor(OpenSCADObject):
-    def __init__(self, anchor=None, geom=None, **kwargs):
-       super().__init__("_find_anchor", {"anchor" : anchor, "geom" : geom, **kwargs})
-
-class _is_shown(OpenSCADObject):
-    def __init__(self, **kwargs):
-       super().__init__("_is_shown", {**kwargs})
-
-class _standard_anchors(OpenSCADObject):
-    def __init__(self, two_d=None, **kwargs):
-       super().__init__("_standard_anchors", {"two_d" : two_d, **kwargs})
-
-class _edges_vec_txt(OpenSCADObject):
-    def __init__(self, x=None, **kwargs):
-       super().__init__("_edges_vec_txt", {"x" : x, **kwargs})
-
-class _edges_text(OpenSCADObject):
-    def __init__(self, edges=None, **kwargs):
-       super().__init__("_edges_text", {"edges" : edges, **kwargs})
-
-class _is_edge_array(OpenSCADObject):
-    def __init__(self, x=None, **kwargs):
-       super().__init__("_is_edge_array", {"x" : x, **kwargs})
-
-class _edge_set(OpenSCADObject):
-    def __init__(self, v=None, **kwargs):
-       super().__init__("_edge_set", {"v" : v, **kwargs})
-
-class _normalize_edges(OpenSCADObject):
-    def __init__(self, v=None, **kwargs):
-       super().__init__("_normalize_edges", {"v" : v, **kwargs})
-
-class _edges(OpenSCADObject):
-    def __init__(self, v=None, _except=None, **kwargs):
-       super().__init__("_edges", {"v" : v, "_except" : _except, **kwargs})
-
-class _is_corner_array(OpenSCADObject):
-    def __init__(self, x=None, **kwargs):
-       super().__init__("_is_corner_array", {"x" : x, **kwargs})
-
-class _normalize_corners(OpenSCADObject):
-    def __init__(self, v=None, **kwargs):
-       super().__init__("_normalize_corners", {"v" : v, **kwargs})
-
-class _corner_set(OpenSCADObject):
-    def __init__(self, v=None, **kwargs):
-       super().__init__("_corner_set", {"v" : v, **kwargs})
-
-class _corners(OpenSCADObject):
-    def __init__(self, v=None, _except=None, **kwargs):
-       super().__init__("_corners", {"v" : v, "_except" : _except, **kwargs})
-
-class _corner_edges(OpenSCADObject):
-    def __init__(self, edges=None, v=None, **kwargs):
-       super().__init__("_corner_edges", {"edges" : edges, "v" : v, **kwargs})
-
-class _corner_edge_count(OpenSCADObject):
-    def __init__(self, edges=None, v=None, **kwargs):
-       super().__init__("_corner_edge_count", {"edges" : edges, "v" : v, **kwargs})
-
-class _corners_text(OpenSCADObject):
-    def __init__(self, corners=None, **kwargs):
-       super().__init__("_corners_text", {"corners" : corners, **kwargs})
-
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/beziers.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/beziers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,135 +1,137 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/beziers.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_bezier_matrix_table = OpenSCADConstant('_bezier_matrix_table')
-class debug_bezier(OpenSCADObject):
-    def __init__(self, bezpath=None, width=None, N=None, **kwargs):
-       super().__init__("debug_bezier", {"bezpath" : bezpath, "width" : width, "N" : N, **kwargs})
-
-class debug_bezier_patches(OpenSCADObject):
-    def __init__(self, patches=None, size=None, splinesteps=None, showcps=None, showdots=None, showpatch=None, convexity=None, style=None, **kwargs):
-       super().__init__("debug_bezier_patches", {"patches" : patches, "size" : size, "splinesteps" : splinesteps, "showcps" : showcps, "showdots" : showdots, "showpatch" : showpatch, "convexity" : convexity, "style" : style, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/beziers.scad'}", use_not_include=False)
 
-class bezier_points(OpenSCADObject):
+_bezier_matrix_table = _OpenSCADConstant('_bezier_matrix_table')
+class bezier_points(_Bosl2Base):
     def __init__(self, curve=None, u=None, **kwargs):
        super().__init__("bezier_points", {"curve" : curve, "u" : u, **kwargs})
 
-class _signed_pascals_triangle(OpenSCADObject):
+class _signed_pascals_triangle(_Bosl2Base):
     def __init__(self, N=None, tri=None, **kwargs):
        super().__init__("_signed_pascals_triangle", {"N" : N, "tri" : tri, **kwargs})
 
-class _compute_bezier_matrix(OpenSCADObject):
+class _compute_bezier_matrix(_Bosl2Base):
     def __init__(self, N=None, **kwargs):
        super().__init__("_compute_bezier_matrix", {"N" : N, **kwargs})
 
-class _bezier_matrix(OpenSCADObject):
+class _bezier_matrix(_Bosl2Base):
     def __init__(self, N=None, **kwargs):
        super().__init__("_bezier_matrix", {"N" : N, **kwargs})
 
-class bezier_curve(OpenSCADObject):
+class bezier_curve(_Bosl2Base):
     def __init__(self, bezier=None, splinesteps=None, endpoint=None, **kwargs):
        super().__init__("bezier_curve", {"bezier" : bezier, "splinesteps" : splinesteps, "endpoint" : endpoint, **kwargs})
 
-class bezier_derivative(OpenSCADObject):
+class bezier_derivative(_Bosl2Base):
     def __init__(self, bezier=None, u=None, order=None, **kwargs):
        super().__init__("bezier_derivative", {"bezier" : bezier, "u" : u, "order" : order, **kwargs})
 
-class bezier_tangent(OpenSCADObject):
+class bezier_tangent(_Bosl2Base):
     def __init__(self, bezier=None, u=None, **kwargs):
        super().__init__("bezier_tangent", {"bezier" : bezier, "u" : u, **kwargs})
 
-class bezier_curvature(OpenSCADObject):
+class bezier_curvature(_Bosl2Base):
     def __init__(self, bezier=None, u=None, **kwargs):
        super().__init__("bezier_curvature", {"bezier" : bezier, "u" : u, **kwargs})
 
-class bezier_closest_point(OpenSCADObject):
+class bezier_closest_point(_Bosl2Base):
     def __init__(self, bezier=None, pt=None, max_err=None, u=None, end_u=None, **kwargs):
        super().__init__("bezier_closest_point", {"bezier" : bezier, "pt" : pt, "max_err" : max_err, "u" : u, "end_u" : end_u, **kwargs})
 
-class bezier_length(OpenSCADObject):
+class bezier_length(_Bosl2Base):
     def __init__(self, bezier=None, start_u=None, end_u=None, max_deflect=None, **kwargs):
        super().__init__("bezier_length", {"bezier" : bezier, "start_u" : start_u, "end_u" : end_u, "max_deflect" : max_deflect, **kwargs})
 
-class bezier_line_intersection(OpenSCADObject):
+class bezier_line_intersection(_Bosl2Base):
     def __init__(self, bezier=None, line=None, **kwargs):
        super().__init__("bezier_line_intersection", {"bezier" : bezier, "line" : line, **kwargs})
 
-class bezpath_points(OpenSCADObject):
+class bezpath_points(_Bosl2Base):
     def __init__(self, bezpath=None, curveind=None, u=None, N=None, **kwargs):
        super().__init__("bezpath_points", {"bezpath" : bezpath, "curveind" : curveind, "u" : u, "N" : N, **kwargs})
 
-class bezpath_curve(OpenSCADObject):
+class bezpath_curve(_Bosl2Base):
     def __init__(self, bezpath=None, splinesteps=None, N=None, endpoint=None, **kwargs):
        super().__init__("bezpath_curve", {"bezpath" : bezpath, "splinesteps" : splinesteps, "N" : N, "endpoint" : endpoint, **kwargs})
 
-class bezpath_closest_point(OpenSCADObject):
+class bezpath_closest_point(_Bosl2Base):
     def __init__(self, bezpath=None, pt=None, N=None, max_err=None, seg=None, min_seg=None, min_u=None, min_dist=None, **kwargs):
        super().__init__("bezpath_closest_point", {"bezpath" : bezpath, "pt" : pt, "N" : N, "max_err" : max_err, "seg" : seg, "min_seg" : min_seg, "min_u" : min_u, "min_dist" : min_dist, **kwargs})
 
-class bezpath_length(OpenSCADObject):
+class bezpath_length(_Bosl2Base):
     def __init__(self, bezpath=None, N=None, max_deflect=None, **kwargs):
        super().__init__("bezpath_length", {"bezpath" : bezpath, "N" : N, "max_deflect" : max_deflect, **kwargs})
 
-class path_to_bezpath(OpenSCADObject):
+class path_to_bezpath(_Bosl2Base):
     def __init__(self, path=None, closed=None, tangents=None, uniform=None, size=None, relsize=None, **kwargs):
        super().__init__("path_to_bezpath", {"path" : path, "closed" : closed, "tangents" : tangents, "uniform" : uniform, "size" : size, "relsize" : relsize, **kwargs})
 
-class bezpath_close_to_axis(OpenSCADObject):
+class bezpath_close_to_axis(_Bosl2Base):
     def __init__(self, bezpath=None, axis=None, N=None, **kwargs):
        super().__init__("bezpath_close_to_axis", {"bezpath" : bezpath, "axis" : axis, "N" : N, **kwargs})
 
-class bezpath_offset(OpenSCADObject):
+class bezpath_offset(_Bosl2Base):
     def __init__(self, offset=None, bezier=None, N=None, **kwargs):
        super().__init__("bezpath_offset", {"offset" : offset, "bezier" : bezier, "N" : N, **kwargs})
 
-class bez_begin(OpenSCADObject):
+class bez_begin(_Bosl2Base):
     def __init__(self, pt=None, a=None, r=None, p=None, **kwargs):
        super().__init__("bez_begin", {"pt" : pt, "a" : a, "r" : r, "p" : p, **kwargs})
 
-class bez_tang(OpenSCADObject):
+class bez_tang(_Bosl2Base):
     def __init__(self, pt=None, a=None, r1=None, r2=None, p=None, **kwargs):
        super().__init__("bez_tang", {"pt" : pt, "a" : a, "r1" : r1, "r2" : r2, "p" : p, **kwargs})
 
-class bez_joint(OpenSCADObject):
+class bez_joint(_Bosl2Base):
     def __init__(self, pt=None, a1=None, a2=None, r1=None, r2=None, p1=None, p2=None, **kwargs):
        super().__init__("bez_joint", {"pt" : pt, "a1" : a1, "a2" : a2, "r1" : r1, "r2" : r2, "p1" : p1, "p2" : p2, **kwargs})
 
-class bez_end(OpenSCADObject):
+class bez_end(_Bosl2Base):
     def __init__(self, pt=None, a=None, r=None, p=None, **kwargs):
        super().__init__("bez_end", {"pt" : pt, "a" : a, "r" : r, "p" : p, **kwargs})
 
-class is_bezier_patch(OpenSCADObject):
+class is_bezier_patch(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("is_bezier_patch", {"x" : x, **kwargs})
 
-class bezier_patch_flat(OpenSCADObject):
+class bezier_patch_flat(_Bosl2Base):
     def __init__(self, size=None, N=None, spin=None, orient=None, trans=None, **kwargs):
        super().__init__("bezier_patch_flat", {"size" : size, "N" : N, "spin" : spin, "orient" : orient, "trans" : trans, **kwargs})
 
-class bezier_patch_reverse(OpenSCADObject):
+class bezier_patch_reverse(_Bosl2Base):
     def __init__(self, patch=None, **kwargs):
        super().__init__("bezier_patch_reverse", {"patch" : patch, **kwargs})
 
-class bezier_patch_points(OpenSCADObject):
+class bezier_patch_points(_Bosl2Base):
     def __init__(self, patch=None, u=None, v=None, **kwargs):
        super().__init__("bezier_patch_points", {"patch" : patch, "u" : u, "v" : v, **kwargs})
 
-class _bezier_rectangle(OpenSCADObject):
+class _bezier_rectangle(_Bosl2Base):
     def __init__(self, patch=None, splinesteps=None, style=None, **kwargs):
        super().__init__("_bezier_rectangle", {"patch" : patch, "splinesteps" : splinesteps, "style" : style, **kwargs})
 
-class bezier_vnf(OpenSCADObject):
+class bezier_vnf(_Bosl2Base):
     def __init__(self, patches=None, splinesteps=None, style=None, **kwargs):
        super().__init__("bezier_vnf", {"patches" : patches, "splinesteps" : splinesteps, "style" : style, **kwargs})
 
-class bezier_vnf_degenerate_patch(OpenSCADObject):
+class bezier_vnf_degenerate_patch(_Bosl2Base):
     def __init__(self, patch=None, splinesteps=None, reverse=None, return_edges=None, **kwargs):
        super().__init__("bezier_vnf_degenerate_patch", {"patch" : patch, "splinesteps" : splinesteps, "reverse" : reverse, "return_edges" : return_edges, **kwargs})
 
-class bezier_patch_normals(OpenSCADObject):
+class bezier_patch_normals(_Bosl2Base):
     def __init__(self, patch=None, u=None, v=None, **kwargs):
        super().__init__("bezier_patch_normals", {"patch" : patch, "u" : u, "v" : v, **kwargs})
 
+class debug_bezier(_Bosl2Base):
+    def __init__(self, bezpath=None, width=None, N=None, **kwargs):
+       super().__init__("debug_bezier", {"bezpath" : bezpath, "width" : width, "N" : N, **kwargs})
+
+class debug_bezier_patches(_Bosl2Base):
+    def __init__(self, patches=None, size=None, splinesteps=None, showcps=None, showdots=None, showpatch=None, convexity=None, style=None, **kwargs):
+       super().__init__("debug_bezier_patches", {"patches" : patches, "size" : size, "splinesteps" : splinesteps, "showcps" : showcps, "showdots" : showdots, "showpatch" : showpatch, "convexity" : convexity, "style" : style, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/bottlecaps.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/bottlecaps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,97 +1,99 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/bottlecaps.scad'}", use_not_include=False)
-
-_sp_specs = OpenSCADConstant('_sp_specs')
-_sp_twist = OpenSCADConstant('_sp_twist')
-_sp_thread_width = OpenSCADConstant('_sp_thread_width')
-class pco1810_neck(OpenSCADObject):
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
+
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/bottlecaps.scad'}", use_not_include=False)
+
+_sp_specs = _OpenSCADConstant('_sp_specs')
+_sp_twist = _OpenSCADConstant('_sp_twist')
+_sp_thread_width = _OpenSCADConstant('_sp_thread_width')
+class pco1810_neck(_Bosl2Base):
     def __init__(self, wall=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1810_neck", {"wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class pco1810_cap(OpenSCADObject):
+class pco1810_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1810_cap", {"wall" : wall, "texture" : texture, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class pco1881_neck(OpenSCADObject):
+class pco1881_neck(_Bosl2Base):
     def __init__(self, wall=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1881_neck", {"wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class pco1881_cap(OpenSCADObject):
+class pco1881_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1881_cap", {"wall" : wall, "texture" : texture, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class generic_bottle_neck(OpenSCADObject):
-    def __init__(self, wall=None, neck_d=None, id=None, thread_od=None, height=None, support_d=None, pitch=None, round_supp=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("generic_bottle_neck", {"wall" : wall, "neck_d" : neck_d, "id" : id, "thread_od" : thread_od, "height" : height, "support_d" : support_d, "pitch" : pitch, "round_supp" : round_supp, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class generic_bottle_neck(_Bosl2Base):
+    def __init__(self, neck_d=None, id=None, thread_od=None, height=None, support_d=None, pitch=None, round_supp=None, wall=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("generic_bottle_neck", {"neck_d" : neck_d, "id" : id, "thread_od" : thread_od, "height" : height, "support_d" : support_d, "pitch" : pitch, "round_supp" : round_supp, "wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class generic_bottle_cap(OpenSCADObject):
+class generic_bottle_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, height=None, thread_od=None, tolerance=None, neck_od=None, flank_angle=None, pitch=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("generic_bottle_cap", {"wall" : wall, "texture" : texture, "height" : height, "thread_od" : thread_od, "tolerance" : tolerance, "neck_od" : neck_od, "flank_angle" : flank_angle, "pitch" : pitch, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class bottle_adapter_neck_to_cap(OpenSCADObject):
+class bottle_adapter_neck_to_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, cap_wall=None, cap_h=None, cap_thread_od=None, tolerance=None, cap_neck_od=None, cap_neck_id=None, cap_thread_taper=None, cap_thread_pitch=None, neck_d=None, neck_id=None, neck_thread_od=None, neck_h=None, neck_thread_pitch=None, neck_support_od=None, d=None, taper_lead_in=None, **kwargs):
        super().__init__("bottle_adapter_neck_to_cap", {"wall" : wall, "texture" : texture, "cap_wall" : cap_wall, "cap_h" : cap_h, "cap_thread_od" : cap_thread_od, "tolerance" : tolerance, "cap_neck_od" : cap_neck_od, "cap_neck_id" : cap_neck_id, "cap_thread_taper" : cap_thread_taper, "cap_thread_pitch" : cap_thread_pitch, "neck_d" : neck_d, "neck_id" : neck_id, "neck_thread_od" : neck_thread_od, "neck_h" : neck_h, "neck_thread_pitch" : neck_thread_pitch, "neck_support_od" : neck_support_od, "d" : d, "taper_lead_in" : taper_lead_in, **kwargs})
 
-class bottle_adapter_cap_to_cap(OpenSCADObject):
+class bottle_adapter_cap_to_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, cap_h1=None, cap_thread_od1=None, tolerance=None, cap_neck_od1=None, cap_thread_pitch1=None, cap_h2=None, cap_thread_od2=None, cap_neck_od2=None, cap_thread_pitch2=None, d=None, neck_id1=None, neck_id2=None, taper_lead_in=None, **kwargs):
        super().__init__("bottle_adapter_cap_to_cap", {"wall" : wall, "texture" : texture, "cap_h1" : cap_h1, "cap_thread_od1" : cap_thread_od1, "tolerance" : tolerance, "cap_neck_od1" : cap_neck_od1, "cap_thread_pitch1" : cap_thread_pitch1, "cap_h2" : cap_h2, "cap_thread_od2" : cap_thread_od2, "cap_neck_od2" : cap_neck_od2, "cap_thread_pitch2" : cap_thread_pitch2, "d" : d, "neck_id1" : neck_id1, "neck_id2" : neck_id2, "taper_lead_in" : taper_lead_in, **kwargs})
 
-class bottle_adapter_neck_to_neck(OpenSCADObject):
+class bottle_adapter_neck_to_neck(_Bosl2Base):
     def __init__(self, d=None, neck_od1=None, neck_id1=None, thread_od1=None, height1=None, support_od1=None, thread_pitch1=None, neck_od2=None, neck_id2=None, thread_od2=None, height2=None, support_od2=None, pitch2=None, taper_lead_in=None, wall=None, **kwargs):
        super().__init__("bottle_adapter_neck_to_neck", {"d" : d, "neck_od1" : neck_od1, "neck_id1" : neck_id1, "thread_od1" : thread_od1, "height1" : height1, "support_od1" : support_od1, "thread_pitch1" : thread_pitch1, "neck_od2" : neck_od2, "neck_id2" : neck_id2, "thread_od2" : thread_od2, "height2" : height2, "support_od2" : support_od2, "pitch2" : pitch2, "taper_lead_in" : taper_lead_in, "wall" : wall, **kwargs})
 
-class sp_neck(OpenSCADObject):
+class _sp_thread_profile(_Bosl2Base):
+    def __init__(self, tpi=None, a=None, S=None, style=None, **kwargs):
+       super().__init__("_sp_thread_profile", {"tpi" : tpi, "a" : a, "S" : S, "style" : style, **kwargs})
+
+class sp_neck(_Bosl2Base):
     def __init__(self, diam=None, type=None, wall=None, id=None, style=None, bead=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("sp_neck", {"diam" : diam, "type" : type, "wall" : wall, "id" : id, "style" : style, "bead" : bead, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class pco1810_neck(OpenSCADObject):
+class sp_diameter(_Bosl2Base):
+    def __init__(self, diam=None, type=None, **kwargs):
+       super().__init__("sp_diameter", {"diam" : diam, "type" : type, **kwargs})
+
+class pco1810_neck(_Bosl2Base):
     def __init__(self, wall=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1810_neck", {"wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class pco1810_cap(OpenSCADObject):
+class pco1810_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1810_cap", {"wall" : wall, "texture" : texture, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class pco1881_neck(OpenSCADObject):
+class pco1881_neck(_Bosl2Base):
     def __init__(self, wall=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1881_neck", {"wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class pco1881_cap(OpenSCADObject):
+class pco1881_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pco1881_cap", {"wall" : wall, "texture" : texture, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class generic_bottle_neck(OpenSCADObject):
-    def __init__(self, neck_d=None, id=None, thread_od=None, height=None, support_d=None, pitch=None, round_supp=None, wall=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("generic_bottle_neck", {"neck_d" : neck_d, "id" : id, "thread_od" : thread_od, "height" : height, "support_d" : support_d, "pitch" : pitch, "round_supp" : round_supp, "wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class generic_bottle_neck(_Bosl2Base):
+    def __init__(self, wall=None, neck_d=None, id=None, thread_od=None, height=None, support_d=None, pitch=None, round_supp=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("generic_bottle_neck", {"wall" : wall, "neck_d" : neck_d, "id" : id, "thread_od" : thread_od, "height" : height, "support_d" : support_d, "pitch" : pitch, "round_supp" : round_supp, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class generic_bottle_cap(OpenSCADObject):
+class generic_bottle_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, height=None, thread_od=None, tolerance=None, neck_od=None, flank_angle=None, pitch=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("generic_bottle_cap", {"wall" : wall, "texture" : texture, "height" : height, "thread_od" : thread_od, "tolerance" : tolerance, "neck_od" : neck_od, "flank_angle" : flank_angle, "pitch" : pitch, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class bottle_adapter_neck_to_cap(OpenSCADObject):
+class bottle_adapter_neck_to_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, cap_wall=None, cap_h=None, cap_thread_od=None, tolerance=None, cap_neck_od=None, cap_neck_id=None, cap_thread_taper=None, cap_thread_pitch=None, neck_d=None, neck_id=None, neck_thread_od=None, neck_h=None, neck_thread_pitch=None, neck_support_od=None, d=None, taper_lead_in=None, **kwargs):
        super().__init__("bottle_adapter_neck_to_cap", {"wall" : wall, "texture" : texture, "cap_wall" : cap_wall, "cap_h" : cap_h, "cap_thread_od" : cap_thread_od, "tolerance" : tolerance, "cap_neck_od" : cap_neck_od, "cap_neck_id" : cap_neck_id, "cap_thread_taper" : cap_thread_taper, "cap_thread_pitch" : cap_thread_pitch, "neck_d" : neck_d, "neck_id" : neck_id, "neck_thread_od" : neck_thread_od, "neck_h" : neck_h, "neck_thread_pitch" : neck_thread_pitch, "neck_support_od" : neck_support_od, "d" : d, "taper_lead_in" : taper_lead_in, **kwargs})
 
-class bottle_adapter_cap_to_cap(OpenSCADObject):
+class bottle_adapter_cap_to_cap(_Bosl2Base):
     def __init__(self, wall=None, texture=None, cap_h1=None, cap_thread_od1=None, tolerance=None, cap_neck_od1=None, cap_thread_pitch1=None, cap_h2=None, cap_thread_od2=None, cap_neck_od2=None, cap_thread_pitch2=None, d=None, neck_id1=None, neck_id2=None, taper_lead_in=None, **kwargs):
        super().__init__("bottle_adapter_cap_to_cap", {"wall" : wall, "texture" : texture, "cap_h1" : cap_h1, "cap_thread_od1" : cap_thread_od1, "tolerance" : tolerance, "cap_neck_od1" : cap_neck_od1, "cap_thread_pitch1" : cap_thread_pitch1, "cap_h2" : cap_h2, "cap_thread_od2" : cap_thread_od2, "cap_neck_od2" : cap_neck_od2, "cap_thread_pitch2" : cap_thread_pitch2, "d" : d, "neck_id1" : neck_id1, "neck_id2" : neck_id2, "taper_lead_in" : taper_lead_in, **kwargs})
 
-class bottle_adapter_neck_to_neck(OpenSCADObject):
+class bottle_adapter_neck_to_neck(_Bosl2Base):
     def __init__(self, d=None, neck_od1=None, neck_id1=None, thread_od1=None, height1=None, support_od1=None, thread_pitch1=None, neck_od2=None, neck_id2=None, thread_od2=None, height2=None, support_od2=None, pitch2=None, taper_lead_in=None, wall=None, **kwargs):
        super().__init__("bottle_adapter_neck_to_neck", {"d" : d, "neck_od1" : neck_od1, "neck_id1" : neck_id1, "thread_od1" : thread_od1, "height1" : height1, "support_od1" : support_od1, "thread_pitch1" : thread_pitch1, "neck_od2" : neck_od2, "neck_id2" : neck_id2, "thread_od2" : thread_od2, "height2" : height2, "support_od2" : support_od2, "pitch2" : pitch2, "taper_lead_in" : taper_lead_in, "wall" : wall, **kwargs})
 
-class _sp_thread_profile(OpenSCADObject):
-    def __init__(self, tpi=None, a=None, S=None, style=None, **kwargs):
-       super().__init__("_sp_thread_profile", {"tpi" : tpi, "a" : a, "S" : S, "style" : style, **kwargs})
-
-class sp_neck(OpenSCADObject):
+class sp_neck(_Bosl2Base):
     def __init__(self, diam=None, type=None, wall=None, id=None, style=None, bead=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("sp_neck", {"diam" : diam, "type" : type, "wall" : wall, "id" : id, "style" : style, "bead" : bead, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class sp_diameter(OpenSCADObject):
-    def __init__(self, diam=None, type=None, **kwargs):
-       super().__init__("sp_diameter", {"diam" : diam, "type" : type, **kwargs})
-
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/color.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/color.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/color.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class recolor(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/color.scad'}", use_not_include=False)
+
+class hsl(_Bosl2Base):
+    def __init__(self, h=None, s=None, l=None, a=None, **kwargs):
+       super().__init__("hsl", {"h" : h, "s" : s, "l" : l, "a" : a, **kwargs})
+
+class hsv(_Bosl2Base):
+    def __init__(self, h=None, s=None, v=None, a=None, **kwargs):
+       super().__init__("hsv", {"h" : h, "s" : s, "v" : v, "a" : a, **kwargs})
+
+class recolor(_Bosl2Base):
     def __init__(self, c=None, **kwargs):
        super().__init__("recolor", {"c" : c, **kwargs})
 
-class color_this(OpenSCADObject):
+class color_this(_Bosl2Base):
     def __init__(self, c=None, **kwargs):
        super().__init__("color_this", {"c" : c, **kwargs})
 
-class rainbow(OpenSCADObject):
+class rainbow(_Bosl2Base):
     def __init__(self, list=None, stride=None, maxhues=None, shuffle=None, seed=None, **kwargs):
        super().__init__("rainbow", {"list" : list, "stride" : stride, "maxhues" : maxhues, "shuffle" : shuffle, "seed" : seed, **kwargs})
 
-class hsl(OpenSCADObject):
-    def __init__(self, h=None, s=None, l=None, a=None, **kwargs):
-       super().__init__("hsl", {"h" : h, "s" : s, "l" : l, "a" : a, **kwargs})
-
-class hsv(OpenSCADObject):
-    def __init__(self, h=None, s=None, v=None, a=None, **kwargs):
-       super().__init__("hsv", {"h" : h, "s" : s, "v" : v, "a" : a, **kwargs})
-
-class hsl(OpenSCADObject):
+class hsl(_Bosl2Base):
     def __init__(self, h=None, s=None, l=None, a=None, **kwargs):
        super().__init__("hsl", {"h" : h, "s" : s, "l" : l, "a" : a, **kwargs})
 
-class hsv(OpenSCADObject):
+class hsv(_Bosl2Base):
     def __init__(self, h=None, s=None, v=None, a=None, **kwargs):
        super().__init__("hsv", {"h" : h, "s" : s, "v" : v, "a" : a, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/comparisons.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/openscad.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,150 +1,134 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/comparisons.scad'}", use_not_include=False)
-
-class approx(OpenSCADObject):
-    def __init__(self, a=None, b=None, eps=None, **kwargs):
-       super().__init__("approx", {"a" : a, "b" : b, "eps" : eps, **kwargs})
-
-class all_zero(OpenSCADObject):
-    def __init__(self, x=None, eps=None, **kwargs):
-       super().__init__("all_zero", {"x" : x, "eps" : eps, **kwargs})
-
-class all_nonzero(OpenSCADObject):
-    def __init__(self, x=None, eps=None, **kwargs):
-       super().__init__("all_nonzero", {"x" : x, "eps" : eps, **kwargs})
-
-class all_positive(OpenSCADObject):
-    def __init__(self, x=None, eps=None, **kwargs):
-       super().__init__("all_positive", {"x" : x, "eps" : eps, **kwargs})
-
-class all_negative(OpenSCADObject):
-    def __init__(self, x=None, eps=None, **kwargs):
-       super().__init__("all_negative", {"x" : x, "eps" : eps, **kwargs})
-
-class all_nonpositive(OpenSCADObject):
-    def __init__(self, x=None, eps=None, **kwargs):
-       super().__init__("all_nonpositive", {"x" : x, "eps" : eps, **kwargs})
-
-class all_nonnegative(OpenSCADObject):
-    def __init__(self, x=None, eps=None, **kwargs):
-       super().__init__("all_nonnegative", {"x" : x, "eps" : eps, **kwargs})
-
-class all_equal(OpenSCADObject):
-    def __init__(self, vec=None, eps=None, **kwargs):
-       super().__init__("all_equal", {"vec" : vec, "eps" : eps, **kwargs})
-
-class is_increasing(OpenSCADObject):
-    def __init__(self, list=None, strict=None, **kwargs):
-       super().__init__("is_increasing", {"list" : list, "strict" : strict, **kwargs})
-
-class is_decreasing(OpenSCADObject):
-    def __init__(self, list=None, strict=None, **kwargs):
-       super().__init__("is_decreasing", {"list" : list, "strict" : strict, **kwargs})
-
-class _type_num(OpenSCADObject):
-    def __init__(self, x=None, **kwargs):
-       super().__init__("_type_num", {"x" : x, **kwargs})
-
-class compare_vals(OpenSCADObject):
-    def __init__(self, a=None, b=None, **kwargs):
-       super().__init__("compare_vals", {"a" : a, "b" : b, **kwargs})
-
-class compare_lists(OpenSCADObject):
-    def __init__(self, a=None, b=None, **kwargs):
-       super().__init__("compare_lists", {"a" : a, "b" : b, **kwargs})
-
-class min_index(OpenSCADObject):
-    def __init__(self, vals=None, all=None, **kwargs):
-       super().__init__("min_index", {"vals" : vals, "all" : all, **kwargs})
-
-class max_index(OpenSCADObject):
-    def __init__(self, vals=None, all=None, **kwargs):
-       super().__init__("max_index", {"vals" : vals, "all" : all, **kwargs})
-
-class find_approx(OpenSCADObject):
-    def __init__(self, val=None, list=None, start=None, all=None, eps=None, **kwargs):
-       super().__init__("find_approx", {"val" : val, "list" : list, "start" : start, "all" : all, "eps" : eps, **kwargs})
-
-class __find_approx(OpenSCADObject):
-    def __init__(self, val=None, list=None, eps=None, i=None, **kwargs):
-       super().__init__("__find_approx", {"val" : val, "list" : list, "eps" : eps, "i" : i, **kwargs})
-
-class deduplicate(OpenSCADObject):
-    def __init__(self, list=None, closed=None, eps=None, **kwargs):
-       super().__init__("deduplicate", {"list" : list, "closed" : closed, "eps" : eps, **kwargs})
-
-class deduplicate_indexed(OpenSCADObject):
-    def __init__(self, list=None, indices=None, closed=None, eps=None, **kwargs):
-       super().__init__("deduplicate_indexed", {"list" : list, "indices" : indices, "closed" : closed, "eps" : eps, **kwargs})
-
-class unique(OpenSCADObject):
-    def __init__(self, list=None, **kwargs):
-       super().__init__("unique", {"list" : list, **kwargs})
-
-class _unique_sort(OpenSCADObject):
-    def __init__(self, l=None, **kwargs):
-       super().__init__("_unique_sort", {"l" : l, **kwargs})
-
-class unique_count(OpenSCADObject):
-    def __init__(self, list=None, **kwargs):
-       super().__init__("unique_count", {"list" : list, **kwargs})
-
-class _valid_idx(OpenSCADObject):
-    def __init__(self, idx=None, imin=None, imax=None, **kwargs):
-       super().__init__("_valid_idx", {"idx" : idx, "imin" : imin, "imax" : imax, **kwargs})
-
-class _group_sort_by_index(OpenSCADObject):
-    def __init__(self, l=None, idx=None, **kwargs):
-       super().__init__("_group_sort_by_index", {"l" : l, "idx" : idx, **kwargs})
-
-class _group_sort(OpenSCADObject):
-    def __init__(self, l=None, **kwargs):
-       super().__init__("_group_sort", {"l" : l, **kwargs})
-
-class _sort_scalars(OpenSCADObject):
-    def __init__(self, arr=None, **kwargs):
-       super().__init__("_sort_scalars", {"arr" : arr, **kwargs})
-
-class _sort_vectors(OpenSCADObject):
-    def __init__(self, arr=None, _i=None, **kwargs):
-       super().__init__("_sort_vectors", {"arr" : arr, "_i" : _i, **kwargs})
-
-class _sort_vectors(OpenSCADObject):
-    def __init__(self, arr=None, idxlist=None, _i=None, **kwargs):
-       super().__init__("_sort_vectors", {"arr" : arr, "idxlist" : idxlist, "_i" : _i, **kwargs})
-
-class _sort_general(OpenSCADObject):
-    def __init__(self, arr=None, idx=None, indexed=None, **kwargs):
-       super().__init__("_sort_general", {"arr" : arr, "idx" : idx, "indexed" : indexed, **kwargs})
-
-class _lexical_sort(OpenSCADObject):
-    def __init__(self, arr=None, **kwargs):
-       super().__init__("_lexical_sort", {"arr" : arr, **kwargs})
-
-class _indexed_sort(OpenSCADObject):
-    def __init__(self, arrind=None, **kwargs):
-       super().__init__("_indexed_sort", {"arrind" : arrind, **kwargs})
-
-class sort(OpenSCADObject):
-    def __init__(self, list=None, idx=None, **kwargs):
-       super().__init__("sort", {"list" : list, "idx" : idx, **kwargs})
-
-class sortidx(OpenSCADObject):
-    def __init__(self, list=None, idx=None, **kwargs):
-       super().__init__("sortidx", {"list" : list, "idx" : idx, **kwargs})
-
-class group_sort(OpenSCADObject):
-    def __init__(self, list=None, idx=None, **kwargs):
-       super().__init__("group_sort", {"list" : list, "idx" : idx, **kwargs})
-
-class group_data(OpenSCADObject):
-    def __init__(self, groups=None, values=None, **kwargs):
-       super().__init__("group_data", {"groups" : groups, "values" : values, **kwargs})
-
-class list_smallest(OpenSCADObject):
-    def __init__(self, list=None, k=None, **kwargs):
-       super().__init__("list_smallest", {"list" : list, "k" : k, **kwargs})
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+class union(_Bosl2Base):
+    def __init__(self, **kwargs):
+       super().__init__("union", {**kwargs})
+
+class difference(_Bosl2Base):
+    def __init__(self, **kwargs):
+       super().__init__("difference", {**kwargs})
+
+class intersection(_Bosl2Base):
+    def __init__(self, **kwargs):
+       super().__init__("intersection", {**kwargs})
+
+class intersection_for(_Bosl2Base):
+    def __init__(self, n=None, **kwargs):
+       super().__init__("intersection_for", {"n" : n, **kwargs})
+
+class translate(_Bosl2Base):
+    def __init__(self, v=None, **kwargs):
+       super().__init__("translate", {"v" : v, **kwargs})
+
+class scale(_Bosl2Base):
+    def __init__(self, v=None, **kwargs):
+       super().__init__("scale", {"v" : v, **kwargs})
+
+class rotate(_Bosl2Base):
+    def __init__(self, a=None, v=None, **kwargs):
+       super().__init__("rotate", {"a" : a, "v" : v, **kwargs})
+
+class mirror(_Bosl2Base):
+    def __init__(self, v=None, **kwargs):
+       super().__init__("mirror", {"v" : v, **kwargs})
+
+class resize(_Bosl2Base):
+    def __init__(self, newsize=None, auto=None, **kwargs):
+       super().__init__("resize", {"newsize" : newsize, "auto" : auto, **kwargs})
+
+class color(_Bosl2Base):
+    def __init__(self, c=None, alpha=None, **kwargs):
+       super().__init__("color", {"c" : c, "alpha" : alpha, **kwargs})
+
+class minkowski(_Bosl2Base):
+    def __init__(self, **kwargs):
+       super().__init__("minkowski", {**kwargs})
+
+class offset(_Bosl2Base):
+    def __init__(self, r=None, delta=None, chamfer=None, _fn=None, **kwargs):
+       super().__init__("offset", {"r" : r, "delta" : delta, "chamfer" : chamfer, "_fn" : _fn, **kwargs})
+
+class hull(_Bosl2Base):
+    def __init__(self, **kwargs):
+       super().__init__("hull", {**kwargs})
+
+class render(_Bosl2Base):
+    def __init__(self, convexity=None, **kwargs):
+       super().__init__("render", {"convexity" : convexity, **kwargs})
+
+class linear_extrude(_Bosl2Base):
+    def __init__(self, height=None, center=None, convexity=None, twist=None, slices=None, scale=None, **kwargs):
+       super().__init__("linear_extrude", {"height" : height, "center" : center, "convexity" : convexity, "twist" : twist, "slices" : slices, "scale" : scale, **kwargs})
+
+class rotate_extrude(_Bosl2Base):
+    def __init__(self, angle=None, convexity=None, _fn=None, **kwargs):
+       super().__init__("rotate_extrude", {"angle" : angle, "convexity" : convexity, "_fn" : _fn, **kwargs})
+
+class projection(_Bosl2Base):
+    def __init__(self, cut=None, **kwargs):
+       super().__init__("projection", {"cut" : cut, **kwargs})
+
+class surface(_Bosl2Base):
+    def __init__(self, file=None, center=None, convexity=None, invert=None, **kwargs):
+       super().__init__("surface", {"file" : file, "center" : center, "convexity" : convexity, "invert" : invert, **kwargs})
+
+class child(_Bosl2Base):
+    def __init__(self, index=None, vector=None, range=None, **kwargs):
+       super().__init__("child", {"index" : index, "vector" : vector, "range" : range, **kwargs})
+
+class children(_Bosl2Base):
+    def __init__(self, index=None, vector=None, range=None, **kwargs):
+       super().__init__("children", {"index" : index, "vector" : vector, "range" : range, **kwargs})
+
+class import_stl(_Bosl2Base):
+    def __init__(self, file=None, origin=None, convexity=None, layer=None, **kwargs):
+       super().__init__("import_stl", {"file" : file, "origin" : origin, "convexity" : convexity, "layer" : layer, **kwargs})
+
+class import_dxf(_Bosl2Base):
+    def __init__(self, file=None, origin=None, convexity=None, layer=None, **kwargs):
+       super().__init__("import_dxf", {"file" : file, "origin" : origin, "convexity" : convexity, "layer" : layer, **kwargs})
+
+class _import(_Bosl2Base):
+    def __init__(self, file=None, origin=None, convexity=None, layer=None, **kwargs):
+       super().__init__("_import", {"file" : file, "origin" : origin, "convexity" : convexity, "layer" : layer, **kwargs})
+
+class assign(_Bosl2Base):
+    def __init__(self, **kwargs):
+       super().__init__("assign", {**kwargs})
+
+class multmatrix(_Bosl2Base):
+    def __init__(self, m=None, **kwargs):
+       super().__init__("multmatrix", {"m" : m, **kwargs})
+
+class polygon(_Bosl2Base):
+    def __init__(self, points=None, paths=None, convexity=None, **kwargs):
+       super().__init__("polygon", {"points" : points, "paths" : paths, "convexity" : convexity, **kwargs})
+
+class circle(_Bosl2Base):
+    def __init__(self, r=None, d=None, _fn=None, **kwargs):
+       super().__init__("circle", {"r" : r, "d" : d, "_fn" : _fn, **kwargs})
+
+class square(_Bosl2Base):
+    def __init__(self, size=None, center=None, **kwargs):
+       super().__init__("square", {"size" : size, "center" : center, **kwargs})
+
+class sphere(_Bosl2Base):
+    def __init__(self, r=None, d=None, _fn=None, **kwargs):
+       super().__init__("sphere", {"r" : r, "d" : d, "_fn" : _fn, **kwargs})
+
+class cube(_Bosl2Base):
+    def __init__(self, size=None, center=None, **kwargs):
+       super().__init__("cube", {"size" : size, "center" : center, **kwargs})
+
+class cylinder(_Bosl2Base):
+    def __init__(self, r=None, h=None, r1=None, r2=None, d=None, d1=None, d2=None, center=None, _fn=None, **kwargs):
+       super().__init__("cylinder", {"r" : r, "h" : h, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "center" : center, "_fn" : _fn, **kwargs})
+
+class polyhedron(_Bosl2Base):
+    def __init__(self, points=None, faces=None, convexity=None, triangles=None, **kwargs):
+       super().__init__("polyhedron", {"points" : points, "faces" : faces, "convexity" : convexity, "triangles" : triangles, **kwargs})
+
+class text(_Bosl2Base):
+    def __init__(self, text=None, size=None, font=None, halign=None, valign=None, spacing=None, direction=None, language=None, script=None, _fn=None, **kwargs):
+       super().__init__("text", {"text" : text, "size" : size, "font" : font, "halign" : halign, "valign" : valign, "spacing" : spacing, "direction" : direction, "language" : language, "script" : script, "_fn" : _fn, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/coords.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/coords.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,72 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/coords.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class point2d(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/coords.scad'}", use_not_include=False)
+
+class point2d(_Bosl2Base):
     def __init__(self, p=None, fill=None, **kwargs):
        super().__init__("point2d", {"p" : p, "fill" : fill, **kwargs})
 
-class path2d(OpenSCADObject):
+class path2d(_Bosl2Base):
     def __init__(self, points=None, **kwargs):
        super().__init__("path2d", {"points" : points, **kwargs})
 
-class point3d(OpenSCADObject):
+class point3d(_Bosl2Base):
     def __init__(self, p=None, fill=None, **kwargs):
        super().__init__("point3d", {"p" : p, "fill" : fill, **kwargs})
 
-class path3d(OpenSCADObject):
+class path3d(_Bosl2Base):
     def __init__(self, points=None, fill=None, **kwargs):
        super().__init__("path3d", {"points" : points, "fill" : fill, **kwargs})
 
-class point4d(OpenSCADObject):
+class point4d(_Bosl2Base):
     def __init__(self, p=None, fill=None, **kwargs):
        super().__init__("point4d", {"p" : p, "fill" : fill, **kwargs})
 
-class path4d(OpenSCADObject):
+class path4d(_Bosl2Base):
     def __init__(self, points=None, fill=None, **kwargs):
        super().__init__("path4d", {"points" : points, "fill" : fill, **kwargs})
 
-class polar_to_xy(OpenSCADObject):
+class polar_to_xy(_Bosl2Base):
     def __init__(self, r=None, theta=None, **kwargs):
        super().__init__("polar_to_xy", {"r" : r, "theta" : theta, **kwargs})
 
-class xy_to_polar(OpenSCADObject):
+class xy_to_polar(_Bosl2Base):
     def __init__(self, x=None, y=None, **kwargs):
        super().__init__("xy_to_polar", {"x" : x, "y" : y, **kwargs})
 
-class project_plane(OpenSCADObject):
+class project_plane(_Bosl2Base):
     def __init__(self, plane=None, p=None, **kwargs):
        super().__init__("project_plane", {"plane" : plane, "p" : p, **kwargs})
 
-class lift_plane(OpenSCADObject):
+class lift_plane(_Bosl2Base):
     def __init__(self, plane=None, p=None, **kwargs):
        super().__init__("lift_plane", {"plane" : plane, "p" : p, **kwargs})
 
-class cylindrical_to_xyz(OpenSCADObject):
+class cylindrical_to_xyz(_Bosl2Base):
     def __init__(self, r=None, theta=None, z=None, **kwargs):
        super().__init__("cylindrical_to_xyz", {"r" : r, "theta" : theta, "z" : z, **kwargs})
 
-class xyz_to_cylindrical(OpenSCADObject):
+class xyz_to_cylindrical(_Bosl2Base):
     def __init__(self, x=None, y=None, z=None, **kwargs):
        super().__init__("xyz_to_cylindrical", {"x" : x, "y" : y, "z" : z, **kwargs})
 
-class spherical_to_xyz(OpenSCADObject):
+class spherical_to_xyz(_Bosl2Base):
     def __init__(self, r=None, theta=None, phi=None, **kwargs):
        super().__init__("spherical_to_xyz", {"r" : r, "theta" : theta, "phi" : phi, **kwargs})
 
-class xyz_to_spherical(OpenSCADObject):
+class xyz_to_spherical(_Bosl2Base):
     def __init__(self, x=None, y=None, z=None, **kwargs):
        super().__init__("xyz_to_spherical", {"x" : x, "y" : y, "z" : z, **kwargs})
 
-class altaz_to_xyz(OpenSCADObject):
+class altaz_to_xyz(_Bosl2Base):
     def __init__(self, alt=None, az=None, r=None, **kwargs):
        super().__init__("altaz_to_xyz", {"alt" : alt, "az" : az, "r" : r, **kwargs})
 
-class xyz_to_altaz(OpenSCADObject):
+class xyz_to_altaz(_Bosl2Base):
     def __init__(self, x=None, y=None, z=None, **kwargs):
        super().__init__("xyz_to_altaz", {"x" : x, "y" : y, "z" : z, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/cubetruss.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/cubetruss.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/cubetruss.scad'}", use_not_include=False)
-
-_cubetruss_size = OpenSCADConstant('_cubetruss_size')
-_cubetruss_strut_size = OpenSCADConstant('_cubetruss_strut_size')
-_cubetruss_bracing = OpenSCADConstant('_cubetruss_bracing')
-_cubetruss_clip_thickness = OpenSCADConstant('_cubetruss_clip_thickness')
-class cubetruss_segment(OpenSCADObject):
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
+
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/cubetruss.scad'}", use_not_include=False)
+
+_cubetruss_size = _OpenSCADConstant('_cubetruss_size')
+_cubetruss_strut_size = _OpenSCADConstant('_cubetruss_strut_size')
+_cubetruss_bracing = _OpenSCADConstant('_cubetruss_bracing')
+_cubetruss_clip_thickness = _OpenSCADConstant('_cubetruss_clip_thickness')
+class cubetruss_dist(_Bosl2Base):
+    def __init__(self, cubes=None, gaps=None, size=None, strut=None, **kwargs):
+       super().__init__("cubetruss_dist", {"cubes" : cubes, "gaps" : gaps, "size" : size, "strut" : strut, **kwargs})
+
+class cubetruss_segment(_Bosl2Base):
     def __init__(self, size=None, strut=None, bracing=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cubetruss_segment", {"size" : size, "strut" : strut, "bracing" : bracing, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cubetruss_support(OpenSCADObject):
+class cubetruss_support(_Bosl2Base):
     def __init__(self, size=None, strut=None, extents=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cubetruss_support", {"size" : size, "strut" : strut, "extents" : extents, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cubetruss_clip(OpenSCADObject):
+class cubetruss_clip(_Bosl2Base):
     def __init__(self, extents=None, size=None, strut=None, clipthick=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cubetruss_clip", {"extents" : extents, "size" : size, "strut" : strut, "clipthick" : clipthick, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cubetruss_foot(OpenSCADObject):
+class cubetruss_foot(_Bosl2Base):
     def __init__(self, w=None, size=None, strut=None, clipthick=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cubetruss_foot", {"w" : w, "size" : size, "strut" : strut, "clipthick" : clipthick, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cubetruss_joiner(OpenSCADObject):
+class cubetruss_joiner(_Bosl2Base):
     def __init__(self, w=None, vert=None, size=None, strut=None, clipthick=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cubetruss_joiner", {"w" : w, "vert" : vert, "size" : size, "strut" : strut, "clipthick" : clipthick, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cubetruss_uclip(OpenSCADObject):
+class cubetruss_uclip(_Bosl2Base):
     def __init__(self, dual=None, size=None, strut=None, clipthick=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cubetruss_uclip", {"dual" : dual, "size" : size, "strut" : strut, "clipthick" : clipthick, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cubetruss(OpenSCADObject):
+class cubetruss(_Bosl2Base):
     def __init__(self, extents=None, clips=None, bracing=None, size=None, strut=None, clipthick=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cubetruss", {"extents" : extents, "clips" : clips, "bracing" : bracing, "size" : size, "strut" : strut, "clipthick" : clipthick, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cubetruss_corner(OpenSCADObject):
+class cubetruss_corner(_Bosl2Base):
     def __init__(self, h=None, extents=None, bracing=None, size=None, strut=None, clipthick=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cubetruss_corner", {"h" : h, "extents" : extents, "bracing" : bracing, "size" : size, "strut" : strut, "clipthick" : clipthick, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cubetruss_dist(OpenSCADObject):
-    def __init__(self, cubes=None, gaps=None, size=None, strut=None, **kwargs):
-       super().__init__("cubetruss_dist", {"cubes" : cubes, "gaps" : gaps, "size" : size, "strut" : strut, **kwargs})
-
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/distributors.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/distributors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,96 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/distributors.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class move_copies(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/distributors.scad'}", use_not_include=False)
+
+class line_of(_Bosl2Base):
+    def __init__(self, spacing=None, n=None, l=None, p1=None, p2=None, **kwargs):
+       super().__init__("line_of", {"spacing" : spacing, "n" : n, "l" : l, "p1" : p1, "p2" : p2, **kwargs})
+
+class move_copies(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("move_copies", {"a" : a, **kwargs})
 
-class line_of(OpenSCADObject):
+class line_of(_Bosl2Base):
     def __init__(self, spacing=None, n=None, l=None, p1=None, p2=None, **kwargs):
        super().__init__("line_of", {"spacing" : spacing, "n" : n, "l" : l, "p1" : p1, "p2" : p2, **kwargs})
 
-class xcopies(OpenSCADObject):
+class xcopies(_Bosl2Base):
     def __init__(self, spacing=None, n=None, l=None, sp=None, **kwargs):
        super().__init__("xcopies", {"spacing" : spacing, "n" : n, "l" : l, "sp" : sp, **kwargs})
 
-class ycopies(OpenSCADObject):
+class ycopies(_Bosl2Base):
     def __init__(self, spacing=None, n=None, l=None, sp=None, **kwargs):
        super().__init__("ycopies", {"spacing" : spacing, "n" : n, "l" : l, "sp" : sp, **kwargs})
 
-class zcopies(OpenSCADObject):
+class zcopies(_Bosl2Base):
     def __init__(self, spacing=None, n=None, l=None, sp=None, **kwargs):
        super().__init__("zcopies", {"spacing" : spacing, "n" : n, "l" : l, "sp" : sp, **kwargs})
 
-class grid2d(OpenSCADObject):
+class grid2d(_Bosl2Base):
     def __init__(self, spacing=None, n=None, size=None, stagger=None, inside=None, nonzero=None, **kwargs):
        super().__init__("grid2d", {"spacing" : spacing, "n" : n, "size" : size, "stagger" : stagger, "inside" : inside, "nonzero" : nonzero, **kwargs})
 
-class rot_copies(OpenSCADObject):
+class rot_copies(_Bosl2Base):
     def __init__(self, rots=None, v=None, cp=None, n=None, sa=None, offset=None, delta=None, subrot=None, **kwargs):
        super().__init__("rot_copies", {"rots" : rots, "v" : v, "cp" : cp, "n" : n, "sa" : sa, "offset" : offset, "delta" : delta, "subrot" : subrot, **kwargs})
 
-class xrot_copies(OpenSCADObject):
+class xrot_copies(_Bosl2Base):
     def __init__(self, rots=None, cp=None, n=None, sa=None, r=None, d=None, subrot=None, **kwargs):
        super().__init__("xrot_copies", {"rots" : rots, "cp" : cp, "n" : n, "sa" : sa, "r" : r, "d" : d, "subrot" : subrot, **kwargs})
 
-class yrot_copies(OpenSCADObject):
+class yrot_copies(_Bosl2Base):
     def __init__(self, rots=None, cp=None, n=None, sa=None, r=None, d=None, subrot=None, **kwargs):
        super().__init__("yrot_copies", {"rots" : rots, "cp" : cp, "n" : n, "sa" : sa, "r" : r, "d" : d, "subrot" : subrot, **kwargs})
 
-class zrot_copies(OpenSCADObject):
+class zrot_copies(_Bosl2Base):
     def __init__(self, rots=None, cp=None, n=None, sa=None, r=None, d=None, subrot=None, **kwargs):
        super().__init__("zrot_copies", {"rots" : rots, "cp" : cp, "n" : n, "sa" : sa, "r" : r, "d" : d, "subrot" : subrot, **kwargs})
 
-class arc_of(OpenSCADObject):
+class arc_of(_Bosl2Base):
     def __init__(self, n=None, r=None, rx=None, ry=None, d=None, dx=None, dy=None, sa=None, ea=None, rot=None, **kwargs):
        super().__init__("arc_of", {"n" : n, "r" : r, "rx" : rx, "ry" : ry, "d" : d, "dx" : dx, "dy" : dy, "sa" : sa, "ea" : ea, "rot" : rot, **kwargs})
 
-class ovoid_spread(OpenSCADObject):
+class ovoid_spread(_Bosl2Base):
     def __init__(self, n=None, r=None, d=None, cone_ang=None, scale=None, perp=None, **kwargs):
        super().__init__("ovoid_spread", {"n" : n, "r" : r, "d" : d, "cone_ang" : cone_ang, "scale" : scale, "perp" : perp, **kwargs})
 
-class path_spread(OpenSCADObject):
+class path_spread(_Bosl2Base):
     def __init__(self, path=None, n=None, spacing=None, sp=None, rotate_children=None, closed=None, **kwargs):
        super().__init__("path_spread", {"path" : path, "n" : n, "spacing" : spacing, "sp" : sp, "rotate_children" : rotate_children, "closed" : closed, **kwargs})
 
-class mirror_copy(OpenSCADObject):
+class mirror_copy(_Bosl2Base):
     def __init__(self, v=None, offset=None, cp=None, **kwargs):
        super().__init__("mirror_copy", {"v" : v, "offset" : offset, "cp" : cp, **kwargs})
 
-class xflip_copy(OpenSCADObject):
+class xflip_copy(_Bosl2Base):
     def __init__(self, offset=None, x=None, **kwargs):
        super().__init__("xflip_copy", {"offset" : offset, "x" : x, **kwargs})
 
-class yflip_copy(OpenSCADObject):
+class yflip_copy(_Bosl2Base):
     def __init__(self, offset=None, y=None, **kwargs):
        super().__init__("yflip_copy", {"offset" : offset, "y" : y, **kwargs})
 
-class zflip_copy(OpenSCADObject):
+class zflip_copy(_Bosl2Base):
     def __init__(self, offset=None, z=None, **kwargs):
        super().__init__("zflip_copy", {"offset" : offset, "z" : z, **kwargs})
 
-class distribute(OpenSCADObject):
+class distribute(_Bosl2Base):
     def __init__(self, spacing=None, sizes=None, dir=None, l=None, **kwargs):
        super().__init__("distribute", {"spacing" : spacing, "sizes" : sizes, "dir" : dir, "l" : l, **kwargs})
 
-class xdistribute(OpenSCADObject):
+class xdistribute(_Bosl2Base):
     def __init__(self, spacing=None, sizes=None, l=None, **kwargs):
        super().__init__("xdistribute", {"spacing" : spacing, "sizes" : sizes, "l" : l, **kwargs})
 
-class ydistribute(OpenSCADObject):
+class ydistribute(_Bosl2Base):
     def __init__(self, spacing=None, sizes=None, l=None, **kwargs):
        super().__init__("ydistribute", {"spacing" : spacing, "sizes" : sizes, "l" : l, **kwargs})
 
-class zdistribute(OpenSCADObject):
+class zdistribute(_Bosl2Base):
     def __init__(self, spacing=None, sizes=None, l=None, **kwargs):
        super().__init__("zdistribute", {"spacing" : spacing, "sizes" : sizes, "l" : l, **kwargs})
 
-class line_of(OpenSCADObject):
-    def __init__(self, spacing=None, n=None, l=None, p1=None, p2=None, **kwargs):
-       super().__init__("line_of", {"spacing" : spacing, "n" : n, "l" : l, "p1" : p1, "p2" : p2, **kwargs})
-
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/drawing.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/drawing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,72 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/drawing.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class stroke(OpenSCADObject):
-    def __init__(self, path=None, width=None, closed=None, endcaps=None, endcap1=None, endcap2=None, joints=None, dots=None, endcap_width=None, endcap_width1=None, endcap_width2=None, joint_width=None, dots_width=None, endcap_length=None, endcap_length1=None, endcap_length2=None, joint_length=None, dots_length=None, endcap_extent=None, endcap_extent1=None, endcap_extent2=None, joint_extent=None, dots_extent=None, endcap_angle=None, endcap_angle1=None, endcap_angle2=None, joint_angle=None, dots_angle=None, endcap_color=None, endcap_color1=None, endcap_color2=None, joint_color=None, dots_color=None, color=None, trim=None, trim1=None, trim2=None, convexity=None, hull=None, **kwargs):
-       super().__init__("stroke", {"path" : path, "width" : width, "closed" : closed, "endcaps" : endcaps, "endcap1" : endcap1, "endcap2" : endcap2, "joints" : joints, "dots" : dots, "endcap_width" : endcap_width, "endcap_width1" : endcap_width1, "endcap_width2" : endcap_width2, "joint_width" : joint_width, "dots_width" : dots_width, "endcap_length" : endcap_length, "endcap_length1" : endcap_length1, "endcap_length2" : endcap_length2, "joint_length" : joint_length, "dots_length" : dots_length, "endcap_extent" : endcap_extent, "endcap_extent1" : endcap_extent1, "endcap_extent2" : endcap_extent2, "joint_extent" : joint_extent, "dots_extent" : dots_extent, "endcap_angle" : endcap_angle, "endcap_angle1" : endcap_angle1, "endcap_angle2" : endcap_angle2, "joint_angle" : joint_angle, "dots_angle" : dots_angle, "endcap_color" : endcap_color, "endcap_color1" : endcap_color1, "endcap_color2" : endcap_color2, "joint_color" : joint_color, "dots_color" : dots_color, "color" : color, "trim" : trim, "trim1" : trim1, "trim2" : trim2, "convexity" : convexity, "hull" : hull, **kwargs})
-
-class dashed_stroke(OpenSCADObject):
-    def __init__(self, path=None, dashpat=None, width=None, closed=None, **kwargs):
-       super().__init__("dashed_stroke", {"path" : path, "dashpat" : dashpat, "width" : width, "closed" : closed, **kwargs})
-
-class arc(OpenSCADObject):
-    def __init__(self, n=None, r=None, angle=None, d=None, cp=None, points=None, corner=None, width=None, thickness=None, start=None, wedge=None, anchor=None, spin=None, **kwargs):
-       super().__init__("arc", {"n" : n, "r" : r, "angle" : angle, "d" : d, "cp" : cp, "points" : points, "corner" : corner, "width" : width, "thickness" : thickness, "start" : start, "wedge" : wedge, "anchor" : anchor, "spin" : spin, **kwargs})
-
-class helix(OpenSCADObject):
-    def __init__(self, l=None, h=None, turns=None, angle=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, **kwargs):
-       super().__init__("helix", {"l" : l, "h" : h, "turns" : turns, "angle" : angle, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, **kwargs})
-
-class turtle(OpenSCADObject):
-    def __init__(self, commands=None, state=None, full_state=None, repeat=None, **kwargs):
-       super().__init__("turtle", {"commands" : commands, "state" : state, "full_state" : full_state, "repeat" : repeat, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/drawing.scad'}", use_not_include=False)
 
-class debug_polygon(OpenSCADObject):
-    def __init__(self, points=None, paths=None, vertices=None, edges=None, convexity=None, size=None, **kwargs):
-       super().__init__("debug_polygon", {"points" : points, "paths" : paths, "vertices" : vertices, "edges" : edges, "convexity" : convexity, "size" : size, **kwargs})
-
-class stroke(OpenSCADObject):
+class stroke(_Bosl2Base):
     def __init__(self, path=None, width=None, closed=None, endcaps=None, endcap1=None, endcap2=None, joints=None, dots=None, endcap_width=None, endcap_width1=None, endcap_width2=None, joint_width=None, dots_width=None, endcap_length=None, endcap_length1=None, endcap_length2=None, joint_length=None, dots_length=None, endcap_extent=None, endcap_extent1=None, endcap_extent2=None, joint_extent=None, dots_extent=None, endcap_angle=None, endcap_angle1=None, endcap_angle2=None, joint_angle=None, dots_angle=None, endcap_color=None, endcap_color1=None, endcap_color2=None, joint_color=None, dots_color=None, color=None, trim=None, trim1=None, trim2=None, convexity=None, hull=None, **kwargs):
        super().__init__("stroke", {"path" : path, "width" : width, "closed" : closed, "endcaps" : endcaps, "endcap1" : endcap1, "endcap2" : endcap2, "joints" : joints, "dots" : dots, "endcap_width" : endcap_width, "endcap_width1" : endcap_width1, "endcap_width2" : endcap_width2, "joint_width" : joint_width, "dots_width" : dots_width, "endcap_length" : endcap_length, "endcap_length1" : endcap_length1, "endcap_length2" : endcap_length2, "joint_length" : joint_length, "dots_length" : dots_length, "endcap_extent" : endcap_extent, "endcap_extent1" : endcap_extent1, "endcap_extent2" : endcap_extent2, "joint_extent" : joint_extent, "dots_extent" : dots_extent, "endcap_angle" : endcap_angle, "endcap_angle1" : endcap_angle1, "endcap_angle2" : endcap_angle2, "joint_angle" : joint_angle, "dots_angle" : dots_angle, "endcap_color" : endcap_color, "endcap_color1" : endcap_color1, "endcap_color2" : endcap_color2, "joint_color" : joint_color, "dots_color" : dots_color, "color" : color, "trim" : trim, "trim1" : trim1, "trim2" : trim2, "convexity" : convexity, "hull" : hull, **kwargs})
 
-class dashed_stroke(OpenSCADObject):
+class dashed_stroke(_Bosl2Base):
     def __init__(self, path=None, dashpat=None, closed=None, **kwargs):
        super().__init__("dashed_stroke", {"path" : path, "dashpat" : dashpat, "closed" : closed, **kwargs})
 
-class arc(OpenSCADObject):
+class arc(_Bosl2Base):
     def __init__(self, n=None, r=None, angle=None, d=None, cp=None, points=None, corner=None, width=None, thickness=None, start=None, wedge=None, long=None, cw=None, ccw=None, endpoint=None, **kwargs):
        super().__init__("arc", {"n" : n, "r" : r, "angle" : angle, "d" : d, "cp" : cp, "points" : points, "corner" : corner, "width" : width, "thickness" : thickness, "start" : start, "wedge" : wedge, "long" : long, "cw" : cw, "ccw" : ccw, "endpoint" : endpoint, **kwargs})
 
-class helix(OpenSCADObject):
+class helix(_Bosl2Base):
     def __init__(self, l=None, h=None, turns=None, angle=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, **kwargs):
        super().__init__("helix", {"l" : l, "h" : h, "turns" : turns, "angle" : angle, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, **kwargs})
 
-class _normal_segment(OpenSCADObject):
+class _normal_segment(_Bosl2Base):
     def __init__(self, p1=None, p2=None, **kwargs):
        super().__init__("_normal_segment", {"p1" : p1, "p2" : p2, **kwargs})
 
-class turtle(OpenSCADObject):
+class turtle(_Bosl2Base):
     def __init__(self, commands=None, state=None, full_state=None, repeat=None, **kwargs):
        super().__init__("turtle", {"commands" : commands, "state" : state, "full_state" : full_state, "repeat" : repeat, **kwargs})
 
-class _turtle_repeat(OpenSCADObject):
+class _turtle_repeat(_Bosl2Base):
     def __init__(self, commands=None, state=None, full_state=None, repeat=None, **kwargs):
        super().__init__("_turtle_repeat", {"commands" : commands, "state" : state, "full_state" : full_state, "repeat" : repeat, **kwargs})
 
-class _turtle_command_len(OpenSCADObject):
+class _turtle_command_len(_Bosl2Base):
     def __init__(self, commands=None, index=None, **kwargs):
        super().__init__("_turtle_command_len", {"commands" : commands, "index" : index, **kwargs})
 
-class _turtle(OpenSCADObject):
+class _turtle(_Bosl2Base):
     def __init__(self, commands=None, state=None, full_state=None, index=None, **kwargs):
        super().__init__("_turtle", {"commands" : commands, "state" : state, "full_state" : full_state, "index" : index, **kwargs})
 
-class _turtle_command(OpenSCADObject):
+class _turtle_command(_Bosl2Base):
     def __init__(self, command=None, parm=None, parm2=None, state=None, index=None, **kwargs):
        super().__init__("_turtle_command", {"command" : command, "parm" : parm, "parm2" : parm2, "state" : state, "index" : index, **kwargs})
 
+class stroke(_Bosl2Base):
+    def __init__(self, path=None, width=None, closed=None, endcaps=None, endcap1=None, endcap2=None, joints=None, dots=None, endcap_width=None, endcap_width1=None, endcap_width2=None, joint_width=None, dots_width=None, endcap_length=None, endcap_length1=None, endcap_length2=None, joint_length=None, dots_length=None, endcap_extent=None, endcap_extent1=None, endcap_extent2=None, joint_extent=None, dots_extent=None, endcap_angle=None, endcap_angle1=None, endcap_angle2=None, joint_angle=None, dots_angle=None, endcap_color=None, endcap_color1=None, endcap_color2=None, joint_color=None, dots_color=None, color=None, trim=None, trim1=None, trim2=None, convexity=None, hull=None, **kwargs):
+       super().__init__("stroke", {"path" : path, "width" : width, "closed" : closed, "endcaps" : endcaps, "endcap1" : endcap1, "endcap2" : endcap2, "joints" : joints, "dots" : dots, "endcap_width" : endcap_width, "endcap_width1" : endcap_width1, "endcap_width2" : endcap_width2, "joint_width" : joint_width, "dots_width" : dots_width, "endcap_length" : endcap_length, "endcap_length1" : endcap_length1, "endcap_length2" : endcap_length2, "joint_length" : joint_length, "dots_length" : dots_length, "endcap_extent" : endcap_extent, "endcap_extent1" : endcap_extent1, "endcap_extent2" : endcap_extent2, "joint_extent" : joint_extent, "dots_extent" : dots_extent, "endcap_angle" : endcap_angle, "endcap_angle1" : endcap_angle1, "endcap_angle2" : endcap_angle2, "joint_angle" : joint_angle, "dots_angle" : dots_angle, "endcap_color" : endcap_color, "endcap_color1" : endcap_color1, "endcap_color2" : endcap_color2, "joint_color" : joint_color, "dots_color" : dots_color, "color" : color, "trim" : trim, "trim1" : trim1, "trim2" : trim2, "convexity" : convexity, "hull" : hull, **kwargs})
+
+class dashed_stroke(_Bosl2Base):
+    def __init__(self, path=None, dashpat=None, width=None, closed=None, **kwargs):
+       super().__init__("dashed_stroke", {"path" : path, "dashpat" : dashpat, "width" : width, "closed" : closed, **kwargs})
+
+class arc(_Bosl2Base):
+    def __init__(self, n=None, r=None, angle=None, d=None, cp=None, points=None, corner=None, width=None, thickness=None, start=None, wedge=None, anchor=None, spin=None, **kwargs):
+       super().__init__("arc", {"n" : n, "r" : r, "angle" : angle, "d" : d, "cp" : cp, "points" : points, "corner" : corner, "width" : width, "thickness" : thickness, "start" : start, "wedge" : wedge, "anchor" : anchor, "spin" : spin, **kwargs})
+
+class helix(_Bosl2Base):
+    def __init__(self, l=None, h=None, turns=None, angle=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, **kwargs):
+       super().__init__("helix", {"l" : l, "h" : h, "turns" : turns, "angle" : angle, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, **kwargs})
+
+class turtle(_Bosl2Base):
+    def __init__(self, commands=None, state=None, full_state=None, repeat=None, **kwargs):
+       super().__init__("turtle", {"commands" : commands, "state" : state, "full_state" : full_state, "repeat" : repeat, **kwargs})
+
+class debug_polygon(_Bosl2Base):
+    def __init__(self, points=None, paths=None, vertices=None, edges=None, convexity=None, size=None, **kwargs):
+       super().__init__("debug_polygon", {"points" : points, "paths" : paths, "vertices" : vertices, "edges" : edges, "convexity" : convexity, "size" : size, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/fnliterals.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/fnliterals.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,358 +1,360 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/fnliterals.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class map(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/fnliterals.scad'}", use_not_include=False)
+
+class map(_Bosl2Base):
     def __init__(self, func=None, list=None, **kwargs):
        super().__init__("map", {"func" : func, "list" : list, **kwargs})
 
-class filter(OpenSCADObject):
+class filter(_Bosl2Base):
     def __init__(self, func=None, list=None, **kwargs):
        super().__init__("filter", {"func" : func, "list" : list, **kwargs})
 
-class reduce(OpenSCADObject):
+class reduce(_Bosl2Base):
     def __init__(self, func=None, list=None, init=None, **kwargs):
        super().__init__("reduce", {"func" : func, "list" : list, "init" : init, **kwargs})
 
-class accumulate(OpenSCADObject):
+class accumulate(_Bosl2Base):
     def __init__(self, func=None, list=None, init=None, **kwargs):
        super().__init__("accumulate", {"func" : func, "list" : list, "init" : init, **kwargs})
 
-class _while(OpenSCADObject):
+class _while(_Bosl2Base):
     def __init__(self, init=None, cond=None, func=None, **kwargs):
        super().__init__("_while", {"init" : init, "cond" : cond, "func" : func, **kwargs})
 
-class for_n(OpenSCADObject):
+class for_n(_Bosl2Base):
     def __init__(self, n=None, init=None, func=None, **kwargs):
        super().__init__("for_n", {"n" : n, "init" : init, "func" : func, **kwargs})
 
-class find_all(OpenSCADObject):
+class find_all(_Bosl2Base):
     def __init__(self, func=None, list=None, **kwargs):
        super().__init__("find_all", {"func" : func, "list" : list, **kwargs})
 
-class find_first(OpenSCADObject):
+class find_first(_Bosl2Base):
     def __init__(self, func=None, list=None, start=None, **kwargs):
        super().__init__("find_first", {"func" : func, "list" : list, "start" : start, **kwargs})
 
-class binsearch(OpenSCADObject):
+class binsearch(_Bosl2Base):
     def __init__(self, key=None, list=None, idx=None, cmp=None, **kwargs):
        super().__init__("binsearch", {"key" : key, "list" : list, "idx" : idx, "cmp" : cmp, **kwargs})
 
-class simple_hash(OpenSCADObject):
+class simple_hash(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("simple_hash", {"x" : x, **kwargs})
 
-class hashmap(OpenSCADObject):
+class hashmap(_Bosl2Base):
     def __init__(self, hashsize=None, items=None, table=None, **kwargs):
        super().__init__("hashmap", {"hashsize" : hashsize, "items" : items, "table" : table, **kwargs})
 
-class f_1arg(OpenSCADObject):
+class f_1arg(_Bosl2Base):
     def __init__(self, target_func=None, **kwargs):
        super().__init__("f_1arg", {"target_func" : target_func, **kwargs})
 
-class f_2arg(OpenSCADObject):
+class f_2arg(_Bosl2Base):
     def __init__(self, target_func=None, **kwargs):
        super().__init__("f_2arg", {"target_func" : target_func, **kwargs})
 
-class f_2arg_simple(OpenSCADObject):
+class f_2arg_simple(_Bosl2Base):
     def __init__(self, target_func=None, **kwargs):
        super().__init__("f_2arg_simple", {"target_func" : target_func, **kwargs})
 
-class f_3arg(OpenSCADObject):
+class f_3arg(_Bosl2Base):
     def __init__(self, target_func=None, **kwargs):
        super().__init__("f_3arg", {"target_func" : target_func, **kwargs})
 
-class ival(OpenSCADObject):
+class ival(_Bosl2Base):
     def __init__(self, target_func=None, **kwargs):
        super().__init__("ival", {"target_func" : target_func, **kwargs})
 
-class xval(OpenSCADObject):
+class xval(_Bosl2Base):
     def __init__(self, target_func=None, **kwargs):
        super().__init__("xval", {"target_func" : target_func, **kwargs})
 
-class f_cmp(OpenSCADObject):
+class f_cmp(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_cmp", {"a" : a, "b" : b, **kwargs})
 
-class f_gt(OpenSCADObject):
+class f_gt(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_gt", {"a" : a, "b" : b, **kwargs})
 
-class f_lt(OpenSCADObject):
+class f_lt(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_lt", {"a" : a, "b" : b, **kwargs})
 
-class f_gte(OpenSCADObject):
+class f_gte(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_gte", {"a" : a, "b" : b, **kwargs})
 
-class f_lte(OpenSCADObject):
+class f_lte(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_lte", {"a" : a, "b" : b, **kwargs})
 
-class f_eq(OpenSCADObject):
+class f_eq(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_eq", {"a" : a, "b" : b, **kwargs})
 
-class f_neq(OpenSCADObject):
+class f_neq(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_neq", {"a" : a, "b" : b, **kwargs})
 
-class f_approx(OpenSCADObject):
+class f_approx(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_approx", {"a" : a, "b" : b, **kwargs})
 
-class f_napprox(OpenSCADObject):
+class f_napprox(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_napprox", {"a" : a, "b" : b, **kwargs})
 
-class f_or(OpenSCADObject):
+class f_or(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_or", {"a" : a, "b" : b, **kwargs})
 
-class f_and(OpenSCADObject):
+class f_and(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_and", {"a" : a, "b" : b, **kwargs})
 
-class f_nor(OpenSCADObject):
+class f_nor(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_nor", {"a" : a, "b" : b, **kwargs})
 
-class f_nand(OpenSCADObject):
+class f_nand(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_nand", {"a" : a, "b" : b, **kwargs})
 
-class f_xor(OpenSCADObject):
+class f_xor(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_xor", {"a" : a, "b" : b, **kwargs})
 
-class f_not(OpenSCADObject):
+class f_not(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_not", {"a" : a, **kwargs})
 
-class f_even(OpenSCADObject):
+class f_even(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_even", {"a" : a, **kwargs})
 
-class f_odd(OpenSCADObject):
+class f_odd(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_odd", {"a" : a, **kwargs})
 
-class f_add(OpenSCADObject):
+class f_add(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_add", {"a" : a, "b" : b, **kwargs})
 
-class f_sub(OpenSCADObject):
+class f_sub(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_sub", {"a" : a, "b" : b, **kwargs})
 
-class f_mul(OpenSCADObject):
+class f_mul(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_mul", {"a" : a, "b" : b, **kwargs})
 
-class f_div(OpenSCADObject):
+class f_div(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_div", {"a" : a, "b" : b, **kwargs})
 
-class f_mod(OpenSCADObject):
+class f_mod(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_mod", {"a" : a, "b" : b, **kwargs})
 
-class f_pow(OpenSCADObject):
+class f_pow(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_pow", {"a" : a, "b" : b, **kwargs})
 
-class f_neg(OpenSCADObject):
+class f_neg(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_neg", {"a" : a, **kwargs})
 
-class f_min(OpenSCADObject):
+class f_min(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_min", {"a" : a, **kwargs})
 
-class f_max(OpenSCADObject):
+class f_max(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_max", {"a" : a, **kwargs})
 
-class f_min2(OpenSCADObject):
+class f_min2(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_min2", {"a" : a, "b" : b, **kwargs})
 
-class f_max2(OpenSCADObject):
+class f_max2(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_max2", {"a" : a, "b" : b, **kwargs})
 
-class f_min3(OpenSCADObject):
+class f_min3(_Bosl2Base):
     def __init__(self, a=None, b=None, c=None, **kwargs):
        super().__init__("f_min3", {"a" : a, "b" : b, "c" : c, **kwargs})
 
-class f_max3(OpenSCADObject):
+class f_max3(_Bosl2Base):
     def __init__(self, a=None, b=None, c=None, **kwargs):
        super().__init__("f_max3", {"a" : a, "b" : b, "c" : c, **kwargs})
 
-class f_sin(OpenSCADObject):
+class f_sin(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_sin", {"a" : a, **kwargs})
 
-class f_cos(OpenSCADObject):
+class f_cos(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_cos", {"a" : a, **kwargs})
 
-class f_tan(OpenSCADObject):
+class f_tan(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_tan", {"a" : a, **kwargs})
 
-class f_asin(OpenSCADObject):
+class f_asin(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_asin", {"a" : a, **kwargs})
 
-class f_acos(OpenSCADObject):
+class f_acos(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_acos", {"a" : a, **kwargs})
 
-class f_atan(OpenSCADObject):
+class f_atan(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_atan", {"a" : a, **kwargs})
 
-class f_atan2(OpenSCADObject):
+class f_atan2(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_atan2", {"a" : a, "b" : b, **kwargs})
 
-class f_len(OpenSCADObject):
+class f_len(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_len", {"a" : a, **kwargs})
 
-class f_chr(OpenSCADObject):
+class f_chr(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_chr", {"a" : a, **kwargs})
 
-class f_ord(OpenSCADObject):
+class f_ord(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_ord", {"a" : a, **kwargs})
 
-class f_str(OpenSCADObject):
+class f_str(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_str", {"a" : a, **kwargs})
 
-class f_str2(OpenSCADObject):
+class f_str2(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_str2", {"a" : a, "b" : b, **kwargs})
 
-class f_str3(OpenSCADObject):
+class f_str3(_Bosl2Base):
     def __init__(self, a=None, b=None, c=None, **kwargs):
        super().__init__("f_str3", {"a" : a, "b" : b, "c" : c, **kwargs})
 
-class f_floor(OpenSCADObject):
+class f_floor(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_floor", {"a" : a, **kwargs})
 
-class f_round(OpenSCADObject):
+class f_round(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_round", {"a" : a, **kwargs})
 
-class f_ceil(OpenSCADObject):
+class f_ceil(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_ceil", {"a" : a, **kwargs})
 
-class f_abs(OpenSCADObject):
+class f_abs(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_abs", {"a" : a, **kwargs})
 
-class f_sign(OpenSCADObject):
+class f_sign(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_sign", {"a" : a, **kwargs})
 
-class f_ln(OpenSCADObject):
+class f_ln(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_ln", {"a" : a, **kwargs})
 
-class f_log(OpenSCADObject):
+class f_log(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_log", {"a" : a, **kwargs})
 
-class f_exp(OpenSCADObject):
+class f_exp(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_exp", {"a" : a, **kwargs})
 
-class f_sqr(OpenSCADObject):
+class f_sqr(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_sqr", {"a" : a, **kwargs})
 
-class f_sqrt(OpenSCADObject):
+class f_sqrt(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_sqrt", {"a" : a, **kwargs})
 
-class f_norm(OpenSCADObject):
+class f_norm(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_norm", {"a" : a, **kwargs})
 
-class f_cross(OpenSCADObject):
+class f_cross(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_cross", {"a" : a, "b" : b, **kwargs})
 
-class f_is_def(OpenSCADObject):
+class f_is_def(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_def", {"x" : x, **kwargs})
 
-class f_is_undef(OpenSCADObject):
+class f_is_undef(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_undef", {"x" : x, **kwargs})
 
-class f_is_bool(OpenSCADObject):
+class f_is_bool(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_bool", {"x" : x, **kwargs})
 
-class f_is_num(OpenSCADObject):
+class f_is_num(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_num", {"x" : x, **kwargs})
 
-class f_is_int(OpenSCADObject):
+class f_is_int(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_int", {"x" : x, **kwargs})
 
-class f_is_nan(OpenSCADObject):
+class f_is_nan(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_nan", {"x" : x, **kwargs})
 
-class f_is_finite(OpenSCADObject):
+class f_is_finite(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_finite", {"x" : x, **kwargs})
 
-class f_is_string(OpenSCADObject):
+class f_is_string(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_string", {"x" : x, **kwargs})
 
-class f_is_list(OpenSCADObject):
+class f_is_list(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_list", {"x" : x, **kwargs})
 
-class f_is_range(OpenSCADObject):
+class f_is_range(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_range", {"x" : x, **kwargs})
 
-class f_is_function(OpenSCADObject):
+class f_is_function(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("f_is_function", {"x" : x, **kwargs})
 
-class f_is_vector(OpenSCADObject):
+class f_is_vector(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_is_vector", {"a" : a, "b" : b, **kwargs})
 
-class f_is_path(OpenSCADObject):
+class f_is_path(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("f_is_path", {"a" : a, "b" : b, **kwargs})
 
-class f_is_region(OpenSCADObject):
+class f_is_region(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_is_region", {"a" : a, **kwargs})
 
-class f_is_vnf(OpenSCADObject):
+class f_is_vnf(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_is_vnf", {"a" : a, **kwargs})
 
-class f_is_patch(OpenSCADObject):
+class f_is_patch(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("f_is_patch", {"a" : a, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/gears.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/gears.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,136 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/gears.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class spur_gear(OpenSCADObject):
-    def __init__(self, pitch=None, teeth=None, thickness=None, shaft_diam=None, hide=None, pressure_angle=None, clearance=None, backlash=None, helical=None, slices=None, interior=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("spur_gear", {"pitch" : pitch, "teeth" : teeth, "thickness" : thickness, "shaft_diam" : shaft_diam, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "helical" : helical, "slices" : slices, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class spur_gear2d(OpenSCADObject):
-    def __init__(self, pitch=None, teeth=None, hide=None, pressure_angle=None, clearance=None, backlash=None, interior=None, mod=None, anchor=None, spin=None, **kwargs):
-       super().__init__("spur_gear2d", {"pitch" : pitch, "teeth" : teeth, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, **kwargs})
-
-class rack(OpenSCADObject):
-    def __init__(self, pitch=None, teeth=None, thickness=None, height=None, pressure_angle=None, backlash=None, clearance=None, helical=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("rack", {"pitch" : pitch, "teeth" : teeth, "thickness" : thickness, "height" : height, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "helical" : helical, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class rack2d(OpenSCADObject):
-    def __init__(self, pitch=None, teeth=None, height=None, pressure_angle=None, backlash=None, clearance=None, mod=None, anchor=None, spin=None, **kwargs):
-       super().__init__("rack2d", {"pitch" : pitch, "teeth" : teeth, "height" : height, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "mod" : mod, "anchor" : anchor, "spin" : spin, **kwargs})
-
-class bevel_gear(OpenSCADObject):
-    def __init__(self, pitch=None, teeth=None, face_width=None, pitch_angle=None, mate_teeth=None, shaft_diam=None, hide=None, pressure_angle=None, clearance=None, backlash=None, cutter_radius=None, spiral_angle=None, left_handed=None, slices=None, interior=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("bevel_gear", {"pitch" : pitch, "teeth" : teeth, "face_width" : face_width, "pitch_angle" : pitch_angle, "mate_teeth" : mate_teeth, "shaft_diam" : shaft_diam, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "cutter_radius" : cutter_radius, "spiral_angle" : spiral_angle, "left_handed" : left_handed, "slices" : slices, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class worm(OpenSCADObject):
-    def __init__(self, pitch=None, d=None, l=None, starts=None, left_handed=None, pressure_angle=None, backlash=None, clearance=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("worm", {"pitch" : pitch, "d" : d, "l" : l, "starts" : starts, "left_handed" : left_handed, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class worm_gear(OpenSCADObject):
-    def __init__(self, pitch=None, teeth=None, worm_diam=None, worm_starts=None, worm_arc=None, crowning=None, left_handed=None, pressure_angle=None, backlash=None, slices=None, clearance=None, mod=None, shaft_diam=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("worm_gear", {"pitch" : pitch, "teeth" : teeth, "worm_diam" : worm_diam, "worm_starts" : worm_starts, "worm_arc" : worm_arc, "crowning" : crowning, "left_handed" : left_handed, "pressure_angle" : pressure_angle, "backlash" : backlash, "slices" : slices, "clearance" : clearance, "mod" : mod, "shaft_diam" : shaft_diam, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class _gear_tooth_profile(OpenSCADObject):
-    def __init__(self, pitch=None, teeth=None, pressure_angle=None, backlash=None, clearance=None, interior=None, valleys=None, center=None, mod=None, **kwargs):
-       super().__init__("_gear_tooth_profile", {"pitch" : pitch, "teeth" : teeth, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "interior" : interior, "valleys" : valleys, "center" : center, "mod" : mod, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/gears.scad'}", use_not_include=False)
 
-class spur_gear(OpenSCADObject):
+class spur_gear(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, thickness=None, shaft_diam=None, hide=None, pressure_angle=None, clearance=None, backlash=None, helical=None, slices=None, interior=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("spur_gear", {"pitch" : pitch, "teeth" : teeth, "thickness" : thickness, "shaft_diam" : shaft_diam, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "helical" : helical, "slices" : slices, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class spur_gear2d(OpenSCADObject):
+class spur_gear2d(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, hide=None, pressure_angle=None, clearance=None, backlash=None, interior=None, mod=None, anchor=None, spin=None, **kwargs):
        super().__init__("spur_gear2d", {"pitch" : pitch, "teeth" : teeth, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class rack(OpenSCADObject):
+class rack(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, thickness=None, height=None, pressure_angle=None, backlash=None, clearance=None, helical=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rack", {"pitch" : pitch, "teeth" : teeth, "thickness" : thickness, "height" : height, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "helical" : helical, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rack2d(OpenSCADObject):
+class rack2d(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, height=None, pressure_angle=None, backlash=None, clearance=None, mod=None, anchor=None, spin=None, **kwargs):
        super().__init__("rack2d", {"pitch" : pitch, "teeth" : teeth, "height" : height, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "mod" : mod, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class bevel_gear(OpenSCADObject):
+class bevel_gear(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, face_width=None, pitch_angle=None, mate_teeth=None, hide=None, pressure_angle=None, clearance=None, backlash=None, cutter_radius=None, spiral_angle=None, left_handed=None, slices=None, interior=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("bevel_gear", {"pitch" : pitch, "teeth" : teeth, "face_width" : face_width, "pitch_angle" : pitch_angle, "mate_teeth" : mate_teeth, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "cutter_radius" : cutter_radius, "spiral_angle" : spiral_angle, "left_handed" : left_handed, "slices" : slices, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class worm(OpenSCADObject):
+class worm(_Bosl2Base):
     def __init__(self, pitch=None, d=None, l=None, starts=None, left_handed=None, pressure_angle=None, backlash=None, clearance=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("worm", {"pitch" : pitch, "d" : d, "l" : l, "starts" : starts, "left_handed" : left_handed, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class worm_gear(OpenSCADObject):
+class worm_gear(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, worm_diam=None, worm_starts=None, worm_arc=None, crowning=None, left_handed=None, pressure_angle=None, backlash=None, clearance=None, mod=None, slices=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("worm_gear", {"pitch" : pitch, "teeth" : teeth, "worm_diam" : worm_diam, "worm_starts" : worm_starts, "worm_arc" : worm_arc, "crowning" : crowning, "left_handed" : left_handed, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "mod" : mod, "slices" : slices, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class _gear_tooth_profile(OpenSCADObject):
+class _gear_tooth_profile(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, pressure_angle=None, clearance=None, backlash=None, interior=None, valleys=None, center=None, mod=None, **kwargs):
        super().__init__("_gear_tooth_profile", {"pitch" : pitch, "teeth" : teeth, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "interior" : interior, "valleys" : valleys, "center" : center, "mod" : mod, **kwargs})
 
-class circular_pitch(OpenSCADObject):
+class circular_pitch(_Bosl2Base):
     def __init__(self, pitch=None, mod=None, **kwargs):
        super().__init__("circular_pitch", {"pitch" : pitch, "mod" : mod, **kwargs})
 
-class diametral_pitch(OpenSCADObject):
+class diametral_pitch(_Bosl2Base):
     def __init__(self, pitch=None, mod=None, **kwargs):
        super().__init__("diametral_pitch", {"pitch" : pitch, "mod" : mod, **kwargs})
 
-class pitch_value(OpenSCADObject):
+class pitch_value(_Bosl2Base):
     def __init__(self, mod=None, **kwargs):
        super().__init__("pitch_value", {"mod" : mod, **kwargs})
 
-class module_value(OpenSCADObject):
+class module_value(_Bosl2Base):
     def __init__(self, pitch=None, **kwargs):
        super().__init__("module_value", {"pitch" : pitch, **kwargs})
 
-class _adendum(OpenSCADObject):
+class _adendum(_Bosl2Base):
     def __init__(self, pitch=None, mod=None, **kwargs):
        super().__init__("_adendum", {"pitch" : pitch, "mod" : mod, **kwargs})
 
-class _dedendum(OpenSCADObject):
+class _dedendum(_Bosl2Base):
     def __init__(self, pitch=None, clearance=None, mod=None, **kwargs):
        super().__init__("_dedendum", {"pitch" : pitch, "clearance" : clearance, "mod" : mod, **kwargs})
 
-class pitch_radius(OpenSCADObject):
+class pitch_radius(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, mod=None, **kwargs):
        super().__init__("pitch_radius", {"pitch" : pitch, "teeth" : teeth, "mod" : mod, **kwargs})
 
-class outer_radius(OpenSCADObject):
+class outer_radius(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, clearance=None, interior=None, mod=None, **kwargs):
        super().__init__("outer_radius", {"pitch" : pitch, "teeth" : teeth, "clearance" : clearance, "interior" : interior, "mod" : mod, **kwargs})
 
-class _root_radius(OpenSCADObject):
+class _root_radius(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, clearance=None, interior=None, mod=None, **kwargs):
        super().__init__("_root_radius", {"pitch" : pitch, "teeth" : teeth, "clearance" : clearance, "interior" : interior, "mod" : mod, **kwargs})
 
-class _base_radius(OpenSCADObject):
+class _base_radius(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, pressure_angle=None, mod=None, **kwargs):
        super().__init__("_base_radius", {"pitch" : pitch, "teeth" : teeth, "pressure_angle" : pressure_angle, "mod" : mod, **kwargs})
 
-class bevel_pitch_angle(OpenSCADObject):
+class bevel_pitch_angle(_Bosl2Base):
     def __init__(self, teeth=None, mate_teeth=None, drive_angle=None, **kwargs):
        super().__init__("bevel_pitch_angle", {"teeth" : teeth, "mate_teeth" : mate_teeth, "drive_angle" : drive_angle, **kwargs})
 
-class worm_gear_thickness(OpenSCADObject):
+class worm_gear_thickness(_Bosl2Base):
     def __init__(self, pitch=None, teeth=None, worm_diam=None, worm_arc=None, crowning=None, clearance=None, mod=None, **kwargs):
        super().__init__("worm_gear_thickness", {"pitch" : pitch, "teeth" : teeth, "worm_diam" : worm_diam, "worm_arc" : worm_arc, "crowning" : crowning, "clearance" : clearance, "mod" : mod, **kwargs})
 
-class _gear_polar(OpenSCADObject):
+class _gear_polar(_Bosl2Base):
     def __init__(self, r=None, t=None, **kwargs):
        super().__init__("_gear_polar", {"r" : r, "t" : t, **kwargs})
 
-class _gear_iang(OpenSCADObject):
+class _gear_iang(_Bosl2Base):
     def __init__(self, r1=None, r2=None, **kwargs):
        super().__init__("_gear_iang", {"r1" : r1, "r2" : r2, **kwargs})
 
-class _gear_q6(OpenSCADObject):
+class _gear_q6(_Bosl2Base):
     def __init__(self, b=None, s=None, t=None, d=None, **kwargs):
        super().__init__("_gear_q6", {"b" : b, "s" : s, "t" : t, "d" : d, **kwargs})
 
-class _gear_q7(OpenSCADObject):
+class _gear_q7(_Bosl2Base):
     def __init__(self, f=None, r=None, b=None, r2=None, t=None, s=None, **kwargs):
        super().__init__("_gear_q7", {"f" : f, "r" : r, "b" : b, "r2" : r2, "t" : t, "s" : s, **kwargs})
 
+class spur_gear(_Bosl2Base):
+    def __init__(self, pitch=None, teeth=None, thickness=None, shaft_diam=None, hide=None, pressure_angle=None, clearance=None, backlash=None, helical=None, slices=None, interior=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("spur_gear", {"pitch" : pitch, "teeth" : teeth, "thickness" : thickness, "shaft_diam" : shaft_diam, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "helical" : helical, "slices" : slices, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class spur_gear2d(_Bosl2Base):
+    def __init__(self, pitch=None, teeth=None, hide=None, pressure_angle=None, clearance=None, backlash=None, interior=None, mod=None, anchor=None, spin=None, **kwargs):
+       super().__init__("spur_gear2d", {"pitch" : pitch, "teeth" : teeth, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, **kwargs})
+
+class rack(_Bosl2Base):
+    def __init__(self, pitch=None, teeth=None, thickness=None, height=None, pressure_angle=None, backlash=None, clearance=None, helical=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("rack", {"pitch" : pitch, "teeth" : teeth, "thickness" : thickness, "height" : height, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "helical" : helical, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class rack2d(_Bosl2Base):
+    def __init__(self, pitch=None, teeth=None, height=None, pressure_angle=None, backlash=None, clearance=None, mod=None, anchor=None, spin=None, **kwargs):
+       super().__init__("rack2d", {"pitch" : pitch, "teeth" : teeth, "height" : height, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "mod" : mod, "anchor" : anchor, "spin" : spin, **kwargs})
+
+class bevel_gear(_Bosl2Base):
+    def __init__(self, pitch=None, teeth=None, face_width=None, pitch_angle=None, mate_teeth=None, shaft_diam=None, hide=None, pressure_angle=None, clearance=None, backlash=None, cutter_radius=None, spiral_angle=None, left_handed=None, slices=None, interior=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("bevel_gear", {"pitch" : pitch, "teeth" : teeth, "face_width" : face_width, "pitch_angle" : pitch_angle, "mate_teeth" : mate_teeth, "shaft_diam" : shaft_diam, "hide" : hide, "pressure_angle" : pressure_angle, "clearance" : clearance, "backlash" : backlash, "cutter_radius" : cutter_radius, "spiral_angle" : spiral_angle, "left_handed" : left_handed, "slices" : slices, "interior" : interior, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class worm(_Bosl2Base):
+    def __init__(self, pitch=None, d=None, l=None, starts=None, left_handed=None, pressure_angle=None, backlash=None, clearance=None, mod=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("worm", {"pitch" : pitch, "d" : d, "l" : l, "starts" : starts, "left_handed" : left_handed, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "mod" : mod, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class worm_gear(_Bosl2Base):
+    def __init__(self, pitch=None, teeth=None, worm_diam=None, worm_starts=None, worm_arc=None, crowning=None, left_handed=None, pressure_angle=None, backlash=None, slices=None, clearance=None, mod=None, shaft_diam=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("worm_gear", {"pitch" : pitch, "teeth" : teeth, "worm_diam" : worm_diam, "worm_starts" : worm_starts, "worm_arc" : worm_arc, "crowning" : crowning, "left_handed" : left_handed, "pressure_angle" : pressure_angle, "backlash" : backlash, "slices" : slices, "clearance" : clearance, "mod" : mod, "shaft_diam" : shaft_diam, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class _gear_tooth_profile(_Bosl2Base):
+    def __init__(self, pitch=None, teeth=None, pressure_angle=None, backlash=None, clearance=None, interior=None, valleys=None, center=None, mod=None, **kwargs):
+       super().__init__("_gear_tooth_profile", {"pitch" : pitch, "teeth" : teeth, "pressure_angle" : pressure_angle, "backlash" : backlash, "clearance" : clearance, "interior" : interior, "valleys" : valleys, "center" : center, "mod" : mod, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/geometry.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/threading.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,378 +1,128 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/geometry.scad'}", use_not_include=False)
-
-class hull_points(OpenSCADObject):
-    def __init__(self, points=None, fast=None, **kwargs):
-       super().__init__("hull_points", {"points" : points, "fast" : fast, **kwargs})
-
-class is_point_on_line(OpenSCADObject):
-    def __init__(self, point=None, line=None, bounded=None, eps=None, **kwargs):
-       super().__init__("is_point_on_line", {"point" : point, "line" : line, "bounded" : bounded, "eps" : eps, **kwargs})
-
-class _is_point_on_line(OpenSCADObject):
-    def __init__(self, point=None, line=None, bounded=None, eps=None, **kwargs):
-       super().__init__("_is_point_on_line", {"point" : point, "line" : line, "bounded" : bounded, "eps" : eps, **kwargs})
-
-class _dist2line(OpenSCADObject):
-    def __init__(self, d=None, n=None, **kwargs):
-       super().__init__("_dist2line", {"d" : d, "n" : n, **kwargs})
-
-class _valid_line(OpenSCADObject):
-    def __init__(self, line=None, dim=None, eps=None, **kwargs):
-       super().__init__("_valid_line", {"line" : line, "dim" : dim, "eps" : eps, **kwargs})
-
-class _valid_plane(OpenSCADObject):
-    def __init__(self, p=None, eps=None, **kwargs):
-       super().__init__("_valid_plane", {"p" : p, "eps" : eps, **kwargs})
-
-class _is_at_left(OpenSCADObject):
-    def __init__(self, pt=None, line=None, eps=None, **kwargs):
-       super().__init__("_is_at_left", {"pt" : pt, "line" : line, "eps" : eps, **kwargs})
-
-class _degenerate_tri(OpenSCADObject):
-    def __init__(self, tri=None, eps=None, **kwargs):
-       super().__init__("_degenerate_tri", {"tri" : tri, "eps" : eps, **kwargs})
-
-class _tri_class(OpenSCADObject):
-    def __init__(self, tri=None, eps=None, **kwargs):
-       super().__init__("_tri_class", {"tri" : tri, "eps" : eps, **kwargs})
-
-class _pt_in_tri(OpenSCADObject):
-    def __init__(self, point=None, tri=None, eps=None, **kwargs):
-       super().__init__("_pt_in_tri", {"point" : point, "tri" : tri, "eps" : eps, **kwargs})
-
-class _point_left_of_line2d(OpenSCADObject):
-    def __init__(self, point=None, line=None, eps=None, **kwargs):
-       super().__init__("_point_left_of_line2d", {"point" : point, "line" : line, "eps" : eps, **kwargs})
-
-class is_collinear(OpenSCADObject):
-    def __init__(self, a=None, b=None, c=None, eps=None, **kwargs):
-       super().__init__("is_collinear", {"a" : a, "b" : b, "c" : c, "eps" : eps, **kwargs})
-
-class point_line_distance(OpenSCADObject):
-    def __init__(self, pt=None, line=None, bounded=None, **kwargs):
-       super().__init__("point_line_distance", {"pt" : pt, "line" : line, "bounded" : bounded, **kwargs})
-
-class segment_distance(OpenSCADObject):
-    def __init__(self, seg1=None, seg2=None, eps=None, **kwargs):
-       super().__init__("segment_distance", {"seg1" : seg1, "seg2" : seg2, "eps" : eps, **kwargs})
-
-class line_normal(OpenSCADObject):
-    def __init__(self, p1=None, p2=None, **kwargs):
-       super().__init__("line_normal", {"p1" : p1, "p2" : p2, **kwargs})
-
-class _general_line_intersection(OpenSCADObject):
-    def __init__(self, s1=None, s2=None, eps=None, **kwargs):
-       super().__init__("_general_line_intersection", {"s1" : s1, "s2" : s2, "eps" : eps, **kwargs})
-
-class line_intersection(OpenSCADObject):
-    def __init__(self, line1=None, line2=None, bounded1=None, bounded2=None, bounded=None, eps=None, **kwargs):
-       super().__init__("line_intersection", {"line1" : line1, "line2" : line2, "bounded1" : bounded1, "bounded2" : bounded2, "bounded" : bounded, "eps" : eps, **kwargs})
-
-class line_closest_point(OpenSCADObject):
-    def __init__(self, line=None, pt=None, bounded=None, **kwargs):
-       super().__init__("line_closest_point", {"line" : line, "pt" : pt, "bounded" : bounded, **kwargs})
-
-class line_from_points(OpenSCADObject):
-    def __init__(self, points=None, fast=None, eps=None, **kwargs):
-       super().__init__("line_from_points", {"points" : points, "fast" : fast, "eps" : eps, **kwargs})
-
-class is_coplanar(OpenSCADObject):
-    def __init__(self, points=None, eps=None, **kwargs):
-       super().__init__("is_coplanar", {"points" : points, "eps" : eps, **kwargs})
-
-class plane3pt(OpenSCADObject):
-    def __init__(self, p1=None, p2=None, p3=None, **kwargs):
-       super().__init__("plane3pt", {"p1" : p1, "p2" : p2, "p3" : p3, **kwargs})
-
-class plane3pt_indexed(OpenSCADObject):
-    def __init__(self, points=None, i1=None, i2=None, i3=None, **kwargs):
-       super().__init__("plane3pt_indexed", {"points" : points, "i1" : i1, "i2" : i2, "i3" : i3, **kwargs})
-
-class plane_from_normal(OpenSCADObject):
-    def __init__(self, normal=None, pt=None, **kwargs):
-       super().__init__("plane_from_normal", {"normal" : normal, "pt" : pt, **kwargs})
-
-class _eigenvals_symm_3(OpenSCADObject):
-    def __init__(self, M=None, **kwargs):
-       super().__init__("_eigenvals_symm_3", {"M" : M, **kwargs})
-
-class _eigenvec_symm_3(OpenSCADObject):
-    def __init__(self, M=None, evals=None, i=None, **kwargs):
-       super().__init__("_eigenvec_symm_3", {"M" : M, "evals" : evals, "i" : i, **kwargs})
-
-class _covariance_evec_eval(OpenSCADObject):
-    def __init__(self, points=None, **kwargs):
-       super().__init__("_covariance_evec_eval", {"points" : points, **kwargs})
-
-class plane_from_points(OpenSCADObject):
-    def __init__(self, points=None, fast=None, eps=None, **kwargs):
-       super().__init__("plane_from_points", {"points" : points, "fast" : fast, "eps" : eps, **kwargs})
-
-class plane_from_polygon(OpenSCADObject):
-    def __init__(self, poly=None, fast=None, eps=None, **kwargs):
-       super().__init__("plane_from_polygon", {"poly" : poly, "fast" : fast, "eps" : eps, **kwargs})
-
-class plane_normal(OpenSCADObject):
-    def __init__(self, plane=None, **kwargs):
-       super().__init__("plane_normal", {"plane" : plane, **kwargs})
-
-class plane_offset(OpenSCADObject):
-    def __init__(self, plane=None, **kwargs):
-       super().__init__("plane_offset", {"plane" : plane, **kwargs})
-
-class _general_plane_line_intersection(OpenSCADObject):
-    def __init__(self, plane=None, line=None, eps=None, **kwargs):
-       super().__init__("_general_plane_line_intersection", {"plane" : plane, "line" : line, "eps" : eps, **kwargs})
-
-class _normalize_plane(OpenSCADObject):
-    def __init__(self, plane=None, **kwargs):
-       super().__init__("_normalize_plane", {"plane" : plane, **kwargs})
-
-class plane_line_intersection(OpenSCADObject):
-    def __init__(self, plane=None, line=None, bounded=None, eps=None, **kwargs):
-       super().__init__("plane_line_intersection", {"plane" : plane, "line" : line, "bounded" : bounded, "eps" : eps, **kwargs})
-
-class plane_intersection(OpenSCADObject):
-    def __init__(self, plane1=None, plane2=None, plane3=None, **kwargs):
-       super().__init__("plane_intersection", {"plane1" : plane1, "plane2" : plane2, "plane3" : plane3, **kwargs})
-
-class plane_line_angle(OpenSCADObject):
-    def __init__(self, plane=None, line=None, **kwargs):
-       super().__init__("plane_line_angle", {"plane" : plane, "line" : line, **kwargs})
-
-class plane_closest_point(OpenSCADObject):
-    def __init__(self, plane=None, points=None, **kwargs):
-       super().__init__("plane_closest_point", {"plane" : plane, "points" : points, **kwargs})
-
-class point_plane_distance(OpenSCADObject):
-    def __init__(self, plane=None, point=None, **kwargs):
-       super().__init__("point_plane_distance", {"plane" : plane, "point" : point, **kwargs})
-
-class _pointlist_greatest_distance(OpenSCADObject):
-    def __init__(self, points=None, plane=None, **kwargs):
-       super().__init__("_pointlist_greatest_distance", {"points" : points, "plane" : plane, **kwargs})
-
-class are_points_on_plane(OpenSCADObject):
-    def __init__(self, points=None, plane=None, eps=None, **kwargs):
-       super().__init__("are_points_on_plane", {"points" : points, "plane" : plane, "eps" : eps, **kwargs})
-
-class _is_point_above_plane(OpenSCADObject):
-    def __init__(self, plane=None, point=None, **kwargs):
-       super().__init__("_is_point_above_plane", {"plane" : plane, "point" : point, **kwargs})
-
-class circle_line_intersection(OpenSCADObject):
-    def __init__(self, r=None, cp=None, line=None, bounded=None, d=None, eps=None, **kwargs):
-       super().__init__("circle_line_intersection", {"r" : r, "cp" : cp, "line" : line, "bounded" : bounded, "d" : d, "eps" : eps, **kwargs})
-
-class _circle_or_sphere_line_intersection(OpenSCADObject):
-    def __init__(self, r=None, cp=None, line=None, bounded=None, d=None, eps=None, **kwargs):
-       super().__init__("_circle_or_sphere_line_intersection", {"r" : r, "cp" : cp, "line" : line, "bounded" : bounded, "d" : d, "eps" : eps, **kwargs})
-
-class circle_circle_intersection(OpenSCADObject):
-    def __init__(self, r1=None, cp1=None, r2=None, cp2=None, eps=None, d1=None, d2=None, **kwargs):
-       super().__init__("circle_circle_intersection", {"r1" : r1, "cp1" : cp1, "r2" : r2, "cp2" : cp2, "eps" : eps, "d1" : d1, "d2" : d2, **kwargs})
-
-class circle_2tangents(OpenSCADObject):
-    def __init__(self, r=None, pt1=None, pt2=None, pt3=None, tangents=None, d=None, **kwargs):
-       super().__init__("circle_2tangents", {"r" : r, "pt1" : pt1, "pt2" : pt2, "pt3" : pt3, "tangents" : tangents, "d" : d, **kwargs})
-
-class circle_3points(OpenSCADObject):
-    def __init__(self, pt1=None, pt2=None, pt3=None, **kwargs):
-       super().__init__("circle_3points", {"pt1" : pt1, "pt2" : pt2, "pt3" : pt3, **kwargs})
-
-class circle_point_tangents(OpenSCADObject):
-    def __init__(self, r=None, cp=None, pt=None, d=None, **kwargs):
-       super().__init__("circle_point_tangents", {"r" : r, "cp" : cp, "pt" : pt, "d" : d, **kwargs})
-
-class circle_circle_tangents(OpenSCADObject):
-    def __init__(self, r1=None, cp1=None, r2=None, cp2=None, d1=None, d2=None, **kwargs):
-       super().__init__("circle_circle_tangents", {"r1" : r1, "cp1" : cp1, "r2" : r2, "cp2" : cp2, "d1" : d1, "d2" : d2, **kwargs})
-
-class _noncollinear_triple(OpenSCADObject):
-    def __init__(self, points=None, error=None, eps=None, **kwargs):
-       super().__init__("_noncollinear_triple", {"points" : points, "error" : error, "eps" : eps, **kwargs})
-
-class sphere_line_intersection(OpenSCADObject):
-    def __init__(self, r=None, cp=None, line=None, bounded=None, d=None, eps=None, **kwargs):
-       super().__init__("sphere_line_intersection", {"r" : r, "cp" : cp, "line" : line, "bounded" : bounded, "d" : d, "eps" : eps, **kwargs})
-
-class polygon_area(OpenSCADObject):
-    def __init__(self, poly=None, signed=None, **kwargs):
-       super().__init__("polygon_area", {"poly" : poly, "signed" : signed, **kwargs})
-
-class centroid(OpenSCADObject):
-    def __init__(self, object=None, eps=None, **kwargs):
-       super().__init__("centroid", {"object" : object, "eps" : eps, **kwargs})
-
-class _region_centroid(OpenSCADObject):
-    def __init__(self, region=None, eps=None, **kwargs):
-       super().__init__("_region_centroid", {"region" : region, "eps" : eps, **kwargs})
-
-class _polygon_centroid(OpenSCADObject):
-    def __init__(self, poly=None, eps=None, **kwargs):
-       super().__init__("_polygon_centroid", {"poly" : poly, "eps" : eps, **kwargs})
-
-class polygon_normal(OpenSCADObject):
-    def __init__(self, poly=None, **kwargs):
-       super().__init__("polygon_normal", {"poly" : poly, **kwargs})
-
-class _point_above_below_segment(OpenSCADObject):
-    def __init__(self, point=None, edge=None, **kwargs):
-       super().__init__("_point_above_below_segment", {"point" : point, "edge" : edge, **kwargs})
-
-class point_in_polygon(OpenSCADObject):
-    def __init__(self, point=None, poly=None, nonzero=None, eps=None, **kwargs):
-       super().__init__("point_in_polygon", {"point" : point, "poly" : poly, "nonzero" : nonzero, "eps" : eps, **kwargs})
-
-class polygon_line_intersection(OpenSCADObject):
-    def __init__(self, poly=None, line=None, bounded=None, nonzero=None, eps=None, **kwargs):
-       super().__init__("polygon_line_intersection", {"poly" : poly, "line" : line, "bounded" : bounded, "nonzero" : nonzero, "eps" : eps, **kwargs})
-
-class _merge_segments(OpenSCADObject):
-    def __init__(self, insegs=None, outsegs=None, eps=None, i=None, **kwargs):
-       super().__init__("_merge_segments", {"insegs" : insegs, "outsegs" : outsegs, "eps" : eps, "i" : i, **kwargs})
-
-class polygon_triangulate(OpenSCADObject):
-    def __init__(self, poly=None, ind=None, error=None, eps=None, **kwargs):
-       super().__init__("polygon_triangulate", {"poly" : poly, "ind" : ind, "error" : error, "eps" : eps, **kwargs})
-
-class _triangulate(OpenSCADObject):
-    def __init__(self, poly=None, ind=None, error=None, eps=None, tris=None, **kwargs):
-       super().__init__("_triangulate", {"poly" : poly, "ind" : ind, "error" : error, "eps" : eps, "tris" : tris, **kwargs})
-
-class _get_ear(OpenSCADObject):
-    def __init__(self, poly=None, ind=None, eps=None, _i=None, **kwargs):
-       super().__init__("_get_ear", {"poly" : poly, "ind" : ind, "eps" : eps, "_i" : _i, **kwargs})
-
-class _none_inside(OpenSCADObject):
-    def __init__(self, idxs=None, poly=None, p0=None, p1=None, p2=None, eps=None, i=None, **kwargs):
-       super().__init__("_none_inside", {"idxs" : idxs, "poly" : poly, "p0" : p0, "p1" : p1, "p2" : p2, "eps" : eps, "i" : i, **kwargs})
-
-class is_polygon_clockwise(OpenSCADObject):
-    def __init__(self, poly=None, **kwargs):
-       super().__init__("is_polygon_clockwise", {"poly" : poly, **kwargs})
-
-class clockwise_polygon(OpenSCADObject):
-    def __init__(self, poly=None, **kwargs):
-       super().__init__("clockwise_polygon", {"poly" : poly, **kwargs})
-
-class ccw_polygon(OpenSCADObject):
-    def __init__(self, poly=None, **kwargs):
-       super().__init__("ccw_polygon", {"poly" : poly, **kwargs})
-
-class reverse_polygon(OpenSCADObject):
-    def __init__(self, poly=None, **kwargs):
-       super().__init__("reverse_polygon", {"poly" : poly, **kwargs})
-
-class reindex_polygon(OpenSCADObject):
-    def __init__(self, reference=None, poly=None, return_error=None, **kwargs):
-       super().__init__("reindex_polygon", {"reference" : reference, "poly" : poly, "return_error" : return_error, **kwargs})
-
-class align_polygon(OpenSCADObject):
-    def __init__(self, reference=None, poly=None, angles=None, cp=None, trans=None, return_ind=None, **kwargs):
-       super().__init__("align_polygon", {"reference" : reference, "poly" : poly, "angles" : angles, "cp" : cp, "trans" : trans, "return_ind" : return_ind, **kwargs})
-
-class are_polygons_equal(OpenSCADObject):
-    def __init__(self, poly1=None, poly2=None, eps=None, **kwargs):
-       super().__init__("are_polygons_equal", {"poly1" : poly1, "poly2" : poly2, "eps" : eps, **kwargs})
-
-class _are_polygons_equal(OpenSCADObject):
-    def __init__(self, poly1=None, poly2=None, eps=None, st=None, **kwargs):
-       super().__init__("_are_polygons_equal", {"poly1" : poly1, "poly2" : poly2, "eps" : eps, "st" : st, **kwargs})
-
-class _is_polygon_in_list(OpenSCADObject):
-    def __init__(self, poly=None, polys=None, **kwargs):
-       super().__init__("_is_polygon_in_list", {"poly" : poly, "polys" : polys, **kwargs})
-
-class ___is_polygon_in_list(OpenSCADObject):
-    def __init__(self, poly=None, polys=None, i=None, **kwargs):
-       super().__init__("___is_polygon_in_list", {"poly" : poly, "polys" : polys, "i" : i, **kwargs})
-
-class hull(OpenSCADObject):
-    def __init__(self, points=None, **kwargs):
-       super().__init__("hull", {"points" : points, **kwargs})
-
-class _backtracking(OpenSCADObject):
-    def __init__(self, i=None, points=None, h=None, t=None, m=None, all=None, **kwargs):
-       super().__init__("_backtracking", {"i" : i, "points" : points, "h" : h, "t" : t, "m" : m, "all" : all, **kwargs})
-
-class _is_cw(OpenSCADObject):
-    def __init__(self, a=None, b=None, c=None, all=None, **kwargs):
-       super().__init__("_is_cw", {"a" : a, "b" : b, "c" : c, "all" : all, **kwargs})
-
-class hull2d_path(OpenSCADObject):
-    def __init__(self, points=None, all=None, **kwargs):
-       super().__init__("hull2d_path", {"points" : points, "all" : all, **kwargs})
-
-class _hull_collinear(OpenSCADObject):
-    def __init__(self, points=None, **kwargs):
-       super().__init__("_hull_collinear", {"points" : points, **kwargs})
-
-class hull3d_faces(OpenSCADObject):
-    def __init__(self, points=None, **kwargs):
-       super().__init__("hull3d_faces", {"points" : points, **kwargs})
-
-class _hull3d_iterative(OpenSCADObject):
-    def __init__(self, points=None, triangles=None, planes=None, remaining=None, _i=None, **kwargs):
-       super().__init__("_hull3d_iterative", {"points" : points, "triangles" : triangles, "planes" : planes, "remaining" : remaining, "_i" : _i, **kwargs})
-
-class _remove_internal_edges(OpenSCADObject):
-    def __init__(self, halfedges=None, **kwargs):
-       super().__init__("_remove_internal_edges", {"halfedges" : halfedges, **kwargs})
-
-class _find_first_noncoplanar(OpenSCADObject):
-    def __init__(self, plane=None, points=None, i=None, **kwargs):
-       super().__init__("_find_first_noncoplanar", {"plane" : plane, "points" : points, "i" : i, **kwargs})
-
-class is_polygon_convex(OpenSCADObject):
-    def __init__(self, poly=None, eps=None, **kwargs):
-       super().__init__("is_polygon_convex", {"poly" : poly, "eps" : eps, **kwargs})
-
-class convex_distance(OpenSCADObject):
-    def __init__(self, points1=None, points2=None, eps=None, **kwargs):
-       super().__init__("convex_distance", {"points1" : points1, "points2" : points2, "eps" : eps, **kwargs})
-
-class _GJK_distance(OpenSCADObject):
-    def __init__(self, points1=None, points2=None, eps=None, lbd=None, d=None, simplex=None, **kwargs):
-       super().__init__("_GJK_distance", {"points1" : points1, "points2" : points2, "eps" : eps, "lbd" : lbd, "d" : d, "simplex" : simplex, **kwargs})
-
-class convex_collision(OpenSCADObject):
-    def __init__(self, points1=None, points2=None, eps=None, **kwargs):
-       super().__init__("convex_collision", {"points1" : points1, "points2" : points2, "eps" : eps, **kwargs})
-
-class _GJK_collide(OpenSCADObject):
-    def __init__(self, points1=None, points2=None, d=None, simplex=None, eps=None, **kwargs):
-       super().__init__("_GJK_collide", {"points1" : points1, "points2" : points2, "d" : d, "simplex" : simplex, "eps" : eps, **kwargs})
-
-class _closest_simplex(OpenSCADObject):
-    def __init__(self, s=None, eps=None, **kwargs):
-       super().__init__("_closest_simplex", {"s" : s, "eps" : eps, **kwargs})
-
-class _closest_s1(OpenSCADObject):
-    def __init__(self, s=None, eps=None, **kwargs):
-       super().__init__("_closest_s1", {"s" : s, "eps" : eps, **kwargs})
-
-class _closest_s2(OpenSCADObject):
-    def __init__(self, s=None, eps=None, **kwargs):
-       super().__init__("_closest_s2", {"s" : s, "eps" : eps, **kwargs})
-
-class _closest_s3(OpenSCADObject):
-    def __init__(self, s=None, eps=None, **kwargs):
-       super().__init__("_closest_s3", {"s" : s, "eps" : eps, **kwargs})
-
-class _tri_normal(OpenSCADObject):
-    def __init__(self, tri=None, **kwargs):
-       super().__init__("_tri_normal", {"tri" : tri, **kwargs})
-
-class _support_diff(OpenSCADObject):
-    def __init__(self, p1=None, p2=None, d=None, **kwargs):
-       super().__init__("_support_diff", {"p1" : p1, "p2" : p2, "d" : d, **kwargs})
-
-class rot_decode(OpenSCADObject):
-    def __init__(self, M=None, long=None, **kwargs):
-       super().__init__("rot_decode", {"M" : M, "long" : long, **kwargs})
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
+
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/threading.scad'}", use_not_include=False)
+
+class threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, d1=None, d2=None, higbee=None, higbee1=None, higbee2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "d1" : d1, "d2" : d2, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, starts=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, id1=None, id2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "starts" : starts, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "id1" : id1, "id2" : id2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class trapezoidal_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, thread_angle=None, thread_depth=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, higbee=None, higbee1=None, higbee2=None, d1=None, d2=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("trapezoidal_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "thread_angle" : thread_angle, "thread_depth" : thread_depth, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "d1" : d1, "d2" : d2, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class trapezoidal_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, thread_angle=None, thread_depth=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, higbee=None, higbee1=None, higbee2=None, d1=None, d2=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("trapezoidal_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "thread_angle" : thread_angle, "thread_depth" : thread_depth, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "d1" : d1, "d2" : d2, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class acme_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, tpi=None, pitch=None, starts=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, internal=None, higbee=None, higbee1=None, higbee2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("acme_threaded_rod", {"d" : d, "l" : l, "tpi" : tpi, "pitch" : pitch, "starts" : starts, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class acme_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, tpi=None, pitch=None, starts=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("acme_threaded_nut", {"od" : od, "id" : id, "h" : h, "tpi" : tpi, "pitch" : pitch, "starts" : starts, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class npt_threaded_rod(_Bosl2Base):
+    def __init__(self, size=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, hollow=None, internal=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("npt_threaded_rod", {"size" : size, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "hollow" : hollow, "internal" : internal, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class buttress_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, internal=None, higbee=None, higbee1=None, higbee2=None, d1=None, d2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("buttress_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "d1" : d1, "d2" : d2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class buttress_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("buttress_threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class square_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, higbee=None, higbee1=None, higbee2=None, d1=None, d2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("square_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "d1" : d1, "d2" : d2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class square_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("square_threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class ball_screw_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, ball_diam=None, ball_arc=None, starts=None, left_handed=None, internal=None, bevel=None, bevel1=None, bevel2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("ball_screw_rod", {"d" : d, "l" : l, "pitch" : pitch, "ball_diam" : ball_diam, "ball_arc" : ball_arc, "starts" : starts, "left_handed" : left_handed, "internal" : internal, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class generic_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, profile=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, d1=None, d2=None, higbee=None, higbee1=None, higbee2=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("generic_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "profile" : profile, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "d1" : d1, "d2" : d2, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class generic_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, profile=None, left_handed=None, starts=None, bevel=None, bevel1=None, bevel2=None, id1=None, id2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("generic_threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "profile" : profile, "left_handed" : left_handed, "starts" : starts, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "id1" : id1, "id2" : id2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class thread_helix(_Bosl2Base):
+    def __init__(self, d=None, pitch=None, thread_depth=None, flank_angle=None, turns=None, profile=None, starts=None, left_handed=None, internal=None, d1=None, d2=None, higbee=None, higbee1=None, higbee2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("thread_helix", {"d" : d, "pitch" : pitch, "thread_depth" : thread_depth, "flank_angle" : flank_angle, "turns" : turns, "profile" : profile, "starts" : starts, "left_handed" : left_handed, "internal" : internal, "d1" : d1, "d2" : d2, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, d1=None, d2=None, higbee=None, higbee1=None, higbee2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "d1" : d1, "d2" : d2, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, starts=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, id1=None, id2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "starts" : starts, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "id1" : id1, "id2" : id2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class trapezoidal_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, thread_angle=None, thread_depth=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, higbee=None, higbee1=None, higbee2=None, d1=None, d2=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("trapezoidal_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "thread_angle" : thread_angle, "thread_depth" : thread_depth, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "d1" : d1, "d2" : d2, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class trapezoidal_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, thread_angle=None, thread_depth=None, left_handed=None, starts=None, bevel=None, bevel1=None, bevel2=None, id1=None, id2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("trapezoidal_threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "thread_angle" : thread_angle, "thread_depth" : thread_depth, "left_handed" : left_handed, "starts" : starts, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "id1" : id1, "id2" : id2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class acme_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, tpi=None, pitch=None, starts=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, internal=None, higbee=None, higbee1=None, higbee2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("acme_threaded_rod", {"d" : d, "l" : l, "tpi" : tpi, "pitch" : pitch, "starts" : starts, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class acme_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, tpi=None, pitch=None, starts=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("acme_threaded_nut", {"od" : od, "id" : id, "h" : h, "tpi" : tpi, "pitch" : pitch, "starts" : starts, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class npt_threaded_rod(_Bosl2Base):
+    def __init__(self, size=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, hollow=None, internal=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("npt_threaded_rod", {"size" : size, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "hollow" : hollow, "internal" : internal, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class buttress_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, internal=None, higbee=None, higbee1=None, higbee2=None, d1=None, d2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("buttress_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "d1" : d1, "d2" : d2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class buttress_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("buttress_threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class square_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, higbee=None, higbee1=None, higbee2=None, d1=None, d2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("square_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "d1" : d1, "d2" : d2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class square_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("square_threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class ball_screw_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, ball_diam=None, ball_arc=None, starts=None, left_handed=None, internal=None, bevel=None, bevel1=None, bevel2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("ball_screw_rod", {"d" : d, "l" : l, "pitch" : pitch, "ball_diam" : ball_diam, "ball_arc" : ball_arc, "starts" : starts, "left_handed" : left_handed, "internal" : internal, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class generic_threaded_rod(_Bosl2Base):
+    def __init__(self, d=None, l=None, pitch=None, profile=None, left_handed=None, bevel=None, bevel1=None, bevel2=None, starts=None, internal=None, d1=None, d2=None, higbee=None, higbee1=None, higbee2=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("generic_threaded_rod", {"d" : d, "l" : l, "pitch" : pitch, "profile" : profile, "left_handed" : left_handed, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "starts" : starts, "internal" : internal, "d1" : d1, "d2" : d2, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class generic_threaded_nut(_Bosl2Base):
+    def __init__(self, od=None, id=None, h=None, pitch=None, profile=None, left_handed=None, starts=None, bevel=None, bevel1=None, bevel2=None, id1=None, id2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("generic_threaded_nut", {"od" : od, "id" : id, "h" : h, "pitch" : pitch, "profile" : profile, "left_handed" : left_handed, "starts" : starts, "bevel" : bevel, "bevel1" : bevel1, "bevel2" : bevel2, "id1" : id1, "id2" : id2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class thread_helix(_Bosl2Base):
+    def __init__(self, d=None, pitch=None, thread_depth=None, flank_angle=None, turns=None, profile=None, starts=None, left_handed=None, internal=None, d1=None, d2=None, higbee=None, higbee1=None, higbee2=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("thread_helix", {"d" : d, "pitch" : pitch, "thread_depth" : thread_depth, "flank_angle" : flank_angle, "turns" : turns, "profile" : profile, "starts" : starts, "left_handed" : left_handed, "internal" : internal, "d1" : d1, "d2" : d2, "higbee" : higbee, "higbee1" : higbee1, "higbee2" : higbee2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/hingesnaps.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/hingesnaps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/hingesnaps.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class apply_folding_hinges_and_snaps(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/hingesnaps.scad'}", use_not_include=False)
+
+class apply_folding_hinges_and_snaps(_Bosl2Base):
     def __init__(self, thick=None, foldangle=None, hinges=None, snaps=None, sockets=None, snaplen=None, snapdiam=None, hingegap=None, layerheight=None, **kwargs):
        super().__init__("apply_folding_hinges_and_snaps", {"thick" : thick, "foldangle" : foldangle, "hinges" : hinges, "snaps" : snaps, "sockets" : sockets, "snaplen" : snaplen, "snapdiam" : snapdiam, "hingegap" : hingegap, "layerheight" : layerheight, **kwargs})
 
-class folding_hinge_mask(OpenSCADObject):
+class folding_hinge_mask(_Bosl2Base):
     def __init__(self, l=None, thick=None, layerheight=None, foldangle=None, hingegap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("folding_hinge_mask", {"l" : l, "thick" : thick, "layerheight" : layerheight, "foldangle" : foldangle, "hingegap" : hingegap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class snap_lock(OpenSCADObject):
+class snap_lock(_Bosl2Base):
     def __init__(self, thick=None, snaplen=None, snapdiam=None, layerheight=None, foldangle=None, hingegap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("snap_lock", {"thick" : thick, "snaplen" : snaplen, "snapdiam" : snapdiam, "layerheight" : layerheight, "foldangle" : foldangle, "hingegap" : hingegap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class snap_socket(OpenSCADObject):
+class snap_socket(_Bosl2Base):
     def __init__(self, thick=None, snaplen=None, snapdiam=None, layerheight=None, foldangle=None, hingegap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("snap_socket", {"thick" : thick, "snaplen" : snaplen, "snapdiam" : snapdiam, "layerheight" : layerheight, "foldangle" : foldangle, "hingegap" : hingegap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/joiners.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/joiners.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,96 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/joiners.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class half_joiner_clear(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/joiners.scad'}", use_not_include=False)
+
+class half_joiner_clear(_Bosl2Base):
     def __init__(self, l=None, w=None, ang=None, clearance=None, overlap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("half_joiner_clear", {"l" : l, "w" : w, "ang" : ang, "clearance" : clearance, "overlap" : overlap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class half_joiner(OpenSCADObject):
+class half_joiner(_Bosl2Base):
     def __init__(self, l=None, w=None, base=None, ang=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("half_joiner", {"l" : l, "w" : w, "base" : base, "ang" : ang, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class half_joiner2(OpenSCADObject):
+class half_joiner2(_Bosl2Base):
     def __init__(self, l=None, w=None, base=None, ang=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("half_joiner2", {"l" : l, "w" : w, "base" : base, "ang" : ang, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class joiner_clear(OpenSCADObject):
+class joiner_clear(_Bosl2Base):
     def __init__(self, l=None, w=None, ang=None, clearance=None, overlap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("joiner_clear", {"l" : l, "w" : w, "ang" : ang, "clearance" : clearance, "overlap" : overlap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class joiner(OpenSCADObject):
+class joiner(_Bosl2Base):
     def __init__(self, l=None, w=None, base=None, ang=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("joiner", {"l" : l, "w" : w, "base" : base, "ang" : ang, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class dovetail(OpenSCADObject):
+class dovetail(_Bosl2Base):
     def __init__(self, gender=None, width=None, height=None, slide=None, h=None, w=None, angle=None, slope=None, taper=None, back_width=None, chamfer=None, extra=None, r=None, radius=None, round=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("dovetail", {"gender" : gender, "width" : width, "height" : height, "slide" : slide, "h" : h, "w" : w, "angle" : angle, "slope" : slope, "taper" : taper, "back_width" : back_width, "chamfer" : chamfer, "extra" : extra, "r" : r, "radius" : radius, "round" : round, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class _pin_nub(OpenSCADObject):
-    def __init__(self, r=None, nub=None, h=None, **kwargs):
-       super().__init__("_pin_nub", {"r" : r, "nub" : nub, "h" : h, **kwargs})
-
-class _pin_slot(OpenSCADObject):
-    def __init__(self, l=None, r=None, t=None, d=None, nub=None, depth=None, stretch=None, **kwargs):
-       super().__init__("_pin_slot", {"l" : l, "r" : r, "t" : t, "d" : d, "nub" : nub, "depth" : depth, "stretch" : stretch, **kwargs})
-
-class _pin_shaft(OpenSCADObject):
-    def __init__(self, r=None, lStraight=None, nub=None, nubscale=None, stretch=None, d=None, pointed=None, **kwargs):
-       super().__init__("_pin_shaft", {"r" : r, "lStraight" : lStraight, "nub" : nub, "nubscale" : nubscale, "stretch" : stretch, "d" : d, "pointed" : pointed, **kwargs})
+class _pin_size(_Bosl2Base):
+    def __init__(self, size=None, **kwargs):
+       super().__init__("_pin_size", {"size" : size, **kwargs})
 
-class snap_pin(OpenSCADObject):
+class snap_pin(_Bosl2Base):
     def __init__(self, size=None, r=None, radius=None, d=None, diameter=None, l=None, length=None, nub_depth=None, snap=None, thickness=None, clearance=None, preload=None, pointed=None, anchor=None, spin=None, orient=None, center=None, **kwargs):
        super().__init__("snap_pin", {"size" : size, "r" : r, "radius" : radius, "d" : d, "diameter" : diameter, "l" : l, "length" : length, "nub_depth" : nub_depth, "snap" : snap, "thickness" : thickness, "clearance" : clearance, "preload" : preload, "pointed" : pointed, "anchor" : anchor, "spin" : spin, "orient" : orient, "center" : center, **kwargs})
 
-class snap_pin_socket(OpenSCADObject):
+class snap_pin_socket(_Bosl2Base):
     def __init__(self, size=None, r=None, radius=None, l=None, length=None, d=None, diameter=None, nub_depth=None, snap=None, fixed=None, pointed=None, fins=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("snap_pin_socket", {"size" : size, "r" : r, "radius" : radius, "l" : l, "length" : length, "d" : d, "diameter" : diameter, "nub_depth" : nub_depth, "snap" : snap, "fixed" : fixed, "pointed" : pointed, "fins" : fins, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rabbit_clip(OpenSCADObject):
+class rabbit_clip(_Bosl2Base):
     def __init__(self, type=None, length=None, width=None, snap=None, thickness=None, depth=None, compression=None, clearance=None, lock=None, lock_clearance=None, splinesteps=None, anchor=None, orient=None, spin=None, **kwargs):
        super().__init__("rabbit_clip", {"type" : type, "length" : length, "width" : width, "snap" : snap, "thickness" : thickness, "depth" : depth, "compression" : compression, "clearance" : clearance, "lock" : lock, "lock_clearance" : lock_clearance, "splinesteps" : splinesteps, "anchor" : anchor, "orient" : orient, "spin" : spin, **kwargs})
 
-class half_joiner_clear(OpenSCADObject):
+class half_joiner_clear(_Bosl2Base):
     def __init__(self, l=None, w=None, ang=None, clearance=None, overlap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("half_joiner_clear", {"l" : l, "w" : w, "ang" : ang, "clearance" : clearance, "overlap" : overlap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class half_joiner(OpenSCADObject):
+class half_joiner(_Bosl2Base):
     def __init__(self, l=None, w=None, base=None, ang=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("half_joiner", {"l" : l, "w" : w, "base" : base, "ang" : ang, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class half_joiner2(OpenSCADObject):
+class half_joiner2(_Bosl2Base):
     def __init__(self, l=None, w=None, base=None, ang=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("half_joiner2", {"l" : l, "w" : w, "base" : base, "ang" : ang, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class joiner_clear(OpenSCADObject):
+class joiner_clear(_Bosl2Base):
     def __init__(self, l=None, w=None, ang=None, clearance=None, overlap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("joiner_clear", {"l" : l, "w" : w, "ang" : ang, "clearance" : clearance, "overlap" : overlap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class joiner(OpenSCADObject):
+class joiner(_Bosl2Base):
     def __init__(self, l=None, w=None, base=None, ang=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("joiner", {"l" : l, "w" : w, "base" : base, "ang" : ang, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class dovetail(OpenSCADObject):
+class dovetail(_Bosl2Base):
     def __init__(self, gender=None, width=None, height=None, slide=None, h=None, w=None, angle=None, slope=None, taper=None, back_width=None, chamfer=None, extra=None, r=None, radius=None, round=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("dovetail", {"gender" : gender, "width" : width, "height" : height, "slide" : slide, "h" : h, "w" : w, "angle" : angle, "slope" : slope, "taper" : taper, "back_width" : back_width, "chamfer" : chamfer, "extra" : extra, "r" : r, "radius" : radius, "round" : round, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class _pin_size(OpenSCADObject):
-    def __init__(self, size=None, **kwargs):
-       super().__init__("_pin_size", {"size" : size, **kwargs})
+class _pin_nub(_Bosl2Base):
+    def __init__(self, r=None, nub=None, h=None, **kwargs):
+       super().__init__("_pin_nub", {"r" : r, "nub" : nub, "h" : h, **kwargs})
+
+class _pin_slot(_Bosl2Base):
+    def __init__(self, l=None, r=None, t=None, d=None, nub=None, depth=None, stretch=None, **kwargs):
+       super().__init__("_pin_slot", {"l" : l, "r" : r, "t" : t, "d" : d, "nub" : nub, "depth" : depth, "stretch" : stretch, **kwargs})
+
+class _pin_shaft(_Bosl2Base):
+    def __init__(self, r=None, lStraight=None, nub=None, nubscale=None, stretch=None, d=None, pointed=None, **kwargs):
+       super().__init__("_pin_shaft", {"r" : r, "lStraight" : lStraight, "nub" : nub, "nubscale" : nubscale, "stretch" : stretch, "d" : d, "pointed" : pointed, **kwargs})
 
-class snap_pin(OpenSCADObject):
+class snap_pin(_Bosl2Base):
     def __init__(self, size=None, r=None, radius=None, d=None, diameter=None, l=None, length=None, nub_depth=None, snap=None, thickness=None, clearance=None, preload=None, pointed=None, anchor=None, spin=None, orient=None, center=None, **kwargs):
        super().__init__("snap_pin", {"size" : size, "r" : r, "radius" : radius, "d" : d, "diameter" : diameter, "l" : l, "length" : length, "nub_depth" : nub_depth, "snap" : snap, "thickness" : thickness, "clearance" : clearance, "preload" : preload, "pointed" : pointed, "anchor" : anchor, "spin" : spin, "orient" : orient, "center" : center, **kwargs})
 
-class snap_pin_socket(OpenSCADObject):
+class snap_pin_socket(_Bosl2Base):
     def __init__(self, size=None, r=None, radius=None, l=None, length=None, d=None, diameter=None, nub_depth=None, snap=None, fixed=None, pointed=None, fins=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("snap_pin_socket", {"size" : size, "r" : r, "radius" : radius, "l" : l, "length" : length, "d" : d, "diameter" : diameter, "nub_depth" : nub_depth, "snap" : snap, "fixed" : fixed, "pointed" : pointed, "fins" : fins, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rabbit_clip(OpenSCADObject):
+class rabbit_clip(_Bosl2Base):
     def __init__(self, type=None, length=None, width=None, snap=None, thickness=None, depth=None, compression=None, clearance=None, lock=None, lock_clearance=None, splinesteps=None, anchor=None, orient=None, spin=None, **kwargs):
        super().__init__("rabbit_clip", {"type" : type, "length" : length, "width" : width, "snap" : snap, "thickness" : thickness, "depth" : depth, "compression" : compression, "clearance" : clearance, "lock" : lock, "lock_clearance" : lock_clearance, "splinesteps" : splinesteps, "anchor" : anchor, "orient" : orient, "spin" : spin, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/linalg.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/linalg.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,134 +1,136 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/linalg.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class echo_matrix(OpenSCADObject):
-    def __init__(self, M=None, description=None, sig=None, sep=None, eps=None, **kwargs):
-       super().__init__("echo_matrix", {"M" : M, "description" : description, "sig" : sig, "sep" : sep, "eps" : eps, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/linalg.scad'}", use_not_include=False)
 
-class is_matrix(OpenSCADObject):
+class is_matrix(_Bosl2Base):
     def __init__(self, A=None, m=None, n=None, square=None, **kwargs):
        super().__init__("is_matrix", {"A" : A, "m" : m, "n" : n, "square" : square, **kwargs})
 
-class is_matrix_symmetric(OpenSCADObject):
+class is_matrix_symmetric(_Bosl2Base):
     def __init__(self, A=None, eps=None, **kwargs):
        super().__init__("is_matrix_symmetric", {"A" : A, "eps" : eps, **kwargs})
 
-class is_rotation(OpenSCADObject):
+class is_rotation(_Bosl2Base):
     def __init__(self, A=None, dim=None, centered=None, **kwargs):
        super().__init__("is_rotation", {"A" : A, "dim" : dim, "centered" : centered, **kwargs})
 
-class echo_matrix(OpenSCADObject):
+class echo_matrix(_Bosl2Base):
     def __init__(self, M=None, description=None, sig=None, sep=None, eps=None, **kwargs):
        super().__init__("echo_matrix", {"M" : M, "description" : description, "sig" : sig, "sep" : sep, "eps" : eps, **kwargs})
 
-class column(OpenSCADObject):
+class column(_Bosl2Base):
     def __init__(self, M=None, i=None, **kwargs):
        super().__init__("column", {"M" : M, "i" : i, **kwargs})
 
-class submatrix(OpenSCADObject):
+class submatrix(_Bosl2Base):
     def __init__(self, M=None, idx1=None, idx2=None, **kwargs):
        super().__init__("submatrix", {"M" : M, "idx1" : idx1, "idx2" : idx2, **kwargs})
 
-class ident(OpenSCADObject):
+class ident(_Bosl2Base):
     def __init__(self, n=None, **kwargs):
        super().__init__("ident", {"n" : n, **kwargs})
 
-class diagonal_matrix(OpenSCADObject):
+class diagonal_matrix(_Bosl2Base):
     def __init__(self, diag=None, offdiag=None, **kwargs):
        super().__init__("diagonal_matrix", {"diag" : diag, "offdiag" : offdiag, **kwargs})
 
-class transpose(OpenSCADObject):
+class transpose(_Bosl2Base):
     def __init__(self, M=None, reverse=None, **kwargs):
        super().__init__("transpose", {"M" : M, "reverse" : reverse, **kwargs})
 
-class outer_product(OpenSCADObject):
+class outer_product(_Bosl2Base):
     def __init__(self, u=None, v=None, **kwargs):
        super().__init__("outer_product", {"u" : u, "v" : v, **kwargs})
 
-class submatrix_set(OpenSCADObject):
+class submatrix_set(_Bosl2Base):
     def __init__(self, M=None, A=None, m=None, n=None, **kwargs):
        super().__init__("submatrix_set", {"M" : M, "A" : A, "m" : m, "n" : n, **kwargs})
 
-class hstack(OpenSCADObject):
+class hstack(_Bosl2Base):
     def __init__(self, M1=None, M2=None, M3=None, **kwargs):
        super().__init__("hstack", {"M1" : M1, "M2" : M2, "M3" : M3, **kwargs})
 
-class block_matrix(OpenSCADObject):
+class block_matrix(_Bosl2Base):
     def __init__(self, M=None, **kwargs):
        super().__init__("block_matrix", {"M" : M, **kwargs})
 
-class linear_solve(OpenSCADObject):
+class linear_solve(_Bosl2Base):
     def __init__(self, A=None, b=None, pivot=None, **kwargs):
        super().__init__("linear_solve", {"A" : A, "b" : b, "pivot" : pivot, **kwargs})
 
-class linear_solve3(OpenSCADObject):
+class linear_solve3(_Bosl2Base):
     def __init__(self, A=None, b=None, **kwargs):
        super().__init__("linear_solve3", {"A" : A, "b" : b, **kwargs})
 
-class matrix_inverse(OpenSCADObject):
+class matrix_inverse(_Bosl2Base):
     def __init__(self, A=None, **kwargs):
        super().__init__("matrix_inverse", {"A" : A, **kwargs})
 
-class rot_inverse(OpenSCADObject):
+class rot_inverse(_Bosl2Base):
     def __init__(self, T=None, **kwargs):
        super().__init__("rot_inverse", {"T" : T, **kwargs})
 
-class null_space(OpenSCADObject):
+class null_space(_Bosl2Base):
     def __init__(self, A=None, eps=None, **kwargs):
        super().__init__("null_space", {"A" : A, "eps" : eps, **kwargs})
 
-class qr_factor(OpenSCADObject):
+class qr_factor(_Bosl2Base):
     def __init__(self, A=None, pivot=None, **kwargs):
        super().__init__("qr_factor", {"A" : A, "pivot" : pivot, **kwargs})
 
-class _qr_factor(OpenSCADObject):
+class _qr_factor(_Bosl2Base):
     def __init__(self, A=None, Q=None, P=None, pivot=None, col=None, m=None, n=None, **kwargs):
        super().__init__("_qr_factor", {"A" : A, "Q" : Q, "P" : P, "pivot" : pivot, "col" : col, "m" : m, "n" : n, **kwargs})
 
-class _swap_matrix(OpenSCADObject):
+class _swap_matrix(_Bosl2Base):
     def __init__(self, n=None, i=None, j=None, **kwargs):
        super().__init__("_swap_matrix", {"n" : n, "i" : i, "j" : j, **kwargs})
 
-class back_substitute(OpenSCADObject):
+class back_substitute(_Bosl2Base):
     def __init__(self, R=None, b=None, transpose=None, **kwargs):
        super().__init__("back_substitute", {"R" : R, "b" : b, "transpose" : transpose, **kwargs})
 
-class _back_substitute(OpenSCADObject):
+class _back_substitute(_Bosl2Base):
     def __init__(self, R=None, b=None, x=None, **kwargs):
        super().__init__("_back_substitute", {"R" : R, "b" : b, "x" : x, **kwargs})
 
-class cholesky(OpenSCADObject):
+class cholesky(_Bosl2Base):
     def __init__(self, A=None, **kwargs):
        super().__init__("cholesky", {"A" : A, **kwargs})
 
-class _cholesky(OpenSCADObject):
+class _cholesky(_Bosl2Base):
     def __init__(self, A=None, L=None, n=None, **kwargs):
        super().__init__("_cholesky", {"A" : A, "L" : L, "n" : n, **kwargs})
 
-class det2(OpenSCADObject):
+class det2(_Bosl2Base):
     def __init__(self, M=None, **kwargs):
        super().__init__("det2", {"M" : M, **kwargs})
 
-class det3(OpenSCADObject):
+class det3(_Bosl2Base):
     def __init__(self, M=None, **kwargs):
        super().__init__("det3", {"M" : M, **kwargs})
 
-class det4(OpenSCADObject):
+class det4(_Bosl2Base):
     def __init__(self, M=None, **kwargs):
        super().__init__("det4", {"M" : M, **kwargs})
 
-class determinant(OpenSCADObject):
+class determinant(_Bosl2Base):
     def __init__(self, M=None, **kwargs):
        super().__init__("determinant", {"M" : M, **kwargs})
 
-class norm_fro(OpenSCADObject):
+class norm_fro(_Bosl2Base):
     def __init__(self, A=None, **kwargs):
        super().__init__("norm_fro", {"A" : A, **kwargs})
 
-class matrix_trace(OpenSCADObject):
+class matrix_trace(_Bosl2Base):
     def __init__(self, M=None, **kwargs):
        super().__init__("matrix_trace", {"M" : M, **kwargs})
 
+class echo_matrix(_Bosl2Base):
+    def __init__(self, M=None, description=None, sig=None, sep=None, eps=None, **kwargs):
+       super().__init__("echo_matrix", {"M" : M, "description" : description, "sig" : sig, "sep" : sep, "eps" : eps, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/linear_bearings.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/linear_bearings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/linear_bearings.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class linear_bearing_housing(OpenSCADObject):
-    def __init__(self, d=None, l=None, tab=None, gap=None, wall=None, tabwall=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("linear_bearing_housing", {"d" : d, "l" : l, "tab" : tab, "gap" : gap, "wall" : wall, "tabwall" : tabwall, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class lmXuu_housing(OpenSCADObject):
-    def __init__(self, size=None, tab=None, gap=None, wall=None, tabwall=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("lmXuu_housing", {"size" : size, "tab" : tab, "gap" : gap, "wall" : wall, "tabwall" : tabwall, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/linear_bearings.scad'}", use_not_include=False)
 
-class get_lmXuu_bearing_diam(OpenSCADObject):
+class get_lmXuu_bearing_diam(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_lmXuu_bearing_diam", {"size" : size, **kwargs})
 
-class get_lmXuu_bearing_length(OpenSCADObject):
+class get_lmXuu_bearing_length(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_lmXuu_bearing_length", {"size" : size, **kwargs})
 
+class linear_bearing_housing(_Bosl2Base):
+    def __init__(self, d=None, l=None, tab=None, gap=None, wall=None, tabwall=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("linear_bearing_housing", {"d" : d, "l" : l, "tab" : tab, "gap" : gap, "wall" : wall, "tabwall" : tabwall, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class lmXuu_housing(_Bosl2Base):
+    def __init__(self, size=None, tab=None, gap=None, wall=None, tabwall=None, screwsize=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("lmXuu_housing", {"size" : size, "tab" : tab, "gap" : gap, "wall" : wall, "tabwall" : tabwall, "screwsize" : screwsize, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/lists.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/lists.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,162 +1,164 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/lists.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class is_homogeneous(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/lists.scad'}", use_not_include=False)
+
+class is_homogeneous(_Bosl2Base):
     def __init__(self, l=None, depth=None, **kwargs):
        super().__init__("is_homogeneous", {"l" : l, "depth" : depth, **kwargs})
 
-class is_homogenous(OpenSCADObject):
+class is_homogenous(_Bosl2Base):
     def __init__(self, l=None, depth=None, **kwargs):
        super().__init__("is_homogenous", {"l" : l, "depth" : depth, **kwargs})
 
-class _same_type(OpenSCADObject):
+class _same_type(_Bosl2Base):
     def __init__(self, a=None, b=None, depth=None, **kwargs):
        super().__init__("_same_type", {"a" : a, "b" : b, "depth" : depth, **kwargs})
 
-class min_length(OpenSCADObject):
+class min_length(_Bosl2Base):
     def __init__(self, list=None, **kwargs):
        super().__init__("min_length", {"list" : list, **kwargs})
 
-class max_length(OpenSCADObject):
+class max_length(_Bosl2Base):
     def __init__(self, list=None, **kwargs):
        super().__init__("max_length", {"list" : list, **kwargs})
 
-class _list_shape_recurse(OpenSCADObject):
+class _list_shape_recurse(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("_list_shape_recurse", {"v" : v, **kwargs})
 
-class _list_shape_recurse(OpenSCADObject):
+class _list_shape_recurse(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("_list_shape_recurse", {"v" : v, **kwargs})
 
-class list_shape(OpenSCADObject):
+class list_shape(_Bosl2Base):
     def __init__(self, v=None, depth=None, **kwargs):
        super().__init__("list_shape", {"v" : v, "depth" : depth, **kwargs})
 
-class in_list(OpenSCADObject):
+class in_list(_Bosl2Base):
     def __init__(self, val=None, list=None, idx=None, **kwargs):
        super().__init__("in_list", {"val" : val, "list" : list, "idx" : idx, **kwargs})
 
-class select(OpenSCADObject):
+class select(_Bosl2Base):
     def __init__(self, list=None, start=None, end=None, **kwargs):
        super().__init__("select", {"list" : list, "start" : start, "end" : end, **kwargs})
 
-class slice(OpenSCADObject):
+class slice(_Bosl2Base):
     def __init__(self, list=None, start=None, end=None, **kwargs):
        super().__init__("slice", {"list" : list, "start" : start, "end" : end, **kwargs})
 
-class last(OpenSCADObject):
+class last(_Bosl2Base):
     def __init__(self, list=None, **kwargs):
        super().__init__("last", {"list" : list, **kwargs})
 
-class list_head(OpenSCADObject):
+class list_head(_Bosl2Base):
     def __init__(self, list=None, to=None, **kwargs):
        super().__init__("list_head", {"list" : list, "to" : to, **kwargs})
 
-class list_tail(OpenSCADObject):
+class list_tail(_Bosl2Base):
     def __init__(self, list=None, _from=None, **kwargs):
        super().__init__("list_tail", {"list" : list, "_from" : _from, **kwargs})
 
-class bselect(OpenSCADObject):
+class bselect(_Bosl2Base):
     def __init__(self, list=None, index=None, **kwargs):
        super().__init__("bselect", {"list" : list, "index" : index, **kwargs})
 
-class repeat(OpenSCADObject):
+class repeat(_Bosl2Base):
     def __init__(self, val=None, n=None, i=None, **kwargs):
        super().__init__("repeat", {"val" : val, "n" : n, "i" : i, **kwargs})
 
-class list_bset(OpenSCADObject):
+class list_bset(_Bosl2Base):
     def __init__(self, indexset=None, valuelist=None, dflt=None, **kwargs):
        super().__init__("list_bset", {"indexset" : indexset, "valuelist" : valuelist, "dflt" : dflt, **kwargs})
 
-class list(OpenSCADObject):
+class list(_Bosl2Base):
     def __init__(self, l=None, **kwargs):
        super().__init__("list", {"l" : l, **kwargs})
 
-class force_list(OpenSCADObject):
+class force_list(_Bosl2Base):
     def __init__(self, value=None, n=None, fill=None, **kwargs):
        super().__init__("force_list", {"value" : value, "n" : n, "fill" : fill, **kwargs})
 
-class reverse(OpenSCADObject):
+class reverse(_Bosl2Base):
     def __init__(self, list=None, **kwargs):
        super().__init__("reverse", {"list" : list, **kwargs})
 
-class list_rotate(OpenSCADObject):
+class list_rotate(_Bosl2Base):
     def __init__(self, list=None, n=None, **kwargs):
        super().__init__("list_rotate", {"list" : list, "n" : n, **kwargs})
 
-class shuffle(OpenSCADObject):
+class shuffle(_Bosl2Base):
     def __init__(self, list=None, seed=None, **kwargs):
        super().__init__("shuffle", {"list" : list, "seed" : seed, **kwargs})
 
-class repeat_entries(OpenSCADObject):
+class repeat_entries(_Bosl2Base):
     def __init__(self, list=None, N=None, exact=None, **kwargs):
        super().__init__("repeat_entries", {"list" : list, "N" : N, "exact" : exact, **kwargs})
 
-class list_pad(OpenSCADObject):
+class list_pad(_Bosl2Base):
     def __init__(self, list=None, minlen=None, fill=None, **kwargs):
        super().__init__("list_pad", {"list" : list, "minlen" : minlen, "fill" : fill, **kwargs})
 
-class list_set(OpenSCADObject):
+class list_set(_Bosl2Base):
     def __init__(self, list=None, indices=None, values=None, dflt=None, minlen=None, **kwargs):
        super().__init__("list_set", {"list" : list, "indices" : indices, "values" : values, "dflt" : dflt, "minlen" : minlen, **kwargs})
 
-class list_insert(OpenSCADObject):
+class list_insert(_Bosl2Base):
     def __init__(self, list=None, indices=None, values=None, **kwargs):
        super().__init__("list_insert", {"list" : list, "indices" : indices, "values" : values, **kwargs})
 
-class list_remove(OpenSCADObject):
+class list_remove(_Bosl2Base):
     def __init__(self, list=None, ind=None, **kwargs):
        super().__init__("list_remove", {"list" : list, "ind" : ind, **kwargs})
 
-class list_remove_values(OpenSCADObject):
+class list_remove_values(_Bosl2Base):
     def __init__(self, list=None, values=None, all=None, **kwargs):
        super().__init__("list_remove_values", {"list" : list, "values" : values, "all" : all, **kwargs})
 
-class idx(OpenSCADObject):
+class idx(_Bosl2Base):
     def __init__(self, list=None, s=None, e=None, step=None, **kwargs):
        super().__init__("idx", {"list" : list, "s" : s, "e" : e, "step" : step, **kwargs})
 
-class pair(OpenSCADObject):
+class pair(_Bosl2Base):
     def __init__(self, list=None, wrap=None, **kwargs):
        super().__init__("pair", {"list" : list, "wrap" : wrap, **kwargs})
 
-class triplet(OpenSCADObject):
+class triplet(_Bosl2Base):
     def __init__(self, list=None, wrap=None, **kwargs):
        super().__init__("triplet", {"list" : list, "wrap" : wrap, **kwargs})
 
-class combinations(OpenSCADObject):
+class combinations(_Bosl2Base):
     def __init__(self, l=None, n=None, _s=None, **kwargs):
        super().__init__("combinations", {"l" : l, "n" : n, "_s" : _s, **kwargs})
 
-class permutations(OpenSCADObject):
+class permutations(_Bosl2Base):
     def __init__(self, l=None, n=None, **kwargs):
        super().__init__("permutations", {"l" : l, "n" : n, **kwargs})
 
-class list_to_matrix(OpenSCADObject):
+class list_to_matrix(_Bosl2Base):
     def __init__(self, v=None, cnt=None, dflt=None, **kwargs):
        super().__init__("list_to_matrix", {"v" : v, "cnt" : cnt, "dflt" : dflt, **kwargs})
 
-class flatten(OpenSCADObject):
+class flatten(_Bosl2Base):
     def __init__(self, l=None, **kwargs):
        super().__init__("flatten", {"l" : l, **kwargs})
 
-class full_flatten(OpenSCADObject):
+class full_flatten(_Bosl2Base):
     def __init__(self, l=None, **kwargs):
        super().__init__("full_flatten", {"l" : l, **kwargs})
 
-class set_union(OpenSCADObject):
+class set_union(_Bosl2Base):
     def __init__(self, a=None, b=None, get_indices=None, **kwargs):
        super().__init__("set_union", {"a" : a, "b" : b, "get_indices" : get_indices, **kwargs})
 
-class set_difference(OpenSCADObject):
+class set_difference(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("set_difference", {"a" : a, "b" : b, **kwargs})
 
-class set_intersection(OpenSCADObject):
+class set_intersection(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("set_intersection", {"a" : a, "b" : b, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/masks2d.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/masks2d.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/masks2d.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class mask2d_roundover(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/masks2d.scad'}", use_not_include=False)
+
+class mask2d_roundover(_Bosl2Base):
     def __init__(self, r=None, inset=None, excess=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_roundover", {"r" : r, "inset" : inset, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_cove(OpenSCADObject):
+class mask2d_cove(_Bosl2Base):
     def __init__(self, r=None, inset=None, excess=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_cove", {"r" : r, "inset" : inset, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_chamfer(OpenSCADObject):
+class mask2d_chamfer(_Bosl2Base):
     def __init__(self, edge=None, angle=None, inset=None, excess=None, x=None, y=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_chamfer", {"edge" : edge, "angle" : angle, "inset" : inset, "excess" : excess, "x" : x, "y" : y, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_rabbet(OpenSCADObject):
+class mask2d_rabbet(_Bosl2Base):
     def __init__(self, size=None, excess=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_rabbet", {"size" : size, "excess" : excess, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_dovetail(OpenSCADObject):
+class mask2d_dovetail(_Bosl2Base):
     def __init__(self, edge=None, angle=None, inset=None, shelf=None, excess=None, x=None, y=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_dovetail", {"edge" : edge, "angle" : angle, "inset" : inset, "shelf" : shelf, "excess" : excess, "x" : x, "y" : y, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_teardrop(OpenSCADObject):
+class mask2d_teardrop(_Bosl2Base):
     def __init__(self, r=None, angle=None, excess=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_teardrop", {"r" : r, "angle" : angle, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_ogee(OpenSCADObject):
+class mask2d_ogee(_Bosl2Base):
     def __init__(self, pattern=None, excess=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_ogee", {"pattern" : pattern, "excess" : excess, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_roundover(OpenSCADObject):
+class mask2d_roundover(_Bosl2Base):
     def __init__(self, r=None, inset=None, excess=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_roundover", {"r" : r, "inset" : inset, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_cove(OpenSCADObject):
+class mask2d_cove(_Bosl2Base):
     def __init__(self, r=None, inset=None, excess=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_cove", {"r" : r, "inset" : inset, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_chamfer(OpenSCADObject):
+class mask2d_chamfer(_Bosl2Base):
     def __init__(self, edge=None, angle=None, inset=None, excess=None, x=None, y=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_chamfer", {"edge" : edge, "angle" : angle, "inset" : inset, "excess" : excess, "x" : x, "y" : y, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_rabbet(OpenSCADObject):
+class mask2d_rabbet(_Bosl2Base):
     def __init__(self, size=None, excess=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_rabbet", {"size" : size, "excess" : excess, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_dovetail(OpenSCADObject):
+class mask2d_dovetail(_Bosl2Base):
     def __init__(self, edge=None, angle=None, inset=None, shelf=None, excess=None, x=None, y=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_dovetail", {"edge" : edge, "angle" : angle, "inset" : inset, "shelf" : shelf, "excess" : excess, "x" : x, "y" : y, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_teardrop(OpenSCADObject):
+class mask2d_teardrop(_Bosl2Base):
     def __init__(self, r=None, angle=None, excess=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_teardrop", {"r" : r, "angle" : angle, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class mask2d_ogee(OpenSCADObject):
+class mask2d_ogee(_Bosl2Base):
     def __init__(self, pattern=None, excess=None, anchor=None, spin=None, **kwargs):
        super().__init__("mask2d_ogee", {"pattern" : pattern, "excess" : excess, "anchor" : anchor, "spin" : spin, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/masks3d.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/masks3d.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,96 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/masks3d.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class chamfer_edge_mask(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/masks3d.scad'}", use_not_include=False)
+
+class chamfer_edge_mask(_Bosl2Base):
     def __init__(self, l=None, chamfer=None, excess=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("chamfer_edge_mask", {"l" : l, "chamfer" : chamfer, "excess" : excess, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class chamfer_corner_mask(OpenSCADObject):
+class chamfer_corner_mask(_Bosl2Base):
     def __init__(self, chamfer=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("chamfer_corner_mask", {"chamfer" : chamfer, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class chamfer_cylinder_mask(OpenSCADObject):
+class chamfer_cylinder_mask(_Bosl2Base):
     def __init__(self, r=None, chamfer=None, d=None, ang=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("chamfer_cylinder_mask", {"r" : r, "chamfer" : chamfer, "d" : d, "ang" : ang, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rounding_edge_mask(OpenSCADObject):
+class rounding_edge_mask(_Bosl2Base):
     def __init__(self, l=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, excess=None, anchor=None, spin=None, orient=None, h=None, **kwargs):
        super().__init__("rounding_edge_mask", {"l" : l, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "excess" : excess, "anchor" : anchor, "spin" : spin, "orient" : orient, "h" : h, **kwargs})
 
-class rounding_corner_mask(OpenSCADObject):
+class rounding_corner_mask(_Bosl2Base):
     def __init__(self, r=None, d=None, style=None, excess=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rounding_corner_mask", {"r" : r, "d" : d, "style" : style, "excess" : excess, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rounding_angled_edge_mask(OpenSCADObject):
+class rounding_angled_edge_mask(_Bosl2Base):
     def __init__(self, h=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rounding_angled_edge_mask", {"h" : h, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "ang" : ang, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rounding_angled_corner_mask(OpenSCADObject):
+class rounding_angled_corner_mask(_Bosl2Base):
     def __init__(self, r=None, ang=None, d=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rounding_angled_corner_mask", {"r" : r, "ang" : ang, "d" : d, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rounding_cylinder_mask(OpenSCADObject):
+class rounding_cylinder_mask(_Bosl2Base):
     def __init__(self, r=None, rounding=None, d=None, **kwargs):
        super().__init__("rounding_cylinder_mask", {"r" : r, "rounding" : rounding, "d" : d, **kwargs})
 
-class rounding_hole_mask(OpenSCADObject):
+class rounding_hole_mask(_Bosl2Base):
     def __init__(self, r=None, rounding=None, excess=None, d=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rounding_hole_mask", {"r" : r, "rounding" : rounding, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class teardrop_edge_mask(OpenSCADObject):
+class teardrop_edge_mask(_Bosl2Base):
     def __init__(self, l=None, r=None, angle=None, excess=None, d=None, **kwargs):
        super().__init__("teardrop_edge_mask", {"l" : l, "r" : r, "angle" : angle, "excess" : excess, "d" : d, **kwargs})
 
-class teardrop_corner_mask(OpenSCADObject):
+class teardrop_corner_mask(_Bosl2Base):
     def __init__(self, r=None, angle=None, excess=None, d=None, **kwargs):
        super().__init__("teardrop_corner_mask", {"r" : r, "angle" : angle, "excess" : excess, "d" : d, **kwargs})
 
-class chamfer_edge_mask(OpenSCADObject):
+class chamfer_edge_mask(_Bosl2Base):
     def __init__(self, l=None, chamfer=None, excess=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("chamfer_edge_mask", {"l" : l, "chamfer" : chamfer, "excess" : excess, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class chamfer_corner_mask(OpenSCADObject):
+class chamfer_corner_mask(_Bosl2Base):
     def __init__(self, chamfer=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("chamfer_corner_mask", {"chamfer" : chamfer, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class chamfer_cylinder_mask(OpenSCADObject):
+class chamfer_cylinder_mask(_Bosl2Base):
     def __init__(self, r=None, chamfer=None, d=None, ang=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("chamfer_cylinder_mask", {"r" : r, "chamfer" : chamfer, "d" : d, "ang" : ang, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rounding_edge_mask(OpenSCADObject):
+class rounding_edge_mask(_Bosl2Base):
     def __init__(self, l=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, excess=None, anchor=None, spin=None, orient=None, h=None, **kwargs):
        super().__init__("rounding_edge_mask", {"l" : l, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "excess" : excess, "anchor" : anchor, "spin" : spin, "orient" : orient, "h" : h, **kwargs})
 
-class rounding_corner_mask(OpenSCADObject):
+class rounding_corner_mask(_Bosl2Base):
     def __init__(self, r=None, d=None, style=None, excess=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rounding_corner_mask", {"r" : r, "d" : d, "style" : style, "excess" : excess, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rounding_angled_edge_mask(OpenSCADObject):
+class rounding_angled_edge_mask(_Bosl2Base):
     def __init__(self, h=None, r=None, r1=None, r2=None, d=None, d1=None, d2=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rounding_angled_edge_mask", {"h" : h, "r" : r, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "ang" : ang, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rounding_angled_corner_mask(OpenSCADObject):
+class rounding_angled_corner_mask(_Bosl2Base):
     def __init__(self, r=None, ang=None, d=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rounding_angled_corner_mask", {"r" : r, "ang" : ang, "d" : d, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rounding_cylinder_mask(OpenSCADObject):
+class rounding_cylinder_mask(_Bosl2Base):
     def __init__(self, r=None, rounding=None, d=None, **kwargs):
        super().__init__("rounding_cylinder_mask", {"r" : r, "rounding" : rounding, "d" : d, **kwargs})
 
-class rounding_hole_mask(OpenSCADObject):
+class rounding_hole_mask(_Bosl2Base):
     def __init__(self, r=None, rounding=None, excess=None, d=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rounding_hole_mask", {"r" : r, "rounding" : rounding, "excess" : excess, "d" : d, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class teardrop_edge_mask(OpenSCADObject):
+class teardrop_edge_mask(_Bosl2Base):
     def __init__(self, l=None, r=None, angle=None, excess=None, d=None, **kwargs):
        super().__init__("teardrop_edge_mask", {"l" : l, "r" : r, "angle" : angle, "excess" : excess, "d" : d, **kwargs})
 
-class teardrop_corner_mask(OpenSCADObject):
+class teardrop_corner_mask(_Bosl2Base):
     def __init__(self, r=None, angle=None, excess=None, d=None, **kwargs):
        super().__init__("teardrop_corner_mask", {"r" : r, "angle" : angle, "excess" : excess, "d" : d, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/math.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/math.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,306 +1,308 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/math.scad'}", use_not_include=False)
-
-PHI = OpenSCADConstant('PHI')
-EPSILON = OpenSCADConstant('EPSILON')
-INF = OpenSCADConstant('INF')
-NAN = OpenSCADConstant('NAN')
-class count(OpenSCADObject):
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
+
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/math.scad'}", use_not_include=False)
+
+PHI = _OpenSCADConstant('PHI')
+EPSILON = _OpenSCADConstant('EPSILON')
+INF = _OpenSCADConstant('INF')
+NAN = _OpenSCADConstant('NAN')
+class count(_Bosl2Base):
     def __init__(self, n=None, s=None, step=None, reverse=None, **kwargs):
        super().__init__("count", {"n" : n, "s" : s, "step" : step, "reverse" : reverse, **kwargs})
 
-class lerp(OpenSCADObject):
+class lerp(_Bosl2Base):
     def __init__(self, a=None, b=None, u=None, **kwargs):
        super().__init__("lerp", {"a" : a, "b" : b, "u" : u, **kwargs})
 
-class lerpn(OpenSCADObject):
+class lerpn(_Bosl2Base):
     def __init__(self, a=None, b=None, n=None, endpoint=None, **kwargs):
        super().__init__("lerpn", {"a" : a, "b" : b, "n" : n, "endpoint" : endpoint, **kwargs})
 
-class sqr(OpenSCADObject):
+class sqr(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("sqr", {"x" : x, **kwargs})
 
-class log2(OpenSCADObject):
+class log2(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("log2", {"x" : x, **kwargs})
 
-class hypot(OpenSCADObject):
+class hypot(_Bosl2Base):
     def __init__(self, x=None, y=None, z=None, **kwargs):
        super().__init__("hypot", {"x" : x, "y" : y, "z" : z, **kwargs})
 
-class factorial(OpenSCADObject):
+class factorial(_Bosl2Base):
     def __init__(self, n=None, d=None, **kwargs):
        super().__init__("factorial", {"n" : n, "d" : d, **kwargs})
 
-class binomial(OpenSCADObject):
+class binomial(_Bosl2Base):
     def __init__(self, n=None, **kwargs):
        super().__init__("binomial", {"n" : n, **kwargs})
 
-class binomial_coefficient(OpenSCADObject):
+class binomial_coefficient(_Bosl2Base):
     def __init__(self, n=None, k=None, **kwargs):
        super().__init__("binomial_coefficient", {"n" : n, "k" : k, **kwargs})
 
-class gcd(OpenSCADObject):
+class gcd(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("gcd", {"a" : a, "b" : b, **kwargs})
 
-class _lcm(OpenSCADObject):
+class _lcm(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("_lcm", {"a" : a, "b" : b, **kwargs})
 
-class _lcmlist(OpenSCADObject):
+class _lcmlist(_Bosl2Base):
     def __init__(self, a=None, **kwargs):
        super().__init__("_lcmlist", {"a" : a, **kwargs})
 
-class lcm(OpenSCADObject):
+class lcm(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("lcm", {"a" : a, "b" : b, **kwargs})
 
-class sinh(OpenSCADObject):
+class sinh(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("sinh", {"x" : x, **kwargs})
 
-class cosh(OpenSCADObject):
+class cosh(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("cosh", {"x" : x, **kwargs})
 
-class tanh(OpenSCADObject):
+class tanh(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("tanh", {"x" : x, **kwargs})
 
-class asinh(OpenSCADObject):
+class asinh(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("asinh", {"x" : x, **kwargs})
 
-class acosh(OpenSCADObject):
+class acosh(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("acosh", {"x" : x, **kwargs})
 
-class atanh(OpenSCADObject):
+class atanh(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("atanh", {"x" : x, **kwargs})
 
-class quant(OpenSCADObject):
+class quant(_Bosl2Base):
     def __init__(self, x=None, y=None, **kwargs):
        super().__init__("quant", {"x" : x, "y" : y, **kwargs})
 
-class quantdn(OpenSCADObject):
+class quantdn(_Bosl2Base):
     def __init__(self, x=None, y=None, **kwargs):
        super().__init__("quantdn", {"x" : x, "y" : y, **kwargs})
 
-class quantup(OpenSCADObject):
+class quantup(_Bosl2Base):
     def __init__(self, x=None, y=None, **kwargs):
        super().__init__("quantup", {"x" : x, "y" : y, **kwargs})
 
-class constrain(OpenSCADObject):
+class constrain(_Bosl2Base):
     def __init__(self, v=None, minval=None, maxval=None, **kwargs):
        super().__init__("constrain", {"v" : v, "minval" : minval, "maxval" : maxval, **kwargs})
 
-class posmod(OpenSCADObject):
+class posmod(_Bosl2Base):
     def __init__(self, x=None, m=None, **kwargs):
        super().__init__("posmod", {"x" : x, "m" : m, **kwargs})
 
-class modang(OpenSCADObject):
+class modang(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("modang", {"x" : x, **kwargs})
 
-class sum(OpenSCADObject):
+class sum(_Bosl2Base):
     def __init__(self, v=None, dflt=None, **kwargs):
        super().__init__("sum", {"v" : v, "dflt" : dflt, **kwargs})
 
-class _sum(OpenSCADObject):
+class _sum(_Bosl2Base):
     def __init__(self, v=None, _total=None, _i=None, **kwargs):
        super().__init__("_sum", {"v" : v, "_total" : _total, "_i" : _i, **kwargs})
 
-class mean(OpenSCADObject):
+class mean(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("mean", {"v" : v, **kwargs})
 
-class median(OpenSCADObject):
+class median(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("median", {"v" : v, **kwargs})
 
-class deltas(OpenSCADObject):
+class deltas(_Bosl2Base):
     def __init__(self, v=None, wrap=None, **kwargs):
        super().__init__("deltas", {"v" : v, "wrap" : wrap, **kwargs})
 
-class cumsum(OpenSCADObject):
+class cumsum(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("cumsum", {"v" : v, **kwargs})
 
-class _cumsum(OpenSCADObject):
+class _cumsum(_Bosl2Base):
     def __init__(self, v=None, _i=None, _acc=None, **kwargs):
        super().__init__("_cumsum", {"v" : v, "_i" : _i, "_acc" : _acc, **kwargs})
 
-class product(OpenSCADObject):
+class product(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("product", {"v" : v, **kwargs})
 
-class _product(OpenSCADObject):
+class _product(_Bosl2Base):
     def __init__(self, v=None, i=None, _tot=None, **kwargs):
        super().__init__("_product", {"v" : v, "i" : i, "_tot" : _tot, **kwargs})
 
-class cumprod(OpenSCADObject):
+class cumprod(_Bosl2Base):
     def __init__(self, list=None, **kwargs):
        super().__init__("cumprod", {"list" : list, **kwargs})
 
-class _cumprod(OpenSCADObject):
+class _cumprod(_Bosl2Base):
     def __init__(self, v=None, _i=None, _acc=None, **kwargs):
        super().__init__("_cumprod", {"v" : v, "_i" : _i, "_acc" : _acc, **kwargs})
 
-class _cumprod_vec(OpenSCADObject):
+class _cumprod_vec(_Bosl2Base):
     def __init__(self, v=None, _i=None, _acc=None, **kwargs):
        super().__init__("_cumprod_vec", {"v" : v, "_i" : _i, "_acc" : _acc, **kwargs})
 
-class convolve(OpenSCADObject):
+class convolve(_Bosl2Base):
     def __init__(self, p=None, q=None, **kwargs):
        super().__init__("convolve", {"p" : p, "q" : q, **kwargs})
 
-class sum_of_sines(OpenSCADObject):
+class sum_of_sines(_Bosl2Base):
     def __init__(self, a=None, sines=None, **kwargs):
        super().__init__("sum_of_sines", {"a" : a, "sines" : sines, **kwargs})
 
-class rand_int(OpenSCADObject):
+class rand_int(_Bosl2Base):
     def __init__(self, minval=None, maxval=None, n=None, seed=None, **kwargs):
        super().__init__("rand_int", {"minval" : minval, "maxval" : maxval, "n" : n, "seed" : seed, **kwargs})
 
-class random_points(OpenSCADObject):
+class random_points(_Bosl2Base):
     def __init__(self, n=None, dim=None, scale=None, seed=None, **kwargs):
        super().__init__("random_points", {"n" : n, "dim" : dim, "scale" : scale, "seed" : seed, **kwargs})
 
-class gaussian_rands(OpenSCADObject):
+class gaussian_rands(_Bosl2Base):
     def __init__(self, n=None, mean=None, cov=None, seed=None, **kwargs):
        super().__init__("gaussian_rands", {"n" : n, "mean" : mean, "cov" : cov, "seed" : seed, **kwargs})
 
-class exponential_rands(OpenSCADObject):
+class exponential_rands(_Bosl2Base):
     def __init__(self, n=None, _lambda=None, seed=None, **kwargs):
        super().__init__("exponential_rands", {"n" : n, "_lambda" : _lambda, "seed" : seed, **kwargs})
 
-class spherical_random_points(OpenSCADObject):
+class spherical_random_points(_Bosl2Base):
     def __init__(self, n=None, radius=None, seed=None, **kwargs):
        super().__init__("spherical_random_points", {"n" : n, "radius" : radius, "seed" : seed, **kwargs})
 
-class random_polygon(OpenSCADObject):
+class random_polygon(_Bosl2Base):
     def __init__(self, n=None, size=None, seed=None, **kwargs):
        super().__init__("random_polygon", {"n" : n, "size" : size, "seed" : seed, **kwargs})
 
-class deriv(OpenSCADObject):
+class deriv(_Bosl2Base):
     def __init__(self, data=None, h=None, closed=None, **kwargs):
        super().__init__("deriv", {"data" : data, "h" : h, "closed" : closed, **kwargs})
 
-class _dnu_calc(OpenSCADObject):
+class _dnu_calc(_Bosl2Base):
     def __init__(self, f1=None, fc=None, f2=None, h1=None, h2=None, **kwargs):
        super().__init__("_dnu_calc", {"f1" : f1, "fc" : fc, "f2" : f2, "h1" : h1, "h2" : h2, **kwargs})
 
-class _deriv_nonuniform(OpenSCADObject):
+class _deriv_nonuniform(_Bosl2Base):
     def __init__(self, data=None, h=None, closed=None, **kwargs):
        super().__init__("_deriv_nonuniform", {"data" : data, "h" : h, "closed" : closed, **kwargs})
 
-class deriv2(OpenSCADObject):
+class deriv2(_Bosl2Base):
     def __init__(self, data=None, h=None, closed=None, **kwargs):
        super().__init__("deriv2", {"data" : data, "h" : h, "closed" : closed, **kwargs})
 
-class deriv3(OpenSCADObject):
+class deriv3(_Bosl2Base):
     def __init__(self, data=None, h=None, closed=None, **kwargs):
        super().__init__("deriv3", {"data" : data, "h" : h, "closed" : closed, **kwargs})
 
-class complex(OpenSCADObject):
+class complex(_Bosl2Base):
     def __init__(self, list=None, **kwargs):
        super().__init__("complex", {"list" : list, **kwargs})
 
-class c_mul(OpenSCADObject):
+class c_mul(_Bosl2Base):
     def __init__(self, z1=None, z2=None, **kwargs):
        super().__init__("c_mul", {"z1" : z1, "z2" : z2, **kwargs})
 
-class _split_complex(OpenSCADObject):
+class _split_complex(_Bosl2Base):
     def __init__(self, data=None, **kwargs):
        super().__init__("_split_complex", {"data" : data, **kwargs})
 
-class _combine_complex(OpenSCADObject):
+class _combine_complex(_Bosl2Base):
     def __init__(self, data=None, **kwargs):
        super().__init__("_combine_complex", {"data" : data, **kwargs})
 
-class _c_mul(OpenSCADObject):
+class _c_mul(_Bosl2Base):
     def __init__(self, z1=None, z2=None, **kwargs):
        super().__init__("_c_mul", {"z1" : z1, "z2" : z2, **kwargs})
 
-class c_div(OpenSCADObject):
+class c_div(_Bosl2Base):
     def __init__(self, z1=None, z2=None, **kwargs):
        super().__init__("c_div", {"z1" : z1, "z2" : z2, **kwargs})
 
-class c_conj(OpenSCADObject):
+class c_conj(_Bosl2Base):
     def __init__(self, z=None, **kwargs):
        super().__init__("c_conj", {"z" : z, **kwargs})
 
-class c_real(OpenSCADObject):
+class c_real(_Bosl2Base):
     def __init__(self, z=None, **kwargs):
        super().__init__("c_real", {"z" : z, **kwargs})
 
-class c_imag(OpenSCADObject):
+class c_imag(_Bosl2Base):
     def __init__(self, z=None, **kwargs):
        super().__init__("c_imag", {"z" : z, **kwargs})
 
-class c_ident(OpenSCADObject):
+class c_ident(_Bosl2Base):
     def __init__(self, n=None, **kwargs):
        super().__init__("c_ident", {"n" : n, **kwargs})
 
-class c_norm(OpenSCADObject):
+class c_norm(_Bosl2Base):
     def __init__(self, z=None, **kwargs):
        super().__init__("c_norm", {"z" : z, **kwargs})
 
-class quadratic_roots(OpenSCADObject):
+class quadratic_roots(_Bosl2Base):
     def __init__(self, a=None, b=None, c=None, real=None, **kwargs):
        super().__init__("quadratic_roots", {"a" : a, "b" : b, "c" : c, "real" : real, **kwargs})
 
-class polynomial(OpenSCADObject):
+class polynomial(_Bosl2Base):
     def __init__(self, p=None, z=None, k=None, total=None, **kwargs):
        super().__init__("polynomial", {"p" : p, "z" : z, "k" : k, "total" : total, **kwargs})
 
-class poly_mult(OpenSCADObject):
+class poly_mult(_Bosl2Base):
     def __init__(self, p=None, q=None, **kwargs):
        super().__init__("poly_mult", {"p" : p, "q" : q, **kwargs})
 
-class poly_div(OpenSCADObject):
+class poly_div(_Bosl2Base):
     def __init__(self, n=None, d=None, **kwargs):
        super().__init__("poly_div", {"n" : n, "d" : d, **kwargs})
 
-class _poly_div(OpenSCADObject):
+class _poly_div(_Bosl2Base):
     def __init__(self, n=None, d=None, q=None, **kwargs):
        super().__init__("_poly_div", {"n" : n, "d" : d, "q" : q, **kwargs})
 
-class _poly_trim(OpenSCADObject):
+class _poly_trim(_Bosl2Base):
     def __init__(self, p=None, eps=None, **kwargs):
        super().__init__("_poly_trim", {"p" : p, "eps" : eps, **kwargs})
 
-class poly_add(OpenSCADObject):
+class poly_add(_Bosl2Base):
     def __init__(self, p=None, q=None, **kwargs):
        super().__init__("poly_add", {"p" : p, "q" : q, **kwargs})
 
-class poly_roots(OpenSCADObject):
+class poly_roots(_Bosl2Base):
     def __init__(self, p=None, tol=None, error_bound=None, **kwargs):
        super().__init__("poly_roots", {"p" : p, "tol" : tol, "error_bound" : error_bound, **kwargs})
 
-class _poly_roots(OpenSCADObject):
+class _poly_roots(_Bosl2Base):
     def __init__(self, p=None, pderiv=None, s=None, z=None, tol=None, i=None, **kwargs):
        super().__init__("_poly_roots", {"p" : p, "pderiv" : pderiv, "s" : s, "z" : z, "tol" : tol, "i" : i, **kwargs})
 
-class real_roots(OpenSCADObject):
+class real_roots(_Bosl2Base):
     def __init__(self, p=None, eps=None, tol=None, **kwargs):
        super().__init__("real_roots", {"p" : p, "eps" : eps, "tol" : tol, **kwargs})
 
-class root_find(OpenSCADObject):
+class root_find(_Bosl2Base):
     def __init__(self, f=None, x0=None, x1=None, tol=None, **kwargs):
        super().__init__("root_find", {"f" : f, "x0" : x0, "x1" : x1, "tol" : tol, **kwargs})
 
-class _rfcheck(OpenSCADObject):
+class _rfcheck(_Bosl2Base):
     def __init__(self, x=None, y=None, range=None, tol=None, **kwargs):
        super().__init__("_rfcheck", {"x" : x, "y" : y, "range" : range, "tol" : tol, **kwargs})
 
-class _rootfind(OpenSCADObject):
+class _rootfind(_Bosl2Base):
     def __init__(self, f=None, xpts=None, ypts=None, yrange=None, tol=None, i=None, **kwargs):
        super().__init__("_rootfind", {"f" : f, "xpts" : xpts, "ypts" : ypts, "yrange" : yrange, "tol" : tol, "i" : i, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/metric_screws.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/metric_screws.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/metric_screws.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class generic_screw(OpenSCADObject):
-    def __init__(self, screwsize=None, screwlen=None, headsize=None, headlen=None, pitch=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("generic_screw", {"screwsize" : screwsize, "screwlen" : screwlen, "headsize" : headsize, "headlen" : headlen, "pitch" : pitch, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class metric_bolt(OpenSCADObject):
-    def __init__(self, headtype=None, size=None, l=None, shank=None, pitch=None, details=None, coarse=None, phillips=None, torx=None, flange=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("metric_bolt", {"headtype" : headtype, "size" : size, "l" : l, "shank" : shank, "pitch" : pitch, "details" : details, "coarse" : coarse, "phillips" : phillips, "torx" : torx, "flange" : flange, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/metric_screws.scad'}", use_not_include=False)
 
-class metric_nut(OpenSCADObject):
-    def __init__(self, size=None, hole=None, pitch=None, details=None, flange=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("metric_nut", {"size" : size, "hole" : hole, "pitch" : pitch, "details" : details, "flange" : flange, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class get_metric_bolt_head_size(OpenSCADObject):
+class get_metric_bolt_head_size(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_bolt_head_size", {"size" : size, **kwargs})
 
-class get_metric_bolt_head_height(OpenSCADObject):
+class get_metric_bolt_head_height(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_bolt_head_height", {"size" : size, **kwargs})
 
-class get_metric_socket_cap_diam(OpenSCADObject):
+class get_metric_socket_cap_diam(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_socket_cap_diam", {"size" : size, **kwargs})
 
-class get_metric_socket_cap_height(OpenSCADObject):
+class get_metric_socket_cap_height(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_socket_cap_height", {"size" : size, **kwargs})
 
-class get_metric_socket_cap_socket_size(OpenSCADObject):
+class get_metric_socket_cap_socket_size(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_socket_cap_socket_size", {"size" : size, **kwargs})
 
-class get_metric_socket_cap_socket_depth(OpenSCADObject):
+class get_metric_socket_cap_socket_depth(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_socket_cap_socket_depth", {"size" : size, **kwargs})
 
-class get_metric_iso_coarse_thread_pitch(OpenSCADObject):
+class get_metric_iso_coarse_thread_pitch(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_iso_coarse_thread_pitch", {"size" : size, **kwargs})
 
-class get_metric_iso_fine_thread_pitch(OpenSCADObject):
+class get_metric_iso_fine_thread_pitch(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_iso_fine_thread_pitch", {"size" : size, **kwargs})
 
-class get_metric_iso_superfine_thread_pitch(OpenSCADObject):
+class get_metric_iso_superfine_thread_pitch(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_iso_superfine_thread_pitch", {"size" : size, **kwargs})
 
-class get_metric_jis_thread_pitch(OpenSCADObject):
+class get_metric_jis_thread_pitch(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_jis_thread_pitch", {"size" : size, **kwargs})
 
-class get_metric_nut_size(OpenSCADObject):
+class get_metric_nut_size(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_nut_size", {"size" : size, **kwargs})
 
-class get_metric_nut_thickness(OpenSCADObject):
+class get_metric_nut_thickness(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("get_metric_nut_thickness", {"size" : size, **kwargs})
 
+class generic_screw(_Bosl2Base):
+    def __init__(self, screwsize=None, screwlen=None, headsize=None, headlen=None, pitch=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("generic_screw", {"screwsize" : screwsize, "screwlen" : screwlen, "headsize" : headsize, "headlen" : headlen, "pitch" : pitch, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class metric_bolt(_Bosl2Base):
+    def __init__(self, headtype=None, size=None, l=None, shank=None, pitch=None, details=None, coarse=None, phillips=None, torx=None, flange=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("metric_bolt", {"headtype" : headtype, "size" : size, "l" : l, "shank" : shank, "pitch" : pitch, "details" : details, "coarse" : coarse, "phillips" : phillips, "torx" : torx, "flange" : flange, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class metric_nut(_Bosl2Base):
+    def __init__(self, size=None, hole=None, pitch=None, details=None, flange=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("metric_nut", {"size" : size, "hole" : hole, "pitch" : pitch, "details" : details, "flange" : flange, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/modular_hose.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/modular_hose.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/modular_hose.scad'}", use_not_include=False)
-
-_small_end = OpenSCADConstant('_small_end')
-_big_end = OpenSCADConstant('_big_end')
-_hose_waist = OpenSCADConstant('_hose_waist')
-class modular_hose(OpenSCADObject):
-    def __init__(self, size=None, type=None, clearance=None, waist_len=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("modular_hose", {"size" : size, "type" : type, "clearance" : clearance, "waist_len" : waist_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
+
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/modular_hose.scad'}", use_not_include=False)
 
-class modular_hose(OpenSCADObject):
+_small_end = _OpenSCADConstant('_small_end')
+_big_end = _OpenSCADConstant('_big_end')
+_hose_waist = _OpenSCADConstant('_hose_waist')
+class modular_hose(_Bosl2Base):
     def __init__(self, size=None, type=None, clearance=None, waist_len=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("modular_hose", {"size" : size, "type" : type, "clearance" : clearance, "waist_len" : waist_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class modular_hose_radius(OpenSCADObject):
+class modular_hose_radius(_Bosl2Base):
     def __init__(self, size=None, outer=None, **kwargs):
        super().__init__("modular_hose_radius", {"size" : size, "outer" : outer, **kwargs})
 
+class modular_hose(_Bosl2Base):
+    def __init__(self, size=None, type=None, clearance=None, waist_len=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("modular_hose", {"size" : size, "type" : type, "clearance" : clearance, "waist_len" : waist_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/mutators.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/mutators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/mutators.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class bounding_box(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/mutators.scad'}", use_not_include=False)
+
+class bounding_box(_Bosl2Base):
     def __init__(self, excess=None, planar=None, **kwargs):
        super().__init__("bounding_box", {"excess" : excess, "planar" : planar, **kwargs})
 
-class chain_hull(OpenSCADObject):
+class chain_hull(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("chain_hull", {**kwargs})
 
-class path_extrude2d(OpenSCADObject):
+class path_extrude2d(_Bosl2Base):
     def __init__(self, path=None, caps=None, closed=None, s=None, convexity=None, **kwargs):
        super().__init__("path_extrude2d", {"path" : path, "caps" : caps, "closed" : closed, "s" : s, "convexity" : convexity, **kwargs})
 
-class cylindrical_extrude(OpenSCADObject):
+class cylindrical_extrude(_Bosl2Base):
     def __init__(self, ir=None, _or=None, od=None, id=None, size=None, convexity=None, spin=None, orient=None, **kwargs):
        super().__init__("cylindrical_extrude", {"ir" : ir, "_or" : _or, "od" : od, "id" : id, "size" : size, "convexity" : convexity, "spin" : spin, "orient" : orient, **kwargs})
 
-class extrude_from_to(OpenSCADObject):
+class extrude_from_to(_Bosl2Base):
     def __init__(self, pt1=None, pt2=None, convexity=None, twist=None, scale=None, slices=None, **kwargs):
        super().__init__("extrude_from_to", {"pt1" : pt1, "pt2" : pt2, "convexity" : convexity, "twist" : twist, "scale" : scale, "slices" : slices, **kwargs})
 
-class path_extrude(OpenSCADObject):
+class path_extrude(_Bosl2Base):
     def __init__(self, path=None, convexity=None, clipsize=None, **kwargs):
        super().__init__("path_extrude", {"path" : path, "convexity" : convexity, "clipsize" : clipsize, **kwargs})
 
-class minkowski_difference(OpenSCADObject):
+class minkowski_difference(_Bosl2Base):
     def __init__(self, planar=None, **kwargs):
        super().__init__("minkowski_difference", {"planar" : planar, **kwargs})
 
-class offset3d(OpenSCADObject):
+class offset3d(_Bosl2Base):
     def __init__(self, r=None, size=None, convexity=None, **kwargs):
        super().__init__("offset3d", {"r" : r, "size" : size, "convexity" : convexity, **kwargs})
 
-class round3d(OpenSCADObject):
+class round3d(_Bosl2Base):
     def __init__(self, r=None, _or=None, ir=None, size=None, **kwargs):
        super().__init__("round3d", {"r" : r, "_or" : _or, "ir" : ir, "size" : size, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/nema_steppers.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/nema_steppers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,76 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/nema_steppers.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class nema11_stepper(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/nema_steppers.scad'}", use_not_include=False)
+
+class nema_motor_width(_Bosl2Base):
+    def __init__(self, size=None, **kwargs):
+       super().__init__("nema_motor_width", {"size" : size, **kwargs})
+
+class nema_motor_plinth_height(_Bosl2Base):
+    def __init__(self, size=None, **kwargs):
+       super().__init__("nema_motor_plinth_height", {"size" : size, **kwargs})
+
+class nema_motor_plinth_diam(_Bosl2Base):
+    def __init__(self, size=None, **kwargs):
+       super().__init__("nema_motor_plinth_diam", {"size" : size, **kwargs})
+
+class nema_motor_screw_spacing(_Bosl2Base):
+    def __init__(self, size=None, **kwargs):
+       super().__init__("nema_motor_screw_spacing", {"size" : size, **kwargs})
+
+class nema_motor_screw_size(_Bosl2Base):
+    def __init__(self, size=None, **kwargs):
+       super().__init__("nema_motor_screw_size", {"size" : size, **kwargs})
+
+class nema_motor_screw_depth(_Bosl2Base):
+    def __init__(self, size=None, **kwargs):
+       super().__init__("nema_motor_screw_depth", {"size" : size, **kwargs})
+
+class nema11_stepper(_Bosl2Base):
     def __init__(self, h=None, shaft=None, shaft_len=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema11_stepper", {"h" : h, "shaft" : shaft, "shaft_len" : shaft_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema14_stepper(OpenSCADObject):
+class nema14_stepper(_Bosl2Base):
     def __init__(self, h=None, shaft=None, shaft_len=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema14_stepper", {"h" : h, "shaft" : shaft, "shaft_len" : shaft_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema17_stepper(OpenSCADObject):
+class nema17_stepper(_Bosl2Base):
     def __init__(self, h=None, shaft=None, shaft_len=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema17_stepper", {"h" : h, "shaft" : shaft, "shaft_len" : shaft_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema23_stepper(OpenSCADObject):
+class nema23_stepper(_Bosl2Base):
     def __init__(self, h=None, shaft=None, shaft_len=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema23_stepper", {"h" : h, "shaft" : shaft, "shaft_len" : shaft_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema34_stepper(OpenSCADObject):
+class nema34_stepper(_Bosl2Base):
     def __init__(self, h=None, shaft=None, shaft_len=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema34_stepper", {"h" : h, "shaft" : shaft, "shaft_len" : shaft_len, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema_mount_holes(OpenSCADObject):
+class nema_mount_holes(_Bosl2Base):
     def __init__(self, size=None, depth=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema_mount_holes", {"size" : size, "depth" : depth, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema11_mount_holes(OpenSCADObject):
+class nema11_mount_holes(_Bosl2Base):
     def __init__(self, depth=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema11_mount_holes", {"depth" : depth, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema14_mount_holes(OpenSCADObject):
+class nema14_mount_holes(_Bosl2Base):
     def __init__(self, depth=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema14_mount_holes", {"depth" : depth, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema17_mount_holes(OpenSCADObject):
+class nema17_mount_holes(_Bosl2Base):
     def __init__(self, depth=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema17_mount_holes", {"depth" : depth, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema23_mount_holes(OpenSCADObject):
+class nema23_mount_holes(_Bosl2Base):
     def __init__(self, depth=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema23_mount_holes", {"depth" : depth, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema34_mount_holes(OpenSCADObject):
+class nema34_mount_holes(_Bosl2Base):
     def __init__(self, depth=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nema34_mount_holes", {"depth" : depth, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class nema_motor_width(OpenSCADObject):
-    def __init__(self, size=None, **kwargs):
-       super().__init__("nema_motor_width", {"size" : size, **kwargs})
-
-class nema_motor_plinth_height(OpenSCADObject):
-    def __init__(self, size=None, **kwargs):
-       super().__init__("nema_motor_plinth_height", {"size" : size, **kwargs})
-
-class nema_motor_plinth_diam(OpenSCADObject):
-    def __init__(self, size=None, **kwargs):
-       super().__init__("nema_motor_plinth_diam", {"size" : size, **kwargs})
-
-class nema_motor_screw_spacing(OpenSCADObject):
-    def __init__(self, size=None, **kwargs):
-       super().__init__("nema_motor_screw_spacing", {"size" : size, **kwargs})
-
-class nema_motor_screw_size(OpenSCADObject):
-    def __init__(self, size=None, **kwargs):
-       super().__init__("nema_motor_screw_size", {"size" : size, **kwargs})
-
-class nema_motor_screw_depth(OpenSCADObject):
-    def __init__(self, size=None, **kwargs):
-       super().__init__("nema_motor_screw_depth", {"size" : size, **kwargs})
-
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/partitions.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/partitions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/partitions.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class half_of(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/partitions.scad'}", use_not_include=False)
+
+class half_of(_Bosl2Base):
+    def __init__(self, p=None, v=None, cp=None, **kwargs):
+       super().__init__("half_of", {"p" : p, "v" : v, "cp" : cp, **kwargs})
+
+class left_half(_Bosl2Base):
+    def __init__(self, p=None, x=None, **kwargs):
+       super().__init__("left_half", {"p" : p, "x" : x, **kwargs})
+
+class right_half(_Bosl2Base):
+    def __init__(self, p=None, x=None, **kwargs):
+       super().__init__("right_half", {"p" : p, "x" : x, **kwargs})
+
+class front_half(_Bosl2Base):
+    def __init__(self, p=None, y=None, **kwargs):
+       super().__init__("front_half", {"p" : p, "y" : y, **kwargs})
+
+class back_half(_Bosl2Base):
+    def __init__(self, p=None, y=None, **kwargs):
+       super().__init__("back_half", {"p" : p, "y" : y, **kwargs})
+
+class bottom_half(_Bosl2Base):
+    def __init__(self, p=None, z=None, **kwargs):
+       super().__init__("bottom_half", {"p" : p, "z" : z, **kwargs})
+
+class top_half(_Bosl2Base):
+    def __init__(self, p=None, z=None, **kwargs):
+       super().__init__("top_half", {"p" : p, "z" : z, **kwargs})
+
+class _partition_subpath(_Bosl2Base):
+    def __init__(self, type=None, **kwargs):
+       super().__init__("_partition_subpath", {"type" : type, **kwargs})
+
+class _partition_cutpath(_Bosl2Base):
+    def __init__(self, l=None, h=None, cutsize=None, cutpath=None, gap=None, **kwargs):
+       super().__init__("_partition_cutpath", {"l" : l, "h" : h, "cutsize" : cutsize, "cutpath" : cutpath, "gap" : gap, **kwargs})
+
+class half_of(_Bosl2Base):
     def __init__(self, v=None, cp=None, s=None, planar=None, **kwargs):
        super().__init__("half_of", {"v" : v, "cp" : cp, "s" : s, "planar" : planar, **kwargs})
 
-class left_half(OpenSCADObject):
+class left_half(_Bosl2Base):
     def __init__(self, s=None, x=None, planar=None, **kwargs):
        super().__init__("left_half", {"s" : s, "x" : x, "planar" : planar, **kwargs})
 
-class right_half(OpenSCADObject):
+class right_half(_Bosl2Base):
     def __init__(self, s=None, x=None, planar=None, **kwargs):
        super().__init__("right_half", {"s" : s, "x" : x, "planar" : planar, **kwargs})
 
-class front_half(OpenSCADObject):
+class front_half(_Bosl2Base):
     def __init__(self, s=None, y=None, planar=None, **kwargs):
        super().__init__("front_half", {"s" : s, "y" : y, "planar" : planar, **kwargs})
 
-class back_half(OpenSCADObject):
+class back_half(_Bosl2Base):
     def __init__(self, s=None, y=None, planar=None, **kwargs):
        super().__init__("back_half", {"s" : s, "y" : y, "planar" : planar, **kwargs})
 
-class bottom_half(OpenSCADObject):
+class bottom_half(_Bosl2Base):
     def __init__(self, s=None, z=None, **kwargs):
        super().__init__("bottom_half", {"s" : s, "z" : z, **kwargs})
 
-class top_half(OpenSCADObject):
+class top_half(_Bosl2Base):
     def __init__(self, s=None, z=None, **kwargs):
        super().__init__("top_half", {"s" : s, "z" : z, **kwargs})
 
-class partition_mask(OpenSCADObject):
+class partition_mask(_Bosl2Base):
     def __init__(self, l=None, w=None, h=None, cutsize=None, cutpath=None, gap=None, inverse=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("partition_mask", {"l" : l, "w" : w, "h" : h, "cutsize" : cutsize, "cutpath" : cutpath, "gap" : gap, "inverse" : inverse, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class partition_cut_mask(OpenSCADObject):
+class partition_cut_mask(_Bosl2Base):
     def __init__(self, l=None, h=None, cutsize=None, cutpath=None, gap=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("partition_cut_mask", {"l" : l, "h" : h, "cutsize" : cutsize, "cutpath" : cutpath, "gap" : gap, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class partition(OpenSCADObject):
+class partition(_Bosl2Base):
     def __init__(self, size=None, spread=None, cutsize=None, cutpath=None, gap=None, spin=None, **kwargs):
        super().__init__("partition", {"size" : size, "spread" : spread, "cutsize" : cutsize, "cutpath" : cutpath, "gap" : gap, "spin" : spin, **kwargs})
 
-class half_of(OpenSCADObject):
-    def __init__(self, p=None, v=None, cp=None, **kwargs):
-       super().__init__("half_of", {"p" : p, "v" : v, "cp" : cp, **kwargs})
-
-class left_half(OpenSCADObject):
-    def __init__(self, p=None, x=None, **kwargs):
-       super().__init__("left_half", {"p" : p, "x" : x, **kwargs})
-
-class right_half(OpenSCADObject):
-    def __init__(self, p=None, x=None, **kwargs):
-       super().__init__("right_half", {"p" : p, "x" : x, **kwargs})
-
-class front_half(OpenSCADObject):
-    def __init__(self, p=None, y=None, **kwargs):
-       super().__init__("front_half", {"p" : p, "y" : y, **kwargs})
-
-class back_half(OpenSCADObject):
-    def __init__(self, p=None, y=None, **kwargs):
-       super().__init__("back_half", {"p" : p, "y" : y, **kwargs})
-
-class bottom_half(OpenSCADObject):
-    def __init__(self, p=None, z=None, **kwargs):
-       super().__init__("bottom_half", {"p" : p, "z" : z, **kwargs})
-
-class top_half(OpenSCADObject):
-    def __init__(self, p=None, z=None, **kwargs):
-       super().__init__("top_half", {"p" : p, "z" : z, **kwargs})
-
-class _partition_subpath(OpenSCADObject):
-    def __init__(self, type=None, **kwargs):
-       super().__init__("_partition_subpath", {"type" : type, **kwargs})
-
-class _partition_cutpath(OpenSCADObject):
-    def __init__(self, l=None, h=None, cutsize=None, cutpath=None, gap=None, **kwargs):
-       super().__init__("_partition_cutpath", {"l" : l, "h" : h, "cutsize" : cutsize, "cutpath" : cutpath, "gap" : gap, **kwargs})
-
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/paths.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/paths.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,152 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/paths.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class is_path(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/paths.scad'}", use_not_include=False)
+
+class is_path(_Bosl2Base):
     def __init__(self, list=None, dim=None, fast=None, **kwargs):
        super().__init__("is_path", {"list" : list, "dim" : dim, "fast" : fast, **kwargs})
 
-class is_1region(OpenSCADObject):
+class is_1region(_Bosl2Base):
     def __init__(self, path=None, name=None, **kwargs):
        super().__init__("is_1region", {"path" : path, "name" : name, **kwargs})
 
-class force_path(OpenSCADObject):
+class force_path(_Bosl2Base):
     def __init__(self, path=None, name=None, **kwargs):
        super().__init__("force_path", {"path" : path, "name" : name, **kwargs})
 
-class is_closed_path(OpenSCADObject):
+class is_closed_path(_Bosl2Base):
     def __init__(self, path=None, eps=None, **kwargs):
        super().__init__("is_closed_path", {"path" : path, "eps" : eps, **kwargs})
 
-class close_path(OpenSCADObject):
+class close_path(_Bosl2Base):
     def __init__(self, path=None, eps=None, **kwargs):
        super().__init__("close_path", {"path" : path, "eps" : eps, **kwargs})
 
-class cleanup_path(OpenSCADObject):
+class cleanup_path(_Bosl2Base):
     def __init__(self, path=None, eps=None, **kwargs):
        super().__init__("cleanup_path", {"path" : path, "eps" : eps, **kwargs})
 
-class _path_select(OpenSCADObject):
+class _path_select(_Bosl2Base):
     def __init__(self, path=None, s1=None, u1=None, s2=None, u2=None, closed=None, **kwargs):
        super().__init__("_path_select", {"path" : path, "s1" : s1, "u1" : u1, "s2" : s2, "u2" : u2, "closed" : closed, **kwargs})
 
-class path_merge_collinear(OpenSCADObject):
+class path_merge_collinear(_Bosl2Base):
     def __init__(self, path=None, closed=None, eps=None, **kwargs):
        super().__init__("path_merge_collinear", {"path" : path, "closed" : closed, "eps" : eps, **kwargs})
 
-class path_length(OpenSCADObject):
+class path_length(_Bosl2Base):
     def __init__(self, path=None, closed=None, **kwargs):
        super().__init__("path_length", {"path" : path, "closed" : closed, **kwargs})
 
-class path_segment_lengths(OpenSCADObject):
+class path_segment_lengths(_Bosl2Base):
     def __init__(self, path=None, closed=None, **kwargs):
        super().__init__("path_segment_lengths", {"path" : path, "closed" : closed, **kwargs})
 
-class path_length_fractions(OpenSCADObject):
+class path_length_fractions(_Bosl2Base):
     def __init__(self, path=None, closed=None, **kwargs):
        super().__init__("path_length_fractions", {"path" : path, "closed" : closed, **kwargs})
 
-class _path_self_intersections(OpenSCADObject):
+class _path_self_intersections(_Bosl2Base):
     def __init__(self, path=None, closed=None, eps=None, **kwargs):
        super().__init__("_path_self_intersections", {"path" : path, "closed" : closed, "eps" : eps, **kwargs})
 
-class _sum_preserving_round(OpenSCADObject):
+class _sum_preserving_round(_Bosl2Base):
     def __init__(self, data=None, index=None, **kwargs):
        super().__init__("_sum_preserving_round", {"data" : data, "index" : index, **kwargs})
 
-class subdivide_path(OpenSCADObject):
+class subdivide_path(_Bosl2Base):
     def __init__(self, path=None, n=None, refine=None, maxlen=None, closed=None, exact=None, method=None, **kwargs):
        super().__init__("subdivide_path", {"path" : path, "n" : n, "refine" : refine, "maxlen" : maxlen, "closed" : closed, "exact" : exact, "method" : method, **kwargs})
 
-class resample_path(OpenSCADObject):
+class resample_path(_Bosl2Base):
     def __init__(self, path=None, n=None, spacing=None, closed=None, **kwargs):
        super().__init__("resample_path", {"path" : path, "n" : n, "spacing" : spacing, "closed" : closed, **kwargs})
 
-class is_path_simple(OpenSCADObject):
+class is_path_simple(_Bosl2Base):
     def __init__(self, path=None, closed=None, eps=None, **kwargs):
        super().__init__("is_path_simple", {"path" : path, "closed" : closed, "eps" : eps, **kwargs})
 
-class path_closest_point(OpenSCADObject):
+class path_closest_point(_Bosl2Base):
     def __init__(self, path=None, pt=None, closed=None, **kwargs):
        super().__init__("path_closest_point", {"path" : path, "pt" : pt, "closed" : closed, **kwargs})
 
-class path_tangents(OpenSCADObject):
+class path_tangents(_Bosl2Base):
     def __init__(self, path=None, closed=None, uniform=None, **kwargs):
        super().__init__("path_tangents", {"path" : path, "closed" : closed, "uniform" : uniform, **kwargs})
 
-class path_normals(OpenSCADObject):
+class path_normals(_Bosl2Base):
     def __init__(self, path=None, tangents=None, closed=None, **kwargs):
        super().__init__("path_normals", {"path" : path, "tangents" : tangents, "closed" : closed, **kwargs})
 
-class path_curvature(OpenSCADObject):
+class path_curvature(_Bosl2Base):
     def __init__(self, path=None, closed=None, **kwargs):
        super().__init__("path_curvature", {"path" : path, "closed" : closed, **kwargs})
 
-class path_torsion(OpenSCADObject):
+class path_torsion(_Bosl2Base):
     def __init__(self, path=None, closed=None, **kwargs):
        super().__init__("path_torsion", {"path" : path, "closed" : closed, **kwargs})
 
-class _path_cut_points(OpenSCADObject):
+class _path_cut_points(_Bosl2Base):
     def __init__(self, path=None, dists=None, closed=None, direction=None, **kwargs):
        super().__init__("_path_cut_points", {"path" : path, "dists" : dists, "closed" : closed, "direction" : direction, **kwargs})
 
-class _path_cut_points_recurse(OpenSCADObject):
+class _path_cut_points_recurse(_Bosl2Base):
     def __init__(self, path=None, dists=None, closed=None, pind=None, dtotal=None, dind=None, result=None, **kwargs):
        super().__init__("_path_cut_points_recurse", {"path" : path, "dists" : dists, "closed" : closed, "pind" : pind, "dtotal" : dtotal, "dind" : dind, "result" : result, **kwargs})
 
-class _path_cut_single(OpenSCADObject):
+class _path_cut_single(_Bosl2Base):
     def __init__(self, path=None, dist=None, closed=None, ind=None, eps=None, **kwargs):
        super().__init__("_path_cut_single", {"path" : path, "dist" : dist, "closed" : closed, "ind" : ind, "eps" : eps, **kwargs})
 
-class _path_cuts_normals(OpenSCADObject):
+class _path_cuts_normals(_Bosl2Base):
     def __init__(self, path=None, cuts=None, dirs=None, closed=None, **kwargs):
        super().__init__("_path_cuts_normals", {"path" : path, "cuts" : cuts, "dirs" : dirs, "closed" : closed, **kwargs})
 
-class _path_plane(OpenSCADObject):
+class _path_plane(_Bosl2Base):
     def __init__(self, path=None, ind=None, i=None, closed=None, **kwargs):
        super().__init__("_path_plane", {"path" : path, "ind" : ind, "i" : i, "closed" : closed, **kwargs})
 
-class _path_cuts_dir(OpenSCADObject):
+class _path_cuts_dir(_Bosl2Base):
     def __init__(self, path=None, cuts=None, closed=None, eps=None, **kwargs):
        super().__init__("_path_cuts_dir", {"path" : path, "cuts" : cuts, "closed" : closed, "eps" : eps, **kwargs})
 
-class path_cut(OpenSCADObject):
+class path_cut(_Bosl2Base):
     def __init__(self, path=None, cutdist=None, closed=None, **kwargs):
        super().__init__("path_cut", {"path" : path, "cutdist" : cutdist, "closed" : closed, **kwargs})
 
-class _path_cut_getpaths(OpenSCADObject):
+class _path_cut_getpaths(_Bosl2Base):
     def __init__(self, path=None, cutlist=None, closed=None, **kwargs):
        super().__init__("_path_cut_getpaths", {"path" : path, "cutlist" : cutlist, "closed" : closed, **kwargs})
 
-class _cut_to_seg_u_form(OpenSCADObject):
+class _cut_to_seg_u_form(_Bosl2Base):
     def __init__(self, pathcut=None, path=None, closed=None, **kwargs):
        super().__init__("_cut_to_seg_u_form", {"pathcut" : pathcut, "path" : path, "closed" : closed, **kwargs})
 
-class split_path_at_self_crossings(OpenSCADObject):
+class split_path_at_self_crossings(_Bosl2Base):
     def __init__(self, path=None, closed=None, eps=None, **kwargs):
        super().__init__("split_path_at_self_crossings", {"path" : path, "closed" : closed, "eps" : eps, **kwargs})
 
-class _tag_self_crossing_subpaths(OpenSCADObject):
+class _tag_self_crossing_subpaths(_Bosl2Base):
     def __init__(self, path=None, nonzero=None, closed=None, eps=None, **kwargs):
        super().__init__("_tag_self_crossing_subpaths", {"path" : path, "nonzero" : nonzero, "closed" : closed, "eps" : eps, **kwargs})
 
-class polygon_parts(OpenSCADObject):
+class polygon_parts(_Bosl2Base):
     def __init__(self, poly=None, nonzero=None, eps=None, **kwargs):
        super().__init__("polygon_parts", {"poly" : poly, "nonzero" : nonzero, "eps" : eps, **kwargs})
 
-class _extreme_angle_fragment(OpenSCADObject):
+class _extreme_angle_fragment(_Bosl2Base):
     def __init__(self, seg=None, fragments=None, rightmost=None, eps=None, **kwargs):
        super().__init__("_extreme_angle_fragment", {"seg" : seg, "fragments" : fragments, "rightmost" : rightmost, "eps" : eps, **kwargs})
 
-class _assemble_a_path_from_fragments(OpenSCADObject):
+class _assemble_a_path_from_fragments(_Bosl2Base):
     def __init__(self, fragments=None, rightmost=None, startfrag=None, eps=None, **kwargs):
        super().__init__("_assemble_a_path_from_fragments", {"fragments" : fragments, "rightmost" : rightmost, "startfrag" : startfrag, "eps" : eps, **kwargs})
 
-class _assemble_path_fragments(OpenSCADObject):
+class _assemble_path_fragments(_Bosl2Base):
     def __init__(self, fragments=None, eps=None, _finished=None, **kwargs):
        super().__init__("_assemble_path_fragments", {"fragments" : fragments, "eps" : eps, "_finished" : _finished, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/polyhedra.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/polyhedra.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/polyhedra.scad'}", use_not_include=False)
-
-_tribonacci = OpenSCADConstant('_tribonacci')
-_polyhedra_ = OpenSCADConstant('_polyhedra_')
-_stellated_polyhedra_ = OpenSCADConstant('_stellated_polyhedra_')
-class regular_polyhedron(OpenSCADObject):
-    def __init__(self, name=None, index=None, type=None, faces=None, facetype=None, hasfaces=None, side=None, ir=None, mr=None, _or=None, r=None, d=None, anchor=None, rounding=None, repeat=None, facedown=None, draw=None, rotate_children=None, stellate=None, longside=None, h=None, **kwargs):
-       super().__init__("regular_polyhedron", {"name" : name, "index" : index, "type" : type, "faces" : faces, "facetype" : facetype, "hasfaces" : hasfaces, "side" : side, "ir" : ir, "mr" : mr, "_or" : _or, "r" : r, "d" : d, "anchor" : anchor, "rounding" : rounding, "repeat" : repeat, "facedown" : facedown, "draw" : draw, "rotate_children" : rotate_children, "stellate" : stellate, "longside" : longside, "h" : h, **kwargs})
-
-class _unique_groups(OpenSCADObject):
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
+
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/polyhedra.scad'}", use_not_include=False)
+
+_tribonacci = _OpenSCADConstant('_tribonacci')
+_polyhedra_ = _OpenSCADConstant('_polyhedra_')
+_stellated_polyhedra_ = _OpenSCADConstant('_stellated_polyhedra_')
+class _unique_groups(_Bosl2Base):
     def __init__(self, m=None, **kwargs):
        super().__init__("_unique_groups", {"m" : m, **kwargs})
 
-class _even_perms(OpenSCADObject):
+class _even_perms(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("_even_perms", {"v" : v, **kwargs})
 
-class _all_perms(OpenSCADObject):
+class _all_perms(_Bosl2Base):
     def __init__(self, v=None, **kwargs):
        super().__init__("_all_perms", {"v" : v, **kwargs})
 
-class _point_ref(OpenSCADObject):
+class _point_ref(_Bosl2Base):
     def __init__(self, points=None, sign=None, **kwargs):
        super().__init__("_point_ref", {"points" : points, "sign" : sign, **kwargs})
 
-class regular_polyhedron_info(OpenSCADObject):
+class regular_polyhedron_info(_Bosl2Base):
     def __init__(self, info=None, name=None, index=None, type=None, faces=None, facetype=None, hasfaces=None, side=None, ir=None, mr=None, _or=None, r=None, d=None, anchor=None, facedown=None, stellate=None, longside=None, h=None, **kwargs):
        super().__init__("regular_polyhedron_info", {"info" : info, "name" : name, "index" : index, "type" : type, "faces" : faces, "facetype" : facetype, "hasfaces" : hasfaces, "side" : side, "ir" : ir, "mr" : mr, "_or" : _or, "r" : r, "d" : d, "anchor" : anchor, "facedown" : facedown, "stellate" : stellate, "longside" : longside, "h" : h, **kwargs})
 
-class _stellate_faces(OpenSCADObject):
+class _stellate_faces(_Bosl2Base):
     def __init__(self, scalefactor=None, stellate=None, vertices=None, faces_normals=None, **kwargs):
        super().__init__("_stellate_faces", {"scalefactor" : scalefactor, "stellate" : stellate, "vertices" : vertices, "faces_normals" : faces_normals, **kwargs})
 
-class _trapezohedron(OpenSCADObject):
+class _trapezohedron(_Bosl2Base):
     def __init__(self, faces=None, r=None, side=None, longside=None, h=None, d=None, **kwargs):
        super().__init__("_trapezohedron", {"faces" : faces, "r" : r, "side" : side, "longside" : longside, "h" : h, "d" : d, **kwargs})
 
-class _facenormal(OpenSCADObject):
+class _facenormal(_Bosl2Base):
     def __init__(self, pts=None, face=None, **kwargs):
        super().__init__("_facenormal", {"pts" : pts, "face" : face, **kwargs})
 
-class _full_faces(OpenSCADObject):
+class _full_faces(_Bosl2Base):
     def __init__(self, pts=None, faces=None, **kwargs):
        super().__init__("_full_faces", {"pts" : pts, "faces" : faces, **kwargs})
 
+class regular_polyhedron(_Bosl2Base):
+    def __init__(self, name=None, index=None, type=None, faces=None, facetype=None, hasfaces=None, side=None, ir=None, mr=None, _or=None, r=None, d=None, anchor=None, rounding=None, repeat=None, facedown=None, draw=None, rotate_children=None, stellate=None, longside=None, h=None, **kwargs):
+       super().__init__("regular_polyhedron", {"name" : name, "index" : index, "type" : type, "faces" : faces, "facetype" : facetype, "hasfaces" : hasfaces, "side" : side, "ir" : ir, "mr" : mr, "_or" : _or, "r" : r, "d" : d, "anchor" : anchor, "rounding" : rounding, "repeat" : repeat, "facedown" : facedown, "draw" : draw, "rotate_children" : rotate_children, "stellate" : stellate, "longside" : longside, "h" : h, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/regions.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/regions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,134 +1,136 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/regions.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class region(OpenSCADObject):
-    def __init__(self, r=None, anchor=None, spin=None, cp=None, atype=None, **kwargs):
-       super().__init__("region", {"r" : r, "anchor" : anchor, "spin" : spin, "cp" : cp, "atype" : atype, **kwargs})
-
-class exclusive_or(OpenSCADObject):
-    def __init__(self, **kwargs):
-       super().__init__("exclusive_or", {**kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/regions.scad'}", use_not_include=False)
 
-class is_region(OpenSCADObject):
+class is_region(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("is_region", {"x" : x, **kwargs})
 
-class is_valid_region(OpenSCADObject):
+class is_valid_region(_Bosl2Base):
     def __init__(self, region=None, eps=None, **kwargs):
        super().__init__("is_valid_region", {"region" : region, "eps" : eps, **kwargs})
 
-class _polygon_crosses_region(OpenSCADObject):
+class _polygon_crosses_region(_Bosl2Base):
     def __init__(self, region=None, poly=None, eps=None, **kwargs):
        super().__init__("_polygon_crosses_region", {"region" : region, "poly" : poly, "eps" : eps, **kwargs})
 
-class is_region_simple(OpenSCADObject):
+class is_region_simple(_Bosl2Base):
     def __init__(self, region=None, eps=None, **kwargs):
        super().__init__("is_region_simple", {"region" : region, "eps" : eps, **kwargs})
 
-class make_region(OpenSCADObject):
+class make_region(_Bosl2Base):
     def __init__(self, polys=None, nonzero=None, eps=None, **kwargs):
        super().__init__("make_region", {"polys" : polys, "nonzero" : nonzero, "eps" : eps, **kwargs})
 
-class force_region(OpenSCADObject):
+class force_region(_Bosl2Base):
     def __init__(self, poly=None, **kwargs):
        super().__init__("force_region", {"poly" : poly, **kwargs})
 
-class point_in_region(OpenSCADObject):
+class point_in_region(_Bosl2Base):
     def __init__(self, point=None, region=None, eps=None, **kwargs):
        super().__init__("point_in_region", {"point" : point, "region" : region, "eps" : eps, **kwargs})
 
-class _point_in_region(OpenSCADObject):
+class _point_in_region(_Bosl2Base):
     def __init__(self, point=None, region=None, eps=None, i=None, cnt=None, **kwargs):
        super().__init__("_point_in_region", {"point" : point, "region" : region, "eps" : eps, "i" : i, "cnt" : cnt, **kwargs})
 
-class region_area(OpenSCADObject):
+class region_area(_Bosl2Base):
     def __init__(self, region=None, **kwargs):
        super().__init__("region_area", {"region" : region, **kwargs})
 
-class _clockwise_region(OpenSCADObject):
+class _clockwise_region(_Bosl2Base):
     def __init__(self, r=None, **kwargs):
        super().__init__("_clockwise_region", {"r" : r, **kwargs})
 
-class are_regions_equal(OpenSCADObject):
+class are_regions_equal(_Bosl2Base):
     def __init__(self, region1=None, region2=None, either_winding=None, **kwargs):
        super().__init__("are_regions_equal", {"region1" : region1, "region2" : region2, "either_winding" : either_winding, **kwargs})
 
-class __are_regions_equal(OpenSCADObject):
+class __are_regions_equal(_Bosl2Base):
     def __init__(self, region1=None, region2=None, i=None, **kwargs):
        super().__init__("__are_regions_equal", {"region1" : region1, "region2" : region2, "i" : i, **kwargs})
 
-class _region_region_intersections(OpenSCADObject):
+class _region_region_intersections(_Bosl2Base):
     def __init__(self, region1=None, region2=None, closed1=None, closed2=None, eps=None, **kwargs):
        super().__init__("_region_region_intersections", {"region1" : region1, "region2" : region2, "closed1" : closed1, "closed2" : closed2, "eps" : eps, **kwargs})
 
-class split_region_at_region_crossings(OpenSCADObject):
+class split_region_at_region_crossings(_Bosl2Base):
     def __init__(self, region1=None, region2=None, closed1=None, closed2=None, eps=None, **kwargs):
        super().__init__("split_region_at_region_crossings", {"region1" : region1, "region2" : region2, "closed1" : closed1, "closed2" : closed2, "eps" : eps, **kwargs})
 
-class region_parts(OpenSCADObject):
+class region_parts(_Bosl2Base):
     def __init__(self, region=None, **kwargs):
        super().__init__("region_parts", {"region" : region, **kwargs})
 
-class _offset_chamfer(OpenSCADObject):
+class _offset_chamfer(_Bosl2Base):
     def __init__(self, center=None, points=None, delta=None, **kwargs):
        super().__init__("_offset_chamfer", {"center" : center, "points" : points, "delta" : delta, **kwargs})
 
-class _shift_segment(OpenSCADObject):
+class _shift_segment(_Bosl2Base):
     def __init__(self, segment=None, d=None, **kwargs):
        super().__init__("_shift_segment", {"segment" : segment, "d" : d, **kwargs})
 
-class _segment_extension(OpenSCADObject):
+class _segment_extension(_Bosl2Base):
     def __init__(self, s1=None, s2=None, **kwargs):
        super().__init__("_segment_extension", {"s1" : s1, "s2" : s2, **kwargs})
 
-class _makefaces(OpenSCADObject):
+class _makefaces(_Bosl2Base):
     def __init__(self, direction=None, startind=None, good=None, pointcount=None, closed=None, **kwargs):
        super().__init__("_makefaces", {"direction" : direction, "startind" : startind, "good" : good, "pointcount" : pointcount, "closed" : closed, **kwargs})
 
-class _makefaces_recurse(OpenSCADObject):
+class _makefaces_recurse(_Bosl2Base):
     def __init__(self, startind1=None, startind2=None, numfirst=None, numsecond=None, lenlist=None, closed=None, firstind=None, secondind=None, faces=None, **kwargs):
        super().__init__("_makefaces_recurse", {"startind1" : startind1, "startind2" : startind2, "numfirst" : numfirst, "numsecond" : numsecond, "lenlist" : lenlist, "closed" : closed, "firstind" : firstind, "secondind" : secondind, "faces" : faces, **kwargs})
 
-class _good_segments(OpenSCADObject):
+class _good_segments(_Bosl2Base):
     def __init__(self, path=None, d=None, shiftsegs=None, closed=None, quality=None, **kwargs):
        super().__init__("_good_segments", {"path" : path, "d" : d, "shiftsegs" : shiftsegs, "closed" : closed, "quality" : quality, **kwargs})
 
-class _segment_good(OpenSCADObject):
+class _segment_good(_Bosl2Base):
     def __init__(self, path=None, pathseg_unit=None, pathseg_len=None, d=None, seg=None, alpha=None, index=None, **kwargs):
        super().__init__("_segment_good", {"path" : path, "pathseg_unit" : pathseg_unit, "pathseg_len" : pathseg_len, "d" : d, "seg" : seg, "alpha" : alpha, "index" : index, **kwargs})
 
-class _point_dist(OpenSCADObject):
+class _point_dist(_Bosl2Base):
     def __init__(self, path=None, pathseg_unit=None, pathseg_len=None, pt=None, **kwargs):
        super().__init__("_point_dist", {"path" : path, "pathseg_unit" : pathseg_unit, "pathseg_len" : pathseg_len, "pt" : pt, **kwargs})
 
-class offset(OpenSCADObject):
+class offset(_Bosl2Base):
     def __init__(self, path=None, r=None, delta=None, chamfer=None, closed=None, check_valid=None, quality=None, return_faces=None, firstface_index=None, flip_faces=None, same_length=None, **kwargs):
        super().__init__("offset", {"path" : path, "r" : r, "delta" : delta, "chamfer" : chamfer, "closed" : closed, "check_valid" : check_valid, "quality" : quality, "return_faces" : return_faces, "firstface_index" : firstface_index, "flip_faces" : flip_faces, "same_length" : same_length, **kwargs})
 
-class _filter_region_parts(OpenSCADObject):
+class _filter_region_parts(_Bosl2Base):
     def __init__(self, region1=None, region2=None, keep=None, eps=None, **kwargs):
        super().__init__("_filter_region_parts", {"region1" : region1, "region2" : region2, "keep" : keep, "eps" : eps, **kwargs})
 
-class _list_three(OpenSCADObject):
+class _list_three(_Bosl2Base):
     def __init__(self, a=None, b=None, c=None, **kwargs):
        super().__init__("_list_three", {"a" : a, "b" : b, "c" : c, **kwargs})
 
-class union(OpenSCADObject):
+class union(_Bosl2Base):
     def __init__(self, regions=None, b=None, c=None, eps=None, **kwargs):
        super().__init__("union", {"regions" : regions, "b" : b, "c" : c, "eps" : eps, **kwargs})
 
-class difference(OpenSCADObject):
+class difference(_Bosl2Base):
     def __init__(self, regions=None, b=None, c=None, eps=None, **kwargs):
        super().__init__("difference", {"regions" : regions, "b" : b, "c" : c, "eps" : eps, **kwargs})
 
-class intersection(OpenSCADObject):
+class intersection(_Bosl2Base):
     def __init__(self, regions=None, b=None, c=None, eps=None, **kwargs):
        super().__init__("intersection", {"regions" : regions, "b" : b, "c" : c, "eps" : eps, **kwargs})
 
-class exclusive_or(OpenSCADObject):
+class exclusive_or(_Bosl2Base):
     def __init__(self, regions=None, b=None, c=None, eps=None, **kwargs):
        super().__init__("exclusive_or", {"regions" : regions, "b" : b, "c" : c, "eps" : eps, **kwargs})
 
+class region(_Bosl2Base):
+    def __init__(self, r=None, anchor=None, spin=None, cp=None, atype=None, **kwargs):
+       super().__init__("region", {"r" : r, "anchor" : anchor, "spin" : spin, "cp" : cp, "atype" : atype, **kwargs})
+
+class exclusive_or(_Bosl2Base):
+    def __init__(self, **kwargs):
+       super().__init__("exclusive_or", {**kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/rounding.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/rounding.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,230 +1,232 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/rounding.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class round_corners(OpenSCADObject):
-    def __init__(self, path=None, method=None, radius=None, r=None, cut=None, joint=None, width=None, k=None, closed=None, verbose=None, **kwargs):
-       super().__init__("round_corners", {"path" : path, "method" : method, "radius" : radius, "r" : r, "cut" : cut, "joint" : joint, "width" : width, "k" : k, "closed" : closed, "verbose" : verbose, **kwargs})
-
-class smooth_path(OpenSCADObject):
-    def __init__(self, path=None, tangents=None, size=None, relsize=None, splinesteps=None, uniform=None, closed=None, **kwargs):
-       super().__init__("smooth_path", {"path" : path, "tangents" : tangents, "size" : size, "relsize" : relsize, "splinesteps" : splinesteps, "uniform" : uniform, "closed" : closed, **kwargs})
-
-class path_join(OpenSCADObject):
-    def __init__(self, paths=None, joint=None, k=None, relocate=None, closed=None, **kwargs):
-       super().__init__("path_join", {"paths" : paths, "joint" : joint, "k" : k, "relocate" : relocate, "closed" : closed, **kwargs})
-
-class offset_stroke(OpenSCADObject):
-    def __init__(self, path=None, width=None, rounded=None, start=None, end=None, check_valid=None, quality=None, chamfer=None, closed=None, **kwargs):
-       super().__init__("offset_stroke", {"path" : path, "width" : width, "rounded" : rounded, "start" : start, "end" : end, "check_valid" : check_valid, "quality" : quality, "chamfer" : chamfer, "closed" : closed, **kwargs})
-
-class offset_sweep(OpenSCADObject):
-    def __init__(self, path=None, height=None, bottom=None, top=None, h=None, l=None, offset=None, r=None, steps=None, quality=None, check_valid=None, extra=None, cut=None, chamfer_width=None, chamfer_height=None, joint=None, k=None, angle=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
-       super().__init__("offset_sweep", {"path" : path, "height" : height, "bottom" : bottom, "top" : top, "h" : h, "l" : l, "offset" : offset, "r" : r, "steps" : steps, "quality" : quality, "check_valid" : check_valid, "extra" : extra, "cut" : cut, "chamfer_width" : chamfer_width, "chamfer_height" : chamfer_height, "joint" : joint, "k" : k, "angle" : angle, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/rounding.scad'}", use_not_include=False)
 
-class convex_offset_extrude(OpenSCADObject):
-    def __init__(self, height=None, bottom=None, top=None, h=None, l=None, length=None, offset=None, r=None, steps=None, extra=None, cut=None, chamfer_width=None, chamfer_height=None, joint=None, k=None, angle=None, convexity=None, thickness=None, **kwargs):
-       super().__init__("convex_offset_extrude", {"height" : height, "bottom" : bottom, "top" : top, "h" : h, "l" : l, "length" : length, "offset" : offset, "r" : r, "steps" : steps, "extra" : extra, "cut" : cut, "chamfer_width" : chamfer_width, "chamfer_height" : chamfer_height, "joint" : joint, "k" : k, "angle" : angle, "convexity" : convexity, "thickness" : thickness, **kwargs})
-
-class rounded_prism(OpenSCADObject):
-    def __init__(self, bottom=None, top=None, joint_bot=None, joint_top=None, joint_sides=None, k_bot=None, k_top=None, k_sides=None, k=None, splinesteps=None, h=None, length=None, l=None, height=None, convexity=None, debug=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
-       super().__init__("rounded_prism", {"bottom" : bottom, "top" : top, "joint_bot" : joint_bot, "joint_top" : joint_top, "joint_sides" : joint_sides, "k_bot" : k_bot, "k_top" : k_top, "k_sides" : k_sides, "k" : k, "splinesteps" : splinesteps, "h" : h, "length" : length, "l" : l, "height" : height, "convexity" : convexity, "debug" : debug, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
-
-class bent_cutout_mask(OpenSCADObject):
-    def __init__(self, r=None, thickness=None, path=None, radius=None, convexity=None, **kwargs):
-       super().__init__("bent_cutout_mask", {"r" : r, "thickness" : thickness, "path" : path, "radius" : radius, "convexity" : convexity, **kwargs})
-
-class join_prism(OpenSCADObject):
-    def __init__(self, polygon=None, base=None, base_r=None, base_d=None, base_T=None, scale=None, prism_end_T=None, short=None, length=None, l=None, height=None, h=None, aux=None, aux_T=None, aux_r=None, aux_d=None, overlap=None, base_overlap=None, aux_overlap=None, n=None, base_n=None, end_n=None, aux_n=None, fillet=None, base_fillet=None, aux_fillet=None, end_round=None, k=None, base_k=None, aux_k=None, end_k=None, uniform=None, base_uniform=None, aux_uniform=None, debug=None, anchor=None, extent=None, cp=None, atype=None, orient=None, spin=None, convexity=None, **kwargs):
-       super().__init__("join_prism", {"polygon" : polygon, "base" : base, "base_r" : base_r, "base_d" : base_d, "base_T" : base_T, "scale" : scale, "prism_end_T" : prism_end_T, "short" : short, "length" : length, "l" : l, "height" : height, "h" : h, "aux" : aux, "aux_T" : aux_T, "aux_r" : aux_r, "aux_d" : aux_d, "overlap" : overlap, "base_overlap" : base_overlap, "aux_overlap" : aux_overlap, "n" : n, "base_n" : base_n, "end_n" : end_n, "aux_n" : aux_n, "fillet" : fillet, "base_fillet" : base_fillet, "aux_fillet" : aux_fillet, "end_round" : end_round, "k" : k, "base_k" : base_k, "aux_k" : aux_k, "end_k" : end_k, "uniform" : uniform, "base_uniform" : base_uniform, "aux_uniform" : aux_uniform, "debug" : debug, "anchor" : anchor, "extent" : extent, "cp" : cp, "atype" : atype, "orient" : orient, "spin" : spin, "convexity" : convexity, **kwargs})
-
-class round_corners(OpenSCADObject):
+class round_corners(_Bosl2Base):
     def __init__(self, path=None, method=None, radius=None, r=None, cut=None, joint=None, width=None, k=None, closed=None, verbose=None, **kwargs):
        super().__init__("round_corners", {"path" : path, "method" : method, "radius" : radius, "r" : r, "cut" : cut, "joint" : joint, "width" : width, "k" : k, "closed" : closed, "verbose" : verbose, **kwargs})
 
-class _smooth_bez_fill(OpenSCADObject):
+class _smooth_bez_fill(_Bosl2Base):
     def __init__(self, points=None, k=None, **kwargs):
        super().__init__("_smooth_bez_fill", {"points" : points, "k" : k, **kwargs})
 
-class _bezcorner(OpenSCADObject):
+class _bezcorner(_Bosl2Base):
     def __init__(self, points=None, parm=None, **kwargs):
        super().__init__("_bezcorner", {"points" : points, "parm" : parm, **kwargs})
 
-class _chamfcorner(OpenSCADObject):
+class _chamfcorner(_Bosl2Base):
     def __init__(self, points=None, parm=None, **kwargs):
        super().__init__("_chamfcorner", {"points" : points, "parm" : parm, **kwargs})
 
-class _circlecorner(OpenSCADObject):
+class _circlecorner(_Bosl2Base):
     def __init__(self, points=None, parm=None, **kwargs):
        super().__init__("_circlecorner", {"points" : points, "parm" : parm, **kwargs})
 
-class _rounding_offsets(OpenSCADObject):
+class _rounding_offsets(_Bosl2Base):
     def __init__(self, edgespec=None, z_dir=None, **kwargs):
        super().__init__("_rounding_offsets", {"edgespec" : edgespec, "z_dir" : z_dir, **kwargs})
 
-class smooth_path(OpenSCADObject):
+class smooth_path(_Bosl2Base):
     def __init__(self, path=None, tangents=None, size=None, relsize=None, splinesteps=None, uniform=None, closed=None, **kwargs):
        super().__init__("smooth_path", {"path" : path, "tangents" : tangents, "size" : size, "relsize" : relsize, "splinesteps" : splinesteps, "uniform" : uniform, "closed" : closed, **kwargs})
 
-class _scalar_to_vector(OpenSCADObject):
+class _scalar_to_vector(_Bosl2Base):
     def __init__(self, value=None, length=None, varname=None, **kwargs):
        super().__init__("_scalar_to_vector", {"value" : value, "length" : length, "varname" : varname, **kwargs})
 
-class path_join(OpenSCADObject):
+class path_join(_Bosl2Base):
     def __init__(self, paths=None, joint=None, k=None, relocate=None, closed=None, **kwargs):
        super().__init__("path_join", {"paths" : paths, "joint" : joint, "k" : k, "relocate" : relocate, "closed" : closed, **kwargs})
 
-class _path_join(OpenSCADObject):
+class _path_join(_Bosl2Base):
     def __init__(self, paths=None, joint=None, k=None, i=None, result=None, relocate=None, closed=None, **kwargs):
        super().__init__("_path_join", {"paths" : paths, "joint" : joint, "k" : k, "i" : i, "result" : result, "relocate" : relocate, "closed" : closed, **kwargs})
 
-class offset_stroke(OpenSCADObject):
+class offset_stroke(_Bosl2Base):
     def __init__(self, path=None, width=None, rounded=None, start=None, end=None, check_valid=None, quality=None, chamfer=None, closed=None, **kwargs):
        super().__init__("offset_stroke", {"path" : path, "width" : width, "rounded" : rounded, "start" : start, "end" : end, "check_valid" : check_valid, "quality" : quality, "chamfer" : chamfer, "closed" : closed, **kwargs})
 
-class os_pointed(OpenSCADObject):
+class os_pointed(_Bosl2Base):
     def __init__(self, dist=None, loc=None, **kwargs):
        super().__init__("os_pointed", {"dist" : dist, "loc" : loc, **kwargs})
 
-class os_round(OpenSCADObject):
+class os_round(_Bosl2Base):
     def __init__(self, cut=None, angle=None, abs_angle=None, k=None, r=None, **kwargs):
        super().__init__("os_round", {"cut" : cut, "angle" : angle, "abs_angle" : abs_angle, "k" : k, "r" : r, **kwargs})
 
-class os_flat(OpenSCADObject):
+class os_flat(_Bosl2Base):
     def __init__(self, angle=None, abs_angle=None, **kwargs):
        super().__init__("os_flat", {"angle" : angle, "abs_angle" : abs_angle, **kwargs})
 
-class angle_between_lines(OpenSCADObject):
+class angle_between_lines(_Bosl2Base):
     def __init__(self, line1=None, line2=None, **kwargs):
        super().__init__("angle_between_lines", {"line1" : line1, "line2" : line2, **kwargs})
 
-class _parse_stroke_end(OpenSCADObject):
+class _parse_stroke_end(_Bosl2Base):
     def __init__(self, spec=None, name=None, **kwargs):
        super().__init__("_parse_stroke_end", {"spec" : spec, "name" : name, **kwargs})
 
-class _stroke_end(OpenSCADObject):
+class _stroke_end(_Bosl2Base):
     def __init__(self, width=None, left=None, right=None, spec=None, **kwargs):
        super().__init__("_stroke_end", {"width" : width, "left" : left, "right" : right, "spec" : spec, **kwargs})
 
-class _path_line_intersection(OpenSCADObject):
+class _path_line_intersection(_Bosl2Base):
     def __init__(self, path=None, line=None, ind=None, **kwargs):
        super().__init__("_path_line_intersection", {"path" : path, "line" : line, "ind" : ind, **kwargs})
 
-class _make_offset_polyhedron(OpenSCADObject):
+class _make_offset_polyhedron(_Bosl2Base):
     def __init__(self, path=None, offsets=None, offset_type=None, flip_faces=None, quality=None, check_valid=None, offsetind=None, vertexcount=None, vertices=None, faces=None, **kwargs):
        super().__init__("_make_offset_polyhedron", {"path" : path, "offsets" : offsets, "offset_type" : offset_type, "flip_faces" : flip_faces, "quality" : quality, "check_valid" : check_valid, "offsetind" : offsetind, "vertexcount" : vertexcount, "vertices" : vertices, "faces" : faces, **kwargs})
 
-class _struct_valid(OpenSCADObject):
+class _struct_valid(_Bosl2Base):
     def __init__(self, spec=None, func=None, name=None, **kwargs):
        super().__init__("_struct_valid", {"spec" : spec, "func" : func, "name" : name, **kwargs})
 
-class offset_sweep(OpenSCADObject):
+class offset_sweep(_Bosl2Base):
     def __init__(self, path=None, height=None, bottom=None, top=None, h=None, l=None, length=None, offset=None, r=None, steps=None, quality=None, check_valid=None, extra=None, cut=None, chamfer_width=None, chamfer_height=None, joint=None, k=None, angle=None, **kwargs):
        super().__init__("offset_sweep", {"path" : path, "height" : height, "bottom" : bottom, "top" : top, "h" : h, "l" : l, "length" : length, "offset" : offset, "r" : r, "steps" : steps, "quality" : quality, "check_valid" : check_valid, "extra" : extra, "cut" : cut, "chamfer_width" : chamfer_width, "chamfer_height" : chamfer_height, "joint" : joint, "k" : k, "angle" : angle, **kwargs})
 
-class os_circle(OpenSCADObject):
+class os_circle(_Bosl2Base):
     def __init__(self, r=None, cut=None, extra=None, check_valid=None, quality=None, steps=None, offset=None, **kwargs):
        super().__init__("os_circle", {"r" : r, "cut" : cut, "extra" : extra, "check_valid" : check_valid, "quality" : quality, "steps" : steps, "offset" : offset, **kwargs})
 
-class os_teardrop(OpenSCADObject):
+class os_teardrop(_Bosl2Base):
     def __init__(self, r=None, cut=None, extra=None, check_valid=None, quality=None, steps=None, offset=None, **kwargs):
        super().__init__("os_teardrop", {"r" : r, "cut" : cut, "extra" : extra, "check_valid" : check_valid, "quality" : quality, "steps" : steps, "offset" : offset, **kwargs})
 
-class os_chamfer(OpenSCADObject):
+class os_chamfer(_Bosl2Base):
     def __init__(self, height=None, width=None, cut=None, angle=None, extra=None, check_valid=None, quality=None, steps=None, offset=None, **kwargs):
        super().__init__("os_chamfer", {"height" : height, "width" : width, "cut" : cut, "angle" : angle, "extra" : extra, "check_valid" : check_valid, "quality" : quality, "steps" : steps, "offset" : offset, **kwargs})
 
-class os_smooth(OpenSCADObject):
+class os_smooth(_Bosl2Base):
     def __init__(self, cut=None, joint=None, k=None, extra=None, check_valid=None, quality=None, steps=None, offset=None, **kwargs):
        super().__init__("os_smooth", {"cut" : cut, "joint" : joint, "k" : k, "extra" : extra, "check_valid" : check_valid, "quality" : quality, "steps" : steps, "offset" : offset, **kwargs})
 
-class os_profile(OpenSCADObject):
+class os_profile(_Bosl2Base):
     def __init__(self, points=None, extra=None, check_valid=None, quality=None, offset=None, **kwargs):
        super().__init__("os_profile", {"points" : points, "extra" : extra, "check_valid" : check_valid, "quality" : quality, "offset" : offset, **kwargs})
 
-class os_mask(OpenSCADObject):
+class os_mask(_Bosl2Base):
     def __init__(self, mask=None, out=None, extra=None, check_valid=None, quality=None, offset=None, **kwargs):
        super().__init__("os_mask", {"mask" : mask, "out" : out, "extra" : extra, "check_valid" : check_valid, "quality" : quality, "offset" : offset, **kwargs})
 
-class convex_offset_extrude(OpenSCADObject):
+class convex_offset_extrude(_Bosl2Base):
     def __init__(self, height=None, bottom=None, top=None, h=None, l=None, length=None, offset=None, r=None, steps=None, extra=None, cut=None, chamfer_width=None, chamfer_height=None, joint=None, k=None, angle=None, convexity=None, thickness=None, **kwargs):
        super().__init__("convex_offset_extrude", {"height" : height, "bottom" : bottom, "top" : top, "h" : h, "l" : l, "length" : length, "offset" : offset, "r" : r, "steps" : steps, "extra" : extra, "cut" : cut, "chamfer_width" : chamfer_width, "chamfer_height" : chamfer_height, "joint" : joint, "k" : k, "angle" : angle, "convexity" : convexity, "thickness" : thickness, **kwargs})
 
-class _remove_undefined_vals(OpenSCADObject):
+class _remove_undefined_vals(_Bosl2Base):
     def __init__(self, list=None, **kwargs):
        super().__init__("_remove_undefined_vals", {"list" : list, **kwargs})
 
-class _rp_compute_patches(OpenSCADObject):
+class _rp_compute_patches(_Bosl2Base):
     def __init__(self, top=None, bot=None, rtop=None, rsides=None, ktop=None, ksides=None, concave=None, **kwargs):
        super().__init__("_rp_compute_patches", {"top" : top, "bot" : bot, "rtop" : rtop, "rsides" : rsides, "ktop" : ktop, "ksides" : ksides, "concave" : concave, **kwargs})
 
-class rounded_prism(OpenSCADObject):
+class rounded_prism(_Bosl2Base):
     def __init__(self, bottom=None, top=None, joint_bot=None, joint_top=None, joint_sides=None, k_bot=None, k_top=None, k_sides=None, k=None, splinesteps=None, h=None, length=None, l=None, height=None, debug=None, **kwargs):
        super().__init__("rounded_prism", {"bottom" : bottom, "top" : top, "joint_bot" : joint_bot, "joint_top" : joint_top, "joint_sides" : joint_sides, "k_bot" : k_bot, "k_top" : k_top, "k_sides" : k_sides, "k" : k, "splinesteps" : splinesteps, "h" : h, "length" : length, "l" : l, "height" : height, "debug" : debug, **kwargs})
 
-class _cyl_hole(OpenSCADObject):
+class _cyl_hole(_Bosl2Base):
     def __init__(self, r=None, path=None, **kwargs):
        super().__init__("_cyl_hole", {"r" : r, "path" : path, **kwargs})
 
-class _circle_mask(OpenSCADObject):
+class _circle_mask(_Bosl2Base):
     def __init__(self, r=None, **kwargs):
        super().__init__("_circle_mask", {"r" : r, **kwargs})
 
-class bent_cutout_mask(OpenSCADObject):
+class bent_cutout_mask(_Bosl2Base):
     def __init__(self, r=None, thickness=None, path=None, radius=None, convexity=None, **kwargs):
        super().__init__("bent_cutout_mask", {"r" : r, "thickness" : thickness, "path" : path, "radius" : radius, "convexity" : convexity, **kwargs})
 
-class join_prism(OpenSCADObject):
+class join_prism(_Bosl2Base):
     def __init__(self, polygon=None, base=None, base_r=None, base_d=None, base_T=None, scale=None, prism_end_T=None, short=None, length=None, l=None, height=None, h=None, aux=None, aux_T=None, aux_r=None, aux_d=None, overlap=None, base_overlap=None, aux_overlap=None, n=None, base_n=None, aux_n=None, end_n=None, fillet=None, base_fillet=None, aux_fillet=None, end_round=None, k=None, base_k=None, aux_k=None, end_k=None, uniform=None, base_uniform=None, aux_uniform=None, debug=None, return_axis=None, **kwargs):
        super().__init__("join_prism", {"polygon" : polygon, "base" : base, "base_r" : base_r, "base_d" : base_d, "base_T" : base_T, "scale" : scale, "prism_end_T" : prism_end_T, "short" : short, "length" : length, "l" : l, "height" : height, "h" : h, "aux" : aux, "aux_T" : aux_T, "aux_r" : aux_r, "aux_d" : aux_d, "overlap" : overlap, "base_overlap" : base_overlap, "aux_overlap" : aux_overlap, "n" : n, "base_n" : base_n, "aux_n" : aux_n, "end_n" : end_n, "fillet" : fillet, "base_fillet" : base_fillet, "aux_fillet" : aux_fillet, "end_round" : end_round, "k" : k, "base_k" : base_k, "aux_k" : aux_k, "end_k" : end_k, "uniform" : uniform, "base_uniform" : base_uniform, "aux_uniform" : aux_uniform, "debug" : debug, "return_axis" : return_axis, **kwargs})
 
-class _fix_angle_list(OpenSCADObject):
+class _fix_angle_list(_Bosl2Base):
     def __init__(self, list=None, ind=None, result=None, **kwargs):
        super().__init__("_fix_angle_list", {"list" : list, "ind" : ind, "result" : result, **kwargs})
 
-class _cyl_line_intersection(OpenSCADObject):
+class _cyl_line_intersection(_Bosl2Base):
     def __init__(self, R=None, line=None, ref=None, **kwargs):
        super().__init__("_cyl_line_intersection", {"R" : R, "line" : line, "ref" : ref, **kwargs})
 
-class _sphere_line_isect_best(OpenSCADObject):
+class _sphere_line_isect_best(_Bosl2Base):
     def __init__(self, R=None, line=None, ref=None, **kwargs):
        super().__init__("_sphere_line_isect_best", {"R" : R, "line" : line, "ref" : ref, **kwargs})
 
-class _prism_line_isect(OpenSCADObject):
+class _prism_line_isect(_Bosl2Base):
     def __init__(self, poly_pairs=None, line=None, ref=None, **kwargs):
        super().__init__("_prism_line_isect", {"poly_pairs" : poly_pairs, "line" : line, "ref" : ref, **kwargs})
 
-class _prism_fillet(OpenSCADObject):
+class _prism_fillet(_Bosl2Base):
     def __init__(self, name=None, base=None, R=None, bot=None, top=None, d=None, k=None, N=None, overlap=None, uniform=None, debug=None, **kwargs):
        super().__init__("_prism_fillet", {"name" : name, "base" : base, "R" : R, "bot" : bot, "top" : top, "d" : d, "k" : k, "N" : N, "overlap" : overlap, "uniform" : uniform, "debug" : debug, **kwargs})
 
-class _prism_fillet_plane(OpenSCADObject):
+class _prism_fillet_plane(_Bosl2Base):
     def __init__(self, name=None, bot=None, top=None, d=None, k=None, N=None, overlap=None, debug=None, **kwargs):
        super().__init__("_prism_fillet_plane", {"name" : name, "bot" : bot, "top" : top, "d" : d, "k" : k, "N" : N, "overlap" : overlap, "debug" : debug, **kwargs})
 
-class _prism_fillet_plane(OpenSCADObject):
+class _prism_fillet_plane(_Bosl2Base):
     def __init__(self, name=None, bot=None, top=None, d=None, k=None, N=None, overlap=None, debug=None, **kwargs):
        super().__init__("_prism_fillet_plane", {"name" : name, "bot" : bot, "top" : top, "d" : d, "k" : k, "N" : N, "overlap" : overlap, "debug" : debug, **kwargs})
 
-class _prism_fillet_cyl(OpenSCADObject):
+class _prism_fillet_cyl(_Bosl2Base):
     def __init__(self, name=None, R=None, bot=None, top=None, d=None, k=None, N=None, overlap=None, uniform=None, debug=None, **kwargs):
        super().__init__("_prism_fillet_cyl", {"name" : name, "R" : R, "bot" : bot, "top" : top, "d" : d, "k" : k, "N" : N, "overlap" : overlap, "uniform" : uniform, "debug" : debug, **kwargs})
 
-class _prism_fillet_sphere(OpenSCADObject):
+class _prism_fillet_sphere(_Bosl2Base):
     def __init__(self, name=None, R=None, bot=None, top=None, d=None, k=None, N=None, overlap=None, uniform=None, debug=None, **kwargs):
        super().__init__("_prism_fillet_sphere", {"name" : name, "R" : R, "bot" : bot, "top" : top, "d" : d, "k" : k, "N" : N, "overlap" : overlap, "uniform" : uniform, "debug" : debug, **kwargs})
 
-class _getnormal(OpenSCADObject):
+class _getnormal(_Bosl2Base):
     def __init__(self, polygon=None, index=None, u=None, **kwargs):
        super().__init__("_getnormal", {"polygon" : polygon, "index" : index, "u" : u, **kwargs})
 
-class _polygon_step(OpenSCADObject):
+class _polygon_step(_Bosl2Base):
     def __init__(self, poly=None, ind=None, u=None, dir=None, length=None, **kwargs):
        super().__init__("_polygon_step", {"poly" : poly, "ind" : ind, "u" : u, "dir" : dir, "length" : length, **kwargs})
 
-class _prism_fillet_prism(OpenSCADObject):
+class _prism_fillet_prism(_Bosl2Base):
     def __init__(self, name=None, basepoly=None, bot=None, top=None, d=None, k=None, N=None, overlap=None, uniform=None, debug=None, **kwargs):
        super().__init__("_prism_fillet_prism", {"name" : name, "basepoly" : basepoly, "bot" : bot, "top" : top, "d" : d, "k" : k, "N" : N, "overlap" : overlap, "uniform" : uniform, "debug" : debug, **kwargs})
 
+class round_corners(_Bosl2Base):
+    def __init__(self, path=None, method=None, radius=None, r=None, cut=None, joint=None, width=None, k=None, closed=None, verbose=None, **kwargs):
+       super().__init__("round_corners", {"path" : path, "method" : method, "radius" : radius, "r" : r, "cut" : cut, "joint" : joint, "width" : width, "k" : k, "closed" : closed, "verbose" : verbose, **kwargs})
+
+class smooth_path(_Bosl2Base):
+    def __init__(self, path=None, tangents=None, size=None, relsize=None, splinesteps=None, uniform=None, closed=None, **kwargs):
+       super().__init__("smooth_path", {"path" : path, "tangents" : tangents, "size" : size, "relsize" : relsize, "splinesteps" : splinesteps, "uniform" : uniform, "closed" : closed, **kwargs})
+
+class path_join(_Bosl2Base):
+    def __init__(self, paths=None, joint=None, k=None, relocate=None, closed=None, **kwargs):
+       super().__init__("path_join", {"paths" : paths, "joint" : joint, "k" : k, "relocate" : relocate, "closed" : closed, **kwargs})
+
+class offset_stroke(_Bosl2Base):
+    def __init__(self, path=None, width=None, rounded=None, start=None, end=None, check_valid=None, quality=None, chamfer=None, closed=None, **kwargs):
+       super().__init__("offset_stroke", {"path" : path, "width" : width, "rounded" : rounded, "start" : start, "end" : end, "check_valid" : check_valid, "quality" : quality, "chamfer" : chamfer, "closed" : closed, **kwargs})
+
+class offset_sweep(_Bosl2Base):
+    def __init__(self, path=None, height=None, bottom=None, top=None, h=None, l=None, offset=None, r=None, steps=None, quality=None, check_valid=None, extra=None, cut=None, chamfer_width=None, chamfer_height=None, joint=None, k=None, angle=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
+       super().__init__("offset_sweep", {"path" : path, "height" : height, "bottom" : bottom, "top" : top, "h" : h, "l" : l, "offset" : offset, "r" : r, "steps" : steps, "quality" : quality, "check_valid" : check_valid, "extra" : extra, "cut" : cut, "chamfer_width" : chamfer_width, "chamfer_height" : chamfer_height, "joint" : joint, "k" : k, "angle" : angle, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
+
+class convex_offset_extrude(_Bosl2Base):
+    def __init__(self, height=None, bottom=None, top=None, h=None, l=None, length=None, offset=None, r=None, steps=None, extra=None, cut=None, chamfer_width=None, chamfer_height=None, joint=None, k=None, angle=None, convexity=None, thickness=None, **kwargs):
+       super().__init__("convex_offset_extrude", {"height" : height, "bottom" : bottom, "top" : top, "h" : h, "l" : l, "length" : length, "offset" : offset, "r" : r, "steps" : steps, "extra" : extra, "cut" : cut, "chamfer_width" : chamfer_width, "chamfer_height" : chamfer_height, "joint" : joint, "k" : k, "angle" : angle, "convexity" : convexity, "thickness" : thickness, **kwargs})
+
+class rounded_prism(_Bosl2Base):
+    def __init__(self, bottom=None, top=None, joint_bot=None, joint_top=None, joint_sides=None, k_bot=None, k_top=None, k_sides=None, k=None, splinesteps=None, h=None, length=None, l=None, height=None, convexity=None, debug=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
+       super().__init__("rounded_prism", {"bottom" : bottom, "top" : top, "joint_bot" : joint_bot, "joint_top" : joint_top, "joint_sides" : joint_sides, "k_bot" : k_bot, "k_top" : k_top, "k_sides" : k_sides, "k" : k, "splinesteps" : splinesteps, "h" : h, "length" : length, "l" : l, "height" : height, "convexity" : convexity, "debug" : debug, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
+
+class bent_cutout_mask(_Bosl2Base):
+    def __init__(self, r=None, thickness=None, path=None, radius=None, convexity=None, **kwargs):
+       super().__init__("bent_cutout_mask", {"r" : r, "thickness" : thickness, "path" : path, "radius" : radius, "convexity" : convexity, **kwargs})
+
+class join_prism(_Bosl2Base):
+    def __init__(self, polygon=None, base=None, base_r=None, base_d=None, base_T=None, scale=None, prism_end_T=None, short=None, length=None, l=None, height=None, h=None, aux=None, aux_T=None, aux_r=None, aux_d=None, overlap=None, base_overlap=None, aux_overlap=None, n=None, base_n=None, end_n=None, aux_n=None, fillet=None, base_fillet=None, aux_fillet=None, end_round=None, k=None, base_k=None, aux_k=None, end_k=None, uniform=None, base_uniform=None, aux_uniform=None, debug=None, anchor=None, extent=None, cp=None, atype=None, orient=None, spin=None, convexity=None, **kwargs):
+       super().__init__("join_prism", {"polygon" : polygon, "base" : base, "base_r" : base_r, "base_d" : base_d, "base_T" : base_T, "scale" : scale, "prism_end_T" : prism_end_T, "short" : short, "length" : length, "l" : l, "height" : height, "h" : h, "aux" : aux, "aux_T" : aux_T, "aux_r" : aux_r, "aux_d" : aux_d, "overlap" : overlap, "base_overlap" : base_overlap, "aux_overlap" : aux_overlap, "n" : n, "base_n" : base_n, "end_n" : end_n, "aux_n" : aux_n, "fillet" : fillet, "base_fillet" : base_fillet, "aux_fillet" : aux_fillet, "end_round" : end_round, "k" : k, "base_k" : base_k, "aux_k" : aux_k, "end_k" : end_k, "uniform" : uniform, "base_uniform" : base_uniform, "aux_uniform" : aux_uniform, "debug" : debug, "anchor" : anchor, "extent" : extent, "cp" : cp, "atype" : atype, "orient" : orient, "spin" : spin, "convexity" : convexity, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/screw_drive.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/screw_drive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/screw_drive.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class phillips_mask(OpenSCADObject):
-    def __init__(self, size=None, _fn=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("phillips_mask", {"size" : size, "_fn" : _fn, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class torx_mask(OpenSCADObject):
-    def __init__(self, size=None, l=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("torx_mask", {"size" : size, "l" : l, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class torx_mask2d(OpenSCADObject):
-    def __init__(self, size=None, **kwargs):
-       super().__init__("torx_mask2d", {"size" : size, **kwargs})
-
-class robertson_mask(OpenSCADObject):
-    def __init__(self, size=None, extra=None, ang=None, **kwargs):
-       super().__init__("robertson_mask", {"size" : size, "extra" : extra, "ang" : ang, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/screw_drive.scad'}", use_not_include=False)
 
-class _phillips_shaft(OpenSCADObject):
+class _phillips_shaft(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("_phillips_shaft", {"x" : x, **kwargs})
 
-class _ph_bot_angle(OpenSCADObject):
+class _ph_bot_angle(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("_ph_bot_angle", {**kwargs})
 
-class _ph_side_angle(OpenSCADObject):
+class _ph_side_angle(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("_ph_side_angle", {**kwargs})
 
-class phillips_depth(OpenSCADObject):
+class phillips_depth(_Bosl2Base):
     def __init__(self, size=None, d=None, **kwargs):
        super().__init__("phillips_depth", {"size" : size, "d" : d, **kwargs})
 
-class phillips_diam(OpenSCADObject):
+class phillips_diam(_Bosl2Base):
     def __init__(self, size=None, depth=None, **kwargs):
        super().__init__("phillips_diam", {"size" : size, "depth" : depth, **kwargs})
 
-class torx_diam(OpenSCADObject):
+class torx_diam(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("torx_diam", {"size" : size, **kwargs})
 
-class _torx_inner_diam(OpenSCADObject):
+class _torx_inner_diam(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("_torx_inner_diam", {"size" : size, **kwargs})
 
-class torx_depth(OpenSCADObject):
+class torx_depth(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("torx_depth", {"size" : size, **kwargs})
 
-class _torx_tip_radius(OpenSCADObject):
+class _torx_tip_radius(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("_torx_tip_radius", {"size" : size, **kwargs})
 
-class _torx_rounding_radius(OpenSCADObject):
+class _torx_rounding_radius(_Bosl2Base):
     def __init__(self, size=None, **kwargs):
        super().__init__("_torx_rounding_radius", {"size" : size, **kwargs})
 
+class phillips_mask(_Bosl2Base):
+    def __init__(self, size=None, _fn=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("phillips_mask", {"size" : size, "_fn" : _fn, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class torx_mask(_Bosl2Base):
+    def __init__(self, size=None, l=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("torx_mask", {"size" : size, "l" : l, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class torx_mask2d(_Bosl2Base):
+    def __init__(self, size=None, **kwargs):
+       super().__init__("torx_mask2d", {"size" : size, **kwargs})
+
+class robertson_mask(_Bosl2Base):
+    def __init__(self, size=None, extra=None, ang=None, **kwargs):
+       super().__init__("robertson_mask", {"size" : size, "extra" : extra, "ang" : ang, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/screws.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/screws.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/screws.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class screw(OpenSCADObject):
-    def __init__(self, name=None, head=None, drive=None, thread=None, drive_size=None, oversize=None, spec=None, length=None, l=None, shank=None, tolerance=None, details=None, anchor=None, anchor_head=None, spin=None, orient=None, **kwargs):
-       super().__init__("screw", {"name" : name, "head" : head, "drive" : drive, "thread" : thread, "drive_size" : drive_size, "oversize" : oversize, "spec" : spec, "length" : length, "l" : l, "shank" : shank, "tolerance" : tolerance, "details" : details, "anchor" : anchor, "anchor_head" : anchor_head, "spin" : spin, "orient" : orient, **kwargs})
-
-class _driver(OpenSCADObject):
-    def __init__(self, spec=None, **kwargs):
-       super().__init__("_driver", {"spec" : spec, **kwargs})
-
-class _rod(OpenSCADObject):
-    def __init__(self, spec=None, length=None, tolerance=None, orient=None, spin=None, anchor=None, **kwargs):
-       super().__init__("_rod", {"spec" : spec, "length" : length, "tolerance" : tolerance, "orient" : orient, "spin" : spin, "anchor" : anchor, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/screws.scad'}", use_not_include=False)
 
-class nut(OpenSCADObject):
-    def __init__(self, name=None, diameter=None, thickness=None, thread=None, oversize=None, spec=None, tolerance=None, bevel=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("nut", {"name" : name, "diameter" : diameter, "thickness" : thickness, "thread" : thread, "oversize" : oversize, "spec" : spec, "tolerance" : tolerance, "bevel" : bevel, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class screw_head(OpenSCADObject):
-    def __init__(self, screw_info=None, details=None, **kwargs):
-       super().__init__("screw_head", {"screw_info" : screw_info, "details" : details, **kwargs})
-
-class screw(OpenSCADObject):
+class screw(_Bosl2Base):
     def __init__(self, name=None, head=None, drive=None, thread=None, drive_size=None, oversize=None, spec=None, length=None, l=None, shank=None, tolerance=None, details=None, anchor=None, anchor_head=None, spin=None, orient=None, **kwargs):
        super().__init__("screw", {"name" : name, "head" : head, "drive" : drive, "thread" : thread, "drive_size" : drive_size, "oversize" : oversize, "spec" : spec, "length" : length, "l" : l, "shank" : shank, "tolerance" : tolerance, "details" : details, "anchor" : anchor, "anchor_head" : anchor_head, "spin" : spin, "orient" : orient, **kwargs})
 
-class _ISO_thread_tolerance(OpenSCADObject):
+class _ISO_thread_tolerance(_Bosl2Base):
     def __init__(self, diameter=None, pitch=None, internal=None, tolerance=None, **kwargs):
        super().__init__("_ISO_thread_tolerance", {"diameter" : diameter, "pitch" : pitch, "internal" : internal, "tolerance" : tolerance, **kwargs})
 
-class _UTS_thread_tolerance(OpenSCADObject):
+class _UTS_thread_tolerance(_Bosl2Base):
     def __init__(self, diam=None, pitch=None, internal=None, tolerance=None, **kwargs):
        super().__init__("_UTS_thread_tolerance", {"diam" : diam, "pitch" : pitch, "internal" : internal, "tolerance" : tolerance, **kwargs})
 
-class _exact_thread_tolerance(OpenSCADObject):
+class _exact_thread_tolerance(_Bosl2Base):
     def __init__(self, d=None, P=None, **kwargs):
        super().__init__("_exact_thread_tolerance", {"d" : d, "P" : P, **kwargs})
 
-class nut(OpenSCADObject):
+class nut(_Bosl2Base):
     def __init__(self, name=None, diameter=None, thickness=None, thread=None, oversize=None, spec=None, tolerance=None, bevel=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("nut", {"name" : name, "diameter" : diameter, "thickness" : thickness, "thread" : thread, "oversize" : oversize, "spec" : spec, "tolerance" : tolerance, "bevel" : bevel, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class _parse_screw_name(OpenSCADObject):
+class _parse_screw_name(_Bosl2Base):
     def __init__(self, name=None, **kwargs):
        super().__init__("_parse_screw_name", {"name" : name, **kwargs})
 
-class _parse_drive(OpenSCADObject):
+class _parse_drive(_Bosl2Base):
     def __init__(self, drive=None, drive_size=None, **kwargs):
        super().__init__("_parse_drive", {"drive" : drive, "drive_size" : drive_size, **kwargs})
 
-class screw_head(OpenSCADObject):
+class screw_head(_Bosl2Base):
     def __init__(self, screw_info=None, details=None, **kwargs):
        super().__init__("screw_head", {"screw_info" : screw_info, "details" : details, **kwargs})
 
-class screw_info(OpenSCADObject):
+class screw_info(_Bosl2Base):
     def __init__(self, name=None, head=None, drive=None, thread=None, drive_size=None, oversize=None, **kwargs):
        super().__init__("screw_info", {"name" : name, "head" : head, "drive" : drive, "thread" : thread, "drive_size" : drive_size, "oversize" : oversize, **kwargs})
 
-class _screw_info_english(OpenSCADObject):
+class _screw_info_english(_Bosl2Base):
     def __init__(self, diam=None, threadcount=None, head=None, thread=None, drive=None, **kwargs):
        super().__init__("_screw_info_english", {"diam" : diam, "threadcount" : threadcount, "head" : head, "thread" : thread, "drive" : drive, **kwargs})
 
-class _screw_info_metric(OpenSCADObject):
+class _screw_info_metric(_Bosl2Base):
     def __init__(self, diam=None, pitch=None, head=None, thread=None, drive=None, **kwargs):
        super().__init__("_screw_info_metric", {"diam" : diam, "pitch" : pitch, "head" : head, "thread" : thread, "drive" : drive, **kwargs})
 
-class _is_positive(OpenSCADObject):
+class _is_positive(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("_is_positive", {"x" : x, **kwargs})
 
-class _validate_screw_spec(OpenSCADObject):
+class _validate_screw_spec(_Bosl2Base):
     def __init__(self, spec=None, **kwargs):
        super().__init__("_validate_screw_spec", {"spec" : spec, **kwargs})
 
-class thread_specification(OpenSCADObject):
+class thread_specification(_Bosl2Base):
     def __init__(self, screw_spec=None, tolerance=None, internal=None, **kwargs):
        super().__init__("thread_specification", {"screw_spec" : screw_spec, "tolerance" : tolerance, "internal" : internal, **kwargs})
 
+class screw(_Bosl2Base):
+    def __init__(self, name=None, head=None, drive=None, thread=None, drive_size=None, oversize=None, spec=None, length=None, l=None, shank=None, tolerance=None, details=None, anchor=None, anchor_head=None, spin=None, orient=None, **kwargs):
+       super().__init__("screw", {"name" : name, "head" : head, "drive" : drive, "thread" : thread, "drive_size" : drive_size, "oversize" : oversize, "spec" : spec, "length" : length, "l" : l, "shank" : shank, "tolerance" : tolerance, "details" : details, "anchor" : anchor, "anchor_head" : anchor_head, "spin" : spin, "orient" : orient, **kwargs})
+
+class _driver(_Bosl2Base):
+    def __init__(self, spec=None, **kwargs):
+       super().__init__("_driver", {"spec" : spec, **kwargs})
+
+class _rod(_Bosl2Base):
+    def __init__(self, spec=None, length=None, tolerance=None, orient=None, spin=None, anchor=None, **kwargs):
+       super().__init__("_rod", {"spec" : spec, "length" : length, "tolerance" : tolerance, "orient" : orient, "spin" : spin, "anchor" : anchor, **kwargs})
+
+class nut(_Bosl2Base):
+    def __init__(self, name=None, diameter=None, thickness=None, thread=None, oversize=None, spec=None, tolerance=None, bevel=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("nut", {"name" : name, "diameter" : diameter, "thickness" : thickness, "thread" : thread, "oversize" : oversize, "spec" : spec, "tolerance" : tolerance, "bevel" : bevel, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class screw_head(_Bosl2Base):
+    def __init__(self, screw_info=None, details=None, **kwargs):
+       super().__init__("screw_head", {"screw_info" : screw_info, "details" : details, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/shapes2d.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/shapes2d.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,166 +1,168 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/shapes2d.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class square(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/shapes2d.scad'}", use_not_include=False)
+
+class square(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, **kwargs):
        super().__init__("square", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class rect(OpenSCADObject):
-    def __init__(self, size=None, rounding=None, atype=None, chamfer=None, anchor=None, spin=None, **kwargs):
-       super().__init__("rect", {"size" : size, "rounding" : rounding, "atype" : atype, "chamfer" : chamfer, "anchor" : anchor, "spin" : spin, **kwargs})
+class rect(_Bosl2Base):
+    def __init__(self, size=None, rounding=None, chamfer=None, atype=None, anchor=None, spin=None, **kwargs):
+       super().__init__("rect", {"size" : size, "rounding" : rounding, "chamfer" : chamfer, "atype" : atype, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class circle(OpenSCADObject):
+class circle(_Bosl2Base):
     def __init__(self, r=None, d=None, points=None, corner=None, anchor=None, spin=None, **kwargs):
        super().__init__("circle", {"r" : r, "d" : d, "points" : points, "corner" : corner, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class ellipse(OpenSCADObject):
+class _ellipse_refine(_Bosl2Base):
+    def __init__(self, a=None, b=None, N=None, _theta=None, **kwargs):
+       super().__init__("_ellipse_refine", {"a" : a, "b" : b, "N" : N, "_theta" : _theta, **kwargs})
+
+class _ellipse_refine_realign(_Bosl2Base):
+    def __init__(self, a=None, b=None, N=None, _theta=None, i=None, **kwargs):
+       super().__init__("_ellipse_refine_realign", {"a" : a, "b" : b, "N" : N, "_theta" : _theta, "i" : i, **kwargs})
+
+class ellipse(_Bosl2Base):
     def __init__(self, r=None, d=None, realign=None, circum=None, uniform=None, anchor=None, spin=None, **kwargs):
        super().__init__("ellipse", {"r" : r, "d" : d, "realign" : realign, "circum" : circum, "uniform" : uniform, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class regular_ngon(OpenSCADObject):
-    def __init__(self, n=None, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, **kwargs):
-       super().__init__("regular_ngon", {"n" : n, "r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, **kwargs})
+class regular_ngon(_Bosl2Base):
+    def __init__(self, n=None, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, _mat=None, _anchs=None, **kwargs):
+       super().__init__("regular_ngon", {"n" : n, "r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, "_mat" : _mat, "_anchs" : _anchs, **kwargs})
 
-class pentagon(OpenSCADObject):
+class pentagon(_Bosl2Base):
     def __init__(self, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, **kwargs):
        super().__init__("pentagon", {"r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class hexagon(OpenSCADObject):
+class hexagon(_Bosl2Base):
     def __init__(self, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, **kwargs):
        super().__init__("hexagon", {"r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class octagon(OpenSCADObject):
+class octagon(_Bosl2Base):
     def __init__(self, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, **kwargs):
        super().__init__("octagon", {"r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class right_triangle(OpenSCADObject):
+class right_triangle(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, **kwargs):
        super().__init__("right_triangle", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class trapezoid(OpenSCADObject):
+class trapezoid(_Bosl2Base):
     def __init__(self, h=None, w1=None, w2=None, angle=None, shift=None, chamfer=None, rounding=None, flip=None, anchor=None, spin=None, **kwargs):
        super().__init__("trapezoid", {"h" : h, "w1" : w1, "w2" : w2, "angle" : angle, "shift" : shift, "chamfer" : chamfer, "rounding" : rounding, "flip" : flip, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class star(OpenSCADObject):
-    def __init__(self, n=None, r=None, ir=None, d=None, _or=None, od=None, id=None, step=None, realign=None, align_tip=None, align_pit=None, anchor=None, spin=None, atype=None, **kwargs):
-       super().__init__("star", {"n" : n, "r" : r, "ir" : ir, "d" : d, "_or" : _or, "od" : od, "id" : id, "step" : step, "realign" : realign, "align_tip" : align_tip, "align_pit" : align_pit, "anchor" : anchor, "spin" : spin, "atype" : atype, **kwargs})
+class star(_Bosl2Base):
+    def __init__(self, n=None, r=None, ir=None, d=None, _or=None, od=None, id=None, step=None, realign=None, align_tip=None, align_pit=None, anchor=None, spin=None, atype=None, _mat=None, _anchs=None, **kwargs):
+       super().__init__("star", {"n" : n, "r" : r, "ir" : ir, "d" : d, "_or" : _or, "od" : od, "id" : id, "step" : step, "realign" : realign, "align_tip" : align_tip, "align_pit" : align_pit, "anchor" : anchor, "spin" : spin, "atype" : atype, "_mat" : _mat, "_anchs" : _anchs, **kwargs})
 
-class jittered_poly(OpenSCADObject):
-    def __init__(self, path=None, dist=None, **kwargs):
-       super().__init__("jittered_poly", {"path" : path, "dist" : dist, **kwargs})
+class _path_add_jitter(_Bosl2Base):
+    def __init__(self, path=None, dist=None, closed=None, **kwargs):
+       super().__init__("_path_add_jitter", {"path" : path, "dist" : dist, "closed" : closed, **kwargs})
 
-class teardrop2d(OpenSCADObject):
+class teardrop2d(_Bosl2Base):
     def __init__(self, r=None, ang=None, cap_h=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("teardrop2d", {"r" : r, "ang" : ang, "cap_h" : cap_h, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class egg(OpenSCADObject):
+class egg(_Bosl2Base):
     def __init__(self, length=None, r1=None, r2=None, R=None, d1=None, d2=None, D=None, anchor=None, spin=None, **kwargs):
        super().__init__("egg", {"length" : length, "r1" : r1, "r2" : r2, "R" : R, "d1" : d1, "d2" : d2, "D" : D, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class glued_circles(OpenSCADObject):
+class glued_circles(_Bosl2Base):
     def __init__(self, r=None, spread=None, tangent=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("glued_circles", {"r" : r, "spread" : spread, "tangent" : tangent, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class supershape(OpenSCADObject):
+class _superformula(_Bosl2Base):
+    def __init__(self, theta=None, m1=None, m2=None, n1=None, n2=None, n3=None, a=None, b=None, **kwargs):
+       super().__init__("_superformula", {"theta" : theta, "m1" : m1, "m2" : m2, "n1" : n1, "n2" : n2, "n3" : n3, "a" : a, "b" : b, **kwargs})
+
+class supershape(_Bosl2Base):
     def __init__(self, step=None, m1=None, m2=None, n1=None, n2=None, n3=None, a=None, b=None, r=None, d=None, anchor=None, spin=None, atype=None, **kwargs):
        super().__init__("supershape", {"step" : step, "m1" : m1, "m2" : m2, "n1" : n1, "n2" : n2, "n3" : n3, "a" : a, "b" : b, "r" : r, "d" : d, "anchor" : anchor, "spin" : spin, "atype" : atype, **kwargs})
 
-class reuleaux_polygon(OpenSCADObject):
+class reuleaux_polygon(_Bosl2Base):
     def __init__(self, n=None, r=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("reuleaux_polygon", {"n" : n, "r" : r, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class text(OpenSCADObject):
-    def __init__(self, text=None, size=None, font=None, halign=None, valign=None, spacing=None, direction=None, language=None, script=None, anchor=None, spin=None, **kwargs):
-       super().__init__("text", {"text" : text, "size" : size, "font" : font, "halign" : halign, "valign" : valign, "spacing" : spacing, "direction" : direction, "language" : language, "script" : script, "anchor" : anchor, "spin" : spin, **kwargs})
-
-class round2d(OpenSCADObject):
-    def __init__(self, r=None, _or=None, ir=None, **kwargs):
-       super().__init__("round2d", {"r" : r, "_or" : _or, "ir" : ir, **kwargs})
-
-class shell2d(OpenSCADObject):
-    def __init__(self, thickness=None, _or=None, ir=None, **kwargs):
-       super().__init__("shell2d", {"thickness" : thickness, "_or" : _or, "ir" : ir, **kwargs})
-
-class square(OpenSCADObject):
+class square(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, **kwargs):
        super().__init__("square", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class rect(OpenSCADObject):
-    def __init__(self, size=None, rounding=None, chamfer=None, atype=None, anchor=None, spin=None, **kwargs):
-       super().__init__("rect", {"size" : size, "rounding" : rounding, "chamfer" : chamfer, "atype" : atype, "anchor" : anchor, "spin" : spin, **kwargs})
+class rect(_Bosl2Base):
+    def __init__(self, size=None, rounding=None, atype=None, chamfer=None, anchor=None, spin=None, **kwargs):
+       super().__init__("rect", {"size" : size, "rounding" : rounding, "atype" : atype, "chamfer" : chamfer, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class circle(OpenSCADObject):
+class circle(_Bosl2Base):
     def __init__(self, r=None, d=None, points=None, corner=None, anchor=None, spin=None, **kwargs):
        super().__init__("circle", {"r" : r, "d" : d, "points" : points, "corner" : corner, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class _ellipse_refine(OpenSCADObject):
-    def __init__(self, a=None, b=None, N=None, _theta=None, **kwargs):
-       super().__init__("_ellipse_refine", {"a" : a, "b" : b, "N" : N, "_theta" : _theta, **kwargs})
-
-class _ellipse_refine_realign(OpenSCADObject):
-    def __init__(self, a=None, b=None, N=None, _theta=None, i=None, **kwargs):
-       super().__init__("_ellipse_refine_realign", {"a" : a, "b" : b, "N" : N, "_theta" : _theta, "i" : i, **kwargs})
-
-class ellipse(OpenSCADObject):
+class ellipse(_Bosl2Base):
     def __init__(self, r=None, d=None, realign=None, circum=None, uniform=None, anchor=None, spin=None, **kwargs):
        super().__init__("ellipse", {"r" : r, "d" : d, "realign" : realign, "circum" : circum, "uniform" : uniform, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class regular_ngon(OpenSCADObject):
-    def __init__(self, n=None, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, _mat=None, _anchs=None, **kwargs):
-       super().__init__("regular_ngon", {"n" : n, "r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, "_mat" : _mat, "_anchs" : _anchs, **kwargs})
+class regular_ngon(_Bosl2Base):
+    def __init__(self, n=None, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, **kwargs):
+       super().__init__("regular_ngon", {"n" : n, "r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class pentagon(OpenSCADObject):
+class pentagon(_Bosl2Base):
     def __init__(self, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, **kwargs):
        super().__init__("pentagon", {"r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class hexagon(OpenSCADObject):
+class hexagon(_Bosl2Base):
     def __init__(self, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, **kwargs):
        super().__init__("hexagon", {"r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class octagon(OpenSCADObject):
+class octagon(_Bosl2Base):
     def __init__(self, r=None, d=None, _or=None, od=None, ir=None, id=None, side=None, rounding=None, realign=None, align_tip=None, align_side=None, anchor=None, spin=None, **kwargs):
        super().__init__("octagon", {"r" : r, "d" : d, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "side" : side, "rounding" : rounding, "realign" : realign, "align_tip" : align_tip, "align_side" : align_side, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class right_triangle(OpenSCADObject):
+class right_triangle(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, **kwargs):
        super().__init__("right_triangle", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class trapezoid(OpenSCADObject):
+class trapezoid(_Bosl2Base):
     def __init__(self, h=None, w1=None, w2=None, angle=None, shift=None, chamfer=None, rounding=None, flip=None, anchor=None, spin=None, **kwargs):
        super().__init__("trapezoid", {"h" : h, "w1" : w1, "w2" : w2, "angle" : angle, "shift" : shift, "chamfer" : chamfer, "rounding" : rounding, "flip" : flip, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class star(OpenSCADObject):
-    def __init__(self, n=None, r=None, ir=None, d=None, _or=None, od=None, id=None, step=None, realign=None, align_tip=None, align_pit=None, anchor=None, spin=None, atype=None, _mat=None, _anchs=None, **kwargs):
-       super().__init__("star", {"n" : n, "r" : r, "ir" : ir, "d" : d, "_or" : _or, "od" : od, "id" : id, "step" : step, "realign" : realign, "align_tip" : align_tip, "align_pit" : align_pit, "anchor" : anchor, "spin" : spin, "atype" : atype, "_mat" : _mat, "_anchs" : _anchs, **kwargs})
+class star(_Bosl2Base):
+    def __init__(self, n=None, r=None, ir=None, d=None, _or=None, od=None, id=None, step=None, realign=None, align_tip=None, align_pit=None, anchor=None, spin=None, atype=None, **kwargs):
+       super().__init__("star", {"n" : n, "r" : r, "ir" : ir, "d" : d, "_or" : _or, "od" : od, "id" : id, "step" : step, "realign" : realign, "align_tip" : align_tip, "align_pit" : align_pit, "anchor" : anchor, "spin" : spin, "atype" : atype, **kwargs})
 
-class _path_add_jitter(OpenSCADObject):
-    def __init__(self, path=None, dist=None, closed=None, **kwargs):
-       super().__init__("_path_add_jitter", {"path" : path, "dist" : dist, "closed" : closed, **kwargs})
+class jittered_poly(_Bosl2Base):
+    def __init__(self, path=None, dist=None, **kwargs):
+       super().__init__("jittered_poly", {"path" : path, "dist" : dist, **kwargs})
 
-class teardrop2d(OpenSCADObject):
+class teardrop2d(_Bosl2Base):
     def __init__(self, r=None, ang=None, cap_h=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("teardrop2d", {"r" : r, "ang" : ang, "cap_h" : cap_h, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class egg(OpenSCADObject):
+class egg(_Bosl2Base):
     def __init__(self, length=None, r1=None, r2=None, R=None, d1=None, d2=None, D=None, anchor=None, spin=None, **kwargs):
        super().__init__("egg", {"length" : length, "r1" : r1, "r2" : r2, "R" : R, "d1" : d1, "d2" : d2, "D" : D, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class glued_circles(OpenSCADObject):
+class glued_circles(_Bosl2Base):
     def __init__(self, r=None, spread=None, tangent=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("glued_circles", {"r" : r, "spread" : spread, "tangent" : tangent, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
-class _superformula(OpenSCADObject):
-    def __init__(self, theta=None, m1=None, m2=None, n1=None, n2=None, n3=None, a=None, b=None, **kwargs):
-       super().__init__("_superformula", {"theta" : theta, "m1" : m1, "m2" : m2, "n1" : n1, "n2" : n2, "n3" : n3, "a" : a, "b" : b, **kwargs})
-
-class supershape(OpenSCADObject):
+class supershape(_Bosl2Base):
     def __init__(self, step=None, m1=None, m2=None, n1=None, n2=None, n3=None, a=None, b=None, r=None, d=None, anchor=None, spin=None, atype=None, **kwargs):
        super().__init__("supershape", {"step" : step, "m1" : m1, "m2" : m2, "n1" : n1, "n2" : n2, "n3" : n3, "a" : a, "b" : b, "r" : r, "d" : d, "anchor" : anchor, "spin" : spin, "atype" : atype, **kwargs})
 
-class reuleaux_polygon(OpenSCADObject):
+class reuleaux_polygon(_Bosl2Base):
     def __init__(self, n=None, r=None, d=None, anchor=None, spin=None, **kwargs):
        super().__init__("reuleaux_polygon", {"n" : n, "r" : r, "d" : d, "anchor" : anchor, "spin" : spin, **kwargs})
 
+class text(_Bosl2Base):
+    def __init__(self, text=None, size=None, font=None, halign=None, valign=None, spacing=None, direction=None, language=None, script=None, anchor=None, spin=None, **kwargs):
+       super().__init__("text", {"text" : text, "size" : size, "font" : font, "halign" : halign, "valign" : valign, "spacing" : spacing, "direction" : direction, "language" : language, "script" : script, "anchor" : anchor, "spin" : spin, **kwargs})
+
+class round2d(_Bosl2Base):
+    def __init__(self, r=None, _or=None, ir=None, **kwargs):
+       super().__init__("round2d", {"r" : r, "_or" : _or, "ir" : ir, **kwargs})
+
+class shell2d(_Bosl2Base):
+    def __init__(self, thickness=None, _or=None, ir=None, **kwargs):
+       super().__init__("shell2d", {"thickness" : thickness, "_or" : _or, "ir" : ir, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/shapes3d.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/shapes3d.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,174 +1,176 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/shapes3d.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class cube(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/shapes3d.scad'}", use_not_include=False)
+
+class cube(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cube", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cuboid(OpenSCADObject):
-    def __init__(self, size=None, p1=None, p2=None, chamfer=None, rounding=None, edges=None, _except=None, except_edges=None, trimcorners=None, teardrop=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("cuboid", {"size" : size, "p1" : p1, "p2" : p2, "chamfer" : chamfer, "rounding" : rounding, "edges" : edges, "_except" : _except, "except_edges" : except_edges, "trimcorners" : trimcorners, "teardrop" : teardrop, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class cuboid(_Bosl2Base):
+    def __init__(self, size=None, p1=None, p2=None, chamfer=None, rounding=None, edges=None, except_edges=None, trimcorners=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("cuboid", {"size" : size, "p1" : p1, "p2" : p2, "chamfer" : chamfer, "rounding" : rounding, "edges" : edges, "except_edges" : except_edges, "trimcorners" : trimcorners, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class prismoid(OpenSCADObject):
+class prismoid(_Bosl2Base):
     def __init__(self, size1=None, size2=None, h=None, shift=None, rounding=None, rounding1=None, rounding2=None, chamfer=None, chamfer1=None, chamfer2=None, l=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("prismoid", {"size1" : size1, "size2" : size2, "h" : h, "shift" : shift, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "l" : l, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class octahedron(OpenSCADObject):
+class octahedron(_Bosl2Base):
     def __init__(self, size=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("octahedron", {"size" : size, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rect_tube(OpenSCADObject):
+class rect_tube(_Bosl2Base):
     def __init__(self, h=None, size=None, isize=None, center=None, shift=None, wall=None, size1=None, size2=None, isize1=None, isize2=None, rounding=None, rounding1=None, rounding2=None, irounding=None, irounding1=None, irounding2=None, chamfer=None, chamfer1=None, chamfer2=None, ichamfer=None, ichamfer1=None, ichamfer2=None, anchor=None, spin=None, orient=None, l=None, **kwargs):
        super().__init__("rect_tube", {"h" : h, "size" : size, "isize" : isize, "center" : center, "shift" : shift, "wall" : wall, "size1" : size1, "size2" : size2, "isize1" : isize1, "isize2" : isize2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "irounding" : irounding, "irounding1" : irounding1, "irounding2" : irounding2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "ichamfer" : ichamfer, "ichamfer1" : ichamfer1, "ichamfer2" : ichamfer2, "anchor" : anchor, "spin" : spin, "orient" : orient, "l" : l, **kwargs})
 
-class wedge(OpenSCADObject):
+class wedge(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("wedge", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cylinder(OpenSCADObject):
+class cylinder(_Bosl2Base):
     def __init__(self, h=None, r1=None, r2=None, center=None, l=None, r=None, d=None, d1=None, d2=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cylinder", {"h" : h, "r1" : r1, "r2" : r2, "center" : center, "l" : l, "r" : r, "d" : d, "d1" : d1, "d2" : d2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cyl(OpenSCADObject):
-    def __init__(self, h=None, r=None, center=None, l=None, r1=None, r2=None, d=None, d1=None, d2=None, chamfer=None, chamfer1=None, chamfer2=None, chamfang=None, chamfang1=None, chamfang2=None, rounding=None, rounding1=None, rounding2=None, circum=None, realign=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("cyl", {"h" : h, "r" : r, "center" : center, "l" : l, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "chamfang" : chamfang, "chamfang1" : chamfang1, "chamfang2" : chamfang2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "circum" : circum, "realign" : realign, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class xcyl(OpenSCADObject):
-    def __init__(self, h=None, r=None, d=None, r1=None, r2=None, d1=None, d2=None, l=None, chamfer=None, chamfer1=None, chamfer2=None, chamfang=None, chamfang1=None, chamfang2=None, rounding=None, rounding1=None, rounding2=None, circum=None, realign=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("xcyl", {"h" : h, "r" : r, "d" : d, "r1" : r1, "r2" : r2, "d1" : d1, "d2" : d2, "l" : l, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "chamfang" : chamfang, "chamfang1" : chamfang1, "chamfang2" : chamfang2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "circum" : circum, "realign" : realign, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class ycyl(OpenSCADObject):
-    def __init__(self, h=None, r=None, d=None, r1=None, r2=None, d1=None, d2=None, l=None, chamfer=None, chamfer1=None, chamfer2=None, chamfang=None, chamfang1=None, chamfang2=None, rounding=None, rounding1=None, rounding2=None, circum=None, realign=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("ycyl", {"h" : h, "r" : r, "d" : d, "r1" : r1, "r2" : r2, "d1" : d1, "d2" : d2, "l" : l, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "chamfang" : chamfang, "chamfang1" : chamfang1, "chamfang2" : chamfang2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "circum" : circum, "realign" : realign, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class zcyl(OpenSCADObject):
-    def __init__(self, h=None, r=None, d=None, r1=None, r2=None, d1=None, d2=None, l=None, chamfer=None, chamfer1=None, chamfer2=None, chamfang=None, chamfang1=None, chamfang2=None, rounding=None, rounding1=None, rounding2=None, circum=None, realign=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("zcyl", {"h" : h, "r" : r, "d" : d, "r1" : r1, "r2" : r2, "d1" : d1, "d2" : d2, "l" : l, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "chamfang" : chamfang, "chamfang1" : chamfang1, "chamfang2" : chamfang2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "circum" : circum, "realign" : realign, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class tube(OpenSCADObject):
-    def __init__(self, h=None, _or=None, ir=None, center=None, od=None, id=None, wall=None, or1=None, or2=None, od1=None, od2=None, ir1=None, ir2=None, id1=None, id2=None, realign=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("tube", {"h" : h, "_or" : _or, "ir" : ir, "center" : center, "od" : od, "id" : id, "wall" : wall, "or1" : or1, "or2" : or2, "od1" : od1, "od2" : od2, "ir1" : ir1, "ir2" : ir2, "id1" : id1, "id2" : id2, "realign" : realign, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class pie_slice(OpenSCADObject):
+class pie_slice(_Bosl2Base):
     def __init__(self, h=None, r=None, ang=None, center=None, r1=None, r2=None, d=None, d1=None, d2=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pie_slice", {"h" : h, "r" : r, "ang" : ang, "center" : center, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class sphere(OpenSCADObject):
+class sphere(_Bosl2Base):
     def __init__(self, r=None, d=None, circum=None, style=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("sphere", {"r" : r, "d" : d, "circum" : circum, "style" : style, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class spheroid(OpenSCADObject):
-    def __init__(self, r=None, style=None, d=None, circum=None, dual=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("spheroid", {"r" : r, "style" : style, "d" : d, "circum" : circum, "dual" : dual, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class _subsample_triangle(_Bosl2Base):
+    def __init__(self, p=None, N=None, **kwargs):
+       super().__init__("_subsample_triangle", {"p" : p, "N" : N, **kwargs})
 
-class torus(OpenSCADObject):
+class _dual_vertices(_Bosl2Base):
+    def __init__(self, vnf=None, **kwargs):
+       super().__init__("_dual_vertices", {"vnf" : vnf, **kwargs})
+
+class spheroid(_Bosl2Base):
+    def __init__(self, r=None, style=None, d=None, circum=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("spheroid", {"r" : r, "style" : style, "d" : d, "circum" : circum, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class torus(_Bosl2Base):
     def __init__(self, r_maj=None, r_min=None, center=None, d_maj=None, d_min=None, _or=None, od=None, ir=None, id=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("torus", {"r_maj" : r_maj, "r_min" : r_min, "center" : center, "d_maj" : d_maj, "d_min" : d_min, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class teardrop(OpenSCADObject):
+class teardrop(_Bosl2Base):
     def __init__(self, h=None, r=None, ang=None, cap_h=None, r1=None, r2=None, d=None, d1=None, d2=None, cap_h1=None, cap_h2=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("teardrop", {"h" : h, "r" : r, "ang" : ang, "cap_h" : cap_h, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "cap_h1" : cap_h1, "cap_h2" : cap_h2, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class onion(OpenSCADObject):
+class onion(_Bosl2Base):
     def __init__(self, r=None, ang=None, cap_h=None, d=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("onion", {"r" : r, "ang" : ang, "cap_h" : cap_h, "d" : d, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class text3d(OpenSCADObject):
-    def __init__(self, text=None, h=None, size=None, font=None, halign=None, valign=None, spacing=None, direction=None, language=None, script=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("text3d", {"text" : text, "h" : h, "size" : size, "font" : font, "halign" : halign, "valign" : valign, "spacing" : spacing, "direction" : direction, "language" : language, "script" : script, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class path_text(OpenSCADObject):
-    def __init__(self, path=None, text=None, font=None, size=None, thickness=None, lettersize=None, offset=None, reverse=None, normal=None, top=None, center=None, textmetrics=None, kern=None, **kwargs):
-       super().__init__("path_text", {"path" : path, "text" : text, "font" : font, "size" : size, "thickness" : thickness, "lettersize" : lettersize, "offset" : offset, "reverse" : reverse, "normal" : normal, "top" : top, "center" : center, "textmetrics" : textmetrics, "kern" : kern, **kwargs})
-
-class interior_fillet(OpenSCADObject):
-    def __init__(self, l=None, r=None, ang=None, overlap=None, d=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("interior_fillet", {"l" : l, "r" : r, "ang" : ang, "overlap" : overlap, "d" : d, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class heightfield(OpenSCADObject):
-    def __init__(self, data=None, size=None, bottom=None, maxz=None, xrange=None, yrange=None, style=None, convexity=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("heightfield", {"data" : data, "size" : size, "bottom" : bottom, "maxz" : maxz, "xrange" : xrange, "yrange" : yrange, "style" : style, "convexity" : convexity, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class _cut_interp(_Bosl2Base):
+    def __init__(self, pathcut=None, path=None, data=None, **kwargs):
+       super().__init__("_cut_interp", {"pathcut" : pathcut, "path" : path, "data" : data, **kwargs})
 
-class cylindrical_heightfield(OpenSCADObject):
-    def __init__(self, data=None, l=None, r=None, base=None, transpose=None, aspect=None, style=None, convexity=None, xrange=None, yrange=None, maxh=None, r1=None, r2=None, d=None, d1=None, d2=None, h=None, height=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("cylindrical_heightfield", {"data" : data, "l" : l, "r" : r, "base" : base, "transpose" : transpose, "aspect" : aspect, "style" : style, "convexity" : convexity, "xrange" : xrange, "yrange" : yrange, "maxh" : maxh, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "h" : h, "height" : height, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class heightfield(_Bosl2Base):
+    def __init__(self, data=None, size=None, bottom=None, maxz=None, xrange=None, yrange=None, style=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("heightfield", {"data" : data, "size" : size, "bottom" : bottom, "maxz" : maxz, "xrange" : xrange, "yrange" : yrange, "style" : style, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class ruler(OpenSCADObject):
-    def __init__(self, length=None, width=None, thickness=None, depth=None, labels=None, pipscale=None, maxscale=None, colors=None, alpha=None, unit=None, inch=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("ruler", {"length" : length, "width" : width, "thickness" : thickness, "depth" : depth, "labels" : labels, "pipscale" : pipscale, "maxscale" : maxscale, "colors" : colors, "alpha" : alpha, "unit" : unit, "inch" : inch, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class cylindrical_heightfield(_Bosl2Base):
+    def __init__(self, data=None, l=None, r=None, base=None, transpose=None, aspect=None, style=None, maxh=None, xrange=None, yrange=None, r1=None, r2=None, d=None, d1=None, d2=None, h=None, height=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("cylindrical_heightfield", {"data" : data, "l" : l, "r" : r, "base" : base, "transpose" : transpose, "aspect" : aspect, "style" : style, "maxh" : maxh, "xrange" : xrange, "yrange" : yrange, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "h" : h, "height" : height, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cube(OpenSCADObject):
+class cube(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cube", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cuboid(OpenSCADObject):
-    def __init__(self, size=None, p1=None, p2=None, chamfer=None, rounding=None, edges=None, except_edges=None, trimcorners=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("cuboid", {"size" : size, "p1" : p1, "p2" : p2, "chamfer" : chamfer, "rounding" : rounding, "edges" : edges, "except_edges" : except_edges, "trimcorners" : trimcorners, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class cuboid(_Bosl2Base):
+    def __init__(self, size=None, p1=None, p2=None, chamfer=None, rounding=None, edges=None, _except=None, except_edges=None, trimcorners=None, teardrop=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("cuboid", {"size" : size, "p1" : p1, "p2" : p2, "chamfer" : chamfer, "rounding" : rounding, "edges" : edges, "_except" : _except, "except_edges" : except_edges, "trimcorners" : trimcorners, "teardrop" : teardrop, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class prismoid(OpenSCADObject):
+class prismoid(_Bosl2Base):
     def __init__(self, size1=None, size2=None, h=None, shift=None, rounding=None, rounding1=None, rounding2=None, chamfer=None, chamfer1=None, chamfer2=None, l=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("prismoid", {"size1" : size1, "size2" : size2, "h" : h, "shift" : shift, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "l" : l, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class octahedron(OpenSCADObject):
+class octahedron(_Bosl2Base):
     def __init__(self, size=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("octahedron", {"size" : size, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rect_tube(OpenSCADObject):
+class rect_tube(_Bosl2Base):
     def __init__(self, h=None, size=None, isize=None, center=None, shift=None, wall=None, size1=None, size2=None, isize1=None, isize2=None, rounding=None, rounding1=None, rounding2=None, irounding=None, irounding1=None, irounding2=None, chamfer=None, chamfer1=None, chamfer2=None, ichamfer=None, ichamfer1=None, ichamfer2=None, anchor=None, spin=None, orient=None, l=None, **kwargs):
        super().__init__("rect_tube", {"h" : h, "size" : size, "isize" : isize, "center" : center, "shift" : shift, "wall" : wall, "size1" : size1, "size2" : size2, "isize1" : isize1, "isize2" : isize2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "irounding" : irounding, "irounding1" : irounding1, "irounding2" : irounding2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "ichamfer" : ichamfer, "ichamfer1" : ichamfer1, "ichamfer2" : ichamfer2, "anchor" : anchor, "spin" : spin, "orient" : orient, "l" : l, **kwargs})
 
-class wedge(OpenSCADObject):
+class wedge(_Bosl2Base):
     def __init__(self, size=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("wedge", {"size" : size, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class cylinder(OpenSCADObject):
+class cylinder(_Bosl2Base):
     def __init__(self, h=None, r1=None, r2=None, center=None, l=None, r=None, d=None, d1=None, d2=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("cylinder", {"h" : h, "r1" : r1, "r2" : r2, "center" : center, "l" : l, "r" : r, "d" : d, "d1" : d1, "d2" : d2, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class pie_slice(OpenSCADObject):
+class cyl(_Bosl2Base):
+    def __init__(self, h=None, r=None, center=None, l=None, r1=None, r2=None, d=None, d1=None, d2=None, chamfer=None, chamfer1=None, chamfer2=None, chamfang=None, chamfang1=None, chamfang2=None, rounding=None, rounding1=None, rounding2=None, circum=None, realign=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("cyl", {"h" : h, "r" : r, "center" : center, "l" : l, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "chamfang" : chamfang, "chamfang1" : chamfang1, "chamfang2" : chamfang2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "circum" : circum, "realign" : realign, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class xcyl(_Bosl2Base):
+    def __init__(self, h=None, r=None, d=None, r1=None, r2=None, d1=None, d2=None, l=None, chamfer=None, chamfer1=None, chamfer2=None, chamfang=None, chamfang1=None, chamfang2=None, rounding=None, rounding1=None, rounding2=None, circum=None, realign=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("xcyl", {"h" : h, "r" : r, "d" : d, "r1" : r1, "r2" : r2, "d1" : d1, "d2" : d2, "l" : l, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "chamfang" : chamfang, "chamfang1" : chamfang1, "chamfang2" : chamfang2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "circum" : circum, "realign" : realign, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class ycyl(_Bosl2Base):
+    def __init__(self, h=None, r=None, d=None, r1=None, r2=None, d1=None, d2=None, l=None, chamfer=None, chamfer1=None, chamfer2=None, chamfang=None, chamfang1=None, chamfang2=None, rounding=None, rounding1=None, rounding2=None, circum=None, realign=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("ycyl", {"h" : h, "r" : r, "d" : d, "r1" : r1, "r2" : r2, "d1" : d1, "d2" : d2, "l" : l, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "chamfang" : chamfang, "chamfang1" : chamfang1, "chamfang2" : chamfang2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "circum" : circum, "realign" : realign, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class zcyl(_Bosl2Base):
+    def __init__(self, h=None, r=None, d=None, r1=None, r2=None, d1=None, d2=None, l=None, chamfer=None, chamfer1=None, chamfer2=None, chamfang=None, chamfang1=None, chamfang2=None, rounding=None, rounding1=None, rounding2=None, circum=None, realign=None, from_end=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("zcyl", {"h" : h, "r" : r, "d" : d, "r1" : r1, "r2" : r2, "d1" : d1, "d2" : d2, "l" : l, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "chamfang" : chamfang, "chamfang1" : chamfang1, "chamfang2" : chamfang2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "circum" : circum, "realign" : realign, "from_end" : from_end, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class tube(_Bosl2Base):
+    def __init__(self, h=None, _or=None, ir=None, center=None, od=None, id=None, wall=None, or1=None, or2=None, od1=None, od2=None, ir1=None, ir2=None, id1=None, id2=None, realign=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("tube", {"h" : h, "_or" : _or, "ir" : ir, "center" : center, "od" : od, "id" : id, "wall" : wall, "or1" : or1, "or2" : or2, "od1" : od1, "od2" : od2, "ir1" : ir1, "ir2" : ir2, "id1" : id1, "id2" : id2, "realign" : realign, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class pie_slice(_Bosl2Base):
     def __init__(self, h=None, r=None, ang=None, center=None, r1=None, r2=None, d=None, d1=None, d2=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("pie_slice", {"h" : h, "r" : r, "ang" : ang, "center" : center, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class sphere(OpenSCADObject):
+class sphere(_Bosl2Base):
     def __init__(self, r=None, d=None, circum=None, style=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("sphere", {"r" : r, "d" : d, "circum" : circum, "style" : style, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class _subsample_triangle(OpenSCADObject):
-    def __init__(self, p=None, N=None, **kwargs):
-       super().__init__("_subsample_triangle", {"p" : p, "N" : N, **kwargs})
-
-class _dual_vertices(OpenSCADObject):
-    def __init__(self, vnf=None, **kwargs):
-       super().__init__("_dual_vertices", {"vnf" : vnf, **kwargs})
-
-class spheroid(OpenSCADObject):
-    def __init__(self, r=None, style=None, d=None, circum=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("spheroid", {"r" : r, "style" : style, "d" : d, "circum" : circum, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class spheroid(_Bosl2Base):
+    def __init__(self, r=None, style=None, d=None, circum=None, dual=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("spheroid", {"r" : r, "style" : style, "d" : d, "circum" : circum, "dual" : dual, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class torus(OpenSCADObject):
+class torus(_Bosl2Base):
     def __init__(self, r_maj=None, r_min=None, center=None, d_maj=None, d_min=None, _or=None, od=None, ir=None, id=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("torus", {"r_maj" : r_maj, "r_min" : r_min, "center" : center, "d_maj" : d_maj, "d_min" : d_min, "_or" : _or, "od" : od, "ir" : ir, "id" : id, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class teardrop(OpenSCADObject):
+class teardrop(_Bosl2Base):
     def __init__(self, h=None, r=None, ang=None, cap_h=None, r1=None, r2=None, d=None, d1=None, d2=None, cap_h1=None, cap_h2=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("teardrop", {"h" : h, "r" : r, "ang" : ang, "cap_h" : cap_h, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "cap_h1" : cap_h1, "cap_h2" : cap_h2, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class onion(OpenSCADObject):
+class onion(_Bosl2Base):
     def __init__(self, r=None, ang=None, cap_h=None, d=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("onion", {"r" : r, "ang" : ang, "cap_h" : cap_h, "d" : d, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class _cut_interp(OpenSCADObject):
-    def __init__(self, pathcut=None, path=None, data=None, **kwargs):
-       super().__init__("_cut_interp", {"pathcut" : pathcut, "path" : path, "data" : data, **kwargs})
+class text3d(_Bosl2Base):
+    def __init__(self, text=None, h=None, size=None, font=None, halign=None, valign=None, spacing=None, direction=None, language=None, script=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("text3d", {"text" : text, "h" : h, "size" : size, "font" : font, "halign" : halign, "valign" : valign, "spacing" : spacing, "direction" : direction, "language" : language, "script" : script, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class heightfield(OpenSCADObject):
-    def __init__(self, data=None, size=None, bottom=None, maxz=None, xrange=None, yrange=None, style=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("heightfield", {"data" : data, "size" : size, "bottom" : bottom, "maxz" : maxz, "xrange" : xrange, "yrange" : yrange, "style" : style, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class path_text(_Bosl2Base):
+    def __init__(self, path=None, text=None, font=None, size=None, thickness=None, lettersize=None, offset=None, reverse=None, normal=None, top=None, center=None, textmetrics=None, kern=None, **kwargs):
+       super().__init__("path_text", {"path" : path, "text" : text, "font" : font, "size" : size, "thickness" : thickness, "lettersize" : lettersize, "offset" : offset, "reverse" : reverse, "normal" : normal, "top" : top, "center" : center, "textmetrics" : textmetrics, "kern" : kern, **kwargs})
 
-class cylindrical_heightfield(OpenSCADObject):
-    def __init__(self, data=None, l=None, r=None, base=None, transpose=None, aspect=None, style=None, maxh=None, xrange=None, yrange=None, r1=None, r2=None, d=None, d1=None, d2=None, h=None, height=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("cylindrical_heightfield", {"data" : data, "l" : l, "r" : r, "base" : base, "transpose" : transpose, "aspect" : aspect, "style" : style, "maxh" : maxh, "xrange" : xrange, "yrange" : yrange, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "h" : h, "height" : height, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+class interior_fillet(_Bosl2Base):
+    def __init__(self, l=None, r=None, ang=None, overlap=None, d=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("interior_fillet", {"l" : l, "r" : r, "ang" : ang, "overlap" : overlap, "d" : d, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class heightfield(_Bosl2Base):
+    def __init__(self, data=None, size=None, bottom=None, maxz=None, xrange=None, yrange=None, style=None, convexity=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("heightfield", {"data" : data, "size" : size, "bottom" : bottom, "maxz" : maxz, "xrange" : xrange, "yrange" : yrange, "style" : style, "convexity" : convexity, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class cylindrical_heightfield(_Bosl2Base):
+    def __init__(self, data=None, l=None, r=None, base=None, transpose=None, aspect=None, style=None, convexity=None, xrange=None, yrange=None, maxh=None, r1=None, r2=None, d=None, d1=None, d2=None, h=None, height=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("cylindrical_heightfield", {"data" : data, "l" : l, "r" : r, "base" : base, "transpose" : transpose, "aspect" : aspect, "style" : style, "convexity" : convexity, "xrange" : xrange, "yrange" : yrange, "maxh" : maxh, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "h" : h, "height" : height, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class ruler(_Bosl2Base):
+    def __init__(self, length=None, width=None, thickness=None, depth=None, labels=None, pipscale=None, maxscale=None, colors=None, alpha=None, unit=None, inch=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("ruler", {"length" : length, "width" : width, "thickness" : thickness, "depth" : depth, "labels" : labels, "pipscale" : pipscale, "maxscale" : maxscale, "colors" : colors, "alpha" : alpha, "unit" : unit, "inch" : inch, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/skin.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/skin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,153 +1,155 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/skin.scad'}", use_not_include=False)
-
-_MAP_DIAG = OpenSCADConstant('_MAP_DIAG')
-_MAP_LEFT = OpenSCADConstant('_MAP_LEFT')
-_MAP_UP = OpenSCADConstant('_MAP_UP')
-class skin(OpenSCADObject):
-    def __init__(self, profiles=None, slices=None, refine=None, method=None, sampling=None, caps=None, closed=None, z=None, style=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
-       super().__init__("skin", {"profiles" : profiles, "slices" : slices, "refine" : refine, "method" : method, "sampling" : sampling, "caps" : caps, "closed" : closed, "z" : z, "style" : style, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
-
-class linear_sweep(OpenSCADObject):
-    def __init__(self, region=None, height=None, center=None, twist=None, scale=None, shift=None, slices=None, maxseg=None, style=None, convexity=None, cp=None, atype=None, h=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("linear_sweep", {"region" : region, "height" : height, "center" : center, "twist" : twist, "scale" : scale, "shift" : shift, "slices" : slices, "maxseg" : maxseg, "style" : style, "convexity" : convexity, "cp" : cp, "atype" : atype, "h" : h, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class spiral_sweep(OpenSCADObject):
-    def __init__(self, poly=None, h=None, r=None, turns=None, higbee=None, center=None, r1=None, r2=None, d=None, d1=None, d2=None, higbee1=None, higbee2=None, internal=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("spiral_sweep", {"poly" : poly, "h" : h, "r" : r, "turns" : turns, "higbee" : higbee, "center" : center, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "higbee1" : higbee1, "higbee2" : higbee2, "internal" : internal, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class path_sweep(OpenSCADObject):
-    def __init__(self, shape=None, path=None, method=None, normal=None, closed=None, twist=None, twist_by_length=None, symmetry=None, last_normal=None, tangent=None, uniform=None, relaxed=None, caps=None, style=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, profiles=None, width=None, **kwargs):
-       super().__init__("path_sweep", {"shape" : shape, "path" : path, "method" : method, "normal" : normal, "closed" : closed, "twist" : twist, "twist_by_length" : twist_by_length, "symmetry" : symmetry, "last_normal" : last_normal, "tangent" : tangent, "uniform" : uniform, "relaxed" : relaxed, "caps" : caps, "style" : style, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, "profiles" : profiles, "width" : width, **kwargs})
-
-class path_sweep2d(OpenSCADObject):
-    def __init__(self, profile=None, path=None, closed=None, caps=None, quality=None, style=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
-       super().__init__("path_sweep2d", {"profile" : profile, "path" : path, "closed" : closed, "caps" : caps, "quality" : quality, "style" : style, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
-
-class sweep(OpenSCADObject):
-    def __init__(self, shape=None, transforms=None, closed=None, caps=None, style=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
-       super().__init__("sweep", {"shape" : shape, "transforms" : transforms, "closed" : closed, "caps" : caps, "style" : style, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
-
-class textured_linear_sweep(OpenSCADObject):
-    def __init__(self, path=None, texture=None, tex_size=None, h=None, inset=None, rot=None, tscale=None, twist=None, scale=None, shift=None, style=None, reverse=None, l=None, counts=None, anchor=None, spin=None, orient=None, convexity=None, **kwargs):
-       super().__init__("textured_linear_sweep", {"path" : path, "texture" : texture, "tex_size" : tex_size, "h" : h, "inset" : inset, "rot" : rot, "tscale" : tscale, "twist" : twist, "scale" : scale, "shift" : shift, "style" : style, "reverse" : reverse, "l" : l, "counts" : counts, "anchor" : anchor, "spin" : spin, "orient" : orient, "convexity" : convexity, **kwargs})
-
-class textured_revolution(OpenSCADObject):
-    def __init__(self, path=None, texture=None, tex_size=None, tscale=None, inset=None, rot=None, caps=None, wrap=None, shift=None, style=None, reverse=None, atype=None, convexity=None, counts=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("textured_revolution", {"path" : path, "texture" : texture, "tex_size" : tex_size, "tscale" : tscale, "inset" : inset, "rot" : rot, "caps" : caps, "wrap" : wrap, "shift" : shift, "style" : style, "reverse" : reverse, "atype" : atype, "convexity" : convexity, "counts" : counts, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class textured_cylinder(OpenSCADObject):
-    def __init__(self, h=None, r=None, texture=None, tex_size=None, counts=None, tscale=None, inset=None, rot=None, style=None, reverse=None, shift=None, l=None, r1=None, r2=None, d=None, d1=None, d2=None, chamfer=None, chamfer1=None, chamfer2=None, rounding=None, rounding1=None, rounding2=None, convexity=None, anchor=None, spin=None, orient=None, **kwargs):
-       super().__init__("textured_cylinder", {"h" : h, "r" : r, "texture" : texture, "tex_size" : tex_size, "counts" : counts, "tscale" : tscale, "inset" : inset, "rot" : rot, "style" : style, "reverse" : reverse, "shift" : shift, "l" : l, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "convexity" : convexity, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
-
-class skin(OpenSCADObject):
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
+
+from .bosl2_base import Bosl2Base as _Bosl2Base
+
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/skin.scad'}", use_not_include=False)
+
+_MAP_DIAG = _OpenSCADConstant('_MAP_DIAG')
+_MAP_LEFT = _OpenSCADConstant('_MAP_LEFT')
+_MAP_UP = _OpenSCADConstant('_MAP_UP')
+class skin(_Bosl2Base):
     def __init__(self, profiles=None, slices=None, refine=None, method=None, sampling=None, caps=None, closed=None, z=None, style=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
        super().__init__("skin", {"profiles" : profiles, "slices" : slices, "refine" : refine, "method" : method, "sampling" : sampling, "caps" : caps, "closed" : closed, "z" : z, "style" : style, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
 
-class linear_sweep(OpenSCADObject):
+class linear_sweep(_Bosl2Base):
     def __init__(self, region=None, height=None, center=None, twist=None, scale=None, shift=None, slices=None, maxseg=None, style=None, cp=None, atype=None, h=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("linear_sweep", {"region" : region, "height" : height, "center" : center, "twist" : twist, "scale" : scale, "shift" : shift, "slices" : slices, "maxseg" : maxseg, "style" : style, "cp" : cp, "atype" : atype, "h" : h, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class _taperfunc(OpenSCADObject):
+class _taperfunc(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("_taperfunc", {"x" : x, **kwargs})
 
-class _ss_polygon_r(OpenSCADObject):
+class _ss_polygon_r(_Bosl2Base):
     def __init__(self, N=None, theta=None, **kwargs):
        super().__init__("_ss_polygon_r", {"N" : N, "theta" : theta, **kwargs})
 
-class spiral_sweep(OpenSCADObject):
+class spiral_sweep(_Bosl2Base):
     def __init__(self, poly=None, h=None, r=None, turns=None, higbee=None, center=None, r1=None, r2=None, d=None, d1=None, d2=None, higbee1=None, higbee2=None, internal=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("spiral_sweep", {"poly" : poly, "h" : h, "r" : r, "turns" : turns, "higbee" : higbee, "center" : center, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "higbee1" : higbee1, "higbee2" : higbee2, "internal" : internal, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class path_sweep(OpenSCADObject):
+class path_sweep(_Bosl2Base):
     def __init__(self, shape=None, path=None, method=None, normal=None, closed=None, twist=None, twist_by_length=None, symmetry=None, last_normal=None, tangent=None, uniform=None, relaxed=None, caps=None, style=None, transforms=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
        super().__init__("path_sweep", {"shape" : shape, "path" : path, "method" : method, "normal" : normal, "closed" : closed, "twist" : twist, "twist_by_length" : twist_by_length, "symmetry" : symmetry, "last_normal" : last_normal, "tangent" : tangent, "uniform" : uniform, "relaxed" : relaxed, "caps" : caps, "style" : style, "transforms" : transforms, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
 
-class path_sweep2d(OpenSCADObject):
+class path_sweep2d(_Bosl2Base):
     def __init__(self, shape=None, path=None, closed=None, caps=None, quality=None, style=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
        super().__init__("path_sweep2d", {"shape" : shape, "path" : path, "closed" : closed, "caps" : caps, "quality" : quality, "style" : style, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
 
-class _ofs_vmap(OpenSCADObject):
+class _ofs_vmap(_Bosl2Base):
     def __init__(self, ofs=None, closed=None, **kwargs):
        super().__init__("_ofs_vmap", {"ofs" : ofs, "closed" : closed, **kwargs})
 
-class _ofs_face_edge(OpenSCADObject):
+class _ofs_face_edge(_Bosl2Base):
     def __init__(self, face=None, firstlen=None, second=None, **kwargs):
        super().__init__("_ofs_face_edge", {"face" : face, "firstlen" : firstlen, "second" : second, **kwargs})
 
-class sweep(OpenSCADObject):
+class sweep(_Bosl2Base):
     def __init__(self, shape=None, transforms=None, closed=None, caps=None, style=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
        super().__init__("sweep", {"shape" : shape, "transforms" : transforms, "closed" : closed, "caps" : caps, "style" : style, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
 
-class subdivide_and_slice(OpenSCADObject):
+class subdivide_and_slice(_Bosl2Base):
     def __init__(self, profiles=None, slices=None, numpoints=None, method=None, closed=None, **kwargs):
        super().__init__("subdivide_and_slice", {"profiles" : profiles, "slices" : slices, "numpoints" : numpoints, "method" : method, "closed" : closed, **kwargs})
 
-class slice_profiles(OpenSCADObject):
+class slice_profiles(_Bosl2Base):
     def __init__(self, profiles=None, slices=None, closed=None, **kwargs):
        super().__init__("slice_profiles", {"profiles" : profiles, "slices" : slices, "closed" : closed, **kwargs})
 
-class _closest_angle(OpenSCADObject):
+class _closest_angle(_Bosl2Base):
     def __init__(self, alpha=None, beta=None, **kwargs):
        super().__init__("_closest_angle", {"alpha" : alpha, "beta" : beta, **kwargs})
 
-class _smooth(OpenSCADObject):
+class _smooth(_Bosl2Base):
     def __init__(self, data=None, len=None, closed=None, angle=None, **kwargs):
        super().__init__("_smooth", {"data" : data, "len" : len, "closed" : closed, "angle" : angle, **kwargs})
 
-class rot_resample(OpenSCADObject):
+class rot_resample(_Bosl2Base):
     def __init__(self, rotlist=None, n=None, twist=None, scale=None, smoothlen=None, long=None, turns=None, closed=None, method=None, **kwargs):
        super().__init__("rot_resample", {"rotlist" : rotlist, "n" : n, "twist" : twist, "scale" : scale, "smoothlen" : smoothlen, "long" : long, "turns" : turns, "closed" : closed, "method" : method, **kwargs})
 
-class _dp_distance_array(OpenSCADObject):
+class _dp_distance_array(_Bosl2Base):
     def __init__(self, small=None, big=None, abort_thresh=None, **kwargs):
        super().__init__("_dp_distance_array", {"small" : small, "big" : big, "abort_thresh" : abort_thresh, **kwargs})
 
-class _dp_distance_row(OpenSCADObject):
+class _dp_distance_row(_Bosl2Base):
     def __init__(self, small=None, big=None, small_ind=None, tdist=None, **kwargs):
        super().__init__("_dp_distance_row", {"small" : small, "big" : big, "small_ind" : small_ind, "tdist" : tdist, **kwargs})
 
-class _dp_extract_map(OpenSCADObject):
+class _dp_extract_map(_Bosl2Base):
     def __init__(self, map=None, **kwargs):
        super().__init__("_dp_extract_map", {"map" : map, **kwargs})
 
-class _skin_distance_match(OpenSCADObject):
+class _skin_distance_match(_Bosl2Base):
     def __init__(self, poly1=None, poly2=None, **kwargs):
        super().__init__("_skin_distance_match", {"poly1" : poly1, "poly2" : poly2, **kwargs})
 
-class _skin_aligned_distance_match(OpenSCADObject):
+class _skin_aligned_distance_match(_Bosl2Base):
     def __init__(self, poly1=None, poly2=None, **kwargs):
        super().__init__("_skin_aligned_distance_match", {"poly1" : poly1, "poly2" : poly2, **kwargs})
 
-class _skin_tangent_match(OpenSCADObject):
+class _skin_tangent_match(_Bosl2Base):
     def __init__(self, poly1=None, poly2=None, **kwargs):
        super().__init__("_skin_tangent_match", {"poly1" : poly1, "poly2" : poly2, **kwargs})
 
-class _find_one_tangent(OpenSCADObject):
+class _find_one_tangent(_Bosl2Base):
     def __init__(self, curve=None, edge=None, curve_offset=None, closed=None, **kwargs):
        super().__init__("_find_one_tangent", {"curve" : curve, "edge" : edge, "curve_offset" : curve_offset, "closed" : closed, **kwargs})
 
-class associate_vertices(OpenSCADObject):
+class associate_vertices(_Bosl2Base):
     def __init__(self, polygons=None, split=None, curpoly=None, **kwargs):
        super().__init__("associate_vertices", {"polygons" : polygons, "split" : split, "curpoly" : curpoly, **kwargs})
 
-class _get_texture(OpenSCADObject):
+class _get_texture(_Bosl2Base):
     def __init__(self, tex=None, n=None, m=None, **kwargs):
        super().__init__("_get_texture", {"tex" : tex, "n" : n, "m" : m, **kwargs})
 
-class textured_linear_sweep(OpenSCADObject):
+class textured_linear_sweep(_Bosl2Base):
     def __init__(self, path=None, texture=None, tex_size=None, h=None, counts=None, inset=None, rot=None, tscale=None, caps=None, col_wrap=None, twist=None, scale=None, shift=None, style=None, reverse=None, l=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("textured_linear_sweep", {"path" : path, "texture" : texture, "tex_size" : tex_size, "h" : h, "counts" : counts, "inset" : inset, "rot" : rot, "tscale" : tscale, "caps" : caps, "col_wrap" : col_wrap, "twist" : twist, "scale" : scale, "shift" : shift, "style" : style, "reverse" : reverse, "l" : l, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class textured_revolution(OpenSCADObject):
+class textured_revolution(_Bosl2Base):
     def __init__(self, path=None, texture=None, tex_size=None, tscale=None, inset=None, rot=None, caps=None, wrap=None, shift=None, style=None, reverse=None, counts=None, **kwargs):
        super().__init__("textured_revolution", {"path" : path, "texture" : texture, "tex_size" : tex_size, "tscale" : tscale, "inset" : inset, "rot" : rot, "caps" : caps, "wrap" : wrap, "shift" : shift, "style" : style, "reverse" : reverse, "counts" : counts, **kwargs})
 
-class textured_cylinder(OpenSCADObject):
+class textured_cylinder(_Bosl2Base):
     def __init__(self, h=None, r=None, texture=None, tex_size=None, counts=None, tscale=None, inset=None, rot=None, caps=None, style=None, reverse=None, shift=None, l=None, r1=None, r2=None, d=None, d1=None, d2=None, chamfer=None, chamfer1=None, chamfer2=None, rounding=None, rounding1=None, rounding2=None, **kwargs):
        super().__init__("textured_cylinder", {"h" : h, "r" : r, "texture" : texture, "tex_size" : tex_size, "counts" : counts, "tscale" : tscale, "inset" : inset, "rot" : rot, "caps" : caps, "style" : style, "reverse" : reverse, "shift" : shift, "l" : l, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, **kwargs})
 
+class skin(_Bosl2Base):
+    def __init__(self, profiles=None, slices=None, refine=None, method=None, sampling=None, caps=None, closed=None, z=None, style=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
+       super().__init__("skin", {"profiles" : profiles, "slices" : slices, "refine" : refine, "method" : method, "sampling" : sampling, "caps" : caps, "closed" : closed, "z" : z, "style" : style, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
+
+class linear_sweep(_Bosl2Base):
+    def __init__(self, region=None, height=None, center=None, twist=None, scale=None, shift=None, slices=None, maxseg=None, style=None, convexity=None, cp=None, atype=None, h=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("linear_sweep", {"region" : region, "height" : height, "center" : center, "twist" : twist, "scale" : scale, "shift" : shift, "slices" : slices, "maxseg" : maxseg, "style" : style, "convexity" : convexity, "cp" : cp, "atype" : atype, "h" : h, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class spiral_sweep(_Bosl2Base):
+    def __init__(self, poly=None, h=None, r=None, turns=None, higbee=None, center=None, r1=None, r2=None, d=None, d1=None, d2=None, higbee1=None, higbee2=None, internal=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("spiral_sweep", {"poly" : poly, "h" : h, "r" : r, "turns" : turns, "higbee" : higbee, "center" : center, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "higbee1" : higbee1, "higbee2" : higbee2, "internal" : internal, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class path_sweep(_Bosl2Base):
+    def __init__(self, shape=None, path=None, method=None, normal=None, closed=None, twist=None, twist_by_length=None, symmetry=None, last_normal=None, tangent=None, uniform=None, relaxed=None, caps=None, style=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, profiles=None, width=None, **kwargs):
+       super().__init__("path_sweep", {"shape" : shape, "path" : path, "method" : method, "normal" : normal, "closed" : closed, "twist" : twist, "twist_by_length" : twist_by_length, "symmetry" : symmetry, "last_normal" : last_normal, "tangent" : tangent, "uniform" : uniform, "relaxed" : relaxed, "caps" : caps, "style" : style, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, "profiles" : profiles, "width" : width, **kwargs})
+
+class path_sweep2d(_Bosl2Base):
+    def __init__(self, profile=None, path=None, closed=None, caps=None, quality=None, style=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
+       super().__init__("path_sweep2d", {"profile" : profile, "path" : path, "closed" : closed, "caps" : caps, "quality" : quality, "style" : style, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
+
+class sweep(_Bosl2Base):
+    def __init__(self, shape=None, transforms=None, closed=None, caps=None, style=None, convexity=None, anchor=None, cp=None, spin=None, orient=None, atype=None, **kwargs):
+       super().__init__("sweep", {"shape" : shape, "transforms" : transforms, "closed" : closed, "caps" : caps, "style" : style, "convexity" : convexity, "anchor" : anchor, "cp" : cp, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
+
+class textured_linear_sweep(_Bosl2Base):
+    def __init__(self, path=None, texture=None, tex_size=None, h=None, inset=None, rot=None, tscale=None, twist=None, scale=None, shift=None, style=None, reverse=None, l=None, counts=None, anchor=None, spin=None, orient=None, convexity=None, **kwargs):
+       super().__init__("textured_linear_sweep", {"path" : path, "texture" : texture, "tex_size" : tex_size, "h" : h, "inset" : inset, "rot" : rot, "tscale" : tscale, "twist" : twist, "scale" : scale, "shift" : shift, "style" : style, "reverse" : reverse, "l" : l, "counts" : counts, "anchor" : anchor, "spin" : spin, "orient" : orient, "convexity" : convexity, **kwargs})
+
+class textured_revolution(_Bosl2Base):
+    def __init__(self, path=None, texture=None, tex_size=None, tscale=None, inset=None, rot=None, caps=None, wrap=None, shift=None, style=None, reverse=None, atype=None, convexity=None, counts=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("textured_revolution", {"path" : path, "texture" : texture, "tex_size" : tex_size, "tscale" : tscale, "inset" : inset, "rot" : rot, "caps" : caps, "wrap" : wrap, "shift" : shift, "style" : style, "reverse" : reverse, "atype" : atype, "convexity" : convexity, "counts" : counts, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
+class textured_cylinder(_Bosl2Base):
+    def __init__(self, h=None, r=None, texture=None, tex_size=None, counts=None, tscale=None, inset=None, rot=None, style=None, reverse=None, shift=None, l=None, r1=None, r2=None, d=None, d1=None, d2=None, chamfer=None, chamfer1=None, chamfer2=None, rounding=None, rounding1=None, rounding2=None, convexity=None, anchor=None, spin=None, orient=None, **kwargs):
+       super().__init__("textured_cylinder", {"h" : h, "r" : r, "texture" : texture, "tex_size" : tex_size, "counts" : counts, "tscale" : tscale, "inset" : inset, "rot" : rot, "style" : style, "reverse" : reverse, "shift" : shift, "l" : l, "r1" : r1, "r2" : r2, "d" : d, "d1" : d1, "d2" : d2, "chamfer" : chamfer, "chamfer1" : chamfer1, "chamfer2" : chamfer2, "rounding" : rounding, "rounding1" : rounding1, "rounding2" : rounding2, "convexity" : convexity, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/sliders.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/sliders.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/sliders.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class slider(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/sliders.scad'}", use_not_include=False)
+
+class slider(_Bosl2Base):
     def __init__(self, l=None, w=None, h=None, base=None, wall=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("slider", {"l" : l, "w" : w, "h" : h, "base" : base, "wall" : wall, "ang" : ang, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rail(OpenSCADObject):
+class rail(_Bosl2Base):
     def __init__(self, l=None, w=None, h=None, chamfer=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rail", {"l" : l, "w" : w, "h" : h, "chamfer" : chamfer, "ang" : ang, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class slider(OpenSCADObject):
+class slider(_Bosl2Base):
     def __init__(self, l=None, w=None, h=None, base=None, wall=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("slider", {"l" : l, "w" : w, "h" : h, "base" : base, "wall" : wall, "ang" : ang, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class rail(OpenSCADObject):
+class rail(_Bosl2Base):
     def __init__(self, l=None, w=None, h=None, chamfer=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("rail", {"l" : l, "w" : w, "h" : h, "chamfer" : chamfer, "ang" : ang, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/strings.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/comparisons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,158 +1,152 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/strings.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class substr(OpenSCADObject):
-    def __init__(self, str=None, pos=None, len=None, **kwargs):
-       super().__init__("substr", {"str" : str, "pos" : pos, "len" : len, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/comparisons.scad'}", use_not_include=False)
 
-class _substr(OpenSCADObject):
-    def __init__(self, str=None, pos=None, len=None, substr=None, **kwargs):
-       super().__init__("_substr", {"str" : str, "pos" : pos, "len" : len, "substr" : substr, **kwargs})
+class approx(_Bosl2Base):
+    def __init__(self, a=None, b=None, eps=None, **kwargs):
+       super().__init__("approx", {"a" : a, "b" : b, "eps" : eps, **kwargs})
 
-class suffix(OpenSCADObject):
-    def __init__(self, str=None, len=None, **kwargs):
-       super().__init__("suffix", {"str" : str, "len" : len, **kwargs})
+class all_zero(_Bosl2Base):
+    def __init__(self, x=None, eps=None, **kwargs):
+       super().__init__("all_zero", {"x" : x, "eps" : eps, **kwargs})
 
-class str_find(OpenSCADObject):
-    def __init__(self, str=None, pattern=None, start=None, last=None, all=None, **kwargs):
-       super().__init__("str_find", {"str" : str, "pattern" : pattern, "start" : start, "last" : last, "all" : all, **kwargs})
+class all_nonzero(_Bosl2Base):
+    def __init__(self, x=None, eps=None, **kwargs):
+       super().__init__("all_nonzero", {"x" : x, "eps" : eps, **kwargs})
 
-class _str_find_first(OpenSCADObject):
-    def __init__(self, str=None, pattern=None, max_sindex=None, sindex=None, **kwargs):
-       super().__init__("_str_find_first", {"str" : str, "pattern" : pattern, "max_sindex" : max_sindex, "sindex" : sindex, **kwargs})
+class all_positive(_Bosl2Base):
+    def __init__(self, x=None, eps=None, **kwargs):
+       super().__init__("all_positive", {"x" : x, "eps" : eps, **kwargs})
 
-class _str_find_last(OpenSCADObject):
-    def __init__(self, str=None, pattern=None, sindex=None, **kwargs):
-       super().__init__("_str_find_last", {"str" : str, "pattern" : pattern, "sindex" : sindex, **kwargs})
+class all_negative(_Bosl2Base):
+    def __init__(self, x=None, eps=None, **kwargs):
+       super().__init__("all_negative", {"x" : x, "eps" : eps, **kwargs})
 
-class _str_find_all(OpenSCADObject):
-    def __init__(self, str=None, pattern=None, **kwargs):
-       super().__init__("_str_find_all", {"str" : str, "pattern" : pattern, **kwargs})
+class all_nonpositive(_Bosl2Base):
+    def __init__(self, x=None, eps=None, **kwargs):
+       super().__init__("all_nonpositive", {"x" : x, "eps" : eps, **kwargs})
 
-class _str_cmp(OpenSCADObject):
-    def __init__(self, str=None, sindex=None, pattern=None, **kwargs):
-       super().__init__("_str_cmp", {"str" : str, "sindex" : sindex, "pattern" : pattern, **kwargs})
+class all_nonnegative(_Bosl2Base):
+    def __init__(self, x=None, eps=None, **kwargs):
+       super().__init__("all_nonnegative", {"x" : x, "eps" : eps, **kwargs})
 
-class _str_cmp_recurse(OpenSCADObject):
-    def __init__(self, str=None, sindex=None, pattern=None, plen=None, pindex=None, **kwargs):
-       super().__init__("_str_cmp_recurse", {"str" : str, "sindex" : sindex, "pattern" : pattern, "plen" : plen, "pindex" : pindex, **kwargs})
+class all_equal(_Bosl2Base):
+    def __init__(self, vec=None, eps=None, **kwargs):
+       super().__init__("all_equal", {"vec" : vec, "eps" : eps, **kwargs})
 
-class starts_with(OpenSCADObject):
-    def __init__(self, str=None, pattern=None, **kwargs):
-       super().__init__("starts_with", {"str" : str, "pattern" : pattern, **kwargs})
+class is_increasing(_Bosl2Base):
+    def __init__(self, list=None, strict=None, **kwargs):
+       super().__init__("is_increasing", {"list" : list, "strict" : strict, **kwargs})
 
-class ends_with(OpenSCADObject):
-    def __init__(self, str=None, pattern=None, **kwargs):
-       super().__init__("ends_with", {"str" : str, "pattern" : pattern, **kwargs})
+class is_decreasing(_Bosl2Base):
+    def __init__(self, list=None, strict=None, **kwargs):
+       super().__init__("is_decreasing", {"list" : list, "strict" : strict, **kwargs})
 
-class str_split(OpenSCADObject):
-    def __init__(self, str=None, sep=None, keep_nulls=None, **kwargs):
-       super().__init__("str_split", {"str" : str, "sep" : sep, "keep_nulls" : keep_nulls, **kwargs})
+class _type_num(_Bosl2Base):
+    def __init__(self, x=None, **kwargs):
+       super().__init__("_type_num", {"x" : x, **kwargs})
 
-class _str_split_recurse(OpenSCADObject):
-    def __init__(self, str=None, sep=None, i=None, result=None, **kwargs):
-       super().__init__("_str_split_recurse", {"str" : str, "sep" : sep, "i" : i, "result" : result, **kwargs})
+class compare_vals(_Bosl2Base):
+    def __init__(self, a=None, b=None, **kwargs):
+       super().__init__("compare_vals", {"a" : a, "b" : b, **kwargs})
 
-class _remove_empty_strs(OpenSCADObject):
+class compare_lists(_Bosl2Base):
+    def __init__(self, a=None, b=None, **kwargs):
+       super().__init__("compare_lists", {"a" : a, "b" : b, **kwargs})
+
+class min_index(_Bosl2Base):
+    def __init__(self, vals=None, all=None, **kwargs):
+       super().__init__("min_index", {"vals" : vals, "all" : all, **kwargs})
+
+class max_index(_Bosl2Base):
+    def __init__(self, vals=None, all=None, **kwargs):
+       super().__init__("max_index", {"vals" : vals, "all" : all, **kwargs})
+
+class find_approx(_Bosl2Base):
+    def __init__(self, val=None, list=None, start=None, all=None, eps=None, **kwargs):
+       super().__init__("find_approx", {"val" : val, "list" : list, "start" : start, "all" : all, "eps" : eps, **kwargs})
+
+class __find_approx(_Bosl2Base):
+    def __init__(self, val=None, list=None, eps=None, i=None, **kwargs):
+       super().__init__("__find_approx", {"val" : val, "list" : list, "eps" : eps, "i" : i, **kwargs})
+
+class deduplicate(_Bosl2Base):
+    def __init__(self, list=None, closed=None, eps=None, **kwargs):
+       super().__init__("deduplicate", {"list" : list, "closed" : closed, "eps" : eps, **kwargs})
+
+class deduplicate_indexed(_Bosl2Base):
+    def __init__(self, list=None, indices=None, closed=None, eps=None, **kwargs):
+       super().__init__("deduplicate_indexed", {"list" : list, "indices" : indices, "closed" : closed, "eps" : eps, **kwargs})
+
+class unique(_Bosl2Base):
+    def __init__(self, list=None, **kwargs):
+       super().__init__("unique", {"list" : list, **kwargs})
+
+class _unique_sort(_Bosl2Base):
+    def __init__(self, l=None, **kwargs):
+       super().__init__("_unique_sort", {"l" : l, **kwargs})
+
+class unique_count(_Bosl2Base):
     def __init__(self, list=None, **kwargs):
-       super().__init__("_remove_empty_strs", {"list" : list, **kwargs})
+       super().__init__("unique_count", {"list" : list, **kwargs})
 
-class str_join(OpenSCADObject):
-    def __init__(self, list=None, sep=None, _i=None, _result=None, **kwargs):
-       super().__init__("str_join", {"list" : list, "sep" : sep, "_i" : _i, "_result" : _result, **kwargs})
-
-class _str_count_leading(OpenSCADObject):
-    def __init__(self, s=None, c=None, _i=None, **kwargs):
-       super().__init__("_str_count_leading", {"s" : s, "c" : c, "_i" : _i, **kwargs})
-
-class _str_count_trailing(OpenSCADObject):
-    def __init__(self, s=None, c=None, _i=None, **kwargs):
-       super().__init__("_str_count_trailing", {"s" : s, "c" : c, "_i" : _i, **kwargs})
-
-class str_strip(OpenSCADObject):
-    def __init__(self, s=None, c=None, start=None, end=None, **kwargs):
-       super().__init__("str_strip", {"s" : s, "c" : c, "start" : start, "end" : end, **kwargs})
-
-class str_pad(OpenSCADObject):
-    def __init__(self, str=None, length=None, char=None, left=None, **kwargs):
-       super().__init__("str_pad", {"str" : str, "length" : length, "char" : char, "left" : left, **kwargs})
-
-class str_replace_char(OpenSCADObject):
-    def __init__(self, str=None, char=None, replace=None, **kwargs):
-       super().__init__("str_replace_char", {"str" : str, "char" : char, "replace" : replace, **kwargs})
-
-class downcase(OpenSCADObject):
-    def __init__(self, str=None, **kwargs):
-       super().__init__("downcase", {"str" : str, **kwargs})
-
-class upcase(OpenSCADObject):
-    def __init__(self, str=None, **kwargs):
-       super().__init__("upcase", {"str" : str, **kwargs})
-
-class rand_str(OpenSCADObject):
-    def __init__(self, n=None, charset=None, seed=None, **kwargs):
-       super().__init__("rand_str", {"n" : n, "charset" : charset, "seed" : seed, **kwargs})
-
-class parse_int(OpenSCADObject):
-    def __init__(self, str=None, base=None, **kwargs):
-       super().__init__("parse_int", {"str" : str, "base" : base, **kwargs})
-
-class _parse_int_recurse(OpenSCADObject):
-    def __init__(self, str=None, base=None, i=None, **kwargs):
-       super().__init__("_parse_int_recurse", {"str" : str, "base" : base, "i" : i, **kwargs})
-
-class parse_float(OpenSCADObject):
-    def __init__(self, str=None, **kwargs):
-       super().__init__("parse_float", {"str" : str, **kwargs})
-
-class parse_frac(OpenSCADObject):
-    def __init__(self, str=None, mixed=None, improper=None, signed=None, **kwargs):
-       super().__init__("parse_frac", {"str" : str, "mixed" : mixed, "improper" : improper, "signed" : signed, **kwargs})
-
-class parse_num(OpenSCADObject):
-    def __init__(self, str=None, **kwargs):
-       super().__init__("parse_num", {"str" : str, **kwargs})
-
-class format_int(OpenSCADObject):
-    def __init__(self, i=None, mindigits=None, **kwargs):
-       super().__init__("format_int", {"i" : i, "mindigits" : mindigits, **kwargs})
-
-class format_fixed(OpenSCADObject):
-    def __init__(self, f=None, digits=None, **kwargs):
-       super().__init__("format_fixed", {"f" : f, "digits" : digits, **kwargs})
-
-class format_float(OpenSCADObject):
-    def __init__(self, f=None, sig=None, **kwargs):
-       super().__init__("format_float", {"f" : f, "sig" : sig, **kwargs})
-
-class _format_matrix(OpenSCADObject):
-    def __init__(self, M=None, sig=None, sep=None, eps=None, **kwargs):
-       super().__init__("_format_matrix", {"M" : M, "sig" : sig, "sep" : sep, "eps" : eps, **kwargs})
-
-class format(OpenSCADObject):
-    def __init__(self, fmt=None, vals=None, **kwargs):
-       super().__init__("format", {"fmt" : fmt, "vals" : vals, **kwargs})
-
-class is_lower(OpenSCADObject):
-    def __init__(self, s=None, **kwargs):
-       super().__init__("is_lower", {"s" : s, **kwargs})
-
-class is_upper(OpenSCADObject):
-    def __init__(self, s=None, **kwargs):
-       super().__init__("is_upper", {"s" : s, **kwargs})
-
-class is_digit(OpenSCADObject):
-    def __init__(self, s=None, **kwargs):
-       super().__init__("is_digit", {"s" : s, **kwargs})
-
-class is_hexdigit(OpenSCADObject):
-    def __init__(self, s=None, **kwargs):
-       super().__init__("is_hexdigit", {"s" : s, **kwargs})
-
-class is_letter(OpenSCADObject):
-    def __init__(self, s=None, **kwargs):
-       super().__init__("is_letter", {"s" : s, **kwargs})
+class _valid_idx(_Bosl2Base):
+    def __init__(self, idx=None, imin=None, imax=None, **kwargs):
+       super().__init__("_valid_idx", {"idx" : idx, "imin" : imin, "imax" : imax, **kwargs})
+
+class _group_sort_by_index(_Bosl2Base):
+    def __init__(self, l=None, idx=None, **kwargs):
+       super().__init__("_group_sort_by_index", {"l" : l, "idx" : idx, **kwargs})
+
+class _group_sort(_Bosl2Base):
+    def __init__(self, l=None, **kwargs):
+       super().__init__("_group_sort", {"l" : l, **kwargs})
+
+class _sort_scalars(_Bosl2Base):
+    def __init__(self, arr=None, **kwargs):
+       super().__init__("_sort_scalars", {"arr" : arr, **kwargs})
+
+class _sort_vectors(_Bosl2Base):
+    def __init__(self, arr=None, _i=None, **kwargs):
+       super().__init__("_sort_vectors", {"arr" : arr, "_i" : _i, **kwargs})
+
+class _sort_vectors(_Bosl2Base):
+    def __init__(self, arr=None, idxlist=None, _i=None, **kwargs):
+       super().__init__("_sort_vectors", {"arr" : arr, "idxlist" : idxlist, "_i" : _i, **kwargs})
+
+class _sort_general(_Bosl2Base):
+    def __init__(self, arr=None, idx=None, indexed=None, **kwargs):
+       super().__init__("_sort_general", {"arr" : arr, "idx" : idx, "indexed" : indexed, **kwargs})
+
+class _lexical_sort(_Bosl2Base):
+    def __init__(self, arr=None, **kwargs):
+       super().__init__("_lexical_sort", {"arr" : arr, **kwargs})
+
+class _indexed_sort(_Bosl2Base):
+    def __init__(self, arrind=None, **kwargs):
+       super().__init__("_indexed_sort", {"arrind" : arrind, **kwargs})
+
+class sort(_Bosl2Base):
+    def __init__(self, list=None, idx=None, **kwargs):
+       super().__init__("sort", {"list" : list, "idx" : idx, **kwargs})
+
+class sortidx(_Bosl2Base):
+    def __init__(self, list=None, idx=None, **kwargs):
+       super().__init__("sortidx", {"list" : list, "idx" : idx, **kwargs})
+
+class group_sort(_Bosl2Base):
+    def __init__(self, list=None, idx=None, **kwargs):
+       super().__init__("group_sort", {"list" : list, "idx" : idx, **kwargs})
+
+class group_data(_Bosl2Base):
+    def __init__(self, groups=None, values=None, **kwargs):
+       super().__init__("group_data", {"groups" : groups, "values" : values, **kwargs})
+
+class list_smallest(_Bosl2Base):
+    def __init__(self, list=None, k=None, **kwargs):
+       super().__init__("list_smallest", {"list" : list, "k" : k, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/structs.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/structs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/structs.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class echo_struct(OpenSCADObject):
-    def __init__(self, struct=None, name=None, **kwargs):
-       super().__init__("echo_struct", {"struct" : struct, "name" : name, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/structs.scad'}", use_not_include=False)
 
-class struct_set(OpenSCADObject):
+class struct_set(_Bosl2Base):
     def __init__(self, struct=None, key=None, value=None, grow=None, **kwargs):
        super().__init__("struct_set", {"struct" : struct, "key" : key, "value" : value, "grow" : grow, **kwargs})
 
-class _format_key(OpenSCADObject):
+class _format_key(_Bosl2Base):
     def __init__(self, key=None, **kwargs):
        super().__init__("_format_key", {"key" : key, **kwargs})
 
-class struct_remove(OpenSCADObject):
+class struct_remove(_Bosl2Base):
     def __init__(self, struct=None, key=None, **kwargs):
        super().__init__("struct_remove", {"struct" : struct, "key" : key, **kwargs})
 
-class struct_val(OpenSCADObject):
+class struct_val(_Bosl2Base):
     def __init__(self, struct=None, key=None, default=None, **kwargs):
        super().__init__("struct_val", {"struct" : struct, "key" : key, "default" : default, **kwargs})
 
-class struct_keys(OpenSCADObject):
+class struct_keys(_Bosl2Base):
     def __init__(self, struct=None, **kwargs):
        super().__init__("struct_keys", {"struct" : struct, **kwargs})
 
-class echo_struct(OpenSCADObject):
+class echo_struct(_Bosl2Base):
     def __init__(self, struct=None, name=None, **kwargs):
        super().__init__("echo_struct", {"struct" : struct, "name" : name, **kwargs})
 
-class is_struct(OpenSCADObject):
+class is_struct(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("is_struct", {"x" : x, **kwargs})
 
+class echo_struct(_Bosl2Base):
+    def __init__(self, struct=None, name=None, **kwargs):
+       super().__init__("echo_struct", {"struct" : struct, "name" : name, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/transforms.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/transforms.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,207 +1,209 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/transforms.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-_NO_ARG = OpenSCADConstant('_NO_ARG')
-class move(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/transforms.scad'}", use_not_include=False)
+
+_NO_ARG = _OpenSCADConstant('_NO_ARG')
+class move(_Bosl2Base):
     def __init__(self, v=None, p=None, **kwargs):
        super().__init__("move", {"v" : v, "p" : p, **kwargs})
 
-class left(OpenSCADObject):
+class translate(_Bosl2Base):
+    def __init__(self, v=None, p=None, **kwargs):
+       super().__init__("translate", {"v" : v, "p" : p, **kwargs})
+
+class left(_Bosl2Base):
     def __init__(self, x=None, p=None, **kwargs):
        super().__init__("left", {"x" : x, "p" : p, **kwargs})
 
-class right(OpenSCADObject):
+class right(_Bosl2Base):
     def __init__(self, x=None, p=None, **kwargs):
        super().__init__("right", {"x" : x, "p" : p, **kwargs})
 
-class xmove(OpenSCADObject):
+class xmove(_Bosl2Base):
     def __init__(self, x=None, p=None, **kwargs):
        super().__init__("xmove", {"x" : x, "p" : p, **kwargs})
 
-class fwd(OpenSCADObject):
+class fwd(_Bosl2Base):
     def __init__(self, y=None, p=None, **kwargs):
        super().__init__("fwd", {"y" : y, "p" : p, **kwargs})
 
-class back(OpenSCADObject):
+class back(_Bosl2Base):
     def __init__(self, y=None, p=None, **kwargs):
        super().__init__("back", {"y" : y, "p" : p, **kwargs})
 
-class ymove(OpenSCADObject):
+class ymove(_Bosl2Base):
     def __init__(self, y=None, p=None, **kwargs):
        super().__init__("ymove", {"y" : y, "p" : p, **kwargs})
 
-class down(OpenSCADObject):
+class down(_Bosl2Base):
     def __init__(self, z=None, p=None, **kwargs):
        super().__init__("down", {"z" : z, "p" : p, **kwargs})
 
-class up(OpenSCADObject):
+class up(_Bosl2Base):
     def __init__(self, z=None, p=None, **kwargs):
        super().__init__("up", {"z" : z, "p" : p, **kwargs})
 
-class zmove(OpenSCADObject):
+class zmove(_Bosl2Base):
     def __init__(self, z=None, p=None, **kwargs):
        super().__init__("zmove", {"z" : z, "p" : p, **kwargs})
 
-class rot(OpenSCADObject):
-    def __init__(self, a=None, v=None, cp=None, _from=None, to=None, reverse=None, **kwargs):
-       super().__init__("rot", {"a" : a, "v" : v, "cp" : cp, "_from" : _from, "to" : to, "reverse" : reverse, **kwargs})
+class rot(_Bosl2Base):
+    def __init__(self, a=None, v=None, cp=None, _from=None, to=None, reverse=None, p=None, _m=None, **kwargs):
+       super().__init__("rot", {"a" : a, "v" : v, "cp" : cp, "_from" : _from, "to" : to, "reverse" : reverse, "p" : p, "_m" : _m, **kwargs})
 
-class xrot(OpenSCADObject):
+class xrot(_Bosl2Base):
     def __init__(self, a=None, p=None, cp=None, **kwargs):
        super().__init__("xrot", {"a" : a, "p" : p, "cp" : cp, **kwargs})
 
-class yrot(OpenSCADObject):
+class yrot(_Bosl2Base):
     def __init__(self, a=None, p=None, cp=None, **kwargs):
        super().__init__("yrot", {"a" : a, "p" : p, "cp" : cp, **kwargs})
 
-class zrot(OpenSCADObject):
+class zrot(_Bosl2Base):
     def __init__(self, a=None, p=None, cp=None, **kwargs):
        super().__init__("zrot", {"a" : a, "p" : p, "cp" : cp, **kwargs})
 
-class xscale(OpenSCADObject):
+class scale(_Bosl2Base):
+    def __init__(self, v=None, p=None, cp=None, **kwargs):
+       super().__init__("scale", {"v" : v, "p" : p, "cp" : cp, **kwargs})
+
+class xscale(_Bosl2Base):
     def __init__(self, x=None, p=None, cp=None, **kwargs):
        super().__init__("xscale", {"x" : x, "p" : p, "cp" : cp, **kwargs})
 
-class yscale(OpenSCADObject):
+class yscale(_Bosl2Base):
     def __init__(self, y=None, p=None, cp=None, **kwargs):
        super().__init__("yscale", {"y" : y, "p" : p, "cp" : cp, **kwargs})
 
-class zscale(OpenSCADObject):
+class zscale(_Bosl2Base):
     def __init__(self, z=None, p=None, cp=None, **kwargs):
        super().__init__("zscale", {"z" : z, "p" : p, "cp" : cp, **kwargs})
 
-class xflip(OpenSCADObject):
+class mirror(_Bosl2Base):
+    def __init__(self, v=None, p=None, **kwargs):
+       super().__init__("mirror", {"v" : v, "p" : p, **kwargs})
+
+class xflip(_Bosl2Base):
     def __init__(self, p=None, x=None, **kwargs):
        super().__init__("xflip", {"p" : p, "x" : x, **kwargs})
 
-class yflip(OpenSCADObject):
+class yflip(_Bosl2Base):
     def __init__(self, p=None, y=None, **kwargs):
        super().__init__("yflip", {"p" : p, "y" : y, **kwargs})
 
-class zflip(OpenSCADObject):
+class zflip(_Bosl2Base):
     def __init__(self, p=None, z=None, **kwargs):
        super().__init__("zflip", {"p" : p, "z" : z, **kwargs})
 
-class frame_map(OpenSCADObject):
+class frame_map(_Bosl2Base):
     def __init__(self, x=None, y=None, z=None, p=None, reverse=None, **kwargs):
        super().__init__("frame_map", {"x" : x, "y" : y, "z" : z, "p" : p, "reverse" : reverse, **kwargs})
 
-class skew(OpenSCADObject):
+class skew(_Bosl2Base):
     def __init__(self, p=None, sxy=None, sxz=None, syx=None, syz=None, szx=None, szy=None, **kwargs):
        super().__init__("skew", {"p" : p, "sxy" : sxy, "sxz" : sxz, "syx" : syx, "syz" : syz, "szx" : szx, "szy" : szy, **kwargs})
 
-class move(OpenSCADObject):
-    def __init__(self, v=None, p=None, **kwargs):
-       super().__init__("move", {"v" : v, "p" : p, **kwargs})
+class is_2d_transform(_Bosl2Base):
+    def __init__(self, t=None, **kwargs):
+       super().__init__("is_2d_transform", {"t" : t, **kwargs})
 
-class translate(OpenSCADObject):
+class apply(_Bosl2Base):
+    def __init__(self, transform=None, points=None, **kwargs):
+       super().__init__("apply", {"transform" : transform, "points" : points, **kwargs})
+
+class _apply(_Bosl2Base):
+    def __init__(self, transform=None, points=None, **kwargs):
+       super().__init__("_apply", {"transform" : transform, "points" : points, **kwargs})
+
+class move(_Bosl2Base):
     def __init__(self, v=None, p=None, **kwargs):
-       super().__init__("translate", {"v" : v, "p" : p, **kwargs})
+       super().__init__("move", {"v" : v, "p" : p, **kwargs})
 
-class left(OpenSCADObject):
+class left(_Bosl2Base):
     def __init__(self, x=None, p=None, **kwargs):
        super().__init__("left", {"x" : x, "p" : p, **kwargs})
 
-class right(OpenSCADObject):
+class right(_Bosl2Base):
     def __init__(self, x=None, p=None, **kwargs):
        super().__init__("right", {"x" : x, "p" : p, **kwargs})
 
-class xmove(OpenSCADObject):
+class xmove(_Bosl2Base):
     def __init__(self, x=None, p=None, **kwargs):
        super().__init__("xmove", {"x" : x, "p" : p, **kwargs})
 
-class fwd(OpenSCADObject):
+class fwd(_Bosl2Base):
     def __init__(self, y=None, p=None, **kwargs):
        super().__init__("fwd", {"y" : y, "p" : p, **kwargs})
 
-class back(OpenSCADObject):
+class back(_Bosl2Base):
     def __init__(self, y=None, p=None, **kwargs):
        super().__init__("back", {"y" : y, "p" : p, **kwargs})
 
-class ymove(OpenSCADObject):
+class ymove(_Bosl2Base):
     def __init__(self, y=None, p=None, **kwargs):
        super().__init__("ymove", {"y" : y, "p" : p, **kwargs})
 
-class down(OpenSCADObject):
+class down(_Bosl2Base):
     def __init__(self, z=None, p=None, **kwargs):
        super().__init__("down", {"z" : z, "p" : p, **kwargs})
 
-class up(OpenSCADObject):
+class up(_Bosl2Base):
     def __init__(self, z=None, p=None, **kwargs):
        super().__init__("up", {"z" : z, "p" : p, **kwargs})
 
-class zmove(OpenSCADObject):
+class zmove(_Bosl2Base):
     def __init__(self, z=None, p=None, **kwargs):
        super().__init__("zmove", {"z" : z, "p" : p, **kwargs})
 
-class rot(OpenSCADObject):
-    def __init__(self, a=None, v=None, cp=None, _from=None, to=None, reverse=None, p=None, _m=None, **kwargs):
-       super().__init__("rot", {"a" : a, "v" : v, "cp" : cp, "_from" : _from, "to" : to, "reverse" : reverse, "p" : p, "_m" : _m, **kwargs})
+class rot(_Bosl2Base):
+    def __init__(self, a=None, v=None, cp=None, _from=None, to=None, reverse=None, **kwargs):
+       super().__init__("rot", {"a" : a, "v" : v, "cp" : cp, "_from" : _from, "to" : to, "reverse" : reverse, **kwargs})
 
-class xrot(OpenSCADObject):
+class xrot(_Bosl2Base):
     def __init__(self, a=None, p=None, cp=None, **kwargs):
        super().__init__("xrot", {"a" : a, "p" : p, "cp" : cp, **kwargs})
 
-class yrot(OpenSCADObject):
+class yrot(_Bosl2Base):
     def __init__(self, a=None, p=None, cp=None, **kwargs):
        super().__init__("yrot", {"a" : a, "p" : p, "cp" : cp, **kwargs})
 
-class zrot(OpenSCADObject):
+class zrot(_Bosl2Base):
     def __init__(self, a=None, p=None, cp=None, **kwargs):
        super().__init__("zrot", {"a" : a, "p" : p, "cp" : cp, **kwargs})
 
-class scale(OpenSCADObject):
-    def __init__(self, v=None, p=None, cp=None, **kwargs):
-       super().__init__("scale", {"v" : v, "p" : p, "cp" : cp, **kwargs})
-
-class xscale(OpenSCADObject):
+class xscale(_Bosl2Base):
     def __init__(self, x=None, p=None, cp=None, **kwargs):
        super().__init__("xscale", {"x" : x, "p" : p, "cp" : cp, **kwargs})
 
-class yscale(OpenSCADObject):
+class yscale(_Bosl2Base):
     def __init__(self, y=None, p=None, cp=None, **kwargs):
        super().__init__("yscale", {"y" : y, "p" : p, "cp" : cp, **kwargs})
 
-class zscale(OpenSCADObject):
+class zscale(_Bosl2Base):
     def __init__(self, z=None, p=None, cp=None, **kwargs):
        super().__init__("zscale", {"z" : z, "p" : p, "cp" : cp, **kwargs})
 
-class mirror(OpenSCADObject):
-    def __init__(self, v=None, p=None, **kwargs):
-       super().__init__("mirror", {"v" : v, "p" : p, **kwargs})
-
-class xflip(OpenSCADObject):
+class xflip(_Bosl2Base):
     def __init__(self, p=None, x=None, **kwargs):
        super().__init__("xflip", {"p" : p, "x" : x, **kwargs})
 
-class yflip(OpenSCADObject):
+class yflip(_Bosl2Base):
     def __init__(self, p=None, y=None, **kwargs):
        super().__init__("yflip", {"p" : p, "y" : y, **kwargs})
 
-class zflip(OpenSCADObject):
+class zflip(_Bosl2Base):
     def __init__(self, p=None, z=None, **kwargs):
        super().__init__("zflip", {"p" : p, "z" : z, **kwargs})
 
-class frame_map(OpenSCADObject):
+class frame_map(_Bosl2Base):
     def __init__(self, x=None, y=None, z=None, p=None, reverse=None, **kwargs):
        super().__init__("frame_map", {"x" : x, "y" : y, "z" : z, "p" : p, "reverse" : reverse, **kwargs})
 
-class skew(OpenSCADObject):
+class skew(_Bosl2Base):
     def __init__(self, p=None, sxy=None, sxz=None, syx=None, syz=None, szx=None, szy=None, **kwargs):
        super().__init__("skew", {"p" : p, "sxy" : sxy, "sxz" : sxz, "syx" : syx, "syz" : syz, "szx" : szx, "szy" : szy, **kwargs})
 
-class is_2d_transform(OpenSCADObject):
-    def __init__(self, t=None, **kwargs):
-       super().__init__("is_2d_transform", {"t" : t, **kwargs})
-
-class apply(OpenSCADObject):
-    def __init__(self, transform=None, points=None, **kwargs):
-       super().__init__("apply", {"transform" : transform, "points" : points, **kwargs})
-
-class _apply(OpenSCADObject):
-    def __init__(self, transform=None, points=None, **kwargs):
-       super().__init__("_apply", {"transform" : transform, "points" : points, **kwargs})
-
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/trigonometry.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/trigonometry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,112 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/trigonometry.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class law_of_cosines(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/trigonometry.scad'}", use_not_include=False)
+
+class law_of_cosines(_Bosl2Base):
     def __init__(self, a=None, b=None, c=None, C=None, **kwargs):
        super().__init__("law_of_cosines", {"a" : a, "b" : b, "c" : c, "C" : C, **kwargs})
 
-class law_of_sines(OpenSCADObject):
+class law_of_sines(_Bosl2Base):
     def __init__(self, a=None, A=None, b=None, B=None, **kwargs):
        super().__init__("law_of_sines", {"a" : a, "A" : A, "b" : b, "B" : B, **kwargs})
 
-class hyp_opp_to_adj(OpenSCADObject):
+class hyp_opp_to_adj(_Bosl2Base):
     def __init__(self, hyp=None, opp=None, **kwargs):
        super().__init__("hyp_opp_to_adj", {"hyp" : hyp, "opp" : opp, **kwargs})
 
-class opp_hyp_to_adj(OpenSCADObject):
+class opp_hyp_to_adj(_Bosl2Base):
     def __init__(self, opp=None, hyp=None, **kwargs):
        super().__init__("opp_hyp_to_adj", {"opp" : opp, "hyp" : hyp, **kwargs})
 
-class hyp_ang_to_adj(OpenSCADObject):
+class hyp_ang_to_adj(_Bosl2Base):
     def __init__(self, hyp=None, ang=None, **kwargs):
        super().__init__("hyp_ang_to_adj", {"hyp" : hyp, "ang" : ang, **kwargs})
 
-class ang_hyp_to_adj(OpenSCADObject):
+class ang_hyp_to_adj(_Bosl2Base):
     def __init__(self, ang=None, hyp=None, **kwargs):
        super().__init__("ang_hyp_to_adj", {"ang" : ang, "hyp" : hyp, **kwargs})
 
-class opp_ang_to_adj(OpenSCADObject):
+class opp_ang_to_adj(_Bosl2Base):
     def __init__(self, opp=None, ang=None, **kwargs):
        super().__init__("opp_ang_to_adj", {"opp" : opp, "ang" : ang, **kwargs})
 
-class ang_opp_to_adj(OpenSCADObject):
+class ang_opp_to_adj(_Bosl2Base):
     def __init__(self, ang=None, opp=None, **kwargs):
        super().__init__("ang_opp_to_adj", {"ang" : ang, "opp" : opp, **kwargs})
 
-class hyp_adj_to_opp(OpenSCADObject):
+class hyp_adj_to_opp(_Bosl2Base):
     def __init__(self, hyp=None, adj=None, **kwargs):
        super().__init__("hyp_adj_to_opp", {"hyp" : hyp, "adj" : adj, **kwargs})
 
-class adj_hyp_to_opp(OpenSCADObject):
+class adj_hyp_to_opp(_Bosl2Base):
     def __init__(self, adj=None, hyp=None, **kwargs):
        super().__init__("adj_hyp_to_opp", {"adj" : adj, "hyp" : hyp, **kwargs})
 
-class hyp_ang_to_opp(OpenSCADObject):
+class hyp_ang_to_opp(_Bosl2Base):
     def __init__(self, hyp=None, ang=None, **kwargs):
        super().__init__("hyp_ang_to_opp", {"hyp" : hyp, "ang" : ang, **kwargs})
 
-class ang_hyp_to_opp(OpenSCADObject):
+class ang_hyp_to_opp(_Bosl2Base):
     def __init__(self, ang=None, hyp=None, **kwargs):
        super().__init__("ang_hyp_to_opp", {"ang" : ang, "hyp" : hyp, **kwargs})
 
-class adj_ang_to_opp(OpenSCADObject):
+class adj_ang_to_opp(_Bosl2Base):
     def __init__(self, adj=None, ang=None, **kwargs):
        super().__init__("adj_ang_to_opp", {"adj" : adj, "ang" : ang, **kwargs})
 
-class ang_adj_to_opp(OpenSCADObject):
+class ang_adj_to_opp(_Bosl2Base):
     def __init__(self, ang=None, adj=None, **kwargs):
        super().__init__("ang_adj_to_opp", {"ang" : ang, "adj" : adj, **kwargs})
 
-class adj_opp_to_hyp(OpenSCADObject):
+class adj_opp_to_hyp(_Bosl2Base):
     def __init__(self, adj=None, opp=None, **kwargs):
        super().__init__("adj_opp_to_hyp", {"adj" : adj, "opp" : opp, **kwargs})
 
-class opp_adj_to_hyp(OpenSCADObject):
+class opp_adj_to_hyp(_Bosl2Base):
     def __init__(self, opp=None, adj=None, **kwargs):
        super().__init__("opp_adj_to_hyp", {"opp" : opp, "adj" : adj, **kwargs})
 
-class adj_ang_to_hyp(OpenSCADObject):
+class adj_ang_to_hyp(_Bosl2Base):
     def __init__(self, adj=None, ang=None, **kwargs):
        super().__init__("adj_ang_to_hyp", {"adj" : adj, "ang" : ang, **kwargs})
 
-class ang_adj_to_hyp(OpenSCADObject):
+class ang_adj_to_hyp(_Bosl2Base):
     def __init__(self, ang=None, adj=None, **kwargs):
        super().__init__("ang_adj_to_hyp", {"ang" : ang, "adj" : adj, **kwargs})
 
-class opp_ang_to_hyp(OpenSCADObject):
+class opp_ang_to_hyp(_Bosl2Base):
     def __init__(self, opp=None, ang=None, **kwargs):
        super().__init__("opp_ang_to_hyp", {"opp" : opp, "ang" : ang, **kwargs})
 
-class ang_opp_to_hyp(OpenSCADObject):
+class ang_opp_to_hyp(_Bosl2Base):
     def __init__(self, ang=None, opp=None, **kwargs):
        super().__init__("ang_opp_to_hyp", {"ang" : ang, "opp" : opp, **kwargs})
 
-class hyp_adj_to_ang(OpenSCADObject):
+class hyp_adj_to_ang(_Bosl2Base):
     def __init__(self, hyp=None, adj=None, **kwargs):
        super().__init__("hyp_adj_to_ang", {"hyp" : hyp, "adj" : adj, **kwargs})
 
-class adj_hyp_to_ang(OpenSCADObject):
+class adj_hyp_to_ang(_Bosl2Base):
     def __init__(self, adj=None, hyp=None, **kwargs):
        super().__init__("adj_hyp_to_ang", {"adj" : adj, "hyp" : hyp, **kwargs})
 
-class hyp_opp_to_ang(OpenSCADObject):
+class hyp_opp_to_ang(_Bosl2Base):
     def __init__(self, hyp=None, opp=None, **kwargs):
        super().__init__("hyp_opp_to_ang", {"hyp" : hyp, "opp" : opp, **kwargs})
 
-class opp_hyp_to_ang(OpenSCADObject):
+class opp_hyp_to_ang(_Bosl2Base):
     def __init__(self, opp=None, hyp=None, **kwargs):
        super().__init__("opp_hyp_to_ang", {"opp" : opp, "hyp" : hyp, **kwargs})
 
-class adj_opp_to_ang(OpenSCADObject):
+class adj_opp_to_ang(_Bosl2Base):
     def __init__(self, adj=None, opp=None, **kwargs):
        super().__init__("adj_opp_to_ang", {"adj" : adj, "opp" : opp, **kwargs})
 
-class opp_adj_to_ang(OpenSCADObject):
+class opp_adj_to_ang(_Bosl2Base):
     def __init__(self, opp=None, adj=None, **kwargs):
        super().__init__("opp_adj_to_ang", {"opp" : opp, "adj" : adj, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/tripod_mounts.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/tripod_mounts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/tripod_mounts.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class manfrotto_rc2_plate(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/tripod_mounts.scad'}", use_not_include=False)
+
+class manfrotto_rc2_plate(_Bosl2Base):
     def __init__(self, chamfer=None, anchor=None, orient=None, spin=None, **kwargs):
        super().__init__("manfrotto_rc2_plate", {"chamfer" : chamfer, "anchor" : anchor, "orient" : orient, "spin" : spin, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/turtle3d.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/turtle3d.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/turtle3d.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class turtle3d(OpenSCADObject):
-    def __init__(self, commands=None, state=None, transforms=None, full_state=None, repeat=None, **kwargs):
-       super().__init__("turtle3d", {"commands" : commands, "state" : state, "transforms" : transforms, "full_state" : full_state, "repeat" : repeat, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/turtle3d.scad'}", use_not_include=False)
 
-class _transpart(OpenSCADObject):
+class _transpart(_Bosl2Base):
     def __init__(self, T=None, **kwargs):
        super().__init__("_transpart", {"T" : T, **kwargs})
 
-class _rotpart(OpenSCADObject):
+class _rotpart(_Bosl2Base):
     def __init__(self, T=None, **kwargs):
        super().__init__("_rotpart", {"T" : T, **kwargs})
 
-class _turtle3d_state_valid(OpenSCADObject):
+class _turtle3d_state_valid(_Bosl2Base):
     def __init__(self, state=None, **kwargs):
        super().__init__("_turtle3d_state_valid", {"state" : state, **kwargs})
 
-class turtle3d(OpenSCADObject):
+class turtle3d(_Bosl2Base):
     def __init__(self, commands=None, state=None, transforms=None, full_state=None, repeat=None, **kwargs):
        super().__init__("turtle3d", {"commands" : commands, "state" : state, "transforms" : transforms, "full_state" : full_state, "repeat" : repeat, **kwargs})
 
-class _turtle3d_repeat(OpenSCADObject):
+class _turtle3d_repeat(_Bosl2Base):
     def __init__(self, commands=None, state=None, repeat=None, **kwargs):
        super().__init__("_turtle3d_repeat", {"commands" : commands, "state" : state, "repeat" : repeat, **kwargs})
 
-class _turtle3d_command_len(OpenSCADObject):
+class _turtle3d_command_len(_Bosl2Base):
     def __init__(self, commands=None, index=None, **kwargs):
        super().__init__("_turtle3d_command_len", {"commands" : commands, "index" : index, **kwargs})
 
-class _turtle3d(OpenSCADObject):
+class _turtle3d(_Bosl2Base):
     def __init__(self, commands=None, state=None, index=None, **kwargs):
        super().__init__("_turtle3d", {"commands" : commands, "state" : state, "index" : index, **kwargs})
 
-class _turtle3d_rotation(OpenSCADObject):
+class _turtle3d_rotation(_Bosl2Base):
     def __init__(self, command=None, angle=None, center=None, **kwargs):
        super().__init__("_turtle3d_rotation", {"command" : command, "angle" : angle, "center" : center, **kwargs})
 
-class _tupdate(OpenSCADObject):
+class _tupdate(_Bosl2Base):
     def __init__(self, state=None, tran=None, pretran=None, **kwargs):
        super().__init__("_tupdate", {"state" : state, "tran" : tran, "pretran" : pretran, **kwargs})
 
-class _turtle3d_command(OpenSCADObject):
+class _turtle3d_command(_Bosl2Base):
     def __init__(self, command=None, parm=None, parm2=None, state=None, index=None, **kwargs):
        super().__init__("_turtle3d_command", {"command" : command, "parm" : parm, "parm2" : parm2, "state" : state, "index" : index, **kwargs})
 
-class _turtle3d_list_command(OpenSCADObject):
+class _turtle3d_list_command(_Bosl2Base):
     def __init__(self, command=None, arcsteps=None, movescale=None, lastT=None, lastPre=None, index=None, **kwargs):
        super().__init__("_turtle3d_list_command", {"command" : command, "arcsteps" : arcsteps, "movescale" : movescale, "lastT" : lastT, "lastPre" : lastPre, "index" : index, **kwargs})
 
+class turtle3d(_Bosl2Base):
+    def __init__(self, commands=None, state=None, transforms=None, full_state=None, repeat=None, **kwargs):
+       super().__init__("turtle3d", {"commands" : commands, "state" : state, "transforms" : transforms, "full_state" : full_state, "repeat" : repeat, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/version.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/version.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-BOSL_VERSION = OpenSCADConstant('BOSL_VERSION')
-class bosl_required(OpenSCADObject):
-    def __init__(self, version=None, **kwargs):
-       super().__init__("bosl_required", {"version" : version, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/version.scad'}", use_not_include=False)
 
-class bosl_version(OpenSCADObject):
+BOSL_VERSION = _OpenSCADConstant('BOSL_VERSION')
+class bosl_version(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("bosl_version", {**kwargs})
 
-class bosl_version_num(OpenSCADObject):
+class bosl_version_num(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("bosl_version_num", {**kwargs})
 
-class bosl_version_str(OpenSCADObject):
+class bosl_version_str(_Bosl2Base):
     def __init__(self, **kwargs):
        super().__init__("bosl_version_str", {**kwargs})
 
-class _version_split_str(OpenSCADObject):
+class _version_split_str(_Bosl2Base):
     def __init__(self, x=None, _i=None, _out=None, _num=None, **kwargs):
        super().__init__("_version_split_str", {"x" : x, "_i" : _i, "_out" : _out, "_num" : _num, **kwargs})
 
-class version_to_list(OpenSCADObject):
+class version_to_list(_Bosl2Base):
     def __init__(self, version=None, **kwargs):
        super().__init__("version_to_list", {"version" : version, **kwargs})
 
-class version_to_str(OpenSCADObject):
+class version_to_str(_Bosl2Base):
     def __init__(self, version=None, **kwargs):
        super().__init__("version_to_str", {"version" : version, **kwargs})
 
-class version_to_num(OpenSCADObject):
+class version_to_num(_Bosl2Base):
     def __init__(self, version=None, **kwargs):
        super().__init__("version_to_num", {"version" : version, **kwargs})
 
-class version_cmp(OpenSCADObject):
+class version_cmp(_Bosl2Base):
     def __init__(self, a=None, b=None, **kwargs):
        super().__init__("version_cmp", {"a" : a, "b" : b, **kwargs})
 
+class bosl_required(_Bosl2Base):
+    def __init__(self, version=None, **kwargs):
+       super().__init__("bosl_required", {"version" : version, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/vnf.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/vnf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,178 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
-
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/vnf.scad'}", use_not_include=False)
-
-EMPTY_VNF = OpenSCADConstant('EMPTY_VNF')
-_vnf_validate_errs = OpenSCADConstant('_vnf_validate_errs')
-class vnf_polyhedron(OpenSCADObject):
-    def __init__(self, vnf=None, convexity=None, extent=None, cp=None, anchor=None, spin=None, orient=None, atype=None, **kwargs):
-       super().__init__("vnf_polyhedron", {"vnf" : vnf, "convexity" : convexity, "extent" : extent, "cp" : cp, "anchor" : anchor, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-class vnf_wireframe(OpenSCADObject):
-    def __init__(self, vnf=None, width=None, **kwargs):
-       super().__init__("vnf_wireframe", {"vnf" : vnf, "width" : width, **kwargs})
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class _show_vertices(OpenSCADObject):
-    def __init__(self, vertices=None, size=None, **kwargs):
-       super().__init__("_show_vertices", {"vertices" : vertices, "size" : size, **kwargs})
-
-class _show_faces(OpenSCADObject):
-    def __init__(self, vertices=None, faces=None, size=None, **kwargs):
-       super().__init__("_show_faces", {"vertices" : vertices, "faces" : faces, "size" : size, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/vnf.scad'}", use_not_include=False)
 
-class debug_vnf(OpenSCADObject):
-    def __init__(self, vnf=None, faces=None, vertices=None, opacity=None, size=None, convexity=None, **kwargs):
-       super().__init__("debug_vnf", {"vnf" : vnf, "faces" : faces, "vertices" : vertices, "opacity" : opacity, "size" : size, "convexity" : convexity, **kwargs})
-
-class vnf_validate(OpenSCADObject):
-    def __init__(self, vnf=None, size=None, show_warns=None, check_isects=None, **kwargs):
-       super().__init__("vnf_validate", {"vnf" : vnf, "size" : size, "show_warns" : show_warns, "check_isects" : check_isects, **kwargs})
-
-class vnf_vertex_array(OpenSCADObject):
+EMPTY_VNF = _OpenSCADConstant('EMPTY_VNF')
+_vnf_validate_errs = _OpenSCADConstant('_vnf_validate_errs')
+class vnf_vertex_array(_Bosl2Base):
     def __init__(self, points=None, caps=None, cap1=None, cap2=None, col_wrap=None, row_wrap=None, reverse=None, style=None, **kwargs):
        super().__init__("vnf_vertex_array", {"points" : points, "caps" : caps, "cap1" : cap1, "cap2" : cap2, "col_wrap" : col_wrap, "row_wrap" : row_wrap, "reverse" : reverse, "style" : style, **kwargs})
 
-class vnf_tri_array(OpenSCADObject):
+class vnf_tri_array(_Bosl2Base):
     def __init__(self, points=None, row_wrap=None, reverse=None, **kwargs):
        super().__init__("vnf_tri_array", {"points" : points, "row_wrap" : row_wrap, "reverse" : reverse, **kwargs})
 
-class vnf_join(OpenSCADObject):
+class vnf_join(_Bosl2Base):
     def __init__(self, vnfs=None, **kwargs):
        super().__init__("vnf_join", {"vnfs" : vnfs, **kwargs})
 
-class vnf_from_polygons(OpenSCADObject):
+class vnf_from_polygons(_Bosl2Base):
     def __init__(self, polygons=None, **kwargs):
        super().__init__("vnf_from_polygons", {"polygons" : polygons, **kwargs})
 
-class _path_path_closest_vertices(OpenSCADObject):
+class _path_path_closest_vertices(_Bosl2Base):
     def __init__(self, path1=None, path2=None, **kwargs):
        super().__init__("_path_path_closest_vertices", {"path1" : path1, "path2" : path2, **kwargs})
 
-class _join_paths_at_vertices(OpenSCADObject):
+class _join_paths_at_vertices(_Bosl2Base):
     def __init__(self, path1=None, path2=None, v1=None, v2=None, **kwargs):
        super().__init__("_join_paths_at_vertices", {"path1" : path1, "path2" : path2, "v1" : v1, "v2" : v2, **kwargs})
 
-class _cleave_connected_region(OpenSCADObject):
+class _cleave_connected_region(_Bosl2Base):
     def __init__(self, region=None, eps=None, **kwargs):
        super().__init__("_cleave_connected_region", {"region" : region, "eps" : eps, **kwargs})
 
-class _polyHoles(OpenSCADObject):
+class _polyHoles(_Bosl2Base):
     def __init__(self, outer=None, holes=None, extremes=None, eps=None, n=None, **kwargs):
        super().__init__("_polyHoles", {"outer" : outer, "holes" : holes, "extremes" : extremes, "eps" : eps, "n" : n, **kwargs})
 
-class _bridge(OpenSCADObject):
+class _bridge(_Bosl2Base):
     def __init__(self, pt=None, outer=None, eps=None, **kwargs):
        super().__init__("_bridge", {"pt" : pt, "outer" : outer, "eps" : eps, **kwargs})
 
-class vnf_from_region(OpenSCADObject):
+class vnf_from_region(_Bosl2Base):
     def __init__(self, region=None, transform=None, reverse=None, **kwargs):
        super().__init__("vnf_from_region", {"region" : region, "transform" : transform, "reverse" : reverse, **kwargs})
 
-class is_vnf(OpenSCADObject):
+class is_vnf(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("is_vnf", {"x" : x, **kwargs})
 
-class is_vnf_list(OpenSCADObject):
+class is_vnf_list(_Bosl2Base):
     def __init__(self, x=None, **kwargs):
        super().__init__("is_vnf_list", {"x" : x, **kwargs})
 
-class vnf_vertices(OpenSCADObject):
+class vnf_vertices(_Bosl2Base):
     def __init__(self, vnf=None, **kwargs):
        super().__init__("vnf_vertices", {"vnf" : vnf, **kwargs})
 
-class vnf_faces(OpenSCADObject):
+class vnf_faces(_Bosl2Base):
     def __init__(self, vnf=None, **kwargs):
        super().__init__("vnf_faces", {"vnf" : vnf, **kwargs})
 
-class vnf_reverse_faces(OpenSCADObject):
+class vnf_reverse_faces(_Bosl2Base):
     def __init__(self, vnf=None, **kwargs):
        super().__init__("vnf_reverse_faces", {"vnf" : vnf, **kwargs})
 
-class vnf_quantize(OpenSCADObject):
+class vnf_quantize(_Bosl2Base):
     def __init__(self, vnf=None, q=None, **kwargs):
        super().__init__("vnf_quantize", {"vnf" : vnf, "q" : q, **kwargs})
 
-class vnf_merge_points(OpenSCADObject):
+class vnf_merge_points(_Bosl2Base):
     def __init__(self, vnf=None, eps=None, **kwargs):
        super().__init__("vnf_merge_points", {"vnf" : vnf, "eps" : eps, **kwargs})
 
-class vnf_drop_unused_points(OpenSCADObject):
+class vnf_drop_unused_points(_Bosl2Base):
     def __init__(self, vnf=None, **kwargs):
        super().__init__("vnf_drop_unused_points", {"vnf" : vnf, **kwargs})
 
-class _link_indicator(OpenSCADObject):
+class _link_indicator(_Bosl2Base):
     def __init__(self, l=None, imin=None, imax=None, **kwargs):
        super().__init__("_link_indicator", {"l" : l, "imin" : imin, "imax" : imax, **kwargs})
 
-class vnf_triangulate(OpenSCADObject):
+class vnf_triangulate(_Bosl2Base):
     def __init__(self, vnf=None, **kwargs):
        super().__init__("vnf_triangulate", {"vnf" : vnf, **kwargs})
 
-class vnf_slice(OpenSCADObject):
+class vnf_slice(_Bosl2Base):
     def __init__(self, vnf=None, dir=None, cuts=None, **kwargs):
        super().__init__("vnf_slice", {"vnf" : vnf, "dir" : dir, "cuts" : cuts, **kwargs})
 
-class _split_polygon_at_x(OpenSCADObject):
+class _split_polygon_at_x(_Bosl2Base):
     def __init__(self, poly=None, x=None, **kwargs):
        super().__init__("_split_polygon_at_x", {"poly" : poly, "x" : x, **kwargs})
 
-class _split_2dpolygons_at_each_x(OpenSCADObject):
+class _split_2dpolygons_at_each_x(_Bosl2Base):
     def __init__(self, polys=None, xs=None, _i=None, **kwargs):
        super().__init__("_split_2dpolygons_at_each_x", {"polys" : polys, "xs" : xs, "_i" : _i, **kwargs})
 
-class _slice_3dpolygons(OpenSCADObject):
+class _slice_3dpolygons(_Bosl2Base):
     def __init__(self, polys=None, dir=None, cuts=None, **kwargs):
        super().__init__("_slice_3dpolygons", {"polys" : polys, "dir" : dir, "cuts" : cuts, **kwargs})
 
-class vnf_volume(OpenSCADObject):
+class vnf_volume(_Bosl2Base):
     def __init__(self, vnf=None, **kwargs):
        super().__init__("vnf_volume", {"vnf" : vnf, **kwargs})
 
-class vnf_area(OpenSCADObject):
+class vnf_area(_Bosl2Base):
     def __init__(self, vnf=None, **kwargs):
        super().__init__("vnf_area", {"vnf" : vnf, **kwargs})
 
-class _vnf_centroid(OpenSCADObject):
+class _vnf_centroid(_Bosl2Base):
     def __init__(self, vnf=None, eps=None, **kwargs):
        super().__init__("_vnf_centroid", {"vnf" : vnf, "eps" : eps, **kwargs})
 
-class vnf_halfspace(OpenSCADObject):
+class vnf_halfspace(_Bosl2Base):
     def __init__(self, plane=None, vnf=None, closed=None, **kwargs):
        super().__init__("vnf_halfspace", {"plane" : plane, "vnf" : vnf, "closed" : closed, **kwargs})
 
-class _assemble_paths(OpenSCADObject):
+class _assemble_paths(_Bosl2Base):
     def __init__(self, vertices=None, edges=None, paths=None, i=None, **kwargs):
        super().__init__("_assemble_paths", {"vertices" : vertices, "edges" : edges, "paths" : paths, "i" : i, **kwargs})
 
-class _vnfcut(OpenSCADObject):
+class _vnfcut(_Bosl2Base):
     def __init__(self, plane=None, vertices=None, vertexmap=None, inside=None, faces=None, vertcount=None, newfaces=None, newedges=None, newvertices=None, i=None, **kwargs):
        super().__init__("_vnfcut", {"plane" : plane, "vertices" : vertices, "vertexmap" : vertexmap, "inside" : inside, "faces" : faces, "vertcount" : vertcount, "newfaces" : newfaces, "newedges" : newedges, "newvertices" : newvertices, "i" : i, **kwargs})
 
-class _triangulate_planar_convex_polygons(OpenSCADObject):
+class _triangulate_planar_convex_polygons(_Bosl2Base):
     def __init__(self, polys=None, **kwargs):
        super().__init__("_triangulate_planar_convex_polygons", {"polys" : polys, **kwargs})
 
-class vnf_bend(OpenSCADObject):
+class vnf_bend(_Bosl2Base):
     def __init__(self, vnf=None, r=None, d=None, axis=None, **kwargs):
        super().__init__("vnf_bend", {"vnf" : vnf, "r" : r, "d" : d, "axis" : axis, **kwargs})
 
-class vnf_validate(OpenSCADObject):
+class vnf_validate(_Bosl2Base):
     def __init__(self, vnf=None, show_warns=None, check_isects=None, **kwargs):
        super().__init__("vnf_validate", {"vnf" : vnf, "show_warns" : show_warns, "check_isects" : check_isects, **kwargs})
 
-class _vnf_validate_err(OpenSCADObject):
+class _vnf_validate_err(_Bosl2Base):
     def __init__(self, name=None, extra=None, **kwargs):
        super().__init__("_vnf_validate_err", {"name" : name, "extra" : extra, **kwargs})
 
-class _pts_not_reported(OpenSCADObject):
+class _pts_not_reported(_Bosl2Base):
     def __init__(self, pts=None, varr=None, reports=None, **kwargs):
        super().__init__("_pts_not_reported", {"pts" : pts, "varr" : varr, "reports" : reports, **kwargs})
 
-class _edge_not_reported(OpenSCADObject):
+class _edge_not_reported(_Bosl2Base):
     def __init__(self, edge=None, varr=None, reports=None, **kwargs):
        super().__init__("_edge_not_reported", {"edge" : edge, "varr" : varr, "reports" : reports, **kwargs})
 
+class vnf_polyhedron(_Bosl2Base):
+    def __init__(self, vnf=None, convexity=None, extent=None, cp=None, anchor=None, spin=None, orient=None, atype=None, **kwargs):
+       super().__init__("vnf_polyhedron", {"vnf" : vnf, "convexity" : convexity, "extent" : extent, "cp" : cp, "anchor" : anchor, "spin" : spin, "orient" : orient, "atype" : atype, **kwargs})
+
+class vnf_wireframe(_Bosl2Base):
+    def __init__(self, vnf=None, width=None, **kwargs):
+       super().__init__("vnf_wireframe", {"vnf" : vnf, "width" : width, **kwargs})
+
+class _show_vertices(_Bosl2Base):
+    def __init__(self, vertices=None, size=None, **kwargs):
+       super().__init__("_show_vertices", {"vertices" : vertices, "size" : size, **kwargs})
+
+class _show_faces(_Bosl2Base):
+    def __init__(self, vertices=None, faces=None, size=None, **kwargs):
+       super().__init__("_show_faces", {"vertices" : vertices, "faces" : faces, "size" : size, **kwargs})
+
+class debug_vnf(_Bosl2Base):
+    def __init__(self, vnf=None, faces=None, vertices=None, opacity=None, size=None, convexity=None, **kwargs):
+       super().__init__("debug_vnf", {"vnf" : vnf, "faces" : faces, "vertices" : vertices, "opacity" : opacity, "size" : size, "convexity" : convexity, **kwargs})
+
+class vnf_validate(_Bosl2Base):
+    def __init__(self, vnf=None, size=None, show_warns=None, check_isects=None, **kwargs):
+       super().__init__("vnf_validate", {"vnf" : vnf, "size" : size, "show_warns" : show_warns, "check_isects" : check_isects, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/walls.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/walls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/walls.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class sparse_wall(OpenSCADObject):
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/walls.scad'}", use_not_include=False)
+
+class sparse_wall(_Bosl2Base):
     def __init__(self, h=None, l=None, thick=None, maxang=None, strut=None, max_bridge=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("sparse_wall", {"h" : h, "l" : l, "thick" : thick, "maxang" : maxang, "strut" : strut, "max_bridge" : max_bridge, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class corrugated_wall(OpenSCADObject):
+class corrugated_wall(_Bosl2Base):
     def __init__(self, h=None, l=None, thick=None, strut=None, wall=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("corrugated_wall", {"h" : h, "l" : l, "thick" : thick, "strut" : strut, "wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class thinning_wall(OpenSCADObject):
+class thinning_wall(_Bosl2Base):
     def __init__(self, h=None, l=None, thick=None, ang=None, braces=None, strut=None, wall=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("thinning_wall", {"h" : h, "l" : l, "thick" : thick, "ang" : ang, "braces" : braces, "strut" : strut, "wall" : wall, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class thinning_triangle(OpenSCADObject):
+class thinning_triangle(_Bosl2Base):
     def __init__(self, h=None, l=None, thick=None, ang=None, strut=None, wall=None, diagonly=None, center=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("thinning_triangle", {"h" : h, "l" : l, "thick" : thick, "ang" : ang, "strut" : strut, "wall" : wall, "diagonly" : diagonly, "center" : center, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
 
-class narrowing_strut(OpenSCADObject):
+class narrowing_strut(_Bosl2Base):
     def __init__(self, w=None, l=None, wall=None, ang=None, anchor=None, spin=None, orient=None, **kwargs):
        super().__init__("narrowing_strut", {"w" : w, "l" : l, "wall" : wall, "ang" : ang, "anchor" : anchor, "spin" : spin, "orient" : orient, **kwargs})
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/bosl2/wiring.py` & `solidpython2-2.0.0b4/solid2/extensions/bosl2/wiring.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from solid2.core.object_base import OpenSCADObject, OpenSCADConstant
-from solid2.core.scad_import import extra_scad_include
-from pathlib import Path
+from solid2.core.object_base import OpenSCADConstant as _OpenSCADConstant
+from solid2.core.scad_import import extra_scad_include as _extra_scad_include
+from pathlib import Path as _Path
 
-extra_scad_include(f"{Path(__file__).parent.parent / '../libs/BOSL2/wiring.scad'}", use_not_include=False)
+from .bosl2_base import Bosl2Base as _Bosl2Base
 
-class wire_bundle(OpenSCADObject):
-    def __init__(self, path=None, wires=None, wirediam=None, rounding=None, wirenum=None, corner_steps=None, **kwargs):
-       super().__init__("wire_bundle", {"path" : path, "wires" : wires, "wirediam" : wirediam, "rounding" : rounding, "wirenum" : wirenum, "corner_steps" : corner_steps, **kwargs})
+_extra_scad_include(f"{_Path(__file__).parent.parent / '../libs/BOSL2/wiring.scad'}", use_not_include=False)
 
-class _hex_offset_ring(OpenSCADObject):
+class _hex_offset_ring(_Bosl2Base):
     def __init__(self, d=None, lev=None, **kwargs):
        super().__init__("_hex_offset_ring", {"d" : d, "lev" : lev, **kwargs})
 
-class _hex_offsets(OpenSCADObject):
+class _hex_offsets(_Bosl2Base):
     def __init__(self, n=None, d=None, lev=None, arr=None, **kwargs):
        super().__init__("_hex_offsets", {"n" : n, "d" : d, "lev" : lev, "arr" : arr, **kwargs})
 
+class wire_bundle(_Bosl2Base):
+    def __init__(self, path=None, wires=None, wirediam=None, rounding=None, wirenum=None, corner_steps=None, **kwargs):
+       super().__init__("wire_bundle", {"path" : path, "wires" : wires, "wirediam" : wirediam, "rounding" : rounding, "wirenum" : wirenum, "corner_steps" : corner_steps, **kwargs})
+
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/greedy_scad_interface/customizer_widgets.py` & `solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/customizer_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .scad_variable import ScadVariable
 
 class CustomizerDropdownVariable(ScadVariable):
-    def __init__(self, name, default_value, options='', label='', tab=''):
-        options_str = options
+    def __init__(self, name, default_value, options=None, label='', tab=''):
+
+        options_str = options if options else ""
         if isinstance(options, list):
             options_str = '[' + ", ".join(map(str, options)) + ']'
 
         if isinstance(options, dict):
             reverse_options = [ f'{options[k]} : "{k}"' for k in options.keys()]
             options_str = f'[{", ".join(reverse_options)}]'
```

### Comparing `solidpython2-2.0.0b3/solid2/extensions/greedy_scad_interface/scad_interface.py` & `solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/scad_interface.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/extensions/greedy_scad_interface/scad_variable.py` & `solidpython2-2.0.0b4/solid2/extensions/greedy_scad_interface/scad_variable.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/CONTRIBUTING.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/LICENSE` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/LICENSE`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/README.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/README.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/WRITING_DOCS.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/WRITING_DOCS.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/affine.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/affine.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/attachments.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/attachments.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/beziers.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/beziers.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/bosl1compat.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/bosl1compat.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/bottlecaps.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/bottlecaps.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/builtins.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/builtins.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/color.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/color.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/comparisons.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/comparisons.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/constants.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/constants.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/coords.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/coords.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/cubetruss.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/cubetruss.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/distributors.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/distributors.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/drawing.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/drawing.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/fnliterals.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/fnliterals.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/gears.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/gears.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/geometry.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/geometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/hingesnaps.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/hingesnaps.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/images/BOSL2logo.png` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/images/BOSL2logo.png`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/joiners.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/joiners.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/linalg.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/linalg.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/linear_bearings.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/linear_bearings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/lists.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/lists.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/masks2d.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/masks2d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/masks3d.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/masks3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/math.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/math.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/metric_screws.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/metric_screws.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/modular_hose.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/modular_hose.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/mutators.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/mutators.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/nema_steppers.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/nema_steppers.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/partitions.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/partitions.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/paths.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/paths.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/polyhedra.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/polyhedra.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/regions.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/regions.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/rounding.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/rounding.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/screw_drive.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/screw_drive.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/screws.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/screws.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/func_coverage.py` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/func_coverage.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/img2scad.py` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/img2scad.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/increment_version.sh` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/increment_version.sh`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/scripts/run_tests.sh` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/scripts/run_tests.sh`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/shapes2d.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/shapes2d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/shapes3d.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/shapes3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/skin.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/skin.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/sliders.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/sliders.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/std.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/std.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/strings.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/strings.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/structs.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/structs.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/threading.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/threading.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/transforms.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/transforms.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/trigonometry.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/trigonometry.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tripod_mounts.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tripod_mounts.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/turtle3d.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/turtle3d.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Attachments.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Attachments.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Distributors.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Distributors.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/FractalTree.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/FractalTree.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Mutators.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Mutators.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Paths.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Paths.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Shapes2d.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Shapes2d.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Shapes3d.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Shapes3d.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/Transforms.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/Transforms.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/tutorials/VNF.md` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/tutorials/VNF.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/utility.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/utility.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/vectors.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/vectors.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/version.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/version.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/vnf.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/vnf.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/walls.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/walls.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/BOSL2/wiring.scad` & `solidpython2-2.0.0b4/solid2/libs/BOSL2/wiring.scad`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/py_scadparser/LICENSE` & `solidpython2-2.0.0b4/solid2/libs/py_scadparser/LICENSE`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/py_scadparser/README.md` & `solidpython2-2.0.0b4/solid2/libs/py_scadparser/README.md`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/py_scadparser/parsetab.py` & `solidpython2-2.0.0b4/solid2/libs/py_scadparser/parsetab.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/py_scadparser/scad_ast.py` & `solidpython2-2.0.0b4/solid2/libs/py_scadparser/scad_ast.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/py_scadparser/scad_parser.py` & `solidpython2-2.0.0b4/solid2/libs/py_scadparser/scad_parser.py`

 * *Files identical despite different names*

### Comparing `solidpython2-2.0.0b3/solid2/libs/py_scadparser/scad_tokens.py` & `solidpython2-2.0.0b4/solid2/libs/py_scadparser/scad_tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 #LICENSE: BSD
 simple_escape = r"""([a-wyzA-Z._~!=&\^\-\\?'"]|x(?![0-9a-fA-F]))"""
 decimal_escape = r"""(\d+)(?!\d)"""
 hex_escape = r"""(x[0-9a-fA-F]+)(?![0-9a-fA-F])"""
 bad_escape = r"""([\\][^a-zA-Z._~^!=&\^\-\\?'"x0-9])"""
 escape_sequence = r"""(\\("""+simple_escape+'|'+decimal_escape+'|'+hex_escape+'))'
 escape_sequence_start_in_string = r"""(\\[0-9a-zA-Z._~!=&\^\-\\?'"])"""
-string_char = r"""([^"\\\n]|"""+escape_sequence_start_in_string+')'
+string_char = r"""([^"\\] | """+escape_sequence_start_in_string+')'
 t_STRING = '"'+string_char+'*"' + " | " + "'" +string_char+ "*'"
 
 t_EQUAL = "=="
 t_GREATER_OR_EQUAL = ">="
 t_LESS_OR_EQUAL = "<="
 t_NOT_EQUAL = "!="
 t_AND = r"\&\&"
```

### Comparing `solidpython2-2.0.0b3/setup.py` & `solidpython2-2.0.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['solid2',
  'solid2.core',
+ 'solid2.core.builtins',
+ 'solid2.core.object_base',
  'solid2.examples',
  'solid2.extensions',
  'solid2.extensions.bosl2',
  'solid2.extensions.greedy_scad_interface',
  'solid2.libs',
  'solid2.libs.BOSL2.scripts',
  'solid2.libs.py_scadparser']
@@ -21,15 +23,15 @@
                  'BOSL2/tutorials/*']}
 
 install_requires = \
 ['ply>=3.11,<4.0', 'setuptools>=65.6.3']
 
 setup_kwargs = {
     'name': 'solidpython2',
-    'version': '2.0.0b3',
+    'version': '2.0.0b4',
     'description': 'Python interface to the OpenSCAD declarative geometry language',
     'long_description': '\n.. image:: https://readthedocs.org/projects/solidpython2/badge/?version=latest\n    :target: http://solidpython2.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\n**If you switch from the regular SolidPython:master branch to this branch, have a\nlook at** `Version 2.x.x`_.\n\nSolidPython\n===========\n\n.. contents::\n   \nOpenSCAD for Python\n-------------------\n\nSolidPython is a generalization of Phillip Tiefenbacher\'s openscad\nmodule, found on `Thingiverse <http://www.thingiverse.com/thing:1481>`__. It\ngenerates valid OpenSCAD code from Python code with minimal overhead. Here\'s a\nsimple example:\n\nThis Python code:\n\n.. code:: python\n\n    from solid2 import *\n    d = difference()(\n        cube(10),\n        sphere(15)\n    )\n    d.as_scad()\n\nGenerates this OpenSCAD code:\n\n.. code:: python\n\n    difference(){\n        cube(10);\n        sphere(15);\n    }\n\nThat doesn\'t seem like such a savings, but the following SolidPython code is a\nlot shorter (and I think clearer) than the SCAD code it compiles to:\n\n.. code:: python\n\n    from solid2 import *\n    d = cube(5) + right(5)(sphere(5)) - cylinder(r=2, h=6)\n\nGenerates this OpenSCAD code:\n\n.. code::\n\n    difference(){\n        union(){\n            cube(5);\n            translate( [5, 0,0]){\n                sphere(5);\n            }\n        }\n        cylinder(r=2, h=6);\n    }\n\nAdvantages\n----------\n\nIn contrast to OpenSCAD -- which is a constrained domain specific language --\nPython is a full blown modern programming language and as such supports\npretty much all modern programming features. Furthermore a huge number of\nlibraries is available.\n\nSolidPython lets you use all these fancy python features to generate your\nconstructive solid geometry models.\n\nOn the one hand it makes the generation of your models a lot easier, because\nyou don\'t need to learn another domain specific language and you can use all\nthe programming technique you\'re already familiar with. On the other hand it\ngives you a lot more power, because you can use all the comprehensive python\nlibraries to generate your models.\n\nI would almost say this enables you to do what ever you want with ease.\nAs (maybe little uncommon) example, you could write a program that:\n\n  - looks up the mail adress of your actuall president (based on your ip address)\n  - writes a mail to him or her and asks for a portrait\n  - waits for a reply\n  - generates a heightmap from the picture you received and maps it onto a vase\n\nThis should be pretty straight forward with SolidPython but is impossible with\npure OpenSCAD.\n\nFurhtermore SolidPython 2.x.x is designed to be extendible. As such you can extend SolidPython itself using python. Actually parts of SolidPython itself are implemented as extensions (everything but the core one-to-one mapping of OpenScad to Python), these include operators, access style syntax, convenience functions, scad_interface and bosl2 support. Furthermore some of the SolidPython 1.x.x solid.utils features are also implemented as extensions (bill of material & part-hole).\n\nInstalling SolidPython\n----------------------\n\n-  Install latest release via\n   `PyPI <https://pypi.python.org/pypi/solidpython2>`__:\n\n   .. code:: bash\n\n       pip install solidpython2\n\n   (You may need to use ``sudo pip install solidpython2``, depending on\n   your environment. This is commonly discouraged though. You\'ll be happiest \n   working in a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`__ \n   where you can easily control dependencies for a given project)\n\n- Install current master straight from Github:\n\n  .. code:: bash\n\n      pip install git+https://github.com/jeff-dh/SolidPython\n\nUsing SolidPython\n-----------------\n\n-  Include SolidPython at the top of your Python file:\n\n   .. code:: python\n\n       from solid2 import *\n\n   (See `this issue <https://github.com/SolidCode/SolidPython/issues/114>`__ for \n   a discussion of other import styles)\n\n-  OpenSCAD uses curly-brace blocks ({}) to create its tree. SolidPython\n   uses parentheses with comma-delimited lists. \n   \n   **OpenSCAD:**\n\n   .. code::\n\n       difference(){\n           cube(10);\n           sphere(15);\n       }\n\n   **SolidPython:**\n\n   .. code::\n\n       d = difference()(\n           cube(10),  # Note the comma between each element!\n           sphere(15)\n       )\n\n-  Call ``py_scad_obj.as_scad()`` to generate SCAD code. This returns\n   a string of valid OpenSCAD code.\n-  *or*: call ``py_scad_obj.save_as_scad("filepath.scad")`` to store\n   that code in a file.\n-  If ``filepath.scad`` is open in the OpenSCAD IDE and Design => \'Automatic\n   Reload and Compile\' is checked in the OpenSCAD IDE, running\n   ``py_scad_obj.save_as_scad()`` from Python will load the object in the\n   IDE.\n-  Alternately, you could call OpenSCAD\'s command line and render\n   straight to STL.\n\nImporting OpenSCAD code\n-----------------------\n\n- Use ``solid2.import_scad(path)`` to import OpenSCAD code. Relative paths will check the current location designated in `OpenSCAD library directories <https://en.wikibooks.org/wiki/OpenSCAD_User_Manual/Libraries>`__.\n\n**Ex:** \n\n``scadfile.scad``\n\n.. code::\n\n    module box(w,h,d){\n        cube([w,h,d]);\n    }\n\n``your_file.py``\n\n.. code:: python\n\n    from solid2 import *\n\n    scadfile = import_scad(\'/path/to/scadfile.scad\') \n    b = scadfile.box(2,4,6)\n    b.save_as_scad(\'out_file.scad\')\n\n- Recursively import OpenSCAD code by calling ``import_scad()`` with a directory argument.\n\n.. code:: python\n\n    from solid2 import *\n\n    # MCAD is OpenSCAD\'s most common utility library: https://github.com/openscad/MCAD\n    # If it\'s installed for OpenSCAD (on MacOS, at: ``$HOME/Documents/OpenSCAD/libraries``)\n    mcad = import_scad(\'MCAD\')\n\n    # MCAD contains about 15 separate packages, each included as its own namespace\n    print(dir(mcad)) # => [\'bearing\', \'bitmap\', \'boxes\', etc...]\n    mount = mcad.motors.stepper_motor_mount(nema_standard=17)\n    mount.save_as_scad(\'motor_mount_file.scad\')\n\n- OpenSCAD has the ``use()`` and ``include()`` statements for importing SCAD code, and SolidPython has them, too. They pollute the global namespace, though, and you may have better luck with ``import_scad()``,\n\n**Ex:**\n\n``scadfile.scad``\n\n.. code::\n\n    module box(w,h,d){\n        cube([w,h,d]);\n    }\n\n``your_file.py``\n\n.. code:: python\n\n    from solid2 import *\n\n    # use() puts the module `box()` into the global namespace\n    use(\'/path/to/scadfile.scad\') \n    b = box(2,4,6)\n    scad_render_to_file(b, \'out_file.scad\')\n\n\nExample Code\n------------\n\nThe best way to learn how SolidPython works is to look at the included\nexample code. If you\'ve installed SolidPython, the following line of\nPython will print (the location of) the examples directory:\n\n.. code:: python\n\n    import os, solid2; print(os.path.dirname(solid2.__file__) + \'/examples\')\n        \n\nOr browse the example code on Github\n`here <https://github.com/jeff-dh/SolidPython/tree/exp_solid/solid2/examples>`__\n\nExtra syntactic sugar\n=====================\n\nBasic operators\n---------------\n\nSolidPython overrides the basic operators + and | (union), - (difference), \\*\nand & (intersection) and ~ (debug). So\n\n.. code:: python\n\n    c = cylinder(r=10, h=5) + cylinder(r=2, h=30)\n\nis the same as:\n\n.. code:: python\n\n    c = union()(\n        cylinder(r=10, h=5),\n        cylinder(r=2, h=30)\n    )\n\nLikewise:\n\n.. code:: python\n\n    c = cylinder(r=10, h=5)\n    c -= cylinder(r=2, h=30)\n\nis the same as:\n\n.. code:: python\n\n    c = difference()(\n        cylinder(r=10, h=5),\n        cylinder(r=2, h=30)\n    )\n\nAccess Style Syntax\n-------------------\n\nSince at least some people (including me) don\'t like the OpenSCAD Syntax, SolidPython 2.x.x introduces the support for the so called "Access-Style-Syntax". This enables you to call some of the SolidPython / OpenSCAD functions as member functions of any OpenSCADObject instead of wrapping it in an instance of it.\n\nIn other words, e.g. code:\n\n.. code:: python\n\n  up(10)(cube(1))\n  #is equal to\n  cube(1).up(10)\n\nThe available member functions are the following:\n\n.. code:: python\n\n  union, difference, intersection, translate, scale, rotate, mirror, resize,\n  color, offset, hull, render, projection, surface, linear_extrude,\n  rotate_extrude, debug, background, root and disable\n\nAlso the convenience functions are available:\n\n.. code:: python\n\n  up, down, left, right, forward, fwd, back, translateX, translateY, translateZ,\n  rotateX, rotateY, rotateZ, mirrorX, mirrorY, mirrorZ, scaleX, scaleY, scaleZ,\n  resizeX, resizeY, resizeZ\n\nFurthermore you can chain these functions, because they all return the transformed OpenSCADObject, e.g.:\n\n.. code:: python\n\n  cube(1).up(10).back(20).rotate(10, 0, 5).mirror(1, 0, 0).color("green").root()\n\nConvenience functions\n---------------------\n\nSolidPython includes a number of convenience functions. Currently these\ninclude:\n\nDirections for arranging things:\n\n.. code:: python\n\n  up, down, left, right, forward, fwd, back\n\nTransformations per dimension:\n\n.. code:: python\n\n  translateX, translateY, translateZ, rotateX, rotateY, rotateZ, mirrorX,\n  mirrorY, mirrorZ, resizeX, resizeY, resizeZ, scaleX, scaleY, scaleZ\n\nFurthermore the operations `translate, scale, resize, mirror, rotate, cube and square` are overwritten in a way that they accept single integer or float values as first parameter. (`translate(1, 2, 3)` equals `translate([1, 2, 3])`)\n\n.. code:: python\n\n    cylinder().rotateY(90).up(10)\n\nseems a lot clearer to me than:\n\n.. code:: python\n\n    translate([0,0,10])(\n        rotate([0, 90, 0])(\n          cylinder()\n    ))\n\nFeatures\n========\n\nBOSL2\n-----\n\nSolidPython supports -- at least -- quite a lot of the **bosl2** library. You can use it by importing the ``solid2.extensions.bosl2``. Take a look at `bosl2 example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/07-libs-bosl2.py>`_ and `mazebox example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/16-mazebox-bosl2.py>`_ to get an idea how to use it and what\'s possible.\n\nI would suggest to use it as kind of a standard library for SolidPython.\nTake a look at their `Wiki <https://github.com/revarbat/BOSL2/wiki>`_ to get an idea about it\'s features.\n\n\nAnimation, Customizer, custom Fonts, ImplicitCad, Extensions\n------------------------------------------------------------\n\nSolidPython supports the following features\n\n* native **OpenSCAD customizer** support `customizer example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/10-customizer.py>`_ `greedy scad interface example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/17-greedy-scad-interface.py>`_\n* native **OpenSCAD animation** support `animation example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/12-animation.py>`_ and `animation example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/13-animated-bouncing-ball.py>`_\n* **custom fonts** `fonts example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/11-fonts.py>`_\n* supports **ImplicitCAD** `implicitCAD example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/14-implicitCAD.py>`_ `implicitCAD example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/15-implicitCAD2.py>`_\n* SolidPython is extendible `extensions example 1 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/08-extensions.py>`_  `extension example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/09-code-attach-extension.py>`_\n\nJupyter Renderer\n================\n\nSolidPython can be rendered inside a Jupyter Notebook using ViewScad. Unfortunately the pypi version of ``viewscad`` seems to be not compatible with ``solid2``. @jreiberkyle created `this viewscad fork <https://github.com/jreiberkyle/ViewSCAD>`__ and made it work with `solid2` (`#7 <https://github.com/jeff-dh/SolidPython/issues/7>`__)\n\nVersion 2.x.x\n=============\n\nSolidPython 2.x.x is a refactored version of SolidPython 1.x.x.\nThe refactoring process was based on the following proposal:\nhttps://github.com/SolidCode/SolidPython/issues/169\n\nThe goal was to\n\n* extract the "core" from SolidPython\n* make a solid package that only contains the fundamentals (+ a few convenience features) \n* make it extendible\n* try to get complex libraries working properly (mcad, bosl, bosl2)\n* **KISS**: ``from solid2 import *`` -> imports only ~1000 lines of source code and has (almost?) all the feautres SolidPython 1.x.x has\n* be a drop in replacement for SolidPython 1.x.x -- as far as possible, see Backwards Compatibility Section\n* get all kinds of nice features working (see Features section)\n\nThe result is a refactored and in some parts rewritten version of SolidPython we would like to release as SolidPython 2.x.x. The major improvement is a code base that should be better maintainable and extendible.\n\nBesides these benefits SolidPython 2.x.x implemented quite a few nice new features (cf. Features section).\n\nFeatures\n--------\n\nSolidPython 2.x.x has support for the following new features:\n\n* **bosl2** - SolidPython is now able to handle bosl2 pretty well (don\'t know whether everything works, but quite a lot). `bosl2 example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/07-libs-bosl2.py>`_ and `mazebox example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/16-mazebox-bosl2.py>`_\n* native **OpenSCAD customizer** support `customizer example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/10-customizer.py>`_ and `greedy scad interface example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/17-greedy-scad-interface.py>`_\n* native **OpenSCAD animation** support `animation example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/12-animation.py>`_ and `animation example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/13-animated-bouncing-ball.py>`_\n* **custom fonts** `fonts example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/11-fonts.py>`_\n* supports **ImplicitCAD** `implicitCAD example <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/14-implicitCAD.py>`_ and `implicitCAD example 2 <https://github.com/jeff-dh/SolidPython/blob/exp_solid/solid2/examples/15-implicitCAD2.py>`_\n\nFurthermore it has several minor improvements, like these which are based on ideas from *posts* from the SolidPython universe:\n\n* use invert operator (~) as # in OpenSCAD `#167 <https://github.com/SolidCode/SolidPython/pull/167>`_\n* convenience function including to pass sizes as integer parameters (``translate(10, 20, 30)``) `#63 <https://github.com/SolidCode/SolidPython/pull/63#issuecomment-688171416>`_\n* *access-style* syntax: ``cube(1).up(5).rotate(45, 0, 0)`` `#66 <https://github.com/SolidCode/SolidPython/pull/66>`_ This is additional! The OpenSCAD / SolidPython style syntax is still fully supported.\n\nAnother nice little feature especially to play around and debug it is that the ``__repr__`` operator of each "OpenSCADObject" now calls ``scad_render``. With this the python shell becomes pretty good in debuging and playing around with solid code and the library itself:\n\n.. code:: python\n\n  >>> from solid2 import *\n  >>> c = cube(5)\n  >>> c.up(5)\n  translate(v = [0, 0, 5]) {\n          cube(size = 5);\n  };\n  >>> c.up(5).save_as_scad()\n  \'/home/xxx/xxx/xxx/SolidPython/expsolid_out.scad\'\n  >>>\n\nBackwards compatibility\n-----------------------\n\nSolidPython 2.x.x should be a complete and mostly backwards compatible drop in\nreplacement for SolidPython 1.x.x.\nThe backwards compatibility is not 100% as depicted by the version number.\nSomethings (and even interfaces) changed. We tried to stay as backward\ncompatible as possible.  The package should behave 98% the same as SolidPython\nunless you do some "deep access" -- that\'s by 99% chance not backwards\ncompatible (like modifying OpenSCADObjects or import internal modules).\n\nAs long as you stick to:\n\n.. code:: python\n\n  from solid2 import *\n\nyou shoul be fine.\n\n**solid.utils**\n\n``solid.utils`` consisted of convenience functions and "modelling extensions" (kind of a small third party library like `mcad, bosl, bosl2`).\nThe convenience functions are now -- or the missing ones are supposed to be -- part of `solid2.extensions.convenience` and are automatically importet with the main package.\n\nConcerning the "modelling extensions" I would actually like to get rid of them as part of the SolidPython 2.x.x package. The resons are the following:\n\n* these modelling extensions (like `extrude_along_path, splines, screw_threads, part_hole,...`) don\'t align with the (core) purpose of SolidPython as I understand it (I think SolidPython is supposed to be a python "wrapper" / interface for OpenSCAD)\n* these modelling extensions are "yet another implementation" of common modelling task that need to be maintained. I would prefere a SolidPython design where these features are outsourced into a third party library\n* SolidPython 2.x.x has a pretty good **bosl2** support and bosl2 has all (?) the features provided by `solid.utils`:\n\n  * extrude_along_path: https://github.com/revarbat/BOSL2/wiki/mutators.scad#module-path_extrude\n  * First-class Negative Space (Holes): https://github.com/revarbat/BOSL2/wiki/attachments.scad#module-diff\n  * Splines / Bezier: https://github.com/revarbat/BOSL2/wiki/beziers.scad\n  * Screw threads: https://github.com/revarbat/BOSL2/wiki/screws.scad https://github.com/revarbat/BOSL2/wiki/metric_screws.scad https://github.com/revarbat/BOSL2/wiki/threading.scad\n  * distributors: https://github.com/revarbat/BOSL2/wiki/distributors.scad\n  * bouding boxes: https://github.com/revarbat/BOSL2/wiki/mutators.scad#module-bounding_box\n  * arcs, pie slices, tubes, ...: https://github.com/revarbat/BOSL2/wiki/shapes3d.scad https://github.com/revarbat/BOSL2/wiki/drawing.scad\n  * cut models in "half" / by a plane: https://github.com/revarbat/BOSL2/wiki/mutators.scad#functionmodule-half_of\n  * attachments: https://github.com/revarbat/BOSL2/wiki/attachments.scad\n\nAnd a looooot more.....\n\nI don\'t see why SolidPython should implement and maintain its own set of these features. Furthermore I assume a third party library (like `bosl2`) is probably able to provide more sophisticated implementations than we will ever be able to provide.\n\nPlease take a look at the `bosl2` implementations. I did some very basic tests in ``examples/07-libs-bosl2.py`` and -- at least -- was able to create basic examples for the core `solid.utils` features using bosl2.\n\nI would also be fine with a python third party library that implements these features, but I would like to seperate it from SolidPython itself. The reason is to achieve a SolidPython module which is independent from it (development, bugs, maintainance) with the goal to get an as solid and stable as possible SolidPython (core) package.\n\nBUT, since I assume quite a few people out there are using `solid.utils` up until now and simply getting rid of it might cause some brouhaha, my suggestion for a compromise is the `solid_legay` extension.\n\n**solid2_legacy**\n\nThe `solid2_legacy` extension is basicly everything that used to be `solid.utils`. Furhtermore it tries to "mimic" the SolidPython 1.x.x interface. This is the effort to become as backward compatible as possible. This might for example be useful when trying to get existing SolidPython 1.x.x code running.\n\nThe `solid2_legacy` extension got extracted into a seperate repo (and pip package). You should be able to just import the package if it is installed or somewhere in your import path.\n\nIf you want to use those features import the extension and take a look at it.\n\n.. code:: python\n\n  from solid2_legacy import *\n\nAnyway SolidPython 1.x.x `imports` do not work with SolidPython 2.x.x! (see Interface changes - imoprt paths have changed)\n\nI was able to get the SolidPython 1.x.x examples running just by changing the imports and they all (except for the splines example which seems to have an internal issue) worked "out of the box".\n\n\n**Interface changes**\n\n* OpenSCAD identifier escaping:\n        * all *illegal* python idetifiers are escape with a single prepending underscore\n        * special variables ``$fn -> _fn`` (*note*: ``segments`` still works)\n        * identifier starting with a digit ``module 12ptStar() -> _12ptStar()`` (*note*: ``__12ptStar`` still works)\n        * python keywords ``module import() -> _import()`` (*note*: ``import\\_``  still works)\n\n* import paths have changed (a lot)\n    * as long as you only import the root package it should be fine, otherwise probably not\n    \n    .. code:: python\n    \n            from solid2 import * #fine\n            from solid2 import objects #crash\n            from solid2 import solidpython #crash\n            from solid2 import splines #crash\n            from solid2 import utils #crash\n\n* all extensions have been moved:\n    * solid.utils has been moved to ``solid2_legacy``. If you want to use them import that extension\n    * there are some example implementations of the part / hole feature and\n      bill of materials in ``solid2_legacy``. They seem to work but are\n      not tested extensively. Take a look at ``examples/xx_legacy*``.\n    * please take a look at the bosl2 example. BOSL2 provides many features which\n      might be alternatives.\n\n* OpenSCADObject internally changed a lot\n    If you access it directly\n    (e.g. mycube.set_modifier) this might not work. But if you import\n    ``solid2_legacy`` some dummy methods will be monkey patched onto\n    OpenSCADObject so you might be able to at least run the code, but it\n    might render not correctly.\n\n* maybe some more things I can\'t remember. Some function signatures changed\n  slightly. But as long as as you stick to the regular public interface\n  everything should be fine.\n\n\nContact\n=======\n\nEnjoy!\n\nIf you have any questions or bug reports please report them to the SolidPython\n`GitHub page <https://github.com/jeff-dh/SolidPython>`__!\n\n\n\nCheers!\n\nLicense\n=======\n\nThis library is free software; you can redistribute it and/or modify it\nunder the terms of the GNU Lesser General Public License as published by\nthe Free Software Foundation; either version 2.1 of the License, or (at\nyour option) any later version.\n\nThis library is distributed in the hope that it will be useful, but\nWITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser\nGeneral Public License for more details.\n\n`Full text of the\nlicense <http://www.gnu.org/licenses/old-licenses/lgpl-2.1.txt>`__.\n\nSome class docstrings are derived from the `OpenSCAD User Manual\n<https://en.wikibooks.org/wiki/OpenSCAD_User_Manual>`__, so \nare available under the `Creative Commons Attribution-ShareAlike License\n<https://creativecommons.org/licenses/by-sa/3.0/>`__. \n\n',
     'author': 'jeff',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jeff-dh/SolidPython',
```

### Comparing `solidpython2-2.0.0b3/PKG-INFO` & `solidpython2-2.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidpython2
-Version: 2.0.0b3
+Version: 2.0.0b4
 Summary: Python interface to the OpenSCAD declarative geometry language
 Home-page: https://github.com/jeff-dh/SolidPython
 License: LGPL-2.1
 Keywords: 3D,CAD,CSG,constructive solid geometry,geometry,modeling,OpenSCAD
 Author: jeff
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
```

