# Comparing `tmp/routingblocks-0.1.1.tar.gz` & `tmp/routingblocks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingblocks-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "routingblocks-0.1.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `routingblocks-0.1.1.tar` & `routingblocks-0.1.2.tar`

### file list

```diff
@@ -1,248 +1,248 @@
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.1/.clang-format
--rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.1/.cmake-format
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2109 2022-11-09 12:37:21.000000 routingblocks-0.1.1/.gitignore
--rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 routingblocks-0.1.1/CMakeLists.txt
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1758 2022-11-09 12:37:21.000000 routingblocks-0.1.1/README.md
--rw-r--r--   0        0        0     2450 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/CMakeLists.txt
--rw-r--r--   0        0        0      197 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/Evaluation.h
--rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/Instance.hpp
--rw-r--r--   0        0        0      216 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/Labeling.h
--rw-r--r--   0        0        0      319 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/LocalSearch.h
--rw-r--r--   0        0        0      421 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/Operators.h
--rw-r--r--   0        0        0      384 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/Solution.h
--rw-r--r--   0        0        0     3072 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/binding_helpers.hpp
--rw-r--r--   0        0        0      256 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/large_neighborhood.h
--rw-r--r--   0        0        0      241 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/include/vrpis_bindings/utility.h
--rw-r--r--   0        0        0    15224 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/Evaluation.cpp
--rw-r--r--   0        0        0     4836 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/Instance.cpp
--rw-r--r--   0        0        0     6002 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/Labeling.cpp
--rw-r--r--   0        0        0     3094 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/LocalSearch.cpp
--rw-r--r--   0        0        0     9943 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/Operators.cpp
--rw-r--r--   0        0        0    21656 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/Solution.cpp
--rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/bindings.cpp
--rw-r--r--   0        0        0    10371 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/large_neighborhood.cpp
--rw-r--r--   0        0        0     6069 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/src/utility.cpp
--rwxr-xr-x   0        0        0      192 2022-11-09 12:37:21.000000 routingblocks-0.1.1/bindings/stubgen.py
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.1/docs/make.bat
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 routingblocks-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 routingblocks-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 routingblocks-0.1.1/docs/source/routingblocks.rst
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 routingblocks-0.1.1/docs/source/usage.rst
--rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/README.md
--rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/__init__.py
--rw-r--r--   0        0        0     3260 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/__main__.py
--rw-r--r--   0        0        0    17856 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/alns.py
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/config.json
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instance/__init__.py
--rw-r--r--   0        0        0     1979 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instance/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instance/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instance/parsing.py
--rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/c101C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/c104C10.txt
--rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/c202C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/c205C10.txt
--rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/r102C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/r103C10.txt
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/r201C10.txt
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/r203C10.txt
--rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/rc102C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/rc108C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/rc201C10.txt
--rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/rc205C10.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c109_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c201_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c203_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c204_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c205_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c206_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c207_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c208_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r105_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r109_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r110_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r111_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r112_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r208_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r209_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r210_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r211_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc108_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc202_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc208_21.txt
--rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/c103C15.txt
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/c106C15.txt
--rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/c202C15.txt
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/c208C15.txt
--rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/r102C15.txt
--rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/r105C15.txt
--rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/r202C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/r209C15.txt
--rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/rc103C15.txt
--rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/rc108C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/rc202C15.txt
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/rc204C15.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/c101C5.txt
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/c103C5.txt
--rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/c206C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/c208C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/r104C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/r105C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/r202C5.txt
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/r203C5.txt
--rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/rc105C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/rc108C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/rc204C5.txt
--rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/rc208C5.txt
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/instances/evrptw/README.txt
--rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/operators/ShawMoveSelector.py
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/operators/ShawRelatedness.py
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/operators/SpatioTemporalRelatedness.py
--rw-r--r--   0        0        0     2061 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/operators/__init__.py
--rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/parameters.py
--rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/requirements.txt
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/utility/__init__.py
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.1/examples/evrptw/utility/algorithms.py
--rw-r--r--   0        0        0     3003 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/CMakeLists.txt
--rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/cmake/CPM.cmake
--rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/cmake/tools.cmake
--rw-r--r--   0        0        0    23731 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/ADPTWEvaluation.h
--rw-r--r--   0        0        0    15998 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/FRVCP.h
--rw-r--r--   0        0        0     2509 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/Instance.h
--rw-r--r--   0        0        0    11789 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/LocalSearch.h
--rw-r--r--   0        0        0     6144 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/NIFTWEvaluation.h
--rw-r--r--   0        0        0    28794 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/Solution.h
--rw-r--r--   0        0        0     5012 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/adaptive_large_neighborhood.hpp
--rw-r--r--   0        0        0      488 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/interfaces/arc.h
--rw-r--r--   0        0        0     8783 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/interfaces/evaluation.h
--rw-r--r--   0        0        0     2910 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/interfaces/node.h
--rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/interfaces/types.h
--rw-r--r--   0        0        0     1309 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/interfaces/vertex.h
--rw-r--r--   0        0        0     1909 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/lns_operators.h
--rw-r--r--   0        0        0     4024 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/operators/InsertStationOperator.h
--rw-r--r--   0        0        0      875 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/operators/InterRouteTwoOptOperator.h
--rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/operators/RemoveStationOperator.h
--rw-r--r--   0        0        0    15752 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/operators/SwapOperator.h
--rw-r--r--   0        0        0     1861 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/operators.h
--rw-r--r--   0        0        0     8030 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/utility/adaptive_priority_list.h
--rw-r--r--   0        0        0      765 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/utility/algorithms.h
--rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/utility/arc_set.h
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/utility/heap.h
--rw-r--r--   0        0        0    11670 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/utility/insertion_cache.h
--rw-r--r--   0        0        0      786 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/utility/iterator_pair.h
--rw-r--r--   0        0        0     3711 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/utility/random.h
--rw-r--r--   0        0        0     4879 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/include/vrpis/utility/removal_cache.h
--rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/CMakeLists.txt
--rw-r--r--   0        0        0      222 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/dynamic_bitset/CMakeLists.txt
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/dynamic_bitset/LICENSE.txt
--rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
--rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/small_vector/CMakeLists.txt
--rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/small_vector/LICENSE.txt
--rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/small_vector/small_vector/small_vector.hpp
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/xoshiro/CMakeLists.txt
--rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/xoshiro/LICENSE.txt
--rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/lib/xoshiro/xoshiro/xoshiro.h
--rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/ADPTWEvaluation.cpp
--rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/FRVCP.cpp
--rw-r--r--   0        0        0     2177 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/Instance.cpp
--rw-r--r--   0        0        0     1964 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/LocalSearch.cpp
--rw-r--r--   0        0        0     8251 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/NIFTWEvaluation.cpp
--rw-r--r--   0        0        0     3749 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/Solution.cpp
--rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/adaptive_large_neighborbood.cpp
--rw-r--r--   0        0        0     4407 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/lns_operators.cpp
--rw-r--r--   0        0        0     1050 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/node.cpp
--rw-r--r--   0        0        0     3396 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/operators/InsertStationOperator.cpp
--rw-r--r--   0        0        0     2027 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/src/operators/InterRouteTwoOptOperator.cpp
--rw-r--r--   0        0        0     1613 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/test/CMakeLists.txt
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.1/native/test/src/dummy.cpp
--rw-r--r--   0        0        0     1330 2022-11-09 12:37:21.000000 routingblocks-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/__init__.py
--rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/operators/__init__.py
--rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/operators/best_insert.py
--rw-r--r--   0        0        0     4390 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/operators/cluster_removal.py
--rw-r--r--   0        0        0     1928 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/operators/move_selectors.py
--rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/operators/related_removal.py
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/operators/route_removal.py
--rw-r--r--   0        0        0     3835 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/operators/station_vicinity_removal.py
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/operators/worst_removal.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.1/routingblocks/utility/__init__.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/benchmarks/reference/insertion_cache.py
--rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/benchmarks/reference/removal_cache.py
--rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/benchmarks/test_benchmark_frvcp.py
--rw-r--r--   0        0        0     2006 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/benchmarks/test_benchmark_local_search.py
--rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/benchmarks/test_benchmark_removal_cache.py
--rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/benchmarks/test_benchmark_route_update.py
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/conftest.py
--rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/fixtures/data/c101C5.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/fixtures/data/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/fixtures/data/r101_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/fixtures/data/r201_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/fixtures/data/rc101_21.txt
--rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/fixtures/mock_evaluation.py
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1979 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/helpers/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/helpers/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/helpers/parsing.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/__init__.py
--rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/test_cluster_removal.py
--rw-r--r--   0        0        0     1635 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/test_random_insertion.py
--rw-r--r--   0        0        0     1815 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/test_random_removal.py
--rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/test_related_removal.py
--rw-r--r--   0        0        0     1904 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/test_station_insertion.py
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/test_station_removal.py
--rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/test_station_vicinity_removal.py
--rw-r--r--   0        0        0    20342 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/operators/test_swap.py
--rw-r--r--   0        0        0     3851 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_evaluation.py
--rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_frvcp.py
--rw-r--r--   0        0        0     6394 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_insertion_cache.py
--rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_large_neighborhood.py
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_lns_helpers.py
--rw-r--r--   0        0        0     2622 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_local_search.py
--rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_node.py
--rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_removal_cache.py
--rw-r--r--   0        0        0    13948 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_route.py
--rw-r--r--   0        0        0    19901 2022-11-09 12:37:21.000000 routingblocks-0.1.1/test/tests/test_solution.py
--rw-r--r--   0        0        0     2797 2022-11-09 12:37:21.000000 routingblocks-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.2/.clang-format
+-rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.2/.cmake-format
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.2/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2109 2022-11-09 12:37:21.000000 routingblocks-0.1.2/.gitignore
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.2/CMakeLists.txt
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1866 2022-11-09 12:37:21.000000 routingblocks-0.1.2/README.md
+-rw-r--r--   0        0        0     2753 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/CMakeLists.txt
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/Evaluation.h
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/Instance.hpp
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/Labeling.h
+-rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/LocalSearch.h
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/Operators.h
+-rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/Solution.h
+-rw-r--r--   0        0        0     3697 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/binding_helpers.hpp
+-rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/large_neighborhood.h
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/include/routingblocks_bindings/utility.h
+-rw-r--r--   0        0        0    15340 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/Evaluation.cpp
+-rw-r--r--   0        0        0     4672 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/Instance.cpp
+-rw-r--r--   0        0        0     6141 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/Labeling.cpp
+-rw-r--r--   0        0        0     3492 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/LocalSearch.cpp
+-rw-r--r--   0        0        0    10602 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/Operators.cpp
+-rw-r--r--   0        0        0    22438 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/Solution.cpp
+-rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/bindings.cpp
+-rw-r--r--   0        0        0    10923 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/large_neighborhood.cpp
+-rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/src/utility.cpp
+-rwxr-xr-x   0        0        0      192 2022-11-09 12:37:21.000000 routingblocks-0.1.2/bindings/stubgen.py
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 routingblocks-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0      482 2022-11-09 12:37:21.000000 routingblocks-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 routingblocks-0.1.2/docs/source/routingblocks.rst
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 routingblocks-0.1.2/docs/source/usage.rst
+-rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/README.md
+-rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/__init__.py
+-rw-r--r--   0        0        0     3260 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/__main__.py
+-rw-r--r--   0        0        0    17856 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/alns.py
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/config.json
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instance/__init__.py
+-rw-r--r--   0        0        0     1979 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instance/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instance/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instance/parsing.py
+-rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/c101C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/c104C10.txt
+-rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/c202C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/c205C10.txt
+-rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/r102C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/r103C10.txt
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/r201C10.txt
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/r203C10.txt
+-rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/rc102C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/rc108C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/rc201C10.txt
+-rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/rc205C10.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c109_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c201_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c203_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c204_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c205_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c206_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c207_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c208_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r105_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r109_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r110_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r111_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r112_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r208_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r209_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r210_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r211_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc108_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc202_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc208_21.txt
+-rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/c103C15.txt
+-rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/c106C15.txt
+-rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/c202C15.txt
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/c208C15.txt
+-rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/r102C15.txt
+-rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/r105C15.txt
+-rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/r202C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/r209C15.txt
+-rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/rc103C15.txt
+-rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/rc108C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/rc202C15.txt
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/rc204C15.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/c101C5.txt
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/c103C5.txt
+-rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/c206C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/c208C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/r104C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/r105C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/r202C5.txt
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/r203C5.txt
+-rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/rc105C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/rc108C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/rc204C5.txt
+-rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/rc208C5.txt
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/instances/evrptw/README.txt
+-rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/operators/ShawMoveSelector.py
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/operators/ShawRelatedness.py
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/operators/SpatioTemporalRelatedness.py
+-rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/operators/__init__.py
+-rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/parameters.py
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/requirements.txt
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/utility/__init__.py
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.2/examples/evrptw/utility/algorithms.py
+-rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/CMakeLists.txt
+-rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/cmake/CPM.cmake
+-rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/cmake/tools.cmake
+-rw-r--r--   0        0        0    23647 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/ADPTWEvaluation.h
+-rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/FRVCP.h
+-rw-r--r--   0        0        0     2551 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/Instance.h
+-rw-r--r--   0        0        0    11828 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/LocalSearch.h
+-rw-r--r--   0        0        0     6234 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/NIFTWEvaluation.h
+-rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/Solution.h
+-rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/adaptive_large_neighborhood.hpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/arc.h
+-rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/evaluation.h
+-rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/insertion_cache.h
+-rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/lns_operators.h
+-rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/node.h
+-rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/operators/InsertStationOperator.h
+-rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
+-rw-r--r--   0        0        0     3158 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/operators/RemoveStationOperator.h
+-rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/operators/SwapOperator.h
+-rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/operators.h
+-rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/removal_cache.h
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/types.h
+-rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/utility/adaptive_priority_list.h
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/utility/algorithms.h
+-rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/utility/arc_set.h
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/utility/heap.h
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/utility/iterator_pair.h
+-rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/utility/random.h
+-rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/include/routingblocks/vertex.h
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/CMakeLists.txt
+-rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/dynamic_bitset/CMakeLists.txt
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/dynamic_bitset/LICENSE.txt
+-rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
+-rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
+-rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/small_vector/CMakeLists.txt
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/small_vector/LICENSE.txt
+-rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/small_vector/small_vector/small_vector.hpp
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/xoshiro/CMakeLists.txt
+-rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/xoshiro/LICENSE.txt
+-rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/lib/xoshiro/xoshiro/xoshiro.h
+-rw-r--r--   0        0        0     3302 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/ADPTWEvaluation.cpp
+-rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/FRVCP.cpp
+-rw-r--r--   0        0        0     2296 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/Instance.cpp
+-rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/LocalSearch.cpp
+-rw-r--r--   0        0        0     8324 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/NIFTWEvaluation.cpp
+-rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/Solution.cpp
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/adaptive_large_neighborbood.cpp
+-rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/lns_operators.cpp
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/node.cpp
+-rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/operators/InsertStationOperator.cpp
+-rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/src/operators/InterRouteTwoOptOperator.cpp
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/test/CMakeLists.txt
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.2/native/test/src/dummy.cpp
+-rw-r--r--   0        0        0     1330 2022-11-09 12:37:21.000000 routingblocks-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/__init__.py
+-rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/operators/__init__.py
+-rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/operators/best_insert.py
+-rw-r--r--   0        0        0     4390 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/operators/cluster_removal.py
+-rw-r--r--   0        0        0     1928 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/operators/move_selectors.py
+-rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/operators/related_removal.py
+-rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/operators/route_removal.py
+-rw-r--r--   0        0        0     3835 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/operators/station_vicinity_removal.py
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/operators/worst_removal.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.2/routingblocks/utility/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/benchmarks/reference/insertion_cache.py
+-rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/benchmarks/reference/removal_cache.py
+-rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/benchmarks/test_benchmark_frvcp.py
+-rw-r--r--   0        0        0     2006 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/benchmarks/test_benchmark_local_search.py
+-rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/benchmarks/test_benchmark_removal_cache.py
+-rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/benchmarks/test_benchmark_route_update.py
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/conftest.py
+-rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/fixtures/data/c101C5.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/fixtures/data/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/fixtures/data/r101_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/fixtures/data/r201_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/fixtures/data/rc101_21.txt
+-rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/fixtures/mock_evaluation.py
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1979 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/helpers/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/helpers/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/helpers/parsing.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/__init__.py
+-rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/test_cluster_removal.py
+-rw-r--r--   0        0        0     1635 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/test_random_insertion.py
+-rw-r--r--   0        0        0     1815 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/test_random_removal.py
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/test_related_removal.py
+-rw-r--r--   0        0        0     1904 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/test_station_insertion.py
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/test_station_removal.py
+-rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/test_station_vicinity_removal.py
+-rw-r--r--   0        0        0    20342 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/operators/test_swap.py
+-rw-r--r--   0        0        0     3851 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_evaluation.py
+-rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_frvcp.py
+-rw-r--r--   0        0        0     6394 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_insertion_cache.py
+-rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_large_neighborhood.py
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_lns_helpers.py
+-rw-r--r--   0        0        0     2622 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_local_search.py
+-rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_node.py
+-rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_removal_cache.py
+-rw-r--r--   0        0        0    13948 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_route.py
+-rw-r--r--   0        0        0    19901 2022-11-09 12:37:21.000000 routingblocks-0.1.2/test/tests/test_solution.py
+-rw-r--r--   0        0        0     2905 2022-11-09 12:37:21.000000 routingblocks-0.1.2/PKG-INFO
```

### Comparing `routingblocks-0.1.1/.cmake-format` & `routingblocks-0.1.2/.cmake-format`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/.github/workflows/wheels.yml` & `routingblocks-0.1.2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/.gitignore` & `routingblocks-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/CONTRIBUTING.md` & `routingblocks-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/README.md` & `routingblocks-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ## Features
 
 * Efficient C++-based solution representation
 * Customizable Local Search Solver
 * Framework for ALNS-based metaheuristics
 * Efficient native implementations of numerous destroy, repair, and local search operators
 * Move caches implemented in native code to allow high-performance operator implementations in Python
