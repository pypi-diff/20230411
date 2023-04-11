# Comparing `tmp/VRPSolverEasy-0.1.2.tar.gz` & `tmp/VRPSolverEasy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VRPSolverEasy-0.1.2.tar", last modified: Thu Apr  6 08:34:04 2023, max compression
+gzip compressed data, was "VRPSolverEasy-0.1.3.tar", last modified: Tue Apr 11 12:44:58 2023, max compression
```

## Comparing `VRPSolverEasy-0.1.2.tar` & `VRPSolverEasy-0.1.3.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.999574 VRPSolverEasy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-04-06 08:34:03.999574 VRPSolverEasy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.927573 VRPSolverEasy-0.1.2/VRPSolverEasy/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.931573 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/CVRP.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/CVRPTW.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/HFVRP.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/MDVRP.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.927573 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.943573 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n32-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n33-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n33-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n34-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n36-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n37-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n37-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n38-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n39-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n39-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n44-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n45-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n45-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n46-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n48-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n53-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n54-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n55-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n60-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n61-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n62-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n63-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n63-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n64-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n65-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n69-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n80-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n31-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n34-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n35-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n38-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n39-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n41-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n43-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n44-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n45-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n45-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n50-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n50-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n51-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n52-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n56-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n57-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n57-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n63-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n64-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n66-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n67-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n68-k9.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n78-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n101-k14.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n101-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n22-k4.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n23-k3.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n30-k3.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n33-k4.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n51-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n76-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n76-k14.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n76-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n76-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/F-n135-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/F-n45-k4.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/F-n72-k4.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n101-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n121-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n151-k12.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n200-k16.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n200-k17.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n101-k4.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n16-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n19-k2.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n20-k2.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n21-k2.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n22-k2.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n22-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n23-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n40-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n45-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n50-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n50-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n50-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n51-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n55-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n55-k15.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n55-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n60-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n60-k15.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n65-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n70-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n76-k4.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n76-k5.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n101-k25.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n106-k14.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n110-k13.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n115-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n120-k6.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n125-k30.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n129-k18.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n134-k13.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n139-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n143-k7.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n148-k46.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n153-k22.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n157-k13.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n162-k11.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n167-k10.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n172-k51.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n176-k26.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n181-k23.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n186-k15.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n190-k8.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n195-k51.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n200-k36.vrp
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.959573 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C101.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C102.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C103.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C104.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C105.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C106.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C107.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C108.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C109.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_6.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C201.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C202.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C203.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C204.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C205.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C206.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C207.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C208.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_6.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R101.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R102.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R103.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R104.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R105.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R106.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R107.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R108.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R109.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R110.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R111.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R112.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_6.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R201.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R202.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R203.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R204.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R205.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R206.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R207.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R208.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R209.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R210.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R211.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_6.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC101.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC102.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC103.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC104.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC105.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC106.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC107.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC108.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_6.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC201.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC202.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC203.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC204.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC205.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC206.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC207.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC208.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_10.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_6.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_8.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_9.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.967573 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X101-FSMFD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X106-FSMD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X110-HD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X115-HVRP.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X120-FSMF.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X125-HVRP.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X129-FSMFD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X134-FSMD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X139-HD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X143-FSMF.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X148-HVRP.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X153-FSMFD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X157-HD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X162-FSMD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X167-FSMF.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X172-HVRP.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X176-FSMFD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X181-HD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X186-FSMD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X190-FSMF.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X195-FSMF.vrp
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X200-HD.vrp
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19fsmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19fsmf.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19fsmfd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19hd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19hvrp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20fsmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20fsmf.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20fsmfd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20hd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20hvrp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13fsmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13fsmf.txt
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13fsmfd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13hd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13hvrp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14fsmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14fsmf.txt
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14fsmfd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14hd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14hvrp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15fsmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15fsmf.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15fsmfd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15hd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15hvrp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16fsmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16fsmf.txt
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16fsmfd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16hd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16hvrp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17fsmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17fsmf.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17fsmfd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17hd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17hvrp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18fsmd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18fsmf.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18fsmfd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18hd.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18hvrp.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.971573 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p01
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p02
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p03
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p04
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p05
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p06
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p07
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p08
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p09
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p10
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p11
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p12
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p13
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p14
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p15
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p16
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p17
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p18
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p19
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p20
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p21
--rw-r--r--   0 runner    (1001) docker     (123)    17560 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p22
--rw-r--r--   0 runner    (1001) docker     (123)    17560 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p23
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pfbo
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr01
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr02
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr03
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr04
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr05
--rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr06
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr07
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr08
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr09
--rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr10
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/demos/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.927573 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.971573 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Darwin/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  9951968 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Darwin/libbapcod-shared.dylib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.983574 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Linux/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 11077488 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Linux/libbapcod-shared.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.999574 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  5190656 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/bapcod-shared.dll
--rw-r--r--   0 runner    (1001) docker     (123)   567184 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/msvcp140.dll
--rw-r--r--   0 runner    (1001) docker     (123)    98192 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/vcruntime140.dll
--rw-r--r--   0 runner    (1001) docker     (123)    38288 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/vcruntime140_1.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.999574 VRPSolverEasy-0.1.2/VRPSolverEasy/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    60570 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/src/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.999574 VRPSolverEasy-0.1.2/VRPSolverEasy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.999574 VRPSolverEasy-0.1.2/VRPSolverEasy/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/tests/config/bc.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    30179 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/VRPSolverEasy/tests/unit_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:34:03.927573 VRPSolverEasy-0.1.2/VRPSolverEasy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-04-06 08:34:03.000000 VRPSolverEasy-0.1.2/VRPSolverEasy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-06 08:34:03.000000 VRPSolverEasy-0.1.2/VRPSolverEasy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:34:03.000000 VRPSolverEasy-0.1.2/VRPSolverEasy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-06 08:34:03.000000 VRPSolverEasy-0.1.2/VRPSolverEasy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 08:34:03.000000 VRPSolverEasy-0.1.2/VRPSolverEasy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-06 08:33:43.000000 VRPSolverEasy-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-06 08:34:03.999574 VRPSolverEasy-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.834350 VRPSolverEasy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-11 12:44:58.834350 VRPSolverEasy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.742348 VRPSolverEasy-0.1.3/VRPSolverEasy/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.742348 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/CVRP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/CVRPTW.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/HFVRP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/MDVRP.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.742348 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.762348 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n32-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n33-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n33-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n34-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n36-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n37-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n37-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n38-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n39-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n39-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n44-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n45-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n45-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n46-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n48-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n53-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n54-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n55-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n60-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n61-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n62-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n63-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n63-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n64-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n65-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n69-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n80-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n31-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n34-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n35-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n38-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n39-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n41-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n43-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n44-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n45-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n45-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n50-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n50-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n51-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n52-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n56-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n57-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n57-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n63-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n64-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n66-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n67-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n68-k9.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n78-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n101-k14.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n101-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n22-k4.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n23-k3.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n30-k3.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n33-k4.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n51-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n76-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n76-k14.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n76-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n76-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/F-n135-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/F-n45-k4.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/F-n72-k4.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n101-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n121-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n151-k12.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n200-k16.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n200-k17.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n101-k4.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n16-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n19-k2.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n20-k2.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n21-k2.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n22-k2.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n22-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n23-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n40-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n45-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n50-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n50-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n50-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n51-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n55-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n55-k15.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n55-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n60-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n60-k15.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n65-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n70-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n76-k4.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n76-k5.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n101-k25.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n106-k14.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n110-k13.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n115-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n120-k6.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n125-k30.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n129-k18.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n134-k13.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n139-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n143-k7.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n148-k46.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n153-k22.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n157-k13.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n162-k11.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n167-k10.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n172-k51.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n176-k26.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n181-k23.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n186-k15.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n190-k8.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n195-k51.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n200-k36.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.786349 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C101.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C102.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C103.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C104.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C105.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C106.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C107.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C108.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C109.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C201.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C202.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C203.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C204.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C205.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C206.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C207.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C208.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R101.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R102.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R103.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R104.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R105.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R106.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R107.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R108.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R109.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R110.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R111.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R112.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R201.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R202.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R203.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R204.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R205.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R206.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R207.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R208.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R209.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R210.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R211.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC101.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC102.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC103.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC104.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC105.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC106.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC107.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC108.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC201.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC202.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC203.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC204.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC205.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC206.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC207.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC208.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.798349 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X101-FSMFD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X106-FSMD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X110-HD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X115-HVRP.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X120-FSMF.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X125-HVRP.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X129-FSMFD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X134-FSMD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X139-HD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X143-FSMF.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X148-HVRP.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X153-FSMFD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X157-HD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X162-FSMD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X167-FSMF.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X172-HVRP.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X176-FSMFD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X181-HD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X186-FSMD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X190-FSMF.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X195-FSMF.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X200-HD.vrp
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19fsmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19fsmf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19fsmfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19hd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19hvrp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20fsmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20fsmf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20fsmfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20hd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20hvrp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13fsmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13fsmf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13fsmfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13hd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13hvrp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14fsmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14fsmf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14fsmfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14hd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14hvrp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15fsmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15fsmf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15fsmfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15hd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15hvrp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16fsmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16fsmf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16fsmfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16hd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16hvrp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17fsmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17fsmf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17fsmfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17hd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17hvrp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18fsmd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18fsmf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18fsmfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18hd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18hvrp.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.806349 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p01
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p02
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p03
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p04
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p05
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p06
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p07
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p08
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p09
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p10
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p11
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p12
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p13
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p14
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p15
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p16
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p17
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p18
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p19
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p20
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p21
+-rw-r--r--   0 runner    (1001) docker     (123)    17560 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p22
+-rw-r--r--   0 runner    (1001) docker     (123)    17560 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p23
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pfbo
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr01
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr02
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr03
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr04
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr05
+-rw-r--r--   0 runner    (1001) docker     (123)    11106 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr06
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr07
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr08
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr09
+-rw-r--r--   0 runner    (1001) docker     (123)    12910 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr10
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/demos/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.742348 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.806349 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  9951968 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Darwin/libbapcod-shared.dylib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.814350 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 11077488 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Linux/libbapcod-shared.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.834350 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  5190656 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/bapcod-shared.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   567184 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/msvcp140.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    98192 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/vcruntime140.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    38288 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/vcruntime140_1.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.834350 VRPSolverEasy-0.1.3/VRPSolverEasy/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60570 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/src/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.834350 VRPSolverEasy-0.1.3/VRPSolverEasy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.834350 VRPSolverEasy-0.1.3/VRPSolverEasy/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/tests/config/bc.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    30179 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/VRPSolverEasy/tests/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:44:58.742348 VRPSolverEasy-0.1.3/VRPSolverEasy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-11 12:44:58.000000 VRPSolverEasy-0.1.3/VRPSolverEasy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-11 12:44:58.000000 VRPSolverEasy-0.1.3/VRPSolverEasy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:44:58.000000 VRPSolverEasy-0.1.3/VRPSolverEasy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 12:44:58.000000 VRPSolverEasy-0.1.3/VRPSolverEasy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 12:44:58.000000 VRPSolverEasy-0.1.3/VRPSolverEasy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-11 12:44:41.000000 VRPSolverEasy-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-11 12:44:58.838350 VRPSolverEasy-0.1.3/setup.cfg
```

### Comparing `VRPSolverEasy-0.1.2/LICENSE.txt` & `VRPSolverEasy-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/PKG-INFO` & `VRPSolverEasy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: VRPSolverEasy
-Version: 0.1.2
+Version: 0.1.3
 Summary: 'VRPSolverEasy is a simplified modeler solving routing problems by using a Branch-Cut-and-Price approach on a solver like CLP or CPLEX'
