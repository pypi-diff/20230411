# Comparing `tmp/pyroll_core-2.0.1.tar.gz` & `tmp/pyroll_core-2.0.2.tar.gz`

## Comparing `pyroll_core-2.0.1.tar` & `pyroll_core-2.0.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/__init__.py
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/config.py
--rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/hooks.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/log.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/repr.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/shapes.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/disk_elements/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/disk_elements/disk_element_unit.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/disk_elements/hookimpls.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/__init__.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/base.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/flat.py
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/generic_elongation.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/generic_elongation_solvers.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/hexagonal.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/spline.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/boxes/__init__.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/boxes/box.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/boxes/constricted_box.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/boxes/upset_box.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/diamonds/__init__.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/diamonds/diamond.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/diamonds/gothic.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/diamonds/square.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/__init__.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/circular_oval.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/constricted_circular_oval.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/constricted_swedish_oval.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/flat_oval.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/oval_3radii.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/oval_3radii_flanked.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/swedish_oval.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/ovals/upset_oval.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/rounds/__init__.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/rounds/false_round.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/grooves/rounds/round.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/profile/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/profile/hookimpls.py
--rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/profile/profile.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll/__init__.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll/hookimpls.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll/roll.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/__init__.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/deformation_unit.py
--rw-r--r--   0        0        0     6458 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/roll_pass.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/three_roll_pass.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/__init__.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/deformation_unit.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/disk_element.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/helpers.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/profile.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/roll.py
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/roll_pass.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/rotator/__init__.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/rotator/hookimpls.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/rotator/rotator.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/sequence/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/sequence/hookimpls.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/sequence/sequence.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/transport/__init__.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/transport/hookimpls.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/transport/transport.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/unit/__init__.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/unit/hookimpls.py
--rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyroll/core/unit/unit.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/.gitignore
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/LICENSE
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/README.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/hatch.toml
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 pyroll_core-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/__init__.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/config.py
+-rw-r--r--   0        0        0    14207 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/hooks.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/log.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/repr.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/shapes.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/disk_elements/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/disk_elements/disk_element_unit.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/disk_elements/hookimpls.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/__init__.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/base.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/flat.py
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/generic_elongation.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/generic_elongation_solvers.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/hexagonal.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/spline.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/boxes/__init__.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/boxes/box.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/boxes/constricted_box.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/boxes/upset_box.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/diamonds/__init__.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/diamonds/diamond.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/diamonds/gothic.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/diamonds/square.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/__init__.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/circular_oval.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/constricted_circular_oval.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/constricted_swedish_oval.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/flat_oval.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/oval_3radii.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/oval_3radii_flanked.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/swedish_oval.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/ovals/upset_oval.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/rounds/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/rounds/false_round.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/grooves/rounds/round.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/profile/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/profile/hookimpls.py
+-rw-r--r--   0        0        0    13141 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/profile/profile.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll/__init__.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll/hookimpls.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll/roll.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/deformation_unit.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/roll_pass.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/three_roll_pass.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/__init__.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/deformation_unit.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/disk_element.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/helpers.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/profile.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/roll.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/roll_pass.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/rotator/__init__.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/rotator/hookimpls.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/rotator/rotator.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/sequence/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/sequence/hookimpls.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/sequence/sequence.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/transport/__init__.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/transport/hookimpls.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/transport/transport.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/unit/__init__.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/unit/hookimpls.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyroll/core/unit/unit.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/LICENSE
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/README.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/hatch.toml
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 pyroll_core-2.0.2/PKG-INFO
```

### Comparing `pyroll_core-2.0.1/pyroll/core/__init__.py` & `pyroll_core-2.0.2/pyroll/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .profile import Profile
 from .rotator import Rotator
 from .sequence import PassSequence
 from .hooks import Hook, HookHost, HookFunction, root_hooks
 from .disk_elements import DiskElementUnit
 from .config import Config, config
 
