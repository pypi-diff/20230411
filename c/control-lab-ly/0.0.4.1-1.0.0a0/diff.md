# Comparing `tmp/control-lab-ly-0.0.4.1.tar.gz` & `tmp/control-lab-ly-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-0.0.4.1.tar", last modified: Thu Mar 16 05:50:53 2023, max compression
+gzip compressed data, was "control-lab-ly-1.0.0a0.tar", last modified: Tue Apr 11 17:19:36 2023, max compression
```

## Comparing `control-lab-ly-0.0.4.1.tar` & `control-lab-ly-1.0.0a0.tar`

### file list

```diff
@@ -1,175 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.488346 control-lab-ly-0.0.4.1/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-0.0.4.1/LICENSE.md
--rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0    14023 2023-03-16 05:50:53.489340 control-lab-ly-0.0.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.029784 control-lab-ly-0.0.4.1/docs/
--rw-rw-rw-   0        0        0     3251 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-0.0.4.1/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-0.0.4.1/docs/LICENSE.md
--rw-rw-rw-   0        0        0     9601 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/docs/README.md
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0     1582 2023-03-16 05:50:53.491715 control-lab-ly-0.0.4.1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-0.0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:51.705959 control-lab-ly-0.0.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.086558 control-lab-ly-0.0.4.1/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    14023 2023-03-16 05:50:51.000000 control-lab-ly-0.0.4.1/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5718 2023-03-16 05:50:51.000000 control-lab-ly-0.0.4.1/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-16 05:50:51.000000 control-lab-ly-0.0.4.1/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2023-03-16 05:50:51.000000 control-lab-ly-0.0.4.1/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-16 05:50:51.000000 control-lab-ly-0.0.4.1/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.105917 control-lab-ly-0.0.4.1/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.126417 control-lab-ly-0.0.4.1/src/controllably/Analyse/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.133024 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.167668 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Database/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Database/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Database/database_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.262889 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/
--rw-rw-rw-   0        0        0      186 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/circuit_datatype.py
--rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/eis_datatype.py
--rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
--rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/eis_tests.json
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.278543 control-lab-ly-0.0.4.1/src/controllably/Analyse/Visualisation/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Visualisation/__init__.py
--rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/Visualisation/visualisation_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.311498 control-lab-ly-0.0.4.1/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.326691 control-lab-ly-0.0.4.1/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.348539 control-lab-ly-0.0.4.1/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0       47 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0     9392 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0       41 2023-02-24 14:02:28.000000 control-lab-ly-0.0.4.1/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.352252 control-lab-ly-0.0.4.1/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.393332 control-lab-ly-0.0.4.1/src/controllably/Control/GUI/
--rw-rw-rw-   0        0        0      122 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0    23122 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Control/GUI/basic_panels.py
--rw-rw-rw-   0        0        0    13985 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Control/GUI/gui_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.422814 control-lab-ly-0.0.4.1/src/controllably/Control/Schedule/
--rw-rw-rw-   0        0        0       56 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Control/Schedule/__init__.py
--rw-rw-rw-   0        0        0     1948 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Control/Schedule/schedule_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.426815 control-lab-ly-0.0.4.1/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.446097 control-lab-ly-0.0.4.1/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0       34 2023-03-10 02:02:34.000000 control-lab-ly-0.0.4.1/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    12019 2023-03-10 02:02:34.000000 control-lab-ly-0.0.4.1/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.472174 control-lab-ly-0.0.4.1/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0       31 2023-03-10 02:02:34.000000 control-lab-ly-0.0.4.1/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     8247 2023-03-10 02:02:34.000000 control-lab-ly-0.0.4.1/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.478174 control-lab-ly-0.0.4.1/src/controllably/Make/Mixture/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.498377 control-lab-ly-0.0.4.1/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0       51 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0     7579 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Make/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.508267 control-lab-ly-0.0.4.1/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.520407 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.556997 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0       73 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    20705 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     3180 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.574165 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    15439 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0       40 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0     9957 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.589059 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.622819 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0       83 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10299 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     2312 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0    11242 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.658470 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     4697 2023-03-10 02:02:34.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.716316 control-lab-ly-0.0.4.1/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0       38 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     7938 2023-03-10 02:02:34.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Measure/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.745697 control-lab-ly-0.0.4.1/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.812216 control-lab-ly-0.0.4.1/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0       68 2023-03-07 09:42:37.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9387 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     4067 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     3048 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.837891 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.874530 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0       37 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.902715 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0     4313 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0    25857 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0       35 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0     8548 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0       30 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    21484 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Move/mover_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.933863 control-lab-ly-0.0.4.1/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.973298 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:52.989217 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.028288 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0       66 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    22944 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      103 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     7597 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.056835 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0       38 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     2351 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    30378 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0       51 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0     6759 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0    15066 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.072592 control-lab-ly-0.0.4.1/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.077803 control-lab-ly-0.0.4.1/src/controllably/Transfer/Substrate/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/Transfer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.110594 control-lab-ly-0.0.4.1/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.139523 control-lab-ly-0.0.4.1/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0       59 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     1670 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.147807 control-lab-ly-0.0.4.1/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0       34 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     1755 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.175535 control-lab-ly-0.0.4.1/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-0.0.4.1/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.207659 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.225106 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.324155 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0       34 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.352798 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     1765 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0     8261 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/image_utils.py
--rw-rw-rw-   0        0        0    12178 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0      178 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.389995 control-lab-ly-0.0.4.1/src/controllably/misc/
--rw-rw-rw-   0        0        0      143 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     1926 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0    13782 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/misc/layout_utils.py
--rw-rw-rw-   0        0        0    16641 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.398994 control-lab-ly-0.0.4.1/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-0.0.4.1/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.414559 control-lab-ly-0.0.4.1/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-0.0.4.1/src/controllably/misc/templates/configs/__init__.py
--rw-rw-rw-   0        0        0      430 2023-02-24 14:02:28.000000 control-lab-ly-0.0.4.1/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-03-16 05:50:53.477341 control-lab-ly-0.0.4.1/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      512 2023-02-24 14:02:28.000000 control-lab-ly-0.0.4.1/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1460 2023-02-24 14:02:28.000000 control-lab-ly-0.0.4.1/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0     1021 2023-03-10 02:06:03.000000 control-lab-ly-0.0.4.1/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:36.154237 control-lab-ly-1.0.0a0/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0a0/LICENSE.md
+-rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/MANIFEST.in
+-rw-rw-rw-   0        0        0    13972 2023-04-11 17:19:36.157240 control-lab-ly-1.0.0a0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.610645 control-lab-ly-1.0.0a0/docs/
+-rw-rw-rw-   0        0        0     3251 2023-04-06 08:36:33.000000 control-lab-ly-1.0.0a0/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.0.0a0/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.0.0a0/docs/LICENSE.md
+-rw-rw-rw-   0        0        0     9601 2023-03-10 02:06:03.000000 control-lab-ly-1.0.0a0/docs/README.md
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/pyproject.toml
+-rw-rw-rw-   0        0        0     1542 2023-04-11 17:19:36.165240 control-lab-ly-1.0.0a0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.0.0a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.187089 control-lab-ly-1.0.0a0/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.715250 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    13972 2023-04-11 17:19:32.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7306 2023-04-11 17:19:33.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 17:19:33.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2023-04-11 17:19:33.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-11 17:19:33.000000 control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.718528 control-lab-ly-1.0.0a0/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.721526 control-lab-ly-1.0.0a0/src/controllably/Analyse/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.732654 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.750585 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Database/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Database/__init__.py
+-rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Database/database_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.814894 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/
+-rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/__init__.py
+-rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/circuit_datatype.py
+-rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_datatype.py
+-rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
+-rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_tests.json
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.823440 control-lab-ly-1.0.0a0/src/controllably/Analyse/Visualisation/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Visualisation/__init__.py
+-rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/Visualisation/visualisation_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Analyse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.852140 control-lab-ly-1.0.0a0/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.874727 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.903288 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-11 13:56:49.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    14057 2023-04-11 13:56:45.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-11 13:56:26.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8733 2023-04-11 13:56:17.000000 control-lab-ly-1.0.0a0/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:33.907295 control-lab-ly-1.0.0a0/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.031250 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/
+-rw-rw-rw-   0        0        0      516 2023-04-11 14:00:31.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    30932 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0    17704 2023-04-11 14:06:14.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0      886 2023-04-11 13:59:24.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/loader_panel.py
+-rw-rw-rw-   0        0        0     8608 2023-04-11 13:59:13.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/measurer_panel.py
+-rw-rw-rw-   0        0        0    15405 2023-04-11 13:58:21.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/mover_panel.py
+-rw-rw-rw-   0        0        0     3624 2023-04-11 13:59:00.000000 control-lab-ly-1.0.0a0/src/controllably/Control/GUI/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.063378 control-lab-ly-1.0.0a0/src/controllably/Control/Schedule/
+-rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.0.0a0/src/controllably/Control/Schedule/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-04-11 14:01:25.000000 control-lab-ly-1.0.0a0/src/controllably/Control/Schedule/schedule_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.106680 control-lab-ly-1.0.0a0/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.146597 control-lab-ly-1.0.0a0/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-11 14:04:55.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    10393 2023-04-11 14:39:53.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.181769 control-lab-ly-1.0.0a0/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-11 14:07:39.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9094 2023-04-11 14:08:32.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.208516 control-lab-ly-1.0.0a0/src/controllably/Make/Mixture/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.239790 control-lab-ly-1.0.0a0/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-11 14:09:21.000000 control-lab-ly-1.0.0a0/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0     9660 2023-04-11 14:10:14.000000 control-lab-ly-1.0.0a0/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-11 14:03:24.000000 control-lab-ly-1.0.0a0/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     3956 2023-04-11 14:04:05.000000 control-lab-ly-1.0.0a0/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.319995 control-lab-ly-1.0.0a0/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.350929 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.434609 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-04-11 14:50:27.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18015 2023-04-11 14:53:07.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7492 2023-04-11 14:52:34.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     2102 2023-04-11 14:53:27.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.453778 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      401 2023-04-11 14:54:22.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10256 2023-04-11 14:55:55.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-11 14:26:43.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.482125 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.531624 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-04-11 14:32:40.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10329 2023-04-11 14:40:14.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3163 2023-04-11 14:36:04.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2093 2023-04-11 14:34:20.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.569223 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      350 2023-04-11 14:46:27.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3973 2023-04-11 14:48:39.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-11 14:27:13.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.614198 control-lab-ly-1.0.0a0/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-11 14:29:04.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     7972 2023-04-11 14:40:46.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0      535 2023-04-11 14:28:21.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5398 2023-04-11 14:13:18.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    13804 2023-04-11 14:14:10.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4176 2023-04-11 14:24:57.000000 control-lab-ly-1.0.0a0/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.642989 control-lab-ly-1.0.0a0/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.713661 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-11 15:42:35.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9049 2023-04-11 15:43:28.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3402 2023-04-11 15:44:47.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2853 2023-04-11 15:45:04.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.740121 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.833086 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-11 15:48:58.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.865186 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24262 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15851 2023-04-11 16:10:31.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7030 2023-04-11 15:51:52.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-11 15:52:41.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-11 15:46:16.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10507 2023-04-11 15:45:49.000000 control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-11 15:40:54.000000 control-lab-ly-1.0.0a0/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32152 2023-04-11 16:11:01.000000 control-lab-ly-1.0.0a0/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.898471 control-lab-ly-1.0.0a0/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:34.954513 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.001141 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.063594 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-11 16:17:38.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3460 2023-04-11 16:21:03.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29831 2023-04-11 16:19:04.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-11 16:16:26.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     9064 2023-04-11 16:16:52.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-11 16:15:20.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.112849 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-11 16:13:12.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     3210 2023-04-11 16:12:23.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    30582 2023-04-11 16:14:25.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-11 16:04:51.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13126 2023-04-11 16:03:59.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3413 2023-04-11 16:06:49.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14619 2023-04-11 16:04:45.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.128095 control-lab-ly-1.0.0a0/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.165640 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.200245 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      348 2023-04-11 17:00:43.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8255 2023-04-11 17:04:17.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-11 16:59:01.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-04-11 16:59:39.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.269947 control-lab-ly-1.0.0a0/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.308060 control-lab-ly-1.0.0a0/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-11 16:27:05.000000 control-lab-ly-1.0.0a0/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-04-11 16:27:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.333310 control-lab-ly-1.0.0a0/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-11 16:28:38.000000 control-lab-ly-1.0.0a0/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-11 16:29:18.000000 control-lab-ly-1.0.0a0/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.355311 control-lab-ly-1.0.0a0/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.0.0a0/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.392852 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.412779 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.559395 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-11 16:29:59.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.592206 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2983 2023-04-11 16:30:36.000000 control-lab-ly-1.0.0a0/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      294 2023-04-11 16:22:53.000000 control-lab-ly-1.0.0a0/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15729 2023-04-11 16:25:00.000000 control-lab-ly-1.0.0a0/src/controllably/View/image_utils.py
+-rw-rw-rw-   0        0        0    17366 2023-04-11 16:26:02.000000 control-lab-ly-1.0.0a0/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0       98 2023-04-11 16:48:22.000000 control-lab-ly-1.0.0a0/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.759907 control-lab-ly-1.0.0a0/src/controllably/misc/
+-rw-rw-rw-   0        0        0      586 2023-04-11 15:22:32.000000 control-lab-ly-1.0.0a0/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-11 15:11:11.000000 control-lab-ly-1.0.0a0/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0    10014 2023-04-11 15:09:55.000000 control-lab-ly-1.0.0a0/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     6551 2023-04-11 15:05:56.000000 control-lab-ly-1.0.0a0/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17274 2023-04-11 15:02:50.000000 control-lab-ly-1.0.0a0/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2867 2023-04-11 15:01:48.000000 control-lab-ly-1.0.0a0/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4576 2023-04-11 15:00:29.000000 control-lab-ly-1.0.0a0/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.802402 control-lab-ly-1.0.0a0/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.818489 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.870191 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1092 2023-04-11 15:28:12.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-11 15:17:49.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:35.910020 control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-11 15:16:54.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-11 15:27:46.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-11 15:24:36.000000 control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-04-11 17:19:36.152238 control-lab-ly-1.0.0a0/tests/
+-rw-rw-rw-   0        0        0      189 2023-04-11 09:35:43.000000 control-lab-ly-1.0.0a0/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      585 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      587 2023-04-11 09:21:52.000000 control-lab-ly-1.0.0a0/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      362 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      578 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0      268 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.0.0a0/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-0.0.4.1/LICENSE.md` & `control-lab-ly-1.0.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/PKG-INFO` & `control-lab-ly-1.0.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 0.0.4.1
+Version: 1.0.0a0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -13,18 +13,17 @@
 Keywords: python,lab automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Control.lab.ly
 Lab Equipment Automation Package
 
 ## Description
```

### Comparing `control-lab-ly-0.0.4.1/docs/CHANGELOG.md` & `control-lab-ly-1.0.0a0/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.0.0a0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/docs/LICENSE.md` & `control-lab-ly-1.0.0a0/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/docs/README.md` & `control-lab-ly-1.0.0a0/docs/README.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/setup.cfg` & `control-lab-ly-1.0.0a0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
-00000020: 790d 0a76 6572 7369 6f6e 203d 2030 2e30  y..version = 0.0
-00000030: 2e34 2e31 0d0a 6465 7363 7269 7074 696f  .4.1..descriptio
+00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e30  y..version = 1.0
+00000030: 2e30 2d61 0d0a 6465 7363 7269 7074 696f  .0-a..descriptio
 00000040: 6e20 3d20 4c61 6220 4571 7569 706d 656e  n = Lab Equipmen
 00000050: 7420 4175 746f 6d61 7469 6f6e 2050 6163  t Automation Pac
 00000060: 6b61 6765 0d0a 6c6f 6e67 5f64 6573 6372  kage..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2064  iption = file: d
 00000080: 6f63 732f 5245 4144 4d45 2e6d 642c 2064  ocs/README.md, d
 00000090: 6f63 732f 4348 414e 4745 4c4f 472e 6d64  ocs/CHANGELOG.md
 000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
@@ -56,44 +56,42 @@
 00000370: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 00000380: 204d 6963 726f 736f 6674 203a 3a20 5769   Microsoft :: Wi
 00000390: 6e64 6f77 730d 0a09 5072 6f67 7261 6d6d  ndows...Programm
 000003a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
 000003b0: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
 000003c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 000003d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000003e0: 332e 370d 0a09 5072 6f67 7261 6d6d 696e  3.7...Programmin