-Home-page: https://vrpsolvereasy.readthedocs.io/en/latest/
+Home-page: https://github.com/inria-UFF/VRPSolverEasy
 Author: "UCHOA Eduardo SADYKOV Ruslan QUEIROGA Eduardo ERRAMI Najib"
 Author-email: "najib.errami@inria.fr"
 Keywords: ['VRP','Branch-Cut-&Price','Operations Research','Optimization','Linear Programming','Routing problems','Solver','Supply chain']
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -127,40 +127,38 @@
 -------
 
 A simple example that shows how to use the VRPSolverEasy package:
 
 .. code:: python
 
 
-   import math
    import VRPSolverEasy as vrpse
+   import math
 
    def compute_euclidean_distance(x_i, y_i, x_j, y_j):
        """compute the euclidean distance between 2 points from graph"""
-       return round(math.sqrt((x_i - x_j)**2 +
-                              (y_i - y_j)**2), 3)
+       return round(math.sqrt((x_i - x_j)**2 + (y_i - y_j)**2), 3)
 
-   # data
+   # Data
    cost_per_distance = 10
    begin_time = 0
    end_time = 5000
    nb_point = 7
 
-   # map with names and coordinates
+   # Map with names and coordinates
    coordinates = {"Wisconsin, USA": (44.50, -89.50),  # depot
                   "West Virginia, USA": (39.000000, -80.500000),
                   "Vermont, USA": (44.000000, -72.699997),
                   "Texas, the USA": (31.000000, -100.000000),
                   "South Dakota, the US": (44.500000, -100.000000),
                   "Rhode Island, the US": (41.742325, -71.742332),
                   "Oregon, the US": (44.000000, -120.500000)
                   }
 