-VERSION = "2.0.1"
+VERSION = "2.0.2"
 
 root_hooks.update(
     {
         RollPass.roll_force,
         RollPass.Roll.roll_torque,
         Unit.OutProfile.cross_section,
         Unit.OutProfile.strain,
```

### Comparing `pyroll_core-2.0.1/pyroll/core/config.py` & `pyroll_core-2.0.2/pyroll/core/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 from typing import Optional, Iterable, Mapping, Any, Callable
 
 
 class ConfigValue:
     """Helper descriptor for storing configuration values, able to determine the value from explictly set values,
      environment variables and default values."""
 
-    def __init__(self, default, env_var: Optional[str] = None, env_var_prefix: Optional[str] = None,
-                 parser: Optional[Callable[[str], Any]] = None):
+    def __init__(
+            self,
+            default,
+            *,
+            env_var: Optional[str] = None,
+            env_var_prefix: Optional[str] = None,
+            parser: Optional[Callable[[str], Any]] = None
+    ):
         self.default = default
         self.type = type(default)
         self.parser = parser
 
         self._env_var = env_var
         self._env_var_prefix = env_var_prefix
 
@@ -27,14 +33,17 @@
         """The name of the related environment variable."""
         if self._env_var:
             return self._env_var
 
         return f"{self._env_var_prefix}_{self.name.upper()}"
 
     def __get__(self, instance, owner):
+        if instance is None:
+            return self
+
         value = getattr(instance, "_" + self.name, None)
 
         if value is not None:
             return value
 
         value = os.getenv(self.env_var, None)
 
@@ -123,15 +132,21 @@
 
         for n, v in cls.__dict__.items():
             if n.isupper() and not n.startswith("_"):
                 del cls_dict[n]
                 if not isinstance(v, ConfigValue):
                     meta_dict[n] = ConfigValue(default=v, env_var_prefix=env_var_prefix)
                 else:
-                    meta_dict[n] = ConfigValue(default=v.default, env_var_prefix=env_var_prefix)
+                    # noinspection PyProtectedMember
+                    meta_dict[n] = ConfigValue(
+                        default=v.default,
+                        env_var_prefix=env_var_prefix,
+                        env_var=v._env_var,
+                        parser=v.parser
+                    )
 
         meta = type(cls.__name__ + "Meta", (ConfigMeta,), meta_dict)
         cls = meta(cls.__name__, cls.__bases__, cls_dict)
         return cls
 
     return dec
```

### Comparing `pyroll_core-2.0.1/pyroll/core/hooks.py` & `pyroll_core-2.0.2/pyroll/core/hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import inspect
 import weakref
 from abc import ABCMeta
 from copy import deepcopy
 from functools import partial
-from typing import overload, TypeVar, Generic, List, Generator, Union
+from typing import overload, TypeVar, Generic, List, Generator, Union, Optional, Any
 
 import numpy as np
 
 from .log import LogMixin
 from .repr import ReprMixin
 
 T = TypeVar("T")
@@ -365,25 +365,35 @@
     def __attrs__(self):
         return {
             n: v
             for n, v in (self.__dict__ | self.__cache__).items()
             if not n.startswith("_") and not isinstance(v, weakref.ref)
         }
 
+    def root_hook_fallback(self, hook: Hook) -> Optional[Any]:
+        """
+        May return a fallback value for getting of root hooks.
+        The default implementation returns None, may be overridden in subclasses.
+        """
+        return None
+
     def evaluate_and_set_hooks(self):
         """Evaluate functions of root hooks and set the results explicitly as attributes."""
 
         def _gen():
             for h in root_hooks:
                 if issubclass(type(self), h.owner):
                     h = getattr(type(self), h.name)
                     result = h.get_result(self)
 
                     if result is None:
-                        continue
+                        result = self.root_hook_fallback(h)
+
+                    if result is None:
+                        raise AttributeError("Call for root hook resulted in None.")
 
                     setattr(self, h.name, result)
 
                     try:
                         arr = np.array(result)
                         yield from arr[np.isfinite(arr)].flat
                     except TypeError:  # yield only numeric values
```

### Comparing `pyroll_core-2.0.1/pyroll/core/repr.py` & `pyroll_core-2.0.2/pyroll/core/repr.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/shapes.py` & `pyroll_core-2.0.2/pyroll/core/shapes.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/disk_elements/disk_element_unit.py` & `pyroll_core-2.0.2/pyroll/core/disk_elements/disk_element_unit.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/disk_elements/hookimpls.py` & `pyroll_core-2.0.2/pyroll/core/disk_elements/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/__init__.py` & `pyroll_core-2.0.2/pyroll/core/grooves/__init__.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/base.py` & `pyroll_core-2.0.2/pyroll/core/grooves/base.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/flat.py` & `pyroll_core-2.0.2/pyroll/core/grooves/flat.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/generic_elongation.py` & `pyroll_core-2.0.2/pyroll/core/grooves/generic_elongation.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/generic_elongation_solvers.py` & `pyroll_core-2.0.2/pyroll/core/grooves/generic_elongation_solvers.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/hexagonal.py` & `pyroll_core-2.0.2/pyroll/core/grooves/hexagonal.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/spline.py` & `pyroll_core-2.0.2/pyroll/core/grooves/spline.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/boxes/box.py` & `pyroll_core-2.0.2/pyroll/core/grooves/boxes/box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/boxes/constricted_box.py` & `pyroll_core-2.0.2/pyroll/core/grooves/boxes/constricted_box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/boxes/upset_box.py` & `pyroll_core-2.0.2/pyroll/core/grooves/boxes/upset_box.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/diamonds/diamond.py` & `pyroll_core-2.0.2/pyroll/core/grooves/diamonds/diamond.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/diamonds/gothic.py` & `pyroll_core-2.0.2/pyroll/core/grooves/diamonds/gothic.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/diamonds/square.py` & `pyroll_core-2.0.2/pyroll/core/grooves/diamonds/square.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/ovals/circular_oval.py` & `pyroll_core-2.0.2/pyroll/core/grooves/ovals/circular_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/ovals/constricted_circular_oval.py` & `pyroll_core-2.0.2/pyroll/core/grooves/ovals/constricted_circular_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/ovals/constricted_swedish_oval.py` & `pyroll_core-2.0.2/pyroll/core/grooves/ovals/constricted_swedish_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/ovals/flat_oval.py` & `pyroll_core-2.0.2/pyroll/core/grooves/ovals/flat_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/ovals/oval_3radii.py` & `pyroll_core-2.0.2/pyroll/core/grooves/ovals/oval_3radii.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/ovals/oval_3radii_flanked.py` & `pyroll_core-2.0.2/pyroll/core/grooves/ovals/oval_3radii_flanked.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/ovals/swedish_oval.py` & `pyroll_core-2.0.2/pyroll/core/grooves/ovals/swedish_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/ovals/upset_oval.py` & `pyroll_core-2.0.2/pyroll/core/grooves/ovals/upset_oval.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/rounds/false_round.py` & `pyroll_core-2.0.2/pyroll/core/grooves/rounds/false_round.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/grooves/rounds/round.py` & `pyroll_core-2.0.2/pyroll/core/grooves/rounds/round.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/profile/hookimpls.py` & `pyroll_core-2.0.2/pyroll/core/profile/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/profile/profile.py` & `pyroll_core-2.0.2/pyroll/core/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/roll/hookimpls.py` & `pyroll_core-2.0.2/pyroll/core/roll/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/roll/roll.py` & `pyroll_core-2.0.2/pyroll/core/roll/roll.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/roll_pass/deformation_unit.py` & `pyroll_core-2.0.2/pyroll/core/roll_pass/deformation_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 
     contact_area = Hook[float]()
     """Area of contact of the workpiece to the rolls."""
 
     free_surface_area = Hook[float]()
     """Area of free surface."""
 
+    deformation_resistance = Hook[float]()
+    """Equivalent deformation resistance (mean flow stress increased by deformation efficiency)."""
+
     class Profile(Unit.Profile):
         """Represents a profile in context of a deformation unit."""
 
     class InProfile(Profile, Unit.InProfile):
         """Represents an incoming profile of a deformation unit."""
 
     class OutProfile(Profile, Unit.OutProfile):
```

### Comparing `pyroll_core-2.0.1/pyroll/core/roll_pass/roll_pass.py` & `pyroll_core-2.0.2/pyroll/core/roll_pass/roll_pass.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
                 label=f"Auto-Rotator for {self}",
                 duration=0, length=0, parent=self
             )
             rotator.solve(in_profile)
             in_profile = rotator.out_profile
 
         super().init_solve(in_profile)
+        self.out_profile.cross_section = self.usable_cross_section
 
     def get_root_hook_results(self):
         super_results = super().get_root_hook_results()
         roll_results = self.roll.evaluate_and_set_hooks()
 
         return np.concatenate([super_results, roll_results], axis=0)
```

### Comparing `pyroll_core-2.0.1/pyroll/core/roll_pass/three_roll_pass.py` & `pyroll_core-2.0.2/pyroll/core/roll_pass/three_roll_pass.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/deformation_unit.py` & `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/deformation_unit.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/helpers.py` & `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 def out_cross_section(rp: RollPass, width: float) -> Polygon:
     poly = Polygon(np.concatenate([cl.coords for cl in rp.contour_lines]))
     return clip_by_rect(poly, -width / 2, -math.inf, width / 2, math.inf)
 
 
-@ThreeRollPass.usable_cross_section
 def out_cross_section3(rp: ThreeRollPass, width: float) -> Polygon:
     poly = Polygon(np.concatenate([cl.coords for cl in rp.contour_lines]))
 
     for _ in range(3):
         poly = clip_by_rect(poly, -math.inf, -math.inf, math.inf, width / 2)
         poly = rotate(poly, angle=120, origin=(0, 0))
```

### Comparing `pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/profile.py` & `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,26 +53,26 @@
 def filling_ratio(self: RollPass.OutProfile):
     return self.width / self.roll_pass.usable_width
 
 
 @RollPass.OutProfile.cross_section
 def cross_section(self: RollPass.OutProfile) -> Polygon:
     cs = helpers.out_cross_section(self.roll_pass, self.width)
-    if cs.width < self.width:
+    if cs.width * 1.01 < self.width:
         raise ValueError(
             "Profile's width can not be larger than its contour lines."
             "May be caused by critical overfilling."
         )
     return cs
 
 
 @ThreeRollPass.OutProfile.cross_section
 def cross_section3(self: ThreeRollPass.OutProfile) -> Polygon:
     cs = helpers.out_cross_section3(self.roll_pass, self.width)
-    if (cs.bounds[3] - cs.centroid.y) * 2 < self.width:
+    if (cs.bounds[3] - cs.centroid.y) * 2.02 < self.width:
         raise ValueError(
             "Profile's width can not be larger than its contour lines."
             "May be caused by critical overfilling."
         )
     return cs
```

### Comparing `pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/roll.py` & `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/roll.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/roll_pass/hookimpls/roll_pass.py` & `pyroll_core-2.0.2/pyroll/core/roll_pass/hookimpls/roll_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 @RollPass.usable_width
 def usable_width(self: RollPass):
     return self.roll.groove.usable_width
 
 
 @ThreeRollPass.usable_width
 def usable_width3(self: RollPass):
-    return 2 / 3 * np.sqrt(3) * (self.roll_pass.roll.groove.usable_width + self.roll_pass.gap / 2)
+    return 2 / 3 * np.sqrt(3) * (self.roll.groove.usable_width + self.gap / 2)
 
 
 @RollPass.tip_width
 def tip_width(self):
     if isinstance(self.roll.groove, GenericElongationGroove):
         return self.roll.groove.usable_width + self.gap / 2 / np.tan(self.roll.groove.flank_angle)
```

### Comparing `pyroll_core-2.0.1/pyroll/core/rotator/hookimpls.py` & `pyroll_core-2.0.2/pyroll/core/rotator/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/rotator/rotator.py` & `pyroll_core-2.0.2/pyroll/core/rotator/rotator.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/sequence/sequence.py` & `pyroll_core-2.0.2/pyroll/core/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/transport/transport.py` & `pyroll_core-2.0.2/pyroll/core/transport/transport.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/unit/hookimpls.py` & `pyroll_core-2.0.2/pyroll/core/unit/hookimpls.py`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyroll/core/unit/unit.py` & `pyroll_core-2.0.2/pyroll/core/unit/unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,18 @@
 
     class InProfile(Profile):
         """Represents an incoming profile of a unit."""
 
     class OutProfile(Profile):
         """Represents an outgoing profile of a unit."""
 
+        def root_hook_fallback(self, hook):
+            """Copy the value from the in profile as fallback for root hooks."""
+            return getattr(self.unit.in_profile, hook.name, None)
+
     class _SubUnitsList(list):
         """Specialized list for holding the units of a pass sequence."""
 
         def __init__(self, owner: 'Unit', units: Sequence['Unit']):
             super().__init__(units)
             self._owner = weakref.ref(owner)
             for u in self:
```

### Comparing `pyroll_core-2.0.1/.gitignore` & `pyroll_core-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/LICENSE` & `pyroll_core-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/README.md` & `pyroll_core-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/pyproject.toml` & `pyroll_core-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyroll_core-2.0.1/PKG-INFO` & `pyroll_core-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroll-core
-Version: 2.0.1
+Version: 2.0.2
 Summary: PyRoll rolling simulation framework - core library.
 Project-URL: Homepage, https://pyroll-project.github.io
 Project-URL: Repository, https://github.com/pyroll-project/pyroll-core
 Project-URL: Documentation, https://pyroll.readthedocs.io/en/latest
 Author-email: Max Weiner <max.weiner@imf.tu-freiberg.de>, Christoph Renzing <christoph.renzing@imf.tu-freiberg.de>, Matthias Schmidtchen <matthias.schmidtchen@imf.tu-freiberg.de>, Max Stirl <max.stirl@imf.tu-freiberg.de>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