-000003f0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000400: 7468 6f6e 203a 3a20 332e 380d 0a09 546f  thon :: 3.8...To
-00000410: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
-00000420: 632f 456e 6769 6e65 6572 696e 670d 0a0d  c/Engineering...
-00000430: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000440: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000450: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-00000460: 696e 643a 0d0a 696e 636c 7564 655f 7061  ind:..include_pa
-00000470: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
-00000480: 650d 0a70 7974 686f 6e5f 7265 7175 6972  e..python_requir
-00000490: 6573 203d 203e 3d33 2e37 0d0a 696e 7374  es = >=3.7..inst
-000004a0: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-000004b0: 0a09 6461 7368 3e3d 322e 370d 0a09 696d  ..dash>=2.7...im
-000004c0: 7065 6461 6e63 653e 3d31 2e34 0d0a 0969  pedance>=1.4...i
-000004d0: 6d75 7469 6c73 3e3d 302e 350d 0a09 6d61  mutils>=0.5...ma
-000004e0: 7470 6c6f 746c 6962 3e3d 332e 330d 0a09  tplotlib>=3.3...
-000004f0: 6e65 7374 5f61 7379 6e63 696f 3e3d 312e  nest_asyncio>=1.
-00000500: 350d 0a09 6e75 6d70 793e 3d31 2e31 390d  5...numpy>=1.19.
-00000510: 0a09 6f70 656e 6376 5f70 7974 686f 6e3e  ..opencv_python>
-00000520: 3d34 2e35 2e30 0d0a 0970 616e 6461 733e  =4.5.0...pandas>
-00000530: 3d31 2e32 0d0a 0970 6c6f 746c 793e 3d35  =1.2...plotly>=5
-00000540: 2e33 0d0a 0970 794d 6f64 6275 7354 4350  .3...pyModbusTCP
-00000550: 3e3d 302e 320d 0a09 7079 7365 7269 616c  >=0.2...pyserial
-00000560: 3e3d 332e 350d 0a09 5079 5369 6d70 6c65  >=3.5...PySimple
-00000570: 4755 493e 3d34 2e36 300d 0a09 5079 5649  GUI>=4.60...PyVI
-00000580: 5341 3e3d 312e 3132 0d0a 0950 7959 414d  SA>=1.12...PyYAM
-00000590: 4c3e 3d36 2e30 0d0a 0973 6369 7079 3e3d  L>=6.0...scipy>=
-000005a0: 312e 360d 0a0d 0a5b 6f70 7469 6f6e 732e  1.6....[options.
-000005b0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-000005c0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-000005d0: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-000005e0: 6461 7461 5d0d 0a2a 203d 202a 2e6a 736f  data]..* = *.jso
-000005f0: 6e2c 202a 2e79 616d 6c2c 202a 2e70 6e67  n, *.yaml, *.png
-00000600: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000610: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000620: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000003e0: 332e 380d 0a09 546f 7069 6320 3a3a 2053  3.8...Topic :: S
+000003f0: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000400: 6572 696e 670d 0a0d 0a5b 6f70 7469 6f6e  ering....[option
+00000410: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000420: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000430: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
+00000440: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
+00000450: 7461 203d 2054 7275 650d 0a70 7974 686f  ta = True..pytho
+00000460: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+00000470: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
+00000480: 6972 6573 203d 200d 0a09 6461 7368 3e3d  ires = ...dash>=
+00000490: 322e 370d 0a09 696d 7065 6461 6e63 653e  2.7...impedance>
+000004a0: 3d31 2e34 0d0a 0969 6d75 7469 6c73 3e3d  =1.4...imutils>=
+000004b0: 302e 350d 0a09 6d61 7470 6c6f 746c 6962  0.5...matplotlib
+000004c0: 3e3d 332e 330d 0a09 6e65 7374 5f61 7379  >=3.3...nest_asy
+000004d0: 6e63 696f 3e3d 312e 350d 0a09 6e75 6d70  ncio>=1.5...nump
+000004e0: 793e 3d31 2e31 390d 0a09 6f70 656e 6376  y>=1.19...opencv
+000004f0: 5f70 7974 686f 6e3e 3d34 2e35 2e30 0d0a  _python>=4.5.0..
+00000500: 0970 616e 6461 733e 3d31 2e32 0d0a 0970  .pandas>=1.2...p
+00000510: 6c6f 746c 793e 3d35 2e33 0d0a 0970 794d  lotly>=5.3...pyM
+00000520: 6f64 6275 7354 4350 3e3d 302e 320d 0a09  odbusTCP>=0.2...
+00000530: 7079 7365 7269 616c 3e3d 332e 350d 0a09  pyserial>=3.5...
+00000540: 5079 5369 6d70 6c65 4755 493e 3d34 2e36  PySimpleGUI>=4.6
+00000550: 300d 0a09 5079 5649 5341 3e3d 312e 3132  0...PyVISA>=1.12
+00000560: 0d0a 0950 7959 414d 4c3e 3d36 2e30 0d0a  ...PyYAML>=6.0..
+00000570: 0973 6369 7079 3e3d 312e 360d 0a0d 0a5b  .scipy>=1.6....[
+00000580: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000590: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+000005a0: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
+000005b0: 7061 636b 6167 655f 6461 7461 5d0d 0a2a  package_data]..*
+000005c0: 203d 202a 2e6a 736f 6e2c 202a 2e79 616d   = *.json, *.yam
+000005d0: 6c2c 202a 2e70 6e67 0d0a 0d0a 5b65 6767  l, *.png....[egg
+000005e0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000005f0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000600: 2030 0d0a 0d0a                            0....
```

### Comparing `control-lab-ly-0.0.4.1/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 0.0.4.1
+Version: 1.0.0a0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -13,18 +13,17 @@
 Keywords: python,lab automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Control.lab.ly
 Lab Equipment Automation Package
 
 ## Description
```

### Comparing `control-lab-ly-0.0.4.1/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.0.0a0/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -30,70 +30,86 @@
 src/controllably/Compound/LiquidMover/__init__.py
 src/controllably/Compound/LiquidMover/liquidmover_utils.py
 src/controllably/Compound/LiquidMover/Opentrons/__init__.py
 src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
 src/controllably/Control/__init__.py
 src/controllably/Control/GUI/__init__.py
 src/controllably/Control/GUI/_guibuilder.py
-src/controllably/Control/GUI/basic_panels.py
 src/controllably/Control/GUI/gui_utils.py
+src/controllably/Control/GUI/loader_panel.py
+src/controllably/Control/GUI/measurer_panel.py
+src/controllably/Control/GUI/mover_panel.py
+src/controllably/Control/GUI/viewer_panel.py
 src/controllably/Control/Schedule/__init__.py
 src/controllably/Control/Schedule/schedule_utils.py
 src/controllably/Make/__init__.py
+src/controllably/Make/make_utils.py
 src/controllably/Make/Heat/__init__.py
 src/controllably/Make/Heat/peltier_utils.py
 src/controllably/Make/Light/__init__.py
 src/controllably/Make/Light/led_utils.py
 src/controllably/Make/Mixture/__init__.py
 src/controllably/Make/ThinFilm/__init__.py
 src/controllably/Make/ThinFilm/spinner_utils.py
 src/controllably/Measure/__init__.py
+src/controllably/Measure/instrument_utils.py
+src/controllably/Measure/measure_utils.py
+src/controllably/Measure/program_utils.py
 src/controllably/Measure/Electrical/__init__.py
 src/controllably/Measure/Electrical/electrical_utils.py
 src/controllably/Measure/Electrical/Keithley/__init__.py
 src/controllably/Measure/Electrical/Keithley/keithley_device.py
+src/controllably/Measure/Electrical/Keithley/keithley_lib.py
 src/controllably/Measure/Electrical/Keithley/keithley_utils.py
 src/controllably/Measure/Electrical/Keithley/programs/__init__.py
 src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
 src/controllably/Measure/Mechanical/__init__.py
+src/controllably/Measure/Mechanical/mechanical_utils.py
 src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
 src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
 src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
 src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
 src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
 src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
 src/controllably/Measure/Physical/__init__.py
 src/controllably/Measure/Physical/balance_utils.py
 src/controllably/Move/__init__.py
-src/controllably/Move/mover_utils.py
+src/controllably/Move/move_utils.py
 src/controllably/Move/Cartesian/__init__.py
 src/controllably/Move/Cartesian/cartesian_utils.py
 src/controllably/Move/Cartesian/ender_utils.py
 src/controllably/Move/Cartesian/primitiv_utils.py
 src/controllably/Move/Jointed/__init__.py
 src/controllably/Move/Jointed/jointed_utils.py
 src/controllably/Move/Jointed/Dobot/__init__.py
-src/controllably/Move/Jointed/Dobot/dobot_attachments.py
 src/controllably/Move/Jointed/Dobot/dobot_utils.py
+src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+src/controllably/Move/Jointed/Dobot/mg400_utils.py
 src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
 src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
 src/controllably/Transfer/__init__.py
+src/controllably/Transfer/transfer_utils.py
 src/controllably/Transfer/Liquid/__init__.py
 src/controllably/Transfer/Liquid/liquid_utils.py
+src/controllably/Transfer/Liquid/syringe_lib.py
 src/controllably/Transfer/Liquid/syringe_utils.py
 src/controllably/Transfer/Liquid/Pumps/__init__.py
+src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
 src/controllably/Transfer/Liquid/Pumps/pump_utils.py
 src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
 src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
 src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
 src/controllably/Transfer/Liquid/Sartorius/__init__.py
 src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
 src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
 src/controllably/Transfer/Powder/__init__.py
 src/controllably/Transfer/Substrate/__init__.py
+src/controllably/Transfer/Substrate/substrate_utils.py
+src/controllably/Transfer/Substrate/Dobot/__init__.py
+src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
 src/controllably/View/__init__.py
 src/controllably/View/image_utils.py
 src/controllably/View/view_utils.py
 src/controllably/View/Classifiers/__init__.py
 src/controllably/View/Classifiers/classifier_utils.py
 src/controllably/View/Optical/__init__.py
 src/controllably/View/Optical/optical_utils.py
@@ -107,15 +123,39 @@
 src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
 src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
 src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
 src/controllably/View/Thermal/placeholders/__init__.py
 src/controllably/View/Thermal/placeholders/infrared_camera.png
 src/controllably/misc/__init__.py
 src/controllably/misc/decorators.py
-src/controllably/misc/layout_utils.py
+src/controllably/misc/factory.py
+src/controllably/misc/helper.py
+src/controllably/misc/layout.py
+src/controllably/misc/logger.py
 src/controllably/misc/misc_utils.py
 src/controllably/misc/templates/__init__.py
 src/controllably/misc/templates/configs/__init__.py
 src/controllably/misc/templates/configs/registry.yaml
+src/controllably/misc/templates/configs/plugins/__init__.py
+src/controllably/misc/templates/configs/plugins/plugin_template.py
 src/controllably/misc/templates/setup/__init__.py
 src/controllably/misc/templates/setup/config.yaml
-src/controllably/misc/templates/setup/layout.json
+src/controllably/misc/templates/setup/layout.json
+tests/test_camera_optical.py
+tests/test_camera_thermal.py
+tests/test_cartesian_ender.py
+tests/test_cartesian_primitiv.py
+tests/test_compound_liquidmover.py
+tests/test_compound_spin_printer.py
+tests/test_dobot_m1pro.py
+tests/test_dobot_mg400.py
+tests/test_electrical_keithley.py
+tests/test_film_spin.py
+tests/test_heat_peltier.py
+tests/test_light_led_array.py
+tests/test_liquid_sartorius.py
+tests/test_liquid_syringe_assembly.py
+tests/test_liquid_tricontinent.py
+tests/test_mechanical_piezorobotics.py
+tests/test_panels.py
+tests/test_physical_balance.py
+tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Database/database_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Database/database_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/circuit_datatype.py` & `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/circuit_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/eis_datatype.py` & `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_datatype.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml` & `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Analyse/Data/Types/eis_tests.json` & `control-lab-ly-1.0.0a0/src/controllably/Analyse/Data/Types/eis_tests.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Analyse/Visualisation/visualisation_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Analyse/Visualisation/visualisation_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,233 +1,269 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
+This module holds the base class for cartesian mover tools.
 
-Notes / actionables:
--
+Classes:
+    Gantry (Mover)
 """
 # Standard library imports
+from __future__ import annotations
 import numpy as np
 import time
+from typing import Optional
 
 # Third party imports
+import serial # pip install pyserial
 
 # Local application imports
-from ..compound_utils import CompoundSetup
+from ...misc import Helper
+from ..move_utils import Mover
 print(f"Import: OK <{__name__}>")
-
-TIP_APPROACH_HEIGHT = 20
-
-class LiquidMoverSetup(CompoundSetup):
+    
+class Gantry(Mover):
     """
-    Liquid Mover Setup routines
+    Abstract Base Class (ABC) for Gantry objects. Gantry provides controls for a general cartesian robot.
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
+    Gantry provides controls for a general cartesian robot
 
+    ### Constructor
     Args:
-        config (str): filename of config .yaml file
-        config_option (int, optional): configuration option from config file. Defaults to 0.
-        layout (str, optional): filename of config .yaml file. Defaults to None.
-        layout_dict (dict, optional): dictionary of layout. Defaults to None.
-        ignore_connections (bool, optional): whether to ignore connections and run methods. Defaults to False.
+        `port` (str): COM port address
+        `limits` (tuple[tuple[float]], optional): lower and upper limits of gantry. Defaults to ((0, 0, 0), (0, 0, 0)).
+        `safe_height` (Optional[float], optional): height at which obstacles can be avoided. Defaults to None.
+        `max_speed` (float, optional): maximum travel speed. Defaults to 250.
+    
+    ### Properties
+    - `limits` (np.ndarray):lower and upper limits of gantry
+    - `port` (str): COM port address
+    
+    ### Methods
+    #### Abstract
+    - `home`: make the robot go home
+    #### Public
+    - `disconnect`: disconnect from device
+    - `isFeasible`: checks and returns whether the target coordinate is feasible
+    - `moveBy`: move the robot by target direction
+    - `moveTo`: move the robot to target position
+    - `reset`: reset the robot
+    - `setSpeed`: set the speed of the robot
+    - `shutdown`: shutdown procedure for tool
     """
-    def __init__(self, config:str = None, layout:str = None, component_config:dict = None, layout_dict:dict = None, ignore_connections:bool = False, tip_approach_height=TIP_APPROACH_HEIGHT, **kwargs):
-        super().__init__(config, layout, component_config, layout_dict, ignore_connections, **kwargs)
-        self.tip_approach_height = tip_approach_height
-        pass
     
-    @property
-    def liquid(self):
-        return self.components.get('liquid')
-    
-    @property
-    def mover(self):
-        return self.components.get('mover')
-
-    def align(self, coordinates:tuple, offset=(0,0,0)):
+    def __init__(self, 
+        port: str, 
+        limits: tuple[tuple[float]] = ((0, 0, 0), (0, 0, 0)), 
+        safe_height: Optional[float] = None, 
+        max_speed: float = 250, # [mm/s] (i.e. 15,000 mm/min)
+        **kwargs
+    ):
         """
-        Align the end effector to the specified coordinates, while considering any addition offset
+        Instantiate the class
 
         Args:
-            coordinates (tuple): coordinates of desired location
-            offset (tuple, optional): x,y,z offset from tool tip. Defaults to (0,0,0).
+            port (str): COM port address
+            limits (tuple[tuple[float]], optional): lower and upper limits of gantry. Defaults to ((0, 0, 0), (0, 0, 0)).
+            safe_height (Optional[float], optional): height at which obstacles can be avoided. Defaults to None.
+            max_speed (float, optional): maximum travel speed. Defaults to 250.
         """
-        coordinates = np.array(coordinates) - np.array(offset)
-        if not self.mover.isFeasible(coordinates, transform=True, tool_offset=True):
-            print(f"Infeasible toolspace coordinates! {coordinates}")
-        self.mover.safeMoveTo(coordinates, ascent_speed_fraction=0.2, descent_speed_fraction=0.2)
-        self._flags['at_rest'] = False
+        super().__init__(**kwargs)
+        self._limits = ((0, 0, 0), (0, 0, 0))
+        
+        self.limits = limits
+        self._speed_max = max_speed
+        if safe_height is not None:
+            self.setHeight(safe=safe_height)
+        
+        self._connect(port)
+        self.home()
         return
     
-    def aspirateAt(self, coordinates:tuple, volume, speed=None, channel=None, **kwargs):
-        """
-        Aspirate specified volume at desired location, at target speed
+    # Properties
+    @property
+    def limits(self) -> np.ndarray:
+        return np.array(self._limits)
+    @limits.setter
+    def limits(self, value:list):
+        if len(value) != 2 or any([len(row)!=3 for row in value]):
+            raise Exception('Please input a sequence of (lower_xyz_limit, upper_xyz_limit)')
+        self._limits = ( tuple(value[0]), tuple(value[1]) )
+        return
+    
+    @property
+    def port(self) -> str:
+        return self.connection_details.get('port', '')
 
-        Args:
-            coordinates (tuple): coordinates of desired location
-            volume (int, or float): volume in uL
-            speed (int, optional): speed to aspirate at (uL/s). Defaults to None.
-            channel (int, optional): channel to use. Defaults to None.
-        """
-        if 'eject' in dir(self.liquid) and not self.liquid.isTipOn():
-            print("[aspirate] There is no tip attached.")
-            return
-        offset = self.liquid.channels[channel].offset if 'channels' in dir(self.liquid) else self.liquid.offset
-        self.align(coordinates=coordinates, offset=offset)
-        self.liquid.aspirate(volume=volume, speed=speed, channel=channel)
+    def disconnect(self):
+        """ Disconnect from device """
+        try:
+            self.device.close()
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        self.setFlag(connected=False)
         return
     
-    def attachTip(self, slot='tip_rack', tip_length=80, channel=None):
+    def isFeasible(self, 
+        coordinates: tuple[float], 
+        transform_in: bool = False, 
+        tool_offset: bool = False, 
+        **kwargs
+    ) -> bool:
         """
-        Attach new pipette tip
+        Checks and returns whether the target coordinate is feasible
 
         Args:
-            slot (str, optional): name of slot with pipette tips. Defaults to 'tip_rack'.
-            tip_length (int, optional): length of pipette tip. Defaults to 80.
-            channel (int, optional): channel to use. Defaults to None.
-        
+            coordinates (tuple[float]): target coordinates
+            transform_in (bool, optional): whether to convert to internal coordinates first. Defaults to False.
+            tool_offset (bool, optional): whether to convert from tool tip coordinates first. Defaults to False.
+
         Returns:
-            tuple: coordinates of top of tip rack well
+            bool: whether the target coordinate is feasible
         """
-        next_tip_location, tip_length = self.positions.get(slot, [(0,0,0), tip_length]).pop(0)
-        return self.attachTipAt(next_tip_location, tip_length=tip_length, channel=channel)
-    
-    def attachTipAt(self, coordinates:tuple, tip_length=80, channel=None):
+        if transform_in:
+            coordinates = self._transform_in(coordinates=coordinates, tool_offset=tool_offset)
+        coordinates = np.array(coordinates)
+        l_bound, u_bound = self.limits
+        
+        if all(np.greater_equal(coordinates, l_bound)) and all(np.less_equal(coordinates, u_bound)):
+            return not self.deck.is_excluded(self._transform_out(coordinates, tool_offset=True))
+        print(f"Range limits reached! {self.limits}")
+        return False
+
+    def moveBy(self, vector:tuple[float], **kwargs) -> bool:
         """
-        Attach new pipette tip from specified location
+        Move the robot by target direction
 
         Args:
-            coordinates (tuple): coordinates of pipette tip
-            tip_length (int, optional): length of pipette tip. Defaults to 80.
-            channel (int, optional): channel to use. Defaults to None.
-            
+            vector (tuple[float]): x,y,z vector to move in
+
         Returns:
-            tuple: coordinates of attach tip location
+            bool: whether the movement is successful
         """
-        if 'eject' not in dir(self.liquid):
-            print("'attachTip' method not available.")
-            return coordinates
-        if self.liquid.isTipOn():
-            print("Please eject current tip before attaching new tip.")
-            return coordinates
-        self.align(coordinates)
-        self.mover.move('z', -self.tip_approach_height, speed_fraction=0.01)
-        time.sleep(3)
-        self.liquid.tip_length = tip_length
-        self.mover.implement_offset = tuple(np.array(self.mover.implement_offset) + np.array([0,0,-tip_length]))
-        self.mover.move('z', self.tip_approach_height+tip_length, speed_fraction=0.2)
-        time.sleep(1)
-        self.liquid.setFlag('tip_on', True)
-        if not self.liquid.isTipOn():
-            tip_length = self.liquid.tip_length
-            self.mover.implement_offset = tuple(np.array(self.mover.implement_offset) - np.array([0,0,-tip_length]))
-            self.liquid.tip_length = 0
-            self.liquid.setFlag('tip_on', False)
-        self._temp_tip_home = coordinates
-        return coordinates
-    
-    def dispenseAt(self, coordinates, volume, speed=None, channel=None, **kwargs):
-        """
-        Dispense specified volume at desired location, at target speed
-
-        Args:
-            coordinates (tuple): coordinates of desired location
-            volume (int, or float): volume in uL
-            speed (int, optional): speed to dispense at (uL/s). Defaults to None.
-            channel (int, optional): channel to use. Defaults to None.
-        """
-        if 'eject' in dir(self.liquid) and not self.liquid.isTipOn():
-            print("[dispense] There is no tip attached.")
-            return
-        offset = self.liquid.channels[channel].offset if 'channels' in dir(self.liquid) else self.liquid.offset
-        self.align(coordinates=coordinates, offset=offset)
-        self.liquid.dispense(volume=volume, speed=speed, channel=channel)
-        return
+        return super().moveBy(vector=vector)
     
-    def ejectTip(self, slot='bin', channel=None):
+    @Helper.safety_measures
+    def moveTo(self, coordinates:tuple[float], tool_offset:bool = True, **kwargs) -> bool:
         """
-        Eject the pipette tip at the specified location
+        Move the robot to target position
 
         Args:
-            slot (str, optional): name of slot with bin. Defaults to 'bin'.
-            channel (int, optional): channel to use. Defaults to None.
-            
-        Raises:
-            Exception: No bin location specified.
-            
+            coordinates (tuple[float]): x,y,z coordinates to move to
+            tool_offset (bool, optional): whether to consider tooltip offset. Defaults to True.
+
         Returns:
-            tuple: coordinates of top of bin well
+            bool: whether movement is successful
         """
-        bin_location,_ = self.positions.get(slot, [(None, 0)])[0]
-        if bin_location is None:
-            raise Exception("No bin location specified.")
-        return self.ejectTipAt(bin_location, channel=channel)
+        coordinates = np.array(self._transform_in(coordinates=coordinates, tool_offset=tool_offset))
+        if not self.isFeasible(coordinates):
+            return False
+            
+        z_first = True if (self.coordinates[2] < coordinates[2]) else False
+        positionXY = f'X{coordinates[0]}Y{coordinates[1]}'
+        position_Z = f'Z{coordinates[2]}'
+        moves = [position_Z, positionXY] if z_first else [positionXY, position_Z]
+        
+        self._query("G90\n")
+        for move in moves:
+            self._query(f"G0 {move}\n")
+        self._query("G90\n")
+        
+        distances = abs(self.coordinates - coordinates)
+        times = distances / self.speed
+        move_time = max(times[:2]) + times[2]
+        time.sleep(move_time)
+        self.updatePosition(coordinates=coordinates)
+        return True
     
-    def ejectTipAt(self, coordinates, channel=None):
+    def reset(self):
+        """Reset the robot"""
+        self.disconnect()
+        self.connect()
+        return super().reset()
+    
+    def setSpeed(self, speed: int): # NOTE: waiting for PR #48
         """
-        Eject the pipette tip at the specified location
+        Set the speed of the robot
 
         Args:
-            coordinates (tuple): coordinate of where to eject tip
-            channel (int, optional): channel to use. Defaults to None.
-            
-        Returns:
-            tuple: coordinates of eject tip location
+            speed (int): speed in mm/s
         """
-        if 'eject' not in dir(self.liquid):
-            print("'ejectTip' method not available.")
-            return coordinates
-        if not self.liquid.isTipOn():
-            print("There is currently no tip to eject.")
-            tip_length = self.liquid.tip_length
-            self.mover.implement_offset = tuple(np.array(self.mover.implement_offset) - np.array([0,0,-tip_length]))
-            self.liquid.tip_length = 0
-            return coordinates
-        self.align(coordinates=coordinates)
-        time.sleep(1)
-        self.liquid.eject()
-        tip_length = self.liquid.tip_length
-        self.mover.implement_offset = tuple(np.array(self.mover.implement_offset) - np.array([0,0,-tip_length]))
-        self.liquid.tip_length = 0
-        self.liquid.setFlag('tip_on', False)
-        return coordinates
+        print(f'Speed: {speed} mm/s')
+        self._speed_fraction = (speed/self._speed_max)
+        speed = int(self._speed_max*self._speed_fraction * 60)   # get speed in mm/min
+        self._query(f"G01 F{speed}\n")  # feed rate (i.e. speed) in mm/min
+        return False, self.speed
+    
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        # self.home()
+        return super().shutdown()
     
-    def loadDeck(self, layout:str = None, layout_dict:dict = None):
+    # Protected method(s)
+    def _connect(self, port:str, baudrate:int = 115200, timeout:int = 1):
         """
-        Load the deck layout from JSON file
-        
+        Connection procedure for tool
+
         Args:
-            layout (str, optional): filename of layout .json file. Defaults to None.
-            layout_dict (dict, optional): dictionary of layout. Defaults to None.
-        """
-        super().loadDeck(layout, layout_dict)
-        self.mover.loadDeck(layout, layout_dict)
-        return
-    
-    def reset(self):
-        """
-        Alias for rest
-        """
-        # Empty liquids
-        self.rest()
+            port (str): COM port address
+            baudrate (int, optional): baudrate. Defaults to 115200.
+            timeout (int, optional): timeout in seconds. Defaults to 1.
+        """
+        self.connection_details = {
+            'port': port,
+            'baudrate': baudrate,
+            'timeout': timeout
+        }
+        device = None
+        try:
+            device = serial.Serial(port, baudrate, timeout=timeout)
+        except Exception as e:
+            print(f"Could not connect to {port}")
+            if self.verbose:
+                print(e)
+        else:
+            time.sleep(2)
+            print(f"Connection opened to {port}")
+            self.setFlag(connected=True)
+        self.device = device
         return
-    
-    def rest(self):
+
+    def _query(self, command:str) -> str:
         """
-        Go back to the rest position, or home
+        Write command to and read response from device
+
+        Args:
+            command (str): command string to send to device
+
+        Returns:
+            str: response string from device
         """
-        if self._flags['at_rest']:
-            return
-        rest_coordinates = self.positions.get('rest', self.mover._transform_out((self.mover.home_coordinates)))
-        self.align(coordinates=rest_coordinates)
-        self._flags['at_rest'] = True
-        return
-    
-    def returnTip(self):
+        response = ''
+        self._write(command)
+        try:
+            response = self.device.readline()
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        else:
+            print(response)
+        return response
+
+    def _write(self, command:str) -> bool:
         """
-        Return current tip to its original rack position
+        Write command to device
+
+        Args:
+            command (str): command string to send to device
 
         Returns:
-            tuple: coordinates of eject tip location
+            bool: whether the command is sent successfully
         """
-        coordinates = self.__dict__.pop('_temp_tip_home')
-        return self.ejectTipAt(coordinates=(*coordinates[:2],coordinates[2]-18))
-    
+        if self.verbose:
+            print(command)
+        try:
+            self.device.write(command.encode('utf-8'))
+        except Exception as e:
+            if self.verbose:
+                print(e)
+            return False
+        return True
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/gui_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,159 +1,165 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/30 10:30:00
-@author: Chang Jie
+This module holds the base class for control panels as well as compound panels.
 
-Notes / actionables:
-- 
+Classes:
+    Panel (ABC)
+    CompoundPanel (Panel)
+    
+Other constants and variables:
+    HEIGHT (int): height of screen size in number of pixels
+    WIDTH (int): width of screen size in number of pixels
 """
 # Standard library imports
+from __future__ import annotations
+from abc import ABC, abstractmethod
 from collections import OrderedDict
+from typing import Optional, Union
 
 # Third party imports
 import PySimpleGUI as sg # pip install PySimpleGUI
 from PySimpleGUI import WIN_CLOSED, WINDOW_CLOSE_ATTEMPTED_EVENT
 
 # Local application imports
 print(f"Import: OK <{__name__}>")
 
 WIDTH, HEIGHT = sg.Window.get_screen_size()
-THEME = 'LightGreen'
-TYPEFACE = "Helvetica"
-FONT_SIZES = [14,12,10,8,6]
 
-class Panel(object):
-    def __init__(self, name='', theme=THEME, typeface=TYPEFACE, font_sizes=FONT_SIZES, group=None):
+class Panel(ABC):
+    """
+    Abstract Base Class (ABC) for Panel objects (i.e. GUI panels).
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
+
+    ### Constructor
+    Args:
+        `name` (str, optional): name of panel. Defaults to ''.
+        `group` (Optional[str], optional): name of group. Defaults to None.
+        `font_sizes` (tuple[int], optional): list of font sizes. Defaults to (14,12,10,8,6).
+        `theme` (str, optional): name of theme. Defaults to 'LightGreen'.
+        `typeface` (str, optional): name of typeface. Defaults to "Helvetica".
+
+    ### Attributes
+    #### Class
+    - `font_sizes` (tuple[int]): list of font sizes
+    - `theme` (str): name of theme
+    - `typeface` (str): name of typeface
+    #### Instance
+    - `flags` (dict[str, bool]): keywords paired with boolean flags
+    - `group` (str): name of group
+    - `name` (str): name of panel
+    - `tool` (Callable): tool to be controlled
+    - `window` (sg.Window): Window object
+    
+    ### Methods
+    #### Abstract
+    - `getLayout`: build `sg.Column` object
+    - `listenEvents`: listen to events and act on values
+    #### Public
+    - `arrangeElements`: arrange elements in a horizontal, vertical, or cross-shape pattern
+    - `close`: exit the application
+    - `configure`: configure GUI defaults
+    - `getButtons`: get a list of panel buttons
+    - `getWindow`: build `sg.Window` object
+    - `pad`: add spacer in GUI
+    - `parseInput`: parse inputs from GUI
+    - `runGUI`: run the GUI loop
+    - `setFlag`: set flags by using keyword arguments
+    """
+    
+    font_sizes: tuple[int]
+    theme: str
+    typeface: str
+    _default_flags: dict[str, bool] = {}
+    def __init__(self, 
+        name: str = '', 
+        group: Optional[str] = None,
+        font_sizes: tuple[int] = (14,12,10,8,6),
+        theme: str = 'LightGreen', 
+        typeface: str = "Helvetica"
+    ):
         """
-        Panel class
+        Instantiate the class
 
         Args:
             name (str, optional): name of panel. Defaults to ''.
-            theme (str, optional): name of theme. Defaults to THEME.
-            typeface (str, optional): name of typeface. Defaults to TYPEFACE.
-            font_sizes (list, optional): list of font sizes. Defaults to FONT_SIZES.
-            group (str, optional): name of group. Defaults to None.
-        """
-        self.theme = theme
-        self.typeface = typeface
-        self.font_sizes = font_sizes
+            group (Optional[str], optional): name of group. Defaults to None.
+            font_sizes (tuple[int], optional): list of font sizes. Defaults to (14,12,10,8,6).
+            theme (str, optional): name of theme. Defaults to 'LightGreen'.
+            typeface (str, optional): name of typeface. Defaults to "Helvetica".
+        """
         self.name = name
         self.group = group
-        
+        self.flags = self._default_flags.copy()
+        self.tool = None
         self.window = None
-        self.configure()
         
-        self.flags = {}
+        Panel.font_sizes = font_sizes
+        Panel.theme = theme
+        Panel.typeface = typeface
+        
+        self.configure()
         return
     
-    @staticmethod
-    def getButtons(labels:list, size, key_prefix, font:tuple, texts=[], **kwargs):
-        """
-        Get list of panel buttons
-
-        Args:
-            labels (list): list of button labels
-            size (int, or tuple): button width (,height)
-            key_prefix (any): prefix of button key
-            font (tuple): (typeface, font size)
-            texts (list, optional): alternative text labels for buttons. Defaults to [].
-
-        Returns:
-            list: list of PySimpleGUI.Button objects
-        """
-        buttons = []
-        specials = kwargs.pop('specials', {})
-        for i,label in enumerate(labels):
-            key_string = label.replace('\n','')
-            key = f"-{key_prefix}-{key_string}-" if key_prefix else f"-{key_string}-"
-            kw = kwargs.copy()
-            if label in specials.keys():
-                for k,v in specials[label].items():
-                    kw[k] = v
-            if len(texts):
-                try:
-                    label = texts[i]
-                except IndexError:
-                    pass
-            buttons.append(sg.Button(label, size=size, key=key, font=font, **kw))
-        return buttons
+    def __del__(self):
+        self.close()
     
-    @staticmethod
-    def parseInput(string:str):
+    @abstractmethod
+    def getLayout(self, title:str = 'Panel', title_font_level:int = 0, **kwargs) -> sg.Column:
         """
-        Parse inputs from GUI
+        Build `sg.Column` object
 
         Args:
-            string (str): input string read from GUI window
+            title (str, optional): title of layout. Defaults to 'Panel'.
+            title_font_level (int, optional): index of font size from levels in `font_sizes`. Defaults to 0.
 
         Returns:
-            any: appropriate values
+            sg.Column: Column object
         """
-        if ',' in string:
-            strings = string.split(',')
-        elif ';' in string:
-            strings = string.split(';')
-        else:
-            try:
-                string = float(string)
-                return string
-            finally:
-                # return string
-                pass
-        output = []
-        for string in strings:
-            try:
-                output.append(float(string))
-            except ValueError:
-                # output.append(string)
-                pass
-        return output
-    
-    def _mangle(self, string:str):
+        font = (self.typeface, self.font_sizes[title_font_level]) if 'font' not in kwargs.keys() else kwargs.pop('font')
+        layout = [[
+            sg.Text(title, 
+                    font=font,
+                    **kwargs)
+        ]]
+        # Build Layout here
+        layout = sg.Column(layout, vertical_alignment='top')
+        return layout
+
+    @abstractmethod
+    def listenEvents(self, event:str, values:dict[str, str]) -> dict[str, str]:
         """
-        Mangle string with name of panel
+        Listen to events and act on values
 
         Args:
-            string (str): string to be mangled
+            event (str): event triggered
+            values (dict[str, str]): dictionary of values from window
 
         Returns:
-            str: mangled string
-        """
-        return f'-{self.name}{string}'
-    
-    @staticmethod
-    def pad():
+            dict: dictionary of updates
         """
-        Spacer / padding
+        updates = {}
+        # Listen to events here
+        return updates
 
-        Returns:
-            PySimpleGUI.Push: padding
-        """
-        ele = sg.Text('', size=(1,1))
-        try:
-            ele = sg.Push()
-        except Exception as e:
-            print(e)
-        return ele
-    
     @classmethod
-    def arrangeElements(cls, elements:list, shape=(0,0), form=''):
+    def arrangeElements(cls, elements:list, shape:tuple[int, int] = (0,0), form:str = '') -> list[list]:
         """
-        Arrange elements in a horizontal / vertical / cross-shape pattern
+        Arrange elements in a horizontal, vertical, or cross-shape pattern
 
         Args:
             elements (list): list of GUI elements
-            shape (tuple, optional): shape of grid. Defaults to (0,0).
+            shape (tuple[int, int], optional): shape of grid. Defaults to (0,0).
             form (str, optional): shape of pattern. Defaults to ''.
 
         Raises:
-            Exception: Grid size must be large enough to accommodate all elements
+            RuntimeError: Make sure grid size is able to fit the number of elements
 
         Returns:
-            list: list of arranged GUI elements
+            list[list]: list of lists of arranged GUI elements
         """
         arranged_elements = []
         if form in ['X', 'x', 'cross', '+']:
             h = elements[0]
             v = elements[1]
             if len(h) == 0:
                 return cls.arrangeElements(v, form='V')
@@ -182,96 +188,182 @@
                     root = 1
                     while True:
                         if root**2 > num:
                             break
                         root += 1
                     row = root
             elif rows*cols < num:
-                raise Exception('Make sure grid size is able to fit the number of elements.')
+                raise RuntimeError('Make sure grid size is able to fit the number of elements.')
             else:
                 row = rows
             while n < num:
                 l,u = n, min(n+row, num)
                 arranged_elements.append([cls.pad()]+ [elements[l:u]] +[cls.pad()])
                 n += row
         return arranged_elements
-    
+
     def close(self):
-        """
-        Close window
-        """
+        """Exit the application"""
+        try:
+            self.window.close()
+        except AttributeError:
+            pass
         return
-    
-    def configure(self, **kwargs):
-        """
-        Configure defaults
-        """
-        theme = self.theme if 'theme' not in kwargs.keys() else kwargs.pop('theme')
-        font = (self.typeface, self.font_sizes[int(len(FONT_SIZES)/2)]) if 'font' not in kwargs.keys() else kwargs.pop('font')
-        element_padding = (0,0) if 'element_padding' not in kwargs.keys() else kwargs.pop('element_padding')
+
+    @classmethod
+    def configure(cls, **kwargs):
+        """Configure GUI defaults"""
+        cls.font_sizes = kwargs.pop('font_sizes', cls.font_sizes)
+        cls.theme = kwargs.pop('theme', cls.theme)
+        cls.typeface = kwargs.pop('typeface', cls.typeface)
         
-        sg.theme(theme)
+        element_padding = kwargs.pop('element_padding', (0,0))
+        font = kwargs.pop('font', (cls.typeface, cls.font_sizes[int(len(cls.font_sizes)/2)]))
+        
+        sg.theme(cls.theme)
         sg.set_options(font=font, element_padding=element_padding, **kwargs)
         return
     
-    def getLayout(self, title='Panel', title_font_level=0, **kwargs):
+    @staticmethod
+    def getButtons(
+        labels: list[str], 
+        size: Union[int, tuple], 
+        key_prefix: str, 
+        font: tuple[str, int], 
+        texts: Optional[list[str]] = None, 
+        **kwargs
+    ) -> list[sg.Button]:
         """
-        Get layout object
+        Get list of panel buttons
 
         Args:
-            title (str, optional): title of layout. Defaults to 'Panel'.
-            title_font_level (int, optional): index of font size from levels in font_sizes. Defaults to 0.
+            labels (list[str]): list of button labels
+            size (Union[int, tuple]): button width (,height)
+            key_prefix (str): prefix of button key
+            font (tuple[str, int]): (typeface, font size)
+            texts (Optional[list[str]], optional): alternative text labels for buttons. Defaults to None.
 
         Returns:
-            PySimpleGUI.Column: Column object
+            list: list of PySimpleGUI.Button objects
         """
-        font = (self.typeface, self.font_sizes[title_font_level]) if 'font' not in kwargs.keys() else kwargs.pop('font')
-        layout = [[
-            sg.Text(title, 
-                    font=font,
-                    **kwargs)
-        ]]
-        # Build Layout here
-        layout = sg.Column(layout, vertical_alignment='top')
-        return layout
-    
-    def getWindow(self, title='Application', **kwargs):
+        texts = [] if texts is None else texts
+        buttons = []
+        specials = kwargs.pop('specials', {})
+        for i,label in enumerate(labels):
+            key_string = label.replace('\n','')
+            key = f"-{key_prefix}-{key_string}-" if key_prefix else f"-{key_string}-"
+            kw = kwargs.copy()
+            if label in specials.keys():
+                for k,v in specials[label].items():
+                    kw[k] = v
+            if len(texts):
+                try:
+                    label = texts[i]
+                except IndexError:
+                    pass
+            buttons.append(sg.Button(label, size=size, key=key, font=font, **kw))
+        return buttons
+
+    def getWindow(self, title:str = 'Application', **kwargs) -> sg.Window:
         """
-        Get window object
+        Build `sg.Window` object
 
         Args:
             title (str, optional): title of window. Defaults to 'Application'.
 
         Returns:
-            PySimpleGUI.Window: Window object
+            sg.Window: Window object
         """
         layout = [[self.getLayout()]]
         window = sg.Window(title, layout, enable_close_attempted_event=True, resizable=False, finalize=True, icon='icon.ico', **kwargs)
         self.window = window
         return window
+
+    @staticmethod
+    def pad() -> Union[sg.Push, sg.Text]:
+        """
+        Add spacer in GUI
+
+        Returns:
+            Union[sg.Push, sg.Text]: GUI spacer
+        """
+        ele = sg.Text('', size=(1,1))
+        try:
+            ele = sg.Push()
+        except Exception as e:
+            print(e)
+        return ele
     
-    def listenEvents(self, event, values):
+    @staticmethod
+    def parseInput(text:str) -> list[Union[float, str]]:
         """
-        Listen to events and act on values
+        Parse inputs from GUI
 
         Args:
-            event (str): event triggered
-            values (dict): dictionary of values from window
+            text (str): input text read from GUI window
 
         Returns:
-            dict: dictionary of updates
+            list[Union[float, str]]: variable output including floats, strings, and tuples
         """
-        updates = {}
-        # Listen to events here
-        return updates
+        if ',' in text:
+            strings = text.split(',')
+        elif ';' in text:
+            strings = text.split(';')
+        else:
+            try:
+                text = float(text)
+                return text
+            finally:
+                # return text
+                pass
+        output = []
+        for text in strings:
+            try:
+                output.append(float(text))
+            except ValueError:
+                # output.append(text)
+                pass
+        return output
+    
+    def runGUI(self, title:str = 'Application', maximize:bool = False):
+        """
+        Run the GUI loop
+
+        Args:
+            title (str, optional): title of window. Defaults to 'Application'.
+            maximize (bool, optional): whether to maximise window. Defaults to False.
+        """
+        self.configure()
+        self.getWindow(title)
+        self.window.Finalize()
+        if maximize:
+            self.window.Maximize()
+        self.window.bring_to_front()
+        try:
+            self._loop_gui()
+        finally:
+            self.close()
+        return
     
-    def loopGUI(self):
+    def setFlag(self, **kwargs):
         """
-        Loop GUI process
+        Set flags by using keyword arguments
+
+        Kwargs:
+            key, value: (flag name, boolean) pairs
         """
+        if not all([type(v)==bool for v in kwargs.values()]):
+            raise ValueError("Ensure all assigned flag values are boolean.")
+        for key, value in kwargs.items():
+            self.flags[key] = value
+        return
+
+    # Protected method(s)
+    def _loop_gui(self):
+        """Loop GUI process"""
         if type(self.window) == type(None):
             return
         while True:
             event, values = self.window.read(timeout=30)
             if event in ('Ok', WIN_CLOSED, WINDOW_CLOSE_ATTEMPTED_EVENT, None):
                 self.window.close()
                 break
@@ -279,67 +371,77 @@
             for ele_key, kwargs in updates.items():
                 tooltip = kwargs.pop('tooltip', None)
                 if tooltip is not None:
                     self.window[ele_key].set_tooltip(str(tooltip))
                 self.window[ele_key].update(**kwargs)
         return
     
-    def runGUI(self, title='Application', maximize=False):
+    def _mangle(self, text:str) -> str:
         """
-        Run the GUI loop
+        Mangle text with name of panel
 
         Args:
-            title (str, optional): title of window. Defaults to 'Application'.
-            maximize (bool, optional): whether to maximise window. Defaults to False.
-        """
-        self.getWindow(title)
-        self.window.Finalize()
-        if maximize:
-            self.window.Maximize()
-        self.window.bring_to_front()
-        self.loopGUI()
-        self.window.close()
-        self.close()
-        return
+            text (str): text to be mangled
 
+        Returns:
+            str: mangled text
+        """
+        return f'-{self.name}{text}'
+    
 
 class CompoundPanel(Panel):
     """
-    Compound Panel class
+    CompoundPanel provides methods to form a multi-tool control panel
 
+    ### Constructor
     Args:
-        ensemble (dict, optional): dictionary of individual sub-panels. Defaults to {}.
-        theme (str, optional): name of theme. Defaults to THEME.
-        typeface (str, optional): name of typeface. Defaults to TYPEFACE.
-        font_sizes (list, optional): list of font sizes. Defaults to FONT_SIZES.
-        group (str, optional): name of group. Defaults to None.
+        `ensemble` (dict[str, Panel]): dictionary of individual sub-panels
+        `group` (Optional[str], optional): name of group. Defaults to None.
+        
+    ### Attributes
+    - `panels` (dict[str, Panel]): dictionary of individual sub-panels
+    
+    ### Methods
+    - `close`: exit the application
+    - `getLayout`: build `sg.Column` object
+    - `listenEvents`: listen to events and act on values
     """
-    def __init__(self, ensemble={}, theme=THEME, typeface=TYPEFACE, font_sizes=FONT_SIZES, group=None):
-        super().__init__(theme=theme, typeface=typeface, font_sizes=font_sizes, group=group)
-        self.panels = {key: value[0](name=key, **value[1]) for key,value in ensemble.items()}
-        return
     
-    def close(self):
+    def __init__(self, 
+        ensemble: dict[str, Panel],
+        group: Optional[str] = None,
+        **kwargs
+    ):
         """
-        Close window
+        Instantiate the class
+
+        Args:
+            ensemble (dict[str, Panel]): dictionary of individual sub-panels
+            group (Optional[str], optional): name of group. Defaults to None.
         """
+        super().__init__(group=group, **kwargs)
+        self.panels = {key: value for key,value in ensemble.items()}
+        return
+    
+    def close(self):
+        """Exit the application"""
         for panel in self.panels.values():
             panel.close()
-        return
+        return super().close()
     
-    def getLayout(self, title='Control Panel', title_font_level=0, **kwargs):
+    def getLayout(self, title:str = 'Control Panel', title_font_level:int = 0, **kwargs) -> sg.Column:
         """
-        Get layout object
+        Build `sg.Column` object
 
         Args:
-            title (str, optional): title of layout. Defaults to 'Panel'.
-            title_font_level (int, optional): index of font size from levels in font_sizes. Defaults to 0.
+            title (str, optional): title of layout. Defaults to 'Control Panel'.
+            title_font_level (int, optional): index of font size from levels in `font_sizes`. Defaults to 0.
 
         Returns:
-            PySimpleGUI.Column: Column object
+            sg.Column: Column object
         """
         font = (self.typeface, self.font_sizes[title_font_level], 'bold')
         layout = super().getLayout(title, justification='center', font=font)
         
         tab_groups = {'main': []}
         for key, panel in self.panels.items():
             group = panel.group
@@ -384,21 +486,21 @@
         layout = [
             [layout],
             [suite]
         ]
         layout = sg.Column(layout, vertical_alignment='top')
         return layout
     
-    def listenEvents(self, event, values):
+    def listenEvents(self, event:str, values:dict[str, str]) -> dict[str, dict]:
         """
         Listen to events and act on values
 
         Args:
             event (str): event triggered
-            values (dict): dictionary of values from window
+            values (dict[str, str]): dictionary of values from window
 
         Returns:
             dict: dictionary of updates
         """
         updates = {}
         for panel in self.panels.values():
             update = panel.listenEvents(event, values)
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Control/Schedule/schedule_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Control/Schedule/schedule_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/12/13 10:30:00
-@author: Chang Jie
 
-Notes / actionables:
-- 
 """
 # Standard library imports
 
 # Third party imports
 
 # Local application imports
 print(f"Import: OK <{__name__}>")
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Make/Heat/peltier_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,364 +1,305 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2023/01/16 11:11:00
-@author: Chang Jie
+This module holds the class for Peltier devices.
 
-Notes / actionables:
--
+Classes:
+    Peltier (Maker)
+
+Other constants and variables:
+    COLUMNS (tuple)
 """
 # Standard library imports
 from datetime import datetime
 import pandas as pd
 from threading import Thread
 import time
 
 # Third party imports
-import serial # pip install pyserial
+import serial   # pip install pyserial
 
 # Local application imports
+from ..make_utils import Maker
 print(f"Import: OK <{__name__}>")
 
-COLUMNS = ['Time', 'Set', 'Hot', 'Cold', 'Power']
-POWER_THRESHOLD = 20
-STABILIZE_TIME_S = 10
-TEMPERATURE_TOLERANCE = 1.5
+COLUMNS = ('Time', 'Set', 'Hot', 'Cold', 'Power')
+"""Headers for output data from Peltier device"""
 
-class Peltier(object):
+class Peltier(Maker):
     """
-    A Peltier device generates heat to provide local temperature control of the sample.
+    A Peltier device generates heat to provide local temperature control of the sample
 
     ### Constructor
     Args:
-        `port` (str): com port address
-        `tolerance` (float, optional): temperature tolerance to determine if device has reached target temperature. Defaults to `TEMPERATURE_TOLERANCE` (i.e. 1.5).
-        
-    ### Attributes:
-    - `buffer_df` (pandas.DataFrame): data output from device
-    - `device` (serial.Serial): serial connection to device
-    - `port` (str): com port address
-    - `precision` (int): number of decimal places to display current temperature
-    - `temperature` (float): current temperature of device
-    - `tolerance` (float): temperature tolerance
-    - `verbose` (bool): verbosity of class
+        `port` (str): COM port of device
+        `power_threshold` (float, optional): minimum threshold under which temperature can be considered stable. Defaults to 20.
+        `stabilize_buffer_time` (float, optional): buffer time over which temperature can be considered stable. Defaults to 10.
+        `tolerance` (float, optional): tolerance above and below target temperature. Defaults to 1.5.
+            
+    ### Attributes
+    - `power_threshold` (float): minimum threshold under which temperature can be considered stable
+    - `set_point` (float): temperature set point
+    - `stabilize_buffer_time` (float): buffer time over which temperature can be considered stable
+    - `temperature` (float): temperature at sample site
+    - `tolerance` (float): tolerance above and below target temperature
     
-    ### Methods:
+    ### Properties
+    - `port`: COM port of device
+    
+    ### Methods
     - `clearCache`: clears and remove data in buffer
-    - `connect`: connects to the device using the existing port, baudrate and timeout values
-    - `getTemperatures`: reads from the device the set temperature, hot temperature, cold temperature, and the power level
-    - `holdTemperature`: holds the device temperature at target temperature for specified duration
-    - `isBusy`: checks whether the device is busy
-    - `isConnected`: checks whether the device is connected
-    - `isReady`: checks whether the device has reached the set temperature
-    - `reset`: clears data in buffer and set the temperature to room temperature (i.e. 25°C)
-    - `setFlag`: set value of flag
-    - `setTemperature`: change the set temperature
-    - `toggleFeedbackLoop`: toggle the feedback loop thread on or off
-    - `toggleRecord`: toggle the data recording on or off
+    - `getTemperatures`: retrieve temperatures from device
+    - `holdTemperature`: hold target temperature for desired duration
+    - `isReady`: checks and returns whether target temperature has been reached
+    - `reset`: reset the device
+    - `setTemperature`: set a target temperature
+    - `shutdown`: shutdown procedure for tool
+    - `toggleFeedbackLoop`: start or stop feedback loop
+    - `toggleRecord`: start or stop data recording
     """
     
-    def __init__(self, port:str, tolerance:float = TEMPERATURE_TOLERANCE):
+    _default_flags = {
+        'busy': False,
+        'connected': False,
+        'get_feedback': False,
+        'pause_feedback': False,
+        'record': False,
+        'temperature_reached': False
+    }
+    
+    def __init__(self, 
+        port: str, 
+        power_threshold: float = 20,
+        stabilize_buffer_time: float = 10, 
+        tolerance: float = 1.5, 
+        **kwargs
+    ):
         """
-        Construct the Peltier object
+        Instantiate the class
 
         Args:
-            `port` (str): com port address
-            `tolerance` (float, optional): temperature tolerance to determine if device has reached target temperature. Defaults to `TEMPERATURE_TOLERANCE` (i.e. 1.5).
-        """
-        self.device = None
-        self._flags = {
-            'busy': False,
-            'connected': False,
-            'get_feedback': False,
-            'pause_feedback': False,
-            'record': False,
-            'temperature_reached': False
-        }
-        self._set_point = None
-        self._temperature = None
-        self._cold_point = None
-        self._power = None
+            port (str): COM port of device
+            power_threshold (float, optional): minimum threshold under which temperature can be considered stable. Defaults to 20.
+            stabilize_buffer_time (float, optional): buffer time over which temperature can be considered stable. Defaults to 10.
+            tolerance (float, optional): tolerance above and below target temperature. Defaults to 1.5.
+        """
+        super().__init__(**kwargs)
+        self.buffer_df = pd.DataFrame(columns=list(COLUMNS))
+        self.power_threshold = power_threshold
+        self.stabilize_buffer_time = stabilize_buffer_time
+        self.tolerance = tolerance
         
-        self._precision = 3
+        self._columns = list(COLUMNS)
         self._stabilize_time = None
-        self._tolerance = tolerance
         self._threads = {}
         
-        self.buffer_df = pd.DataFrame(columns=COLUMNS)
-        
-        self.verbose = True
-        self.port = ''
-        self._baudrate = None
-        self._timeout = None
+        # Device read-outs
+        self.set_point = None
+        self.temperature = None
+        self._cold_point = None
+        self._power = None
         self._connect(port)
         return
     
+    # Properties
     @property
-    def precision(self):
-        return self._precision
-    @precision.setter
-    def precision(self, value:int):
-        self._precision = abs(value)
-        return
-    
-    @property
-    def temperature(self):
-        return round(self._temperature, self._precision)
-    
-    @property
-    def tolerance(self):
-        return f"+- {self._tolerance} °C"
-    @tolerance.setter
-    def tolerance(self, value:float):
-        self._tolerance = abs(value)
-        return
-    
-    def __delete__(self):
-        self._shutdown()
-        return
-    
-    def _connect(self, port:str, baudrate:int = 115200, timeout:int = 1):
-        """
-        Connect to machine control unit
-
-        Args:
-            `port` (str): com port address
-            `baudrate` (int, optional): baudrate. Defaults to 115200.
-            `timeout` (int, optional): timeout in seconds. Defaults to 1.
-            
-        Returns:
-            `serial.Serial`: serial connection to machine control unit if connection is successful, else `None`
-        """
-        self.port = port
-        self._baudrate = baudrate
-        self._timeout = timeout
-        device = None
-        try:
-            device = serial.Serial(port, self._baudrate, timeout=self._timeout)
-            self.device = device
-            print(f"Connection opened to {port}")
-            self.setFlag('connected', True)
-            time.sleep(1)
-            print(self.getTemperatures())
-            # self.toggleFeedbackLoop(on=True)
-        except Exception as e:
-            print(f"Could not connect to {port}")
-            if self.verbose:
-                print(e)
-        return self.device
-    
-    def _loop_feedback(self):
-        """
-        Feedback loop to constantly read values from device
-        """
-        print('Listening...')
-        while self._flags['get_feedback']:
-            if self._flags['pause_feedback']:
-                continue
-            self.getTemperatures()
-            time.sleep(0.1)
-        print('Stop listening...')
-        return
-
-    def _read(self):
-        """
-        Read values from the device
-
-        Returns:
-            `str`: response string
-        """
-        response = ''
-        try:
-            response = self.device.readline()
-            response = response.decode('utf-8').strip()
-        except Exception as e:
-            if self.verbose:
-                print(e)
-        # print(response)
-        return response
-    
-    def _shutdown(self):
-        """
-        Close serial connection and shutdown feedback loop
-        """
-        self.toggleFeedbackLoop(on=False)
-        self.device.close()
-        self._flags = {
-            'busy': False,
-            'connected': False,
-            'get_feedback': False,
-            'pause_feedback':False
-        }
-        return
+    def port(self) -> str:
+        return self.connection_details.get('port', '')
     
     def clearCache(self):
-        """
-        Clear data from buffer
-        """
-        self.setFlag('pause_feedback', True)
+        """Clears and remove data in buffer"""
+        self.setFlag(pause_feedback=True)
         time.sleep(0.1)
-        self.buffer_df = pd.DataFrame(columns=COLUMNS)
-        self.setFlag('pause_feedback', False)
+        self.buffer_df = pd.DataFrame(columns=self._columns)
+        self.setFlag(pause_feedback=False)
         return
     
-    def connect(self):
-        """
-        Reconnect to device using existing port and baudrate
-        
-        Returns:
-            `serial.Serial`: serial connection to machine control unit if connection is successful, else `None`
-        """
-        return self._connect(self.port, self._baudrate, self._timeout)
-    
-    def getTemperatures(self):
+    def getTemperatures(self) -> str:
         """
-        Reads from the device the set temperature, hot temperature, cold temperature, and the power level
+        Retrieve temperatures from device 
+        Including the set temperature, hot temperature, cold temperature, and the power level
         
         Returns:
-            `str`: response from device output
+            str: response from device
         """
         response = self._read()
         now = datetime.now()
         try:
             values = [float(v) for v in response.split(';')]
-            self._set_point, self._temperature, self._cold_point, self._power = values
-            ready = (abs(self._set_point - self._temperature)<=TEMPERATURE_TOLERANCE)
+            self.set_point, self.temperature, self._cold_point, self._power = values
+        except ValueError:
+            pass
+        else:
+            ready = (abs(self.set_point - self.temperature)<=self.tolerance)
             if not ready:
                 pass
             elif not self._stabilize_time:
                 self._stabilize_time = time.time()
                 print(response)
-            elif self._flags['temperature_reached']:
+            elif self.flags['temperature_reached']:
                 pass
-            elif (self._power <= POWER_THRESHOLD) or (time.time()-self._stabilize_time >= STABILIZE_TIME_S):
+            elif (self._power <= self.power_threshold) or (time.time()-self._stabilize_time >= self.stabilize_buffer_time):
                 print(response)
-                self.setFlag('temperature_reached', True)
-                print(f"Temperature of {self._set_point}°C reached!")
-            
-            if self._flags.get('record', False):
+                self.setFlag(temperature_reached=True)
+                print(f"Temperature of {self.set_point}°C reached!")
+            if self.flags['record']:
                 values = [now] + values
-                row = {k:v for k,v in zip(COLUMNS, values)}
+                row = {k:v for k,v in zip(self._columns, values)}
                 self.buffer_df = self.buffer_df.append(row, ignore_index=True)
-        except ValueError:
-            pass
         return response
     
     def holdTemperature(self, temperature:float, time_s:float):
         """
-        Hold the device temperature at target temperature for specified duration
+        Hold target temperature for desired duration
 
         Args:
-            `temperature` (float): temperature in degree Celsius
-            `time_s` (float): duration in seconds
+            temperature (float): temperature in degree Celsius
+            time_s (float): duration in seconds
         """
         self.setTemperature(temperature)
-        print(f"Holding at {self._set_point}°C for {time_s} seconds")
+        print(f"Holding at {self.set_point}°C for {time_s} seconds")
         time.sleep(time_s)
         print(f"End of temperature hold")
         return
     
-    def isBusy(self):
-        """
-        Check whether the device is busy
-        
-        Returns:
-            `bool`: whether the device is busy
-        """
-        return self._flags['busy']
-    
-    def isConnected(self):
+    def isReady(self) -> bool:
         """
-        Check whether the device is connected
+        Checks and returns whether target temperature has been reached
 
         Returns:
-            `bool`: whether the device is connected
+            bool: whether target temperature has been reached
         """
-        return self._flags['connected']
-    
-    def isReady(self):
-        """
-        Check whether target temperature has been reached
-
-        Returns:
-            `bool`: whether target temperature has been reached
-        """
-        return self._flags['temperature_reached']
+        return self.flags['temperature_reached']
     
     def reset(self):
-        """
-        Clears data in buffer and set the temperature to room temperature (i.e. 25°C)
-        """
+        """Reset the device"""
         self.toggleRecord(False)
         self.clearCache()
         self.setTemperature(set_point=25, blocking=False)
         return
-
-    def setFlag(self, name:str, value:bool):
-        """
-        Set a flag's truth value
-
-        Args:
-            `name` (str): label
-            `value` (bool): flag value
-        """
-        self._flags[name] = value
-        return
     
     def setTemperature(self, set_point:int, blocking:bool = True):
         """
-        Set temperature of the device
+        Set a temperature
 
         Args:
-            `set_point` (int): target temperature in degree Celsius
+            set_point (int): target temperature in degree Celsius
+            blocking (bool, optional): whether to wait for temperature to reach set point. Defaults to True.
         """
-        self.setFlag('pause_feedback', True)
+        self.setFlag(pause_feedback=True)
         time.sleep(0.5)
         try:
             self.device.write(bytes(f"{set_point}\n", 'utf-8'))
-            while self._set_point != float(set_point):
-                self.getTemperatures()
         except AttributeError:
             pass
+        else:
+            while self.set_point != float(set_point):
+                self.getTemperatures()
         print(f"New set temperature at {set_point}°C")
         
         self._stabilize_time = None
-        self.setFlag('temperature_reached', False)
-        self.setFlag('pause_feedback', False)
-        print(f"Waiting for temperature to reach {self._set_point}°C")
+        self.setFlag(temperature_reached=False, pause_feedback=False)
+        if blocking:
+            print(f"Waiting for temperature to reach {self.set_point}°C")
         while not self.isReady():
-            if not self._flags['get_feedback']:
+            if not self.flags['get_feedback']:
                 self.getTemperatures()
             time.sleep(0.1)
             if not blocking:
                 break
         return
     
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        for thread in self._threads.values():
+            thread.join()
+        return super().shutdown()
+
     def toggleFeedbackLoop(self, on:bool):
         """
-        Toggle between starting and stopping feedback loop
+        Start or stop feedback loop
 
         Args:
-            `on` (bool): whether to have loop to continuously read from device
+            on (bool): whether to start loop to continuously read from device
         """
-        self.setFlag('get_feedback', on)
+        self.setFlag(get_feedback=on)
         if on:
             if 'feedback_loop' in self._threads:
                 self._threads['feedback_loop'].join()
             thread = Thread(target=self._loop_feedback)
             thread.start()
             self._threads['feedback_loop'] = thread
         else:
             self._threads['feedback_loop'].join()
         return
     
     def toggleRecord(self, on:bool):
         """
-        Toggle between starting and stopping temperature recording
+        Start or stop data recording
 
         Args:
-            `on` (bool): whether to start recording temperature
+            on (bool): whether to start recording temperature
         """
-        self.setFlag('record', on)
-        self.setFlag('get_feedback', on)
-        self.setFlag('pause_feedback', False)
+        self.setFlag(record=on, get_feedback=on, pause_feedback=False)
         self.toggleFeedbackLoop(on=on)
         return
+
+    # Protected method(s)
+    def _connect(self, port:str, baudrate:int = 115200, timeout:int = 1):
+        """
+        Connection procedure for tool
+
+        Args:
+            port (str): COM port address
+            baudrate (int, optional): baudrate. Defaults to 115200.
+            timeout (int, optional): timeout in seconds. Defaults to 1.
+        """
+        self.connection_details = {
+            'port': port,
+            'baudrate': baudrate,
+            'timeout': timeout
+        }
+        device = None
+        try:
+            device = serial.Serial(port, baudrate, timeout=timeout)
+        except Exception as e:
+            print(f"Could not connect to {port}")
+            if self.verbose:
+                print(e)
+        else:
+            print(f"Connection opened to {port}")
+            self.setFlag(connected=True)
+            time.sleep(1)
+            print(self.getTemperatures())
+        self.device = device
+        return
+    
+    def _loop_feedback(self):
+        """Loop to constantly read from device"""
+        print('Listening...')
+        while self.flags['get_feedback']:
+            if self.flags['pause_feedback']:
+                continue
+            self.getTemperatures()
+            time.sleep(0.1)
+        print('Stop listening...')
+        return
+
+    def _read(self) -> str:
+        """
+        Read response from device
+
+        Returns:
+            str: response string
+        """
+        response = ''
+        try:
+            response = self.device.readline()
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        else:
+            response = response.decode('utf-8').strip()
+            if self.verbose:
+                print(response)
+        return response
+
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Make/Light/led_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,277 +1,286 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
+This module holds the class for LED arrays.
 
-Notes / actionables:
--
+Classes:
+    LEDArray (Maker)
+    LED (dataclass)
 """
 # Standard library imports
+from __future__ import annotations
+from dataclasses import dataclass, field
 from threading import Thread
 import time
+from typing import Optional
 
 # Third party imports
-import serial # pip install pyserial
+import serial   # pip install pyserial
 
 # Local application imports
+from ..make_utils import Maker
 print(f"Import: OK <{__name__}>")
 
-class LED(object):
+@dataclass
+class LED:
     """
-    LED class represents a LED unit
+    LED dataclass represents a single LED unit
 
+    ### Constructor
     Args:
-        channel (int): channel index
-    """
-    def __init__(self, channel:int):
-        self.channel = channel
-        self._duration = 0
-        self._end_time = time.time()
-        self._power = 0
+        `channel` (int): channel id
         
-        self._flags = {
-            'power_update': False
-        }
-        pass
+    ### Attributes
+    - `channel` (int): channel id
+    - `update_power` (bool): whether to update the LED's power
+    
+    ### Properties
+    - `power` (int): power level of LED (0~255)
+    
+    ### Methods
+    - `setPower`: set power and duration for illumination
+    """
     
+    channel: int
+    update_power: bool = field(default=False, init=False)
+    _duration: int = field(default=0, init=False)
+    _end_time: float = field(default=time.time(), init=False)
+    _power: int = field(default=0, init=False)
+    
+    # Properties
     @property
-    def power(self):
+    def power(self) -> int:
         return self._power
     @power.setter
     def power(self, value:int):
-        if type(value) == int and (0 <= value <= 255):
+        if type(value) is int and (0 <= value <= 255):
             self._power = value
-            self.setFlag('power_update', True)
+            self.update_power = True
         else:
             print('Please input an integer between 0 and 255.')
         return
     
-    def setFlag(self, name:str, value:bool):
-        """
-        Set a flag truth value
-
-        Args:
-            name (str): label
-            value (bool): flag value
-        """
-        self._flags[name] = value
-        return
-    
     def setPower(self, value:int, time_s:int = 0):
         """
         Set power and duration for illumination
 
         Args:
             value (int): power level between 0 and 255
-            time_s (int, optional): time duration in seconds. Defaults to 0.
+            time_s (int, optional): duration in seconds. Defaults to 0.
         """
         self.power = value
-        if time_s:
-            self._duration = time_s
+        self._duration = time_s
         return
     
 
-class LEDArray(object):
+class LEDArray(Maker):
     """
-    UVLed class contains methods to control an LED array
+    LEDArray provides methods to control an array of LEDs connected to a controller
 
+    ### Constructor
     Args:
-        port (str): com port address
-        channels (list, optional): list of channels. Defaults to [0].
-        verbose (bool, optional): whether to print outputs. Defaults to False.
+        `port` (str): COM port address
+        `channels` (list, optional): list of channels. Defaults to [0].
+        `verbose` (bool, optional): whether to print outputs. Defaults to False.
+    
+    ### Attributes
+    - `channels` (dict[int, LED]): dictionary of {channel id, `LED` objects}
+    
+    ### Properties
+    - `port` (str): COM port address
+    
+    ### Methods
+    - `getPower`: get power level(s) of channel(s)
+    - `getTimedChannels`: get channels that are still timed
+    - `isBusy`: checks and returns whether the LED array is still busy
+    - `setPower`: set the power value(s) for channel(s)
+    - `shutdown`: shutdown procedure for tool
+    - `startTiming`: start counting down time left with LEDs on
+    - `turnOff`: turn of specified LED channels
     """
-    def __init__(self, port:str, channels:list = [0], verbose:bool = False):
+    
+    _default_flags = {
+        'busy': False,
+        'connected': False,
+        'execute_now': False,
+        'timing_loop': False
+    }
+    
+    def __init__(self, port:str, channels:list[int] = [0], **kwargs):
+        super().__init__(**kwargs)
         self.channels = {chn: LED(chn) for chn in channels}
-        
-        self.device = None
-        self._flags = {
-            'execute_now': False,
-            'timing_loop': False
-        }
         self._threads = {}
         self._timed_channels = []
-        
-        self.verbose = verbose
-        self.port = None
-        self._baudrate = None
-        self._timeout = None
         self._connect(port)
         return
     
-    def _connect(self, port:str, baudrate=9600, timeout=1):
-        """
-        Connect to serial port
-
-        Args:
-            port (str): com port address
-            baudrate (int): baudrate
-            timeout (int, optional): timeout in seconds. Defaults to None.
-            
-        Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
-        """
-        self.port = port
-        self._baudrate = baudrate
-        self._timeout = timeout
-        device = None
-        try:
-            device = serial.Serial(port, baudrate, timeout=timeout)
-            time.sleep(5)   # Wait for grbl to initialize
-            device.flushInput()
-            self.turnOff()
-            print(f"Connection opened to {port}")
-        except Exception as e:
-            if self.verbose:
-                print(f"Could not connect to {port}")
-                print(e)
-        self.device = device
-        return self.device
-    
-    def _loop_count_time(self):
-        """
-        Loop for counting time and flagging channels
-        """
-        self.setFlag('timing_loop', True)
-        busy = self.isBusy()
-        timed_channels = self._timed_channels
-        last_round = False
-        while busy:
-            finished_channels = list(set(timed_channels) - set(self._timed_channels))
-            timed_channels = self._timed_channels
-            if len(finished_channels):
-                for c in finished_channels:
-                    self.turnOff(c)
-            self._update_power()
-            time.sleep(0.01)
-            if last_round:
-                break
-            if not self.isBusy():
-                last_round = True
-        self.setFlag('timing_loop', False)
-        self._timed_channels = []
-        return
-    
-    def _update_power(self):
-        """
-        Update power levels by sending message to device
-
-        Returns:
-            str: message string
-        """
-        if not any([chn._flags['power_update'] for chn in self.channels.values()]):
-            return ''
-        message = f"{';'.join([str(v) for v in self.getPower()])}\n"
-        try:
-            self.device.write(bytes(message, 'utf-8'))
-        except AttributeError:
-            pass
-        now = time.time()
-        for chn in self.channels.values():
-            if chn._flags['power_update']:
-                chn._end_time = now + chn._duration
-                chn._duration = 0
-                chn.setFlag('power_update', False)
-        if self.verbose:
-            print(message)
-        return message
+    # Properties
+    @property
+    def port(self) -> str:
+        return self.connection_details.get('port', '')
     
-    def getPower(self, channel:int = None):
+    def getPower(self, channel:Optional[int] = None) -> list[int]:
         """
-        Get power levels of channels
+        Get power level(s) of channel(s)
 
         Args:
-            channel (int, optional): channel index. Defaults to None.
+            channel (Optional[int], optional): channel index. Defaults to None.
 
         Returns:
-            list: list of power levels
+            list[int]: list of power level(s)
         """
         power = []
         if channel is None:
             power = [chn.power for chn in self.channels.values()]
         else:
             power = [self.channels[channel].power]
         return power
     
-    def getTimedChannels(self):
+    def getTimedChannels(self) -> list[int]:
         """
         Get channels that are still timed
 
         Returns:
-            list: list of channels that are still timed
+            list[int]: list of channels that are still timed
         """
         now = time.time()
-        self._timed_channels = [chn.channel for chn in self.channels.values() if chn._end_time>now]
+        self._timed_channels = [chn.channel for chn in self.channels.values() if (chn._end_time>now and chn._duration)]
         return self._timed_channels
     
-    def isBusy(self):
+    def isBusy(self) -> bool:
         """
-        Check whether LED array is still busy
+        Checks and returns whether the LED array is still busy
 
         Returns:
-            bool: whether LED array is still busy
+            bool: whether the LED array is still busy
         """
         busy = bool(len(self.getTimedChannels()))
         busy = busy | any([chn._duration for chn in self.channels.values()])
         return busy
     
-    def isConnected(self):
-        """
-        Checks whether the LED array is connected
-
-        Returns:
-            bool: whether the spinner is connected
-        """
-        if self.device is None:
-            print(f"{self.__class__} ({self.port}) not connected.")
-            return False
-        return True
-    
-    def setFlag(self, name:str, value:bool):
-        """
-        Set a flag truth value
-
-        Args:
-            name (str): label
-            value (bool): flag value
-        """
-        self._flags[name] = value
-        return
-    
-    def setPower(self, value:int, time_s:int = 0, channel:int =None):
+    def setPower(self, value:int, time_s:int = 0, channel:Optional[int] = None):
         """
         Set the power value(s) for channel(s)
 
         Args:
-            value (int): 8-bit integer for LED power
-            time_s (int, optional): time duration in seconds. Defaults to 0.
-            channel (int/iterable, optional): channel(s) for which to set power. Defaults to None.
+            value (int): 8-bit integer for LED power (i.e. 0~255)
+            time_s (int, optional): duration in seconds. Defaults to 0.
+            channel (Optional[int], optional): channel id. Defaults to None.
         """
         if channel is None:
             for chn in self.channels.values():
                 chn.setPower(value, time_s)
-        elif type(channel) == int and channel in self.channels:
+        elif type(channel) is int and channel in self.channels:
             self.channels[channel].setPower(value, time_s)
-        self.startTiming()
+        if time_s:
+            self.startTiming()
+        else:
+            self._update_power()
         return
     
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        for thread in self._threads.values():
+            thread.join()
+        return super().shutdown()
+    
     def startTiming(self):
-        """
-        Start timing the illumination steps
-        """
-        if not self._flags['timing_loop']:
-            thread = Thread(target=self._loop_count_time)
+        """Start counting down time left with LEDs on"""
+        print("Timing...")
+        if not self.flags['timing_loop']:
+            if 'timing_loop'in self._threads and self._threads['timing_loop'].is_alive():
+                return
+            thread = Thread(target=self._loop_timer)
             thread.start()
             self._threads['timing_loop'] = thread
-            print("Timing...")
         return
     
-    def turnOff(self, channel:int = None):
+    def turnOff(self, channel:Optional[int] = None):
         """
         Turn off the LED corresponding to the channel(s)
 
         Args:
-            channel (int, optional): channel index to turn off. Defaults to None.
+            channel (Optional[int], optional): channel id. Defaults to None.
         """
         print(f"Turning off LED {channel}")
         self.setPower(0, channel=channel)
         return
+
+    # Protected method(s)
+    def _connect(self, port:str, baudrate:int = 9600, timeout:int = 1):
+        """
+        Connection procedure for tool
+
+        Args:
+            port (str): COM port address
+            baudrate (int, optional): baudrate. Defaults to 9600.
+            timeout (int, optional): timeout in seconds. Defaults to 1.
+        """
+        self.connection_details = {
+            'port': port,
+            'baudrate': baudrate,
+            'timeout': timeout
+        }
+        device = None
+        try:
+            device = serial.Serial(port, baudrate, timeout=timeout)
+        except Exception as e:
+            print(f"Could not connect to {port}")
+            if self.verbose:
+                print(e)
+        else:
+            time.sleep(5)   # Wait for grbl to initialize
+            device.flushInput()
+            self.turnOff()
+            print(f"Connection opened to {port}")
+            self.setFlag(connected=True)
+        self.device = device
+        return
+        
+    def _loop_timer(self):
+        """Loop for counting time and flagging channels"""
+        self.setFlag(timing_loop=True)
+        busy = self.isBusy()
+        timed_channels = self._timed_channels
+        last_round = False
+        while busy:
+            finished_channels = list(set(timed_channels) - set(self._timed_channels))
+            timed_channels = self._timed_channels
+            if len(finished_channels):
+                for c in finished_channels:
+                    if self.channels[c]._duration == 0:
+                        continue
+                    self.turnOff(c)
+            self._update_power()
+            time.sleep(0.01)
+            if last_round:
+                break
+            if not self.isBusy():
+                last_round = True
+        self.setFlag(timing_loop=False)
+        self._threads.pop('timing_loop')
+        self._timed_channels = []
+        return
+    
+    def _update_power(self) -> str:
+        """
+        Update LED power levels by sending command to device
+
+        Returns:
+            str: command string
+        """
+        if not any([chn.update_power for chn in self.channels.values()]):
+            return ''
+        command = f"{';'.join([str(v) for v in self.getPower()])}\n"
+        try:
+            self.device.write(command.encode('utf-8'))
+        except AttributeError:
+            pass
+        now = time.time()
+        for chn in self.channels.values():
+            if chn.update_power:
+                chn._end_time = now + chn._duration
+                chn.update_power = False
+        if self.verbose:
+            print(command)
+        return command
+
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Measure/Physical/balance_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,257 +1,258 @@
 # %% -*- coding: utf-8 -*-
 """
-Adapted from @jaycecheng spinutils
+This module holds the class for mass balances.
 
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
+Classes:
+    MassBalance (Measurer)
 
-Notes / actionables:
--
+Other constants and variables:
+    CALIBRATION_FACTOR (float)
+    COLUMNS (tuple)
 """
 # Standard library imports
+from datetime import datetime
+import pandas as pd
 from threading import Thread
 import time
 
 # Third party imports
 import serial # pip install pyserial
 
 # Local application imports
-from ...misc import Helper
+from ..measure_utils import Measurer
 print(f"Import: OK <{__name__}>")
 
-class Spinner(object):
+CALIBRATION_FACTOR = 6.862879436681862
+"""Empirical factor by which to divide output reading by to get mass in mg"""
+COLUMNS = ('Time', 'Value', 'Factor', 'Baseline', 'Mass')
+"""Headers for output data from mass balance"""
+
+class MassBalance(Measurer):
     """
-    Spinner class contains methods to control the spin coater unit
+    MassBalance provides methods to read out values from a precision mass balance
 
+    ### Constructor
     Args:
-        port (str): com port address
-        order (int, optional): channel order. Defaults to 0.
-        position (tuple, optional): x,y,z position of spinner. Defaults to (0,0,0).
-        verbose (bool, optional): whether to print outputs. Defaults to False.
-    """
-    def __init__(self, port:str, order=0, position=(0,0,0), verbose=False, **kwargs):
-        self.order = order
-        self.position = tuple(position)
-        self.speed = 0
-        
-        self.device = None
-        self._flags = {
-            'busy': False
-        }
+        `port` (str): COM port address
+        `calibration_factor` (float, optional): calibration factor of device readout to mg. Defaults to CALIBRATION_FACTOR.
         
-        self.verbose = verbose
-        self.port = None
-        self._baudrate = None
-        self._timeout = None
-        self._connect(port)
-        return
+    ### Attributes
+    - `baseline` (float): baseline readout at which zero mass is set
+    - `calibration_factor` (float): calibration factor of device readout to mg
+    - `precision` (int): number of decimal places to print mass value
+    
+    ### Properties
+    - `mass` (float): mass of sample
+    
+    ### Methods
+    - `clearCache`: clear most recent data and configurations
+    - `disconnect`: disconnect from device
+    - `getMass`: get the mass of the sample by measuring the force response
+    - `reset`: reset the device
+    - `shutdown`: shutdown procedure for tool
+    - `tare`: alias for `zero()`
+    - `toggleFeedbackLoop`: start or stop feedback loop
+    - `toggleRecord`: start or stop data recording
+    - `zero`: set the current reading as baseline (i.e. zero mass)
+    """
     
-    def _connect(self, port:str, baudrate=9600, timeout=1):
+    _default_flags = {
+        'busy': False,
+        'connected': False,
+        'get_feedback': False,
+        'pause_feedback': False,
+        'read': True,
+        'record': False
+    }
+    def __init__(self, port:str, calibration_factor:float = CALIBRATION_FACTOR, **kwargs):
         """
-        Connect to serial port
+        Instantiate the class
 
         Args:
-            port (str): com port address
-            baudrate (int): baudrate
-            timeout (int, optional): timeout in seconds. Defaults to None.
-            
-        Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
+            port (str): COM port address
+            calibration_factor (float, optional): calibration factor of device readout to mg. Defaults to CALIBRATION_FACTOR.
         """
-        self.port = port
-        self._baudrate = baudrate
-        self._timeout = timeout
-        device = None
+        super().__init__(**kwargs)
+        self.baseline = 0
+        self.buffer_df = pd.DataFrame(columns=COLUMNS)
+        self.calibration_factor = calibration_factor
+        self.precision = 3
+        self._mass = 0
+        self._threads = {}
+        self._connect(port)
+        return
+    
+    # Properties
+    @property
+    def mass(self) -> float:
+        return round(self._mass, self.precision)
+   
+    def clearCache(self):
+        """Clear most recent data and configurations"""
+        self.setFlag(pause_feedback=True)
+        time.sleep(0.1)
+        self.buffer_df = pd.DataFrame(columns=COLUMNS)
+        self.setFlag(pause_feedback=False)
+        return
+    
+    def disconnect(self):
+        """Disconnect from device"""
         try:
-            device = serial.Serial(port, 9600, timeout=1)
-            time.sleep(2)   # Wait for grbl to initialize
-            device.flushInput()
-            print(f"Connection opened to {port}")
+            self.device.close()
         except Exception as e:
             if self.verbose:
-                print(f"Could not connect to {port}")
                 print(e)
-        self.device = device
-        return self.device
-    
-    def _diagnostic(self):
-        """
-        Run diagnostic on tool
-        """
-        thread = Thread(target=self.execute, name=f'maker_diag_{self.order}')
-        thread.start()
-        time.sleep(1)
+        self.setFlag(connected=False)
         return
     
-    def _run_speed(self, speed:int):
+    def getMass(self) -> str:
         """
-        Relay spin speed to spinner
-
-        Args:
-            speed (int): spin speed
+        Get the mass of the sample by measuring the force response
+        
+        Returns:
+            str: device response
         """
+        response = self._read()
+        now = datetime.now()
         try:
-            self.device.write(bytes(f"{speed}\n", 'utf-8'))
-        except AttributeError:
+            value = int(response)
+        except ValueError:
             pass
-        print("Spin speed: {}".format(speed))
+        else:
+            self._mass = (value - self.baseline) / self.calibration_factor
+            if self.flags['record']:
+                values = [
+                    now, 
+                    value, 
+                    self.calibration_factor, 
+                    self.baseline, 
+                    self._mass
+                ]
+                row = {k:v for k,v in zip(COLUMNS, values)}
+                self.buffer_df = self.buffer_df.append(row, ignore_index=True)
+        return response
+  
+    def reset(self):
+        """Reset the device"""
+        super().reset()
+        self.baseline = 0
         return
     
-    def _run_spin_step(self, speed:int, run_time:int):
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        self.toggleFeedbackLoop(on=False)
+        return super().shutdown()
+ 
+    def tare(self):
+        """Alias for `zero()`"""
+        return self.zero()
+    
+    def toggleFeedbackLoop(self, on:bool):
         """
-        Perform timed spin step
+        Start or stop feedback loop
 
         Args:
-            speed (int): spin speed
-            run_time (int): spin time
-        """
-        interval = 1
-        start_time = time.time()
-        self._run_speed(speed)
-        
-        while(True):
-            time.sleep(0.1)
-            if (interval <= time.time() - start_time):
-                interval += 1
-            if (run_time <= time.time() - start_time):
-                self._run_speed(0)
-                break
-        return
-
-    def execute(self, soak_time=0, spin_speed=2000, spin_time=1, channel=None):
+            on (bool): whether to start loop to continuously read from device
         """
-        Executes the soak and spin steps
-
-        Args:
-            soak_time (int, optional): soak time. Defaults to 0.
-            spin_speed (int, optional): spin speed. Defaults to 2000.
-            spin_time (int, optional): spin time. Defaults to 1.
-            channel (int, optional): channel index. Defaults to None.
-        """
-        self._flags['busy'] = True
-        self.soak(soak_time)
-        self.spin(spin_speed, spin_time)
-        self._flags['busy'] = False
+        self.setFlag(get_feedback=on)
+        if on:
+            if 'feedback_loop' in self._threads:
+                self._threads['feedback_loop'].join()
+            thread = Thread(target=self._loop_feedback)
+            thread.start()
+            self._threads['feedback_loop'] = thread
+        else:
+            self._threads['feedback_loop'].join()
         return
     
-    def isBusy(self):
-        """
-        Checks whether the spinner is busy
-
-        Returns:
-            bool: whether the spinner is busy
-        """
-        return self._flags['busy']
-    
-    def isConnected(self):
+    def toggleRecord(self, on:bool):
         """
-        Checks whether the spinner is connected
+        Start or stop data recording
 
-        Returns:
-            bool: whether the spinner is connected
+        Args:
+            on (bool): whether to start recording temperature
         """
-        if self.device is None:
-            print(f"{self.__class__} ({self.port}) not connected.")
-            return False
-        return True
+        self.setFlag(record=on, get_feedback=on, pause_feedback=False)
+        self.toggleFeedbackLoop(on=on)
+        return
 
-    def soak(self, seconds:int, channel=None):
+    def zero(self, wait:int = 5):
         """
-        Executes the soak step
-
+        Set current reading as baseline (i.e. zero mass)
+        
         Args:
-            seconds (int): soak time
-            channel (int, optional): channel index. Defaults to None.
+            wait (int, optional): duration to wait while zeroing, in seconds. Defaults to 5.
         """
-        self.speed = 0
-        if seconds:
-            time.sleep(seconds)
+        temp_record_state = self.flags['record']
+        temp_buffer_df = self.buffer_df.copy()
+        self.reset()
+        self.toggleRecord(True)
+        print(f"Zeroing... ({wait}s)")
+        time.sleep(wait)
+        self.toggleRecord(False)
+        self.baseline = self.buffer_df['Value'].mean()
+        self.clearCache()
+        self.buffer_df = temp_buffer_df.copy()
+        print("Zeroing complete.")
+        self.toggleRecord(temp_record_state)
         return
 
-    def spin(self, speed:int, seconds:int, channel=None):
+    # Protected method(s)
+    def _connect(self, port:str, baudrate:int = 115200, timeout:int = 1):
         """
-        Executes the spin step
+        Connection procedure for tool
 
         Args:
-            speed (int): spin speed
-            seconds (int): spin time
-            channel (int, optional): channel index. Defaults to None.
-        """
-        self.speed = speed
-        self._run_spin_step(speed, seconds)
-        self.speed = 0
-        return
-
-
-class SpinnerAssembly(object):
-    """
-    Spinner assembly with multiple spinners
-
-    Args:
-        ports (list, optional): list of com port strings. Defaults to [].
-        channels (list, optional): list of int channel indices. Defaults to [].
-        positions (list, optional): list of tuples of x,y,z spinner positions. Defaults to [].
-    """
-    def __init__(self, ports=[], channels=[], positions=[]):
-        properties = Helper.zip_inputs('channel', port=ports, channel=channels, position=positions)
-        self.channels = {key: Spinner(**value) for key,value in properties.items()}
+            port (str): COM port address
+            baudrate (int, optional): baudrate. Defaults to 115200.
+            timeout (int, optional): timeout in seconds. Defaults to 1.
+        """
+        self.connection_details = {
+            'port': port,
+            'baudrate': baudrate,
+            'timeout': timeout
+        }
+        device = None
+        try:
+            device = serial.Serial(port, baudrate, timeout=timeout)
+        except Exception as e:
+            print(f"Could not connect to {port}")
+            if self.verbose:
+                print(e)
+        else:
+            print(f"Connection opened to {port}")
+            self.setFlag(connected=True)
+            time.sleep(1)
+            self.zero()
+        self.device = device
         return
     
-    def _diagnostic(self):
-        """
-        Run diagnostic on tool
-        """
-        for _,spinner in self.channels.items():
-            spinner._diagnostic()
+    def _loop_feedback(self):
+        """Loop to constantly read from device"""
+        print('Listening...')
+        while self.flags['get_feedback']:
+            if self.flags['pause_feedback']:
+                continue
+            self.getMass()
+        print('Stop listening...')
         return
-        
-    def execute(self, soak_time:int, spin_speed:int, spin_time:int, channel:int):
-        """
-        Executes the soak and spin steps
 
-        Args:
-            soak_time (int): soak time
-            spin_speed (int): spin speed
-            spin_time (int): spin time
-            channel (int): channel index
-        """
-        return self.channels[channel].execute(soak_time, spin_speed, spin_time)
-    
-    def isBusy(self):
+    def _read(self):
         """
-        Check whether any of the spinners are still busy
+        Read response from device
 
         Returns:
-            bool: whether any of the spinners are busy
+            str: response string
         """
-        return any([spinner.isBusy() for spinner in self.channels.values()])
-    
-    def isConnected(self):
-        """
-        Check whether all spinners are connected
-
-        Returns:
-            bool: whether all spinners are connected
-        """
-        return all([spinner.isConnected() for spinner in self.channels.values()])
-    
-    def soak(self, seconds:int, channel:int):
-        """
-        Executes the soak step
-
-        Args:
-            seconds (int): soak time
-            channel (int): channel index
-        """
-        return self.channels[channel].soak(seconds)
-    
-    def spin(self, speed:int, seconds:int, channel:int):
-        """
-        Executes the spin step
-
-        Args:
-            speed (int): spin speed
-            seconds (int): spin time
-            channel (int): channel index
-        """
-        return self.channels[channel].spin(speed, seconds)
+        response = ''
+        try:
+            response = self.device.readline()
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        else:
+            response = response.decode('utf-8').strip()
+            if self.verbose:
+                print(response)
+        return response
+
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.0.0a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,629 +1,521 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/02 17:13:35
-@author: Chang Jie
+This module holds the instrument class for tools from Keithley.
 
-Notes / actionables:
-- validation on copper
+Classes:
+    KeithleyDevice (Instrument)
 """
 # Standard library imports
+from __future__ import annotations
 import numpy as np
 import pandas as pd
+from typing import Optional, Union
 
 # Third party imports
 import pyvisa as visa # pip install -U pyvisa
 
 # Local application imports
+from ...instrument_utils import Instrument
+from .keithley_lib import SenseDetails, SourceDetails
 print(f"Import: OK <{__name__}>")
 
-class KeithleyDevice(object):
+class KeithleyDevice(Instrument):
     """
-    Keithley device object
+    KeithleyDevice provides methods to interface with the potentiometer from Keithley
     
+    ### Constructor
     Args:
-        ip_address (str): IP address of Keithley
-        name (str, optional): nickname for Keithley. Defaults to 'def'.
+        `ip_address` (str): IP address of device
+        `name` (str, optional): name of device. Defaults to 'def'.
+        
+    ### Attributes
+    - `active_buffer` (str): name of active buffer in Keithley
+    - `name` (str): name of device
+    - `sense` (SenseDetails): parameters for Keithley's sense terminal
+    - `source` (SourceDetails): parameters for Keithley's source terminal
+    
+    ### Properties
+    - `buffer_name` (str): name of buffer
+    - `fields` (tuple[str]): tuple of data fields to read from device
+    
+    ### Methods
+    - `beep`: make device emit a beep sound
+    - `clearBuffer`: clear the buffer on the device
+    - `configureSense`: configure the sense terminal
+    - `configureSource`: configure the source terminal
+    - `disconnect`: disconnect from device (NOTE: not implemented)
+    - `getBufferIndices`: get the buffer indices where the the data start and end
+    - `getErrors`: get error messages from device
+    - `getStatus`: get status of device
+    - `makeBuffer`: create a new buffer on the device
+    - `read`: read the latest data from buffer
+    - `readAll`: read the data from buffer after a series of measurements
+    - `recallState`: recall a previously saved device setting
+    - `reset`: reset the device
+    - `run`: start the measurement
+    - `saveState`: save current settings on device
+    - `sendCommands`: write a series of commands to device
+    - `setSource`: set the source to a specified value
+    - `stop`: abort all actions
+    - `toggleOutput`: turn on or off output from device
     """
-    def __init__(self, ip_address:str, name='def'):
-        self._ip_address = ip_address
-        self._name = name
-        self.instrument = None
-        
-        self._active_buffer = 'defbuffer1'
-        self._sense_details = {}
-        self._source_details = {}
-        
-        self.verbose = True
-        self._flags = {
-            'busy': False
-        }
-        self.connect(ip_address)
-        return
-    
-    @property
-    def buffer_name(self):
-        return f'{self.name}buffer'
-    
-    @property
-    def ip_address(self):
-        return self._ip_address
-    
-    @property
-    def name(self):
-        return self._name
-    
-    @property
-    def sense(self):
-        return self._sense_details['function']
-    @sense.setter
-    def sense(self, func:str):
-        self._sense_details['function'] = self._get_function(func=func, sense=True)
-        return
-    
-    @property
-    def source(self):
-        return self._source_details['function']
-    @source.setter
-    def source(self, func:str):
-        self._source_details['function'] = self._get_function(func=func, sense=False)
-        return
-    
-    @staticmethod
-    def _get_fields(fields:list):
-        """
-        Check list of fields
-
-        Args:
-            fields (list): list of fields to retrieve from the buffer
-
-        Raises:
-            Exception: List should have 14 or fewer items
-
-        Returns:
-            list: list of fields
-        """
-        if len(fields) > 14:
-            raise Exception("Please input 14 or fewer buffer elements to read out")
-        return fields
-    
-    @staticmethod
-    def _get_function(func:str, sense=True):
-        """
-        Get the function name and check for validity
-
-        Args:
-            func (str): function name from current, resistance, and voltage
-            sense (bool, optional): whether function is for sensing. Defaults to True.
-
-        Raises:
-            Exception: Select a valid function
-
-        Returns:
-            str: function name
-        """
-        func = func.upper()
-        valid_functions = ['current', 'resistance', 'voltage'] if sense else ['current', 'voltage']
-        if func in ['CURR','CURRENT']:
-            return 'CURRent'
-        elif func in ['RES','RESISTANCE'] and sense:
-            return 'RESistance'
-        elif func in ['VOLT','VOLTAGE']:
-            return 'VOLTage'
-        raise Exception(f"Select a valid function from: {', '.join(valid_functions)}")
-    
-    @staticmethod
-    def _get_limit(limit, current=True):
-        """
-        Get the limits for input
-
-        Args:
-            limit (str, or float): limit of source or reading
-            current (bool, optional): whether limit is for current. Defaults to True.
-
-        Raises:
-            Exception: Select a valid string from default, maximum, minimum
-            Exception: Select a valid current limit
-
-        Returns:
-            str: limit
-        """
-        if limit is None:
-            return 'AUTO ON'
-        if type(limit) == str:
-            if limit.upper() in ['DEF','DEFAULT','MAX','MAXIMUM','MIN','MINIMUM']:
-                return limit
-            raise Exception(f"Select a valid function from: default, maximum, minimum")
-        lim = 0
-        unit = ''
-        if current:
-            unit = 'A'
-            for lim in [10e-9, 100e-9, 1e-6, 10e-6, 100e-6, 1e-3, 10e-3, 100e-3, 1]:
-                if lim >= abs(limit):
-                    return lim
-        else:
-            unit = 'V'
-            for lim in [20e-3, 200e-3, 2, 20, 200]:
-                if lim >= abs(limit):
-                    return lim
-        raise Exception(f'Please set a current limit that is between -{lim} and {lim} {unit}')
     
-    @staticmethod
-    def _get_limit_type(source):
+    _default_buffer = 'defbuffer1'
+    def __init__(self, ip_address:str, name:str = 'def', **kwargs):
         """
-        Get the limit type for the source
-
+        Instantiate the class
+        
         Args:
-            source (str): function type of source
-
-        Returns:
-            str: 'ILIMit' or 'VLIMit'
+            ip_address (str): IP address of device
+            name (str, optional): name of device. Defaults to 'def'.
         """
-        if source == 'CURRent':
-            return 'VLIMit'
-        return 'ILIMit'
+        super().__init__(**kwargs)
+        self.name = name
+        self._fields = ('',)
+        
+        self.active_buffer = self._default_buffer
+        self.sense = SenseDetails()
+        self.source = SourceDetails()
+        self._connect(ip_address)
+        return
     
-    def __info__(self):
+    def __info__(self) -> str:
         """
         Get device system info
 
         Returns:
             str: system info
         """
-        return self._send('*IDN?')
-    
-    def _generate_commands(self, sense=True):
-        func_details = self._sense_details if sense else self._source_details
-        header = 'SENSe' if sense else 'SOURce'
-        excluded_keys = ['COUNt', 'function', 'invoked']
-        commands = [f'{header}:{func_details["function"]}:{key} {value}' for key,value in func_details.items() if key not in excluded_keys]
-        
-        for i,command in enumerate(commands):
-            if 'AUTO' in command:
-                new_command = ':AUTO'.join((command.split(' AUTO')))
-                commands[i] = new_command
-        if sense:
-            commands = commands + [f'SENSe:COUNt {func_details.get("COUNt",1)}']
-        return commands
-    
-    def _parse_reply(self, raw_reply:str):
-        """
-        Parse the response from instrument
-
-        Args:
-            raw_reply (str): raw response string from instrument
-
-        Returns:
-            float, str, or list: float for numeric values, str for strings, list for multiple replies
-        """
-        if ',' in raw_reply:
-            replies = raw_reply.split(',')
-        elif ';' in raw_reply:
-            replies = raw_reply.split(';')
-        else:
-            try:
-                raw_reply = float(raw_reply)
-            finally:
-                return raw_reply
-        output = []
-        for reply in replies:
-            try:
-                output.append(float(reply))
-            except ValueError:
-                output.append(reply)
-        if self.verbose:
-            print(output)
-            self.getErrors()
-        return output
+        return self._query('*IDN?')
     
-    def _send(self, command:str):
-        """
-        Write command to instrument, using query if expecting reply
-
-        Args:
-            command (str): command string to write
-
-        Returns:
-            any: response from query, or None
-        """
-        reply = None 
-        if self.instrument is None:
-            print(command)
-            _dummy_return = [0 for _ in range(command.count(';')+1)] if "?" in command else None
-            return _dummy_return
-        if self.verbose:
-            print(command)
-        try:
-            if "?" not in command:
-                self.instrument.write(command)
-            else:
-                raw_reply = self._query(command)
-                reply = self._parse_reply(raw_reply=raw_reply)
-            if self.verbose and "*WAI" not in command:
-                self.getErrors()
-        except visa.VisaIOError:
-            self.getErrors()
-        return reply
+    # Properties
+    @property
+    def buffer_name(self) -> str:
+        return f'{self.name}buffer'
     
-    def _query(self, command:str):
-        """
-        Perform a query on instrument
-
-        Args:
-            command (str): command string to query
-
-        Returns:
-            str: response from query, or None
-        """
-        reply = ''
-        if self.instrument is not None:
-            reply = self.instrument.query(command)
-        # self.instrument.write(command)
-        # while reply is None:
-        #     reply = self.instrument.read()
-        return reply
+    @property
+    def fields(self) -> tuple[str]:
+        return self._fields
+    @fields.setter
+    def fields(self, value:tuple[str]):
+        if len(value) > 14:
+            raise RuntimeError("Please input 14 or fewer fields to read out from instrument.")
+        self._fields = tuple(value)
+        return
     
-    def beep(self, frequency=440, duration=1):
+    def beep(self, frequency:int = 440, duration:float = 1):
         """
-        Set off beeper
+        Make device emit a beep sound
 
         Args:
             frequency (int, optional): frequency of sound wave. Defaults to 440.
             duration (int, optional): duration to play beep. Defaults to 1.
-
-        Raises:
-            Exception: Select a valid frequency
-            Exception: select a valid duration
         """
         if not 20<=frequency<=8000:
-            raise Exception('Please enter a frequency between 20 and 8000')
+            print('Please enter a frequency between 20 and 8000')
+            print('Defaulting to 440 Hz')
+            frequency = 440
         if not 0.001<=duration<=100:
-            raise Exception('Please enter a duration between 0.001 and 100')
-        return self._send(f'SYSTem:BEEPer {frequency},{duration}')
+            print('Please enter a duration between 0.001 and 100')
+            print('Defaulting to 1 s')
+            duration = 1
+        return self._query(f'SYSTem:BEEPer {frequency},{duration}')
     
-    def clearBuffer(self, name=None):
+    def clearBuffer(self, name:Optional[str] = None):
         """
-        Clear buffer
+        Clear the buffer on the device
 
         Args:
-            name (str, optional): name of buffer to clear. Defaults to None.
+            name (Optional[str] , optional): name of buffer to clear. Defaults to None.
         """
-        if name is None:
-            name = self._active_buffer
-        return self._send(f'TRACe:CLEar "{name}"')
+        name = self.active_buffer if name is None else name
+        return self._query(f'TRACe:CLEar "{name}"')
     
-    def configure(self, commands:list):
+    def configureSense(self, 
+        func: str, 
+        limit: Union[str, float, None] = 'DEFault',
+        four_point: bool = True,
+        count: int = 1
+    ):
         """
-        Write multiple commands to instrument
+        Configure the sense terminal
 
         Args:
-            commands (list): list of commands to write
+            func (str): name of function, choice from current, resistance, and voltage
+            limit (Union[str, float, None], optional): sensing range. Defaults to 'DEFault'.
+            four_point (bool, optional): whether to use four-point probe measurement. Defaults to True.
+            count (int, optional): number of readings to measure for each condition. Defaults to 1.
         """
-        for command in commands:
-            self._send(command)
-        return
-
-    def configureSense(self, func, limit='DEFault', probe_4_point=True, unit=None, count=1):
+        self.sense = SenseDetails(func, limit, four_point, count)
+        self._query(f'SENSe:FUNCtion "{self.sense.function_type}"')
+        return self.sendCommands(commands=self.sense.get_commands())
+    
+    def configureSource(self, 
+        func: str, 
+        limit: Union[str, float, None] = None,
+        measure_limit: Union[str, float, None] = 'DEFault'
+    ):
         """
-        Configure the sense function
+        Configure the source terminal
 
         Args:
-            func (str): function to be read, from current, resistance, and voltage
-            limit (str or float, optional): sensing range. Defaults to 'DEFault'.
-            probe_4_point (bool, optional): whether to use 4-point reading. Defaults to True.
-            unit (str, optional): units for reading. Defaults to None.
-            count (int, optional): number of readings per measurement. Defaults to 1.
-
-        Raises:
-            Exception: Select a valid count number
+            func (str): name of function, choice from current and voltage
+            limit (Union[str, float, None], optional): sourcing range. Defaults to None.
+            measure_limit (Union[str, float, None], optional): limit imposed on the measurement range. Defaults to 'DEFault'.
         """
-        self.sense = func
-        self._send(f'SENSe:FUNCtion "{self.sense}"')
-        
-        is_current = (self.sense=='CURRent')
-        if unit is None:
-            if self.sense == 'CURRent':
-                unit = 'AMP'
-            elif self.sense == 'VOLTage':
-                unit = 'VOLT'
-        count_upper_limit = min(300000, 300000)
-        count = max(1,count)
-        if count>count_upper_limit:
-            raise Exception(f"Please select a count from 1 to {count_upper_limit}")
-        kwargs = {
-            'RANGe': self._get_limit(limit=limit, current=is_current),
-            'RSENse': 'ON' if probe_4_point else 'OFF',
-            'UNIT': unit,
-            'COUNt': int(count)
-        }
-        self._sense_details.update(kwargs)
-        commands = self._generate_commands(sense=True)
-        return self.configure(commands=commands)
-    
-    def configureSource(self, func, limit=None, measure_limit='DEFault'):
-        """
-        Configure the source function
-
-        Args:
-            func (str): function to be sourced, from current, and voltage
-            limit (str or float, optional): sourcing range. Defaults to None.
-            measure_limit (str or float, optional): limit imposed on the measurement range. Defaults to 'DEFault'.
-        """
-        self.source = func
-        self._send(f'SOURce:FUNCtion {self.source}')
-        
-        is_current = (self.source=='CURRent')
-        kwargs = {
-            'RANGe': self._get_limit(limit=limit, current=is_current),
-            self._get_limit_type(self.source): self._get_limit(limit=measure_limit, current=not(is_current))
-        }
-        self._source_details.update(kwargs)
-        self._source_details.update({'invoked': 0})
-        commands = self._generate_commands(sense=False)
-        return self.configure(commands=commands)
+        self.source = SourceDetails(func, limit, measure_limit)
+        self._query(f'SOURce:FUNCtion {self.source.function_type}')
+        return self.sendCommands(commands=self.source.get_commands())
     
-    def connect(self, ip_address=None):
-        """
-        Establish connection with Keithley
-        
-        Args:
-            ip_address (str, optional): IP address of Keithley. Defaults to None
-            
-        Returns:
-            Instrument: Keithley object
-        """
-        print("Setting up Keithley communications...")
-        if ip_address is None:
-            ip_address = self.ip_address
-        self._ip_address = ip_address
-        instrument = None
-        try:
-            rm = visa.ResourceManager('@py')
-            instrument = rm.open_resource(f"TCPIP0::{ip_address}::5025::SOCKET")
-            self.instrument = instrument
-            instrument.write_termination = '\n'
-            instrument.read_termination = '\n'
-            
-            self.beep(500)
-            print(f"{self.__info__()}")
-            print(f"{self.name.title()} Keithley ready")
-        except Exception as e:
-            print("Unable to connect to Keithley!")
-            if self.verbose:
-                print(e) 
-        return instrument
+    def disconnect(self):       # NOTE: not implemented
+        return super().disconnect()
     
-    def getBufferIndices(self, name=None):
+    def getBufferIndices(self, name:Optional[str] = None) -> tuple[int]:
         """
-        Get the start and end buffer indices
+        Get the buffer indices where the the data start and end
 
         Args:
-            name (str, optional): name of buffer. Defaults to None.
+            name (Optional[str], optional): name of buffer. Defaults to None.
 
         Returns:
-            list: start and end buffer indices
+            tuple[int]: start and end buffer indices
         """
-        if name is None:
-            name = self.buffer_name
-        return self._send(f'TRACe:ACTual:STARt? "{name}" ; END? "{name}"')
+        name = self.buffer_name if name is None else name
+        reply = self._query(f'TRACe:ACTual:STARt? "{name}" ; END? "{name}"')
+        try:
+            start,end = self._parse(reply=reply)
+            start = int(start)
+            end = int(end)
+        except ValueError:
+            return 0,0
+        start = max(1, start)
+        end = max(start, end)
+        return start,end
     
-    def getErrors(self):
+    def getErrors(self) -> list[str]:
         """
-        Get Errors from Keithley
+        Gget error messages from device
+        
+        Returns:
+            list[str]: list of error messages from device
         """
         errors = []
-        reply = self._query('SYSTem:ERRor:COUNt?')
+        reply = ''
         while not reply.isnumeric():
-            print(reply)
             reply = self._query('SYSTem:ERRor:COUNt?')
+            print(reply)
         num_errors = int(reply)
         for i in range(num_errors):
-            error = self._query('SYSTem:ERRor?')
+            reply = self._query('SYSTem:ERRor?')
+            error = self._parse(reply=reply)
             errors.append((error))
             print(f'>>> Error {i+1}: {error}')
         return errors
     
-    def getStatus(self):
+    def getStatus(self) -> str:
         """
-        Get status of instrument
+        Get status of device
 
         Returns:
-            str: instrument state
-        """
-        return self._send('TRIGger:STATe?')
-    
-    def isBusy(self):
-        """
-        Checks whether the instrument is busy
-        
-        Returns:
-            bool: whether the instrument is busy
+            str: device status
         """
-        return self._flags['busy']
+        return self._query('TRIGger:STATe?')
     
-    def isConnected(self):
+    def makeBuffer(self, name:Optional[str] = None, buffer_size:int = 100000):
         """
-        Check whether instrument is connected
-
-        Returns:
-            bool: whether instrument is connected
-        """
-        if self.instrument is None:
-            return False
-        return True
-    
-    def makeBuffer(self, name=None, buffer_size=100000):
-        """
-        Make a buffer on the instrument
+        Create a new buffer on the device
 
         Args:
-            name (str, optional): buffer name. Defaults to None.
+            name (Optional[str] , optional): buffer name. Defaults to None.
             buffer_size (int, optional): buffer size. Defaults to 100000.
         """
-        if name is None:
-            name = self.buffer_name
-            self._active_buffer = name
+        name = self.buffer_name if name is None else name
+        self.active_buffer = name
         if buffer_size < 10 and buffer_size != 0:
             buffer_size = 10
-        return self._send(f'TRACe:MAKE "{name}",{buffer_size}')
+        return self._query(f'TRACe:MAKE "{name}",{buffer_size}')
     
-    def readAll(self, name=None, fields=['SOURce','READing', 'SEConds'], average=True):
+    def read(self, 
+        name: Optional[str] = None, 
+        fields: tuple[str] = ('SOURce','READing', 'SEConds'), 
+        average: bool = True
+    ) -> pd.DataFrame:
         """
-        Read all data on buffer
+        Read the latest data fom buffer
 
         Args:
-            name (str, optional): buffer name. Defaults to None.
-            fields (list, optional): fields of interest. Defaults to ['SOURce','READing', 'SEConds'].
+            name (Optional[str], optional): buffer name. Defaults to None.
+            fields (tuple[str], optional): fields of interest. Defaults to ('SOURce','READing', 'SEConds').
             average (bool, optional): whether to average the data of multiple readings. Defaults to True.
 
         Returns:
             pd.DataFrame: dataframe of measurements
         """
-        if name is None:
-            name = self._active_buffer
-        fields = self._get_fields(fields=fields)
-        start,end = self.getBufferIndices(name=name)
-        start = max(1, start)
-        end = max(start, end)
-        count = self._sense_details.get('COUNt', 1)
+        return self._read(bulk=False, name=name, fields=fields, average=average)
         
-        data = self._send(f'TRACe:DATA? {int(start)},{int(end)},"{name}",{",".join(fields)}')
-        if not all([start,end]): # dummy data
-            num_rows = count * max(1, self._source_details.get('invoked', 1))
-            data = [0] * int(num_rows * len(fields))
-        data = np.reshape(np.array(data), (-1,len(fields)))
-        df = pd.DataFrame(data, columns=fields)
-        if average and count > 1:
-            avg = df.groupby(np.arange(len(df))//count).mean()
-            std = df.groupby(np.arange(len(df))//count).std()
-            df = avg.join(std, rsuffix='_std')
-        return df
-    
-    def readPacket(self, name=None, fields=['SOURce','READing', 'SEConds'], average=True):
+    def readAll(self, 
+        name: Optional[str] = None, 
+        fields: tuple[str] = ('SOURce','READing', 'SEConds'), 
+        average: bool = True
+    ) -> pd.DataFrame:
         """
-        Read data on buffer as measurements take place
+        Read the data from buffer after a series of measurements
 
         Args:
-            name (str, optional): buffer name. Defaults to None.
-            fields (list, optional): fields of interest. Defaults to ['SOURce','READing', 'SEConds'].
-            average (bool, optional): whether ot average the data of multiple readings. Defaults to True.
+            name (Optional[str], optional): buffer name. Defaults to None.
+            fields (tuple[str], optional): fields of interest. Defaults to ('SOURce','READing', 'SEConds').
+            average (bool, optional): whether to average the data of multiple readings. Defaults to True.
 
         Returns:
             pd.DataFrame: dataframe of measurements
         """
-        if name is None:
-            name = self._active_buffer
-        fields = self._get_fields(fields=fields)
-        _start,end = self.getBufferIndices(name=name)
-        _start = max(1, _start)
-        end = max(_start, end)
-        count = self._sense_details.get('COUNt', 1)
-        start = max(1, end - count + 1)
-        
-        data = self._send(f'TRACe:DATA? {int(start)},{int(end)},"{name}",{",".join(fields)}')
-        if not all([start,end]): # dummy data
-            data = [0] * int(count * len(fields))
-        data = np.reshape(np.array(data), (-1,len(fields)))
-        df = pd.DataFrame(data, columns=fields)
-        if average and count > 1:
-            avg = df.groupby(np.arange(len(df))//count).mean()
-            std = df.groupby(np.arange(len(df))//count).std()
-            df = avg.join(std, rsuffix='_std')
-        return df
+        return self._read(bulk=True, name=name, fields=fields, average=average)
     
     def recallState(self, state:int):
         """
-        Recall a previously saved settings of instrument
+        Recall a previously saved device setting
 
         Args:
             state (int): state index to recall from
 
         Raises:
-            Exception: Select an index from 0 to 4
+            ValueError: Select an index from 0 to 4
         """
         if not 0 <= state <= 4:
-            raise Exception("Please select a state index from 0 to 4")
-        return self._send(f'*RCL {state}')
+            raise ValueError("Please select a state index from 0 to 4")
+        return self._query(f'*RCL {state}')
     
     def reset(self):
+        """Reset the device"""
+        self.active_buffer = self._default_buffer
+        self.sense = SenseDetails()
+        self.source = SourceDetails()
+        return self._query('*RST')
+    
+    def run(self, sequential_commands:bool = True):
         """
-        Reset the instrument
+        Start the measurement
+
+        Args:
+            sequential_commands (bool, optional): whether commands whose operations must finish before the next command is executed. Defaults to True.
         """
-        self._active_buffer = 'defbuffer1'
-        self._sense_details = {}
-        self._source_details = {}
-        return self._send('*RST')
+        if sequential_commands:
+            commands = [f'TRACe:TRIGger "{self.active_buffer}"']
+        else:
+            commands = ['INITiate ; *WAI']
+        return self.sendCommands(commands=commands)
     
     def saveState(self, state:int):
         """
-        Save current settings / state of instrument
+        Save current settings on device
 
         Args:
             state (int): state index to save to
 
         Raises:
-            Exception: Select an index from 0 to 4
+            ValueError: Select an index from 0 to 4
         """
         if not 0 <= state <= 4:
-            raise Exception("Please select a state index from 0 to 4")
-        return self._send(f'*SAV {state}')
+            raise ValueError("Please select a state index from 0 to 4")
+        return self._query(f'*SAV {state}')
     
-    def setFlag(self, name:str, value:bool):
+    def sendCommands(self, commands:list[str]):
         """
-        Set a flag truth value
+        Write a series of commands to device
 
         Args:
-            name (str): label
-            value (bool): flag value
+            commands (list[str]): list of commands strings
         """
-        self._flags[name] = value
+        for command in commands:
+            self._query(command)
         return
-
-    def setSource(self, value):
+    
+    def setSource(self, value:float):
         """
-        Set source to desired value
+        Set the source to a specified value
 
         Args:
-            value (int or float): value to set source to 
+            value (float): value to set source to 
 
         Raises:
-            Exception: Set a value within limits
+            ValueError: Please set a source value within limits
         """
-        capacity = 1 if self.source=='CURRent' else 200
-        limit = self._source_details.get('RANGe', capacity)
-        if type(limit) == str:
-            limit = capacity
-        unit = 'A' if self.source=='CURRent' else 'V'
+        unit = 'A' if self.source.function_type == 'CURRent' else 'V'
+        capacity = 1 if self.source.function_type == 'CURRent' else 200
+        limit = capacity if type(self.source.range_limit) is str else self.source.range_limit
+        
         if abs(value) > limit:
-            raise Exception(f'Please set a source value between -{limit} and {limit} {unit}')
-        self._source_details['invoked'] += 1
-        return self._send(f'SOURce:{self.source} {value}')
+            raise ValueError(f'Please set a source value between -{limit} and {limit} {unit}')
+        self.source._count += 1
+        return self._query(f'SOURce:{self.source.function_type} {value}')
+
+    def stop(self):
+        """Abort all actions"""
+        return self._query('ABORt')
 
-    def start(self, sequential_commands=True):
+    def toggleOutput(self, on:bool):
         """
-        Initialise the measurement
+        Turn on or off output from device
 
         Args:
-            sequential_commands (bool, optional): whether commands whose operations must finish before the next command is executed. Defaults to True.
+            on (bool): whether to turn on output
         """
-        if sequential_commands:
-            commands = [f'TRACe:TRIGger "{self._active_buffer}"']
+        state = 'ON' if on else 'OFF'
+        return self._query(f'OUTPut {state}')
+    
+    # Protected method(s)
+    def _connect(self, ip_address:str):
+        """
+        Connection procedure for tool
+        
+        Args:
+            ip_address (str): IP address of device
+        """
+        print("Setting up Keithley communications...")
+        self.connection_details['ip_address'] = ip_address
+        device = None
+        try:
+            rm = visa.ResourceManager('@py')
+            device = rm.open_resource(f"TCPIP0::{ip_address}::5025::SOCKET")
+            device.write_termination = '\n'
+        except Exception as e:
+            print("Unable to connect to Keithley")
+            if self.verbose:
+                print(e) 
         else:
-            commands = ['INITiate ; *WAI']
-        return self.configure(commands=commands)
+            device.read_termination = '\n'
+            self.device = device
+            self.setFlag(connected=True)
+            self.beep(500)
+            print(f"{self.__info__()}")
+            print(f"{self.name.title()} Keithley ready")
+        self.device = device
+        return
 
-    def stop(self):
+    def _parse(self, reply:str) -> Union[float, str, tuple[Union[float, str]]]:
         """
-        Abort all actions
+        Parse the response from device
+
+        Args:
+            reply (str): raw response string from device
+
+        Returns:
+            Union[float, str, tuple[Union[float, str]]]: variable output including floats, strings, and tuples
         """
-        return self._send('ABORt')
+        if ',' not in reply and ';' not in reply:
+            try:
+                reply = float(reply)
+            except ValueError:
+                pass
+            return reply
+        
+        if ',' in reply:
+            replies = reply.split(',')
+        elif ';' in reply:
+            replies = reply.split(';')
 
-    def toggleOutput(self, on:bool):
+        outs = []
+        for reply in replies:
+            try:
+                out = float(reply)
+            except ValueError:
+                pass
+            outs.append(out)
+        if self.verbose:
+            print(tuple(outs))
+        return tuple(outs)
+    
+    def _query(self, command:str) -> str:
         """
-        Toggle turning on output
+        Write command to and read response from device
 
         Args:
-            on (bool): whether to turn on output
+            command (str): SCPI command string
+
+        Returns:
+            str: response string
         """
-        state = 'ON' if on else 'OFF'
-        return self._send(f'OUTPut {state}')
-    
+        if self.verbose:
+            print(command)
+        
+        if not self.isConnected():
+            print(command)
+            dummy_return = ';'.join(['0' for _ in range(command.count(';')+1)]) if "?" in command else ''
+            return dummy_return
+        
+        if "?" not in command:
+            self._write(command)
+            return ''
+        
+        reply = ''
+        try:
+            reply = self.device.query(command)
+            # self.device.write(command)
+            # while raw_reply is None:
+            #     raw_reply = self.device.read()
+        except visa.VisaIOError:
+            self.getErrors()
+        else:
+            if self.verbose and "*WAI" not in command:
+                self.getErrors()
+        return reply
+    
+    def _read(self, 
+        bulk: bool,
+        name: Optional[str] = None, 
+        fields: tuple[str] = ('SOURce','READing', 'SEConds'), 
+        average: bool = True
+    ) -> pd.DataFrame:
+        """
+        Read all data on buffer
+
+        Args:
+            bulk (bool): whether to read data after a series of measurements
+            name (Optional[str], optional): buffer name. Defaults to None.
+            fields (tuple[str], optional): fields of interest. Defaults to ('SOURce','READing', 'SEConds').
+            average (bool, optional): whether to average the data of multiple readings. Defaults to True.
+
+        Returns:
+            pd.DataFrame: dataframe of measurements
+        """
+        name = self.active_buffer if name is None else name
+        self.fields = fields
+        count = int(self.sense.count)
+        start,end = self.getBufferIndices(name=name)
+        
+        start = start if bulk else max(1, end-count+1)
+        if not all([start,end]): # dummy data
+            num_rows = count * max(1, int(self.source._count)) if bulk else count
+            data = [0] * num_rows * len(self.fields)
+        else:
+            reply = self._query(f'TRACe:DATA? {int(start)},{int(end)},"{name}",{",".join(self.fields)}')
+            data = self._parse(reply=reply)
+        
+        data = np.reshape(np.array(data), (-1,len(self.fields)))
+        df = pd.DataFrame(data, columns=self.fields)
+        if average and count > 1:
+            avg = df.groupby(np.arange(len(df))//count).mean()
+            std = df.groupby(np.arange(len(df))//count).std()
+            df = avg.join(std, rsuffix='_std')
+        return df
+    
+    def _write(self, command:str) -> bool:
+        """
+        Write command to device
+
+        Args:
+            command (str): SCPI command string
+
+        Returns:
+            bool: whether command was sent successfully
+        """
+        if self.verbose:
+            print(command)
+        try:
+            self.device.write(command)
+        except visa.VisaIOError:
+            self.getErrors()
+            return False
+        if self.verbose and "*WAI" not in command:
+            self.getErrors()
+        return True
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.0.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,325 +1,306 @@
 # %% -*- coding: utf-8 -*-
 """
-Adapted from DMA code by @pablo
+This module holds the instrument class for tools from PiezoRobotics.
 
-Created: Tue 2023/01/03 17:13:35
-@author: Chang Jie
+Classes:
+    PiezoRoboticsDevice (Instrument)
 
-Notes / actionables:
--
+Other constants and variables:
+    FREQUENCIES (tuple)
 """
 # Standard library imports
+from __future__ import annotations
 import numpy as np
 import pandas as pd
 import time
+from typing import Optional, Union
 
 # Third party imports
 import serial # pip install pyserial
 
 # Local application imports
-from .piezorobotics_lib import ErrorCode, FrequencyCode
-from .piezorobotics_lib import COMMANDS, ERRORS, FREQUENCIES
+from ...instrument_utils import Instrument
+from .piezorobotics_lib import CommandCode, ErrorCode, FrequencyCode, Frequency
 print(f"Import: OK <{__name__}>")
 
-TIMEOUT_S = 60
+FREQUENCIES = tuple([frequency.value for frequency in FrequencyCode])
+"""Collection of all available frequency values"""
 
-class PiezoRoboticsDevice(object):
+class PiezoRoboticsDevice(Instrument):
     """
-    PiezoRoboticsDevice object
+    PiezoRoboticsDevice provides methods to interface with the characterisation device from PiezoRobotics
 
+    ### Constructor
     Args:
-        port (str): com port address
-        channel (int, optional): assigned device channel. Defaults to 1.
+        `port` (str): COM port address
+        `channel` (int, optional): channel id. Defaults to 1.
+        
+    ### Attributes
+    - `channel` (int): channel id
+    
+    ### Properties
+    - `frequency` (Frequency): lower and upper frequency range limit
+    
+    ### Methods
+    - `disconnect`: disconnect from device
+    - `initialise`: initialise the device with the desired frequency range
+    - `readAll`: read all the data on device buffer
+    - `reset`: reset the device
+    - `run`: start the measurement
+    - `setFrequency`: frequency range to measure
+    - `shutdown`: shutdown procedure for tool
+    - `toggleClamp`: close or open the clamp
     """
-    def __init__(self, port:str, channel=1, **kwargs):
+    
+    _default_flags = {
+        'busy': False,
+        'connected': False,
+        'initialised': False,
+        'measured': False,
+        'read': False
+    }
+    def __init__(self, port:str, channel:int = 1, **kwargs):
+        """
+        Instantiate the class
+
+        Args:
+            port (str): COM port address
+            channel (int, optional): channel id. Defaults to 1.
+        """
+        super().__init__(**kwargs)
         self.channel = channel
-        self.instrument = None
-        
-        self._frequency_range_codes = ('0','0')
-        
-        self.verbose = True
-        self._flags = {
-            'busy': False,
-            'connected': False,
-            'initialised': False,
-            'measured': False,
-            'read': False
-        }
-        self.port = ''
-        self._baudrate = None
-        self._timeout = None
+        self._frequency = Frequency()
         self._connect(port)
         pass
     
+    # Properties
     @property
-    def frequency_codes(self):
-        lo_code, hi_code = self._frequency_range_codes
-        return int(lo_code[-2:]), int(hi_code[-2:])
+    def frequency(self) -> Frequency:
+        return self._frequency
+    @frequency.setter
+    def frequency(self, value: tuple[float]):
+        """
+        Set the operating frequency range
+
+        Args:
+            value (tuple[float]): frequency lower and upper limits
+        """
+        self._frequency = self._range_finder(frequencies=value)
+        return
     
     @property
-    def frequency_range(self):
-        lo_code, hi_code = self._frequency_range_codes
-        return FrequencyCode[lo_code].value, FrequencyCode[hi_code].value
-    @frequency_range.setter
-    def frequency_range(self, frequencies):
+    def port(self) -> str:
+        return self.connection_details.get('port', '')
+    
+    def disconnect(self):
+        """Disconnect from device"""
+        try:
+            self.device.close()
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        self.setFlag(connected=False)
+        return
+    
+    def initialise(self, low_frequency:Optional[float] = None, high_frequency:Optional[float] = None):
         """
-        Set the operating frequency range
+        Initialise the device with the desired frequency range
 
         Args:
-            frequencies (iterable): frequency lower and upper limits
-                low_frequency (float): lower frequency limit
-                high_frequency (float): upper frequency limit
+            low_frequency (Optional[float], optional): lowest desired frequency. Defaults to None.
+            high_frequency (Optional[float], optional): highest desired frequency. Defaults to None.
         """
-        lo_code_number, hi_code_number = self.range_finder(frequencies=frequencies)
-        self._frequency_range_codes = (f'FREQ_{lo_code_number:02}', f'FREQ_{hi_code_number:02}')
+        if not all((low_frequency, high_frequency)):
+            low_frequency, high_frequency = FREQUENCIES[0], FREQUENCIES[-1]
+        if self.flags['initialised']:
+            return
+        frequency = self._range_finder(low_frequency, high_frequency)
+        if frequency == self.frequency:
+            print('Appropriate frequency range remains the same!')
+        else:
+            self.reset()
+            self._frequency = frequency
+            input("Ensure no samples within the clamp area during initialization. Press 'Enter' to proceed.")
+            self._query(f"INIT,{','.join(self.frequency.code)}")
+        self.setFlag(initialised=True)
+        print(self.frequency)
         return
+
+    def readAll(self, **kwargs) -> pd.DataFrame:
+        """
+        Read all data on device buffer
+            
+        Returns:
+            pd.DataFrame: dataframe of measurements
+        """
+        data = [line.split(', ') for line in self._query('GET,0') if ',' in line]
+        df = pd.DataFrame(data[1:], columns=data[0], dtype=float)
+        return df
     
-    @staticmethod
-    def range_finder(frequencies):
+    def reset(self) -> str:
+        """Reset the device"""
+        self._frequency = Frequency()
+        self.resetFlags()
+        return self._query('CLR,0')
+    
+    def run(self, sample_thickness:float = 1E-6) -> Optional[str]:
+        """Start the measurement"""
+        if not self.flags['initialised']:
+            self.initialise()
+        return self._query(f"RUN,{sample_thickness}")
+    
+    def setFrequency(self, low_frequency:float = None, high_frequency:float = None):
         """
-        Find the appropriate the operating frequency range
+        Set the frequency range to measure
 
         Args:
-            frequencies (iterable): frequency lower and upper limits
-                low_frequency (float): lower frequency limit
-                high_frequency (float): upper frequency limit
-        """
-        low_frequency, high_frequency = sorted(list(frequencies))
-        all_freq = np.array(FREQUENCIES)
-        freq_in_range_indices = np.where((all_freq>=low_frequency) & (all_freq<=high_frequency))
-        lo_code_number = max( (freq_in_range_indices[0][0]+1) - 1, 1)
-        hi_code_number = min( (freq_in_range_indices[0][-1]+1) + 1, len(all_freq))
-        return lo_code_number, hi_code_number
+            low_frequency (Optional[float], optional): lowest desired frequency. Defaults to None.
+            high_frequency (Optional[float], optional): highest desired frequency. Defaults to None.
+        """
+        return self.initialise(low_frequency=low_frequency, high_frequency=high_frequency)
     
-    def __delete__(self):
-        self._shutdown()
-        return
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        self.toggleClamp(False)
+        return super().shutdown()
     
-    def _connect(self, port:str, baudrate=115200, timeout=1):
+    def toggleClamp(self, on:bool = False) -> str:
         """
-        Connect to machine control unit
+        Close or open the clamp
 
         Args:
-            port (str): com port address
-            baudrate (int): baudrate. Defaults to 115200.
-            timeout (int, optional): timeout in seconds. Defaults to None.
+            on (bool, optional): whether to clamp down on sample. Defaults to False.
             
         Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
+            str: response string
         """
-        self.port = port
-        self._baudrate = baudrate
-        self._timeout = timeout
-        instrument = None
+        option = -1 if on else 1
+        return self._query(f'CLAMP,{option}')
+
+    # Protected method(s)
+    def _connect(self, port:str, baudrate:int = 115200, timeout:int = 1):
+        """
+        Connection procedure for tool
+
+        Args:
+            port (str): COM port address
+            baudrate (int): baudrate. Defaults to 115200.
+            timeout (int, optional): timeout in seconds. Defaults to None.
+        """
+        self.connection_details = {
+            'port': port,
+            'baudrate': baudrate,
+            'timeout': timeout
+        }
+        device = None
         try:
-            instrument = serial.Serial(port, self._baudrate, timeout=self._timeout)
-            self.instrument = instrument
-            print(f"Connection opened to {port}")
-            self.setFlag('connected', True)
-            
+            device = serial.Serial(port, baudrate, timeout=timeout)
         except Exception as e:
+            print(f"Could not connect to {port}")
             if self.verbose:
-                print(f"Could not connect to {port}")
-        return self.instrument
+                print(e)
+        else:
+            print(f"Connection opened to {port}")
+            self.setFlag(connected=True)
+        self.device = device
+        return
     
-    def _query(self, string:str, timeout_s=TIMEOUT_S):
+    def _query(self, command:str, timeout_s:int = 60) -> Union[str, tuple[str]]:
         """
-        Send query and wait for reponse
+        Write command to and read response from device
 
         Args:
-            string (str): message string
-            timeout_s (int, optional): duration to wait before timeout. If None, no timeout duration. Defaults to TIMEOUT_S.
+            command (str): command string
+            timeout_s (float, optional): duration to wait before timeout. Defaults to 60.
 
-        Yields:
-            str: response string
+        Returns:
+            Union[str, tuple[str]]: response string, or list of response strings
         """
+        command_code = command.split(',')[0].strip().upper()
+        if command_code not in CommandCode._member_names_:
+            raise Exception(f"Please select a valid command code from: {', '.join(CommandCode._member_names_)}")
+        
         start_time = time.time()
-        message_code = self._write(string)
+        self._write(command)
         cache = []
         response = ''
         while response != 'OKC':
             if timeout_s is not None and (time.time()-start_time) > timeout_s:
                 print('Timeout! Aborting run...')
                 break
             response = self._read()
-            if message_code == 'GET' and len(response):
+            if command_code == 'GET' and len(response):
                 cache.append(response)
-
-        self.setFlag('busy', False)
+        self.setFlag(busy=False)
         time.sleep(0.1)
-        if message_code == 'GET':
-            return cache
+        if command_code == 'GET':
+            return tuple(cache)
         return response
     
-    def _read(self):
+    @staticmethod
+    def _range_finder(frequency_1:float, frequency_2:float) -> Frequency:
         """
-        Read response from instrument
+        Find the appropriate the operating frequency range
+
+        Args:
+            frequency_1 (float): lower frequency limit
+            frequency_2 (float): upper frequency limit
+            
+        Returns:
+            Frequency: optimal frequency range that covers desired values
+        """
+        frequencies = np.array(FREQUENCIES)
+        low_frequency, high_frequency = sorted((frequency_1, frequency_2))
+        lower = frequencies[frequencies < low_frequency]
+        higher = frequencies[frequencies > high_frequency]
+        low = lower[-1] if len(lower) else frequencies[0]
+        high = higher[0] if len(higher) else frequencies[-1]
+        return Frequency(low, high)
+    
+    def _read(self) -> str:
+        """
+        Read response from device
 
         Returns:
             str: response string
         """
         response = ''
         try:
-            response = self.instrument.readline()
+            response = self.device.readline()
             response = response.decode("utf-8").strip()
+        except AttributeError:
+            pass
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        else:
             if len(response) and (self.verbose or 'High-Voltage' in response):
                 print(response)
-            if response in ERRORS:
+            if response in ErrorCode._member_names_:
                 print(ErrorCode[response].value)
-        except Exception as e:
-            if self.verbose:
-                pass
         return response
     
-    def _shutdown(self):
-        """
-        Close serial connection and shutdown
-        """
-        self.toggleClamp(False)
-        self.reset()
-        self.instrument.close()
-        return
-
-    def _write(self, string:str):
+    def _write(self, command:str) -> bool:
         """
-        Sends message to instrument
+        Write command to device
 
         Args:
-            string (str): <message code>,<option 1>[,<option 2>]
-
-        Raises:
-            Exception: Select a valid command code.
+            command (str): <command code>,<option 1>[,<option 2>]
         
         Returns:
-            str: two-character message code
+            bool: whether command was sent successfully
         """
-        message_code = string.split(',')[0].strip().upper()
-        if message_code not in COMMANDS:
-            raise Exception(f"Please select a valid command code from: {', '.join(COMMANDS)}")
-        fstring = f'DMA,SN{self.channel},{string},END' # message template: <PRE>,<SN>,<CODE>,<OPTIONS>,<POST>
-        bstring = bytearray.fromhex(fstring.encode('utf-8').hex())
+        if self.verbose:
+            print(command)
+        fstring = f'DMA,SN{self.channel},{command},END' # command template: <PRE>,<SN>,<CODE>,<OPTIONS>,<POST>
+        # bstring = bytearray.fromhex(fstring.encode('utf-8').hex())
         try:
-            self.instrument.write(bstring)
-            self.setFlag('busy', True)
+            self.device.write(fstring.encode('utf-8'))
+        except AttributeError:
+            pass
         except Exception as e:
-            print(e)
-        if self.verbose:
-            print(fstring)
-        return message_code
-    
-    def close(self):
-        """
-        Alias for _shutdown method
-        """
-        return self._shutdown()
-    
-    def connect(self):
-        """
-        Reconnect to instrument using existing port and baudrate
-        
-        Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
-        """
-        return self._connect(self.port, self._baudrate, self._timeout)
-    
-    def initialise(self, low_frequency, high_frequency): # TODO: check frequencies if same as previous
-        if self._flags['initialised']:
-            return
-        if self.range_finder((low_frequency, high_frequency)) == self.frequency_codes:
-            print('Appropriate frequency range remains the same!')
-        else:
-            if any(self.frequency_codes):
-                self.reset()
-            self.frequency_range = low_frequency, high_frequency
-            input("Ensure no samples within the clamp area during initialization. Press 'Enter' to proceed.")
-            self._query(f"INIT,{','.join([str(_f) for _f in self.frequency_codes])}")
-        self.setFlag('initialised', True)
-        print(self.frequency_range)
-        return
-    
-    def isBusy(self):
-        """
-        Checks whether the instrument is busy
-        
-        Returns:
-            bool: whether the instrument is busy
-        """
-        return self._flags['busy']
-    
-    def isConnected(self):
-        """
-        Check whether instrument is connected
-
-        Returns:
-            bool: whether instrument is connected
-        """
-        return self._flags['connected']
-
-    def readAll(self, **kwargs):
-        """
-        Read all data on buffer
-
-        Args:
-            fields (list, optional): fields of interest. Defaults to [].
-            
-        Returns:
-            pd.DataFrame: dataframe of measurements
-        """
-        data = [line.split(', ') for line in self._query('GET,0') if ',' in line]
-        df = pd.DataFrame(data[1:], columns=data[0], dtype=float)
-        return df
-    
-    def reset(self):
-        """
-        Clear settings from instrument. Reset the program, data, and flags
-        """
-        self._query('CLR,0')
-        self._frequency_range_codes = ('0','0')
-        self._flags = {
-            'busy': False,
-            'connected': False,
-            'initialised': False,
-            'measured': False,
-            'read': False
-        }
-        return
-        
-    def setFlag(self, name:str, value:bool):
-        """
-        Set a flag truth value
-
-        Args:
-            name (str): label
-            value (bool): flag value
-        """
-        self._flags[name] = value
-        return
-    
-    def start(self, sample_thickness=1E-6):
-        """
-        Initialise the measurement
-        """
-        if not self._flags['initialised']:
-            print("Please initialise the instrument using the 'initialise' method first")
-            return
-        self._query(f"RUN,{sample_thickness}")
-        return
-    
-    def stopClamp(self):
-        """
-        Stop clamp movement
-        """
-        # self._query('CLAMP,0')
-        print('Stop clamp function not available.')
-        return
-    
-    def toggleClamp(self, on=False):
-        """
-        Toggle between clamp and release state
-
-        Args:
-            on (bool, optional): whether to clamp down on sample. Defaults to False.
-        """
-        option = -1 if on else 1
-        self._query(f'CLAMP,{option}')
-        return
+            if self.verbose:
+                print(e)
+            return False
+        self.setFlag(busy=True)
+        return True
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.0.0a0/src/controllably/Measure/program_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,146 +1,141 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2023/01/05 17:13:35
-@author: Chang Jie
+This module holds the base class for measurement programs.
 
-Notes / actionables:
--
+Classes:
+    Program (ABC)
+    ProgramDetails (dataclass)
+
+Functions:
+    get_program_details
 """
 # Standard library imports
-from datetime import datetime
+from __future__ import annotations
+from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
+import inspect
 import pandas as pd
-import time
-
-# Local application imports
-from ..piezorobotics_device import PiezoRoboticsDevice
-from ..piezorobotics_lib import FREQUENCIES
+from typing import Callable, Optional, Protocol, Any
 print(f"Import: OK <{__name__}>")
 
-class Program(object):
+class Device(Protocol):
+    ...
+
+@dataclass
+class ProgramDetails:
+    """
+    ProgramDetails dataclass represents the set of inputs, default values, truncated docstring and tooltip of a program class
+    
+    ### Constructor
+    Args:
+        `inputs` (list[str]): list of input field names
+        `defaults` (dict[str, Any]): dictionary of kwargs and default values
+        `short_doc` (str): truncated docstring of the program
+        `tooltip` (str): descriptions of input fields
+    """
+    
+    inputs: list[str] = field(default_factory=lambda: [])
+    defaults: dict[str, Any] = field(default_factory=lambda: {})
+    short_doc: str = ''
+    tooltip: str = ''
+
+
+class Program(ABC):
     """
     Base Program template
 
+    ### Constructor
     Args:
-        device (PiezoRoboticsDevice): PiezoRobotics Device object
-        parameters (dict, optional): dictionary of measurement parameters. Defaults to {}.
+        `device` (Device): device object
+        `parameters` (Optional[dict], optional): dictionary of kwargs. Defaults to None.
+        `verbose` (bool, optional): verbosity of class. Defaults to False.
+
+    ### Attributes
+    - `data_df` (pd.DataFrame): data collected from device when running the program
+    - `device` (Device): device object
+    - `parameters` (dict[str, ...]): parameters
+    - `verbose` (bool): verbosity of class
+    
+    ### Methods
+    #### Abstract
+    - `run`: run the measurement program
     
     ==========
-    Parameters:
+    
+    ### Parameters:
         None
     """
-    details = {
-        'inputs_and_defaults': {},
-        'short_doc': '',
-        'tooltip': ''
-    }
-    def __init__(self, device:PiezoRoboticsDevice, parameters={}, **kwargs):
-        self.device = device
-        self.parameters = parameters
-        
-        self.data_df = pd.DataFrame
-        self._flags = {}
-        return
     
-    @classmethod
-    def getDetails(cls, verbose=False):
+    details: ProgramDetails = ProgramDetails()
+    def __init__(self, 
+        device: Device, 
+        parameters: Optional[dict] = None,
+        verbose: bool = False, 
+        **kwargs
+    ):
         """
-        Get the input fields and defaults
-        
-        Args:
-            verbose: whether to print out truncated docstring. Defaults to False.
+        Instantiate the class
 
-        Returns:
-            dict: dictionary of program details
-        """
-        doc = cls.__doc__
-        
-        # Extract truncated docstring and parameter listing
-        lines = doc.split('\n')
-        start, end = 0,0
-        for i,line in enumerate(lines):
-            line = line.strip()
-            if line.startswith('Args:'):
-                start = i
-            if line.startswith('==========') and start:
-                end = i
-                break
-        parameter_list = sorted([_l.strip() for _l in lines[end+2:] if len(_l.strip())])
-        short_lines = lines[:start-1] + lines[end:]
-        short_doc = '\n'.join(short_lines)
-        tooltip = '\n'.join(['Parameters:'] + [f'- {_p}' for _p in parameter_list])
-        if verbose:
-            print(short_doc)
-        
-        # Extract input fields and defaults
-        input_parameters = {}
-        for parameter in parameter_list:
-            if len(parameter) == 0:
-                continue
-            _input = parameter.split(' ')[0]
-            _default = parameter.split(' ')[-1][:-1] if 'Defaults' in parameter else ''
-            input_parameters[_input] = _default
-        
-        cls.details = {
-            'inputs_and_defaults': input_parameters,
-            'short_doc': short_doc,
-            'tooltip': tooltip
-        }
-        return cls.details
-    
-    def run(self):
-        """
-        Run the measurement program
+        Args:
+            device (Device): device object
+            parameters (Optional[dict], optional): dictionary of kwargs. Defaults to None.
+            verbose (bool, optional): verbosity of class. Defaults to False.
         """
+        self.device = device
+        self.data_df = pd.DataFrame()
+        self.parameters = parameters
+        self.verbose = verbose
         return
     
-class DMA(Program):
-    """
-    Dynamic Mechanical Analysis
+    @abstractmethod
+    def run(self, *args, **kwargs):
+        """Run the measurement program"""
 
-    Args:
-        device (PiezoRoboticsDevice): PiezoRobotics Device object
-        parameters (dict, optional): dictionary of measurement parameters. Defaults to {}.
-    
-    ==========
-    Parameters:
-        low_frequency (float): lower frequency limit to test
-        high_frequency (float): upper frequency limit to test
-        sample_thickness (float): thickness of measured sample
+
+def get_program_details(program_class: Callable, verbose:bool = False) -> ProgramDetails:
     """
-    def __init__(self, device:PiezoRoboticsDevice, parameters={}, **kwargs):
-        super().__init__(device, parameters, **kwargs)
-        return
+    Get the input fields and defaults
     
-    def run(self):
-        """
-        Run the measurement program
-        """
-        device = self.device
-        repeat = self.parameters.get('repeat', 1)
-        device.toggleClamp(False)
-        device.initialise(
-            low_frequency=self.parameters.get('low_frequency', FREQUENCIES[0]), 
-            high_frequency=self.parameters.get('high_frequency', FREQUENCIES[-1])
-        )
-        
-        input("Please load sample. Press 'Enter' to proceed")
-        device.toggleClamp(True)
-        for i in range(repeat):
-            print(f"Start run {i+1} at {datetime.now()}")
-            device.start(sample_thickness=self.parameters.get('sample_thickness', 1E-3))
-            print(f"End run {i+1} at {datetime.now()}")
-            time.sleep(1)
-            df = device.readAll()
-            df['run'] = i+1
-            if i == 0:
-                self.data_df = df
-            else:
-                self.data_df = pd.concat([self.data_df, df], ignore_index=True)
-        device.toggleClamp(False)
-        return
-
+    Args:
+        program_class (Callable): program class of interest
+        verbose: whether to print out truncated docstring. Defaults to False.
 
-PROGRAMS = [DMA]
-PROGRAM_NAMES = [prog.__name__ for prog in PROGRAMS]
-INPUTS = [item for item in [[key for key in prog.getDetails().get('inputs_and_defaults', {})] for prog in PROGRAMS]]
-INPUTS_SET = sorted( list(set([item for sublist in INPUTS for item in sublist])) )
+    Returns:
+        ProgramDetails: details of program class
+    """
+    doc = inspect.getdoc(program_class)
+    
+    # Extract truncated docstring and parameter listing
+    lines = doc.split('\n')
+    start, end = 0,0
+    for i,line in enumerate(lines):
+        # line = line.strip()
+        if line.startswith('### Constructor'):
+            start = i
+        if line.startswith('===') and start:
+            end = i
+            break
+    short_lines = [''] + lines[:start-1] + lines[end:]
+    short_doc = '\n'.join(short_lines).replace("### ", "")
+    parameter_list = [l.strip() for l in lines[end+3:] if len(l.strip())]
+    tooltip = '\n'.join(['Parameters:'] + [f'- {p}' for p in parameter_list])
+    
+    # Extract input fields and defaults
+    inputs = []
+    defaults = {}
+    for parameter in parameter_list:
+        if len(parameter) == 0:
+            continue
+        inputs.append(parameter.split(' ')[0])
+        if 'Defaults' in parameter:
+            defaults[inputs[-1]] = parameter.split(' ')[-1][:-1]
+
+    details = ProgramDetails(
+        inputs=inputs,
+        defaults=defaults,
+        short_doc=short_doc,
+        tooltip=tooltip
+    )
+    if verbose:
+        print(short_doc)
+    return details
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,247 +1,323 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
+This module holds the class for spin-coaters.
 
-Notes / actionables:
--
+Classes:
+    Spinner (Maker)
+    SpinnerAssembly (Maker)
 """
 # Standard library imports
+from __future__ import annotations
 import numpy as np
+from threading import Thread
 import time
 
 # Third party imports
-import serial # pip install pyserial
+import serial   # pip install pyserial
 
 # Local application imports
-from ...misc import HELPER
-from ..mover_utils import Mover
+from ...misc import Helper
+from ..make_utils import Maker
 print(f"Import: OK <{__name__}>")
 
-MAX_SPEED = 250 # [mm/s]
-    
-class Gantry(Mover):
+class Spinner(Maker):
     """
-    Gantry robot controls
-
+    Spinner provides methods to control a single spin coater controller unit
+    
+    ### Constructor
     Args:
-        port (str): com port address
-        limits (list, optional): lower and upper bounds of movement. Defaults to [(0,0,0), (0,0,0)].
-        safe_height (float, optional): safe height. Defaults to None.
-        max_speed (float, optional): maximum movement speed. Defaults to 250.
-    
-    Kwargs:
-        home_coordinates (tuple, optional): position to home in arm coordinates. Defaults to (0,0,0).
-        home_orientation (tuple, optional): orientation to home. Defaults to (0,0,0).
-        orientate_matrix (numpy.matrix, optional): matrix to transform arm axes to workspace axes. Defaults to np.identity(3).
-        translate_vector (numpy.ndarray, optional): vector to transform arm position to workspace position. Defaults to (0,0,0).
-        implement_offset (tuple, optional): implement offset vector pointing from end of effector to tool tip. Defaults to (0,0,0).
-        scale (int, optional): scale factor to transform arm scale to workspace scale. Defaults to 1.
-        verbose (bool, optional): whether to print outputs. Defaults to False.
+        `port` (str): COM port address
+        `channel` (int, optional): channel id. Defaults to 0.
+        `position` (tuple[float], optional): x,y,z position of spinner. Defaults to (0,0,0).
+
+    ### Attributes
+    - `channel` (int): channel id
+    - `speed` (int): spin speed in rpm
+    
+    ### Properties
+    - `port` (str): COM port address
+    - `position` (np.ndarray): x,y,z position of spinner
+    
+    ### Methods
+    - `run`: executes the soak and spin steps
+    - `shutdown`: shutdown procedure for tool
+    - `soak`: executes a soak step
+    - `spin`: execute a spin step
     """
-    def __init__(self, port:str, limits=[(0, 0, 0), (0, 0, 0)], safe_height=None, max_speed=MAX_SPEED, **kwargs):
+    
+    _default_flags = {
+        'busy': False,
+        'connected': False
+    }
+    
+    def __init__(self, 
+        port: str, 
+        channel: int = 0, 
+        position: tuple[float] = (0,0,0), 
+        **kwargs
+    ):
+        """
+        Instantiate the class
+
+        Args:
+            port (str): COM port address
+            channel (int, optional): channel id. Defaults to 0.
+            position (tuple[float], optional): x,y,z position of spinner. Defaults to (0,0,0).
+        """
         super().__init__(**kwargs)
-        self._limits = [(0, 0, 0), (0, 0, 0)]
-        
-        self.device = None
-        self.limits = limits
-        self._speed = max_speed
-        
-        self.port = ''
-        self._baudrate = None
-        self._timeout = None
-        
-        if safe_height is not None:
-            self.setHeight('safe', safe_height)
+        self.channel = channel
+        self._position = tuple(position)
+        self.speed = 0
         self._connect(port)
-        self.home()
         return
     
+    # Properties
+    @property
+    def port(self) -> str:
+        return self.connection_details.get('port', '')
+    
     @property
-    def limits(self):
-        return np.array(self._limits)
-    @limits.setter
-    def limits(self, value:list):
-        if len(value) != 2 or any([len(row)!=3 for row in value]):
-            raise Exception('Please input a list of [lower_xyz_limit, upper_xyz_limit]')
-        self._limits = ( tuple(value[0]), tuple(value[1]) )
+    def position(self) -> np.ndarray:
+        return np.array(self._position)
+    
+    def run(self, soak_time:int = 0, spin_speed:int = 2000, spin_time:int = 1, **kwargs):
+        """
+        Execute the soak and spin steps
+
+        Args:
+            soak_time (int, optional): soak time. Defaults to 0.
+            spin_speed (int, optional): spin speed. Defaults to 2000.
+            spin_time (int, optional): spin time. Defaults to 1.
+        """
+        self.setFlag(busy=True)
+        self.soak(soak_time)
+        self.spin(spin_speed, spin_time)
+        self.setFlag(busy=False)
         return
     
-    def _connect(self, port:str, baudrate:int, timeout=None):
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        return super().shutdown()
+
+    def soak(self, time_s:int, **kwargs):
         """
-        Connect to machine control unit
+        Executes a soak step
 
         Args:
-            port (str): com port address
-            baudrate (int): baudrate
-            timeout (int, optional): timeout in seconds. Defaults to None.
-            
-        Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
+            time_s (int): soak time in seconds
+        """
+        self.speed = 0
+        print(f"Soaking    (channel {self.channel}): {time_s}s")
+        if time_s:
+            time.sleep(time_s)
+        return
+
+    def spin(self, speed:int, time_s:int, **kwargs):
+        """
+        Executes a spin step
+
+        Args:
+            speed (int): spin speed in rpm
+            time_s (int): spin time in seconds
+        """
+        self._write(speed)
+        self.speed = speed
+        print(f"Duration   (channel {self.channel}): {time_s}s")
+        interval = 1
+        start_time = time.time()
+        while(True):
+            time.sleep(0.1)
+            if (interval <= time.time() - start_time):
+                interval += 1
+            if (time_s <= time.time() - start_time):
+                break
+        self._write(0)
+        self.speed = 0
+        return
+
+    # Protected method(s)
+    def _connect(self, port:str, baudrate:int = 9600, timeout:int = 1):
         """
-        self.port = port
-        self._baudrate = baudrate
-        self._timeout = timeout
+        Connection procedure for tool
+
+        Args:
+            port (str): COM port address
+            baudrate (int, optional): baudrate. Defaults to 9600.
+            timeout (int, optional): timeout in seconds. Defaults to 1.
+        """
+        self.connection_details = {
+            'port': port,
+            'baudrate': baudrate,
+            'timeout': timeout
+        }
         device = None
         try:
             device = serial.Serial(port, baudrate, timeout=timeout)
-            print(f"Connection opened to {port}")
         except Exception as e:
+            print(f"Could not connect to {port}")
             if self.verbose:
-                print(f"Could not connect to {port}")
                 print(e)
+        else:
+            time.sleep(2)   # Wait for grbl to initialize
+            device.flushInput()
+            print(f"Connection opened to {port}")
+            self.setFlag(connected=True)
         self.device = device
-        return self.device
+        return
+    
+    def _diagnostic(self):
+        """Run diagnostic test"""
+        thread = Thread(target=self.run, name=f'maker_diag_{self.channel}')
+        thread.start()
+        time.sleep(1)
+        return
     
-    def _shutdown(self):
+    def _write(self, speed:int):
         """
-        Close serial connection and shutdown
+        Relay spin speed to spinner
+
+        Args:
+            speed (int): spin speed in rpm
         """
-        self.home()
-        self.disconnect()
+        try:
+            self.device.write(bytes(f"{speed}\n", 'utf-8'))
+        except AttributeError:
+            pass
+        print(f"Spin speed (channel {self.channel}): {speed}")
         return
 
-    def connect(self):
-        """
-        Reconnect to robot using existing port and baudrate
-        
-        Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
-        """
-        return self._connect(self.port, self._baudrate, self._timeout)
+
+class SpinnerAssembly(Maker):
+    """
+    SpinnerAssembly provides methods to control multiple spin coater controller units
     
-    def disconnect(self):
+    ### Constructor
+    Args:
+        `ports` (list[str]): COM port addresses
+        `channels` (list[int]): channel ids
+        `positions` (list[tuple[float]]): x,y,z positions of spinners
+
+    ### Attributes
+    - `channels` (dict[int, Spinner]): dictionary of {channel id, `Spinner` objects}
+    
+    ### Methods
+    - `disconnect`: disconnect from device
+    - `isBusy`: checks and returns whether any of the spinners are still busy
+    - `isConnected`: checks and returns whether all spinners are connected
+    - `run`: executes the soak and spin steps
+    - `shutdown`: shutdown procedure for tool
+    - `soak`: executes a soak step
+    - `spin`: execute a spin step
+    """
+    
+    _default_flags = {
+        'busy': False,
+        'connected': False
+    }
+    
+    def __init__(self, 
+        ports:list[str], 
+        channels:list[int], 
+        positions:list[tuple[float]], 
+        **kwargs
+    ):
         """
-        Disconnect serial connection to robot
-        
-        Returns:
-            None: None is successfully disconnected, else serial.Serial
+        Instantiate the class
+
+        Args:
+            ports (list[str]): COM port addresses
+            channels (list[int]): channel ids
+            positions (list[tuple[float]]): x,y,z positions of spinners
         """
-        try:
-            self.device.close()
-        except Exception as e:
-            if self.verbose:
-                print(e)
-        self.device = None
-        return self.device
+        super().__init__(**kwargs)
+        self.channels = {}
+        self._threads = {}
+        
+        self._connect(port=ports, channel=channels, position=positions)
+        return
 
-    def isConnected(self):
+    def disconnect(self):
+        """Disconnect from device"""
+        for channel in self.channels.values():
+            channel.disconnect()
+        return super().disconnect() 
+        
+    def isBusy(self) -> bool:
         """
-        Check whether machine control unit is connected
+        Checks and returns whether any of the spinners are still busy
 
         Returns:
-            bool: whether machine control unit is connected
+            bool: whether any of the spinners are still busy
         """
-        if self.device is None:
-            print(f"{self.__class__} ({self.port}) not connected.")
-            return False
-        return True
+        return any([channel.isBusy() for channel in self.channels.values()])
     
-    def isFeasible(self, coordinates, transform=False, tool_offset=False, **kwargs):
+    def isConnected(self) -> bool:
         """
-        Checks if specified coordinates is a feasible position for robot to access
-
-        Args:
-            coordinates (tuple): x,y,z coordinates
-            transform (bool, optional): whether to transform the coordinates. Defaults to False.
-            tool_offset (bool, optional): whether to consider tooltip offset. Defaults to False.
+        Checks and returns whether all spinners are connected
 
         Returns:
-            bool: whether coordinates is a feasible position
+            bool: whether all spinners are connected
         """
-        if transform:
-            coordinates = self._transform_in(coordinates=coordinates, tool_offset=tool_offset)
-        coordinates = np.array(coordinates)
-        l_bound, u_bound = self.limits
-        
-        if all(np.greater_equal(coordinates, l_bound)) and all(np.less_equal(coordinates, u_bound)):
-            if self.deck.is_excluded(coordinates=self._transform_out(coordinates, tool_offset=True)):
-                return False
-            return True
-        print(f"Range limits reached! {self.limits}")
-        return False
-
-    def moveBy(self, vector, to_safe_height=False, **kwargs):
+        return all([channel.isConnected() for channel in self.channels.values()])
+    
+    def run(self, soak_time:int, spin_speed:int, spin_time:int, channel:int):
         """
-        Move robot by specified vector
+        Execute the soak and spin steps
 
         Args:
-            vector (tuple): x,y,z vector to move in
-            to_safe_height (bool, optional): whether to return to safe height first. Defaults to False.
-
-        Returns:
-            bool: whether movement is successful
-        """
-        return super().moveBy(vector=vector, to_safe_height=to_safe_height)
+            soak_time (int): soak time
+            spin_speed (int): spin speed
+            spin_time (int): spin time
+            channel (int): channel id
+        """
+        thread = Thread(target=self.channels[channel].run, args=(soak_time, spin_speed, spin_time))
+        thread.start()
+        self._threads[f'channel_{channel}_run'] = thread
+        return
+    
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        for thread in self._threads.values():
+            thread.join()
+        return super().shutdown()
     
-    @HELPER.safety_measures
-    def moveTo(self, coordinates, to_safe_height=True, jump_height=None, tool_offset=True, **kwargs):
+    def soak(self, seconds:int, channel:int):
         """
-        Move robot to specified coordinates and orientation
+        Executes a soak step
 
         Args:
-            coordinates (tuple): x,y,z coordinates to move to. Defaults to None.
-            to_safe_height (bool, optional): whether to return to safe height first. Defaults to True.
-            jump_height (int, or float): height value to jump to. Defaults to None.
-            tool_offset (bool, optional): whether to consider tooltip offset. Defaults to True.
-            
-        Returns:
-            bool: whether movement is successful
+            time_s (int): soak time in seconds
+            channel (int): channel id
         """
-        coordinates = self._transform_in(coordinates=coordinates, tool_offset=tool_offset)
-        coordinates = np.array(coordinates)
-        if not self.isFeasible(coordinates):
-            return
-        
-        # Retreat to safe height first
-        if jump_height is None:
-            jump_height = self.heights['safe']
-        if to_safe_height and self.coordinates[2] < jump_height:
-            try:
-                self.device.write(bytes("G90\n", 'utf-8'))
-                print(self.device.readline())
-                self.device.write(bytes(f"G0 Z{jump_height}\n", 'utf-8'))
-                print(self.device.readline())
-                self.device.write(bytes("G90\n", 'utf-8'))
-                print(self.device.readline())
-            except Exception as e:
-                if self.verbose:
-                    print(e)
-            self.coordinates = (*self.coordinates[0:2], jump_height)
-        
-        z_first = True if self.coordinates[2]<coordinates[2] else False
-        positionXY = f'X{coordinates[0]}Y{coordinates[1]}'
-        position_Z = f'Z{coordinates[2]}'
-        moves = [position_Z, positionXY] if z_first else [positionXY, position_Z]
-        try:
-            self.device.write(bytes("G90\n", 'utf-8'))
-            print(self.device.readline())
-            for move in moves:
-                self.device.write(bytes(f"G0 {move}\n", 'utf-8'))
-                print(self.device.readline())
-            self.device.write(bytes("G90\n", 'utf-8'))
-            print(self.device.readline())
-        except Exception as e:
-            if self.verbose:
-                print(e)
-        distances = abs(self.coordinates - coordinates)
-        times = distances / self.speed
-        move_time = max(times[:2]) + times[2]
-        time.sleep(move_time)
-        self.updatePosition(coordinates=coordinates)
+        thread = Thread(target=self.channels[channel].soak, args=(seconds,))
+        thread.start()
+        self._threads[f'channel_{channel}_soak'] = thread
         return
     
-    def safeMoveTo(self, coordinates, jump_height=None, tool_offset=True, **kwargs):
+    def spin(self, speed:int, seconds:int, channel:int):
         """
-        Safe version of moveTo
+        Executes a spin step
 
         Args:
-            coordinates (tuple): x,y,z coordinates to move to. Defaults to None.
-            jump_height (int, or float): height value to jump to. Defaults to None.
-            tool_offset (bool, optional): whether to consider tooltip offset. Defaults to True.
-            
-        Returns:
-            bool: whether movement is successful
-        """
-        return self.moveTo(coordinates, to_safe_height=True, jump_height=jump_height, tool_offset=tool_offset, **kwargs)
+            speed (int): spin speed in rpm
+            time_s (int): spin time in seconds
+            channel (int): channel id
+        """
+        thread = Thread(target=self.channels[channel].spin, args=(speed, seconds))
+        thread.start()
+        self._threads[f'channel_{channel}_spin'] = thread
+        return
+
+    # Protected method(s)
+    def _connect(self, **kwargs):
+        """Connection procedure for tool"""
+        properties = Helper.zip_inputs('channel', **kwargs)
+        self.channels = {key: Spinner(**value) for key,value in properties.items()}
+        return
+    
+    def _diagnostic(self):
+        """Run diagnostic test"""
+        for channel in self.channels.values():
+            channel._diagnostic()
+        return
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Control/GUI/viewer_panel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,120 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
+This module holds the class for viewer control panels.
 
-Notes / actionables:
--
+Classes:
+    ViewerPanel (Panel)
 """
+# Standard library imports
+from __future__ import annotations
+import time
+from typing import Protocol
+
+# Third party imports
+import PySimpleGUI as sg # pip install PySimpleGUI
+
 # Local application imports
-from ...misc import HELPER
-from .cartesian_utils import Gantry
+from .gui_utils import Panel
 print(f"Import: OK <{__name__}>")
 
-class Ender(Gantry):
-    """
-    Ender platform controls
+class Viewer(Protocol):
+    def getImage(self, *args, **kwargs):
+        ...
+    def shutdown(self, *args, **kwargs):
+        ...
 
+class ViewerPanel(Panel):
+    """
+    ViewerPanel provides methods to create a control panel for a viewer
+    
+    ### Constructor
     Args:
-        port (str): com port address
-        limits (list, optional): lower and upper bounds of movement. Defaults to [(0,0,0), (0,0,0)].
-        safe_height (float, optional): safe height. Defaults to None.
-    
-    Kwargs:
-        max_speed (float, optional): maximum movement speed. Defaults to 250.
-        home_coordinates (tuple, optional): position to home in arm coordinates. Defaults to (0,0,0).
-        home_orientation (tuple, optional): orientation to home. Defaults to (0,0,0).
-        orientate_matrix (numpy.matrix, optional): matrix to transform arm axes to workspace axes. Defaults to np.identity(3).
-        translate_vector (numpy.ndarray, optional): vector to transform arm position to workspace position. Defaults to (0,0,0).
-        implement_offset (tuple, optional): implement offset vector pointing from end of effector to tool tip. Defaults to (0,0,0).
-        scale (int, optional): scale factor to transform arm scale to workspace scale. Defaults to 1.
-        verbose (bool, optional): whether to print outputs. Defaults to False.
+        `viewer` (Viewer): Viewer object
+        `name` (str, optional): name of panel. Defaults to 'VIEW'.
+        `group` (str, optional): name of group. Defaults to 'viewer'.
+
+    ### Attributes
+    - `display_box` (str): element id
+    
+    ### Properties
+    - `viewer` (Viewer): alias for `tool`
+    
+    ### Methods
+    - `close`: exit the application
+    - `getLayout`: build `sg.Column` object
+    - `listenEvents`: listen to events and act on values
     """
-    def __init__(self, port:str, limits=[(0,0,0), (240,235,210)], safe_height=30, **kwargs):
-        super().__init__(port=port, limits=limits, safe_height=safe_height, **kwargs)
+    
+    def __init__(self, 
+        viewer: Viewer, 
+        name: str = 'VIEW', 
+        group: str = 'viewer', 
+        **kwargs
+    ):
+        """
+        Instantiate the class
+
+        Args:
+            viewer (Viewer): viewer object
+            name (str, optional): name of panel. Defaults to 'VIEW'.
+            group (str, optional): name of group. Defaults to 'viewer'.
+        """
+        super().__init__(name=name, group=group, **kwargs)
+        self.tool = viewer
+        
+        self.display_box = self._mangle('-IMAGE-')
+        self._last_read_time = time.time()
+        
+        self.setFlag(update_display=True)
         return
     
-    def _connect(self, port:str, baudrate=115200, timeout=None):
+    # Properties
+    @property
+    def viewer(self) -> Viewer:
+        return self.tool
+    
+    def close(self):
+        """Exit the application"""
+        self.viewer.shutdown()
+        return super().close()
+        
+    def getLayout(self, title_font_level:int = 1, **kwargs) -> sg.Column:
         """
-        Connect to machine control unit
+        Build `sg.Column` object
 
         Args:
-            port (str): com port address
-            baudrate (int): baudrate. Defaults to 115200.
-            timeout (int, optional): timeout in seconds. Defaults to None.
-            
+            title_font_level (int, optional): index of font size from levels in `font_sizes`. Defaults to 1.
+
         Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
+            sg.Column: Column object
         """
-        self.port = port
-        self._baudrate = baudrate
-        self._timeout = timeout
-        return super()._connect(self.port, self._baudrate, self._timeout)
-
-    def heat(self, bed_temperature):
+        font = (self.typeface, self.font_sizes[title_font_level])
+        layout = super().getLayout(f'{self.name} Control', justification='center', font=font)
+        layout = [
+            [layout],
+            [sg.Image(filename='', key=self.display_box, enable_events=True)]
+        ]
+        layout = sg.Column(layout, vertical_alignment='top')
+        return layout
+    
+    def listenEvents(self, event:str, values:dict[str, str]) -> dict[str, dict]:
         """
-        Heat bed to temperature
+        Listen to events and act on values
 
         Args:
-            bed_temperature (int, or float): temperature of platform
+            event (str): event triggered
+            values (dict[str, str]): dictionary of values from window
 
         Returns:
-            bool: whether setting bed temperature was successful
+            dict: dictionary of updates
         """
-        bed_temperature = round( min(max(bed_temperature,0), 110) )
-        try:
-            self.device.write(bytes(f'M140 S{bed_temperature}\n', 'utf-8'))
-        except Exception as e:
-            print('Unable to heat stage!')
-            if self.verbose:
-                print(e)
-            return False
-        return True
-
-    @HELPER.safety_measures
-    def home(self):
-        """
-        Homing cycle for Ender platform
-        """
-        try:
-            self.device.write(bytes("G90\n", 'utf-8'))
-            print(self.device.readline())
-            self.device.write(bytes(f"G0 Z{self.heights['safe']}\n", 'utf-8'))
-            print(self.device.readline())
-            self.device.write(bytes("G90\n", 'utf-8'))
-            print(self.device.readline())
-
-            self.device.write(bytes("G28\n", 'utf-8'))
-
-            self.device.write(bytes("G90\n", 'utf-8'))
-            print(self.device.readline())
-            self.device.write(bytes(f"G0 Z{self.heights['safe']}\n", 'utf-8'))
-            print(self.device.readline())
-            self.device.write(bytes("G90\n", 'utf-8'))
-            print(self.device.readline())
-        except Exception as e:
-            if self.verbose:
-                print(e)
-        
-        self.coordinates = (0,0,self.heights['safe'])
-        try:
-            self.device.write(bytes("G1 F10000\n", 'utf-8'))
-            print(self.device.readline())
-        except Exception as e:
-            if self.verbose:
-                print(e)
-        return
+        updates = {}
+        if self.flags['update_display']:
+            frame_interval = time.time() - self._last_read_time
+            fps = round(1/frame_interval, 2)
+            ret, image = self.viewer.getImage()
+            self._last_read_time = time.time()
+            if ret:
+                image = image.addText(f'FPS: {fps}', position=(0,image.frame.shape[0]-5), inplace=False)
+            updates[self.display_box] = dict(data=image.encode())
+        return updates
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,112 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
+This module holds the base class for liquid pumps.
 
-Notes / actionables:
--
+Classes:
+    Pump (LiquidHandler)
 """
 # Standard library imports
 import time
 
+# Third party imports
+import serial # pip install pyserial
+
 # Local application imports
-from ...misc import HELPER
-from .cartesian_utils import Gantry
+from ..liquid_utils import LiquidHandler
 print(f"Import: OK <{__name__}>")
 
-class Primitiv(Gantry):
+class Pump(LiquidHandler):
     """
-    Primitiv platform controls
-
+    Abstract Base Class (ABC) for Pump objects (i.e. tools that moves liquids).
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
+    
+    ### Constructor
     Args:
-        port (str): com port address
-        limits (list, optional): lower and upper bounds of movement. Defaults to [(0,0,0), (0,0,0)].
-        safe_height (float, optional): safe height. Defaults to None.
-    
-    Kwargs:
-        max_speed (float, optional): maximum movement speed. Defaults to 250.
-        home_coordinates (tuple, optional): position to home in arm coordinates. Defaults to (0,0,0).
-        home_orientation (tuple, optional): orientation to home. Defaults to (0,0,0).
-        orientate_matrix (numpy.matrix, optional): matrix to transform arm axes to workspace axes. Defaults to np.identity(3).
-        translate_vector (numpy.ndarray, optional): vector to transform arm position to workspace position. Defaults to (0,0,0).
-        implement_offset (tuple, optional): implement offset vector pointing from end of effector to tool tip. Defaults to (0,0,0).
-        scale (int, optional): scale factor to transform arm scale to workspace scale. Defaults to 1.
-        verbose (bool, optional): whether to print outputs. Defaults to False.
+        `port` (str): COM port address
+    
+    ### Properties
+    - `port` (str): COM port address
+    
+    ### Methods
+    #### Abstract
+    - `aspirate`: aspirate desired volume of reagent
+    - `blowout`: blowout liquid from tip
+    - `dispense`: dispense desired volume of reagent
+    - `pullback`: pullback liquid from tip
+    #### Public
+    - `disconnect`: disconnect from device
     """
-    def __init__(self, port:str, limits=[(-410,-290,-120), (0,0,0)], safe_height=-80, **kwargs):
-        super().__init__(port=port, limits=limits, safe_height=safe_height, **kwargs)
-        self.selected_position = ''
-        return
     
-    def _connect(self, port:str, baudrate=115200, timeout=None):
+    def __init__(self, port:str, **kwargs):
         """
-        Connect to machine control unit
+        Instantiate the class
 
         Args:
-            port (str): com port address
-            baudrate (int): baudrate. Defaults to 115200.
-            timeout (int, optional): timeout in seconds. Defaults to None.
-            
-        Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
+            port (str): COM port address
         """
-        self.port = port
-        self._baudrate = baudrate
-        self._timeout = timeout
-        device = super()._connect(self.port, self._baudrate, self._timeout)
+        super().__init__(**kwargs)
+        self._connect(port)
+        return
+    
+    # Properties
+    @property
+    def port(self) -> str:
+        return self.connection_details.get('port', '')
+    
+    def disconnect(self):
+        """Disconnect from device"""
         try:
-            device.close()
-            device.open()
+            self.device.close()
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        self.setFlag(connected=False)
+        return
+     
+    # Protected method(s)
+    def _connect(self, port:str, baudrate:int = 9600, timeout:int = 1):
+        """
+        Connection procedure for tool
 
-            # Start grbl 
-            device.write(bytes("\r\n\r\n", 'utf-8'))
-            time.sleep(2)
-            device.flushInput()
+        Args:
+            port (str): COM port address
+            baudrate (int, optional): baudrate. Defaults to 9600.
+            timeout (int, optional): timeout in seconds. Defaults to 1.
+        """
+        self.connection_details = {
+            'port': port,
+            'baudrate': baudrate,
+            'timeout': timeout
+        }
+        device = None
+        try:
+            device = serial.Serial(port, baudrate, timeout=timeout)
         except Exception as e:
+            print(f"Could not connect to {port}")
             if self.verbose:
                 print(e)
-        return device
+        else:
+            time.sleep(2)   # Wait for grbl to initialize
+            device.flushInput()
+            print(f"Connection opened to {port}")
+            self.setFlag(connected=True)
+        self.device = device
+        return
     
-    @HELPER.safety_measures
-    def home(self):
+    def _write(self, command:str) -> bool:
         """
-        Homing cycle for Primitiv platform
+        Write command to device
+
+        Args:
+            command (str): command string
+
+        Returns:
+            bool: whether command was sent successfully
         """
         try:
-            self.device.write(bytes("$H\n", 'utf-8'))
-            print(self.device.readline())
+            self.device.write(command.encode('utf-8'))
         except Exception as e:
             if self.verbose:
                 print(e)
-        
-        self.coordinates = (0,0,0)
-        return
+            return False
+        return True
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,663 +1,858 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
+This module holds the class for syringe pumps from TriContinent.
 
-Notes / actionables:
-- 
+Classes:
+    TriContinent (Pump)
 """
 # Standard library imports
-import math
-import numpy as np
+from __future__ import annotations
+from functools import wraps
+import string
 import time
+from typing import Callable, Optional, Union
 
 # Local application imports
-from ....misc import HELPER
-from ..jointed_utils import RobotArm
-from .dobot_api import dobot_api_dashboard, dobot_api_feedback
-from . import dobot_attachments as attachments
+from .....misc import Helper
+from ...liquid_utils import Speed
+from ..pump_utils import Pump
+from .tricontinent_lib import ErrorCode, StatusCode, TriContinentPump
 print(f"Import: OK <{__name__}>")
 
-CONNECTION_TIMEOUT = 20
-SCALE = True
-MOVE_TIME_BUFFER_S = 0.5
+class TriContinent(Pump):
+    """
+    TriContinent provides methods to control a syringe pump from TriContinent
 
-class Dobot(RobotArm):
+    ### Constructor
+    Args:
+        `port` (str): COM port address
+        `channel` (Union[int, tuple[int]]): channel id(s)
+        `model` (Union[str, tuple[str]]): model name(s)
+        `capacity` (Union[int, tuple[int]]): capacity (capacities)
+        `output_right` (Union[bool, tuple[bool]]): whether liquid is pumped out to the right for channel(s)
+        `name` (Union[str, tuple[str]], optional): name of the pump(s). Defaults to ''.
+        
+    ### Attributes
+    - `channels` (dict[int, TriContinentPump]): dictionary of {channel id, TriContinentPump object}
+    - `current_channel` (TriContinentPump): currently active pump
+    - `name` (str): name of current pump
+    - `capacity` (int): syringe capacity of current pump
+    - `resolution` (float): volume resolution of current pump (i.e. uL per step)
+    - `step_limit` (int): maximum allowable position of current pump
+    - `position` (int): position of plunger for current pump
+    
+    ### Properties
+    - `current_pump` (TriContinentPump): alias for `current_channel`
+    - `pumps` (dict[int, TriContinentPump]): alias for `channels`
+    - `status` (str): current status of active pump
+    - `volume` (float): volume of current pump
+    
+    ### Methods
+    - `aspirate`: aspirate desired volume of reagent
+    - `blowout`: blowout liquid from tip (NOTE: not implemented)
+    - `cycle`: cycle between aspirate and dispense
+    - `dispense`: dispense desired volume of reagent
+    - `empty`: empty the syringe pump
+    - `fill`: fill the syringe pump
+    - `getPosition`: get the position of the pump plunger from the device
+    - `getStatus`: get the status of the pump from the device
+    - `initialise`: empty pump and set pump outlet direction
+    - `isBusy`: checks and returns whether the device is busy
+    - `loop`: loop a set of actions
+    - `move`: move the plunger either up or down by a specified number of steps
+    - `moveBy`: move the plunger by a specified number of steps
+    - `moveTo`: move the plunger to a specified position
+    - `prime`: prime the pump by cycling the plunger through its maximum and minimum positions
+    - `pullback`: pullback liquid from tip (NOTE: not implemented)
+    - `queue`: queue several commands together before sending to the device
+    - `reset`: reset the device
+    - `resetChannel`: reset the current channel to default (i.e. first channel)
+    - `rinse`: rinse the channel with aspirate and dispense cycles
+    - `run`: execute the command(s)
+    - `setCurrentChannel`: set the current active pump
+    - `setSpeedRamp`: set the acceleration from start speed to top speed
+    - `setStartSpeed`: set the starting speed of plunger
+    - `setTopSpeed`: set the top speed of plunger
+    - `setValve`: set valve position to one of [I]nput, [O]utput, [B]ypass, [E]xtra
+    - `stop`: stop the device immediately, terminating any actions in progress or in queue
+    - `wait`: wait for a specified amount of time
     """
-    Dobot class.
     
-    Args:
-        ip_address (str): IP address of arm
+    _default_flags = {
+        'busy': False, 
+        'connected': False,
+        'execute_now': True
+    }
+    def __init__(self, 
+        port: str, 
+        channel: Union[int, tuple[int]], 
+        model: Union[str, tuple[str]], 
+        capacity: Union[int, tuple[int]], 
+        output_right: Union[bool, tuple[bool]], 
+        name: Union[str, tuple[str]] = '',
+        **kwargs
+    ):
+        """
+        Instantiate the class
+
+        Args:
+            port (str): COM port address
+            channel (Union[int, tuple[int]]): channel id(s)
+            model (Union[str, tuple[str]]): model name(s)
+            capacity (Union[int, tuple[int]]): capacity (capacities)
+            output_right (Union[bool, tuple[bool]]): whether liquid is pumped out to the right for channel(s)
+            name (Union[str, tuple[str]], optional): name of the pump(s). Defaults to ''.
+        """
+        super().__init__(port, **kwargs)
+        self.channels = self._get_pumps(
+            channel = channel,
+            model = model,
+            capacity = capacity,
+            output_right = output_right,
+            name = name
+        )
+        self.current_channel = None
+        
+        self.channel = list(self.channels)[0]
+        self.name = ''
+        self.capacity = 0
+        self.resolution = 1
+        self.step_limit = 1
+        
+        self.position = 0
+        for channel in self.channels:
+            self.setCurrentChannel(channel=channel)
+            self.initialise()
+        self.resetChannel()
+        return
+    
+    # Properties
+    @property
+    def current_pump(self) -> TriContinentPump:
+        return self.current_channel
 
-    Kwargs:
-        home_coordinates (tuple, optional): position to home in arm coordinates. Defaults to (0,0,0).
-        home_orientation (tuple, optional): orientation to home. Defaults to (0,0,0).
-        orientate_matrix (numpy.matrix, optional): matrix to transform arm axes to workspace axes. Defaults to np.identity(3).
-        translate_vector (numpy.ndarray, optional): vector to transform arm position to workspace position. Defaults to (0,0,0).
-        implement_offset (tuple, optional): implement offset vector pointing from end of effector to tool tip. Defaults to (0,0,0).
-        scale (int, optional): scale factor to transform arm scale to workspace scale. Defaults to 1.
-        verbose (bool, optional): whether to print outputs. Defaults to False.
-        safe_height (float, optional): safe height. Defaults to None.
-    """
-    possible_attachments = attachments.ATTACHMENT_NAMES
-    max_actions = max( [len(m) for m in attachments.METHODS] )
-    def __init__(self, ip_address:str, **kwargs):
-        super().__init__(**kwargs)
-        self.ip_address = ip_address
-        self.attachment = None
-        
-        self._speed = 100
-        
-        self.setFlag('retract', True)
-        self._connect(ip_address)
-        pass
+    @property
+    def pumps(self) -> dict[int, TriContinentPump]:
+        return self.channels
     
     @property
-    def dashboard(self):
-        if type(self.device) != dict:
-            return None
-        return self.device.get('dashboard')
-    @dashboard.setter
-    def dashboard(self, value):
-        if type(self.device) != dict:
-            self.device = {}
-        self.device['dashboard'] = value
-        return
+    def status(self) -> str:
+        return self.getStatus()
     
     @property
-    def feedback(self):
-        if type(self.device) != dict:
-            return None
-        return self.device.get('feedback')
-    @feedback.setter
-    def feedback(self, value):
-        if type(self.device) != dict:
-            self.device = {}
-        self.device['feedback'] = value
-        return
+    def volume(self) -> float:
+        return self.position/self.step_limit * self.capacity
     
-    def _connect(self, ip_address:str, timeout=CONNECTION_TIMEOUT):
+    # Decorators
+    def _single_action(func: Callable) -> Callable:
         """
-        Connect to robot hardware
+        Turns a method into a single action that runs only if it is not contained in a compound action
 
         Args:
-            ip_address (str): IP address of robot
-            timeout (int, optional): duration to wait before timeout
-            
+            func (Callable): action method
+        
         Returns:
-            dict: dictionary of dashboard and feedback objects
+            Callable: wrapped method
         """
-        self.device = {
-            'dashboard': None,
-            'feedback': None
-        }
-        try:
-            start_time = time.time()
-            dashboard = dobot_api_dashboard(ip_address, 29999)
-            if time.time() - start_time > timeout:
-                self.device is None
-                raise Exception(f"Unable to connect to arm at {ip_address}")
-            
-            start_time = time.time()
-            feedback = dobot_api_feedback(ip_address, 30003)
-            if time.time() - start_time > timeout:
-                self.device is None
-                raise Exception(f"Unable to connect to arm at {ip_address}")
-
-            self.device['dashboard'] = dashboard
-            self.device['feedback'] = feedback
-            self.reset()
-            self.dashboard.User(0)
-            self.dashboard.Tool(0)
-            self.setSpeed(speed=100)
-        except Exception as e:
-            print(e)
-        return self.device
+        @wraps(func)
+        def wrapper(self, *args, **kwargs) -> str:
+            channel = kwargs.get('channel')
+            self.setCurrentChannel(channel)
+            command = func(self, *args, **kwargs)
+            if self.flags['execute_now']:
+                return self.run(command)
+            return command
+        return wrapper
+    
+    def _compound_action(func: Callable) -> Callable:
+        """
+        Turns a method into a compound action that suppresses single actions within from running
 
-    def _freeze(self):
+        Args:
+            func (Callable): action method
+        
+        Returns:
+            Callable: wrapped method
         """
-        Halt and disable robot
+        @wraps(func)
+        def wrapper(self, *args, **kwargs) -> str:
+            channel = kwargs.get('channel')
+            self.setCurrentChannel(channel)
+            self.setFlag(execute_now=False)
+            command = func(self, *args, **kwargs)
+            self.setFlag(execute_now=True)
+            return command
+        return wrapper
+
+    # Public methods
+    @_compound_action
+    def aspirate(self, 
+        volume: float, 
+        speed: int = 200, 
+        wait: int = 0, 
+        pause: bool = False, 
+        start_speed: int = 50,
+        reagent: Optional[str] = None, 
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> str:
+        """
+        Aspirate desired volume of reagent
+
+        Args:
+            volume (float): target volume
+            speed (int, optional): speed to aspirate at. Defaults to 200.
+            wait (int, optional): time delay after aspirate. Defaults to 0.
+            pause (bool, optional): whether to pause for user intervention. Defaults to False.
+            start_speed (int, optional): starting speed of plunger. Defaults to 50.
+            reagent (Optional[str], optional): name of reagent. Defaults to None.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
         """
-        try:
-            self.dashboard.ResetRobot()
-            self.dashboard.DisableRobot()
-        except (AttributeError, OSError):
-            if self.verbose:
-                print("Not connected to arm!")
-        return
-      
-    def _shutdown(self):
-        """Halt robot and close connections."""
-        self._freeze()
-        self.disconnect()
-        return
+        steps = min(int(volume/self.resolution), self.step_limit-self.position)
+        volume = steps * self.resolution
+        self.queue([
+            self.setStartSpeed(start_speed),
+            self.setTopSpeed(speed),
+            self.setSpeedRamp(1),
+            self.setValve('I'),
+            self.moveBy(steps),
+            self.wait(wait)
+        ], channel=channel)
+        command = self.current_pump.command
+        print(f"Pump: {self.name}")
+        print(f"Aspirating {volume}uL...")
+        self.run()
+        if reagent is not None:
+            self.current_pump.reagent = reagent
+        if pause:
+            input("Press 'Enter' to proceed.")
+        return command
+    
+    def blowout(self, channel: Optional[Union[int, tuple[int]]] = None, **kwargs) -> str: # NOTE: no implementation
+        return ''
+    
+    @_compound_action
+    def cycle(self, 
+        volume: float, 
+        speed: Optional[float] = 200, 
+        wait: int = 0,  
+        cycles: int = 3,
+        start_speed: int = 50,
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> str:
+        """
+        Cycle between aspirate and dispense
+
+        Args:
+            volume (float): target volume
+            speed (Optional[float], optional): speed to aspirate and dispense at. Defaults to 200.
+            wait (int, optional): time delay after each action. Defaults to 0.
+            cycles (int, optional): number of cycles. Defaults to 3.
+            start_speed (int, optional): starting speed of plunger. Defaults to 50.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id(s). Defaults to None.
 
-    def calibrate(self, external_pt1:np.ndarray, internal_pt1:np.ndarray, external_pt2:np.ndarray, internal_pt2:np.ndarray):
+        Returns:
+            str: command string
         """
-        Calibrate internal and external coordinate systems, then verify points.
+        self.queue([
+            self.initialise(),
+            self.setStartSpeed(start_speed),
+            self.setTopSpeed(speed),
+            self.setSpeedRamp(1),
+            self.loop(cycles,
+                self.aspirate(volume, speed=speed, wait=wait, start_speed=start_speed),
+                self.wait(wait),
+                self.dispense(volume, speed=speed, wait=wait, start_speed=start_speed),
+                self.wait(wait)
+            )
+        ], channel=channel)
+        command = self.current_pump.command
+        print(f"Pump: {self.name}")
+        self.run()
+        print(f"Cycling complete: {cycles} time(s)")
+        return command     
+    
+    @_compound_action
+    def dispense(self, 
+        volume: float, 
+        speed: int = 200, 
+        wait: int = 0, 
+        pause: bool = False, 
+        start_speed: int = 50,
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> str:
+        """
+        Dispense desired volume of reagent
+
+        Args:
+            volume (float): target volume
+            speed (int, optional): speed to dispense at. Defaults to 200.
+            wait (int, optional): time delay after dispense. Defaults to 0.
+            pause (bool, optional): whether to pause for user intervention. Defaults to False.
+            start_speed (int, optional): starting speed of plunger. Defaults to 50.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
+        """
+        steps = min(int(volume/self.resolution), self.step_limit)
+        volume = steps * self.resolution
+        self.queue([
+            self.setStartSpeed(start_speed),
+            self.setTopSpeed(speed),
+            self.setSpeedRamp(1)
+        ], channel=channel)
+        if self.position <= steps:
+            print("Refilling first...")
+            self.queue([self.fill()], channel=channel)
+        self.queue([
+            self.setValve('O'),
+            self.moveBy(-abs(steps)),
+            self.wait(wait)
+        ], channel=channel)
+        command = self.current_pump.command
+        print(f"Pump: {self.name}")
+        print(f"Dispensing {volume}uL...")
+        self.run()
+        if pause:
+            input("Press 'Enter' to proceed.")
+        return command
+
+    @_single_action
+    def empty(self, channel:Optional[int] = None, **kwargs) -> str:
+        """
+        Empty the syringe pump
 
         Args:
-            external_pt1 (numpy.ndarray): x,y,z coordinates of physical point 1
-            internal_pt1 (numpy.ndarray): x,y,z coordinates of robot point 1
-            external_pt2 (numpy.ndarray): x,y,z coordinates of physical point 2
-            internal_pt2 (numpy.ndarray): x,y,z coordinates of robot point 2
+            channel (Optional[int], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
         """
-        super().calibrate(external_pt1, internal_pt1, external_pt2, internal_pt2)
+        self.position = 0
+        self.current_pump.position = self.position
+        return "OA0"
 
-        # Verify calibrated points
-        for pt in [external_pt1, external_pt2]:
-            self.home()
-            self.moveTo( pt + np.array([0,0,10]) )
-            input("Press Enter to verify reference point")
-        self.home()
-        return
-    
-    def connect(self):
+    @_single_action
+    def fill(self, channel:Optional[int] = None, **kwargs) -> str:
         """
-        Reconnect to robot using existing IP address
-        
+        Fill the syringe pump
+
+        Args:
+            channel (Optional[int], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
+        """
+        self.position = self.step_limit
+        self.current_pump.position = self.position
+        return f"IA{self.step_limit}"
+
+    def getPosition(self, channel:Optional[int] = None) -> int:
+        """
+        Get the position of the pump plunger from the device
+
+        Args:
+            channel (Optional[int], optional): channel id(s). Defaults to None.
+
         Returns:
-            dict: dictionary of dashboard and feedback objects
+            int: position of plunger
         """
-        return self._connect(self.ip_address)
+        self.setCurrentChannel(channel=channel)
+        response = self._query('?')
+        self.position = int(response[3:]) if len(response) else self.position
+        self.current_pump.position = self.position
+        return self.position
     
-    def disconnect(self):
+    def getStatus(self, channel:Optional[int] = None) -> str:
         """
-        Disconnect serial connection to robot
-        
+        Get the status of the pump from the device
+
+        Args:
+            channel (Optional[int], optional): channel id(s). Defaults to None.
+
+        Raises:
+            RuntimeError: Unable to get status from pump
+            ConnectionError: Please reinitialize pump
+
         Returns:
-            None: None is successfully disconnected, else dict
+            str: status message
         """
-        try:
-            self.dashboard.close()
-            self.feedback.close()
-        except (AttributeError, OSError):
-            if self.verbose:
-                print("Not connected to arm!")
+        self.setCurrentChannel(channel=channel)
+        response = self._query('Q')
+        _status_code = response[2] if len(response) else ''
+        if self.device is not None:
+            if _status_code not in StatusCode.Busy.value and _status_code not in StatusCode.Idle.value:
+                raise RuntimeError(f"Unable to get status from Pump: {self.name}")
+    
+        if _status_code in StatusCode.Busy.value:
+            self.setFlag(busy=True)
+            self.current_pump.busy = True
+        elif _status_code in StatusCode.Idle.value:
+            self.setFlag(busy=False)
+            self.current_pump.busy = False
+        else:
+            self.setFlag(busy=False)
+            self.current_pump.busy = False
+        
+        code = 'er0'
+        if _status_code.isalpha():
+            index = 1 + string.ascii_lowercase.index(_status_code.lower())
+            code = f"er{index}"
+            print(ErrorCode[code].value)
+            if index in [1,7,9,10]:
+                raise ConnectionError(f"Please reinitialize: Pump {self.channel}.")
+        self.current_pump.status = code
+        return ErrorCode[code].value
+ 
+    @_single_action
+    def initialise(self, output_right:Optional[bool] = None, channel:Optional[int] = None) -> str:
+        """
+        Empty pump and set pump outlet direction
+
+        Args:
+            output_right (Optional[bool], optional): whether liquid is pumped out to the right. Defaults to None.
+            channel (Optional[int], optional): channel id(s). Defaults to None.
 
-        self.device = None
-        return self.device
+        Returns:
+            str: command string
+        """
+        output_right = self.current_pump.output_right if output_right is None else output_right
+        command = 'Z' if output_right else 'Y'
+        return command
     
-    def getConfigSettings(self):
+    def isBusy(self) -> bool:
         """
-        Read the robot configuration settings
-        
+        Checks and returns whether the device is busy
+
         Returns:
-            dict: dictionary of robot class and settings
+            bool: whether the device is busy
         """
-        attributes = [
-            "ip_address", 
-            "home_coordinates", 
-            "home_orientation", 
-            "orientate_matrix", 
-            "translate_vector", 
-            "implement_offset",
-            "scale"
-        ]
-        return super().getConfigSettings(attributes)
+        self.getStatus()
+        return super().isBusy()
 
-    def isConnected(self):
+    @staticmethod
+    def loop(cycles:int, *args) -> str:
         """
-        Check whether machine control unit is connected
+        Loop a set of actions
+
+        Args:
+            cycles (int): number of times to loop
 
         Returns:
-            bool: whether machine control unit is connected
+            str: command string
         """
-        if self.device is None:
-            print(f"{self.__class__} ({self.ip_address}) not connected.")
-            return False
-        return True
-
-    @HELPER.safety_measures
-    def moveCoordBy(self, vector=None, angles=None):
+        return f"g{''.join(args)}G{cycles}"
+     
+    @_single_action
+    def move(self, steps:int, up:bool, channel:Optional[int] = None) -> str:
         """
-        Relative Cartesian movement and tool orientation, using robot coordinates.
+        Move the plunger either up or down by a specified number of steps
 
         Args:
-            vector (tuple, optional): x,y,z displacement vector. Defaults to None.
-            angles (tuple, optional): a,b,c rotation angles in degrees. Defaults to None.
+            steps (int): number of steps to move plunger by
+            up (bool): whether to move the plunger up
+            channel (Optional[int], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
         """
-        if vector is None:
-            vector = (0,0,0)
-        if angles is None:
-            angles = (0,0,0)
-        vector = tuple(vector)
-        angles = tuple(angles)
-        try:
-            self.feedback.RelMovL(*vector)
-            self.rotateBy(angles)
-            move_time = max(abs(np.array(vector)) / self.speed) + max(abs(np.array(angles)) / self.speed_angular) +MOVE_TIME_BUFFER_S
-            print(f'Move time: {move_time}s ({self._speed_fraction})')
-            time.sleep(move_time)
-        except (AttributeError, OSError):
-            if self.verbose:
-                print("Not connected to arm!")
-            self.updatePosition(vector=vector, angles=angles)
-            return False
-        self.updatePosition(vector=vector, angles=angles)
-        return True
+        steps = abs(steps)
+        command = ''
+        if up:
+            self.position -= steps
+            command =  f"D{steps}"
+        else:
+            self.position += steps
+            command =  f"P{steps}"
+        self.current_pump.position = self.position
+        return command
+        
+    @_single_action
+    def moveBy(self, steps:int, channel:Optional[int] = None) -> str:
+        """
+        Move plunger by specified number of steps
 
-    @HELPER.safety_measures
-    def moveCoordTo(self, coordinates=None, orientation=None):
+        Args:
+            steps (int): number of steps to move plunger by (>0: aspirate/move down; <0 dispense/move up)
+            channel (Optional[int], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
         """
-        Absolute Cartesian movement and tool orientation, using robot coordinates.
+        self.position += steps
+        self.current_pump.position = self.position
+        command = f"P{abs(steps)}" if steps > 0 else f"D{abs(steps)}"
+        return command
+    
+    @_single_action
+    def moveTo(self, position:int, channel:Optional[int] = None) -> str:
+        """
+        Move plunger to specified position
 
         Args:
-            coordinates (tuple): x,y,z position vector. Defaults to None.
-            orientation (tuple, optional): a,b,c orientation angles in degrees. Defaults to None.
-            tool_offset (bool, optional): whether to consider implement offset. Defaults to True.
-        """
-        if coordinates is None:
-            coordinates = self.coordinates
-        if orientation is None:
-            orientation = self.orientation
-        coordinates = tuple(coordinates)
-        orientation = tuple(orientation)
-        if len(orientation) == 1 and orientation[0] == 0:
-            orientation = self.orientation
-        if not self.isFeasible(coordinates):
-            print(f"Infeasible coordinates! {coordinates}")
-            return
-        
-        try:
-            self.feedback.MovJ(*coordinates, *orientation)
-            position = self.position
-            distances = abs(position[0] - np.array(coordinates))
-            rotations = abs(position[1] - np.array(orientation))
-            move_time = max([max(distances / self.speed),  max(rotations / self.speed_angular)]) +MOVE_TIME_BUFFER_S
-            print(f'Move time: {move_time}s ({self._speed_fraction})')
-            time.sleep(move_time)
-        except (AttributeError, OSError):
-            if self.verbose:
-                print("Not connected to arm!")
-            self.updatePosition(coordinates=coordinates, orientation=orientation)
-            return False
-        self.updatePosition(coordinates=coordinates, orientation=orientation)
-        return True
+            position (int): target plunger position
+            channel (Optional[int], optional): channel id(s). Defaults to None.
 
-    @HELPER.safety_measures
-    def moveJointBy(self, relative_angles):
+        Returns:
+            str: command string
+        """
+        self.position = position
+        self.current_pump.position = self.position
+        return f"A{position}"
+    
+    def prime(self, cycles:int = 3, channel:Optional[int] = None) -> str:
         """
-        Relative joint movement
+        Prime the pump by cycling the plunger through its max and min positions
 
         Args:
-            relative_angles (tuple): j1~j6 rotation angles in degrees
+            cycles (int, optional): number of times to cycle. Defaults to 3.
+            channel (Optional[int], optional): channel id(s). Defaults to None.
             
-        Raises:
-            Exception: Input has to be length 6
+        Returns:
+            str: command string
         """
-        if len(relative_angles) != 6:
-            raise Exception('Length of input needs to be 6')
-        relative_angles = tuple(relative_angles)
-        try:
-            self.feedback.RelMovJ(*relative_angles)
-            move_time = max(abs(np.array(relative_angles)) / self.speed_angular) +MOVE_TIME_BUFFER_S
-            print(f'Move time: {move_time}s ({self._speed_fraction})')
-            time.sleep(move_time)
-        except (AttributeError, OSError):
-            if self.verbose:
-                print("Not connected to arm!")
-            self.updatePosition(angles=relative_angles[3:])
-            return False
-        self.updatePosition(angles=relative_angles[3:])
-        return True
+        command = self.rinse(cycles=cycles, channel=channel, print_message=False)
+        print(f"Priming complete")
+        return command
+    
+    def pullback(self, channel: Optional[Union[int, tuple[int]]] = None, **kwargs) -> bool: # NOTE: no implementation
+        return ''
 
-    @HELPER.safety_measures
-    def moveJointTo(self, absolute_angles):
+    def queue(self, actions:list[str], channel:Optional[int] = None) -> str:
         """
-        Absolute joint movement
+        Queue several commands together before sending to the device
 
         Args:
-            absolute_angles (tuple): j1~j6 orientation angles in degrees
-        
-        Raises:
-            Exception: Input has to be length 6
-        """
-        if len(absolute_angles) != 6:
-            raise Exception('Length of input needs to be 6')
-        absolute_angles = tuple(absolute_angles)
-        try:
-            self.feedback.JointMovJ(*absolute_angles)
-            move_time = max(abs(np.array(absolute_angles)) / self.speed_angular) +MOVE_TIME_BUFFER_S
-            print(f'Move time: {move_time}s ({self._speed_fraction})')
-            time.sleep(move_time)
-        except (AttributeError, OSError):
-            if self.verbose:
-                print("Not connected to arm!")
-            self.updatePosition(orientation=absolute_angles[3:])
-            return False
-        self.updatePosition(orientation=absolute_angles[3:])
-        return True
+            actions (list[str]): list of command strings
+            channel (Optional[int], optional): channel id(s). Defaults to None.
 
-    def reset(self):
+        Returns:
+            str: command string
         """
-        Clear any errors and enable robot
+        self.setCurrentChannel(channel=channel)
+        command = ''.join(actions)
+        self.current_pump.command = self.current_pump.command + command
+        return command
+    
+    def reset(self, channel:Optional[int] = None) -> str:
         """
-        try:
-            self.dashboard.ClearError()
-            self.dashboard.EnableRobot()
-        except (AttributeError, OSError):
-            if self.verbose:
-                print("Not connected to arm!")
+        Reset and initialise the device
+
+        Args:
+            channel (Optional[int], optional): channel id(s). Defaults to None.
+        """
+        return self.initialise()
+    
+    def resetChannel(self):
+        """Reset the current channel to default (i.e. first channel)"""
+        self.setCurrentChannel(list(self.channels)[0])
         return
+    
+    @_compound_action
+    def rinse(self, 
+        speed: int = 200, 
+        wait: int = 0, 
+        cycles: int = 3, 
+        start_speed: int = 50,
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> str:
+        """
+        Rinse the channel with aspirate and dispense cycles
 
-    def setSpeed(self, speed:int):
+        Args:
+            speed (int, optional): speed to aspirate and dispense at. Defaults to 200.
+            wait (int, optional): time delay after each action. Defaults to 0.
+            cycles (int, optional): number of cycles. Defaults to 3.
+            start_speed (int, optional): starting speed of plunger. Defaults to 50.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
         """
-        Setting the Global speed rate.
+        self.queue([
+            self.initialise(),
+            self.setStartSpeed(start_speed),
+            self.setTopSpeed(speed),
+            self.setSpeedRamp(1),
+            self.loop(cycles,
+                self.fill(),
+                self.wait(wait),
+                self.empty(),
+                self.wait(wait)
+            )
+        ], channel=channel)
+        command = self.current_pump.command
+        print(f"Pump: {self.name}")
+        self.run()
+        if kwargs.get('print_message', True):
+            print(f"Rinsing complete")
+        return command
+
+    def run(self, command:Optional[str] = None, channel:Optional[int] = None) -> str:
+        """
+        Execute the command(s)
 
         Args:
-            speed (int): rate value (value range: 1~100)
+            command (str, optional): command string. Defaults to None.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id(s). Defaults to None.
+
+        Returns:
+            str: command string
         """
-        try:
-            speed = int(speed)
-            print(f'Speed: {speed}')
-            self.dashboard.SpeedFactor(speed)
-            self._speed_fraction = (speed/self._speed)
-        except (AttributeError, OSError):
-            if self.verbose:
-                print("Not connected to arm!")
-        return
+        self.setCurrentChannel(channel=channel)
+        if command is None:
+            command = self.current_pump.command
+            self.current_pump.command = ''
+        command = f"{command}R"
+        self._query(command)
+        while self.isBusy():
+            time.sleep(0.2)
+        if 'Z' in command or 'Y' in command:
+            self.current_pump.init_status = True
+        self.getPosition()
+        self.getStatus()
+        return command
     
-    def toggleAttachment(self, on:bool, name='', attachment_type=None, attachment_module=attachments):
+    def setCurrentChannel(self, channel:Optional[int] = None) -> TriContinentPump:
         """
-        Add an attachment that interfaces with the Dobot's Digital Output (DO)
+        Set the current active pump
 
         Args:
-            on (bool): whether to add attachment, False if removing attachment
-            name (str, optional): name of attachment type in attachment_module. Defaults to None.
-            attachment_type (any, optional): attachment to load. Defaults to None.
-            attachment_module (module, optional): module containing relevant attachments. Defaults to None.
+            channel (Optional[int], optional): channel id. Defaults to None.
+
+        Returns:
+            TriContinentPump: currently active pump
+        """
+        channel = self.channel if channel not in self.channels else channel
+        self.current_channel = self.channels[channel]
+        pump = self.current_pump
         
-        Raises:
-            Exception: Provide a module containing relevant attachments
-            Exception: Select a valid attachment name
-            Exception: Input at least one of 'name' or 'attachment_type'
-            Exception: Input only one of 'name' or 'attachment_type'
-        """
-        if on: # Add attachment
-            if name is None and attachment_type is not None:
-                pass
-            elif name is not None and attachment_type is None:
-                if attachment_module is None:
-                    raise Exception(f"Please provide a module containing relevant attachments")
-                if name not in attachment_module.ATTACHMENT_NAMES:
-                    raise Exception(f"Please select a program name from: {', '.join(attachment_module.ATTACHMENT_NAMES)}")
-                attachment_type = getattr(attachment_module, name)
-            elif name is None and attachment_type is None:
-                if len(attachment_module.ATTACHMENTS) > 1:
-                    raise Exception("Please input at least one of 'name' or 'attachment_type'")
-                attachment_type = attachment_module.ATTACHMENTS[0]
-            else:
-                raise Exception("Please input only one of 'name' or 'attachment_type'")
-            
-            # input("Please secure tool attachment")
-            print("Please secure tool attachment")
-            self.attachment = attachment_type(self.dashboard)
-            self.setImplementOffset(self.attachment.implement_offset)
-        else: # Remove attachment
-            # input("Please remove tool attachment")
-            print("Please remove tool attachment")
-            self.attachment = None
-            self.setImplementOffset((0,0,0))
+        self.channel = pump.channel
+        self.name = pump.name
+        self.capacity = pump.capacity
+        self.resolution = pump.resolution
+        self.step_limit = pump.step_limit
+        self.position = pump.position
         return
-    
-    def toggleCalibration(self, on:bool, tip_length=21):
+ 
+    @_single_action
+    def setSpeedRamp(self, ramp:int, channel:Optional[int] = None) -> str:
         """
-        Enter into calibration mode, with a sharp point implement for alignment.
+        Set the acceleration from start speed to top speed
 
         Args:
-            on (bool): whether to set to calibration mode
-            tip_length (int, optional): length of sharp point alignment implement. Defaults to 21.
-        """
-        if on: # Enter calibration mode
-            tip_length = int(input(f"Please swap to calibration tip and enter tip length in mm (Default: {tip_length}mm)") or str(tip_length))
-            self._temporary_tool_offset = self.implement_offset
-            self.setImplementOffset((0,0,-tip_length))
-        else: # Exit calibration mode
-            input("Please swap back to original tool")
-            self.setImplementOffset(self._temporary_tool_offset)
-            del self._temporary_tool_offset
-        return
+            ramp (int): acceleration rate
+            channel (Optional[int], optional): channel id. Defaults to None.
 
+        Returns:
+            str: command string
+        """
+        return f"L{ramp}"
+    
+    @_single_action
+    def setStartSpeed(self, speed:int, channel:Optional[int] = None) -> str:
+        """
+        Set the starting speed of the plunger
 
-class MG400(Dobot):
-    """
-    MG400 class.
+        Args:
+            speed (int): starting speed of plunger
+            channel (Optional[int], optional): channel id. Defaults to None.
 
-    Args:
-        ip_address (str, optional): IP address of arm. Defaults to '192.168.2.8'.
-        retract (bool, optional): whether to tuck arm before each movement. Defaults to True.
-        home_coordinates (tuple, optional): position to home in arm coordinates. Defaults to (0,300,0).
-        
-    Kwargs:
-        home_orientation (tuple, optional): orientation to home. Defaults to (0,0,0).
-        orientate_matrix (numpy.matrix, optional): matrix to transform arm axes to workspace axes. Defaults to np.identity(3).
-        translate_vector (numpy.ndarray, optional): vector to transform arm position to workspace position. Defaults to (0,0,0).
-        implement_offset (tuple, optional): implement offset vector pointing from end of effector to tool tip. Defaults to (0,0,0).
-        scale (int, optional): scale factor to transform arm scale to workspace scale. Defaults to 1.
-        verbose (bool, optional): whether to print outputs. Defaults to False.
-        safe_height (float, optional): safe height. Defaults to None.
-    """
-    def __init__(self, ip_address='192.168.2.8', retract=True, home_coordinates=(0,300,0), **kwargs):
-        super().__init__(ip_address=ip_address, home_coordinates=home_coordinates, **kwargs)
-        self._speed = 100
-        self._speed_angular = 300
-        self.home()
-        
-        self.setFlag('retract', retract)
-        self.setHeight('safe', 75)
-        return
+        Returns:
+            str: command string
+        """
+        return f"v{speed}"
     
-    def isFeasible(self, coordinates, transform=False, tool_offset=False):
+    @_single_action
+    def setTopSpeed(self, speed:int, channel:Optional[int] = None) -> str:
         """
-        Checks if specified coordinates is a feasible position for robot to access.
+        Set the top speed of the plunger
 
         Args:
-            coordinates (tuple): x,y,z coordinates
-            transform (bool, optional): whether to transform the coordinates. Defaults to False.
-            tool_offset (bool, optional): whether to consider tooltip offset. Defaults to False.
+            speed (int): top speed of plunger
+            channel (Optional[int], optional): channel id. Defaults to None.
 
         Returns:
-            bool: whether coordinates is a feasible position
+            str: command string
         """
-        if transform:
-            coordinates = self._transform_in(coordinates=coordinates, tool_offset=tool_offset)
-        x,y,z = coordinates
-        j1 = round(math.degrees(math.atan(x/(y + 1E-6))), 3)
-        if y < 0:
-            j1 += (180 * math.copysign(1, x))
-        if abs(j1) > 160:
-            return False
-        if not (-150 < z < 230):
-            return False
-        if self.deck.is_excluded(coordinates=self._transform_out(coordinates, tool_offset=True)):
-            return False
-        return True
+        self.speed = Speed(speed,speed)
+        return f"V{speed}"
     
-    def retractArm(self, target=None):
+    @_single_action
+    def setValve(self, 
+        valve: str, 
+        value: Optional[int] = None, 
+        channel: Optional[int] = None
+    ) -> str:
         """
-        Tuck in arm, rotate about base, then extend again.
+        Set valve position to one of [I]nput, [O]utput, [B]ypass, [E]xtra
 
         Args:
-            target (tuple, optional): x,y,z coordinates of destination. Defaults to None.
-        
+            valve (str): one of the above positions
+            value (Optional[int], optional): only for 6-way distribution. Defaults to None.
+            channel (Optional[int], optional): channel to set. Defaults to None.
+
+        Raises:
+            Exception: Please select a valid position
+
         Returns:
-            bool: whether movement is successful
+            str: command string
         """
-        return_values= []
-        safe_radius = 225
-        safe_height = self.heights.get('safe', 75)
-        x,y,_ = self.coordinates
-        if any((x,y)):
-            w = ( (safe_radius**2)/(x**2 + y**2) )**0.5
-            x,y = (x*w,y*w)
-        else:
-            x,y = (0,safe_radius)
-        ret = self.moveCoordTo((x,y,safe_height), self.orientation)
-        return_values.append(ret)
-
-        if target is not None and len(target) == 3:
-            x1,y1,_ = target
-            if any((x1,y1)):
-                w1 = ( (safe_radius**2)/(x1**2 + y1**2) )**0.5
-                x1,y1 = (x1*w1,y1*w1)
-            else:
-                x1,y1 = (0,safe_radius)
-            ret = self.moveCoordTo((x1,y1,75), self.orientation)
-            return_values.append(ret)
-        return all(return_values)
+        valves = ['I','O','B','E']
+        valve = valve.upper()[0]
+        if valve not in valves:
+            raise Exception(f"Please select a valve position from {', '.join(valves)}")
+        command = valve
+        if value in [1,2,3,4,5,6]:
+            command = f'{valve}{value}'
+        return command
+   
+    def stop(self, channel:Optional[int] = None) -> str:
+        """
+        Stops the pump immediately, terminating any actions in progress or in queue
 
+        Args:
+            channel (Optional[int], optional): channel to stop. Defaults to None.
 
-class M1Pro(Dobot):
-    """
-    M1 Pro class.
-    
-    Args:
-        ip_address (str, optional): IP address of arm. Defaults to '192.168.2.21'.
-        retract (bool, optional): whether to tuck arm before each movement. Defaults to False.
-        handedness (str, optional): handedness of robot (i.e. left or right). Defaults to 'left'.
-        home_coordinates (tuple, optional): position to home in arm coordinates. Defaults to (0,300,100).
-        
-    Kwargs:
-        home_orientation (tuple, optional): orientation to home. Defaults to (0,0,0).
-        orientate_matrix (numpy.matrix, optional): matrix to transform arm axes to workspace axes. Defaults to np.identity(3).
-        translate_vector (numpy.ndarray, optional): vector to transform arm position to workspace position. Defaults to (0,0,0).
-        implement_offset (tuple, optional): implement offset vector pointing from end of effector to tool tip. Defaults to (0,0,0).
-        scale (int, optional): scale factor to transform arm scale to workspace scale. Defaults to 1.
-        verbose (bool, optional): whether to print outputs. Defaults to False.
-        safe_height (float, optional): safe height. Defaults to None.
-    """
-    def __init__(self, ip_address='192.168.2.21', handedness='right', home_coordinates=(0,300,100), **kwargs):
-        super().__init__(ip_address=ip_address, home_coordinates=home_coordinates, **kwargs)
-        self._speed = 100
-        self._speed_angular = 180
-        self.home()
-        
-        self.setFlag('right_handed', None)
-        self.setHandedness(handedness)
-        return
-    
-    def home(self, tool_offset=False):
+        Returns:
+            str: command string
         """
-        Return the robot to home
+        _channel = self.channel
+        self.channel = _channel if channel is None else channel
+        response = self._query('T')
+        self.channel = _channel
+        return response
+   
+    @_single_action
+    def wait(self, time_ms:int, channel:Optional[int] = None) -> str:
+        """
+        Wait for a specified amount of time
 
         Args:
-            tool_offset (bool, optional): whether to consider the offset of the tooltip. Defaults to False.
-        
+            time_ms (int): duration in milliseconds
+            channel (Optional[int], optional): channel id. Defaults to None.
+
+        Returns:
+            str: command string
+        """
+        command = f"M{time_ms}" if time_ms else ""
+        return command
+
+    # Protected method(s)
+    @staticmethod
+    def _get_pumps(**kwargs) -> dict[int, TriContinentPump]:
+        """
+        Generate TriContinentPump dataclass objects from parameters
+
+        Raises:
+            ValueError: Ensure that the length of inputs are the same as the number of channels
+
         Returns:
-            bool: whether movement is successful
+            dict[int, TriContinentPump]: dictionary of {channel id, `TriContinentPump` object}
         """
-        return super().home(tool_offset)
+        channel_arg = kwargs.get('channel', 1)
+        n_channel = 1 if type(channel_arg) is int else len(channel_arg)
+        for key, arg in kwargs.items():
+            if type(arg) is not tuple and type(arg) is not list:
+                kwargs[key] = [arg] * n_channel
+            elif len(arg) != n_channel:
+                raise ValueError("Ensure that the length of inputs are the same as the number of channels.")
+        properties = Helper.zip_inputs(primary_keyword='channel', **kwargs)
+        return {key: TriContinentPump(**value) for key,value in properties.items()}
     
-    def isFeasible(self, coordinates, transform=False, tool_offset=False):
+    def _is_expected_reply(self, response:str, **kwargs) -> bool:
         """
-        Checks if specified coordinates is a feasible position for robot to access.
+        Checks and returns whether the response is an expected reply
 
         Args:
-            coordinates (tuple): x,y,z coordinates
-            transform (bool, optional): whether to transform the coordinates. Defaults to False.
-            tool_offset (bool, optional): whether to consider tooltip offset. Defaults to False.
+            response (str): response string from device
 
         Returns:
-            bool: whether coordinates is a feasible position
+            bool: whether the response is an expected reply
         """
-        if transform:
-            coordinates = self._transform_in(coordinates=coordinates, tool_offset=tool_offset)
-        x,y,z = coordinates
-        
-        if not (5 < z < 245):
+        if len(response) == 0:
             return False
-        if x >= 0:
-            r = (x**2 + y**2)**0.5
-            if not (153 <= r <= 400):
-                return False
-        elif abs(y) < 230/2:
+        if response[0] != '/':
             return False
-        elif (x**2 + (abs(y)-200)**2)**0.5 > 200:
-            return False
-        
-        # Space constraints
-        # if x > 344: # front edge
-        #     return False
-        # if x < 76 and abs(y) < 150: # elevated structure
-        #     return False
-        if self.deck.is_excluded(coordinates=self._transform_out(coordinates, tool_offset=True)):
+        if response[1] != str(self.channel) and response[1] != str(0):
             return False
-                
-        # x=4, y=3
-        grad = abs(y/(x+1E-6))
-        if grad > 0.75 or x < 0:
-            hand = 'right' if y>0 else 'left'
-            self.setHandedness(hand, stretch=True)
         return True
     
-    def moveCoordBy(self, vector=None, angles=None):
+    def _query(self, command:str, timeout_s:int = 2) -> str:
         """
-        Relative Cartesian movement and tool orientation, using robot coordinates.
+        Write command to and read response from device
 
         Args:
-            vector (tuple, optional): x,y,z displacement vector. Defaults to None.
-            angles (tuple, optional): a,b,c rotation angles in degrees. Defaults to None.
-        """
-        if vector is None:
-            vector = (0,0,0)
-        if angles is None:
-            angles = (0,0,0)
-        coordinates, orientation = self.position
-        new_coordinates = np.array(coordinates) + np.array(vector)
-        new_orientation = np.array(orientation) + np.array(angles)
-        return self.moveCoordTo(new_coordinates, new_orientation)
+            command (str): command string
+            timeout_s (int, optional): duration to wait before timeout. Defaults to 2.
 
-    def setHandedness(self, hand, stretch=False):
+        Returns:
+            str: response string
         """
-        Set handedness of robot arm
+        # self.connect()
+        start_time = time.time()
+        self._write(command)
+        response = ''
+        while not self._is_expected_reply(response):
+            if not self.isConnected():
+                break
+            if time.time() - start_time > timeout_s:
+                break
+            response = self._read()
+            if response == '__break__':
+                response = ''
+                break
+        # print(time.time() - start_time)
+        # self.disconnect()
+        return response
 
-        Args:
-            hand (str): handedness
-            stretch (bool, optional): whether to stretch the arm. Defaults to False.
+    def _read(self) -> str:
+        """
+        Read response from device
 
-        Raises:
-            Exception: The parameter 'hand' has to be either 'left' or 'right'
+        Returns:
+            str: response string
         """
-        set_hand = False
-        handedness = None
-        if self._flags.get('right_handed', None) is not None:
-            handedness = 'right' if self._flags['right_handed'] else 'left'
-        if hand not in ['left','l','L','right','r','R']:
-            raise Exception("Please select between 'left' or 'right'")
-        if hand in ['left','l','L'] and handedness != 'left': #0
-            try:
-                self.dashboard.SetArmOrientation(0,1,1,1)
-                time.sleep(2)
-            except (AttributeError, OSError):
-                if self.verbose:
-                    print("Not connected to arm!")
-            finally:
-                self.setFlag('right_handed', False)
-                set_hand = True
-        elif hand in ['right','r','R'] and handedness != 'right': #1
-            try:
-                self.dashboard.SetArmOrientation(1,1,1,1)
-                time.sleep(2)
-            except (AttributeError, OSError):
-                if self.verbose:
-                    print("Not connected to arm!")
-            finally:
-                self.setFlag('right_handed', True)
-                set_hand = True
-        if set_hand and stretch:
-            self.stretchArm()
-            time.sleep(1)
-        return
-            
-    def stretchArm(self):
+        response = ''
+        try:
+            response = self.device.read_until().decode('utf-8')
+            response = response.split('\x03')[0]
+        except AttributeError:
+            pass
+        except Exception as e:
+            if self.verbose:
+                print(e)
+            response = '__break__'
+        return response
+    
+    def _write(self, command:str) -> bool:
         """
-        Stretch arm to switch handedness
-        
+        Write command to device
+
+        Args:
+            command (str): <command code><value>
+
         Returns:
-            bool: whether movement is successful
+            bool: whether command was sent successfully
         """
-        _,y,z = self.coordinates
-        y = 240 * math.copysign(1, y)
-        return self.moveCoordTo(coordinates=(320,y,z))
-    
+        if self.verbose:
+            print(command)
+        fstring = f'/{self.channel}{command}\r' # command template: <PRE><ADR><STRING><POST>
+        try:
+            # Typical timeout wait is 2s
+            self.device.write(fstring.encode('utf-8'))
+        except AttributeError:
+            pass
+        except Exception as e:
+            if self.verbose:
+                print(e)
+            return False
+        return True
+
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,243 +1,292 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
+This module holds the base class for jointed mover tools.
 
-Notes / actionables:
--
+Classes:
+    RobotArm (Mover)
 """
 # Standard library imports
+from __future__ import annotations
+from abc import abstractmethod
 import numpy as np
+from typing import Optional
 
 # Local application imports
-from ...misc import HELPER
-from ..mover_utils import Mover
+from ..move_utils import Mover
 print(f"Import: OK <{__name__}>")
 
 class RobotArm(Mover):
     """
-    Robot arm controls
+    Abstract Base Class (ABC) for Robot Arm objects. RobotArm provides controls for jointed robots with articulated arms.
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
     
+    ### Constructor
     Args:
-        safe_height (float, optional): safe height. Defaults to None.
+        `safe_height` (Optional[float], optional): height at which obstacles can be avoided. Defaults to None.
+        `retract` (bool, optional): whether to retract arm before movement. Defaults to False.
 
-    Kwargs:
-        home_coordinates (tuple, optional): position to home in arm coordinates. Defaults to (0,0,0).
-        home_orientation (tuple, optional): orientation to home. Defaults to (0,0,0).
-        orientate_matrix (numpy.matrix, optional): matrix to transform arm axes to workspace axes. Defaults to np.identity(3).
-        translate_vector (numpy.ndarray, optional): vector to transform arm position to workspace position. Defaults to (0,0,0).
-        implement_offset (tuple, optional): implement offset vector pointing from end of effector to tool tip. Defaults to (0,0,0).
-        scale (int, optional): scale factor to transform arm scale to workspace scale. Defaults to 1.
-        verbose (bool, optional): whether to print outputs. Defaults to False.
+    ### Properties
+    - `speed_angular` (float): angular speed of the robot
+
+    ### Methods
+    #### Abstract
+    - `disconnect`: disconnect from device
+    - `isFeasible`: checks and returns whether the target coordinate is feasible
+    - `moveCoordBy`: relative Cartesian movement and tool orientation, using robot coordinates
+    - `moveCoordTo`: absolute Cartesian movement and tool orientation, using robot coordinates
+    - `moveJointBy`: relative joint movement
+    - `moveJointTo`: absolute joint movement
+    - `reset`: reset the robot
+    - `retractArm`: tuck in arm, rotate about base, then extend again
+    - `setSpeed`: set the speed of the robot
+    - `shutdown`: shutdown procedure for tool
+    - `_connect`: connection procedure for tool
+    #### Public
+    - `home`: make the robot go home
+    - `moveBy`: move the robot by target direction, by specified vector and angles
+    - `moveTo`: move the robot to target position, using workspace coordinates
+    - `rotateBy`: relative end effector rotation
+    - `rotateTo`: absolute end effector rotation
     """
-    def __init__(self, safe_height=None, **kwargs):
+    
+    _default_flags = {
+        'busy': False,
+        'connected': False,
+        'retract': False
+    }
+    def __init__(self, safe_height:Optional[float] = None, retract:bool = False, **kwargs):
+        """
+        Instantiate the class
+
+        Args:
+            safe_height (Optional[float], optional): height at which obstacles can be avoided. Defaults to None.
+            retract (bool, optional): whether to retract arm before movement. Defaults to False.
+        """
         super().__init__(**kwargs)
-        self.device = None
-        self._speed_angular = 1
-        self.setFlag('retract', False)
+        self._speed_angular_max = 1
         
+        self.setFlag(retract=retract)
         if safe_height is not None:
-            self.setHeight('safe', safe_height)
+            self.setHeight(safe=safe_height)
         # else:
         #     self.setHeight('safe', self.home_coordinates[2])
         return
     
+    @abstractmethod
+    def moveCoordBy(self, 
+        vector: tuple[float] = (0,0,0), 
+        angles: tuple[float] = (0,0,0)
+    ) -> bool:
+        """
+        Relative Cartesian movement and tool orientation, using robot coordinates
+
+        Args:
+            vector (tuple[float], optional): x,y,z displacement vector. Defaults to (0,0,0).
+            angles (tuple[float], optional): a,b,c rotation angles in degrees. Defaults to (0,0,0).
+
+        Returns:
+            bool: whether movement is successful
+        """
+
+    @abstractmethod
+    def moveCoordTo(self, 
+        coordinates: Optional[tuple[float]] = None, 
+        orientation: Optional[tuple[float]] = None
+    ) -> bool:
+        """
+        Absolute Cartesian movement and tool orientation, using robot coordinates
+
+        Args:
+            coordinates (Optional[tuple[float]], optional): x,y,z position vector. Defaults to None.
+            orientation (Optional[tuple[float]], optional): a,b,c orientation angles in degrees. Defaults to None.
+        
+        Returns:
+            bool: whether movement is successful
+        """
+
+    @abstractmethod
+    def moveJointBy(self, relative_angles: tuple[float]) -> bool:
+        """
+        Relative joint movement
+
+        Args:
+            relative_angles (tuple[float]): j1~j6 rotation angles in degrees
+
+        Raises:
+            ValueError: Length of input needs to be 6.
+
+        Returns:
+            bool: whether movement is successful
+        """
+        if len(relative_angles) == 6:
+            raise ValueError('Length of input needs to be 6.')
+
+    @abstractmethod
+    def moveJointTo(self, absolute_angles: tuple[float]) -> bool:
+        """
+        Absolute joint movement
+
+        Args:
+            absolute_angles (tuple[float]): j1~j6 orientation angles in degrees
+
+        Raises:
+            ValueError: Length of input needs to be 6.
+
+        Returns:
+            bool: whether movement is successful
+        """
+        if len(absolute_angles) != 6:
+            raise ValueError('Length of input needs to be 6.')
+    
+    @abstractmethod
+    def retractArm(self, target: Optional[tuple[float]] = None) -> bool:
+        """
+        Tuck in arm, rotate about base, then extend again
+
+        Args:
+            target (Optional[tuple[float]], optional): x,y,z coordinates of destination. Defaults to None.
+
+        Returns:
+            bool: whether movement is successful
+        """
+  
+    # Properties
     @property
-    def speed_angular(self):
-        return self._speed_angular * self._speed_fraction
+    def speed_angular(self) -> float:
+        if self.verbose:
+            print(f'Max speed: {self._speed_max}')
+            print(f'Speed fraction: {self._speed_fraction}')
+        return self._speed_angular_max * self._speed_fraction
     
-    def home(self, tool_offset=True):
+    def home(self, safe:bool = True, tool_offset:bool = True) -> bool:
         """
-        Return the robot to home
+        Make the robot go home
 
         Args:
-            tool_offset (bool, optional): whether to consider the offset of the tooltip. Defaults to True.
+            safe (bool, optional): whether to use `safeMoveTo()`. Defaults to True.
+            tool_offset (bool, optional): whether to consider tooltip offset. Defaults to True.
         
         Returns:
             bool: whether movement is successful
         """
-        return_values= []
+        success= []
+        ret = False
+        coordinates = self.home_coordinates - self.implement_offset if tool_offset else self.home_coordinates
+        
         # Tuck arm in to avoid collision
-        if self._flags['retract']:
-            ret = self.retractArm(self.home_coordinates)
-            return_values.append(ret)
+        if self.flags.get('retract', False):
+            ret = self.retractArm(coordinates)
+            success.append(ret)
         
         # Go to home position
-        coordinates = self.home_coordinates - self.implement_offset if tool_offset else self.home_coordinates
-        # coordinates = self._transform_out(coordinates=coordinates, tool_offset=tool_offset)
-        # ret = self.safeMoveTo(coordinates=coordinates, orientation=self.home_orientation)
-        ret = self.moveCoordTo(coordinates, self.home_orientation)
-        return_values.append(ret)
+        if safe:
+            coordinates = self._transform_out(coordinates=coordinates, tool_offset=tool_offset)
+            ret = self.safeMoveTo(coordinates=coordinates, orientation=self.home_orientation, tool_offset=tool_offset)
+        else:
+            ret = self.moveCoordTo(coordinates, self.home_orientation)
+        success.append(ret)
         print("Homed")
-        return all(return_values)
+        return all(success)
     
-    def moveBy(self, vector=None, angles=None, **kwargs):
+    def moveBy(self, 
+        vector: tuple[float] = (0,0,0), 
+        angles: tuple[float] = (0,0,0), 
+        **kwargs
+    ) -> bool:
         """
-        Move robot by specified vector and angles
+        Move the robot by target direction, by specified vector and angles
 
         Args:
-            vector (tuple, optional): x,y,z vector to move in. Defaults to None.
-            angles (tuple, optional): a,b,c angles to move in. Defaults to None.
+            vector (tuple[float], optional): x,y,z vector to move in. Defaults to (0,0,0).
+            angles (tuple[float], optional): a,b,c angles to move in. Defaults to (0,0,0).
 
         Returns:
             bool: whether movement is successful
         """
-        if vector is None:
-            vector = (0,0,0)
-        if angles is None:
-            angles = (0,0,0)
         vector = self._transform_in(vector=vector)
         vector = np.array(vector)
         angles = np.array(angles)
         
         if len(angles) != 3:
             if len(angles) == 6:
                 return self.moveJointBy(relative_angle=angles)
             return False
         return self.moveCoordBy(vector, angles)
 
-    def moveTo(self, coordinates=None, orientation=None, tool_offset=True, retract=False, **kwargs):
+    def moveTo(self, 
+        coordinates: Optional[tuple[float]] = None, 
+        orientation: Optional[tuple[float]] = None, 
+        tool_offset: bool = True, 
+        retract: bool = False, 
+        **kwargs
+    ) -> bool:
         """
-        Absolute Cartesian movement, using workspace coordinates.
+        Move the robot to target position, using workspace coordinates
 
         Args:
-            coordinates (tuple, optional): x,y,z coordinates to move to. Defaults to None.
-            orientation (tuple, optional): a,b,c orientation to move to. Defaults to None.
-            retract (bool, optional): whether to tuck in arm before moving. Defaults to False.
+            coordinates (Optional[tuple[float]], optional): x,y,z coordinates to move to. Defaults to None.
+            orientation (Optional[tuple[float]], optional): a,b,c orientation to move to. Defaults to None.
             tool_offset (bool, optional): whether to consider tooltip offset. Defaults to True.
-        
+            retract (bool, optional): whether to retract arm before movement. Defaults to False.
+
         Returns:
             bool: whether movement is successful
         """
         if coordinates is None:
-            coordinates,_ = self.getToolPosition() if tool_offset else self.getUserPosition()
+            coordinates,_ = self.tool_position if tool_offset else self.user_position
         if orientation is None:
             orientation = self.orientation
         coordinates = self._transform_in(coordinates=coordinates, tool_offset=tool_offset)
         coordinates = np.array(coordinates)
         orientation = np.array(orientation)
         
-        if self._flags['retract'] and retract:
+        if self.flags['retract'] and retract:
             self.retractArm(coordinates)
         
         if len(orientation) != 3:
             if len(orientation) == 6:
                 return self.moveJointTo(absolute_angle=orientation)
             return False
         return self.moveCoordTo(coordinates, orientation)
     
-    @HELPER.safety_measures
-    def moveCoordBy(self, vector=None, angles=None):
-        """
-        Relative Cartesian movement and tool orientation, using robot coordinates.
-
-        Args:
-            vector (tuple, optional): x,y,z displacement vector. Defaults to None.
-            angles (tuple, optional): a,b,c rotation angles in degrees. Defaults to None.
-        
-        Returns:
-            bool: whether movement is successful
-        """
-        return True
-
-    @HELPER.safety_measures
-    def moveCoordTo(self, coordinates=None, orientation=None):
-        """
-        Absolute Cartesian movement and tool orientation, using robot coordinates.
-
-        Args:
-            coordinates (tuple, optional): x,y,z position vector. Defaults to None.
-            orientation (tuple, optional): a,b,c orientation angles in degrees. Defaults to None.
-            tool_offset (bool, optional): whether to consider implement offset. Defaults to True.
-        
-        Returns:
-            bool: whether movement is successful
-        """
-        return True
-
-    @HELPER.safety_measures
-    def moveJointBy(self, relative_angles):
-        """
-        Relative joint movement.
-
-        Args:
-            relative_angles (tuple): j1~j6 rotation angles in degrees
-        
-        Raises:
-            Exception: Input has to be length 6
-        
-        Returns:
-            bool: whether movement is successful
-        """
-        if len(relative_angles) != 6:
-            raise Exception('Length of input needs to be 6')
-        return True
-
-    @HELPER.safety_measures
-    def moveJointTo(self, absolute_angles):
-        """
-        Absolute joint movement.
-
-        Args:
-            absolute_angles (tuple): j1~j6 orientation angles in degrees
-        
-        Raises:
-            Exception: Input has to be length 6
-        
-        Returns:
-            bool: whether movement is successful
-        """
-        if len(absolute_angles) != 6:
-            raise Exception('Length of input needs to be 6')
-        return True
-    
-    @HELPER.safety_measures
-    def retractArm(self, target=None):
+    def rotateBy(self, angles: tuple[float]) -> bool:
         """
-        Tuck in arm, rotate about base, then extend again.
+        Relative effector rotation
 
         Args:
-            target (tuple, optional): x,y,z coordinates of destination. Defaults to None.
-        
-        Returns:
-            bool: whether movement is successful
-        """
-        return True
-    
-    def rotateBy(self, angles):
-        """
-        Relative effector rotation.
-
-        Args:
-            angles (tuple): a,b,c rotation angles in degrees
+            angles (tuple[float]): a,b,c rotation angles in degrees
         
         Raises:
-            Exception: Input has to be length 3
+            Exception: Length of input needs to be 3 or 6
         
         Returns:
             bool: whether movement is successful
         """
-        if len(angles) != 3:
-            raise Exception('Length of input needs to be 3')
-        angles = tuple(angles)
         if not any(angles):
             return True
-        return self.moveJointBy((0,0,0,*angles))
+        if len(angles) == 3:
+            return self.moveJointBy((0,0,0,*angles))
+        if len(angles) == 6:
+            return self.moveJointBy(angles)
+        raise ValueError('Length of input needs to be 3 or 6.')
 
-    def rotateTo(self, orientation):
+    def rotateTo(self, orientation: tuple[float]) -> bool:
         """
-        Absolute effector rotation.
+        Absolute end effector rotation
 
         Args:
-            orientation (tuple): a,b,c orientation angles in degrees
+            orientation (tuple[float]): a,b,c orientation angles in degrees
         
         Raises:
-            Exception: Input has to be length 3
+            Exception: Length of input needs to be 3 or 6
         
         Returns:
             bool: whether movement is successful
         """
-        if len(orientation) != 3:
-            raise Exception('Length of input needs to be 3')
-        angles = np.array(orientation) - np.array(self.orientation)
-        return self.rotateBy(angles)
+        if not any(orientation):
+            return True
+        if len(orientation) == 3:
+            return self.rotateBy(orientation - self.orientation)
+        if len(orientation) == 6:
+            return self.moveJointTo(orientation)
+        raise ValueError('Length of input needs to be 3 or 6.')
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,383 +1,370 @@
 # %% -*- coding: utf-8 -*-
 """
-Adapted from @jaycecheng spinutils
+This module holds the base class for liquid handler tools.
 
-Created: Tue 2022/11/01 17:13:35
-@author: Chang Jie
-
-Notes / actionables:
--
+Classes:
+    LiquidHandler (ABC)
+    Speed (dataclass)
 """
 # Standard library imports
-import time
-
-# Third party imports
-import serial # pip install pyserial
-
-# Local application imports
-from ...misc import Helper
-from .liquid_utils import LiquidHandler
-from .Pumps import Peristaltic
+from __future__ import annotations
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
+import numpy as np
+from typing import Optional, Union
 print(f"Import: OK <{__name__}>")
 
-CALIBRATION_ASPIRATE = 27
-CALIBRATION_DISPENSE = 23.5
-DEFAULT_SPEED = 3000 # speed of pump
-PULLBACK_TIME = 2 # amount of time to pullback [s]
-
-class Syringe(LiquidHandler):
+@dataclass
+class Speed:
+    """
+    Speed dataclass represents a single aspirate-dispense speed pair
+    
+    ### Constructor
+    Args:
+        up (float): speed of upwards movement
+        down (float): speed of downwards movement
     """
-    Syringe class
+    
+    up: float
+    down: float
 
+class LiquidHandler(ABC):
+    """
+    Abstract Base Class (ABC) for Liquid Handler objects (i.e. tools that transfer liquids).
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
+    
+    ### Constructor
     Args:
-        capacity (int, or float): capacity of syringe
-        channel (int): channel index
-        offset (tuple, optional): coordinates offset. Defaults to None.
-        pullback_time (int, optional): duration of pullback. Defaults to 2.
-        
-    Kwargs:
-        verbose (bool, optional): whether to print output. Defaults to False.
+        `verbose` (bool, optional): verbosity of class. Defaults to False.
+    
+    ### Attributes
+    - `capacity` (float): maximum amount of liquid that can be held
+    - `channel` (int): channel id
+    - `connection_details` (dict): dictionary of connection details (e.g. COM port / IP address)
+    - `device` (Callable): device object that communicates with physical tool
+    - `flags` (dict[str, bool]): keywords paired with boolean flags
+    - `reagent` (str): name of reagent held in liquid handler
+    - `speed` (Speed): up and down speeds of liquid handler
+    - `verbose` (bool): verbosity of class
+    
+    ### Properties
+    - `offset` (np.ndarray): liquid handler offset
+    - `volume` (float): volume held in liquid handler
+    
+    ### Methods
+    #### Abstract
+    - `aspirate`: aspirate desired volume of reagent
+    - `blowout`: blowout liquid from tip
+    - `dispense`: dispense desired volume of reagent
+    - `pullback`: pullback liquid from tip
+    - `_connect`: connection procedure for tool
+    #### Public
+    - `connect`: establish connection with device
+    - `cycle`: cycle between aspirate and dispense
+    - `disconnect`: disconnect from device
+    - `empty`: empty the channel
+    - `fill`: fill the channel
+    - `isBusy`: checks and returns whether the device is busy
+    - `isConnected`: checks and returns whether the device is connected
+    - `resetFlags`: reset all flags to class attribute `_default_flags`
+    - `rinse`: rinse the channel with aspirate and dispense cycles
+    - `setFlag`: set flags by using keyword arguments
+    - `shutdown`: shutdown procedure for tool
     """
-    def __init__(
-        self, 
-        capacity, 
-        channel, 
-        offset=None, 
-        pullback_time=PULLBACK_TIME, 
-        default_speed=DEFAULT_SPEED,
-        calibration_aspirate=CALIBRATION_ASPIRATE,
-        calibration_dispense=CALIBRATION_DISPENSE, 
-        **kwargs
-    ):
-        super().__init__(**kwargs)
-        self.capacity = capacity
-        self.channel = channel
-        if offset is None:
-            offset = (0,0,0)
-        self.offset = tuple(offset)
-        
-        self.pump = None
-        
-        self.calibration_aspirate = calibration_aspirate
-        self.calibration_dispense = calibration_dispense
-        self._previous_action = 'first'
-        self._pullback_time = pullback_time
-        self._speed_in = default_speed
-        self._speed_out = default_speed
-        pass
     
-    def aspirate(self, volume, speed=None, wait=0, reagent='', pause=False, channel=None):
+    _default_flags: dict[str, bool] = {'busy': False, 'connected': False}
+    def __init__(self, verbose:bool = False, **kwargs):
         """
-        Aspirate desired volume of reagent into channel
+        Instantiate the class
 
         Args:
-            volume (int, or float): volume to be aspirated
-            speed (int, optional): speed to aspirate. Defaults to None.
-            wait (int, optional): wait time between steps in seconds. Defaults to 0.
-            reagent (str, optional): name of reagent. Defaults to ''.
-            pause (bool, optional): whether to pause for intervention / operator input. Defaults to False.
-            channel (int, optional): channel to aspirate. Defaults to None.
-        """
-        if speed is None:
-            speed = self.speed['in']
-        self.pump.setFlag('busy', True)
-        volume = min(volume, self.capacity - self.volume)
-
-        if volume != 0:
-            speed = -abs(speed)
-            t_aspirate = (volume / speed) * self.calibration_aspirate
-            if self._previous_action == 'first':
-                t_aspirate *= 1.3
-            elif self._previous_action == 'aspirate':
-                t_aspirate *= 1
-            elif self._previous_action == 'dispense':
-                t_aspirate *= 1.6
-            print(t_aspirate)
-            t_pullback = (50 / speed) * self.calibration_aspirate
-            print(f'Aspirate {volume} uL')
-            self.pump.push(speed=speed, push_time=t_aspirate, pullback_time=t_pullback, channel=self.channel)
-            
-            # Update values
-            self._previous_action = 'aspirate'
-            self.volume += volume
-            if len(reagent) and len(self.reagent) == 0:
-                self.reagent = reagent
+            verbose (bool, optional): verbosity of class. Defaults to False.
+        """
+        self.capacity = 0
+        self.channel = 0
+        self.reagent = ''
+        self.speed = Speed(0,0)
+        self._volume = 0
+        self._offset = (0,0,0)
         
-        time.sleep(wait)
-        self.pump.setFlag('busy', False)
-        if pause:
-            input("Press 'Enter to proceed.")
+        self.connection_details = {}
+        self.device = None
+        self.flags = self._default_flags.copy()
+        self.verbose = verbose
+        return
+
+    def __del__(self):
+        self.shutdown()
         return
     
-    def dispense(self, volume, speed=None, wait=0, force_dispense=False, pause=False, channel=None):
+    @abstractmethod
+    def aspirate(self, 
+        volume: float, 
+        speed: Optional[float] = None, 
+        wait: int = 0, 
+        pause: bool = False, 
+        reagent: Optional[str] = None, 
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> bool:
         """
-        Aspirate desired volume of reagent into channel
+        Aspirate desired volume of reagent
 
         Args:
-            volume (int, or float): volume to be dispensed
-            speed (int, optional): speed to dispense. Defaults to None.
-            wait (int, optional): wait time between steps in seconds. Defaults to 0.
-            force_dispense (bool, optional): whether to continue dispensing even if insufficient volume in channel. Defaults to False.
-            pause (bool, optional): whether to pause for intervention / operator input. Defaults to False.
-            pump (Pump, optional): pump object. Defaults to None.
-            channel (int, optional): channel to dispense. Defaults to None.
-            
-        Raises:
-            Exception: Required dispense volume is greater than volume in tip
+            volume (float): target volume
+            speed (Optional[float], optional): speed to aspirate at. Defaults to None.
+            wait (int, optional): time delay after aspirate. Defaults to 0.
+            pause (bool, optional): whether to pause for user intervention. Defaults to False.
+            reagent (Optional[str], optional): name of reagent. Defaults to None.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
+
+        Returns:
+            bool: whether the action is successful
         """
-        if speed is None:
-            speed = self.speed['out']
-        self.pump.setFlag('busy', True)
-        if force_dispense:
-            volume = min(volume, self.volume)
-        elif volume > self.volume:
-            raise Exception('Required dispense volume is greater than volume in tip')
-        
-        if force_dispense or volume <= self.volume:
-            speed = abs(speed)
-            t_dispense = (volume / speed) * self.calibration_dispense
-            if self._previous_action == 'first':
-                t_dispense *= 1
-            elif self._previous_action == 'aspirate':
-                t_dispense *= 1.55
-            elif self._previous_action == 'dispense':
-                t_dispense *= 1
-            print(t_dispense)
-            t_pullback = (50 / speed) * self.calibration_dispense
-            self.pump.push(speed=speed, push_time=t_dispense, pullback_time=t_pullback, channel=self.channel)
-            
-            # Update values
-            self._previous_action = 'dispense'
-            self.volume = max(self.volume - volume, 0)
-        
-        time.sleep(wait)
-        self.pump.setFlag('busy', False)
-        if pause:
-            input("Press 'Enter to proceed.")
-        return
     
-    def pullback(self, channel=None):
+    @abstractmethod
+    def blowout(self, channel: Optional[Union[int, tuple[int]]] = None, **kwargs) -> bool:
         """
-        Pullback liquid from tip
+        Blowout liquid from tip
 
         Args:
-            channel (int, optional): channel to pullback. Defaults to None.
+            channel (Optional[Union[int, tuple[int]], optional): channel id. Defaults to None.
+            
+        Returns:
+            bool: whether the action is successful
         """
-        self.pump.setFlag('busy', True)
-        self.pump.push(speed=-300, push_time=0, pullback_time=self._pullback_time, channel=self.channel)
-        self.pump.setFlag('busy', False)
-        return
+        return False
     
-    def update(self, field:str, value):
+    @abstractmethod
+    def dispense(self, 
+        volume: float, 
+        speed: Optional[float] = None, 
+        wait: int = 0, 
+        pause: bool = False, 
+        blowout: bool = False,
+        force_dispense: bool = False, 
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> bool:
         """
-        Update the desired attribute
+        Dispense desired volume of reagent
 
         Args:
-            field (str): name of attribute
-            value (any): new value of attribute
+            volume (float): target volume
+            speed (Optional[float], optional): speed to dispense at. Defaults to None.
+            wait (int, optional): time delay after dispense. Defaults to 0.
+            pause (bool, optional): whether to pause for user intervention. Defaults to False.
+            blowout (bool, optional): whether perform blowout. Defaults to False.
+            force_dispense (bool, optional): whether to dispense reagent regardless. Defaults to False.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
+
+        Returns:
+            bool: whether the action is successful
         """
-        attrs = ['reagent', 'volume', '_previous_action']
-        if field not in attrs:
-            print(f"Select a field from: {', '.join(attrs)}")
-        else:
-            setattr(self, field, value)
-        return
 
+    @abstractmethod
+    def pullback(self, channel: Optional[Union[int, tuple[int]]] = None, **kwargs) -> bool:
+        """
+        Pullback liquid from tip
 
-class SyringeAssembly(LiquidHandler):
-    """
-    SyringeAssembly consisting of a pump and syringe(s)
+        Args:
+            channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
+            
+        Returns:
+            bool: whether the action is successful
+        """
+        return False
 
-    Args:
-        port (str): com port address
-        capacities (list, optional): list of syringe capacities. Defaults to [].
-        channels (list, optional): list of syringe channels. Defaults to [].
-        offsets (list, optional): list of syringe offsets. Defaults to [].
+    @abstractmethod
+    def _connect(self):
+        """Connection procedure for tool"""
+        self.connection_details = {}
+        self.device = None
+        self.setFlag(connected=True)
+        return
+
+    # Properties
+    @property
+    def offset(self) -> np.ndarray:
+        return np.array(self._offset)
+    @offset.setter
+    def offset(self, value:tuple[float]):
+        if len(value) != 3:
+            raise Exception('Please input x,y,z offset')
+        self._offset = tuple(value)
+        return
     
-    Kwargs:
-        verbose (bool, optional): whether to print output. Defaults to False.
-    """
-    def __init__(self, port:str, capacities=[], channels=[], offsets=[], **kwargs):
-        super().__init__(**kwargs)
-        self.pump = Peristaltic(port)
-        properties = Helper.zip_inputs('channel', capacity=capacities, channel=channels, offset=offsets)
-        self.channels = {key: Syringe(**value) for key,value in properties.items()}
-        for syringe in self.channels.values():
-            syringe.pump = self.pump
+    @property
+    def volume(self) -> float:
+        return self._volume
+    @volume.setter
+    def volume(self, value:float):
+        self._volume = value
         return
     
-    def aspirate(self, volume, speed=None, wait=0, reagent='', pause=False, channel=None):
+    def connect(self):
+        """Establish connection with device"""
+        return self._connect(**self.connection_details)
+    
+    def cycle(self, 
+        volume: float, 
+        speed: Optional[float] = None, 
+        wait: int = 0,  
+        cycles: int = 1,
+        reagent: Optional[str] = None, 
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> bool:
         """
-        Aspirate desired volume of reagent into channel
+        Cycle between aspirate and dispense
 
         Args:
-            volume (int, or float): volume to be aspirated
-            speed (int, optional): speed to aspirate. Defaults to None.
-            wait (int, optional): wait time between steps in seconds. Defaults to 0.
-            reagent (str, optional): name of reagent. Defaults to ''.
-            pause (bool, optional): whether to pause for intervention / operator input. Defaults to False.
-            channel (int, optional): channel to aspirate. Defaults to None.
-        
-        Raises:
-            Exception: Select a valid key
-        """
-        if channel not in self.channels.keys():
-            raise Exception(f"Select a valid key from: {', '.join(self.channels.keys())}")
-        return self.channels[channel].aspirate(volume=volume, speed=speed, wait=wait, reagent=reagent, pause=pause)
+            volume (float): target volume
+            speed (Optional[float], optional): speed to aspirate and dispense at. Defaults to None.
+            wait (int, optional): time delay after each action. Defaults to 0.
+            cycles (int, optional): number of cycles. Defaults to 1.
+            reagent (Optional[str], optional): name of reagent. Defaults to None.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
 
-    def connect(self):
-        """
-        Reconnect to device using existing port and baudrate
-        
         Returns:
-            serial.Serial: serial connection to machine control unit if connection is successful, else None
+            bool: whether the action is successful
         """
-        return self.pump.connect()
+        success = []
+        for _ in range(cycles):
+            ret1 = self.aspirate(volume=volume, speed=speed, wait=wait, pause=False, reagent=reagent, channel=channel)
+            ret2 = self.dispense(volume=volume, speed=speed, wait=wait, pause=False, force_dispense=True, channel=channel)
+            success.extend([ret1,ret2])
+        return all(success)
     
-    def dispense(self, volume, speed=None, wait=0, force_dispense=False, pause=False, channel=None):
-        """
-        Aspirate desired volume of reagent into channel
-
-        Args:
-            volume (int, or float): volume to be dispensed
-            speed (int, optional): speed to dispense. Defaults to None.
-            wait (int, optional): wait time between steps in seconds. Defaults to 0.
-            force_dispense (bool, optional): whether to continue dispensing even if insufficient volume in channel. Defaults to False.
-            pause (bool, optional): whether to pause for intervention / operator input. Defaults to False.
-            channel (int, optional): channel to dispense. Defaults to None.
-        
-        Raises:
-            Exception: Select a valid key
-        """
-        if channel not in self.channels.keys():
-            raise Exception(f"Select a valid key from: {', '.join(self.channels.keys())}")
-        return self.channels[channel].dispense(volume=volume, speed=speed, wait=wait, force_dispense=force_dispense, pause=pause)
- 
-    def empty(self, speed=None, wait=0, pause=False, channel:list=[]):
+    def disconnect(self):
+        """Disconnect from device"""
+        try:
+            self.device.close()
+        except Exception as e:
+            if self.verbose:
+                print(e)
+        self.setFlag(connected=False)
+        return
+    
+    def empty(self, 
+        speed: Optional[float] = None, 
+        wait: int = 0, 
+        pause: bool = False, 
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> bool:
         """
-        Empty multiple channels
+        Empty the channel
 
         Args:
-            speed (int, optional): speed to empty. Defaults to None.
+            speed (Optional[float], optional): speed to empty. Defaults to None.
             wait (int, optional): wait time between steps in seconds. Defaults to 0.
-            pause (bool, optional): whether to pause for intervention / operator input. Defaults to False.
-            channel (list, optional): channel to empty. Defaults to None.
-        
-        Raises:
-            Exception: Select a valid key
-        
+            pause (bool, optional): whether to pause for user intervention. Defaults to False.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
+            
         Returns:
-            dict: dictionary of (channel, return value)
+            bool: whether the action is successful
         """
-        if len(channel) == 0: # all channels instead
-            channel = list(self.channels.keys())
-        
-        return_values = {}
-        for chn in channel:
-            if chn not in self.channels.keys():
-                raise Exception(f"Select a valid key from: {', '.join(self.channels.keys())}")
-            return_values[chn] = self.channels[channel].empty(speed=speed, wait=wait, pause=pause)
-        return return_values
-
-    def fill(self, speed=None, wait=0, reagents='', pause=False, pre_wet=True, channel:list=[]):
+        ret1 = self.dispense(volume=self.capacity, speed=speed, wait=wait, pause=pause, force_dispense=True, channel=channel)
+        ret2 = self.blowout(channel=channel)
+        return all([ret1,ret2])
+    
+    def fill(self, 
+        speed: Optional[float] = None, 
+        wait: int = 0, 
+        pause: bool = False, 
+        cycles: int = 1,
+        reagent: Optional[str] = None, 
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> bool:
         """
-        Fill multiple channels
+        Fill the channel
 
         Args:
-            speed (int, optional): speed to fill. Defaults to None.
-            wait (int, optional): wait time between steps in seconds. Defaults to 0.
-            reagents (list, optional): name of reagent. Defaults to [''].
-            pause (bool, optional): whether to pause for intervention / operator input. Defaults to False.
-            pre_wet (bool, optional): whether to pre-wet the channel. Defaults to True.
-            channel (list, optional): channel to fill. Defaults to [].
-        
-        Raises:
-            Exception: Select a valid key
+            speed (Optional[float], optional): speed to aspirate and dispense at. Defaults to None.
+            wait (int, optional): time delay after each action. Defaults to 0.
+            pause (bool, optional): whether to pause for user intervention. Defaults to False.
+            cycles (int, optional): number of cycles. Defaults to 1.
+            reagent (Optional[str], optional): name of reagent. Defaults to None.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
         
         Returns:
-            dict: dictionary of (channel, return value)
+            bool: whether the action is successful
         """
-        if len(channel) == 0: # all channels instead
-            channel = list(self.channels.keys())
-        
-        return_values = {}
-        for chn in channel:
-            if chn not in self.channels.keys():
-                raise Exception(f"Select a valid key from: {', '.join(self.channels.keys())}")
-            return_values[chn] = self.channels[channel].fill(speed=speed, wait=wait, reagent=reagents, pause=pause, pre_wet=pre_wet)
-        return return_values
-
-    def isBusy(self):
+        ret1 = self.cycle(volume=self.capacity, speed=speed, wait=wait, cycles=cycles, reagent=reagent, channel=channel)
+        ret2 = self.aspirate(volume=self.capacity, speed=speed, wait=wait, pause=pause, reagent=reagent, channel=channel)
+        ret3 = self.pullback(channel=channel)
+        return all([ret1,ret2,ret3])
+    
+    def isBusy(self) -> bool:
         """
-        Checks whether the pump is busy
+        Checks and returns whether the device is busy
         
         Returns:
-            bool: whether the pump is busy
+            bool: whether the device is busy
         """
-        return self.pump.isBusy()
+        return self.flags.get('busy', False)
     
-    def isConnected(self):
+    def isConnected(self) -> bool:
         """
-        Check whether pump is connected
+        Checks and returns whether the device is connected
 
         Returns:
-            bool: whether pump is connected
-        """
-        return self.pump.isConnected()
-
-    def pullback(self, channel:list=[]):
-        """
-        Pullback liquid from tip for multiple channels
-
-        Raises:
-            Exception: Select a valid key
-        
-        Args:
-            channel (int, optional): channel to pullback
+            bool: whether the device is connected
         """
-        if len(channel) == 0: # all channels instead
-            channel = list(self.channels.keys())
-        for chn in channel:
-            if chn not in self.channels.keys():
-                raise Exception(f"Select a valid key from: {', '.join(self.channels.keys())}")
-            self.channels[chn].pullback()
+        if not self.flags.get('connected', False):
+            if self.verbose:
+                print(f"{self.__class__} is not connected. Details: {self.connection_details}")
+        return self.flags.get('connected', False)
+
+    def resetFlags(self):
+        """Reset all flags to class attribute `_default_flags`"""
+        self.flags = self._default_flags.copy()
         return
     
-    def rinseMany(self, volume, speed=None, wait=0, reagents='', cycles=3, channel:list=[]):
+    def rinse(self, 
+        speed: Optional[float] = None, 
+        wait: int = 0, 
+        cycles: int = 3, 
+        channel: Optional[Union[int, tuple[int]]] = None,
+        **kwargs
+    ) -> bool:
         """
-        Rinse multiple channels
-
+        Rinse the channel with aspirate and dispense cycles
+        
         Args:
-            volume (int, or float): volume to be rinsed
-            speed (int, optional): speed to cycle. Defaults to None.
-            wait (int, optional): wait time between steps in seconds. Defaults to 0.
-            reagent (list, optional): name of reagent. Defaults to [''].
-            cycles (int, optional): number of cycles to perform. Defaults to 3.
-            channel (list, optional): channel to cycle. Defaults to [].
-
-        Raises:
-            Exception: Select a valid key
+            speed (Optional[float], optional): speed to aspirate and dispense at. Defaults to None.
+            wait (int, optional): time delay after each action. Defaults to 0.
+            cycles (int, optional): number of cycles. Defaults to 1.
+            channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
 
         Returns:
-            dict: dictionary of (channel, return value)
+            bool: whether the action is successful
         """
-        if len(channel) == 0: # all channels instead
-            channel = list(self.channels.keys())
-        
-        return_values = {}
-        for chn in channel:
-            if chn not in self.channels.keys():
-                raise Exception(f"Select a valid key from: {', '.join(self.channels.keys())}")
-            return_values[chn] = self.channels[channel].rinse(volume=volume, speed=speed, wait=wait, reagent=reagents, cycles=cycles)
-        return return_values
+        return self.cycle(volume=self.capacity, speed=speed, wait=wait, cycles=cycles, channel=channel)
     
-    def update(self, field, value, channel):
+    def setFlag(self, **kwargs):
         """
-        Update the desired channel attribute
+        Set flags by using keyword arguments
 
-        Args:
-            field (str): name of attribute
-            value (any): new value of attribute
-            channel (int): channel to update
+        Kwargs:
+            key, value: (flag name, boolean) pairs
         """
-        return self.channels[channel].update(field, value)
+        if not all([type(v)==bool for v in kwargs.values()]):
+            raise ValueError("Ensure all assigned flag values are boolean.")
+        for key, value in kwargs.items():
+            self.flags[key] = value
+        return
+
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        self.disconnect()
+        self.resetFlags()
+        return
+
+    # Protected method(s)
+    def _diagnostic(self):
+        """Run diagnostic test"""
+        self.pullback()
+        return
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,85 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/1 13:20:00
-@author: Chang Jie
+This module holds the base class for image classifiers
+and the class for cascade classifiers.
 
-Notes / actionables:
-- validation on copper 
-- rewrite the operation modes as programs, instead of subclasses
+Classes:
+    Classifier (ABC)
+    CascadeClassifier (Classifier)
 """
+# Standard library imports
+from abc import ABC, abstractmethod
+
 # Third party imports
 import cv2 # pip install opencv-python
 
 # Local application imports
 from ..image_utils import Image
 print(f"Import: OK <{__name__}>")
 
-class Classifier(object):
+class Classifier(ABC):
     """
-    Classifier object
+    Abstract Base Class (ABC) for Classifier objects (i.e. models that can detect image targets).
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
+    
+    ### Attributes
+    - `classifier` (Callable): image classifier model
+    
+    ### Methods
+    #### Abstract
+    - `detect`: detect image targets
     """
+    
     def __init__(self):
+        """Instantiate the class"""
+        self.classifier = None
         pass
     
-    def detect(self, image:Image, scale:int, neighbors:int):
+    @abstractmethod
+    def detect(self, image:Image, scale:int, neighbors:int) -> dict:
         """
-        Detect targets
+        Detect image targets
 
         Args:
             image (Image): image to detect from
             scale (int): scale at which to detect targets
             neighbors (int): minimum number of neighbors for targets
 
         Returns:
             dict: dictionary of detected targets
         """
-        return
 
 class CascadeClassifier(Classifier):
+    """
+    Abstract Base Class (ABC) for Classifier objects (i.e. models that can detect image targets).
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
+    
+    ### Constructor
+    Args:
+        `xml_path` (str): filepath of trained cascade xml file
+    
+    ### Methods
+    #### Abstract
+    - `detect`: detect image targets
+    """
+    
     def __init__(self, xml_path:str):
         """
         Cascade classifier object
 
         Args:
             xml_path (str): filepath of trained cascade xml file
         """
         self.classifier = cv2.CascadeClassifier(xml_path)
         pass
     
-    def detect(self, image:Image, scale:int, neighbors:int):
+    def detect(self, image:Image, scale:int, neighbors:int) -> dict:
         """
-        Detect targets
+        Detect image targets
 
         Args:
             image (Image): image to detect from
             scale (int): scale at which to detect targets
             neighbors (int): minimum number of neighbors for targets
 
         Returns:
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.0.0a0/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-0.0.4.1/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/View/Thermal/thermal_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,95 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/1 13:20:00
-@author: Chang Jie
+This module holds the class for thermal cameras.
 
-Notes / actionables:
-- 
+Classes:
+    Thermal (Camera)
 """
 # Standard library imports
-import pkgutil
+from __future__ import annotations
+import numpy as np
 
 # Local application imports
 from ..view_utils import Camera
 from .Flir.ax8 import Ax8ThermalCamera
 print(f"Import: OK <{__name__}>")
 
 class Thermal(Camera):
     """
     Thermal camera object
 
+    ### Constructor
     Args:
-        ip_address (str): IP address of thermal camera
-        calibration_unit (int, optional): calibration of pixels to mm. Defaults to 1.
-        cam_size (tuple, optional): width and height of image. Defaults to (640,480).
-        rotation (int, optional): rotation of camera feed. Defaults to 0.
+        `ip_address` (str): IP address of thermal camera
+        `calibration_unit` (float, optional): calibration from pixels to mm. Defaults to 1.
+        `cam_size` (tuple[int], optional): (width, height) of camera output. Defaults to (640,480).
+        `rotation` (int, optional): rotation angle for camera feed. Defaults to 180.
+    
+    ### Properties
+    - `ip_address` (str): IP address of thermal camera
+    
+    ### Methods
+    - `disconnect`: disconnect from camera
     """
-    def __init__(self, ip_address:str, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.ip_address = ip_address
-        self.rotation = 180
-        self._connect()
-        
-        img_bytes = pkgutil.get_data(__name__, 'placeholders/infrared_camera.png')
-        self._set_placeholder(img_bytes=img_bytes)
+    _package = __name__
+    _placeholder_filename = 'placeholders/infrared_camera.png'
+    def __init__(self, 
+        ip_address:str, 
+        calibration_unit: float = 1, 
+        cam_size: tuple[int] = (640,480), 
+        rotation:int = 180, 
+        **kwargs
+    ):
+        """
+        Instantiate the class
+
+        Args:
+            ip_address (str): IP address of thermal camera
+            calibration_unit (float, optional): calibration from pixels to mm. Defaults to 1.
+            cam_size (tuple[int], optional): (width, height) of camera output. Defaults to (640,480).
+            rotation (int, optional): rotation angle for camera feed. Defaults to 180.
+        """
+        super().__init__(calibration_unit=calibration_unit, cam_size=cam_size, rotation=rotation, **kwargs)
+        self._connect(ip_address)
+        return
+    
+    # Properties
+    @property
+    def ip_address(self) -> str:
+        return self.connection_details.get('ip_address', '')
+
+    def disconnect(self):
+        """Disconnect from camera"""
+        try:
+            self.feed.stop()
+            self.feed.stream.release()
+        except AttributeError:
+            pass
+        self.setFlag(connected=False)
         return
     
-    def _connect(self):
+    # Protected method(s)
+    def _connect(self, ip_address:str, **kwargs):
         """
-        Connect to the imaging device
+        Connection procedure for tool
+        
+        Args:
+            ip_address (str): IP address of thermal camera
         """
-        self.device = Ax8ThermalCamera(self.ip_address, verbose=True)
+        self.connection_details['ip_address'] = ip_address
+        self.device = Ax8ThermalCamera(ip_address, verbose=True)
         # if self.device.modbus.is_open:
         if True:
             self.feed = self.device.video.stream
-            self._flags['isConnected'] = True
+            self.setFlag(connected=True)
         return
     
-    def _read(self):
+    def _read(self) -> tuple[bool, np.ndarray]:
         """
-        Read camera feed
+        Read camera feed to retrieve image
 
         Returns:
-            bool, array: True if frame is obtained; array of frame
+            tuple[bool, np.ndarray]: (whether frame is obtained, frame array)
         """
         return True, self.feed.read()
-    
-    def _release(self):
-        """
-        Release the camera feed
-        """
-        self.feed.stop()
-        self.feed.stream.release()
-        return
-    
+
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/misc/decorators.py` & `control-lab-ly-1.0.0a0/src/controllably/misc/decorators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,69 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/02 17:13:35
-@author: Chang Jie
+This module holds the decorator functions in Control.lab.ly.
 
-Notes / actionables:
--
+Functions:
+    named_tuple_from_dict (decorator)
+    safety_measures (decorator)
 """
 # Standard library imports
 from collections import namedtuple
+from functools import wraps
 import time
-
-# Third party imports
-
-# Local application imports
+from typing import Callable, Optional
 print(f"Import: OK <{__name__}>")
 
-def named_tuple_from_dict(func):
+def named_tuple_from_dict(func:Callable) -> Callable:
     """
     Wrapper for creating named tuple from dictionary
 
     Args:
         func (Callable): function to be wrapped
+        
+    Returns:
+        Callable: wrapped function
     """
-    def wrapper(*args, **kwargs):
+    @wraps(func)
+    def wrapper(*args, **kwargs) -> tuple:
         setup_dict = func(*args, **kwargs)
         field_list = []
         object_list = []
         for k,v in setup_dict.items():
             field_list.append(k)
             object_list.append(v)
         
         Setup = namedtuple('Setup', field_list)
         print(f"Objects created: {', '.join(field_list)}")
         return Setup(*object_list)
     return wrapper
 
-def safety_measures(mode=None, countdown=3):
+def safety_measures(mode:Optional[str] = None, countdown:int = 3) -> Callable:
     """
     Wrapper for creating safe move functions
 
     Args:
-        func (Callable): function to be wrapped
-        mode (str, optional): mode for implementing safety measure. Defaults to None.
+        mode (Optional[str], optional): mode for implementing safety measure. Defaults to None.
+        countdown (int, optional): time delay before executing action. Defaults to 3.
+        
+    Returns:
+        Callable: wrapped function
     """
-    def inner(func):
-        def wrapper(*args, **kwargs):
+    def inner(func:Callable) -> Callable:
+        """
+        Inner wrapper for creating safe move functions
+
+        Args:
+            func (Callable): function to be wrapped
+
+        Returns:
+            Callable: wrapped function
+        """
+        @wraps(func)
+        def wrapper(*args, **kwargs) -> Callable:
             str_method = repr(func).split(' ')[1]
             str_args = ','.join([repr(a) for a in args[1:]])
             str_kwargs = ','.join([f'{k}={v}' for k,v in kwargs.items()])
             str_inputs = ','.join(filter(None, [str_args, str_kwargs]))
             str_call = f"{str_method}({str_inputs})"
             if mode == 'wait':
                 print(f"Executing in {countdown} seconds:")
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.0.0a0/src/controllably/View/view_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,509 +1,486 @@
 # %% -*- coding: utf-8 -*-
 """
-Created: Tue 2022/11/02 17:13:35
-@author: Chang Jie
+This module holds the base class for camera tools.
 
-Notes / actionables:
--
+Classes:
+    Camera (ABC)
+
+Other constants and variables:
+    DIMENSION_THRESHOLD (int)
+    ROW_DISTANCE (int)
 """
 # Standard library imports
+from __future__ import annotations
+from abc import ABC, abstractmethod
 from datetime import datetime
-import importlib
-import json
 import numpy as np
-import os
 import pandas as pd
-from pathlib import Path
 import pkgutil
-from shutil import copytree
-import time
-import uuid
+from threading import Thread
+from typing import Optional, Protocol
 
 # Third party imports
-import serial.tools.list_ports # pip install pyserial
-import yaml # pip install pyyaml
+import cv2              # pip install opencv-python
 
 # Local application imports
-from . import decorators
+from ..misc import Helper
+from .image_utils import Image
+# from . import image_utils as Image
 print(f"Import: OK <{__name__}>")
 
-here = str(Path(__file__).parent.absolute()).replace('\\', '/')
+DIMENSION_THRESHOLD = 36
+"""Minimum width in pixels of target for detection"""
+ROW_DISTANCE = 30
+"""Number of pixels between rows of detected targets"""
 
-class Helper(object):
-    """
-    Helper class with miscellaneous methods
+class Classifier(Protocol):
+    def detect(self, frame:np.ndarray, scale:int, neighbors:int, **kwargs) -> dict:
+        ...
+
+class Camera(ABC):
     """
-    def __init__(self):
-        self.safety_countdown = 3
-        self.safety_mode = None
+    Abstract Base Class (ABC) for Camera objects (i.e. tools that capture images).
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
+    
+    ### Constructor
+    Args:
+        `calibration_unit` (float, optional): calibration from pixels to mm. Defaults to 1.
+        `cam_size` (tuple[int], optional): (width, height) of camera feed. Defaults to (640,480).
+        `rotation` (int, optional): rotation angle for camera feed. Defaults to 0.
+        `verbose` (bool, optional): verbosity of class. Defaults to False.
+    
+    ### Attributes
+    - `calibration_unit` (float): calibration from pixels to mm
+    - `cam_size` (tuple[int], optional): (width, height) of camera feed
+    - `classifier` (Classifier): image classifier object
+    - `connection_details` (dict): dictionary of connection details (e.g. COM port / IP address)
+    - `device` (Callable): device object that communicates with physical tool
+    - `feed` (Callable): connection to image feed
+    - `flags` (dict[str, bool]): keywords paired with boolean flags
+    - `placeholder_image` (Image): placeholder image for when there is no feed available
+    - `record_folder` (str): filepath at which to store images and data
+    - `record_timeout` (int): number of seconds to record images for
+    - `rotation` (int): rotation angle for camera feed (multiples of 90 degrees)
+    - `verbose` (bool): verbosity of class
+    
+    ### Methods
+    #### Abstract
+    - `disconnect`: disconnect from device
+    - `_connect`: connection procedure for tool
+    - `_read`: read camera feed to retrieve image
+    #### Public
+    - `annotateAll`: annotate all detected targets
+    - `connect`: establish connection with device
+    - `decodeImage`: decode byte array of image
+    - `detect`: perform image detection
+    - `encodeImage`: encode image into byte array
+    - `getImage`: retrieve image from camera feed
+    - `isConnected`: checks and returns whether the device is connected
+    - `loadClassifier`: load the desired image classifier
+    - `loadImage`: load an image from file
+    - `resetFlags`: reset all flags to class attribute `_default_flags`
+    - `saveImage`: save image to file
+    - `setFlag`: set flags by using keyword arguments
+    - `shutdown`: shutdown procedure for tool
+    - `toggleRecord`: start or stop data recording
+    """
+    
+    _default_flags: dict[str, bool] = {
+        'connected': False,
+        'pause_record': False,
+        'record': False
+    }
+    _package: str
+    _placeholder_filename: str
+    def __init__(self, 
+        calibration_unit: float = 1, 
+        cam_size: tuple[int] = (640,480), 
+        rotation: int = 0,
+        verbose: bool = False,
+        **kwargs
+    ):
+        """
+        Instantiate the class
+
+        Args:
+            calibration_unit (float, optional): calibration from pixels to mm. Defaults to 1.
+            cam_size (tuple[int], optional): (width, height) of camera output. Defaults to (640,480).
+            rotation (int, optional): rotation angle for camera feed. Defaults to 0.
+            verbose (bool, optional): verbosity of class. Defaults to False.
+        """
+        self.calibration_unit = calibration_unit
+        self.cam_size = cam_size
+        self.classifier = None
+        self.connection_details = {}
+        self.device = None
+        self.feed = None
+        self.placeholder_image = None
+        self.record_folder = ''
+        self.record_timeout = None
+        self.rotation = rotation
+        
+        self.flags = self._default_flags.copy() 
+        self.verbose = verbose
+        self._threads = {}
+        self._set_placeholder()
         pass
     
-    # Static methods
-    @staticmethod
-    def create_folder(parent_folder:str = None, child_folder:str = None):
-        """
-        Check and create folder if it does not exist
-
-        Args:
-            parent_folder (str, optional): parent folder directory. Defaults to None.
-            child_folder (str, optional): child folder directory. Defaults to None.
-        """
-        main_folder = datetime.now().strftime("%Y-%m-%d_%H%M")
-        if parent_folder:
-            main_folder = '/'.join([parent_folder, main_folder])
-        folder = '/'.join([main_folder, child_folder]) if child_folder else main_folder
-        if not os.path.exists(folder):
-            os.makedirs(folder)
-        return main_folder
+    def __del__(self):
+        self.shutdown()
+        return
     
-    @staticmethod
-    def get_class(module, dot_notation:str):
+    @abstractmethod
+    def disconnect(self):
+        """Disconnect from device"""
+        self.setFlag(connected=False)
+    
+    @abstractmethod
+    def _connect(self, *args, **kwargs):
+        """Connection procedure for tool"""
+        self.connection_details = {}
+        self.device = None
+        self.setFlag(connected=True)
+        return
+   
+    @abstractmethod
+    def _read(self) -> tuple[bool, np.ndarray]:
         """
-        Retrieve the relevant class from the sub-package
-
-        Args:
-            module (module): sub-package
-            dot_notation (str): dot notation of class / module / package
+        Read camera feed to retrieve image
 
         Returns:
-            class: relevant class
+            tuple[bool, np.ndarray]: (whether frame is obtained, frame array)
         """
-        print('\n')
-        top_package = __name__.split('.')[0]
-        import_path = f'{top_package}.{module}.{dot_notation}'
-        package = importlib.import_module('.'.join(import_path.split('.')[:-1]))
-        _class = getattr(package, import_path.split('.')[-1])
-        return _class
-        
-    @staticmethod
-    def get_method_names(obj):
+    
+    def annotateAll(self, 
+        df: pd.DataFrame, 
+        image: Optional[Image] = None, 
+        frame: Optional[np.ndarray] = None    
+    ) -> tuple[dict[str,tuple[int]], Image]:
         """
-        Get the names of the methods in object (class/instance)
+        Annotate all detected targets
 
         Args:
-            obj (any): object of interest
+            df (pd.DataFrame): dataframe of detected targets details
+            image (Optional[Image], optional): image object. Defaults to None.
+            frame (Optional[np.ndarray], optional): frame array. Defaults to None.
 
         Returns:
-            list: list of method names
-        """
-        method_list = []
-        # attribute is a string representing the attribute name
-        for attribute in dir(obj):
-            # Get the attribute value
-            attribute_value = getattr(obj, attribute)
-            # Check that it is callable; Filter all dunder (__ prefix) methods
-            if callable(attribute_value) and not attribute.startswith('__'):
-                method_list.append(attribute)
-        return method_list
-    
-    @staticmethod
-    def get_node():
+            tuple[dict[str,tuple[int]], Image]: ({target index: center positions}, image object)
         """
-        Display the machine's unique identifier
+        data = {}
+        if (frame is None) == (image is None):
+            raise Exception('Please input either image or frame.')
+        elif frame is not None:
+            image = Image(frame)
+            
+        for index in range(len(df)):
+            dimensions = df.loc[index, ['x','y','w','h']].to_list()
+            x,y,w,h = dimensions
+            if w*h >= DIMENSION_THRESHOLD**2:                       # Compare area to threshold
+                image.annotate(index, (x,y,w,h), inplace=True)
+                data[f'C{index+1}'] = (int(x+(w/2)), int(y+(h/2)))  # Center of target
+        return data, image
+    
+    def connect(self):
+        """Establish connection with device"""
+        return self._connect(**self.connection_details)
+
+    def detect(self, image:Image, scale:int, neighbors:int) -> pd.DataFrame:
+        """
+        Perform image detection
+
+        Args:
+            image (Image): image to detect from
+            scale (int): scale at which to detect targets
+            neighbors (int): minimum number of neighbors for targets
+
+        Raises:
+            RuntimeError: Please load a classifier first.
 
         Returns:
-            str: machine unique identifier
+            pd.DataFrame: dataframe of detected targets
         """
-        return str(uuid.getnode())
+        if self.classifier is None:
+            raise RuntimeError('Please load a classifier first.')
+        image.grayscale(inplace=True)
+        detected_data = self.classifier.detect(frame=image.frame, scale=scale, neighbors=neighbors)
+        return self._data_to_df(detected_data)
     
-    @staticmethod
-    def get_ports():
+    def isConnected(self) -> bool:
         """
-        Get available ports
+        Checks and returns whether the device is connected
 
         Returns:
-            list: list of connected serial ports
+            bool: whether the device is connected
         """
-        com_ports = []
-        ports = serial.tools.list_ports.comports()
-        for port, desc, hwid in sorted(ports):
-            com_ports.append(str(port))
-            print(f"{port}: {desc} [{hwid}]")
-        if len(ports) == 0:
-            print("No ports detected!")
-            return ['']
-        return com_ports
+        if not self.flags.get('connected', False):
+            print(f"{self.__class__} is not connected.")
+        return self.flags.get('connected', False)
     
-    @staticmethod
-    def is_overrun(start_time:float, timeout:float):
+    def loadClassifier(self, classifier:Classifier):
         """
-        Check whether the process has timed out
+        Load the desired image classifier
 
         Args:
-            start_time (float): start time in seconds since epoch
-            timeout (float): timeout duration
-
-        Returns:
-            bool: whether process has overrun
+            classifier (Classifier): desired image classifier
         """
-        if timeout!=None and time.time() - start_time > timeout:
-            return True
-        return False
+        # try:
+        self.classifier = classifier
+        # except SystemError:
+        #     print('Please select a classifier.')
+        return
+
+    def resetFlags(self):
+        """Reset all flags to class attribute `_default_flags`"""
+        self.flags = self._default_flags.copy()
+        return
     
-    @staticmethod
-    def pretty_print_duration(total_time:float):
+    def setFlag(self, **kwargs):
         """
-        Display time duration (s) as HH:MM:SS text
+        Set flags by using keyword arguments
 
-        Args:
-            total_time (float): duration in seconds
-
-        Returns:
-            str: formatted time string
+        Kwargs:
+            key, value: (flag name, boolean) pairs
         """
-        m, s = divmod(total_time, 60)
-        h, m = divmod(m, 60)
-        return f'{int(h)}hr {int(m)}min {int(s):02}sec'
+        if not all([type(v)==bool for v in kwargs.values()]):
+            raise ValueError("Ensure all assigned flag values are boolean.")
+        for key, value in kwargs.items():
+            self.flags[key] = value
+        return
+    
+    def shutdown(self):
+        """Shutdown procedure for tool"""
+        self.disconnect()
+        cv2.destroyAllWindows()
+        self.resetFlags()
+        return
     
-    @staticmethod
-    def read_json(json_file:str, package:str = None):
+    def toggleRecord(self, on:bool, folder:str = '', timeout:Optional[int] = None):
         """
-        Read JSON file
+        Start or stop image capture and recording
 
         Args:
-            json_file (str): JSON filepath
-            package (str, optional): name of package to look in. Defaults to None.
-
-        Returns:
-            dict: dictionary loaded from JSON file
+            on (bool): whether to start recording frames
+            folder (str, optional): folder to save to. Defaults to ''.
+            timeout (Optional[int], optional): number of seconds to record. Defaults to None.
         """
-        if package is not None:
-            jsn = pkgutil.get_data(package, json_file).decode('utf-8')
+        self.setFlag(record=on)
+        if on:
+            # Ensure only one record thread at a time
+            if 'record_loop' in self._threads:
+                self._threads['record_loop'].join()
+            
+            self.record_folder = folder
+            self.record_timeout = timeout
+            thread = Thread(target=self._loop_record)
+            thread.start()
+            self._threads['record_loop'] = thread
         else:
-            with open(json_file) as file:
-                jsn = file.read()
-        return json.loads(jsn)
-    
-    @staticmethod
-    def read_yaml(yaml_file:str, package:str = None):
+            self._threads['record_loop'].join()
+        return
+ 
+    # Image handling
+    def decodeImage(self, array:bytes) -> Image:
         """
-        Read YAML file
+        Decode byte array of image
 
         Args:
-            yaml_file (str): YAML filepath
-            package (str, optional): name of package to look in. Defaults to None.
+            array (bytes): byte array of image
 
         Returns:
-            dict: dictionary loaded from YAML file
+            Image: image of decoded byte array
         """
-        if package is not None:
-            yml = pkgutil.get_data(package, yaml_file).decode('utf-8')
-        else:
-            with open(yaml_file) as file:
-                yml = file.read()
-        return yaml.safe_load(yml)
+        frame = cv2.imdecode(array, cv2.IMREAD_COLOR)
+        return Image(frame)
     
-    @staticmethod
-    def zip_inputs(primary_keyword:str, **kwargs):
+    def encodeImage(self, 
+        image: Optional[Image] = None, 
+        frame: Optional[np.ndarray] = None, 
+        extension: str = '.png'
+    ) -> bytes:
         """
-        Checks and zips multiple keyword arguments of lists into dictionary
+        Encode image into byte array
 
         Args:
-            primary_keyword (str): primary keyword to be used as key
+            image (Optional[Image], optional): image object to be encoded. Defaults to None.
+            frame (Optional[np.ndarray], optional): frame array to be encoded. Defaults to None.
+            extension (str, optional): image format to encode to. Defaults to '.png'.
 
         Raises:
-            Exception: Inputs have to be of the same length
+            ValueError: Please input either image or frame.
 
         Returns:
-            dict: dictionary of (primary keyword, kwargs)
+            bytes: byte array of image / frame
         """
-        input_length = len(kwargs[primary_keyword])
-        keys = list(kwargs.keys())
-        for key, value in kwargs.items():
-            if type(value) != list:
-                if type(value) in [tuple, set]:
-                    kwargs[key] = list(value)
-                else:
-                    value = [value]
-                    kwargs[key] = value * input_length
-        if not all(len(kwargs[key]) == input_length for key in keys):
-            raise Exception(f"Ensure the lengths of these inputs are the same: {', '.join(keys)}")
-        kwargs_df = pd.DataFrame(kwargs)
-        kwargs_df.set_index(primary_keyword, drop=False, inplace=True)
-        return kwargs_df.to_dict('index')
+        if (frame is None) == (image is None):
+            raise ValueError('Please input either image or frame.')
+        elif image is not None:
+            return image.encode(extension)
+        return cv2.imencode(extension, frame)[1].tobytes()
     
-    # Class methods
-    @classmethod
-    def get_details(cls, configs:dict, addresses:dict = {}):
+    def getImage(self, 
+        crosshair: bool = False, 
+        resize: bool = False
+    ) -> tuple[bool, Image]:
         """
-        Decode dictionary of configuration details to get np.ndarrays and tuples
+        Get image from camera feed
 
         Args:
-            configs (dict): dictionary of configuration details
-            addresses (dict, optional): dictionary of registered addresses. Defaults to {}.
+            crosshair (bool, optional): whether to overlay crosshair on image. Defaults to False.
+            resize (bool, optional): whether to resize the image. Defaults to False.
 
         Returns:
-            dict: dictionary of configuration details
+            tuple[bool, Image]: (whether an image is obtained, image object)
         """
-        for name, details in configs.items():
-            settings = details.get('settings', {})
-            
-            for key,value in settings.items():
-                if key == 'component_config':
-                    value = cls.get_details(value, addresses=addresses)
-                if type(value) == str:
-                    if key in ['cam_index', 'port'] and value.startswith('__'):
-                        settings[key] = addresses.get(key, {}).get(settings[key], value)
-                if type(value) == dict:
-                    if "tuple" in value:
-                        settings[key] = tuple(value['tuple'])
-                    elif "array" in value:
-                        settings[key] = np.array(value['array'])
+        ret = False
+        image = self.placeholder_image
+        try:
+            ret, frame = self._read()
+        except AttributeError:
+            pass
+        if ret:
+            image = Image(frame)
+            if resize:
+                image.resize(self.cam_size, inplace=True)
+            image.rotate(self.rotation, inplace=True)
+        if crosshair:
+            image.crosshair(inplace=True)
+        return ret, image
 
-            configs[name] = details
-        return configs
-    
-    @classmethod
-    def get_machine_addresses(cls, registry:dict):
+    def loadImage(self, filename:str) -> Image:
         """
-        Get the appropriate addresses for current machine
+        Load image from file
 
         Args:
-            registry (str): dictionary of yaml file with com port addresses and camera ids
+            filename (str): image filename
 
         Returns:
-            dict: dictionary of com port addresses and camera ids for current machine
+            Image: image from file
         """
-        node_id = cls.get_node()
-        addresses = registry.get('machine_id',{}).get(node_id,{})
-        if len(addresses) == 0:
-            print("\nAppend machine id and camera ids/port addresses to registry file")
-            print(yaml.dump(registry))
-            raise Exception(f"Machine not yet registered. (Current machine id: {node_id})")
-        return addresses
+        frame = cv2.imread(filename)
+        return Image(frame)
     
-    @classmethod
-    def get_plans(cls, config_file:str, registry_file:str = None, package:str = None):
+    def saveImage(self, 
+        image: Optional[Image] = None, 
+        frame: Optional[np.ndarray] = None, 
+        filename: str = 'image.png'
+    ) -> bool:
         """
-        Read configuration file (yaml) and get details
+        Save image to file
 
         Args:
-            config_file (str): filename of configuration file
-            registry_file (str, optional): filename of registry file. Defaults to None.
-            package (str, optional): name of package to look in. Defaults to None.
+            image (Optional[Image], optional): image object to be saved. Defaults to None.
+            frame (Optional[np.ndarray], optional): frame array to be saved. Defaults to None.
+            filename (str, optional): filename to save to. Defaults to 'image.png'.
 
-        Returns:
-            dict: dictionary of configuration parameters
-        """
-        configs = cls.read_yaml(config_file, package)
-        registry = cls.read_yaml(registry_file, package)
-        addresses = cls.get_machine_addresses(registry=registry)
-        configs = cls.get_details(configs, addresses=addresses)
-        return configs
-    
-    @classmethod
-    def load_components(cls, config:dict):
-        """
-        Load components of compound tools
-
-        Args:
-            config (dict): dictionary of configuration parameters
-
-        Returns:
-            dict: dictionary of component tools
-        """
-        components = {}
-        for name, details in config.items():
-            _module = details.get('module')
-            if _module is None:
-                continue
-            _class = cls.get_class(_module, details.get('class', ''))
-            settings = details.get('settings', {})
-            components[name] = _class(**settings)
-        return components
-    
-    # Instance methods
-    def safety_measures(self, func):
-        return decorators.safety_measures(mode=self.safety_mode, countdown=self.safety_countdown)(func=func)
-    
-    # NOTE: DEPRECATE
-    @classmethod
-    def display_ports(cls):
-        """
-        Get available ports
-
-        Returns:
-            list: list of connected serial ports
-        """
-        print("'display_ports' method to be deprecated. Use 'get_ports' instead.")
-        return cls.get_ports()
-
-HELPER = Helper() 
-"""NOTE: importing HELPER gives the same instance of the 'Helper' class wherever you import it"""
-
-
-class Logger(object):
-    """
-    Logger class with miscellaneous methods
-    """
-    def __init__(self):
-        self.all_logs = []
-        self.logs = {}
-        pass
-    
-    # Instance methods
-    def log_now(self, message:str, group=None):
-        """
-        Add log with timestamp
-
-        Args:
-            message (str): message to be logged
-            group (str, optional): message group. Defaults to None.
+        Raises:
+            ValueError: Please input either image or frame.
 
         Returns:
-            str: log message with timestamp
-        """
-        log = time.strftime("%H:%M:%S", time.localtime()) + ' >> ' + message
-        self.all_logs.append(log)
-        if group:
-            if group not in self.logs.keys():
-                self.logs[group] = []
-            self.logs[group].append(message)
-        return log
-
-    def reset_logs(self):
-        """
-        Reset all logs
+            bool: whether the image is successfully saved
         """
-        self.all_logs = []
-        self.logs = {}
-        return
-
-    def save_logs(self, groups=[], folder=''):
-        """
-        Write logs into txt files
-
-        Args:
-            groups (list, optional): list of log messages. Defaults to [].
-            folder (str, optional): folder to save to. Defaults to ''.
-        """
-        dst_folder = '/'.join([folder, 'logs'])
-        if not os.path.exists(dst_folder):
-            os.makedirs(dst_folder)
+        if filename == 'image.png':
+            now = datetime.now().strftime("%Y%m%d_%H-%M-%S")
+            filename = f'image{now}.png'
         
-        with open(f'{dst_folder}/activity_log.txt', 'w') as f:
-            for line in self.all_logs:
-                f.write(line + '\n')
+        if (frame is None) == (image is None):
+            raise ValueError('Please input either image or frame.')
+        elif image is not None:
+            return image.save(filename)
+        return cv2.imwrite(filename, frame)
+    
+    # Protected method(s)
+    def _data_to_df(self, data:dict) -> pd.DataFrame:
+        """
+        Convert data dictionary to dataframe
+
+        Args:
+            data (dict): dictionary of data
+
+        Returns:
+            pd.DataFrame: dataframe of data
+        """
+        df = pd.DataFrame(data)
+        df.rename(columns={0: 'x', 1: 'y', 2: 'w', 3: 'h'}, inplace=True)
+        df.sort_values(by='y', ascending=True, inplace=True)
+        df.reset_index(inplace=True, drop=True)
+        differences = df['y'].diff()[1:]
+        row_numbers = [1]
+        for diff in differences: 
+            # If diff in y-coordinates > 30, assign next row (adjustable)
+            row = (row_numbers[-1] + 1) if diff > ROW_DISTANCE else row_numbers[-1]
+            row_numbers.append(row)
+        df['row'] = row_numbers
+        df.sort_values(by=['row','x'], ascending=[True,True], inplace=True) 
+        df.reset_index(inplace = True, drop = True)
+        return df
+    
+    def _loop_record(self):
+        """Loop to constantly get and save image frames"""
+        start_message = f'Recording...' if self.record_timeout is None else f'Recording... ({self.record_timeout}s)'
+        print(start_message)
+        timestamps = []
+        # frames = []
+        frame_num = 0
+        folder = Helper.create_folder(self.record_folder, 'frames')
         
-        for group in groups:
-            if group not in self.logs.keys():
-                print(f"'{group}' not found in log groups!")
+        start = datetime.now()
+        while self.flags['record']:
+            if self.flags['pause_record']:
                 continue
-            with open(f'{dst_folder}/{group}_log.txt', 'w') as f:
-                for line in self.logs[group]:
-                    f.write(line + '\n')
-        return
-
-LOGGER = Logger() 
-"""NOTE: importing LOGGER gives the same instance of the 'Logger' class wherever you import it"""
-
-
-# Core functions
-def create_configs():
-    """
-    Create new configs folder
-    """
-    cwd = os.getcwd().replace('\\', '/')
-    src = f"{here}/templates/configs"
-    dst = f"{cwd}/configs"
-    if not os.path.exists(dst):
-        print("Creating configs folder...\n")
-        copytree(src=src, dst=dst)
-        node_id = Helper.get_node()
-        print(f"Current machine id: {node_id}")
-    return
-
-def create_setup(setup_name:str = None):
-    """
-    Create new setup folder
-
-    Args:
-        setup_name (str, optional): name of new setup. Defaults to None.
-    """
-    cwd = os.getcwd().replace('\\', '/')
-    if setup_name is None:
-        setup_num = 1
-        while True:
-            setup_name = f'Setup{str(setup_num).zfill(2)}'
-            if not os.path.exists(f"{cwd}/configs/{setup_name}"):
+            now = datetime.now()
+            _, image = self.getImage()
+            self.saveImage(image, filename=f'{folder}/frames/frame_{frame_num:05}.png')
+            timestamps.append(now)
+            # frames.append(image.frame)
+            frame_num += 1
+            
+            # Timer check
+            if self.record_timeout is not None and (now - start).seconds > self.record_timeout:
                 break
-            setup_num += 1
-    src = f"{here}/templates/setup"
-    cfg = f"{cwd}/configs"
-    dst = f"{cfg}/{setup_name}"
-    if not os.path.exists(cfg):
-        create_configs()
-    if not os.path.exists(dst):
-        print(f"Creating setup folder ({setup_name})...\n")
-        copytree(src=src, dst=dst)
-    return
-
-@decorators.named_tuple_from_dict
-def load_setup(config_file:str, registry_file:str = None):
-    """
-    Load and initialise setup
-
-    Args:
-        config_file (str): config filename
-        registry_file (str, optional): registry filename. Defaults to None.
-
-    Returns:
-        dict: dictionary of loaded devices
-    """
-    config = Helper.get_plans(config_file=config_file, registry_file=registry_file)
-    setup = Helper.load_components(config=config)
-    shortcuts = config.get('SHORTCUTS',{})
-    
-    for key,value in shortcuts.items():
-        parent, child = value.split('.')
-        tool = setup.get(parent)
-        if tool is None:
-            print(f"Tool does not exist ({parent})")
-            continue
-        if 'components' not in tool.__dict__:
-            print(f"Tool ({parent}) does not have components")
-            continue
-        setup[key] = tool.components.get(child)
-    return setup
-
-def load_deck(device, layout_file:str, get_absolute_filepath:bool = True):
-    """
-    Load the deck information from layout file
-
-    Args:
-        device (object): device object that has the deck attribute
-        layout_file (str): layout file name
-        get_absolute_filepath (bool, optional): whether to extend the filepaths defined in layout file to their absolute filepaths. Defaults to True.
-
-    Returns:
-        object: device with deck loaded
-    """
-    layout_dict = Helper.read_json(layout_file)
-    if get_absolute_filepath:
-        get_repo_name = True
-        root = ''
-        for slot in layout_dict['slots'].values():
-            if get_repo_name:
-                repo_name = slot.get('filepath','').replace('\\', '/').split('/')[0]
-                root = layout_file.split(repo_name)[0]
-                get_repo_name = False
-            slot['filepath'] = f"{root}{slot['filepath']}"
-    device.loadDeck(layout_dict=layout_dict)
-    return device
-
-def set_safety(safety_level:str = None, safety_countdown:int = 3):
-    """
-    Set safety level of session
-
-    Args:
-        safety_level (str): 'high' - pauses for input before every move action; 'low' - waits for safety timeout before every move action
-        safety_countdown (int, optional): safety timeout in seconds. Defaults to 3.
-    """
-    safety_mode = None
-    if safety_level == 'high':
-        safety_mode = 'pause'
-    elif safety_level == 'low':
-        safety_mode = 'wait'
-    HELPER.safety_mode = safety_mode
-    HELPER.safety_countdown = safety_countdown
-    return
+        end = datetime.now()
+        
+        # for i,frame in enumerate(frames):
+        #     self.saveImage(frame=frame, filename=f'{folder}/frames/frame_{i:05}.png')
+        # frame_num = len(frames)
+        # del frames
+        
+        duration = end - start
+        print('Stop recording...')
+        print(f'\nDuration: {str(duration)}')
+        print(f'\nFrames recorded: {frame_num}')
+        print(f'\nAverage FPS: {frame_num/duration.seconds}')
+        df = pd.DataFrame({'frame_num': [i for i in range(frame_num)], 'timestamp': timestamps})
+        df.to_csv(f'{folder}/timestamps.csv')
+        return
+    
+    def _set_placeholder(self, 
+        filename: str = '', 
+        img_bytes: Optional[bytes] = None, 
+        resize: bool = False
+    ):
+        """
+        Sets placeholder image for camera, if not  camera is not connected
+
+        Args:
+            filename (str, optional): name of placeholder image file. Defaults to class attribute `_placeholder_filename`.
+            img_bytes (Optional[bytes], optional): byte array of placeholder image. Defaults to None.
+            resize (bool, optional): whether to resize the image. Defaults to False.
+
+        Returns:
+            Image: image of placeholder
+        """
+        image = None
+        if not len(filename) and img_bytes is None:
+            img_bytes = pkgutil.get_data(self._package, self._placeholder_filename)
+        if len(filename):
+            image = self.loadImage(filename)
+        elif type(img_bytes) == bytes:
+            array = np.asarray(bytearray(img_bytes), dtype="uint8")
+            image = self.decodeImage(array)
+        
+        if resize:
+            image.resize(self.cam_size, inplace=True)
+        self.placeholder_image = image
+        return
+
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Device01:                                         # name of simple device (user-defined)
-  module: __module_name_01__                      # device module
-  class: __submodule_1A__.__class_1A__            # device class
+_Device01_:                                     # name of simple device (user-defined)
+  module: _module_name_01_                      # device module
+  class: _submodule_1A_._class_1A_              # device class
   settings:
-    port: __device_01__                           # port addresses defined in registry.yaml
-    __setting_A__: {'tuple': [300,0,200]}         # use keys to define the type of iterable
-    __setting_B__: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
+    port: _device_01_                           # port addresses defined in registry.yaml
+    _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
+    _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
 
-Device02:                                         # name of 'Compound' device (user-defined)
+_Device02_:                                     # name of 'Compound' device (user-defined)
   module: Compound                            
-  class: __submodule_2A__.__class_2A__
+  class: _submodule_2A_._class_2A_
   settings:
-    __setting_C__: 1                              # other settings for your 'Compound' device
-    component_config:                             # nest component configuration settings here
-      Component01:                                # name of component
-        module: __module_name_03__
-        class: __submodule_3A__.__class_3A__
+    _setting_C_: 1                              # other settings for your 'Compound' device
+    component_config:                           # nest component configuration settings here
+      _Component01_:                            # name of component
+        module: _module_name_03_
+        class: _submodule_3A_._class_3A_
         settings:
-          ip_address: '192.0.0.1'                 # IP addresses do not vary between machines
-      Component02: 
-        module: __module_name_04__
-        class: __submodule_4A__.__class_4A__
+          ip_address: '192.0.0.1'               # IP addresses do not vary between machines
+      _Component02_: 
+        module: _module_name_04_
+        class: _submodule_4A_._class_4A_
         settings:
-          __setting_D__: 2                        # settings for your component device
+          _setting_D_: 2                        # settings for your component device
 
 SHORTCUTS:
-  Nickname1: 'Device02.Component01'
-  Nickname2: 'Device02.Component02'
+  _Nickname1_: '_Device02_._Component01_'
+  _Nickname2_: '_Device02_._Component02_'
```

### Comparing `control-lab-ly-0.0.4.1/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.0.0a0/src/controllably/misc/templates/setup/layout.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9618055555555555%*

 * *Differences: {"'slots'": "{'1': {'name': '_name_01_', 'filepath': '_repo_name_/.../_labware_01_.json'}, '2': "*

 * *            "{'filepath': '_repo_name_/.../_labware_02_.json'}, '3': {'name': '_name_03_', "*

 * *            "'filepath': '_repo_name_/.../_labware_03_.json'}, '4': {'name': '_name_04_', "*

 * *            "'filepath': '_repo_name_/.../_labware_04_.json'}, '5': {'name': '_name_05_', "*

 * *            "'filepath': '_repo_name_/.../_labware_05_.json'}, '6': {'name': '_name_06_', "*

 * *            "'filepath': '_repo_name_/.../_la […]*

```diff
@@ -30,37 +30,37 @@
             "_y06_",
             "_z06_"
         ]
     },
     "slots": {
         "1": {
             "exclusion_height": -1,
-            "filepath": "__repo_name__/.../__labware_01__.json",
-            "name": "__name_01__"
+            "filepath": "_repo_name_/.../_labware_01_.json",
+            "name": "_name_01_"
         },
         "2": {
             "exclusion_height": -1,
-            "filepath": "__repo_name__/.../__labware_02__.json",
+            "filepath": "_repo_name_/.../_labware_02_.json",
             "name": "__name_02__"
         },
         "3": {
             "exclusion_height": -1,
-            "filepath": "__repo_name__/.../__labware_03__.json",
-            "name": "__name_03__"
+            "filepath": "_repo_name_/.../_labware_03_.json",
+            "name": "_name_03_"
         },
         "4": {
             "exclusion_height": -1,
-            "filepath": "__repo_name__/.../__labware_04__.json",
-            "name": "__name_04__"
+            "filepath": "_repo_name_/.../_labware_04_.json",
+            "name": "_name_04_"
         },
         "5": {
             "exclusion_height": -1,
-            "filepath": "__repo_name__/.../__labware_05__.json",
-            "name": "__name_05__"
+            "filepath": "_repo_name_/.../_labware_05_.json",
+            "name": "_name_05_"
         },
         "6": {
             "exclusion_height": -1,
-            "filepath": "__repo_name__/.../__labware_06__.json",
-            "name": "__name_06__"
+            "filepath": "_repo_name_/.../_labware_06_.json",
+            "name": "_name_06_"
         }
     }
 }
```