-
-   # demands of points
+   # Demands of points
    demands = [0, 500, 300, 600, 658, 741, 436]
 
    # Initialisation
    model = vrpse.Model()
 
    # Add vehicle type
    model.add_vehicle_type(
@@ -173,15 +171,15 @@
        var_cost_dist=cost_per_distance,
        tw_end=5000)
 
    # Add depot
    model.add_depot(id=0, name="D1", tw_begin=0, tw_end=5000)
 
    coordinates_keys = list(coordinates.keys())
-   # Add Customers
+   # Add customers
    for i in range(1, nb_point):
        model.add_customer(
            id=i,
            name=coordinates_keys[i],
            demand=demands[i],
            tw_begin=begin_time,
            tw_end=end_time)
```

### Comparing `VRPSolverEasy-0.1.2/README.rst` & `VRPSolverEasy-0.1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -106,40 +106,38 @@
 -------
 
 A simple example that shows how to use the VRPSolverEasy package:
 
 .. code:: python
 
 
-   import math
    import VRPSolverEasy as vrpse
+   import math
 
    def compute_euclidean_distance(x_i, y_i, x_j, y_j):
        """compute the euclidean distance between 2 points from graph"""
-       return round(math.sqrt((x_i - x_j)**2 +
-                              (y_i - y_j)**2), 3)
+       return round(math.sqrt((x_i - x_j)**2 + (y_i - y_j)**2), 3)
 