+* Support for custom [native extensions](https://github.com/tumBAIS/routingblocks-native-extension-example)
 
 ## Usage
 
 We provide an [example implementation](https://github.com/tumBAIS/RoutingBlocks/tree/main/examples) of an ALNS-based
 algorithm for
 the [EVRPTW-PR](https://research.sabanciuniv.edu/id/eprint/26033/1/WP_EVRPTW-Partial_Recharge_KeskinCatay.pdf) as part
 of this repository.
```

### Comparing `routingblocks-0.1.1/bindings/CMakeLists.txt` & `routingblocks-0.1.2/bindings/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,32 +10,36 @@
 set(PYBIND11_PYTHON_VERSION ${Python_VERSION})
 set(PYTHON_EXECUTABLE ${Python_EXECUTABLE})
 set(PYTHON_LIBS ${Python_LIBS})
 FIND_PACKAGE(pybind11 CONFIG REQUIRED)
 
 option(${PROJECT_NAME_UPPER}_ENABLE_STUB_GEN "Generate python stub files for the bindings generated." ON)
 
-file(GLOB_RECURSE headers CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/include/vrpis_bindings/*.h")
+file(GLOB_RECURSE headers CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/include/routingblocks_bindings/*.h")
 file(GLOB_RECURSE sources CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp")
 
 pybind11_add_module(${PROJECT_NAME} ${sources})
 
 target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
-target_compile_definitions(${PROJECT_NAME} PUBLIC "VRPIS_MODULE_NAME=${PROJECT_NAME}")
-target_compile_definitions(${PROJECT_NAME} PUBLIC "VRPIS_VERSION=${PROJECT_VERSION}")
+target_compile_definitions(${PROJECT_NAME} PUBLIC "routingblocks_MODULE_NAME=${PROJECT_NAME}")
+target_compile_definitions(${PROJECT_NAME} PUBLIC "routingblocks_VERSION=${PROJECT_VERSION}")
+
+# Configure optimization flags
 if (CMAKE_COMPILER_IS_GNUCC)
     target_compile_options(${PROJECT_NAME} PUBLIC "$<$<CONFIG:DEBUG>:-O0;-g3>")
     target_compile_options(${PROJECT_NAME} PUBLIC "$<$<CONFIG:RELEASE>:-O3;>")
     target_compile_options(${PROJECT_NAME} PUBLIC "$<$<CONFIG:PROFILE>:-O2;-pg;-fno-omit-frame-pointer;-fno-optimize-sibling-calls;>")
 endif ()
 if (MSVC)
     target_compile_options(${PROJECT_NAME} PUBLIC "$<$<CONFIG:DEBUG>:/Od>")
     target_compile_options(${PROJECT_NAME} PUBLIC "$<$<CONFIG:RELEASE>:/O2y>")
 endif ()
-target_link_libraries(${PROJECT_NAME} PUBLIC VRPIS)
+
+# Link to main routing blocks library
+target_link_libraries(${PROJECT_NAME} PUBLIC routingblocks)
 
 check_ipo_supported(RESULT ${PROJECT_NAME}_HAS_LTO)
 if (${${PROJECT_NAME}_HAS_LTO})
     message(STATUS "LTO is supported")
     set_target_properties(${PROJECT_NAME} PROPERTIES INTERPROCEDUAL_OPTIMIZATION TRUE)
 endif ()
 
@@ -45,7 +49,10 @@
     INSTALL(FILES ${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}.pyi DESTINATION routingblocks)
 endif ()
 
 #
 # Set the compiler standard
 #
 target_compile_features(${PROJECT_NAME} PUBLIC cxx_std_20)
+
+INSTALL(TARGETS routingblocks DESTINATION routingblocks)
+INSTALL(FILES ${CMAKE_CURRENT_SOURCE_DIR}/include/routingblocks_bindings/binding_helpers.hpp DESTINATION routingblocks/include/routingblocks/)
```

### Comparing `routingblocks-0.1.1/bindings/include/vrpis_bindings/binding_helpers.hpp` & `routingblocks-0.1.2/bindings/include/routingblocks_bindings/binding_helpers.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -41,10 +41,21 @@
         return ss.str();
     }
 
     template <class T> auto py_iterator_from_range(T&& range) {
         return pybind11::make_iterator(std::begin(range), std::end(range));
     }
 
+    template <class data_t> routingblocks::Vertex vertex_constructor(size_t vid, std::string name,
+                                                                     bool is_station, bool is_depot,
+                                                                     data_t user_data) {
+        return routingblocks::Vertex(vid, name, is_station, is_depot,
+                                     std::make_shared<data_t>(std::move(user_data)));
+    }
+
+    template <class data_t> routingblocks::Arc arc_constructor(data_t user_data) {
+        return routingblocks::Arc(std::make_shared<data_t>(std::move(user_data)));
+    }
+
 }  // namespace bindings::helpers
 
 #endif
```

### Comparing `routingblocks-0.1.1/bindings/src/Evaluation.cpp` & `routingblocks-0.1.2/bindings/src/Evaluation.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-#include "vrpis_bindings/Evaluation.h"
-
 #include <pybind11/stl.h>
+#include <routingblocks/ADPTWEvaluation.h>
+#include <routingblocks/NIFTWEvaluation.h>
+#include <routingblocks/evaluation.h>
+#include <routingblocks_bindings/Evaluation.h>
 
-#include "vrpis/ADPTWEvaluation.h"
-#include "vrpis/NIFTWEvaluation.h"
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis_bindings/binding_helpers.hpp"
+#include <routingblocks_bindings/binding_helpers.hpp>
 
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
 
-    class PyEvaluation : public vrpis::Evaluation {
+    class PyEvaluation : public routingblocks::Evaluation {
       protected:
         using py_type = pybind11::object;
         using py_segment_node_type = std::tuple<const Vertex*, py_type, py_type>;
         using py_segment_type = std::vector<py_segment_node_type>;
 
       public:
-        using vrpis::Evaluation::Evaluation;
+        using routingblocks::Evaluation::Evaluation;
 
         virtual cost_t py_evaluate(const Instance& instance, std::vector<py_segment_type> segments)
             = 0;
 
         virtual cost_t py_compute_cost(const py_type& label) const = 0;
         virtual bool py_is_feasible(const py_type& label) const = 0;
 
@@ -95,20 +94,20 @@
 
         std::vector<resource_t> get_cost_components(
             const Evaluation::label_holder_t& label) const final {
             return py_get_cost_components(label.get<py_type>());
         }
     };
 
-    class PyConcatenationBasedEvaluation : public vrpis::ConcatenationBasedEvaluation {
+    class PyConcatenationBasedEvaluation : public routingblocks::ConcatenationBasedEvaluation {
       protected:
         using py_type = pybind11::object;
 
       public:
-        using vrpis::ConcatenationBasedEvaluation::ConcatenationBasedEvaluation;
+        using routingblocks::ConcatenationBasedEvaluation::ConcatenationBasedEvaluation;
 
         virtual cost_t py_concatenate(const py_type& fwd, const py_type& bwd, const Vertex& vertex)
             = 0;
 
         virtual cost_t py_compute_cost(const py_type& label) const = 0;
         virtual bool py_is_feasible(const py_type& label) const = 0;
 
@@ -168,20 +167,20 @@
 
         std::vector<resource_t> get_cost_components(
             const ConcatenationBasedEvaluation::label_holder_t& label) const final {
             return py_get_cost_components(label.get<py_type>());
         }
     };
 
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
 
-BIND_LIFETIME_PYTHON(vrpis::Evaluation, "Evaluation")
-BIND_LIFETIME_PYTHON(vrpis::bindings::PyEvaluation, "PyEvaluation")
+BIND_LIFETIME_PYTHON(routingblocks::Evaluation, "Evaluation")
+BIND_LIFETIME_PYTHON(routingblocks::bindings::PyEvaluation, "PyEvaluation")
 
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
 
     class PyConcatenationBasedEvaluationTramboline : public PyConcatenationBasedEvaluation {
         using PyConcatenationBasedEvaluation::PyConcatenationBasedEvaluation;
 
       public:
         cost_t py_concatenate(const py_type& fwd, const py_type& bwd,
                               const Vertex& vertex) override {
@@ -279,15 +278,15 @@
         adptw_module.attr("OverloadCostComponent")
             = pybind11::int_(static_cast<int>(ADPTWEvaluation::CostComponent::OVERLOAD_INDEX));
         adptw_module.attr("TimeShiftCostComponent")
             = pybind11::int_(static_cast<int>(ADPTWEvaluation::CostComponent::TIME_SHIFT_INDEX));
 
         auto niftw_module = m.def_submodule("niftw");
         bind_evaluation<NIFTWEvaluation>(
-            pybind11::class_<vrpis::NIFTWEvaluation, std::shared_ptr<NIFTWEvaluation>>(
+            pybind11::class_<routingblocks::NIFTWEvaluation, std::shared_ptr<NIFTWEvaluation>>(
                 niftw_module, "Evaluation", evaluation_interface)
                 .def(pybind11::init<resource_t, resource_t, resource_t>()))
             .def_property("penalty_factors", &NIFTWEvaluation::get_penalty_factors,
                           &NIFTWEvaluation::set_penalty_factors);
 
         niftw_module.attr("DistanceCostComponent")
             = pybind11::int_(static_cast<int>(NIFTWEvaluation::CostComponent::DIST_INDEX));
@@ -295,8 +294,8 @@
             = pybind11::int_(static_cast<int>(NIFTWEvaluation::CostComponent::OVERCHARGE_INDEX));
         niftw_module.attr("OverloadCostComponent")
             = pybind11::int_(static_cast<int>(NIFTWEvaluation::CostComponent::OVERLOAD_INDEX));
         niftw_module.attr("TimeShiftCostComponent")
             = pybind11::int_(static_cast<int>(NIFTWEvaluation::CostComponent::TIME_SHIFT_INDEX));
     }
 
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.1/bindings/src/Instance.cpp` & `routingblocks-0.1.2/bindings/src/Instance.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,79 @@
-#include "vrpis_bindings/Instance.hpp"
+#include "routingblocks_bindings/Instance.hpp"
 
 #include <pybind11/stl.h>
-#include <vrpis/ADPTWEvaluation.h>
-#include <vrpis/Instance.h>
-#include <vrpis/NIFTWEvaluation.h>
-
-#include "vrpis_bindings/binding_helpers.hpp"
-
-namespace {
-    template <class data_t> vrpis::Vertex vertex_constructor(size_t vid, std::string name,
-                                                             bool is_station, bool is_depot,
-                                                             data_t user_data) {
-        return vrpis::Vertex(vid, name, is_station, is_depot,
-                             std::make_shared<data_t>(std::move(user_data)));
-    }
+#include <routingblocks/ADPTWEvaluation.h>
+#include <routingblocks/Instance.h>
+#include <routingblocks/NIFTWEvaluation.h>
 
-    template <class data_t> vrpis::Arc arc_constructor(data_t user_data) {
-        return vrpis::Arc(std::make_shared<data_t>(std::move(user_data)));
-    }
-}  // namespace
+#include <routingblocks_bindings/binding_helpers.hpp>
 
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
     template <class VertexData> auto bind_vertex(pybind11::module& m, std::string_view name) {
-        return pybind11::class_<vrpis::Vertex>(m, name.data())
-            .def(pybind11::init(&vertex_constructor<VertexData>))
-            .def_readonly("id", &vrpis::Vertex::id)
-            .def_readonly("vertex_id", &vrpis::Vertex::id)
-            .def_readonly("str_id", &vrpis::Vertex::str_id)
-            .def_readonly("is_station", &vrpis::Vertex::is_station)
-            .def_readonly("is_depot", &vrpis::Vertex::is_depot)
+        return pybind11::class_<routingblocks::Vertex>(m, name.data())
+            .def(pybind11::init(&::bindings::helpers::vertex_constructor<VertexData>))
+            .def_readonly("id", &routingblocks::Vertex::id)
+            .def_readonly("vertex_id", &routingblocks::Vertex::id)
+            .def_readonly("str_id", &routingblocks::Vertex::str_id)
+            .def_readonly("is_station", &routingblocks::Vertex::is_station)
+            .def_readonly("is_depot", &routingblocks::Vertex::is_depot)
             .def_property_readonly("is_customer",
                                    [](const Vertex& v) { return !v.is_station && !v.is_depot; })
-            .def("__str__", &::bindings::helpers::ostream_to_string<vrpis::Vertex>);
+            .def("__str__", &::bindings::helpers::ostream_to_string<routingblocks::Vertex>);
     }
 
     template <class ArcData> auto bind_arc(pybind11::module& m, std::string_view name) {
-        return pybind11::class_<vrpis::Arc>(m, name.data())
-            .def(pybind11::init<>(&arc_constructor<ArcData>));
+        return pybind11::class_<routingblocks::Arc>(m, name.data())
+            .def(pybind11::init<>(&::bindings::helpers::arc_constructor<ArcData>));
     }
 
-    void bind_vrpis_instance(pybind11::module& m) {
+    void bind_routingblocks_instance(pybind11::module& m) {
         bind_vertex<pybind11::object>(m, "Vertex");
-        m.def("create_adptw_vertex", &vertex_constructor<ADPTWVertexData>);
-        m.def("create_niftw_vertex", &vertex_constructor<NIFTWVertexData>);
+        m.def("create_adptw_vertex", &::bindings::helpers::vertex_constructor<ADPTWVertexData>);
+        m.def("create_niftw_vertex", &::bindings::helpers::vertex_constructor<NIFTWVertexData>);
 
         bind_arc<pybind11::object>(m, "Arc");
-        m.def("create_adptw_arc", &arc_constructor<ADPTWArcData>);
-        m.def("create_niftw_arc", &arc_constructor<NIFTWArcData>);
+        m.def("create_adptw_arc", &::bindings::helpers::arc_constructor<ADPTWArcData>);
+        m.def("create_niftw_arc", &::bindings::helpers::arc_constructor<NIFTWArcData>);
 
-        pybind11::class_<vrpis::ADPTWVertexData>(m, "ADPTWVertexData")
+        pybind11::class_<routingblocks::ADPTWVertexData>(m, "ADPTWVertexData")
             .def(pybind11::init<float, float, resource_t, resource_t, resource_t, resource_t>());
-        pybind11::class_<vrpis::ADPTWArcData>(m, "ADPTWArcData")
+        pybind11::class_<routingblocks::ADPTWArcData>(m, "ADPTWArcData")
             .def(pybind11::init<resource_t, resource_t, resource_t>());
 
-        pybind11::class_<vrpis::Instance>(m, "Instance")
-            .def(pybind11::init<std::vector<vrpis::Vertex>, std::vector<std::vector<vrpis::Arc>>,
-                                int>())
-            .def_property_readonly("fleet_size", &vrpis::Instance::FleetSize)
-            .def_property_readonly("number_of_customers", &vrpis::Instance::NumberOfCustomers)
-            .def_property_readonly("number_of_stations", &vrpis::Instance::NumberOfStations)
-            .def_property_readonly("number_of_vertices", &vrpis::Instance::NumberOfVertices)
-            .def_property_readonly("depot", &vrpis::Instance::Depot)
+        pybind11::class_<routingblocks::Instance>(m, "Instance")
+            .def(pybind11::init<std::vector<routingblocks::Vertex>,
+                                std::vector<std::vector<routingblocks::Arc>>, int>())
+            .def_property_readonly("fleet_size", &routingblocks::Instance::FleetSize)
+            .def_property_readonly("number_of_customers",
+                                   &routingblocks::Instance::NumberOfCustomers)
+            .def_property_readonly("number_of_stations", &routingblocks::Instance::NumberOfStations)
+            .def_property_readonly("number_of_vertices", &routingblocks::Instance::NumberOfVertices)
+            .def_property_readonly("depot", &routingblocks::Instance::Depot)
             .def_property_readonly("stations",
-                                   [](const vrpis::Instance& inst) {
+                                   [](const routingblocks::Instance& inst) {
                                        auto stations = inst.Stations();
                                        return pybind11::make_iterator(std::begin(stations),
                                                                       std::end(stations));
                                    })
             .def_property_readonly("customers",
-                                   [](const vrpis::Instance& inst) {
+                                   [](const routingblocks::Instance& inst) {
                                        auto customers = inst.Customers();
                                        return pybind11::make_iterator(std::begin(customers),
                                                                       std::end(customers));
                                    })
-            .def("__len__", &vrpis::Instance::NumberOfVertices)
+            .def("__len__", &routingblocks::Instance::NumberOfVertices)
             .def("__iter__",
-                 [](const vrpis::Instance& inst) {
+                 [](const routingblocks::Instance& inst) {
                      return pybind11::make_iterator(inst.begin(), inst.end());
                  })
-            .def("get_vertex", &vrpis::Instance::getVertex,
+            .def("get_vertex", &routingblocks::Instance::getVertex,
                  pybind11::return_value_policy::reference_internal)
-            .def("get_customer", &vrpis::Instance::getCustomer,
+            .def("get_customer", &routingblocks::Instance::getCustomer,
                  pybind11::return_value_policy::reference_internal)
-            .def("get_station", &vrpis::Instance::getStation,
+            .def("get_station", &routingblocks::Instance::getStation,
                  pybind11::return_value_policy::reference_internal)
-            .def("get_arc", &vrpis::Instance::getArc, "Gets an arc by vertex id",
+            .def("get_arc", &routingblocks::Instance::getArc, "Gets an arc by vertex id",
                  pybind11::return_value_policy::reference_internal);
     }
 
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.1/bindings/src/Labeling.cpp` & `routingblocks-0.1.2/bindings/src/Labeling.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-#include "vrpis_bindings/Labeling.h"
-
-#include <vrpis/ADPTWEvaluation.h>
-#include <vrpis/FRVCP.h>
-#include <vrpis/Instance.h>
 #include <pybind11/stl.h>
+#include <routingblocks/ADPTWEvaluation.h>
+#include <routingblocks/FRVCP.h>
+#include <routingblocks/Instance.h>
+#include <routingblocks_bindings/Labeling.h>
 
-#include "vrpis_bindings/binding_helpers.hpp"
+#include <routingblocks_bindings/binding_helpers.hpp>
 
-namespace vrpis {
+namespace routingblocks {
     template <> class Propagator<pybind11::object> {
       public:
         using value_type = pybind11::object;
         virtual std::optional<value_type> propagate(const value_type& predecessor,
                                                     const Vertex& origin, const Vertex& target,
                                                     const Arc& arc)
             = 0;
@@ -27,19 +26,19 @@
         virtual bool is_final_label(const value_type& _label) = 0;
 
         virtual void prepare(const std::vector<VertexID>&) = 0;
 
         virtual value_type create_root_label() = 0;
     };
     using PyPropagator = Propagator<pybind11::object>;
-}  // namespace vrpis
+}  // namespace routingblocks
 
-BIND_LIFETIME_PYTHON(vrpis::Propagator<pybind11::object>, "Propagator")
+BIND_LIFETIME_PYTHON(routingblocks::Propagator<pybind11::object>, "Propagator")
 
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
     class PyPropagatorTramboline : public PyPropagator {
       public:
         using value_type = PyPropagator::value_type;
         using PyPropagator::PyPropagator;
 
         std::optional<value_type> propagate(const value_type& predecessor, const Vertex& origin,
                                             const Vertex& target, const Arc& arc) override {
@@ -72,15 +71,15 @@
         }
 
         value_type create_root_label() override {
             PYBIND11_OVERRIDE_PURE(value_type, PyPropagator, create_root_label, );
         }
     };
 
-    using PyFRVCP = vrpis::FRVCP<pybind11::object>;
+    using PyFRVCP = routingblocks::FRVCP<pybind11::object>;
 
     template <class PropagatorClass> auto bind_propagator(auto& propagator) {
         return propagator.def("propagate", &PropagatorClass::propagate)
             .def("dominates", &PropagatorClass::dominates, "Returns true if label dominates other.")
             .def("cheaper_than", &PropagatorClass::cheaper_than,
                  "Returns true if label is cheaper than other, i.e., has lower cost.")
             .def("extract_path", &PropagatorClass::extract_path,
@@ -111,25 +110,25 @@
 
         pybind11::class_<FRVCP<PyPropagator::value_type>>(m, "FRVCP")
             .def(pybind11::init<const Instance&, std::shared_ptr<PyPropagator>>())
             .def("optimize", &FRVCP<PyPropagator::value_type>::optimize,
                  "Solve FRVCP for the specified route.");
 
         /*auto propagator_interface
-            = bind_propagator<vrpis::Propagator, PyPropagator>(m, "Propagator")
+            = bind_propagator<routingblocks::Propagator, PyPropagator>(m, "Propagator")
                   .def(pybind11::init<>());
 
-        bind_propagator<vrpis::ADPTWPropagation>(m, "ADPTWPropagation", propagator_interface)
-            .def(pybind11::init<const vrpis::Instance&>());
+        bind_propagator<routingblocks::ADPTWPropagation>(m, "ADPTWPropagation",
+        propagator_interface) .def(pybind11::init<const routingblocks::Instance&>());
 
-        m.def("create_adptw_propagator", [](const vrpis::Instance& instance) {
-            return std::make_shared<vrpis::ADPTWPropagation>(instance);
+        m.def("create_adptw_propagator", [](const routingblocks::Instance& instance) {
+            return std::make_shared<routingblocks::ADPTWPropagation>(instance);
         });
 
-        pybind11::class_<vrpis::Label, std::shared_ptr<vrpis::Label>>(m, "DPLabel",
+        pybind11::class_<routingblocks::Label, std::shared_ptr<routingblocks::Label>>(m, "DPLabel",
                                                                         pybind11::dynamic_attr())
             .def(pybind11::init<>());
 
         */
     }
 
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.1/bindings/src/LocalSearch.cpp` & `routingblocks-0.1.2/bindings/src/LocalSearch.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-#include "vrpis_bindings/LocalSearch.h"
-
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
+#include <routingblocks/LocalSearch.h>
+#include <routingblocks/utility/random.h>
+#include <routingblocks_bindings/LocalSearch.h>
+#include <routingblocks_bindings/Operators.h>
 
-#include "vrpis/LocalSearch.h"
-#include "vrpis/utility/random.h"
-#include "vrpis_bindings/Operators.h"
-
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
 
     void bind_local_search(pybind11::module& m) {
-        pybind11::class_<vrpis::LocalSearch>(m, "LocalSearch")
-            .def(pybind11::init<const vrpis::Instance&, std::shared_ptr<Evaluation>,
+        pybind11::class_<routingblocks::LocalSearch>(m, "LocalSearch")
+            .def(pybind11::init<const routingblocks::Instance&, std::shared_ptr<Evaluation>,
                                 std::shared_ptr<Evaluation>>())
             .def(
                 "optimize",
                 [](LocalSearch& ls, Solution& sol, std::vector<Operator*> operators) -> void {
                     ls.run(sol, operators.begin(), operators.end());
                 },
                 "Optimizes the passed solution inplace.")
@@ -30,26 +28,30 @@
                 auto origin_route_iterator = std::next(solution.begin(), origin_route);
                 auto target_route_iterator = std::next(solution.begin(), target_route);
                 auto origin_node_iterator = std::next(origin_route_iterator->begin(), origin_node);
                 auto target_node_iterator = std::next(target_route_iterator->begin(), target_node);
                 return GeneratorArc{origin_route_iterator, origin_node_iterator,
                                     target_route_iterator, target_node_iterator};
             }))
-            .def_property_readonly(
-                "origin_route",
-                [](const vrpis::GeneratorArc& arc) -> const Route& { return *arc.origin_route; })
-            .def_property_readonly(
-                "target_route",
-                [](const vrpis::GeneratorArc& arc) -> const Route& { return *arc.target_route; })
-            .def_property_readonly(
-                "origin_node",
-                [](const vrpis::GeneratorArc& arc) -> const Node& { return *arc.origin_node; })
-            .def_property_readonly(
-                "target_node",
-                [](const vrpis::GeneratorArc& arc) -> const Node& { return *arc.target_node; });
+            .def_property_readonly("origin_route",
+                                   [](const routingblocks::GeneratorArc& arc) -> const Route& {
+                                       return *arc.origin_route;
+                                   })
+            .def_property_readonly("target_route",
+                                   [](const routingblocks::GeneratorArc& arc) -> const Route& {
+                                       return *arc.target_route;
+                                   })
+            .def_property_readonly("origin_node",
+                                   [](const routingblocks::GeneratorArc& arc) -> const Node& {
+                                       return *arc.origin_node;
+                                   })
+            .def_property_readonly("target_node",
+                                   [](const routingblocks::GeneratorArc& arc) -> const Node& {
+                                       return *arc.target_node;
+                                   });
     }
 
     void bind_neighborhood_structures(pybind11::module& m) {
         bind_generator_arc<GeneratorArc>(m, "GeneratorArc");
 
         pybind11::class_<QuadraticNeighborhoodIterator>(m, "QuadraticNeighborhoodIterator");
         m.def("iter_neighborhood", [](const Solution& solution) {
@@ -57,8 +59,8 @@
                 QuadraticNeighborhoodIterator(
                     solution, {solution.begin(), solution.begin()->begin(), solution.begin(),
                                solution.begin()->begin()}),
                 QuadraticNeighborhoodIterator());
         });
     }
 
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.1/bindings/src/Operators.cpp` & `routingblocks-0.1.2/bindings/src/Operators.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,76 @@
-#include "vrpis_bindings/Operators.h"
+#include <routingblocks/LocalSearch.h>
+#include <routingblocks/operators/InsertStationOperator.h>
+#include <routingblocks/operators/InterRouteTwoOptOperator.h>
+#include <routingblocks/operators/RemoveStationOperator.h>
+#include <routingblocks/operators/SwapOperator.h>
+#include <routingblocks_bindings/Operators.h>
 