-   # data
+   # Data
    cost_per_distance = 10
    begin_time = 0
    end_time = 5000
    nb_point = 7
 
-   # map with names and coordinates
+   # Map with names and coordinates
    coordinates = {"Wisconsin, USA": (44.50, -89.50),  # depot
                   "West Virginia, USA": (39.000000, -80.500000),
                   "Vermont, USA": (44.000000, -72.699997),
                   "Texas, the USA": (31.000000, -100.000000),
                   "South Dakota, the US": (44.500000, -100.000000),
                   "Rhode Island, the US": (41.742325, -71.742332),
                   "Oregon, the US": (44.000000, -120.500000)
                   }
 
-
-   # demands of points
+   # Demands of points
    demands = [0, 500, 300, 600, 658, 741, 436]
 
    # Initialisation
    model = vrpse.Model()
 
    # Add vehicle type
    model.add_vehicle_type(
@@ -152,15 +150,15 @@
        var_cost_dist=cost_per_distance,
        tw_end=5000)
 
    # Add depot
    model.add_depot(id=0, name="D1", tw_begin=0, tw_end=5000)
 
    coordinates_keys = list(coordinates.keys())
-   # Add Customers
+   # Add customers
    for i in range(1, nb_point):
        model.add_customer(
            id=i,
            name=coordinates_keys[i],
            demand=demands[i],
            tw_begin=begin_time,
            tw_end=end_time)
```

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/CVRP.py` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/CVRP.py`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/CVRPTW.py` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/CVRPTW.py`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/HFVRP.py` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/HFVRP.py`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/MDVRP.py` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/MDVRP.py`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n32-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n32-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n33-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n33-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n33-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n33-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n34-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n34-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n36-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n36-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n37-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n37-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n37-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n37-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n38-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n38-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n39-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n39-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n39-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n39-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n44-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n44-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n45-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n45-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n45-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n45-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n46-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n46-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n48-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n48-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n53-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n53-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n54-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n54-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n55-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n55-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n60-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n60-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n61-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n61-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n62-k8.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n62-k8.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n63-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n63-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n63-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n63-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n64-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n64-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n65-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n65-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n69-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n69-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/A-n80-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/A-n80-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n31-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n31-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n34-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n34-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n35-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n35-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n38-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n38-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n39-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n39-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n41-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n41-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n43-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n43-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n44-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n44-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n45-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n45-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n45-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n45-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n50-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n50-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n50-k8.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n50-k8.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n51-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n51-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n52-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n52-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n56-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n56-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n57-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n57-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n57-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n57-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n63-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n63-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n64-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n64-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n66-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n66-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n67-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n67-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n68-k9.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n68-k9.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/B-n78-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/B-n78-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n101-k14.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n101-k14.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n101-k8.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n101-k8.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n22-k4.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n22-k4.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n23-k3.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n23-k3.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n30-k3.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n30-k3.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n33-k4.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n33-k4.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n51-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n51-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n76-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n76-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n76-k14.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n76-k14.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n76-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n76-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/E-n76-k8.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/E-n76-k8.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/F-n135-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/F-n135-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/F-n45-k4.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/F-n45-k4.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/F-n72-k4.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/F-n72-k4.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n101-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n101-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n121-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n121-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n151-k12.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n151-k12.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n200-k16.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n200-k16.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/M-n200-k17.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/M-n200-k17.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n101-k4.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n101-k4.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n22-k8.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n22-k8.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n23-k8.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n23-k8.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n40-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n40-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n45-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n45-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n50-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n50-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n50-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n50-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n50-k8.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n50-k8.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n51-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n51-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n55-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n55-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n55-k15.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n55-k15.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n55-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n55-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n60-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n60-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n60-k15.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n60-k15.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n65-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n65-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n70-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n70-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n76-k4.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n76-k4.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/P-n76-k5.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/P-n76-k5.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n101-k25.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n101-k25.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n106-k14.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n106-k14.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n110-k13.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n110-k13.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n115-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n115-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n120-k6.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n120-k6.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n125-k30.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n125-k30.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n129-k18.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n129-k18.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n134-k13.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n134-k13.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n139-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n139-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n143-k7.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n143-k7.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n148-k46.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n148-k46.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n153-k22.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n153-k22.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n157-k13.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n157-k13.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n162-k11.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n162-k11.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n167-k10.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n167-k10.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n172-k51.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n172-k51.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n176-k26.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n176-k26.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n181-k23.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n181-k23.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n186-k15.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n186-k15.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n190-k8.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n190-k8.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n195-k51.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n195-k51.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRP/X-n200-k36.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRP/X-n200-k36.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C101.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C101.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C102.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C102.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C103.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C103.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C104.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C104.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C105.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C105.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C106.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C106.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C107.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C107.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C108.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C108.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C109.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C109.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_1.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_1.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_10.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_10.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_2.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_2.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_3.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_3.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_4.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_4.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_5.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_5.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_6.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_6.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_7.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_7.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_8.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_8.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C1_2_9.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C1_2_9.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C201.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C201.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C202.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C202.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C203.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C203.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C204.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C204.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C205.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C205.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C206.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C206.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C207.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C207.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C208.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C208.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_1.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_1.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_10.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_10.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_2.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_2.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_3.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_3.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_4.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_4.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_5.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_5.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_6.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_6.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_7.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_7.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_8.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_8.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/C2_2_9.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/C2_2_9.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R101.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R101.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R102.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R102.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R103.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R103.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R104.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R104.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R105.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R105.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R106.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R106.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R107.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R107.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R108.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R108.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R109.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R109.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R110.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R110.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R111.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R111.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R112.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R112.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_1.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_1.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_10.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_10.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_2.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_2.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_3.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_3.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_4.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_4.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_5.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_5.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_6.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_6.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_7.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_7.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_8.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_8.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R1_2_9.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R1_2_9.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R201.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R201.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R202.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R202.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R203.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R203.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R204.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R204.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R205.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R205.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R206.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R206.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R207.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R207.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R208.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R208.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R209.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R209.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R210.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R210.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R211.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R211.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_1.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_1.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_10.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_10.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_2.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_2.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_3.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_3.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_4.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_4.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_5.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_5.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_6.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_6.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_7.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_7.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_8.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_8.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/R2_2_9.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/R2_2_9.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC101.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC101.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC102.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC102.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC103.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC103.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC104.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC104.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC105.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC105.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC106.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC106.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC107.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC107.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC108.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC108.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_1.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_1.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_10.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_10.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_2.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_2.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_3.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_3.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_4.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_4.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_5.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_5.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_6.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_6.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_7.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_7.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_8.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_8.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC1_2_9.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC1_2_9.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC201.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC201.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC202.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC202.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC203.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC203.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC204.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC204.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC205.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC205.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC206.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC206.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC207.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC207.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC208.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC208.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_1.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_1.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_10.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_10.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_2.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_2.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_3.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_3.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_4.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_4.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_5.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_5.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_6.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_6.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_7.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_7.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_8.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_8.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/CVRPTW/RC2_2_9.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/CVRPTW/RC2_2_9.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X101-FSMFD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X101-FSMFD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X106-FSMD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X106-FSMD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X110-HD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X110-HD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X115-HVRP.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X115-HVRP.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X120-FSMF.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X120-FSMF.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X125-HVRP.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X125-HVRP.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X129-FSMFD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X129-FSMFD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X134-FSMD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X134-FSMD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X139-HD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X139-HD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X143-FSMF.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X143-FSMF.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X148-HVRP.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X148-HVRP.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X153-FSMFD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X153-FSMFD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X157-HD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X157-HD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X162-FSMD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X162-FSMD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X167-FSMF.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X167-FSMF.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X172-HVRP.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X172-HVRP.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X176-FSMFD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X176-FSMFD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X181-HD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X181-HD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X186-FSMD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X186-FSMD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X190-FSMF.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X190-FSMF.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X195-FSMF.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X195-FSMF.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/X200-HD.vrp` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/X200-HD.vrp`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19fsmd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19fsmd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19fsmf.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19fsmf.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19fsmfd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19fsmfd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19hd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19hd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_19hvrp.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_19hvrp.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20fsmd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20fsmd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20fsmf.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20fsmf.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20fsmfd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20fsmfd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20hd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20hd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c100_20hvrp.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c100_20hvrp.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13fsmd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13fsmd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13fsmf.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13fsmf.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13fsmfd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13fsmfd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13hd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13hd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_13hvrp.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_13hvrp.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14fsmd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14fsmd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14fsmf.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14fsmf.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14fsmfd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14fsmfd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14hd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14hd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_14hvrp.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_14hvrp.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15fsmd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15fsmd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15fsmf.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15fsmf.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15fsmfd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15fsmfd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15hd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15hd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_15hvrp.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_15hvrp.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16fsmd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16fsmd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16fsmf.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16fsmf.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16fsmfd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16fsmfd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16hd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16hd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c50_16hvrp.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c50_16hvrp.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17fsmd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17fsmd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17fsmf.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17fsmf.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17fsmfd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17fsmfd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17hd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17hd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_17hvrp.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_17hvrp.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18fsmd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18fsmd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18fsmf.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18fsmf.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18fsmfd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18fsmfd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18hd.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18hd.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/HFVRP/c75_18hvrp.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/HFVRP/c75_18hvrp.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p01` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p01`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p02` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p02`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p03` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p03`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p04` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p04`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p05` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p05`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p06` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p06`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p07` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p07`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p08` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p08`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p09` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p09`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p10` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p10`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p11` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p11`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p12` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p12`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p13` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p13`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p14` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p14`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p15` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p15`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p16` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p16`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p17` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p17`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p18` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p18`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p19` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p19`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p20` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p20`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p21` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p21`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p22` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p22`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/p23` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/p23`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr01` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr01`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr02` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr02`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr03` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr03`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr04` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr04`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr05` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr05`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr06` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr06`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr07` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr07`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr08` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr08`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr09` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr09`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/data/MDVRP/pr10` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/data/MDVRP/pr10`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/demos/example.py` & `VRPSolverEasy-0.1.3/VRPSolverEasy/demos/example.py`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Darwin/libbapcod-shared.dylib` & `VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Darwin/libbapcod-shared.dylib`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Linux/libbapcod-shared.so` & `VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Linux/libbapcod-shared.so`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/bapcod-shared.dll` & `VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/bapcod-shared.dll`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/msvcp140.dll` & `VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/vcruntime140.dll` & `VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/lib/Windows/vcruntime140_1.dll` & `VRPSolverEasy-0.1.3/VRPSolverEasy/lib/Windows/vcruntime140_1.dll`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/src/constants.py` & `VRPSolverEasy-0.1.3/VRPSolverEasy/src/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 # VRPSolverReal informations
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 
 LIBRARY_WINDOWS = "bapcod-shared.dll"
 LIBRARY_LINUX = "libbapcod-shared.so"
 LIBRARY_MAC = "libbapcod-shared.dylib"
 
 WINDOWS_PLATFORM = "Windows"
 LINUX_PLATFORM = "Linux"