-#include <vrpis/LocalSearch.h>
-#include <vrpis/operators/InsertStationOperator.h>
-#include <vrpis/operators/InterRouteTwoOptOperator.h>
-#include <vrpis/operators/RemoveStationOperator.h>
+#include <routingblocks_bindings/binding_helpers.hpp>
 
-#include "vrpis/operators/SwapOperator.h"
-#include "vrpis_bindings/binding_helpers.hpp"
+namespace routingblocks::bindings {
 
-namespace vrpis::bindings {
-
-    class PyOperator : public vrpis::Operator {
-        using vrpis::Operator::Operator;
+    class PyOperator : public routingblocks::Operator {
+        using routingblocks::Operator::Operator;
 
       public:
         void prepare_search(const Solution& solution) override {
-            PYBIND11_OVERLOAD_PURE(void, vrpis::Operator, prepare_search, solution);
+            PYBIND11_OVERLOAD_PURE(void, routingblocks::Operator, prepare_search, solution);
         }
         std::shared_ptr<Move> find_next_improving_move(eval_t& evaluation, const Solution& solution,
                                                        const Move* previous_move) override {
-            PYBIND11_OVERLOAD_PURE(std::shared_ptr<Move>, vrpis::Operator, find_next_improving_move,
-                                   evaluation, solution, previous_move);
+            PYBIND11_OVERLOAD_PURE(std::shared_ptr<Move>, routingblocks::Operator,
+                                   find_next_improving_move, evaluation, solution, previous_move);
         }
         void finalize_search() override {
-            PYBIND11_OVERLOAD_PURE(void, vrpis::Operator, finalize_search);
+            PYBIND11_OVERLOAD_PURE(void, routingblocks::Operator, finalize_search);
         }
     };
 
-    class PyMove : public vrpis::Move {
-        using vrpis::Move::Move;
+    class PyMove : public routingblocks::Move {
+        using routingblocks::Move::Move;
 
       public:
         cost_t get_cost_delta(Evaluation& evaluation, const Instance& instance,
                               const Solution& solution) const override {
-            PYBIND11_OVERLOAD_PURE(cost_t, vrpis::Move, get_cost_delta, evaluation, instance,
-                                   solution);
+            PYBIND11_OVERLOAD_PURE(cost_t, routingblocks::Move, get_cost_delta, evaluation,
+                                   instance, solution);
         }
 
         void apply(const Instance& instance, Solution& solution) const override {
-            PYBIND11_OVERRIDE_PURE(void, vrpis::Move, apply, instance, solution);
+            PYBIND11_OVERRIDE_PURE(void, routingblocks::Move, apply, instance, solution);
         }
     };
 
     auto bind_operator_interface(pybind11::module_& m) {
-        return pybind11::class_<vrpis::Operator, PyOperator, std::shared_ptr<vrpis::Operator>>(
-                   m, "Operator")
+        return pybind11::class_<routingblocks::Operator, PyOperator,
+                                std::shared_ptr<routingblocks::Operator>>(m, "Operator")
             .def(pybind11::init<>())
-            .def("prepare_search", &vrpis::Operator::prepare_search,
+            .def("prepare_search", &routingblocks::Operator::prepare_search,
                  "Prepare the operator for "
                  "searching for a move.")
-            .def("find_next_improving_move", &vrpis::Operator::find_next_improving_move,
+            .def("find_next_improving_move", &routingblocks::Operator::find_next_improving_move,
                  "Find the next improving move.")
-            .def("finalize_search", &vrpis::Operator::finalize_search, "Finalize the search.");
+            .def("finalize_search", &routingblocks::Operator::finalize_search,
+                 "Finalize the search.");
     }
 
     auto bind_move_interface(pybind11::module_& m) {
-        return pybind11::class_<vrpis::Move, PyMove, std::shared_ptr<vrpis::Move>>(m, "Move")
+        return pybind11::class_<routingblocks::Move, PyMove, std::shared_ptr<routingblocks::Move>>(
+                   m, "Move")
             .def(pybind11::init<>())
-            .def("get_cost_delta", &vrpis::Move::get_cost_delta, "Get the cost of the move.")
-            .def("apply", &vrpis::Move::apply, "Apply the move to the solution.");
+            .def("get_cost_delta", &routingblocks::Move::get_cost_delta,
+                 "Get the cost of the move.")
+            .def("apply", &routingblocks::Move::apply, "Apply the move to the solution.");
     }
 
     template <size_t OriginSegmentSize, size_t TargetSegmentSize>
     void bind_swap_operator(pybind11::module_& m, auto& operator_interface, auto& move_interface) {
-        using operator_t = vrpis::SwapOperator<OriginSegmentSize, TargetSegmentSize>;
-        using operator_move_t = vrpis::SwapMove<OriginSegmentSize, TargetSegmentSize>;
+        using operator_t = routingblocks::SwapOperator<OriginSegmentSize, TargetSegmentSize>;
+        using operator_move_t = routingblocks::SwapMove<OriginSegmentSize, TargetSegmentSize>;
 
         std::stringstream base_name;
         base_name << "SwapOperator"
                   << "_" << OriginSegmentSize << "_" << TargetSegmentSize;
         auto base_name_str = base_name.str();
 
         pybind11::class_<operator_t, std::shared_ptr<operator_t>>(
@@ -94,71 +96,74 @@
             .def(pybind11::init<NodeLocation, NodeLocation>())
             .def("get_cost_delta", &operator_move_t::get_cost_delta)
             .def("apply", &operator_move_t::apply);
     }
 
     void bind_inter_route_two_opt(pybind11::module_& m, auto& operator_interface,
                                   auto& move_interface) {
-        pybind11::class_<vrpis::InterRouteTwoOptOperator,
-                         std::shared_ptr<vrpis::InterRouteTwoOptOperator>>(
+        pybind11::class_<routingblocks::InterRouteTwoOptOperator,
+                         std::shared_ptr<routingblocks::InterRouteTwoOptOperator>>(
             m, "InterRouteTwoOptOperator", operator_interface,
             "Considers two-opt moves between distinct routes. Tries to integrate the "
             "generator arc into the solution.")
             .def(pybind11::init<const Instance&, const utility::arc_set*>(),
                  pybind11::keep_alive<1, 3>())
-            .def("prepare_search", &vrpis::InterRouteTwoOptOperator::prepare_search)
+            .def("prepare_search", &routingblocks::InterRouteTwoOptOperator::prepare_search)
             .def("find_next_improving_move",
-                 &vrpis::InterRouteTwoOptOperator::find_next_improving_move)
-            .def("finalize_search", &vrpis::InterRouteTwoOptOperator::finalize_search)
-            .def("create_move", &vrpis::InterRouteTwoOptOperator::create_move,
+                 &routingblocks::InterRouteTwoOptOperator::find_next_improving_move)
+            .def("finalize_search", &routingblocks::InterRouteTwoOptOperator::finalize_search)
+            .def("create_move", &routingblocks::InterRouteTwoOptOperator::create_move,
                  "Create a move that represents a given generator arc.");
 
-        pybind11::class_<vrpis::InterRouteTwoOptMove, std::shared_ptr<vrpis::InterRouteTwoOptMove>>(
+        pybind11::class_<routingblocks::InterRouteTwoOptMove,
+                         std::shared_ptr<routingblocks::InterRouteTwoOptMove>>(
             m, "InterRouteTwoOptMove", move_interface)
             .def(pybind11::init<NodeLocation, NodeLocation>())
-            .def("get_cost_delta", &vrpis::InterRouteTwoOptMove::get_cost_delta)
-            .def("apply", &vrpis::InterRouteTwoOptMove::apply);
+            .def("get_cost_delta", &routingblocks::InterRouteTwoOptMove::get_cost_delta)
+            .def("apply", &routingblocks::InterRouteTwoOptMove::apply);
     }
 
     void bind_station_in_operator(pybind11::module_& m, auto& operator_interface,
                                   auto& move_interface) {
-        pybind11::class_<vrpis::InsertStationOperator,
-                         std::shared_ptr<vrpis::InsertStationOperator>>(
+        pybind11::class_<routingblocks::InsertStationOperator,
+                         std::shared_ptr<routingblocks::InsertStationOperator>>(
             m, "InsertStationOperator", operator_interface,
             "Considers station insertions between consecutive vertices.")
             .def(pybind11::init<const Instance&>())
-            .def("prepare_search", &vrpis::InsertStationOperator::prepare_search)
+            .def("prepare_search", &routingblocks::InsertStationOperator::prepare_search)
             .def("find_next_improving_move",
-                 &vrpis::InsertStationOperator::find_next_improving_move)
-            .def("finalize_search", &vrpis::InsertStationOperator::finalize_search);
+                 &routingblocks::InsertStationOperator::find_next_improving_move)
+            .def("finalize_search", &routingblocks::InsertStationOperator::finalize_search);
 
-        pybind11::class_<vrpis::InsertStationMove, std::shared_ptr<vrpis::InsertStationMove>>(
+        pybind11::class_<routingblocks::InsertStationMove,
+                         std::shared_ptr<routingblocks::InsertStationMove>>(
             m, "StationInsertionMove", move_interface)
             .def(pybind11::init<NodeLocation, VertexID>())
-            .def("get_cost_delta", &vrpis::InsertStationMove::get_cost_delta)
-            .def("apply", &vrpis::InsertStationMove::apply);
+            .def("get_cost_delta", &routingblocks::InsertStationMove::get_cost_delta)
+            .def("apply", &routingblocks::InsertStationMove::apply);
     }
 
     void bind_station_out_operator(pybind11::module_& m, auto& operator_interface,
                                    auto& move_interface) {
-        pybind11::class_<vrpis::RemoveStationOperator,
-                         std::shared_ptr<vrpis::RemoveStationOperator>>(
+        pybind11::class_<routingblocks::RemoveStationOperator,
+                         std::shared_ptr<routingblocks::RemoveStationOperator>>(
             m, "RemoveStationOperator", operator_interface,
             "Considers station removals between consecutive vertices.")
             .def(pybind11::init<const Instance&>())
-            .def("prepare_search", &vrpis::RemoveStationOperator::prepare_search)
+            .def("prepare_search", &routingblocks::RemoveStationOperator::prepare_search)
             .def("find_next_improving_move",
-                 &vrpis::RemoveStationOperator::find_next_improving_move)
-            .def("finalize_search", &vrpis::RemoveStationOperator::finalize_search);
+                 &routingblocks::RemoveStationOperator::find_next_improving_move)
+            .def("finalize_search", &routingblocks::RemoveStationOperator::finalize_search);
 
-        pybind11::class_<vrpis::RemoveStationMove, std::shared_ptr<vrpis::RemoveStationMove>>(
-            m, "StationRemovalMove", move_interface)
+        pybind11::class_<routingblocks::RemoveStationMove,
+                         std::shared_ptr<routingblocks::RemoveStationMove>>(m, "StationRemovalMove",
+                                                                            move_interface)
             .def(pybind11::init<NodeLocation>())
-            .def("get_cost_delta", &vrpis::RemoveStationMove::get_cost_delta)
-            .def("apply", &vrpis::RemoveStationMove::apply);
+            .def("get_cost_delta", &routingblocks::RemoveStationMove::get_cost_delta)
+            .def("apply", &routingblocks::RemoveStationMove::apply);
     }
 
     void bind_arc_set(pybind11::module_& m) {
         pybind11::class_<utility::arc_set>(m, "ArcSet", "A set of arcs.")
             .def(pybind11::init<VertexID>())
             .def("include_arc", &utility::arc_set::include_arc, "Include an arc in the set.")
             .def("forbid_arc", &utility::arc_set::forbid_arc, "Forbid an arc in the set.")
@@ -185,8 +190,8 @@
         bind_swap_operator<2, 2>(m, operator_interface, move_interface);
         bind_swap_operator<2, 3>(m, operator_interface, move_interface);
         bind_swap_operator<3, 1>(m, operator_interface, move_interface);
         bind_swap_operator<3, 2>(m, operator_interface, move_interface);
         bind_swap_operator<3, 3>(m, operator_interface, move_interface);
     }
 
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.1/bindings/src/Solution.cpp` & `routingblocks-0.1.2/bindings/src/Solution.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,95 @@
-#include "vrpis_bindings/Solution.h"
-
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
+#include <routingblocks/Solution.h>
+#include <routingblocks_bindings/Solution.h>
 
-#include "vrpis/Solution.h"
-#include "vrpis_bindings/binding_helpers.hpp"
+#include <routingblocks_bindings/binding_helpers.hpp>
 
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
 
     void bind_node(pybind11::module& m) {
-        pybind11::class_<vrpis::Node>(m, "Node")
-            .def(pybind11::init([](const vrpis::Vertex& vertex, pybind11::object fwd_label,
+        pybind11::class_<routingblocks::Node>(m, "Node")
+            .def(pybind11::init([](const routingblocks::Vertex& vertex, pybind11::object fwd_label,
                                    pybind11::object bwd_label) {
-                     return vrpis::Node{vertex,
-                                        {std::make_shared<pybind11::object>(std::move(fwd_label))},
-                                        {std::make_shared<pybind11::object>(std::move(bwd_label))}};
+                     return routingblocks::Node{
+                         vertex,
+                         {std::make_shared<pybind11::object>(std::move(fwd_label))},
+                         {std::make_shared<pybind11::object>(std::move(bwd_label))}};
                  }),
                  "Creates a node tracking the given vertex and initializes forward and backward"
                  "labels.")
-            .def("update_forward", &vrpis::Node::update_forward,
+            .def("update_forward", &routingblocks::Node::update_forward,
                  "Updates the forward label of this node using the given predecessor node and arc.")
-            .def("update_backward", &vrpis::Node::update_backward,
+            .def("update_backward", &routingblocks::Node::update_backward,
                  "Updates the backward label of this node using the given successor node and arc.")
-            .def_property_readonly("vertex_id", &vrpis::Node::vertex_id, "The vertex ID")
-            .def_property_readonly("vertex_strid", &vrpis::Node::vertex_strid, "The vertex StrID")
-            .def_property_readonly("vertex", &vrpis::Node::vertex,
+            .def_property_readonly("vertex_id", &routingblocks::Node::vertex_id, "The vertex ID")
+            .def_property_readonly("vertex_strid", &routingblocks::Node::vertex_strid,
+                                   "The vertex StrID")
+            .def_property_readonly("vertex", &routingblocks::Node::vertex,
                                    "The vertex associated with this node")
-            .def("cost", &vrpis::Node::cost, "The total route cost up to this node")
-            .def("cost_components", &vrpis::Node::cost_components,
+            .def("cost", &routingblocks::Node::cost, "The total route cost up to this node")
+            .def("cost_components", &routingblocks::Node::cost_components,
                  "The cost components of the route up to this node")
-            .def("feasible", &vrpis::Node::feasible, "Whether the route up to the node is feasible")
+            .def("feasible", &routingblocks::Node::feasible,
+                 "Whether the route up to the node is feasible")
             .def_property_readonly(
                 "forward_label",
                 [](const Node& node) -> const pybind11::object& {
                     return node.forward_label().get<pybind11::object>();
                 },
                 "Forward label at the node", pybind11::return_value_policy::reference_internal)
             .def_property_readonly(
                 "backward_label",
                 [](const Node& node) -> const pybind11::object& {
                     return node.backward_label().get<pybind11::object>();
                 },
                 "Backward label at the node", pybind11::return_value_policy::reference_internal)
-            .def_property_readonly("__str__", &vrpis::Node::vertex_strid);
+            .def_property_readonly("__str__", &routingblocks::Node::vertex_strid);
     }
 
     void bind_route(pybind11::module& m) {
-        pybind11::class_<vrpis::Route>(m, "Route")
+        pybind11::class_<routingblocks::Route>(m, "Route")
             .def(pybind11::init<std::shared_ptr<Evaluation>, const Instance&>(),
                  "Creates an empty route.")
-            .def_property_readonly("cost", &vrpis::Route::cost, "The cost of the route.")
-            .def_property_readonly("cost_components", &vrpis::Route::cost_components,
+            .def_property_readonly("cost", &routingblocks::Route::cost, "The cost of the route.")
+            .def_property_readonly("cost_components", &routingblocks::Route::cost_components,
                                    "The cost components of the route.")
-            .def_property_readonly("feasible", &vrpis::Route::feasible,
+            .def_property_readonly("feasible", &routingblocks::Route::feasible,
                                    "Whether the route is feasible.")
-            .def_property_readonly("empty", &vrpis::Route::empty, "Whether the route is empty.")
-            .def_property_readonly("modification_timestamp", &vrpis::Route::modification_timestamp,
+            .def_property_readonly("empty", &routingblocks::Route::empty,
+                                   "Whether the route is empty.")
+            .def_property_readonly("modification_timestamp",
+                                   &routingblocks::Route::modification_timestamp,
                                    "The route modification_timestamp. May be used for caching.")
-            .def("__len__", &vrpis::Route::size, "The number of vertices in the route.")
+            .def("__len__", &routingblocks::Route::size, "The number of vertices in the route.")
             .def("__copy__", [](const Route& r) { return Route(r); })
             .def("__deepcopy__", [](const Route& r, const pybind11::dict&) { return Route(r); })
             .def_property_readonly(
-                "end_depot", [](const Route& r) -> const vrpis::Node& { return *r.end_depot(); },
+                "end_depot",
+                [](const Route& r) -> const routingblocks::Node& { return *r.end_depot(); },
                 "The depot at the end of the route.",
                 pybind11::return_value_policy::reference_internal)
             .def_property_readonly(
-                "depot", [](const Route& r) -> const vrpis::Node& { return *r.begin(); },
+                "depot", [](const Route& r) -> const routingblocks::Node& { return *r.begin(); },
                 "Starting depot of the route.", pybind11::return_value_policy::reference_internal)
             .def(
                 "__getitem__",
-                [](const vrpis::Route& route, size_t pos) -> const vrpis::Node& {
+                [](const routingblocks::Route& route, size_t pos) -> const routingblocks::Node& {
                     return *std::next(route.begin(), pos);
                 },
                 "The node at the given index.", pybind11::return_value_policy::reference_internal)
             .def(
                 "__iter__",
                 [](const Route& route) {
                     return pybind11::make_iterator(route.begin(), route.end());
                 },
                 pybind11::return_value_policy::reference_internal)
-            .def("__str__", ::bindings::helpers::ostream_to_string<vrpis::Route>)
-            .def("__repr__", ::bindings::helpers::ostream_to_string<vrpis::Route>)
+            .def("__str__", ::bindings::helpers::ostream_to_string<routingblocks::Route>)
+            .def("__repr__", ::bindings::helpers::ostream_to_string<routingblocks::Route>)
             .def(
                 "remove_segment",
                 [](Route& route, size_t begin_pos, size_t end_pos) {
                     auto ret = route.remove_segment(std::next(route.begin(), begin_pos),
                                                     std::next(route.begin(), end_pos));
                     return std::distance(route.begin(), ret);
                 },
@@ -126,62 +131,65 @@
                          // Inter-route exchange
                          return route.exchange_segments(begin, end, other_begin, other_end, other);
                      } else {
                          // Intra-route exchange
                          return route.exchange_segments(begin, end, other_begin, other_end);
                      }
                  })
-            .def("update", pybind11::overload_cast<>(&vrpis::Route::update), "Updates the route.")
-            .def("__eq__", &vrpis::Route::operator==, "Whether the routes are equal.")
-            .def("__ne__", &vrpis::Route::operator!=, "Whether the routes are not equal.");
+            .def("update", pybind11::overload_cast<>(&routingblocks::Route::update),
+                 "Updates the route.")
+            .def("__eq__", &routingblocks::Route::operator==, "Whether the routes are equal.")
+            .def("__ne__", &routingblocks::Route::operator!=, "Whether the routes are not equal.");
 
-        m.def("create_route", &vrpis::create_route_from_vector,
+        m.def("create_route", &routingblocks::create_route_from_vector,
               "Creates a route from the given vertices.");
     }
 
     void bind_node_location(pybind11::module_& m) {
-        pybind11::class_<vrpis::NodeLocation>(m, "NodeLocation")
+        pybind11::class_<routingblocks::NodeLocation>(m, "NodeLocation")
             .def(pybind11::init<unsigned int, unsigned int>())
             .def("__getitem__",
-                 [](const vrpis::NodeLocation& location, size_t pos) {
+                 [](const routingblocks::NodeLocation& location, size_t pos) {
                      switch (pos) {
                          case 0:
                              return location.route;
                          case 1:
                              return location.position;
                          default:
                              throw std::out_of_range("Index out of range");
                      }
                  })
-            .def("__len__", [](const vrpis::NodeLocation&) { return 2; })
-            .def_readwrite("route", &vrpis::NodeLocation::route, "The route index.")
-            .def_readwrite("position", &vrpis::NodeLocation::position, "The position in the route.")
-            .def("__eq__", &vrpis::NodeLocation::operator==,
+            .def("__len__", [](const routingblocks::NodeLocation&) { return 2; })
+            .def_readwrite("route", &routingblocks::NodeLocation::route, "The route index.")
+            .def_readwrite("position", &routingblocks::NodeLocation::position,
+                           "The position in the route.")
+            .def("__eq__", &routingblocks::NodeLocation::operator==,
                  "Whether the node locations are equal.")
-            .def("__ne__", &vrpis::NodeLocation::operator!=,
+            .def("__ne__", &routingblocks::NodeLocation::operator!=,
                  "Whether the node locations are not equal.")
-            .def("__lt__", &vrpis::NodeLocation::operator<,
+            .def("__lt__", &routingblocks::NodeLocation::operator<,
                  "Whether the node locations compare lexicographically smaller. Route index is "
                  "ordered before node position.")
-            .def("__str__", ::bindings::helpers::ostream_to_string<vrpis::NodeLocation>)
-            .def("__repr__", ::bindings::helpers::ostream_to_string<vrpis::NodeLocation>);
+            .def("__str__", ::bindings::helpers::ostream_to_string<routingblocks::NodeLocation>)
+            .def("__repr__", ::bindings::helpers::ostream_to_string<routingblocks::NodeLocation>);
     }
 
     void bind_solution(pybind11::module_& m) {
         bind_node_location(m);
 
-        pybind11::class_<vrpis::Solution>(m, "Solution")
+        pybind11::class_<routingblocks::Solution>(m, "Solution")
             .def(pybind11::init<std::shared_ptr<Evaluation>, const Instance&, size_t>(),
                  "Creates an empty solution with the specified number of routes.")
             .def(pybind11::init<std::shared_ptr<Evaluation>, const Instance&, std::vector<Route>>(),
                  "Creates a solution from the specified routes.")
-            .def_property_readonly("cost", &vrpis::Solution::cost, "The cost of the solution.")
-            .def_property_readonly("cost_components", &vrpis::Solution::cost_components,
+            .def_property_readonly("cost", &routingblocks::Solution::cost,
+                                   "The cost of the solution.")
+            .def_property_readonly("cost_components", &routingblocks::Solution::cost_components,
                                    "The cost components of the solution.")
-            .def_property_readonly("feasible", &vrpis::Solution::feasible,
+            .def_property_readonly("feasible", &routingblocks::Solution::feasible,
                                    "Whether the solution is "
                                    "feasible.")
             .def("__copy__", [](const Solution& s) { return Solution(s); })
             .def("__deepcopy__",
                  [](const Solution& s, const pybind11::dict&) -> Solution { return Solution(s); })
             .def(
                 "__iter__",
@@ -192,28 +200,28 @@
             .def_property_readonly(
                 "routes",
                 [](const Solution& solution) {
                     return pybind11::make_iterator(solution.begin(), solution.end());
                 },
                 "Iterator over the routes in the solution.",
                 pybind11::return_value_policy::reference_internal)
-            .def("__len__", &vrpis::Solution::size, "The number of routes in the solution.")
+            .def("__len__", &routingblocks::Solution::size, "The number of routes in the solution.")
             .def_property_readonly(
                 "number_of_non_depot_nodes",
-                [](const Solution& sol) { return vrpis::number_of_nodes(sol, false); },
+                [](const Solution& sol) { return routingblocks::number_of_nodes(sol, false); },
                 "The number of non-depot nodes in the solution.")
             .def_property_readonly(
                 "number_of_insertion_points",
-                [](const Solution& sol) { return vrpis::number_of_nodes(sol, true); },
+                [](const Solution& sol) { return routingblocks::number_of_nodes(sol, true); },
                 "The number of possible insertion points in the solution.")
             .def_property_readonly(
                 "insertion_points",
                 [](const Solution& sol) {
                     std::vector<NodeLocation> locations;
-                    locations.reserve(vrpis::number_of_nodes(sol, true));
+                    locations.reserve(routingblocks::number_of_nodes(sol, true));
                     size_t route_index = 0;
                     for (auto route = sol.begin(); route != sol.end(); ++route, ++route_index) {
                         size_t node_position = 0;
                         for (auto node = route->begin(); node != route->end_depot();
                              ++node, ++node_position) {
                             locations.emplace_back(route_index, node_position);
                         }
@@ -222,42 +230,42 @@
                 },
                 pybind11::return_value_policy::move,
                 "A list of possible insertion points in the solution.")
             .def_property_readonly(
                 "non_depot_nodes",
                 [](const Solution& sol) {
                     std::vector<NodeLocation> locations;
-                    locations.reserve(vrpis::number_of_nodes(sol, true));
+                    locations.reserve(routingblocks::number_of_nodes(sol, true));
                     size_t route_index = 0;
                     for (auto route = sol.begin(); route != sol.end(); ++route, ++route_index) {
                         size_t node_position = 1;
                         for (auto node = std::next(route->begin()); node != route->end_depot();
                              ++node, ++node_position) {
                             locations.emplace_back(route_index, node_position);
                         }
                     }
                     return locations;
                 },
                 pybind11::return_value_policy::move,
                 "Returns a list of all non-depot nodes in the solution.")
             .def(
                 "__getitem__",
-                [](const Solution& solution, size_t pos) -> const vrpis::Route& {
+                [](const Solution& solution, size_t pos) -> const routingblocks::Route& {
                     return *std::next(solution.begin(), pos);
                 },
                 "The route at the given index.", pybind11::return_value_policy::reference_internal)
             .def(
                 "lookup",
                 [](const Solution& sol, const NodeLocation& location) -> const Node* {
                     return to_ref(location, sol).second;
                 },
                 pybind11::return_value_policy::reference_internal,
                 "Get the node at the given "
                 "location.")
-            .def("find", &vrpis::Solution::find,
+            .def("find", &routingblocks::Solution::find,
                  "Finds locations where the given vertex occurs in the solution.")
             .def(
                 "exchange_segment",
                 [](Solution& solution, size_t route_index, size_t begin_pos, size_t end_pos,
                    size_t other_route_index, size_t other_begin_pos, size_t other_end_pos) {
                     auto route = std::next(solution.begin(), route_index);
                     auto other = std::next(solution.begin(), other_route_index);
@@ -321,46 +329,48 @@
                     if (route.has_value()) {
                         sol.add_route(**route);
                     } else {
                         sol.add_route();
                     }
                 },
                 pybind11::arg("route") = std::nullopt, "Adds an empty route to the solution.")
-            .def("__str__", &::bindings::helpers::ostream_to_string<vrpis::Solution>)
-            .def("__eq__", &vrpis::Solution::operator==, "Whether the solutions are equal.")
-            .def("__ne__", &vrpis::Solution::operator!=, "Whether the solutions are not equal.");
+            .def("__str__", &::bindings::helpers::ostream_to_string<routingblocks::Solution>)
+            .def("__eq__", &routingblocks::Solution::operator==, "Whether the solutions are equal.")
+            .def("__ne__", &routingblocks::Solution::operator!=,
+                 "Whether the solutions are not equal.");
     }
 
     class RouteSegment {
         // TODO
-        friend vrpis::route_segment cast_route_segment(const RouteSegment&);
+        friend routingblocks::route_segment cast_route_segment(const RouteSegment&);
         const Route& route;
         size_t begin;
         size_t end;
 
       public:
-        constexpr RouteSegment(const vrpis::Route& route, size_t begin, size_t end)
+        constexpr RouteSegment(const routingblocks::Route& route, size_t begin, size_t end)
             : route(route), begin(begin), end(end){};
 
-        /*operator vrpis::route_segment<vrpis::Route::const_iterator>() const {
-            return vrpis::route_segment(std::next(route.begin(), begin),
+        /*operator routingblocks::route_segment<routingblocks::Route::const_iterator>() const {
+            return routingblocks::route_segment(std::next(route.begin(), begin),
                                         std::next(route.begin(), end));
         }*/
     };
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
 
 namespace {
-    vrpis::route_segment cast_route_segment(const vrpis::bindings::RouteSegment& segment) {
+    routingblocks::route_segment cast_route_segment(
+        const routingblocks::bindings::RouteSegment& segment) {
         throw std::runtime_error("Not implemented!");
-        /*return vrpis::route_segment(std::next(segment.route.begin(), segment.begin),
+        /*return routingblocks::route_segment(std::next(segment.route.begin(), segment.begin),
                                     std::next(segment.route.begin(), segment.end));*/
     }
 }  // namespace
 
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
 
     void bind_solution_functions(pybind11::module& m) {
         pybind11::class_<RouteSegment>(m, "RouteSegment")
             .def(pybind11::init<const Route&, size_t, size_t>());
 
         m.def("evaluate_insertion",
               [](Evaluation& evaluation, const Instance& instance, const Route& route,
@@ -389,8 +399,8 @@
                     evaluation, instance,
                     route_segment{route.begin(), std::next(route.begin(), pred_index + 1)},
                     route_segment{std::next(route.begin(), succ_index), route.end()});
             },
             "Compute the cost of the route resulting from concatenating the route segment ending "
             "at pred with the route segment starting at succ. Shorthand method for concatenate.");
     }
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.1/bindings/src/large_neighborhood.cpp` & `routingblocks-0.1.2/bindings/src/large_neighborhood.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,128 @@
-#include "vrpis_bindings/large_neighborhood.h"
-
 #include <pybind11/stl.h>
-#include <vrpis/Instance.h>
-#include <vrpis/lns_operators.h>
-
-#include <vrpis/adaptive_large_neighborhood.hpp>
+#include <routingblocks/Instance.h>
+#include <routingblocks/lns_operators.h>
+#include <routingblocks/operators.h>
+#include <routingblocks_bindings/large_neighborhood.h>
 
-#include "vrpis/operators.h"
-#include "vrpis_bindings/binding_helpers.hpp"
+#include <routingblocks/adaptive_large_neighborhood.hpp>
+#include <routingblocks_bindings/binding_helpers.hpp>
 
 /*
  * Couple the lifetime of objects created in python to the shared_ptr lifetime in c++.
  */
 
-BIND_LIFETIME_PYTHON(vrpis::repair_operator, "RepairOperator")
-BIND_LIFETIME_PYTHON(vrpis::destroy_operator, "DestroyOperator")
+BIND_LIFETIME_PYTHON(routingblocks::repair_operator, "RepairOperator")
+BIND_LIFETIME_PYTHON(routingblocks::destroy_operator, "DestroyOperator")
 
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
 
-    class py_repair_operator : public vrpis::repair_operator {
+    class py_repair_operator : public routingblocks::repair_operator {
       public:
-        using vrpis::repair_operator::repair_operator;
+        using routingblocks::repair_operator::repair_operator;
 
         void apply(Evaluation& evaluation, Solution& sol,
-                   const std::vector<vrpis::VertexID>& missing_vertices) override {
-            PYBIND11_OVERRIDE_PURE(void, vrpis::repair_operator, apply, evaluation, sol,
+                   const std::vector<routingblocks::VertexID>& missing_vertices) override {
+            PYBIND11_OVERRIDE_PURE(void, routingblocks::repair_operator, apply, evaluation, sol,
                                    missing_vertices);
         }
         std::string_view name() const override {
-            PYBIND11_OVERRIDE_PURE(std::string_view, vrpis::repair_operator, name, );
+            PYBIND11_OVERRIDE_PURE(std::string_view, routingblocks::repair_operator, name, );
         }
 
-        bool can_apply_to(const vrpis::Solution& sol) const override {
-            PYBIND11_OVERRIDE_PURE(bool, vrpis::repair_operator, can_apply_to, sol);
+        bool can_apply_to(const routingblocks::Solution& sol) const override {
+            PYBIND11_OVERRIDE_PURE(bool, routingblocks::repair_operator, can_apply_to, sol);
         }
     };
 
     auto bind_repair_operator_interface(pybind11::module_& m) {
-        return pybind11::class_<vrpis::repair_operator, py_repair_operator,
-                                std::shared_ptr<vrpis::repair_operator>>(m, "RepairOperator")
+        return pybind11::class_<routingblocks::repair_operator, py_repair_operator,
+                                std::shared_ptr<routingblocks::repair_operator>>(m,
+                                                                                 "RepairOperator")
             .def(pybind11::init<>())
-            .def("apply", &vrpis::repair_operator::apply,
+            .def("apply", &routingblocks::repair_operator::apply,
                  "Apply the repair operator to the passed solution.")
-            .def("name", &vrpis::repair_operator::name, "Returns the name of the repair operator.")
-            .def("can_apply_to", &vrpis::repair_operator::can_apply_to,
+            .def("name", &routingblocks::repair_operator::name,
+                 "Returns the name of the repair operator.")
+            .def("can_apply_to", &routingblocks::repair_operator::can_apply_to,
                  "Returns true if the repair operator can be applied to the passed solution. False "
                  "otherwise.");
     }
 
-    class py_destroy_operator : public vrpis::destroy_operator {
+    class py_destroy_operator : public routingblocks::destroy_operator {
       public:
-        using vrpis::destroy_operator::destroy_operator;
+        using routingblocks::destroy_operator::destroy_operator;
 
-        std::vector<vrpis::VertexID> apply(Evaluation& evaluation, vrpis::Solution& sol,
-                                           size_t numberOfRemovedCustomers) override {
-            PYBIND11_OVERRIDE_PURE(std::vector<vrpis::VertexID>, vrpis::destroy_operator, apply,
-                                   evaluation, sol, numberOfRemovedCustomers);
+        std::vector<routingblocks::VertexID> apply(Evaluation& evaluation,
+                                                   routingblocks::Solution& sol,
+                                                   size_t numberOfRemovedCustomers) override {
+            PYBIND11_OVERRIDE_PURE(std::vector<routingblocks::VertexID>,
+                                   routingblocks::destroy_operator, apply, evaluation, sol,
+                                   numberOfRemovedCustomers);
         }
         std::string_view name() const override {
-            PYBIND11_OVERRIDE_PURE(std::string_view, vrpis::destroy_operator, name, );
+            PYBIND11_OVERRIDE_PURE(std::string_view, routingblocks::destroy_operator, name, );
         }
 
-        bool can_apply_to(const vrpis::Solution& sol) const override {
-            PYBIND11_OVERRIDE_PURE(bool, vrpis::destroy_operator, can_apply_to, sol);
+        bool can_apply_to(const routingblocks::Solution& sol) const override {
+            PYBIND11_OVERRIDE_PURE(bool, routingblocks::destroy_operator, can_apply_to, sol);
         };
     };
 
     auto bind_destroy_operator_interface(pybind11::module_& m) {
-        return pybind11::class_<vrpis::destroy_operator, py_destroy_operator,
-                                std::shared_ptr<vrpis::destroy_operator>>(m, "DestroyOperator")
+        return pybind11::class_<routingblocks::destroy_operator, py_destroy_operator,
+                                std::shared_ptr<routingblocks::destroy_operator>>(m,
+                                                                                  "DestroyOperator")
             .def(pybind11::init<>())
-            .def("apply", &vrpis::destroy_operator::apply,
+            .def("apply", &routingblocks::destroy_operator::apply,
                  "Apply the destroy operator to the passed solution and return the id's of any "
                  "removed vertices. May contain the same vertex several times.")
-            .def("name", &vrpis::destroy_operator::name,
+            .def("name", &routingblocks::destroy_operator::name,
                  "Returns the name of the destroy operator.")
-            .def("can_apply_to", &vrpis::destroy_operator::can_apply_to,
+            .def("can_apply_to", &routingblocks::destroy_operator::can_apply_to,
                  "Returns true if the destroy operator can be applied to the passed solution. "
                  "False otherwise.");
     }
 
     void bind_helpers(pybind11::module_& m) {
-        m.def("sample_positions", &vrpis::lns::operators::sample_positions,
+        m.def("sample_positions", &routingblocks::lns::operators::sample_positions,
               "Samples k positions with replacement from the solution. Can optionally include the "
               "start depot.");
     }
 
     auto bind_random_destory_operator(pybind11::module_& m, auto& interface) {
-        using _operator = vrpis::lns::operators::RandomRemoval;
+        using _operator = routingblocks::lns::operators::RandomRemoval;
         return pybind11::class_<_operator, std::shared_ptr<_operator>>(m, "RandomRemoveOperator",
                                                                        interface)
-            .def(pybind11::init<vrpis::utility::random&>())
+            .def(pybind11::init<routingblocks::utility::random&>())
             .def("apply", &_operator::apply, "Remove random vertices from the solution.")
             .def("name", &_operator::name)
             .def("can_apply_to", &_operator::can_apply_to,
                  "Returns true. Random remove is always possible.");
     }
 
     void bind_random_insertion_operator(pybind11::module_& m, auto& interface) {
-        using _operator = vrpis::lns::operators::RandomInsertion;
+        using _operator = routingblocks::lns::operators::RandomInsertion;
         pybind11::class_<_operator, std::shared_ptr<_operator>>(m, "RandomInsertionOperator",
                                                                 interface)
-            .def(pybind11::init<vrpis::utility::random&>())
+            .def(pybind11::init<routingblocks::utility::random&>())
             .def("apply", &_operator ::apply,
                  "Inserts the passed vertices in order at random locations.")
             .def("name", &_operator ::name)
             .def("can_apply_to", &_operator ::can_apply_to,
                  "Return true: random insertion is always possible.");
     }
 
     void bind_large_neighborhood(pybind11::module_& m) {
-        using lns_t = vrpis::adaptive_large_neighborhood;
+        using lns_t = routingblocks::adaptive_large_neighborhood;
         using destroy_operator_t = lns_t::destroy_operator_type;
         using repair_operator_t = lns_t::repair_operator_type;
         bind_helpers(m);
-        pybind11::class_<vrpis::adaptive_large_neighborhood>(m, "AdaptiveLargeNeighborhood")
-            .def(pybind11::init<vrpis::utility::random, double>())
+        pybind11::class_<routingblocks::adaptive_large_neighborhood>(m, "AdaptiveLargeNeighborhood")
+            .def(pybind11::init<routingblocks::utility::random, double>())
             .def(
                 "generate",
                 [](lns_t& lns, Evaluation& evaluation, Solution& sol,
                    size_t num_removed_customers) {
                     auto operator_pick = lns.generate(evaluation, sol, num_removed_customers);
                     return std::make_pair(*operator_pick.first, *operator_pick.second);
                 },
@@ -154,31 +157,31 @@
                 [](lns_t& lns, const destroy_operator_t& destroy_operator) {
                     auto iter = std::find(lns.destroy_operators_begin(),
                                           lns.destroy_operators_end(), destroy_operator);
                     assert(iter != lns.destroy_operators_end());
                     lns.remove_operator(iter);
                 },
                 "Removes the references destroy operator from the large neighborhood.")
-            .def_property_readonly("destroy_operators",
-                                   [](const vrpis::adaptive_large_neighborhood& vrpis) {
-                                       return pybind11::make_iterator(
-                                           vrpis.destroy_operators_begin(),
-                                           vrpis.destroy_operators_end());
-                                   })
-            .def_property_readonly("repair_operators",
-                                   [](const vrpis::adaptive_large_neighborhood& vrpis) {
-                                       return pybind11::make_iterator(
-                                           vrpis.repair_operators_begin(),
-                                           vrpis.repair_operators_end());
-                                   })
+            .def_property_readonly(
+                "destroy_operators",
+                [](const routingblocks::adaptive_large_neighborhood& routingblocks) {
+                    return pybind11::make_iterator(routingblocks.destroy_operators_begin(),
+                                                   routingblocks.destroy_operators_end());
+                })
+            .def_property_readonly(
+                "repair_operators",
+                [](const routingblocks::adaptive_large_neighborhood& routingblocks) {
+                    return pybind11::make_iterator(routingblocks.repair_operators_begin(),
+                                                   routingblocks.repair_operators_end());
+                })
             .def("reset_operator_weights",
-                 &vrpis::adaptive_large_neighborhood::reset_operator_weights,
+                 &routingblocks::adaptive_large_neighborhood::reset_operator_weights,
                  "Sets the weights of all operators to 1 and resets collected scores.")
             .def("adapt_operator_weights",
-                 &vrpis::adaptive_large_neighborhood::adapt_operator_weights,
+                 &routingblocks::adaptive_large_neighborhood::adapt_operator_weights,
                  "Adapts the weights of all operators based on the recorded performance. Resets "
                  "collected scores.")
             .def(
                 "collect_score",
                 [](lns_t& neighborhood, const destroy_operator_t& destroy_operator,
                    const repair_operator_t& repair_operator, double score) {
                     neighborhood.collect_score(
@@ -194,8 +197,8 @@
         auto destroy_operator_interface = bind_destroy_operator_interface(m);
         auto repair_operator_interface = bind_repair_operator_interface(m);
 
         bind_random_insertion_operator(m, repair_operator_interface);
         bind_random_destory_operator(m, destroy_operator_interface);
     }
 
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.1/bindings/src/utility.cpp` & `routingblocks-0.1.2/bindings/src/utility.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-#include "vrpis_bindings/utility.h"
-
 #include <pybind11/stl.h>
+#include <routingblocks/insertion_cache.h>
+#include <routingblocks/lns_operators.h>
+#include <routingblocks/removal_cache.h>
+#include <routingblocks/utility/random.h>
+#include <routingblocks_bindings/utility.h>
 
-#include "vrpis/lns_operators.h"
-#include "vrpis/utility/insertion_cache.h"
-#include "vrpis/utility/random.h"
-#include "vrpis/utility/removal_cache.h"
-
-namespace vrpis::bindings {
+namespace routingblocks::bindings {
     void bind_removal_cache(pybind11::module_& m) {
-        using cache_t = vrpis::utility::removal_cache<>;
+        using cache_t = routingblocks::utility::removal_cache<>;
 
         pybind11::class_<cache_t::move_t>(m, "RemovalMove")
             .def(pybind11::init<VertexID, NodeLocation, resource_t>())
             .def_readwrite("vertex_id", &cache_t::move_t::vertex_id)
             .def_readwrite("node_location", &cache_t::move_t::node_location,
                            pybind11::return_value_policy::reference_internal)
             .def_readwrite("delta_cost", &cache_t::move_t::delta_cost)
@@ -33,15 +31,15 @@
                     return std::vector<cache_t::move_t>(cache.begin(), cache.end());
                 },
                 "Returns the list of moves in the cache ordered by their cost delta in "
                 "increasing order.");
     }
 
     void bind_insertion_cache(pybind11::module_& m) {
-        using cache_t = vrpis::utility::insertion_cache<>;
+        using cache_t = routingblocks::utility::insertion_cache<>;
 
         pybind11::class_<cache_t::move_t>(m, "InsertionMove")
             .def(pybind11::init<VertexID, NodeLocation, resource_t>())
             .def_readwrite("vertex_id", &cache_t::move_t::vertex_id)
             .def_readwrite("after_node", &cache_t::move_t::after_node,
                            pybind11::return_value_policy::reference_internal)
             .def_readwrite("delta_cost", &cache_t::move_t::delta_cost)
@@ -89,37 +87,37 @@
                     return std::vector<cache_t::move_t>(cache.begin(), cache.end());
                 },
                 "Returns the list of moves in the cache ordered by their cost delta in "
                 "increasing order.");
     }
 
     void bind_random(pybind11::module_& m) {
-        pybind11::class_<vrpis::utility::random>(m, "Random")
+        pybind11::class_<routingblocks::utility::random>(m, "Random")
             .def(pybind11::init<>(),
                  "Initialize random number generator with a seed based on the current time.")
             .def(pybind11::init<uint64_t>(), "Initialize the random number generator with a seed.")
             .def(
                 "randint",
-                [](vrpis::utility::random& r, size_t min, size_t max) {
+                [](routingblocks::utility::random& r, size_t min, size_t max) {
                     return r.generateInt(min, max);
                 },
                 "Generates a random integer between min and max")
             .def(
                 "uniform",
-                [](vrpis::utility::random& r, double min, double max) {
+                [](routingblocks::utility::random& r, double min, double max) {
                     return r.uniform(min, max);
                 },
                 "Generates a random float between min and max");
     }
 
     void bind_algorithms(pybind11::module_& m) {
-        m.def("sample_locations", &vrpis::lns::operators::sample_positions,
+        m.def("sample_locations", &routingblocks::lns::operators::sample_positions,
               "Samples node locations for the passed solution.");
     }
 
     void bind_utility(pybind11::module_& m) {
         bind_random(m);
         bind_removal_cache(m);
         bind_insertion_cache(m);
         bind_algorithms(m);
     }
-}  // namespace vrpis::bindings
+}  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.1/docs/make.bat` & `routingblocks-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/docs/source/conf.py` & `routingblocks-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/__main__.py` & `routingblocks-0.1.2/examples/evrptw/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/alns.py` & `routingblocks-0.1.2/examples/evrptw/alns.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/config.json` & `routingblocks-0.1.2/examples/evrptw/config.json`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instance/interface.py` & `routingblocks-0.1.2/examples/evrptw/instance/interface.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instance/models.py` & `routingblocks-0.1.2/examples/evrptw/instance/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instance/parsing.py` & `routingblocks-0.1.2/examples/evrptw/instance/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/c101C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/c101C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/c104C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/c104C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/c202C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/c202C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/c205C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/c205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/r102C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/r102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/r103C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/r103C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/r201C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/r201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/r203C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/r203C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/rc102C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/rc102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/rc108C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/rc108C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/rc201C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/rc201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/10/rc205C10.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/10/rc205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c101_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c102_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c103_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c104_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c105_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c106_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c107_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c108_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c109_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c201_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c202_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c203_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c204_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c205_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c206_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c207_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/c208_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/c208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r101_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r102_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r103_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r104_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r105_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r106_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r107_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r108_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r109_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r110_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r110_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r111_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r111_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r112_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r112_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r201_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r202_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r203_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r204_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r205_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r206_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r207_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r208_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r209_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r209_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r210_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r210_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/r211_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/r211_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc101_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc102_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc103_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc104_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc105_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc106_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc107_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc108_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc201_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc202_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc203_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc204_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc205_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc206_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc207_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/100/rc208_21.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/100/rc208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/c103C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/c103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/c106C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/c106C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/c202C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/c202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/c208C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/c208C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/r102C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/r102C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/r105C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/r105C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/r202C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/r202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/r209C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/r209C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/rc103C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/rc103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/rc108C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/rc108C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/rc202C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/rc202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/15/rc204C15.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/15/rc204C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/c101C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/c103C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/c103C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/c206C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/c206C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/c208C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/c208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/r104C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/r104C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/r105C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/r105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/r202C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/r202C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/r203C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/r203C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/rc105C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/rc105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/rc108C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/rc108C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/rc204C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/rc204C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/5/rc208C5.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/5/rc208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/instances/evrptw/README.txt` & `routingblocks-0.1.2/examples/evrptw/instances/evrptw/README.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/operators/ShawMoveSelector.py` & `routingblocks-0.1.2/examples/evrptw/operators/ShawMoveSelector.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/operators/ShawRelatedness.py` & `routingblocks-0.1.2/examples/evrptw/operators/ShawRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/operators/SpatioTemporalRelatedness.py` & `routingblocks-0.1.2/examples/evrptw/operators/SpatioTemporalRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/examples/evrptw/operators/__init__.py` & `routingblocks-0.1.2/examples/evrptw/operators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import routingblocks
-from examples.evrptw.operators.ShawMoveSelector import ShawMoveSelector
-from examples.evrptw.operators.ShawRelatedness import ShawRelatedness
-from examples.evrptw.operators.SpatioTemporalRelatedness import SpatioTemporalRelatedness
+from evrptw.operators.ShawMoveSelector import ShawMoveSelector
+from evrptw.operators.ShawRelatedness import ShawRelatedness
+from evrptw.operators.SpatioTemporalRelatedness import SpatioTemporalRelatedness
 from routingblocks.operators.related_removal import RelatedRemovalOperator, build_relatedness_matrix
 from routingblocks.operators.move_selectors import random_selector_factory, first_move_selector
 
 
 def create_shaw_remove_operator(py_instance, cpp_instance, randgen: routingblocks.Random, distance_weight=1.0,
                                 demand_weight=1.0, time_weight=1.0, shaw_exponent=1.0):
     relatedness_matrix = build_relatedness_matrix(cpp_instance,
@@ -15,15 +15,16 @@
     return RelatedRemovalOperator(
         relatedness_matrix=relatedness_matrix,
         move_selector=ShawMoveSelector(py_instance, cpp_instance, randgen, shaw_exponent=shaw_exponent),
         seed_selector=random_selector_factory(randgen),
         initial_seed_selector=first_move_selector)
 
 
-def create_related_remove_operator(py_instance, cpp_instance, randgen: routingblocks.Random, tw_shift_weight, slack_weight):
+def create_related_remove_operator(py_instance, cpp_instance, randgen: routingblocks.Random, tw_shift_weight,
+                                   slack_weight):
     relatedness_matrix = build_relatedness_matrix(cpp_instance,
                                                   SpatioTemporalRelatedness(py_instance, cpp_instance,
                                                                             slack_weight=slack_weight,
                                                                             tw_shift_weight=tw_shift_weight))
     return RelatedRemovalOperator(
         relatedness_matrix=relatedness_matrix,
         move_selector=first_move_selector,
```

### Comparing `routingblocks-0.1.1/examples/evrptw/parameters.py` & `routingblocks-0.1.2/examples/evrptw/parameters.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/CMakeLists.txt` & `routingblocks-0.1.2/native/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 cmake_minimum_required(VERSION 3.15)
 
-project(VRPIS VERSION 0.1 LANGUAGES CXX)
+project(routingblocks VERSION 0.1 LANGUAGES CXX)
 
 include(${CMAKE_CURRENT_SOURCE_DIR}/cmake/CPM.cmake)
 include(${CMAKE_CURRENT_SOURCE_DIR}/cmake/tools.cmake)
 
 option(${PROJECT_NAME}_BUILD_TESTS on)
 option(${PROJECT_NAME}_ENABLE_ASAN off)
 option(${PROJECT_NAME}_BUILD_NATIVE off)
 option(${PROJECT_NAME}_ENABLE_LTO on)
 
-CPMAddPackage(
-        NAME fmt
-        GIT_TAG 8.1.1
-        GITHUB_REPOSITORY fmtlib/fmt
-        OPTIONS "FMT_INSTALL YES" # create an installable target
-)
-set_target_properties(fmt PROPERTIES POSITION_INDEPENDENT_CODE ON)
-
 add_subdirectory(lib)
 
-file(GLOB_RECURSE headers CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/include/vrpis/*.h")
-file(GLOB_RECURSE public_headers CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/include/vrpis/interfaces/*.h")
+file(GLOB_RECURSE headers CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/include/routingblocks/*.h")
 file(GLOB_RECURSE sources CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp")
 
-add_library(${PROJECT_NAME} ${headers} ${sources})
-target_link_libraries(${PROJECT_NAME} PUBLIC fmt::fmt)
+add_library(${PROJECT_NAME} STATIC ${headers} ${sources})
 target_link_libraries(${PROJECT_NAME} PUBLIC XOSHIRO)
 target_link_libraries(${PROJECT_NAME} PUBLIC DYNAMIC_BITSET)
 target_link_libraries(${PROJECT_NAME} PUBLIC SMALL_VECTOR)
 set_target_properties(${PROJECT_NAME} PROPERTIES CXX_STANDARD 20 POSITION_INDEPENDENT_CODE ON)
 set_target_properties(${PROJECT_NAME} PROPERTIES CXX_STANDARD_REQUIRED ON)
-set_target_properties(${PROJECT_NAME} PROPERTIES PUBLIC_HEADER "${public_headers}")
 
 target_include_directories(
         ${PROJECT_NAME} PUBLIC $<BUILD_INTERFACE:${PROJECT_SOURCE_DIR}/include>
 )
 
 if (CMAKE_COMPILER_IS_GNUCC)
     target_compile_options(${PROJECT_NAME} PRIVATE -Wall -Wextra -Wpedantic)
@@ -72,10 +61,12 @@
     add_subdirectory(bindings)
 endif ()
 
 if (${${PROJECT_NAME}_BUILD_TESTS})
     add_subdirectory(test)
 endif ()
 
-INSTALL(TARGETS ${PROJECT_NAME}
-        PUBLIC_HEADER DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}/vrpis
-        )
+# Install native library
+INSTALL(TARGETS ${PROJECT_NAME})
+# Install include/ directory and libs
+INSTALL(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/routingblocks DESTINATION routingblocks/include/)
+INSTALL(TARGETS DYNAMIC_BITSET XOSHIRO SMALL_VECTOR)
```

### Comparing `routingblocks-0.1.1/native/cmake/CPM.cmake` & `routingblocks-0.1.2/native/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/cmake/tools.cmake` & `routingblocks-0.1.2/native/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/include/vrpis/ADPTWEvaluation.h` & `routingblocks-0.1.2/native/include/routingblocks/ADPTWEvaluation.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
-#ifndef vrpis_ADPTWEVALUATION_H
-#define vrpis_ADPTWEVALUATION_H
+#ifndef routingblocks_ADPTWEVALUATION_H
+#define routingblocks_ADPTWEVALUATION_H
+
+#include <routingblocks/FRVCP.h>
+#include <routingblocks/evaluation.h>
+#include <routingblocks/types.h>
 
 #include <array>
 #include <dynamic_bitset/dynamic_bitset.hpp>
 #include <optional>
 #include <vector>
 
-#include "FRVCP.h"
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis/interfaces/types.h"
-
-namespace vrpis {
+namespace routingblocks {
     struct ADPTWVertexData {
         float x_coord;
         float y_coord;
         resource_t demand;
         resource_t earliest_arrival_time;
         resource_t latest_arrival_time;
         resource_t service_time;
@@ -71,20 +71,21 @@
         bool operator!=(const ADPTWResourceLabel& other) const { return !(*this == other); }
     };
 
     struct ADPTWForwardResourceLabel : public ADPTWResourceLabel {
         resource_t prev_time_shift;
         resource_t prev_overcharge;
         ADPTWForwardResourceLabel() = default;
-        explicit ADPTWForwardResourceLabel(const vrpis::Vertex& depot, resource_t battery_capacity);
+        explicit ADPTWForwardResourceLabel(const routingblocks::Vertex& depot,
+                                           resource_t battery_capacity);
     };
 
     struct ADPTWBackwardResourceLabel : public ADPTWResourceLabel {
         ADPTWBackwardResourceLabel() = default;
-        explicit ADPTWBackwardResourceLabel(const vrpis::Vertex& depot,
+        explicit ADPTWBackwardResourceLabel(const routingblocks::Vertex& depot,
                                             resource_t battery_capacity);
     };
 
     class ADPTWEvaluation
         : public ConcatenationBasedEvaluationImpl<ADPTWEvaluation, ADPTWForwardResourceLabel,
                                                   ADPTWBackwardResourceLabel, ADPTWVertexData,
                                                   ADPTWArcData> {
@@ -92,16 +93,16 @@
         const resource_t _storage_capacity;
 
         double _overcharge_penalty_factor = 1.;
         double _time_shift_penalty_factor = 1.;
         double _overload_penalty_factor = 1.;
 
       public:
-        using fwd_label_t = vrpis::ADPTWForwardResourceLabel;
-        using bwd_label_t = vrpis::ADPTWBackwardResourceLabel;
+        using fwd_label_t = routingblocks::ADPTWForwardResourceLabel;
+        using bwd_label_t = routingblocks::ADPTWBackwardResourceLabel;
         using vertex_data_t = ADPTWVertexData;
         using arc_data_t = ADPTWArcData;
 
         ADPTWEvaluation(resource_t batteryCapacity, resource_t storageCapacity);
 
         enum CostComponent {
             DIST_INDEX = 0,
@@ -127,15 +128,15 @@
         void set_penalty_factors(const std::array<double, 4>& factors) {
             _overload_penalty_factor = factors[OVERLOAD_INDEX];
             _overcharge_penalty_factor = factors[OVERCHARGE_INDEX];
             _time_shift_penalty_factor = factors[TIME_SHIFT_INDEX];
         };
 
         double concatenate(const fwd_label_t& fwd, const bwd_label_t& bwd,
-                           const vrpis::Vertex& vertex, const vertex_data_t& vertex_data) {
+                           const routingblocks::Vertex& vertex, const vertex_data_t& vertex_data) {
             using std::max;
             using std::min;
 
             resource_t distance = fwd.cum_distance + bwd.cum_distance;
             resource_t overload
                 = max(fwd.cum_load + bwd.cum_load - vertex_data.demand - _storage_capacity,
                       resource_t(0));
@@ -191,21 +192,19 @@
         };
 
         [[nodiscard]] bool is_feasible(const fwd_label_t& label) const {
             return label.cum_overcharge == 0 && label.cum_time_shift == 0
                    && label.cum_load <= _storage_capacity;
         };
 
-        [[nodiscard]] fwd_label_t propagate_forward(const fwd_label_t& pred_label,
-                                                    const vrpis::Vertex& pred_vertex,
-                                                    const vertex_data_t& pred_vertex_data,
-                                                    [[maybe_unused]] const vrpis::Vertex& vertex,
-                                                    const vertex_data_t& vertex_data,
-                                                    [[maybe_unused]] const vrpis::Arc& arc,
-                                                    const arc_data_t& arc_data) const {
+        [[nodiscard]] fwd_label_t propagate_forward(
+            const fwd_label_t& pred_label, const routingblocks::Vertex& pred_vertex,
+            const vertex_data_t& pred_vertex_data,
+            [[maybe_unused]] const routingblocks::Vertex& vertex, const vertex_data_t& vertex_data,
+            [[maybe_unused]] const routingblocks::Arc& arc, const arc_data_t& arc_data) const {
             using std::max;
             using std::min;
             ADPTWForwardResourceLabel propagated_label;
             auto t_ij = arc_data.duration;
             auto q_ij = arc_data.consumption;
             auto c_ij = arc_data.cost;
             resource_t l_j = vertex_data.latest_arrival_time;
@@ -274,18 +273,18 @@
                   + max(propagated_label.earliest_arrival - propagated_label.latest_arrival,
                         resource_t(0));
 
             return propagated_label;
         };
 
         [[nodiscard]] bwd_label_t propagate_backward(
-            const bwd_label_t& succ_label, const vrpis::Vertex& succ_vertex,
+            const bwd_label_t& succ_label, const routingblocks::Vertex& succ_vertex,
             [[maybe_unused]] const vertex_data_t& succ_vertex_data,
-            [[maybe_unused]] const vrpis::Vertex& vertex, const vertex_data_t& vertex_data,
-            [[maybe_unused]] const vrpis::Arc& arc, const arc_data_t& arc_data) const {
+            [[maybe_unused]] const routingblocks::Vertex& vertex, const vertex_data_t& vertex_data,
+            [[maybe_unused]] const routingblocks::Arc& arc, const arc_data_t& arc_data) const {
             using std::max;
             using std::min;
             ADPTWBackwardResourceLabel propagated_label;
 
             const auto t_ij = arc_data.duration + vertex_data.service_time;
             const auto q_ij = arc_data.consumption;
             const auto c_ij = arc_data.cost;
@@ -516,9 +515,9 @@
         }
 
         void prepare(const std::vector<VertexID>&) {}
 
         ADPTWLabel create_root_label() { return ADPTWLabel{_instance->NumberOfVertices()}; }
     };
 
-}  // namespace vrpis
-#endif  // vrpis_ADPTWEVALUATION_H
+}  // namespace routingblocks
+#endif  // routingblocks_ADPTWEVALUATION_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/FRVCP.h` & `routingblocks-0.1.2/native/include/routingblocks/FRVCP.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 
-#ifndef vrpis_FRVCP_H
-#define vrpis_FRVCP_H
+#ifndef routingblocks_FRVCP_H
+#define routingblocks_FRVCP_H
 
-#include <fmt/format.h>
-#include <fmt/ostream.h>
-#include <fmt/ranges.h>
+#include <routingblocks/Instance.h>
+#include <routingblocks/utility/heap.h>
 
 #include <algorithm>
 #include <bitset>
 #include <deque>
 #include <iostream>
-
-#include "Instance.h"
-#include "vrpis/utility/heap.h"
-namespace vrpis {
+namespace routingblocks {
 
     using DPVertexID = size_t;
 
     class DPVertex {
         DPVertexID _vertex_id;
         const Vertex* _original_vertex;
 
@@ -329,21 +325,14 @@
         }
 
         void _initialize_buckets() {
             // Create a bucket for each DPVertex
             _buckets.resize(_graph.size(), LabelBucket(*_propagator));
         }
 
-        void log(std::string_view msg, const DPVertex& extracted_dp_vertex,
-                 const DPVertex* target_dp_vertex) const {
-            if (extracted_dp_vertex.original_vertex().id == 95) {
-                std::cout << msg << std::flush;
-            }
-        }
-
         void _enqueue(VertexID vertex_id) { _node_queue.insert({vertex_id, &_buckets[vertex_id]}); }
         void _update_queue(VertexID vertex_id) {
             _node_queue.update({vertex_id, &_buckets[vertex_id]});
         }
 
         std::vector<VertexID> optimize(const std::vector<VertexID>& route) {
             assert(route.front() == 0);
@@ -363,55 +352,42 @@
                 _buckets[0].add(root_label);
                 _enqueue(0);
             }
 
             while (!_node_queue.empty()) {
                 auto [extracted_label, origin_vertex_id] = _extract_next_label();
                 const auto& origin_dp_vertex = _graph.get_vertex(origin_vertex_id);
-                // log(fmt::format("\nExtracted {} at {}\n", *extracted_label, origin_dp_vertex),
                 // origin_dp_vertex, nullptr);
 
                 if (_propagator->is_final_label(*extracted_label)) {
                     // We have found a feasible solution
-                    // log(fmt::format("Reached root!\n"), origin_dp_vertex, nullptr);
                     return _propagator->extract_path(*extracted_label);
                 }
 
                 // Propagate the label to all adjacent vertices
                 auto [next_target_dp_vertex, target_vertices_end]
                     = _graph.get_successors(origin_vertex_id);
                 for (; next_target_dp_vertex != target_vertices_end; ++next_target_dp_vertex) {
                     const auto& target_dp_vertex = **next_target_dp_vertex;
 
-                    // log(fmt::format("\tAttempting to propgate {} to {}: ", *extracted_label,
-                    //            target_dp_vertex), origin_dp_vertex, &target_dp_vertex);
-
                     if (auto propagated_label = _propagator->propagate(
                             *extracted_label, origin_dp_vertex.original_vertex(),
                             target_dp_vertex.original_vertex(),
                             _instance.getArc(origin_dp_vertex.original_vertex().id,
                                              target_dp_vertex.original_vertex().id));
                         propagated_label) {
                         // Store candidate label
                         Label* next_label = _label_slab.allocate();
                         *next_label = std::move(*propagated_label);
-                        // log(fmt::format("feasible: {}", *next_label), origin_dp_vertex,
-                        // &target_dp_vertex);
                         if (_buckets[target_dp_vertex.dp_vertex_id()].add(next_label)) {
                             _update_queue(target_dp_vertex.dp_vertex_id());
-                        } else {
-                            // log(fmt::format(" but dominated"), origin_dp_vertex,
-                            // &target_dp_vertex);
                         }
-                        // log(fmt::format("\n"), origin_dp_vertex, &target_dp_vertex);
-                    } else {
-                        // log(fmt::format("discarded\n"), origin_dp_vertex, &target_dp_vertex);
                     }
                 }
             }
             return route;
         }
     };
 
-}  // namespace vrpis
+}  // namespace routingblocks
 
-#endif  // vrpis_FRVCP_H
+#endif  // routingblocks_FRVCP_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/Instance.h` & `routingblocks-0.1.2/native/include/routingblocks/Instance.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
-#ifndef vrpis_INSTANCE_H
-#define vrpis_INSTANCE_H
+#ifndef routingblocks_INSTANCE_H
+#define routingblocks_INSTANCE_H
+
+#include <routingblocks/arc.h>
+#include <routingblocks/utility/iterator_pair.h>
+#include <routingblocks/vertex.h>
 
 #include <cassert>
 #include <memory>
 #include <ostream>
 #include <vector>
 
-#include "vrpis/interfaces/arc.h"
-#include "vrpis/interfaces/vertex.h"
-#include "vrpis/utility/iterator_pair.h"
-
-namespace vrpis {
+namespace routingblocks {
     class Instance {
         // contains [depot, customer_1, ..., customer_n, station_1, ..., station_n]
         std::vector<Vertex> _vertices;
         std::vector<std::vector<Arc>> _arcs;
 
         VertexID _number_of_customers;
         VertexID _number_of_stations;
@@ -66,9 +66,9 @@
         }
 
         [[nodiscard]] auto begin() { return _vertices.begin(); }
         [[nodiscard]] auto begin() const { return _vertices.begin(); }
         [[nodiscard]] auto end() { return _vertices.end(); }
         [[nodiscard]] auto end() const { return _vertices.end(); }
     };
-}  // namespace vrpis
-#endif  // vrpis_INSTANCE_H
+}  // namespace routingblocks
+#endif  // routingblocks_INSTANCE_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/LocalSearch.h` & `routingblocks-0.1.2/native/include/routingblocks/LocalSearch.h`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,25 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.*/
 
 #ifndef LOCALSEARCH_H
 #define LOCALSEARCH_H
 
-#include <fmt/format.h>
-#include <fmt/ostream.h>
-#include <fmt/ranges.h>
+#include <routingblocks/Instance.h>
+#include <routingblocks/Solution.h>
+#include <routingblocks/evaluation.h>
+#include <routingblocks/utility/arc_set.h>
+#include <routingblocks/utility/random.h>
 
 #include <memory>
 #include <set>
 #include <vector>
 
-#include "Instance.h"
-#include "Solution.h"
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis/utility/arc_set.h"
-#include "vrpis/utility/random.h"
-
-namespace vrpis {
+namespace routingblocks {
     struct GeneratorArc {
         Solution::const_iterator origin_route;
         Solution::route_t::const_iterator origin_node;
 
         Solution::const_iterator target_route;
         Solution::route_t::const_iterator target_node;
     };
@@ -55,15 +51,15 @@
             = 0;
         virtual void apply(const Instance& instance, Solution& solution) const = 0;
         virtual ~Move() = default;
     };
 
     class Operator {
       public:
-        using eval_t = vrpis::Evaluation;
+        using eval_t = routingblocks::Evaluation;
 
         virtual void prepare_search(const Solution& solution) = 0;
 
         [[nodiscard]] virtual std::shared_ptr<Move> find_next_improving_move(
             eval_t& evaluation, const Solution& solution, const Move* previous_move)
             = 0;
 
@@ -71,15 +67,15 @@
 
         virtual ~Operator() = default;
     };
 
     template <class move_t>
     concept specializes_exact_cost_computation
         = requires(move_t move) {
-              move.evaluate_exact(std::declval<vrpis::Evaluation&>(),
+              move.evaluate_exact(std::declval<routingblocks::Evaluation&>(),
                                   std::declval<const Instance&>(), std::declval<const Solution&>());
           };
 
     template <class operator_t>
     concept specializes_move_construction
         = requires(operator_t op) {
               op.create_move(std::declval<NodeLocation>(), std::declval<NodeLocation>());
@@ -242,19 +238,19 @@
         }
 
         void finalize_search() override {}
     };
 
     // Main local learch structure
     class LocalSearch {
-        using eval_t = vrpis::Evaluation;
-        using solution_t = vrpis::Solution;
+        using eval_t = routingblocks::Evaluation;
+        using solution_t = routingblocks::Solution;
 
       private:
-        const vrpis::Instance* _instance;  // Problem instance
+        const routingblocks::Instance* _instance;  // Problem instance
         std::shared_ptr<eval_t> _evaluation;
         std::shared_ptr<eval_t> _exact_evaluation;
         std::vector<Operator*> _operators;
 
         int loopID = 0;  // Current loop index
         bool use_best_improvement = false;
 
@@ -287,16 +283,16 @@
                 _apply_move(*first_improving_move);
             }
 
             sol = std::move(_current_solution);
         }
 
         // Constructor
-        LocalSearch(const vrpis::Instance& instance, std::shared_ptr<eval_t> evaluation,
+        LocalSearch(const routingblocks::Instance& instance, std::shared_ptr<eval_t> evaluation,
                     std::shared_ptr<eval_t> exact_evaluation);
     };
 
-}  // namespace vrpis
+}  // namespace routingblocks
 
-std::ostream& operator<<(std::ostream& out, const vrpis::Node& node);
+std::ostream& operator<<(std::ostream& out, const routingblocks::Node& node);
 
 #endif
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/NIFTWEvaluation.h` & `routingblocks-0.1.2/native/include/routingblocks/NIFTWEvaluation.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
-#ifndef vrpis_NIFTWEVALUATION_H
-#define vrpis_NIFTWEVALUATION_H
-#include <array>
+#ifndef routingblocks_NIFTWEVALUATION_H
+#define routingblocks_NIFTWEVALUATION_H
+#include <routingblocks/evaluation.h>
+#include <routingblocks/types.h>
 
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis/interfaces/types.h"
+#include <array>
 
-namespace vrpis {
+namespace routingblocks {
 
     struct NIFTWVertexData {
         float x_coord;
         float y_coord;
         resource_t demand;
         resource_t earliest_arrival_time;
         resource_t latest_arrival_time;
@@ -110,43 +110,43 @@
         void set_penalty_factors(const std::array<double, 4>& factors) {
             _overload_penalty_factor = factors[OVERLOAD_INDEX];
             _overcharge_penalty_factor = factors[OVERCHARGE_INDEX];
             _time_shift_penalty_factor = factors[TIME_SHIFT_INDEX];
         };
 
         cost_t concatenate(const fwd_label_t& fwd, const bwd_label_t& bwd,
-                           const vrpis::Vertex& vertex, const vertex_data_t& vertex_data);
+                           const routingblocks::Vertex& vertex, const vertex_data_t& vertex_data);
 
         [[nodiscard]] std::vector<resource_t> get_cost_components(const fwd_label_t& fwd) const {
             return {fwd.cum_distance, std::max(resource_t(0), fwd.cum_load - _storage_capacity),
                     fwd.cum_overcharge, fwd.cum_time_shift};
         };
 
         [[nodiscard]] cost_t compute_cost(const fwd_label_t& label) const;
 
         [[nodiscard]] bool is_feasible(const fwd_label_t& fwd) const {
             return fwd.cum_overcharge == 0 && fwd.cum_time_shift == 0
                    && fwd.cum_load <= _storage_capacity;
         };
 
         [[nodiscard]] fwd_label_t propagate_forward(const fwd_label_t& pred_label,
-                                                    const vrpis::Vertex& pred_vertex,
+                                                    const routingblocks::Vertex& pred_vertex,
                                                     const vertex_data_t& pred_vertex_data,
-                                                    const vrpis::Vertex& vertex,
+                                                    const routingblocks::Vertex& vertex,
                                                     const vertex_data_t& vertex_data,
-                                                    const vrpis::Arc& arc,
+                                                    const routingblocks::Arc& arc,
                                                     const arc_data_t& arc_data) const;
 
         [[nodiscard]] bwd_label_t propagate_backward(const bwd_label_t& succ_label,
-                                                     const vrpis::Vertex& succ_vertex,
+                                                     const routingblocks::Vertex& succ_vertex,
                                                      const vertex_data_t& succ_vertex_data,
-                                                     const vrpis::Vertex& vertex,
+                                                     const routingblocks::Vertex& vertex,
                                                      const vertex_data_t& vertex_data,
-                                                     const vrpis::Arc& arc,
+                                                     const routingblocks::Arc& arc,
                                                      const arc_data_t& arc_data) const;
 
         fwd_label_t create_forward_label(const Vertex& vertex, const vertex_data_t& vertex_data);
         bwd_label_t create_backward_label(const Vertex& vertex, const vertex_data_t& vertex_data);
     };
-}  // namespace vrpis
+}  // namespace routingblocks
 
-#endif  // vrpis_NIFTWEVALUATION_H
+#endif  // routingblocks_NIFTWEVALUATION_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/Solution.h` & `routingblocks-0.1.2/native/include/routingblocks/Solution.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 
-#ifndef vrpis_SOLUTION_H
-#define vrpis_SOLUTION_H
+#ifndef routingblocks_SOLUTION_H
+#define routingblocks_SOLUTION_H
+
+#include <routingblocks/ADPTWEvaluation.h>
+#include <routingblocks/evaluation.h>
+#include <routingblocks/utility/algorithms.h>
 
 #include <any>
 #include <atomic>
 #include <concepts>
+#include <iterator>
 #include <numeric>
 
-#include "ADPTWEvaluation.h"
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis/utility/algorithms.h"
-
 namespace {
     template <class Iterator> constexpr bool has_efficient_size() {
         return std::is_same_v<typename std::iterator_traits<Iterator>::iterator_category,
                               std::random_access_iterator_tag>;
     }
 
     template <class Iterator> constexpr Iterator proper_end_iterator(auto&& container) {
@@ -22,15 +23,15 @@
             return container.end();
         } else {
             return container.rend();
         }
     }
 }  // namespace
 
-namespace vrpis {
+namespace routingblocks {
     class NodeLocation;
 
     inline Node create_node(Evaluation& evaluation, const Vertex& vertex) {
         return {vertex, evaluation.create_forward_label(vertex),
                 evaluation.create_backward_label(vertex)};
     }
 
@@ -51,15 +52,15 @@
     template <class InputIterator>
     concept NodeLocationIterator
         = std::is_same_v<std::decay_t<typename std::iterator_traits<InputIterator>::value_type>,
                          std::decay_t<NodeLocation>>;
 
     class Route {
       public:
-        using eval_t = vrpis::Evaluation;
+        using eval_t = routingblocks::Evaluation;
         using node_t = Node;
 
       private:
         using node_container_t = std::vector<node_t>;
         using instance_t = Instance;
 
       public:
@@ -629,9 +630,9 @@
 
     inline size_t number_of_nodes(const Solution& solution, bool include_start_depot = false) {
         return std::accumulate(solution.begin(), solution.end(), 0,
                                [include_start_depot](size_t acc, const auto& route) {
                                    return acc + number_of_nodes(route, include_start_depot);
                                });
     }
-}  // namespace vrpis
-#endif  // vrpis_SOLUTION_H
+}  // namespace routingblocks
+#endif  // routingblocks_SOLUTION_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/adaptive_large_neighborhood.hpp` & `routingblocks-0.1.2/native/include/routingblocks/adaptive_large_neighborhood.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #pragma once
 
+#include <routingblocks/Solution.h>
+#include <routingblocks/operators.h>
+#include <routingblocks/utility/adaptive_priority_list.h>
+#include <routingblocks/utility/random.h>
+
 #include <type_traits>
 #include <vector>
 
-#include "vrpis/Solution.h"
-#include "vrpis/operators.h"
-#include "vrpis/utility/adaptive_priority_list.h"
-#include "vrpis/utility/random.h"
-
-namespace vrpis {
+namespace routingblocks {
     class adaptive_large_neighborhood {
       private:
         template <typename T> using OperatorList = utility::adaptive_priority_list<T>;
 
         using destroy_operator_list = OperatorList<std::shared_ptr<destroy_operator>>;
         using repair_operator_list = OperatorList<std::shared_ptr<repair_operator>>;
 
-        vrpis::utility::random _random;
+        routingblocks::utility::random _random;
 
         destroy_operator_list _destroy_operators;
         repair_operator_list _repair_operators;
 
         std::pair<decltype(_destroy_operators)::const_iterator,
                   decltype(_repair_operators)::const_iterator>
             _last_pick;
@@ -29,22 +29,22 @@
         using destroy_operator_type = destroy_operator_list::value_type;
         using repair_operator_type = repair_operator_list::value_type;
         using repair_operator_iterator = decltype(_repair_operators)::iterator;
         using destroy_operator_iterator = decltype(_destroy_operators)::iterator;
         using repair_operator_const_iterator = decltype(_repair_operators)::const_iterator;
         using destroy_operator_const_iterator = decltype(_destroy_operators)::const_iterator;
 
-        adaptive_large_neighborhood(vrpis::utility::random random,
+        adaptive_large_neighborhood(routingblocks::utility::random random,
                                     destroy_operator_list destroy_operator_list,
                                     repair_operator_list repair_operator_list)
             : _random(random),
               _destroy_operators(std::move(destroy_operator_list)),
               _repair_operators(std::move(repair_operator_list)) {}
 
-        adaptive_large_neighborhood(vrpis::utility::random random, double smoothingFactor)
+        adaptive_large_neighborhood(routingblocks::utility::random random, double smoothingFactor)
             : _random(random),
               _destroy_operators(_random, smoothingFactor),
               _repair_operators(_random, smoothingFactor) {}
 
         void collect_score(
             std::pair<destroy_operator_list::iterator, repair_operator_list::iterator> pick,
             double score) {
@@ -75,28 +75,29 @@
         }
 
         void remove_operator(destroy_operator_list::const_iterator elem) {
             _destroy_operators.erase(elem);
         }
 
         std::pair<destroy_operator_list::iterator, repair_operator_list::iterator> generate(
-            vrpis::Evaluation& evaluation, vrpis::Solution& sol, size_t num_removed_customers) {
+            routingblocks::Evaluation& evaluation, routingblocks::Solution& sol,
+            size_t num_removed_customers) {
             if (_destroy_operators.empty() || _repair_operators.empty()) {
                 throw std::runtime_error(
                     "Tried to generate a neighbourhood without any operators registered");
             }
 
             // pick operators
             auto destroy_op = _destroy_operators.end();
             do {
                 destroy_op = _destroy_operators.pick();
             } while (!(*destroy_op)->can_apply_to(sol));
 
             // pick a operator to apply
-            assert(vrpis::number_of_nodes(sol) > 0);
+            assert(routingblocks::number_of_nodes(sol) > 0);
 
             auto removed_vertices = (*destroy_op)->apply(evaluation, sol, num_removed_customers);
 
             auto repair_op = _repair_operators.end();
             do {
                 repair_op = _repair_operators.pick();
             } while (!(*repair_op)->can_apply_to(sol));
@@ -112,8 +113,8 @@
         [[nodiscard]] auto destroy_operators_end() { return _destroy_operators.end(); }
 
         [[nodiscard]] auto repair_operators_begin() const { return _repair_operators.begin(); }
         [[nodiscard]] auto repair_operators_end() const { return _repair_operators.end(); }
         [[nodiscard]] auto repair_operators_begin() { return _repair_operators.begin(); }
         [[nodiscard]] auto repair_operators_end() { return _repair_operators.end(); }
     };
-}  // namespace vrpis
+}  // namespace routingblocks
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/interfaces/evaluation.h` & `routingblocks-0.1.2/native/include/routingblocks/evaluation.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 
-#ifndef HGS_EVALUATION_H
-#define HGS_EVALUATION_H
+#ifndef ROUTINGBLOCKS_EVALUATION_H
+#define ROUTINGBLOCKS_EVALUATION_H
+
+#include <routingblocks/Instance.h>
+#include <routingblocks/arc.h>
+#include <routingblocks/node.h>
+#include <routingblocks/types.h>
+#include <routingblocks/vertex.h>
 
 #include <memory>
 #include <span>
 #include <vector>
 
-#include "arc.h"
-#include "node.h"
-#include "types.h"
-#include "vertex.h"
-#include "vrpis/Instance.h"
-
-namespace vrpis {
+namespace routingblocks {
 
     class Evaluation : public std::enable_shared_from_this<Evaluation> {
       public:
         using label_holder_t = Node::label_holder_t;
 
         virtual cost_t evaluate(const Instance& instance, std::span<const route_segment> segments)
             = 0;
 
         [[nodiscard]] virtual cost_t compute_cost(const label_holder_t& label) const = 0;
         [[nodiscard]] virtual bool is_feasible(const label_holder_t& label) const = 0;
         [[nodiscard]] virtual std::vector<resource_t> get_cost_components(
             const label_holder_t& label) const
             = 0;
 
-        [[nodiscard]] virtual label_holder_t propagate_forward(const label_holder_t& pred_label,
-                                                               const vrpis::Vertex& pred_vertex,
-                                                               const vrpis::Vertex& vertex,
-                                                               const vrpis::Arc& arc) const
+        [[nodiscard]] virtual label_holder_t propagate_forward(
+            const label_holder_t& pred_label, const routingblocks::Vertex& pred_vertex,
+            const routingblocks::Vertex& vertex, const routingblocks::Arc& arc) const
             = 0;
 
-        [[nodiscard]] virtual label_holder_t propagate_backward(const label_holder_t& succ_label,
-                                                                const vrpis::Vertex& succ_vertex,
-                                                                const vrpis::Vertex& vertex,
-                                                                const vrpis::Arc& arc) const
+        [[nodiscard]] virtual label_holder_t propagate_backward(
+            const label_holder_t& succ_label, const routingblocks::Vertex& succ_vertex,
+            const routingblocks::Vertex& vertex, const routingblocks::Arc& arc) const
             = 0;
 
         [[nodiscard]] virtual label_holder_t create_forward_label(const Vertex& vertex) = 0;
         [[nodiscard]] virtual label_holder_t create_backward_label(const Vertex& vertex) = 0;
 
         virtual ~Evaluation() = default;
     };
 
     /**
      * Specializes the generic Evaluation class to evaluation functions that provide 2EVAL (cf.,
      * Vidal 2014, https://doi.org/10.1016/j.ejor.2013.09.045)
      */
     class ConcatenationBasedEvaluation : public Evaluation {
         virtual cost_t concatenate(const label_holder_t& fwd, const label_holder_t& bwd,
-                                   const vrpis::Vertex& vertex)
+                                   const routingblocks::Vertex& vertex)
             = 0;
 
         cost_t evaluate(const Instance& instance,
                         const std::span<const route_segment> segments) final {
             auto next_segment = segments.begin();
             // Last segment with a valid forward label
             auto cur_segment = next_segment++;
@@ -115,15 +113,15 @@
         Impl& get_impl() { return static_cast<Impl&>(*this); }
         const Impl& get_impl() const { return static_cast<const Impl&>(*this); }
 
       public:
         using label_holder_t = detail::label_holder;
 
         [[nodiscard]] cost_t concatenate(const label_holder_t& fwd, const label_holder_t& bwd,
-                                         const vrpis::Vertex& vertex) final {
+                                         const routingblocks::Vertex& vertex) final {
             return get_impl().concatenate(fwd.get<fwd_label_t>(), bwd.get<bwd_label_t>(), vertex,
                                           vertex.get_data<vertex_data_t>());
         }
 
         [[nodiscard]] cost_t compute_cost(const label_holder_t& label) const final {
             return get_impl().compute_cost(label.get<fwd_label_t>());
         }
@@ -134,29 +132,29 @@
         }
 
         [[nodiscard]] bool is_feasible(const label_holder_t& label) const final {
             return get_impl().is_feasible(label.get<fwd_label_t>());
         }
 
         [[nodiscard]] label_holder_t propagate_forward(const label_holder_t& pred_label,
-                                                       const vrpis::Vertex& pred_vertex,
-                                                       const vrpis::Vertex& vertex,
-                                                       const vrpis::Arc& arc) const final {
+                                                       const routingblocks::Vertex& pred_vertex,
+                                                       const routingblocks::Vertex& vertex,
+                                                       const routingblocks::Arc& arc) const final {
             const auto& pred_vertex_data = pred_vertex.get_data<vertex_data_t>();
             const auto& vertex_data = vertex.get_data<vertex_data_t>();
             const auto& arc_data = arc.get_data<arc_data_t>();
             return label_holder_t(std::make_shared<fwd_label_t>(get_impl().propagate_forward(
                 pred_label.get<fwd_label_t>(), pred_vertex, pred_vertex_data, vertex, vertex_data,
                 arc, arc_data)));
         }
 
         [[nodiscard]] label_holder_t propagate_backward(const label_holder_t& succ_label,
-                                                        const vrpis::Vertex& succ_vertex,
-                                                        const vrpis::Vertex& vertex,
-                                                        const vrpis::Arc& arc) const final {
+                                                        const routingblocks::Vertex& succ_vertex,
+                                                        const routingblocks::Vertex& vertex,
+                                                        const routingblocks::Arc& arc) const final {
             const auto& succ_vertex_data = succ_vertex.get_data<vertex_data_t>();
             const auto& vertex_data = vertex.get_data<vertex_data_t>();
             const auto& arc_data = arc.get_data<arc_data_t>();
             return label_holder_t(std::make_shared<bwd_label_t>(get_impl().propagate_backward(
                 succ_label.get<bwd_label_t>(), succ_vertex, succ_vertex_data, vertex, vertex_data,
                 arc, arc_data)));
         }
@@ -172,10 +170,10 @@
             return label_holder_t(std::make_shared<bwd_label_t>(
                 get_impl().create_backward_label(vertex, vertex_data)));
         }
     };
 
     template <class eval_t>
     concept is_evaluation = std::derived_from<eval_t, Evaluation>;
-}  // namespace vrpis
+}  // namespace routingblocks
 
-#endif  // HGS_EVALUATION_H
+#endif  // ROUTINGBLOCKS_EVALUATION_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/interfaces/node.h` & `routingblocks-0.1.2/native/include/routingblocks/node.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
-#ifndef _VRPIS_NODE_H
-#define _VRPIS_NODE_H
+#ifndef _routingblocks_NODE_H
+#define _routingblocks_NODE_H
+
+#include <routingblocks/arc.h>
+#include <routingblocks/types.h>
+#include <routingblocks/vertex.h>
 
 #include <concepts>
 #include <memory>
 #include <span>
 #include <vector>
 
-#include "arc.h"
-#include "types.h"
-#include "vertex.h"
-
-namespace vrpis {
+namespace routingblocks {
 
     namespace detail {
         struct label_holder {
             std::shared_ptr<void> _data;
 
             label_holder(std::shared_ptr<void> data) : _data(std::move(data)){};
 
@@ -35,18 +35,18 @@
         using label_holder_t = detail::label_holder;
         using fwd_label_t = label_holder_t;
         using bwd_label_t = label_holder_t;
 
       private:
         fwd_label_t _forward_label;
         bwd_label_t _backward_label;
-        const vrpis::Vertex* _vertex;
+        const routingblocks::Vertex* _vertex;
 
       public:
-        Node(const vrpis::Vertex& vertex, fwd_label_t fwd_label, bwd_label_t bwd_label)
+        Node(const routingblocks::Vertex& vertex, fwd_label_t fwd_label, bwd_label_t bwd_label)
             : _forward_label(std::move(fwd_label)),
               _backward_label(std::move(bwd_label)),
               _vertex(&vertex) {}
 
         void update_forward(Evaluation& evaluation, const Node& pred_node, const Arc& arc);
 
         void update_backward(Evaluation& evaluation, const Node& succ_node, const Arc& arc);
@@ -82,10 +82,10 @@
             : std::span<const Node>(&*begin, &*end) {}
     };
 
     inline route_segment singleton_route_segment(const Node& node) {
         return route_segment{&node, 1};
     }
 
-}  // namespace vrpis
+}  // namespace routingblocks
 
-#endif  //_VRPIS_NODE_H
+#endif  //_routingblocks_NODE_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/operators/InsertStationOperator.h` & `routingblocks-0.1.2/native/include/routingblocks/operators/InsertStationOperator.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
-#ifndef vrpis_INSERTSTATIONOPERATOR_H
-#define vrpis_INSERTSTATIONOPERATOR_H
+#ifndef routingblocks_INSERTSTATIONOPERATOR_H
+#define routingblocks_INSERTSTATIONOPERATOR_H
 
-#include "vrpis/Instance.h"
-#include "vrpis/LocalSearch.h"
-#include "vrpis/Solution.h"
-#include "vrpis/interfaces/evaluation.h"
+#include <routingblocks/Instance.h>
+#include <routingblocks/LocalSearch.h>
+#include <routingblocks/Solution.h>
+#include <routingblocks/evaluation.h>
 
-namespace vrpis {
+namespace routingblocks {
 
     struct SolutionArc {
         Solution::const_iterator route;
         Solution::route_t::const_iterator origin_node;
         Solution::route_t::const_iterator target_node;
 
         SolutionArc(Solution::const_iterator route, Solution::route_t::const_iterator origin_node,
@@ -109,9 +109,9 @@
 
         void prepare_search(const Solution& solution) override;
         std::shared_ptr<Move> find_next_improving_move(eval_t& evaluation, const Solution& solution,
                                                        const Move* previous_move) override;
         void finalize_search() override;
     };
 
-}  // namespace vrpis
-#endif  // vrpis_INSERTSTATIONOPERATOR_H
+}  // namespace routingblocks
+#endif  // routingblocks_INSERTSTATIONOPERATOR_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/operators/RemoveStationOperator.h` & `routingblocks-0.1.2/native/include/routingblocks/operators/RemoveStationOperator.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
-#ifndef vrpis_REMOVESTATIONOPERATOR_H
-#define vrpis_REMOVESTATIONOPERATOR_H
+#ifndef routingblocks_REMOVESTATIONOPERATOR_H
+#define routingblocks_REMOVESTATIONOPERATOR_H
 
-#include "vrpis/Instance.h"
-#include "vrpis/LocalSearch.h"
-#include "vrpis/Solution.h"
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis/operators/InsertStationOperator.h"
+#include <routingblocks/Instance.h>
+#include <routingblocks/LocalSearch.h>
+#include <routingblocks/Solution.h>
+#include <routingblocks/evaluation.h>
+#include <routingblocks/operators/InsertStationOperator.h>
 
-namespace vrpis {
+namespace routingblocks {
     class RemoveStationOperator;
 
     class RemoveStationMove : public Move {
         friend RemoveStationOperator;
         NodeLocation _node;
 
       public:
@@ -73,9 +73,9 @@
             }
 
             return nullptr;
         };
         void finalize_search() override{};
     };
 
-}  // namespace vrpis
-#endif  // vrpis_REMOVESTATIONOPERATOR_H
+}  // namespace routingblocks
+#endif  // routingblocks_REMOVESTATIONOPERATOR_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/operators/SwapOperator.h` & `routingblocks-0.1.2/native/include/routingblocks/operators/SwapOperator.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 
-#ifndef vrpis_SWAPOPERATOR_H
-#define vrpis_SWAPOPERATOR_H
+#ifndef routingblocks_SWAPOPERATOR_H
+#define routingblocks_SWAPOPERATOR_H
 
-#include "vrpis/Instance.h"
-#include "vrpis/LocalSearch.h"
-#include "vrpis/Solution.h"
-#include "vrpis/interfaces/evaluation.h"
+#include <routingblocks/Instance.h>
+#include <routingblocks/LocalSearch.h>
+#include <routingblocks/Solution.h>
+#include <routingblocks/evaluation.h>
 
-namespace vrpis {
+namespace routingblocks {
 
     // "Proper" swaps
     template <size_t origin_segment_length, size_t target_segment_length> class SwapMove
         : public GeneratorArcMove<SwapMove<origin_segment_length, target_segment_length>> {
         /**
          * Generator arc is (origin, target). Our goal is to include this arc into the solution.
          * This operator swaps two sequences, hence the most straightforward way to do this is to
@@ -290,9 +290,9 @@
     template <size_t origin_segment_length, size_t target_segment_length> class SwapOperator
         : public GeneratorArcOperator<SwapMove<origin_segment_length, target_segment_length>> {
       public:
         using GeneratorArcOperator<
             SwapMove<origin_segment_length, target_segment_length>>::GeneratorArcOperator;
     };
 
-}  // namespace vrpis
-#endif  // vrpis_SWAPOPERATOR_H
+}  // namespace routingblocks
+#endif  // routingblocks_SWAPOPERATOR_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/operators.h` & `routingblocks-0.1.2/native/include/routingblocks/operators.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 
-#ifndef vrpis_OPERATORS_H
-#define vrpis_OPERATORS_H
+#ifndef routingblocks_OPERATORS_H
+#define routingblocks_OPERATORS_H
+
+#include <routingblocks/evaluation.h>
+#include <routingblocks/types.h>
+#include <routingblocks/vertex.h>
 
 #include <memory>
 #include <vector>
 
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis/interfaces/types.h"
-#include "vrpis/interfaces/vertex.h"
-
-namespace vrpis {
+namespace routingblocks {
 
     class Solution;
 
     /**
      * \brief Destory Operator interface
      */
     class destroy_operator : public std::enable_shared_from_this<destroy_operator> {
       public:
         /**
          * Applies the operator to the passed solution.
          */
-        virtual std::vector<vrpis::VertexID> apply(vrpis::Evaluation& evaluation,
-                                                   vrpis::Solution& sol,
-                                                   size_t numberOfRemovedCustomers)
+        virtual std::vector<routingblocks::VertexID> apply(routingblocks::Evaluation& evaluation,
+                                                           routingblocks::Solution& sol,
+                                                           size_t numberOfRemovedCustomers)
             = 0;
 
         [[nodiscard]] virtual std::string_view name() const = 0;
 
         /**
          * Returns true if the operator can be applied to the passed solution. False otherwise.
          */
-        [[nodiscard]] virtual bool can_apply_to(const vrpis::Solution& sol) const = 0;
+        [[nodiscard]] virtual bool can_apply_to(const routingblocks::Solution& sol) const = 0;
 
         virtual ~destroy_operator() = default;
     };
 
     /**
      * \brief Destory Operator interface
      */
     class repair_operator : public std::enable_shared_from_this<repair_operator> {
       public:
         /**
          * Applies the operator to the passed solution.
          */
-        virtual void apply(vrpis::Evaluation& evaluation, vrpis::Solution& sol,
-                           const std::vector<vrpis::VertexID>& missing_vertices)
+        virtual void apply(routingblocks::Evaluation& evaluation, routingblocks::Solution& sol,
+                           const std::vector<routingblocks::VertexID>& missing_vertices)
             = 0;
 
         [[nodiscard]] virtual std::string_view name() const = 0;
 
         /**
          * Returns true if the operator can be applied to the passed solution. False otherwise.
          */
-        [[nodiscard]] virtual bool can_apply_to(const vrpis::Solution& sol) const = 0;
+        [[nodiscard]] virtual bool can_apply_to(const routingblocks::Solution& sol) const = 0;
 
         virtual ~repair_operator() = default;
     };
 
-}  // namespace vrpis
+}  // namespace routingblocks
 
-#endif  // vrpis_OPERATORS_H
+#endif  // routingblocks_OPERATORS_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/utility/adaptive_priority_list.h` & `routingblocks-0.1.2/native/include/routingblocks/utility/adaptive_priority_list.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 #include <forward_list>
 #include <iterator>
 #include <memory>
 #include <numeric>
 #include <utility>
 
-#include "vrpis/utility/random.h"
+#include "random.h"
 
-namespace vrpis::utility {
+namespace routingblocks::utility {
     template <class T> class adaptive_priority_list {
       public:
         using value_type = T;
 
       private:
         struct priority_list_entry {
             T value;
@@ -221,8 +221,8 @@
         };
 
         [[nodiscard]] double _avg_weight() const {
             if (_size == 0) return 1.0;
             return _total_weight / _size;
         }
     };
-}  // namespace vrpis::utility
+}  // namespace routingblocks::utility
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/utility/arc_set.h` & `routingblocks-0.1.2/native/include/routingblocks/utility/arc_set.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
-#ifndef _VRPIS_ARC_SET_H
-#define _VRPIS_ARC_SET_H
+#ifndef _routingblocks_ARC_SET_H
+#define _routingblocks_ARC_SET_H
 
 #include <dynamic_bitset/dynamic_bitset.hpp>
 
-namespace vrpis::utility {
+namespace routingblocks::utility {
     class arc_set {
         using bitset_t = sul::dynamic_bitset<>;
         bitset_t _bitset;
         size_t _number_of_vertices;
 
       public:
         explicit arc_set(size_t number_of_vertices)
@@ -25,10 +25,10 @@
             _bitset[from * _number_of_vertices + to] = true;
         }
 
         [[nodiscard]] bool includes_arc(VertexID from, VertexID to) const {
             return _bitset.test(from * _number_of_vertices + to);
         }
     };
-}  // namespace vrpis::utility
+}  // namespace routingblocks::utility
 
-#endif  //_VRPIS_ARC_SET_H
+#endif  //_routingblocks_ARC_SET_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/utility/heap.h` & `routingblocks-0.1.2/native/include/routingblocks/utility/heap.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/include/vrpis/utility/insertion_cache.h` & `routingblocks-0.1.2/native/include/routingblocks/insertion_cache.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
-#ifndef vrpis_INSERTION_CACHE_H
-#define vrpis_INSERTION_CACHE_H
+#ifndef routingblocks_INSERTION_CACHE_H
+#define routingblocks_INSERTION_CACHE_H
+
+#include <routingblocks/Instance.h>
+#include <routingblocks/Solution.h>
+#include <routingblocks/evaluation.h>
+#include <routingblocks/types.h>
 
 #include <dynamic_bitset/dynamic_bitset.hpp>
 #include <vector>
 
-#include "vrpis/Instance.h"
-#include "vrpis/Solution.h"
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis/interfaces/types.h"
-
-namespace vrpis::utility {
+namespace routingblocks::utility {
     struct insertion_move {
-        vrpis::VertexID vertex_id{};
-        vrpis::NodeLocation after_node{0, 0};
+        routingblocks::VertexID vertex_id{};
+        routingblocks::NodeLocation after_node{0, 0};
         cost_t delta_cost{};
 
         auto operator<=>(const insertion_move& other) const {
             return delta_cost <=> other.delta_cost;
         }
 
         bool operator==(const insertion_move& other) const {
@@ -245,32 +245,32 @@
 
       private:
         void _restore_order(VertexID vertex) {
             std::sort(_caches[vertex].begin(), _caches[vertex].end(), _comp);
         }
 
         auto _overwrite_sequence_with_moves_from_route(std::vector<move_t>::iterator seq_begin,
-                                                       const vrpis::Route& route,
+                                                       const routingblocks::Route& route,
                                                        size_t route_index, VertexID vertex_id) {
             auto succ = route.begin();
             auto pred = succ++;
             size_t pos = 0;
             auto route_cost = route.cost();
             Node n = create_node(*_evaluation, *_instance, vertex_id);
             for (; succ != route.end(); ++succ, ++pred, ++pos, ++seq_begin) {
                 cost_t insertion_cost
                     = evaluate_insertion(*_evaluation, *_instance, route, pred, n);
-                *seq_begin = move_t{vertex_id, vrpis::NodeLocation(route_index, pos),
+                *seq_begin = move_t{vertex_id, routingblocks::NodeLocation(route_index, pos),
                                     insertion_cost - route_cost};
             }
             return seq_begin;
         }
 
-        void _update_moves_of_route(const vrpis::Route& route, size_t route_index, auto& cache,
-                                    VertexID vertex_id) {
+        void _update_moves_of_route(const routingblocks::Route& route, size_t route_index,
+                                    auto& cache, VertexID vertex_id) {
             // Partitions the vector into [route_i, route_j, ..., route_index...]
             auto first_invalid_move = std::partition(
                 cache.begin(), cache.end(),
                 [route_index](const move_t& move) { return move.after_node.route != route_index; });
             const size_t first_invalid_move_index
                 = std::distance(cache.begin(), first_invalid_move);
             // Resize the cache to have space for all elements
@@ -283,10 +283,10 @@
             first_invalid_move = std::next(cache.begin(), first_invalid_move_index);
             // Now just replace
             auto cache_end = _overwrite_sequence_with_moves_from_route(first_invalid_move, route,
                                                                        route_index, vertex_id);
             assert(cache_end == cache.end());
         }
     };
-}  // namespace vrpis::utility
+}  // namespace routingblocks::utility
 
-#endif  // vrpis_INSERTION_CACHE_H
+#endif  // routingblocks_INSERTION_CACHE_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/utility/iterator_pair.h` & `routingblocks-0.1.2/native/include/routingblocks/utility/iterator_pair.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
-#ifndef _VRPIS_ITERATOR_PAIR_H
-#define _VRPIS_ITERATOR_PAIR_H
+#ifndef _routingblocks_ITERATOR_PAIR_H
+#define _routingblocks_ITERATOR_PAIR_H
 
-namespace vrpis::utility {
+namespace routingblocks::utility {
     /***
      * Provides a simple iterator helper class that allows to use range-based for loops with
      * std::pair<iterator, iterator> objects.
      */
     template <typename Iterator> class iterator_pair {
         Iterator _begin;
         Iterator _end;
@@ -17,10 +17,10 @@
         Iterator end() const { return _end; }
     };
 
     template <typename Iterator>
     iterator_pair<Iterator> make_iterator_pair(Iterator begin, Iterator end) {
         return iterator_pair<Iterator>(begin, end);
     }
-}  // namespace vrpis::utility
+}  // namespace routingblocks::utility
 
-#endif  //_VRPIS_ITERATOR_PAIR_H
+#endif  //_routingblocks_ITERATOR_PAIR_H
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/utility/random.h` & `routingblocks-0.1.2/native/include/routingblocks/utility/random.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #pragma once
 
+#include <xoshiro/xoshiro.h>
+
 #include <algorithm>
 #include <concepts>
 #include <ctime>
 #include <limits>
 #include <random>
 
-#include "xoshiro/xoshiro.h"
-
-namespace vrpis::utility {
+namespace routingblocks::utility {
     class random {
       public:
         using result_type = size_t;
 
         constexpr static result_type min() { return std::numeric_limits<result_type>::min(); }
 
         constexpr static result_type max() { return std::numeric_limits<result_type>::max(); }
@@ -95,8 +95,8 @@
             if (aggregated_weights == 0.0) {  // All options are equally good
                 return (beg + generateInt(0, std::distance(beg, end) - 1));
             }
 
             throw std::logic_error("Reached end of roulette pick");
         }
     };
-}  // namespace vrpis::utility
+}  // namespace routingblocks::utility
```

### Comparing `routingblocks-0.1.1/native/include/vrpis/utility/removal_cache.h` & `routingblocks-0.1.2/native/include/routingblocks/removal_cache.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
-#ifndef vrpis_REMOVAL_CACHE_H
-#define vrpis_REMOVAL_CACHE_H
+#ifndef routingblocks_REMOVAL_CACHE_H
+#define routingblocks_REMOVAL_CACHE_H
 
-#include <concepts>
+#include <routingblocks/Instance.h>
+#include <routingblocks/Solution.h>
+#include <routingblocks/evaluation.h>
+#include <routingblocks/types.h>
 
-#include "vrpis/Instance.h"
-#include "vrpis/Solution.h"
-#include "vrpis/interfaces/evaluation.h"
-#include "vrpis/interfaces/types.h"
+#include <concepts>
 
-namespace vrpis::utility {
+namespace routingblocks::utility {
 
     struct removal_move {
-        vrpis::VertexID vertex_id{};
-        vrpis::NodeLocation node_location{0, 0};
+        routingblocks::VertexID vertex_id{};
+        routingblocks::NodeLocation node_location{0, 0};
         cost_t delta_cost{};
 
         auto operator<=>(const removal_move& other) const {
             return delta_cost <=> other.delta_cost;
         }
 
         bool operator==(const removal_move& other) const {
@@ -28,41 +28,41 @@
     template <class Comp = std::less<removal_move>> class removal_cache {
       public:
         using move_t = removal_move;
         using iterator = std::vector<move_t>::iterator;
         using const_iterator = std::vector<move_t>::const_iterator;
 
       private:
-        const vrpis::Instance* _instance;
-        vrpis::Evaluation* _evaluation;
+        const routingblocks::Instance* _instance;
+        routingblocks::Evaluation* _evaluation;
 
         // Cache structure. Holds all removal moves.
         std::vector<move_t> _cache;
         // Comparator
         Comp _comp;
 
         auto _overwrite_sequence_with_moves_from_route(iterator seq_begin,
-                                                       const vrpis::Route& route,
+                                                       const routingblocks::Route& route,
                                                        size_t route_index) {
             auto succ = route.begin();
             auto pred = succ++;
             auto cur = succ++;
             size_t pos = 1;
             auto route_cost = route.cost();
             for (; succ != route.end(); ++succ, ++pred, ++cur, ++pos, ++seq_begin) {
                 cost_t removal_cost
                     = concatenate(*_evaluation, *_instance, route_segment{route.begin(), cur},
                                   route_segment{succ, route.end()});
-                *seq_begin = move_t{cur->vertex_id(), vrpis::NodeLocation(route_index, pos),
+                *seq_begin = move_t{cur->vertex_id(), routingblocks::NodeLocation(route_index, pos),
                                     removal_cost - route_cost};
             }
             return seq_begin;
         }
 
-        void _update_moves_of_route(const vrpis::Route& route, size_t route_index) {
+        void _update_moves_of_route(const routingblocks::Route& route, size_t route_index) {
             // Partitions the vector into [route_i, route_j, ..., route_index...]
             auto first_invalid_move
                 = std::partition(_cache.begin(), _cache.end(), [route_index](const move_t& move) {
                       return move.node_location.route != route_index;
                   });
             const size_t first_invalid_move_index
                 = std::distance(_cache.begin(), first_invalid_move);
@@ -79,44 +79,45 @@
                 = _overwrite_sequence_with_moves_from_route(first_invalid_move, route, route_index);
             assert(cache_end == _cache.end());
         }
 
         void _restore_order() { std::sort(_cache.begin(), _cache.end(), _comp); }
 
       public:
-        explicit removal_cache(const vrpis::Instance& instance)
+        explicit removal_cache(const routingblocks::Instance& instance)
             : _instance(&instance), _evaluation{}, _cache{} {};
-        removal_cache(const vrpis::Instance& instance, Comp comp)
+        removal_cache(const routingblocks::Instance& instance, Comp comp)
             : _instance(&instance), _evaluation{}, _cache{}, _comp(std::move(comp)){};
 
         void clear() {
             _evaluation = nullptr;
             _cache.clear();
         };
 
-        void rebuild(vrpis::Evaluation& evaluation, const vrpis::Solution& solution) {
+        void rebuild(routingblocks::Evaluation& evaluation,
+                     const routingblocks::Solution& solution) {
             clear();
             _evaluation = &evaluation;
-            _cache.resize(vrpis::number_of_nodes(solution));
+            _cache.resize(routingblocks::number_of_nodes(solution));
             size_t route_index = 0;
             auto next_move_storage = _cache.begin();
             for (auto route_iter = solution.begin(); route_iter != solution.end();
                  ++route_index, ++route_iter) {
                 next_move_storage = _overwrite_sequence_with_moves_from_route(
                     next_move_storage, *route_iter, route_index);
             }
             assert(next_move_storage == _cache.end());
             _restore_order();
         }
 
-        void invalidate_route(const vrpis::Route& route, size_t route_index) {
+        void invalidate_route(const routingblocks::Route& route, size_t route_index) {
             _update_moves_of_route(route, route_index);
             _restore_order();
         }
 
         auto begin() const { return _cache.begin(); }
         auto end() const { return _cache.end(); }
     };
 
-}  // namespace vrpis::utility
+}  // namespace routingblocks::utility
 
-#endif  // vrpis_REMOVAL_CACHE_H
+#endif  // routingblocks_REMOVAL_CACHE_H
```

### Comparing `routingblocks-0.1.1/native/lib/dynamic_bitset/LICENSE.txt` & `routingblocks-0.1.2/native/lib/dynamic_bitset/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp` & `routingblocks-0.1.2/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h` & `routingblocks-0.1.2/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/lib/small_vector/LICENSE.txt` & `routingblocks-0.1.2/native/lib/small_vector/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/lib/small_vector/small_vector/small_vector.hpp` & `routingblocks-0.1.2/native/lib/small_vector/small_vector/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/lib/xoshiro/LICENSE.txt` & `routingblocks-0.1.2/native/lib/xoshiro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/lib/xoshiro/xoshiro/xoshiro.h` & `routingblocks-0.1.2/native/lib/xoshiro/xoshiro/xoshiro.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/native/src/ADPTWEvaluation.cpp` & `routingblocks-0.1.2/native/src/ADPTWEvaluation.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-#include "vrpis/ADPTWEvaluation.h"
+#include <routingblocks/ADPTWEvaluation.h>
 
 #include <iostream>
 
-#include "fmt/core.h"
-
-namespace vrpis {
+namespace routingblocks {
 
     ADPTWForwardResourceLabel::ADPTWForwardResourceLabel(
-        const vrpis::Vertex &depot, [[maybe_unused]] resource_t battery_capacity)
+        const routingblocks::Vertex &depot, [[maybe_unused]] resource_t battery_capacity)
         : ADPTWResourceLabel{.earliest_arrival
                              = depot.get_data<ADPTWVertexData>().earliest_arrival_time,
                              .latest_arrival
                              = depot.get_data<ADPTWVertexData>().earliest_arrival_time,
                              .shifted_earliest_arrival
                              = depot.get_data<ADPTWVertexData>().earliest_arrival_time,
                              .shifted_latest_arrival
@@ -22,15 +20,15 @@
                              .cum_load = 0,
                              .cum_time_shift = 0,
                              .cum_overcharge = 0},
           prev_time_shift(0),
           prev_overcharge(0) {}
 
     ADPTWBackwardResourceLabel::ADPTWBackwardResourceLabel(
-        const vrpis::Vertex &depot, [[maybe_unused]] resource_t battery_capacity)
+        const routingblocks::Vertex &depot, [[maybe_unused]] resource_t battery_capacity)
         : ADPTWResourceLabel{
             .earliest_arrival = depot.get_data<ADPTWVertexData>().latest_arrival_time,
             .latest_arrival = depot.get_data<ADPTWVertexData>().latest_arrival_time,
             .shifted_earliest_arrival = depot.get_data<ADPTWVertexData>().latest_arrival_time,
             .shifted_latest_arrival = depot.get_data<ADPTWVertexData>().latest_arrival_time,
             .residual_charge_in_time = 0,
             .f = 0,
@@ -57,8 +55,8 @@
     cost_t ADPTWEvaluation::_compute_cost(resource_t distance, resource_t overload,
                                           resource_t overcharge, resource_t time_shift) const {
         return static_cast<cost_t>(static_cast<double>(distance)
                                    + static_cast<double>(overload) * _overload_penalty_factor
                                    + static_cast<double>(time_shift) * _time_shift_penalty_factor
                                    + static_cast<double>(overcharge) * _overcharge_penalty_factor);
     }
-}  // namespace vrpis
+}  // namespace routingblocks
```

### Comparing `routingblocks-0.1.1/native/src/Instance.cpp` & `routingblocks-0.1.2/native/src/Instance.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-#include "vrpis/Instance.h"
-
-#include <fmt/format.h>
-#include <fmt/ostream.h>
+#include <routingblocks/Instance.h>
 
 #include <algorithm>
 #include <iostream>
 
-using namespace vrpis;
+using namespace routingblocks;
 
 Instance::Instance(std::vector<Vertex> vertices, std::vector<std::vector<Arc>> arcs, int fleetSize)
     : _vertices(std::move(vertices)), _arcs(std::move(arcs)), _fleet_size(fleetSize) {
     // vertices should be ordered as [depot, cust_1, ..., cust_n, station_1, ..., station_n]
     auto next_vertex = _vertices.begin();
     size_t next_vertex_id = 0;
 
     if (!next_vertex->is_depot || next_vertex->id != next_vertex_id) {
         throw std::runtime_error("Depot is not first vertex");
     }
 
-    for (next_vertex = std::next(next_vertex), next_vertex_id = 1; !next_vertex->is_station;
+    for (next_vertex = std::next(next_vertex), next_vertex_id = 1;
+         !next_vertex->is_station && next_vertex != _vertices.end();
          ++next_vertex, ++next_vertex_id) {
         if (next_vertex->is_depot || next_vertex->is_station || next_vertex->id != next_vertex_id) {
-            throw std::runtime_error(fmt::format(
-                "expected vertex {} to have id {} and to be a customer (not a station or depot)",
-                *next_vertex, next_vertex_id));
+            throw std::runtime_error(
+                "Wrong vertex ordering! Expected order: depot, customers, stations with sequential "
+                "id's. Problem: a depot or station vertex is at a position where a customer was "
+                "expected.");
         }
     }
 
     _number_of_customers = next_vertex_id - 1;  // Account for depot
     _number_of_stations = _vertices.size() - 1 - _number_of_customers;
     auto station_offset = next_vertex_id;
 
     for (; next_vertex != _vertices.end(); ++next_vertex, ++next_vertex_id) {
         if (next_vertex->is_depot || !next_vertex->is_station
             || next_vertex_id != next_vertex->id) {
             throw std::runtime_error(
-                fmt::format("expected vertex {} to have id {} and to be a station", *next_vertex,
-                            next_vertex_id));
+                "Wrong vertex ordering! Expected order: depot, customers, stations with sequential "
+                "id's. Problem: A non-station vertex follows customer vertices");
         }
     }
 
     if (_fleet_size <= 0) {
         throw std::runtime_error(
             "fleet size, vehicle capacity, and vehicle battery capacity must be greater than 0");
     }
```

### Comparing `routingblocks-0.1.1/native/src/NIFTWEvaluation.cpp` & `routingblocks-0.1.2/native/src/NIFTWEvaluation.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-#include "vrpis/NIFTWEvaluation.h"
+#include <routingblocks/NIFTWEvaluation.h>
 
 #include <iostream>
 
-#include "fmt/core.h"
-
-namespace vrpis {
+namespace routingblocks {
 
     auto NIFTWEvaluation::propagate_backward(const bwd_label_t &succ_label,
-                                             const vrpis::Vertex &succ_vertex,
+                                             const routingblocks::Vertex &succ_vertex,
                                              [[maybe_unused]] const vertex_data_t &succ_vertex_data,
-                                             [[maybe_unused]] const vrpis::Vertex &vertex,
+                                             [[maybe_unused]] const routingblocks::Vertex &vertex,
                                              const vertex_data_t &vertex_data,
-                                             [[maybe_unused]] const vrpis::Arc &arc,
+                                             [[maybe_unused]] const routingblocks::Arc &arc,
                                              const arc_data_t &arc_data) const -> bwd_label_t {
         using std::max;
         using std::min;
 
-        vrpis::NIFTWBackwardLabel propagated_label;
+        routingblocks::NIFTWBackwardLabel propagated_label;
 
         const auto t_ij = arc_data.duration + vertex_data.service_time;
         const auto q_ij = arc_data.consumption;
         const auto c_ij = arc_data.cost;
 
         propagated_label.cum_distance = succ_label.cum_distance + c_ij;
         propagated_label.cum_load = succ_label.cum_load + vertex_data.demand;
@@ -47,24 +45,24 @@
             = succ_label.cum_overcharge
               + max(resource_t(0), propagated_label.residual_charge_in_time - _battery_capacity);
 
         return propagated_label;
     }
 
     auto NIFTWEvaluation::propagate_forward(const fwd_label_t &pred_label,
-                                            const vrpis::Vertex &pred_vertex,
+                                            const routingblocks::Vertex &pred_vertex,
                                             const vertex_data_t &pred_vertex_data,
-                                            [[maybe_unused]] const vrpis::Vertex &vertex,
+                                            [[maybe_unused]] const routingblocks::Vertex &vertex,
                                             const vertex_data_t &vertex_data,
-                                            [[maybe_unused]] const vrpis::Arc &arc,
+                                            [[maybe_unused]] const routingblocks::Arc &arc,
                                             const arc_data_t &arc_data) const -> fwd_label_t {
         using std::max;
         using std::min;
 
-        vrpis::NIFTWForwardLabel propagated_label;
+        routingblocks::NIFTWForwardLabel propagated_label;
         auto t_ij = arc_data.duration + pred_vertex_data.service_time;
         auto q_ij = arc_data.consumption;
         auto c_ij = arc_data.cost;
 
         propagated_label.cum_distance = pred_label.cum_distance + c_ij;
         propagated_label.cum_load = pred_label.cum_load + vertex_data.demand;
 
@@ -94,15 +92,15 @@
         propagated_label.prev_time_shift = pred_label.cum_time_shift;
         propagated_label.prev_overcharge = pred_label.cum_overcharge;
 
         return propagated_label;
     }
 
     cost_t NIFTWEvaluation::concatenate(const fwd_label_t &fwd, const bwd_label_t &bwd,
-                                        const vrpis::Vertex &vertex,
+                                        const routingblocks::Vertex &vertex,
                                         const vertex_data_t &vertex_data) {
         using std::max;
         using std::min;
 
         resource_t distance = fwd.cum_distance + bwd.cum_distance;
         resource_t overload = max(
             fwd.cum_load + bwd.cum_load - vertex_data.demand - _storage_capacity, resource_t(0));
@@ -166,8 +164,8 @@
     cost_t NIFTWEvaluation::_compute_cost(resource_t distance, resource_t overload,
                                           resource_t overcharge, resource_t time_shift) const {
         return static_cast<cost_t>(static_cast<double>(distance)
                                    + static_cast<double>(overload) * _overload_penalty_factor
                                    + static_cast<double>(time_shift) * _time_shift_penalty_factor
                                    + static_cast<double>(overcharge) * _overcharge_penalty_factor);
     }
-}  // namespace vrpis
+}  // namespace routingblocks
```

### Comparing `routingblocks-0.1.1/native/src/Solution.cpp` & `routingblocks-0.1.2/native/src/Solution.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-#include "vrpis/Solution.h"
+#include <routingblocks/Solution.h>
 
 #include <numeric>
 
-namespace vrpis {
+namespace routingblocks {
 
     bool NodeLocation::operator==(const NodeLocation& rhs) const {
         return route == rhs.route && position == rhs.position;
     }
 
     bool NodeLocation::operator!=(const NodeLocation& rhs) const { return !(rhs == *this); }
 
@@ -69,8 +69,8 @@
         _update_vertex_lookup();
         return new_pos;
     }
     auto Solution::remove_vertex(Solution::iterator route, typename route_t::iterator position) ->
         typename route_t::iterator {
         return this->remove_route_segment(route, position, std::next(position));
     }
-}  // namespace vrpis
+}  // namespace routingblocks
```

### Comparing `routingblocks-0.1.1/native/src/node.cpp` & `routingblocks-0.1.2/native/src/node.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-#include "vrpis/interfaces/node.h"
+#include <routingblocks/evaluation.h>
+#include <routingblocks/node.h>
 
-#include "vrpis/interfaces/evaluation.h"
-
-namespace vrpis {
+namespace routingblocks {
 
     void Node::update_forward(Evaluation& evaluation, const Node& pred_node, const Arc& arc) {
         _forward_label = evaluation.propagate_forward(pred_node._forward_label, *pred_node._vertex,
                                                       *_vertex, arc);
     }
     void Node::update_backward(Evaluation& evaluation, const Node& succ_node, const Arc& arc) {
         _backward_label = evaluation.propagate_backward(succ_node._backward_label,
@@ -17,8 +16,8 @@
     }
     std::vector<resource_t> Node::cost_components(Evaluation& evaluation) const {
         return evaluation.get_cost_components(_forward_label);
     }
     bool Node::feasible(Evaluation& evaluation) const {
         return evaluation.is_feasible(_forward_label);
     }
-}  // namespace vrpis
+}  // namespace routingblocks
```

### Comparing `routingblocks-0.1.1/native/src/operators/InsertStationOperator.cpp` & `routingblocks-0.1.2/native/src/operators/InsertStationOperator.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#include "vrpis/operators/InsertStationOperator.h"
+#include <routingblocks/operators/InsertStationOperator.h>
 
-namespace vrpis {
+namespace routingblocks {
 
     cost_t InsertStationMove::get_cost_delta(Evaluation& evaluation, const Instance& instance,
                                              const Solution& solution) const {
         auto [route, node] = to_iter(_after_node, solution);
         const auto& station = instance.getVertex(_station_id);
 
         cost_t cost = evaluate_insertion(evaluation, instance, *route, node, station);
@@ -69,8 +69,8 @@
             return {SolutionArcIterator(solution, {solution.begin(), solution.begin()->begin()}),
                     0};
         }
     }
 
     InsertStationOperator::InsertStationOperator(const Instance& instance) : _instance(instance) {}
 
-}  // namespace vrpis
+}  // namespace routingblocks
```

### Comparing `routingblocks-0.1.1/native/src/operators/InterRouteTwoOptOperator.cpp` & `routingblocks-0.1.2/native/src/operators/InterRouteTwoOptOperator.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#include "vrpis/operators/InterRouteTwoOptOperator.h"
+#include <routingblocks/operators/InterRouteTwoOptOperator.h>
 
-namespace vrpis {
+namespace routingblocks {
 
     cost_t InterRouteTwoOptMove::evaluate(Evaluation& evaluation, const Instance& instance,
                                           const Solution& solution) const {
         const auto& origin_location = origin();
         const auto& target_location = target();
         auto [origin_route, origin_node] = to_iter(origin_location, solution);
         auto [target_route, target_node] = to_iter(target_location, solution);
@@ -32,8 +32,8 @@
         auto [origin_route, origin_node] = to_iter(origin_location, solution);
         auto [target_route, target_node] = to_iter(target_location, solution);
 
         solution.exchange_segment(origin_route, std::next(origin_node), origin_route->end_depot(),
                                   target_route, std::next(target_node), target_route->end_depot());
     }
 
-}  // namespace vrpis
+}  // namespace routingblocks
```

### Comparing `routingblocks-0.1.1/native/test/CMakeLists.txt` & `routingblocks-0.1.2/native/test/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 message("Adding tests under ${CMAKE_PROJECT_NAME}Tests...")
 
 #
 # Set the sources for the unit tests and add the executable(s)
 #
 
-file(GLOB_RECURSE test_headers CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/include/vrpis-tests/*.h")
+file(GLOB_RECURSE test_headers CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/include/routingblocks-tests/*.h")
 file(GLOB_RECURSE test_sources CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp")
 
 add_executable(${PROJECT_NAME} ${test_headers} ${test_sources})
 
 #
 # Set seed for reproducibility
 #
-target_compile_definitions(${PROJECT_NAME} PUBLIC -DVRPIS_RAND_SEED=2021)
+target_compile_definitions(${PROJECT_NAME} PUBLIC -DROUTINGBLOCKS_RAND_SEED=2021)
 
 #
 # Set the compiler standard
 #
 
 target_compile_features(${PROJECT_NAME} PUBLIC cxx_std_20)
```

### Comparing `routingblocks-0.1.1/pyproject.toml` & `routingblocks-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core>=0.2.1", "pybind11", "mypy"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "RoutingBlocks"
-version = "0.1.1"
+version = "0.1.2"
 description = "A package for the implementation of vehicle routing problems with intermediate stops"
 readme = "README.md"
 authors = [
     { name = "Patrick Sean Klein", email = "patrick.sean.klein@tum.de" },
 ]
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `routingblocks-0.1.1/routingblocks/operators/__init__.py` & `routingblocks-0.1.2/routingblocks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/routingblocks/operators/best_insert.py` & `routingblocks-0.1.2/routingblocks/operators/best_insert.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/routingblocks/operators/cluster_removal.py` & `routingblocks-0.1.2/routingblocks/operators/cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/routingblocks/operators/move_selectors.py` & `routingblocks-0.1.2/routingblocks/operators/move_selectors.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/routingblocks/operators/related_removal.py` & `routingblocks-0.1.2/routingblocks/operators/related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/routingblocks/operators/route_removal.py` & `routingblocks-0.1.2/routingblocks/operators/route_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/routingblocks/operators/station_vicinity_removal.py` & `routingblocks-0.1.2/routingblocks/operators/station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/routingblocks/operators/worst_removal.py` & `routingblocks-0.1.2/routingblocks/operators/worst_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/benchmarks/reference/insertion_cache.py` & `routingblocks-0.1.2/test/tests/benchmarks/reference/insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/benchmarks/reference/removal_cache.py` & `routingblocks-0.1.2/test/tests/benchmarks/reference/removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/benchmarks/test_benchmark_frvcp.py` & `routingblocks-0.1.2/test/tests/benchmarks/test_benchmark_frvcp.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/benchmarks/test_benchmark_local_search.py` & `routingblocks-0.1.2/test/tests/benchmarks/test_benchmark_local_search.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/benchmarks/test_benchmark_removal_cache.py` & `routingblocks-0.1.2/test/tests/benchmarks/test_benchmark_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/benchmarks/test_benchmark_route_update.py` & `routingblocks-0.1.2/test/tests/benchmarks/test_benchmark_route_update.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/fixtures/__init__.py` & `routingblocks-0.1.2/test/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/fixtures/data/c101C5.txt` & `routingblocks-0.1.2/test/tests/fixtures/data/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/fixtures/data/c101_21.txt` & `routingblocks-0.1.2/test/tests/fixtures/data/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/fixtures/data/r101_21.txt` & `routingblocks-0.1.2/test/tests/fixtures/data/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/fixtures/data/r201_21.txt` & `routingblocks-0.1.2/test/tests/fixtures/data/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/fixtures/data/rc101_21.txt` & `routingblocks-0.1.2/test/tests/fixtures/data/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/fixtures/mock_evaluation.py` & `routingblocks-0.1.2/test/tests/fixtures/mock_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/helpers/interface.py` & `routingblocks-0.1.2/test/tests/helpers/interface.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/helpers/models.py` & `routingblocks-0.1.2/test/tests/helpers/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/helpers/parsing.py` & `routingblocks-0.1.2/test/tests/helpers/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/operators/test_cluster_removal.py` & `routingblocks-0.1.2/test/tests/operators/test_cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/operators/test_random_insertion.py` & `routingblocks-0.1.2/test/tests/operators/test_random_insertion.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/operators/test_random_removal.py` & `routingblocks-0.1.2/test/tests/operators/test_random_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/operators/test_related_removal.py` & `routingblocks-0.1.2/test/tests/operators/test_related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/operators/test_station_insertion.py` & `routingblocks-0.1.2/test/tests/operators/test_station_insertion.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/operators/test_station_vicinity_removal.py` & `routingblocks-0.1.2/test/tests/operators/test_station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/operators/test_swap.py` & `routingblocks-0.1.2/test/tests/operators/test_swap.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_evaluation.py` & `routingblocks-0.1.2/test/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_frvcp.py` & `routingblocks-0.1.2/test/tests/test_frvcp.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_insertion_cache.py` & `routingblocks-0.1.2/test/tests/test_insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_large_neighborhood.py` & `routingblocks-0.1.2/test/tests/test_large_neighborhood.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_lns_helpers.py` & `routingblocks-0.1.2/test/tests/test_lns_helpers.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_local_search.py` & `routingblocks-0.1.2/test/tests/test_local_search.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_node.py` & `routingblocks-0.1.2/test/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_removal_cache.py` & `routingblocks-0.1.2/test/tests/test_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_route.py` & `routingblocks-0.1.2/test/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/test/tests/test_solution.py` & `routingblocks-0.1.2/test/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.1/PKG-INFO` & `routingblocks-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingblocks
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for the implementation of vehicle routing problems with intermediate stops
 Author-Email: Patrick Sean Klein <patrick.sean.klein@tum.de>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -51,14 +51,15 @@
 ## Features
 
 * Efficient C++-based solution representation
 * Customizable Local Search Solver
 * Framework for ALNS-based metaheuristics
 * Efficient native implementations of numerous destroy, repair, and local search operators
 * Move caches implemented in native code to allow high-performance operator implementations in Python
+* Support for custom [native extensions](https://github.com/tumBAIS/routingblocks-native-extension-example)
 
 ## Usage
 
 We provide an [example implementation](https://github.com/tumBAIS/RoutingBlocks/tree/main/examples) of an ALNS-based
 algorithm for
 the [EVRPTW-PR](https://research.sabanciuniv.edu/id/eprint/26033/1/WP_EVRPTW-Partial_Recharge_KeskinCatay.pdf) as part
 of this repository.
```