```

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/src/solver.py` & `VRPSolverEasy-0.1.3/VRPSolverEasy/src/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from VRPSolverEasy.src import constants
 if sys.version_info > (3, 7):
     import collections.abc as collections
 else:
     import collections
 
 ########
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = "Najib ERRAMI Ruslan SADYKOV Eduardo UCHOA Eduardo QUEIROGA"
 __copyright__ = "Copyright VRPYSolver, all rights reserved"
 __email__ = "najib.errami@inria.fr"
 
 
 class PropertyError(Exception):
     """Exception raised for errors in the input property.
```

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/tests/config/bc.cfg` & `VRPSolverEasy-0.1.3/VRPSolverEasy/tests/config/bc.cfg`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy/tests/unit_tests.py` & `VRPSolverEasy-0.1.3/VRPSolverEasy/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy.egg-info/PKG-INFO` & `VRPSolverEasy-0.1.3/VRPSolverEasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: VRPSolverEasy
-Version: 0.1.2
+Version: 0.1.3
 Summary: 'VRPSolverEasy is a simplified modeler solving routing problems by using a Branch-Cut-and-Price approach on a solver like CLP or CPLEX'
-Home-page: https://vrpsolvereasy.readthedocs.io/en/latest/
+Home-page: https://github.com/inria-UFF/VRPSolverEasy
 Author: "UCHOA Eduardo SADYKOV Ruslan QUEIROGA Eduardo ERRAMI Najib"
 Author-email: "najib.errami@inria.fr"
 Keywords: ['VRP','Branch-Cut-&Price','Operations Research','Optimization','Linear Programming','Routing problems','Solver','Supply chain']
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -127,40 +127,38 @@
 -------
 
 A simple example that shows how to use the VRPSolverEasy package:
 
 .. code:: python
 
 
-   import math
    import VRPSolverEasy as vrpse
+   import math
 
    def compute_euclidean_distance(x_i, y_i, x_j, y_j):
        """compute the euclidean distance between 2 points from graph"""
-       return round(math.sqrt((x_i - x_j)**2 +
-                              (y_i - y_j)**2), 3)
+       return round(math.sqrt((x_i - x_j)**2 + (y_i - y_j)**2), 3)
 
-   # data
+   # Data
    cost_per_distance = 10
    begin_time = 0
    end_time = 5000
    nb_point = 7
 
-   # map with names and coordinates
+   # Map with names and coordinates
    coordinates = {"Wisconsin, USA": (44.50, -89.50),  # depot
                   "West Virginia, USA": (39.000000, -80.500000),
                   "Vermont, USA": (44.000000, -72.699997),
                   "Texas, the USA": (31.000000, -100.000000),
                   "South Dakota, the US": (44.500000, -100.000000),
                   "Rhode Island, the US": (41.742325, -71.742332),
                   "Oregon, the US": (44.000000, -120.500000)
                   }
 
-
-   # demands of points
+   # Demands of points
    demands = [0, 500, 300, 600, 658, 741, 436]
 
    # Initialisation
    model = vrpse.Model()
 
    # Add vehicle type
    model.add_vehicle_type(
@@ -173,15 +171,15 @@
        var_cost_dist=cost_per_distance,
        tw_end=5000)
 
    # Add depot
    model.add_depot(id=0, name="D1", tw_begin=0, tw_end=5000)
 
    coordinates_keys = list(coordinates.keys())
-   # Add Customers
+   # Add customers
    for i in range(1, nb_point):
        model.add_customer(
            id=i,
            name=coordinates_keys[i],
            demand=demands[i],
            tw_begin=begin_time,
            tw_end=end_time)
```

### Comparing `VRPSolverEasy-0.1.2/VRPSolverEasy.egg-info/SOURCES.txt` & `VRPSolverEasy-0.1.3/VRPSolverEasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VRPSolverEasy-0.1.2/setup.cfg` & `VRPSolverEasy-0.1.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = VRPSolverEasy
-version = 0.1.2
+version = 0.1.3
 author = "UCHOA Eduardo SADYKOV Ruslan QUEIROGA Eduardo ERRAMI Najib"
 author_email = "najib.errami@inria.fr"
-url = https://vrpsolvereasy.readthedocs.io/en/latest/
+url = https://github.com/inria-UFF/VRPSolverEasy
 description = 'VRPSolverEasy is a simplified modeler solving routing problems by using a Branch-Cut-and-Price approach on a solver like CLP or CPLEX'
 long_description = file: README.rst
 license_files = LICENSE.txt
 keywords = ['VRP','Branch-Cut-&Price','Operations Research','Optimization','Linear Programming','Routing problems','Solver','Supply chain']
 classifier = 
 	Development Status :: 4 - Beta
 	Environment :: Console
```

