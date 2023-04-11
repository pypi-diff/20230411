# Comparing `tmp/atlas-densities-0.1.3.tar.gz` & `tmp/atlas-densities-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlas-densities-0.1.3.tar", last modified: Thu Nov 17 13:31:29 2022, max compression
+gzip compressed data, was "atlas-densities-0.1.4.tar", last modified: Tue Apr 11 08:53:26 2023, max compression
```

## Comparing `atlas-densities-0.1.3.tar` & `atlas-densities-0.1.4.tar`

### file list

```diff
@@ -1,191 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.357059 atlas-densities-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.325059 atlas-densities-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.333059 atlas-densities-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    23400 2022-11-17 13:31:29.353059 atlas-densities-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19330 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    55115 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas-densities.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.333059 atlas-densities-0.1.3/atlas_densities/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.333059 atlas-densities-0.1.3/atlas_densities/app/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40084 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/cell_densities.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7873 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.333059 atlas-densities-0.1.3/atlas_densities/app/data/
--rw-r--r--   0 runner    (1001) docker     (121)   637735 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/1.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.337059 atlas-densities-0.1.3/atlas_densities/app/data/markers/
--rw-r--r--   0 runner    (1001) docker     (121)     4228 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/markers/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/markers/realigned_slices_bbp.json
--rw-r--r--   0 runner    (1001) docker     (121)     7524 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/markers/realigned_slices_ccfv2.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.337059 atlas-densities-0.1.3/atlas_densities/app/data/measurements/
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/._std_cells.json
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    59787 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/gaba_papers.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/homogenous_regions.csv
--rw-r--r--   0 runner    (1001) docker     (121)   839727 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/measurements.csv
--rw-r--r--   0 runner    (1001) docker     (121)   347207 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/mmc1.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)   291827 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/mmc3.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)    13614 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/non_density_measurements.csv
--rw-r--r--   0 runner    (1001) docker     (121)   199258 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/measurements/std_cells.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.341059 atlas-densities-0.1.3/atlas_densities/app/data/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/metadata/ca1_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/metadata/excitatory-inhibitory-splitting.json
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/metadata/isocortex_23_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/metadata/isocortex_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/metadata/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/metadata/thalamus_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.341059 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.341059 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/composition/
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/composition/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10928 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/composition/composition.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.341059 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.341059 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/meta/layers.tsv
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.345059 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_DAC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_HAC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_LAC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-DA.dat
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-SA.dat
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_SAC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_SSC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_TPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TPC-C.dat
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_BPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_HPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-C.dat
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_UPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      660 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.345059 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/probability_map/
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/probability_map/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14404 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/data/mtypes/probability_map/probability_map.csv
--rw-r--r--   0 runner    (1001) docker     (121)    20294 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/mtype_densities.py
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.345059 atlas-densities-0.1.3/atlas_densities/combination/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5272 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/combination/annotations_combinator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7295 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/combination/markers_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.345059 atlas-densities-0.1.3/atlas_densities/densities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11342 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/cell_counts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/cell_density.py
--rw-r--r--   0 runner    (1001) docker     (121)    25935 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3843 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/excitatory_inhibitory_splitting.py
--rw-r--r--   0 runner    (1001) docker     (121)    27739 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/fitting.py
--rw-r--r--   0 runner    (1001) docker     (121)     8008 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/glia_densities.py
--rw-r--r--   0 runner    (1001) docker     (121)     7916 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/inhibitory_neuron_densities_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    33784 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/inhibitory_neuron_densities_optimization.py
--rw-r--r--   0 runner    (1001) docker     (121)     8830 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (121)    15479 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/measurement_to_density.py
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/mtype_densities_from_composition.py
--rw-r--r--   0 runner    (1001) docker     (121)    12051 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/mtype_densities_from_map.py
--rw-r--r--   0 runner    (1001) docker     (121)    22055 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/mtype_densities_from_profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)    21524 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/refined_inhibitory_neuron_densities.py
--rw-r--r--   0 runner    (1001) docker     (121)    26678 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/densities/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10610 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/atlas_densities/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.333059 atlas-densities-0.1.3/atlas_densities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23400 2022-11-17 13:31:28.000000 atlas-densities-0.1.3/atlas_densities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7633 2022-11-17 13:31:29.000000 atlas-densities-0.1.3/atlas_densities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-17 13:31:28.000000 atlas-densities-0.1.3/atlas_densities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-17 13:31:28.000000 atlas-densities-0.1.3/atlas_densities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-11-17 13:31:28.000000 atlas-densities-0.1.3/atlas_densities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-17 13:31:28.000000 atlas-densities-0.1.3/atlas_densities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.345059 atlas-densities-0.1.3/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.349059 atlas-densities-0.1.3/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)   230179 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/bbpp82_628_linear_program.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/cell_densities.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/combination.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6651 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/mtype_densities.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/doc/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-17 13:31:29.357059 atlas-densities-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.349059 atlas-densities-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)   637735 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/1.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.353059 atlas-densities-0.1.3/tests/app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15159 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/app/test_cell_densities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3639 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/app/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (121)    18212 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/app/test_mtype_densities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/app/test_refined_inhibitory_neuron_densities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.353059 atlas-densities-0.1.3/tests/combination/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8828 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/combination/test_annotations_combinator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3362 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/combination/test_markers_combinator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.353059 atlas-densities-0.1.3/tests/densities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.329059 atlas-densities-0.1.3/tests/densities/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.353059 atlas-densities-0.1.3/tests/densities/data/meta/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/meta/layers.tsv
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/meta/mapping.tsv
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/meta/mapping_exc_only.tsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-17 13:31:29.353059 atlas-densities-0.1.3/tests/densities/data/mtypes/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/mtypes/BP.dat
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/mtypes/L2_IPC.dat
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/mtypes/L2_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/mtypes/L3_TPC-A.dat
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/mtypes/L3_TPC-B.dat
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/data/mtypes/mtype-taxonomy.tsv
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_cell_counts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_cell_density.py
--rw-r--r--   0 runner    (1001) docker     (121)    14023 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_excel_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    10133 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_excitatory_inhibitory_splitting.py
--rw-r--r--   0 runner    (1001) docker     (121)    19714 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_fitting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5165 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_glia_densities.py
--rw-r--r--   0 runner    (1001) docker     (121)     6785 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_inhibitory_neuron_densities_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     5973 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (121)     9897 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_inhibitory_neuron_density_optimization.py
--rw-r--r--   0 runner    (1001) docker     (121)    12395 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_measurement_to_density.py
--rw-r--r--   0 runner    (1001) docker     (121)     5355 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_mtype_densities_from_composition.py
--rw-r--r--   0 runner    (1001) docker     (121)    10654 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_mtype_densities_from_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     8771 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_mtype_densities_from_profiles.py
--rw-r--r--   0 runner    (1001) docker     (121)    25302 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_optimization_initialization.py
--rw-r--r--   0 runner    (1001) docker     (121)    13993 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_refined_inhibitory_neuron_density.py
--rw-r--r--   0 runner    (1001) docker     (121)    14539 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/densities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/markers_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/mocking_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     9143 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-11-17 13:31:23.000000 atlas-densities-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.761378 atlas-densities-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.717378 atlas-densities-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-04-11 08:53:26.761378 atlas-densities-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    55115 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas-densities.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/atlas_densities/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/atlas_densities/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40078 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/cell_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.725378 atlas-densities-0.1.4/atlas_densities/app/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   637735 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.725378 atlas-densities-0.1.4/atlas_densities/app/data/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/realigned_slices_bbp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/markers/realigned_slices_ccfv2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59787 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/gaba_papers.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/homogenous_regions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   839727 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   347207 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/mmc1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   291827 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/mmc3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/non_density_measurements.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   199258 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/measurements/std_cells.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/ca1_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/excitatory-inhibitory-splitting.json
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/isocortex_23_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/isocortex_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/metadata/thalamus_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/composition.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.733378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/meta/layers.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.737378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_DAC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_HAC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_LAC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-DA.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_NGC-SA.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L1_SAC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L2_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L3_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_SSC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_TPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L4_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TPC-C.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_TTPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L5_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_BPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_HPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_TPC-C.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/L6_UPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/mtypes_probability_map_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.737378 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/probability_map.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/mtype_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.737378 atlas-densities-0.1.4/atlas_densities/combination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/combination/annotations_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/combination/markers_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.745378 atlas-densities-0.1.4/atlas_densities/densities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/cell_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/excitatory_inhibitory_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27944 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/glia_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_densities_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33784 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_densities_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/measurement_to_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22055 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21524 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/refined_inhibitory_neuron_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26913 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/densities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/atlas_densities/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/atlas_densities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23400 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 08:53:26.000000 atlas-densities-0.1.4/atlas_densities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.745378 atlas-densities-0.1.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.749378 atlas-densities-0.1.4/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)   230179 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/bbpp82_628_linear_program.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/cell_densities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/combination.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/mtype_densities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/doc/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:53:26.761378 atlas-densities-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.749378 atlas-densities-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   637735 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.753378 atlas-densities-0.1.4/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/test_cell_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18212 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/test_mtype_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/app/test_refined_inhibitory_neuron_densities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.753378 atlas-densities-0.1.4/tests/combination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/combination/test_annotations_combinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/combination/test_markers_combinator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.757378 atlas-densities-0.1.4/tests/densities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.721378 atlas-densities-0.1.4/tests/densities/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.757378 atlas-densities-0.1.4/tests/densities/data/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/meta/layers.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/meta/mapping.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/meta/mapping_exc_only.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:26.761378 atlas-densities-0.1.4/tests/densities/data/mtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/BP.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/L2_IPC.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/L2_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/L3_TPC-A.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/L3_TPC-B.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/data/mtypes/mtype-taxonomy.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_cell_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_cell_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_excel_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_excitatory_inhibitory_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19954 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_glia_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_densities_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_density_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_measurement_to_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25302 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_optimization_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_refined_inhibitory_neuron_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/densities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/markers_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/mocking_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-11 08:53:15.000000 atlas-densities-0.1.4/tox.ini
```

### Comparing `atlas-densities-0.1.3/.github/workflows/publish-sdist.yml` & `atlas-densities-0.1.4/.github/workflows/publish-sdist.yml`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
       - 'v[0-9]+.[0-9]+.[0-9]+'
 
 jobs:
   build-n-publish:
     name: Build and publish on PyPI
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@master
+      - uses: actions/checkout@v3
       - name: Set up Python 3.8
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
 
       - name: Build a source tarball
         run:
             python setup.py sdist
 
       - name: Publish distribution package to PyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_PASSWORD }}
```

### Comparing `atlas-densities-0.1.3/.github/workflows/run-tox.yml` & `atlas-densities-0.1.4/.github/workflows/run-tox.yml`

 * *Files 18% similar despite different names*

```diff
@@ -10,17 +10,17 @@
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ['3.7', '3.8', '3.9', '3.10']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox-gh-actions
@@ -29,17 +29,17 @@
       run: |
         tox -etests
 
   lint:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox
@@ -48,17 +48,17 @@
       run: |
         tox -elint
 
   coverage:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
         pip install tox
```

### Comparing `atlas-densities-0.1.3/.pylintrc` & `atlas-densities-0.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/CONTRIBUTING.rst` & `atlas-densities-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/LICENSE.txt` & `atlas-densities-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/PKG-INFO` & `atlas-densities-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-densities
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library containing command lines and tools to compute volumetric cell densities in the rodent brain
 Home-page: https://github.com/BlueBrain/atlas-densities
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-densities
 Description: .. image:: atlas-densities.jpg
```

### Comparing `atlas-densities-0.1.3/README.rst` & `atlas-densities-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas-densities.jpg` & `atlas-densities-0.1.4/atlas-densities.jpg`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/cell_densities.py` & `atlas-densities-0.1.4/atlas_densities/app/cell_densities.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     The output density field array is a float64 array of shape (W, H, D) where (W, H, D)
     is the shape of the input annotated volume.
 
     The computation of the overall cell density is based on:
 
     \b
     - the Nissl stain intensity, which is supposed to represent the overall cell density, up to
-    to region-dependent constant scaling factors.
+    region-dependent constant scaling factors.
     - cell counts from the scientific literature, which are used to determine a local
     linear dependency factor for each region where a cell count is available.
     - the optional soma radii, used to operate a correction.
     """
 
     annotation = VoxelData.load_nrrd(annotation_path)
     nissl = VoxelData.load_nrrd(nissl_path)
@@ -413,15 +413,15 @@
 
     An optimization process is responsible for enforcing these constraints while keeping
     the output densities as close as possible to the unconstrained input densities.
 
     Note: optimization is not fully implemented and the current process only returns a
     feasible point.
 
-    The ouput densities are saved in the specified output directory under the following
+    The output densities are saved in the specified output directory under the following
     names:
 
     \b
     - inhibitory_neuron_density.nrrd
     - excitatory_neuron_density.nrrd
     """
 
@@ -486,15 +486,15 @@
 
     \b
     - `mm3c.xls` from the supplementary materials of
     'Brain-wide Maps Reveal Stereotyped Cell-Type-Based Cortical Architecture and Subcortical
     Sexual Dimorphism' by Kim et al., 2017.
     https://ars.els-cdn.com/content/image/1-s2.0-S0092867417310693-mmc3.xlsx
     - `atlas_densities/app/data/measurements/gaba_papers.xlsx`, a compilation of measurements
-    from the scientifc literature made by Rodarie Dimitri (BBP).
+    from the scientific literature made by Rodarie Dimitri (BBP).
 
     This command extracts measurements from the above two files and gathers them into a unique
     CSV file with the following columns:
 
     \b
     - brain_region (str), a mouse brain region name, not necessarily compliant
     with AIBS 1.json file. Thus some filtering must be done when working with AIBS
@@ -527,15 +527,15 @@
     - ``neuron proportion``: None (empty)
     - ``cell proportion``: None (empty)
     - ``cell count per slice``: e.g, number of cells per 50-micrometer-thick slice
 
     See `atlas_densities/densities/excel_reader.py` for more information.
 
     Note: This function should be deprecated once its output has been stored permanently as the
-    the unique source of density-related measurements for the AIBS mouse brain. New measurements
+    unique source of density-related measurements for the AIBS mouse brain. New measurements
     should be added to the stored file (Nexus).
     """
 
     L.info("Loading hierarchy ...")
     region_map = RegionMap.load_json(Path(DATA_PATH, "1.json"))  # Unmodified AIBS 1.json
     L.info("Loading excel files ...")
     measurements = read_measurements(
@@ -615,15 +615,15 @@
     For measurements such as cell proportions, neuron proportions or cell counts per slice, the
     brain-wide volumetric cell densities (`cell_density_path` or `neuron_density_path`) are used to
     compute average cell densities.
 
     If several combinations of measurements yield several average cell densities for the same
     region, then the output data frame records the average of these measurements.
 
-    The ouput average cell densities are saved in under the CSV format as a dataframe with the same
+    The output average cell densities are saved in under the CSV format as a dataframe with the same
     columns as the input data frame specified via `--measurements-path`.
     See :mod:`atlas_densities.app.densities.compile_measurements`.
 
     All output measurements are average cell densities of various cell types over AIBS brain
     regions expressed in number of cells per mm^3.
     """
 
@@ -740,15 +740,15 @@
     In addition to the records from the scientific literature, we consider as input of our fitting
     the average densities of the brain regions where neurons are either all inhibitory or all
     excitatory. These regions are listed in `homogenous_regions_path`. The volumetric density
     `neuron_density_path` is used to compute the average density of inhibitory neurons (a.k.a
     gad67+) in every homogenous region of type "inhibitory".
 
     Our linear fitting of density values relies on the assumption that the average cell density
-    (number of cells per mm^3) of a cell type T in a brain region R depends linearily on the
+    (number of cells per mm^3) of a cell type T in a brain region R depends linearly on the
     average intensity of a gene marker of T. The conversion factor is a constant which depends only
     on T and on which of the following three groups R belongs to:
 
     \b
     - isocortex
     - cerebellum
     - the rest
@@ -890,15 +890,15 @@
     labelling the columns of the data frame stored in `average_densities_path`.
 
     This function support the use case of "Atlas of inhibitory neurons in the mouse brain" by
     D. Rodarie et al., 2021. The densities to be computed in this case are those of GAD67+
     (inhibitory neurons) and those of the inhibitory neuron subtypes PV+, SST+ and VIP+.
 
     The function modifies the estimates in `average_densities` (the "first estimates" of the paper)
-    to make them consistent accross cell types: the average density of GAD67+ cells in a leaf
+    to make them consistent across cell types: the average density of GAD67+ cells in a leaf
     region L should be at most the sum of the average densities of its subtypes under scrutiny
     (e.g. PV+, SST+ and VIP+) and should not exceed the neuron density of L.
 
     Two algorithms can be used:
 
     - keep-proportions:
```

### Comparing `atlas-densities-0.1.3/atlas_densities/app/cli.py` & `atlas-densities-0.1.4/atlas_densities/app/cli.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/combination.py` & `atlas-densities-0.1.4/atlas_densities/app/combination.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/1.json` & `atlas-densities-0.1.4/atlas_densities/app/data/1.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/markers/README.rst` & `atlas-densities-0.1.4/atlas_densities/app/data/markers/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml` & `atlas-densities-0.1.4/atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/markers/realigned_slices_bbp.json` & `atlas-densities-0.1.4/atlas_densities/app/data/markers/realigned_slices_bbp.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/markers/realigned_slices_ccfv2.json` & `atlas-densities-0.1.4/atlas_densities/app/data/markers/realigned_slices_ccfv2.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/measurements/README.rst` & `atlas-densities-0.1.4/atlas_densities/app/data/measurements/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/measurements/gaba_papers.xlsx` & `atlas-densities-0.1.4/atlas_densities/app/data/measurements/gaba_papers.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/measurements/homogenous_regions.csv` & `atlas-densities-0.1.4/atlas_densities/app/data/measurements/homogenous_regions.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/measurements/measurements.csv` & `atlas-densities-0.1.4/atlas_densities/app/data/measurements/measurements.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/measurements/mmc1.xlsx` & `atlas-densities-0.1.4/atlas_densities/app/data/measurements/mmc1.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/measurements/mmc3.xlsx` & `atlas-densities-0.1.4/atlas_densities/app/data/measurements/mmc3.xlsx`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/measurements/non_density_measurements.csv` & `atlas-densities-0.1.4/atlas_densities/app/data/measurements/non_density_measurements.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/measurements/std_cells.json` & `atlas-densities-0.1.4/atlas_densities/app/data/measurements/std_cells.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/metadata/thalamus_metadata.json` & `atlas-densities-0.1.4/atlas_densities/app/data/metadata/thalamus_metadata.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/composition/README.rst` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/composition/composition.yaml` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/composition.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/composition/neurons-mtype-taxonomy.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/README.rst` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/meta/mapping.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BP.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/BTC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/CHC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/DBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/LBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/MC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/NGC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/density_profiles/profiles/SBC.dat`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/mapping_cortex_all_to_exc_mtypes.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/probability_map/README.rst` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/README.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/data/mtypes/probability_map/probability_map.csv` & `atlas-densities-0.1.4/atlas_densities/app/data/mtypes/probability_map/probability_map.csv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/app/mtype_densities.py` & `atlas-densities-0.1.4/atlas_densities/app/mtype_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/combination/annotations_combinator.py` & `atlas-densities-0.1.4/atlas_densities/combination/annotations_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/combination/markers_combinator.py` & `atlas-densities-0.1.4/atlas_densities/combination/markers_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/cell_counts.py` & `atlas-densities-0.1.4/atlas_densities/densities/cell_counts.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/cell_density.py` & `atlas-densities-0.1.4/atlas_densities/densities/cell_density.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,11 +103,14 @@
     nissl = np.asarray(nissl, dtype=np.float64)
     nissl = normalize_intensity(nissl, annotation, threshold_scale_factor=1.0, copy=False)
     nissl = compensate_cell_overlap(nissl, annotation, gaussian_filter_stdv=-1.0, copy=False)
 
     group_ids = get_group_ids(region_map)
     region_masks = get_region_masks(group_ids, annotation)
     fix_purkinje_layer_intensity(region_map, annotation, region_masks, nissl)
+    non_zero_nissl = nissl > 0
     for group, mask in region_masks.items():
-        nissl[mask] = nissl[mask] * (cell_counts()[group] / np.sum(nissl[mask]))
+        mask = np.logical_and(non_zero_nissl, mask)
+        if mask.any():
+            nissl[mask] = nissl[mask] * (cell_counts()[group] / np.sum(nissl[mask]))
 
     return nissl / voxel_volume
```

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/excel_reader.py` & `atlas-densities-0.1.4/atlas_densities/densities/excel_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     """
     Add a source title a comment to every measurement in `dataframe`
 
     The input `dataframe` is modified in-place.
 
     In `dataframe`, the rows corresponding to the same article have no valid 'source title',
     'comment' nor 'specimen age' except the first one. This function makes sure every row is
-    set with approriate values in the aforementioned columns.
+    set with appropriate values in the aforementioned columns.
 
     Args:
         dataframe: DataFrame obtained when reading the worksheets 'GAD67 densities' or 'PV-SST-VIP'
             of gaba_papers.xlsx.
         bibliography: DataFrame of the form
                 source title                              specimen age
             6   'A Cell Atlas for the Mouse Brain'        11 week old
@@ -348,24 +348,22 @@
 def read_inhibitory_neuron_measurement_compilation(
     measurements_path: Union[str, "Path"]
 ) -> Tuple[pd.DataFrame, Set[str]]:
     """
     Read the neuron densities of the worksheet 'GAD67 densities' in gaba_papers.xlsx
 
     Args:
-        region_map: RegionMap object to navigate the brain regions hierarchy.
-            Assumed to be instantiated with AIBS 1.json.
         measurements_path: path to the file gaba_papers.xlsx
 
     Returns:
         a pd.DataFrame with the columns listed in the description at the top of
         this module.
     """
 
-    # Reading takes several seconds, possibly due to formulaes interpretation
+    # Reading takes several seconds, possibly due to formulas interpretation
     L.info("Loading excel worksheet ...")
     inhibitory_neurons_worksheet = pd.read_excel(
         str(measurements_path),
         sheet_name="GAD67 densities",
         header=None,
         names=[
             "brain_region",
@@ -431,16 +429,14 @@
 
 
 def read_pv_sst_vip_measurement_compilation(measurements_path: Union[str, "Path"]) -> pd.DataFrame:
     """
     Read the neuron densities of the worksheet 'PV-SST-VIP' in gaba_papers.xlsx
 
     Args:
-        region_map: RegionMap object to navigate the brain regions hierarchy.
-            Assumed to be instantiated with AIBS 1.json.
         measurements_path: path to the file gaba_papers.xlsx
 
     Returns:
         dataframe is a pd.DataFrame with the columns listed in the description at the top of
         this module.
     """
     pv_sst_vip_neurons_worksheet = pd.read_excel(
@@ -480,15 +476,15 @@
     Read the region list of the worksheet 'Full inhibexc regions' in gaba_papers.xlsx
 
     Args:
         measurements_path: path to the file gaba_papers.xlsx
 
     Returns:
         pd.DataFrame with two columns: 'brain_region' and 'cell_type'. A cell type value
-        is either 'ihibitory' or 'excitatory' and applies to every cell in the region.
+        is either 'inhibitory' or 'excitatory' and applies to every cell in the region.
     """
 
     homogenous_regions_worksheet = pd.read_excel(
         str(measurements_path),
         sheet_name="Fully inhibexc regions",
         names=["brain_region", "comment"],
         header=None,
```

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/excitatory_inhibitory_splitting.py` & `atlas-densities-0.1.4/atlas_densities/densities/excitatory_inhibitory_splitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
     assert (mapping.to_numpy() >= 0).all(), "Cannot have negative scaling factors"
 
     for layer, df in mapping.iterrows():
         L.info("Performing layer: %s", layer)
         idx = np.nonzero(np.isin(brain_regions.raw, layer_ids[layer]))
 
-        for mtype, scale in df.iteritems():
+        for mtype, scale in df.items():
             if scale == 0:
                 continue
 
             L.info("  Performing %s", mtype)
 
             raw = np.zeros_like(density.raw)
             raw[idx] = scale * density.raw[idx]
```

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/fitting.py` & `atlas-densities-0.1.4/atlas_densities/densities/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,16 @@
 def compute_average_intensity(
     intensity: FloatArray, volume_mask: BoolArray, slices: Optional[List[int]] = None
 ) -> float:
     """
     Compute the average of `intensity` within the volume defined by `volume_mask`.
 
     If `slices` is a non-empty list of slice indices along the x-axis, then the average is
-    restricted to the subvolume of `volume_mask` enclosed by these slices.
+    restricted to the subvolume of `volume_mask` enclosed by these slices. Slices indices outside
+    the `volume_mask` will be ignored.
 
     Args:
         intensity: a float array of shape (W, H, D) where W, H and D are integer dimensions.
         volume_mask: boolean mask of the same shape as `instensity` defining the volume on which
             the average intensity is computed.
         slices (optional): list of integer indices along the x-axis of `intensity`. Indices range in
             [0, W - 1] with W = `intensity.shape[0]`. Defaults to None, in which case the average is
@@ -192,15 +193,17 @@
         the returned value is 0.0.
     """
 
     if slices is None:
         restricted_mask = volume_mask
     else:
         restricted_mask = np.zeros_like(volume_mask)
-        restricted_mask[slices] = True
+        # remove slices indices outside the volume_mask
+        slices_ = [slice_ for slice_ in slices if 0 <= slice_ < volume_mask.shape[0]]
+        restricted_mask[slices_] = True
         restricted_mask = np.logical_and(restricted_mask, volume_mask)
 
     if np.any(restricted_mask):
         return np.mean(intensity[restricted_mask])
 
     return 0.0
```

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/glia_densities.py` & `atlas-densities-0.1.4/atlas_densities/densities/glia_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/inhibitory_neuron_densities_helper.py` & `atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_densities_helper.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/inhibitory_neuron_densities_optimization.py` & `atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_densities_optimization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/inhibitory_neuron_density.py` & `atlas-densities-0.1.4/atlas_densities/densities/inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/measurement_to_density.py` & `atlas-densities-0.1.4/atlas_densities/densities/measurement_to_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/mtype_densities_from_composition.py` & `atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_composition.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     """
     excitatory_mtype_composition = mtype_composition[
         mtype_composition["mtype"].isin(_excitatory_mtypes_from_taxonomy(mtype_taxonomy))
     ]
 
     layer_masks = get_layer_masks(annotation.raw, region_map, metadata)
 
-    for layer, layer_data in excitatory_mtype_composition.groupby(["layer"]):
+    for layer, layer_data in excitatory_mtype_composition.groupby("layer"):
 
         layer_sum = layer_data["density"].sum()
 
         for row in layer_data.itertuples():
 
             volumetric_density = np.zeros_like(annotation.raw, dtype=np.float32)
```

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/mtype_densities_from_map.py` & `atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_map.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/mtype_densities_from_profiles.py` & `atlas-densities-0.1.4/atlas_densities/densities/mtype_densities_from_profiles.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/refined_inhibitory_neuron_densities.py` & `atlas-densities-0.1.4/atlas_densities/densities/refined_inhibitory_neuron_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/atlas_densities/densities/utils.py` & `atlas-densities-0.1.4/atlas_densities/densities/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     threshold: float = 1e-7,
     max_iter: int = 45,
     copy: bool = True,
 ) -> FloatArray:
     """
     Find inside a box the closest point to a line with prescribed coordinate sum.
 
-    This function aims at solving the following (convex quadratic) optmization problem:
+    This function aims at solving the following (convex quadratic) optimization problem:
 
     Given a sum S >= 0.0, a line D in the non-negative orthant of the Euclidean N-dimensional
     space and a box B in this orthant (an N-dimensional vector with non-negative coordinates),
     find, if it exists, the point P in B which is the closest to D and whose coordinate sum is S.
 
     The point P exists if and only if the coordinate sum of B is not less than S.
     The proposed algorithm is iterative and starts with the end point of a direction vector of D.
@@ -172,34 +172,38 @@
 
     Note: The convergence to the optimal solution is obvious in 2D, but can already fail in 3D.
     At the moment, the function only returns a feasible point.
 
     Args:
         line_direction_vector: N-dimensional float vector with non-negative coordinates.
         upper_bounds: N-dimensional float vector with non-negative coordinates. Defines the
-            the box constraining the optimization process.
-        sum_constraints: non-negative float number. The coordinate sum constraints imposed on
+            box constraining the optimization process.
+        sum_constraint: non-negative float number. The coordinate sum constraints imposed on
             the point P we are looking for.
         threshold: non-negative float value. If the coordinate sum of the current point
             is below `threshold`, the function returns the current point.
         max_iter: maximum number of iterations.
-        copy: If True, the function makes a copy of the input `line_direction_vector`. Otherwise
+        copy: If True, the function makes a copy of the input `line_direction_vector`. Otherwise,
             `line_direction_vector` is modified in-place and holds the optimal value.
 
     Returns: N-dimensional float vector with non-negative coordinates. The solution point of the
-        optimization problem, if it exists, up to inacurracy due to threshold size or early
-        termination of the algorithm. Otherwise a point on the boundary of the box B defined by
+        optimization problem, if it exists, up to inaccuracy due to threshold size or early
+        termination of the algorithm. Otherwise, a point on the boundary of the box B defined by
         `upper_bounds`.
     """
     diff = float("inf")
     iter_ = 0
     point = line_direction_vector.copy() if copy else line_direction_vector
-    while diff > threshold and iter_ < max_iter:
-        point *= sum_constraint / np.sum(point)
+    scalable_voxels = point != 0
+    while diff > threshold and iter_ < max_iter and scalable_voxels.any():
+        point[scalable_voxels] *= (sum_constraint - np.sum(point[~scalable_voxels])) / np.sum(
+            point[scalable_voxels]
+        )
         point = np.min([point, upper_bounds], axis=0)
+        scalable_voxels = np.logical_and(point != 0, point < upper_bounds)
         diff = np.abs(np.sum(point) - sum_constraint)
         iter_ += 1
 
     return point
 
 
 def constrain_cell_counts_per_voxel(  # pylint: disable=too-many-arguments, too-many-branches
@@ -381,15 +385,15 @@
 
 def get_group_names(region_map: "RegionMap", cleanup_rest: bool = False) -> Dict[str, Set[str]]:
     """
     Get AIBS names for regions in several region groups of interest.
 
     Args:
         region_map: object to navigate the mouse brain regions hierarchy
-            (instantied from AIBS 1.json).
+            (instantiated from AIBS 1.json).
         cleanup_rest: (Optional) If True, the name of any ascendant region of the Cerebellum and
             Isocortex groups are removed from the names of the Rest group. This makes sure that
             the set of names of the Rest group is closed under taking descendants.
 
     Returns:
         A dictionary whose keys are region group names and whose values are
         sets of brain region names.
@@ -481,15 +485,16 @@
     region_ids = list(region_map.find(root, attr="name", with_descendants=True))
     region_ids.sort()
     descendant_id_sets = [
         region_map.find(id_, attr="id", with_descendants=True) for id_ in region_ids
     ]
     region_names = [region_map.get(id_, attr="name") for id_ in region_ids]
     data_frame = pd.DataFrame(
-        {"brain_region": region_names, "descendant_id_set": descendant_id_sets}, index=region_ids
+        {"brain_region": region_names, "descendant_id_set": descendant_id_sets},
+        index=region_ids,
     )
 
     return data_frame
 
 
 def compute_region_volumes(
     annotation: AnnotationT,
```

### Comparing `atlas-densities-0.1.3/atlas_densities/utils.py` & `atlas-densities-0.1.4/atlas_densities/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Generic Atlas files tools"""
 
-from typing import Dict, Tuple, Union
+from typing import Dict, Union
 
 import numpy as np
 import scipy.ndimage
 import scipy.signal
 from atlas_commons.typing import AnnotationT, BoolArray, NDArray, NumericArray
 from voxcell import RegionMap  # type: ignore
 
@@ -78,39 +78,14 @@
 
     """
     region = {"query": acronym, "attribute": "acronym", "with_descendants": True}
 
     return query_region_mask(region, annotation, region_map)
 
 
-def split_into_halves(
-    volume: NumericArray,
-    halfway_offset: int = 0,
-) -> Tuple[NumericArray, NumericArray]:
-    """
-    Split input 3D volume into two halves along the z-axis.
-
-    Args:
-        volume: 3D numeric array.
-            halfway_offset: Optional offset used for the
-            splitting along the z-axis.
-    Returns:
-        tuple(left_volume, right_volume), the two halves of the
-        input volume. Each has the same shape as `volume`.
-        Voxels are zeroed for the z-values above, respectively
-        below, the half of the z-dimension.
-    """
-    z_halfway = volume.shape[2] // 2 + halfway_offset
-    left_volume = volume.copy()
-    left_volume[..., z_halfway:] = 0
-    right_volume = volume.copy()
-    right_volume[..., :z_halfway] = 0
-    return left_volume, right_volume
-
-
 def is_obtuse_angle(vector_field_1: NumericArray, vector_field_2: NumericArray) -> BoolArray:
     """
     Returns a mask indicating which vector pairs form an obtuse angle.
 
     Arguments:
         vector_field_1: 3D vector field, i.e., numeric array of shape
             (M, N, ..., 3).
```

### Comparing `atlas-densities-0.1.3/atlas_densities.egg-info/PKG-INFO` & `atlas-densities-0.1.4/atlas_densities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlas-densities
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library containing command lines and tools to compute volumetric cell densities in the rodent brain
 Home-page: https://github.com/BlueBrain/atlas-densities
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/atlas-densities
 Description: .. image:: atlas-densities.jpg
```

### Comparing `atlas-densities-0.1.3/atlas_densities.egg-info/SOURCES.txt` & `atlas-densities-0.1.4/atlas_densities.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 atlas_densities/app/data/1.json
 atlas_densities/app/data/__init__.py
 atlas_densities/app/data/markers/README.rst
 atlas_densities/app/data/markers/combine_markers_ccfv2_config.yaml
 atlas_densities/app/data/markers/fit_average_densities_ccfv2_config.yaml
 atlas_densities/app/data/markers/realigned_slices_bbp.json
 atlas_densities/app/data/markers/realigned_slices_ccfv2.json
-atlas_densities/app/data/measurements/._std_cells.json
 atlas_densities/app/data/measurements/README.rst
 atlas_densities/app/data/measurements/gaba_papers.xlsx
 atlas_densities/app/data/measurements/homogenous_regions.csv
 atlas_densities/app/data/measurements/measurements.csv
 atlas_densities/app/data/measurements/mmc1.xlsx
 atlas_densities/app/data/measurements/mmc3.xlsx
 atlas_densities/app/data/measurements/non_density_measurements.csv
```

### Comparing `atlas-densities-0.1.3/doc/Makefile` & `atlas-densities-0.1.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/doc/source/bbpp82_628_linear_program.pdf` & `atlas-densities-0.1.4/doc/source/bbpp82_628_linear_program.pdf`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/doc/source/conf.py` & `atlas-densities-0.1.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/doc/source/index.rst` & `atlas-densities-0.1.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/setup.py` & `atlas-densities-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/1.json` & `atlas-densities-0.1.4/tests/1.json`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/app/test_cell_densities.py` & `atlas-densities-0.1.4/tests/app/test_cell_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/app/test_combination.py` & `atlas-densities-0.1.4/tests/app/test_combination.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/app/test_mtype_densities.py` & `atlas-densities-0.1.4/tests/app/test_mtype_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/app/test_refined_inhibitory_neuron_densities.py` & `atlas-densities-0.1.4/tests/app/test_refined_inhibitory_neuron_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/combination/test_annotations_combinator.py` & `atlas-densities-0.1.4/tests/combination/test_annotations_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/combination/test_markers_combinator.py` & `atlas-densities-0.1.4/tests/combination/test_markers_combinator.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/data/mtypes/mtype-taxonomy.tsv` & `atlas-densities-0.1.4/tests/densities/data/mtypes/mtype-taxonomy.tsv`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_cell_counts.py` & `atlas-densities-0.1.4/tests/densities/test_cell_counts.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_cell_density.py` & `atlas-densities-0.1.4/tests/densities/test_cell_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_excel_reader.py` & `atlas-densities-0.1.4/tests/densities/test_excel_reader.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_excitatory_inhibitory_splitting.py` & `atlas-densities-0.1.4/tests/densities/test_excitatory_inhibitory_splitting.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_fitting.py` & `atlas-densities-0.1.4/tests/densities/test_fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,18 @@
     assert actual == 0.1
 
     volume_mask = np.array([[[False, False], [True, True]], [[True, True], [False, False]]])
     actual = tested.compute_average_intensity(intensity, volume_mask, slices=[0])
     assert np.allclose(actual, 0.3 / 2.0)
     actual = tested.compute_average_intensity(intensity, volume_mask, slices=[1])
     assert np.allclose(actual, 0.1 / 2.0)
+    actual = tested.compute_average_intensity(intensity, volume_mask, slices=[-1, 1, 3])
+    assert np.allclose(actual, 0.1 / 2.0)
+    actual = tested.compute_average_intensity(intensity, volume_mask, slices=[-1, 3])
+    assert actual == 0
 
 
 def test_compute_average_intensities(hierarchy_info):
     annotation = np.array(
         [[[0, 976], [976, 936]], [[976, 936], [936, 936]]]  # 976 = Lobule II, 936 = "Declive (VI)""
     )
     marker_volumes = {
```

### Comparing `atlas-densities-0.1.3/tests/densities/test_glia_densities.py` & `atlas-densities-0.1.4/tests/densities/test_glia_densities.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_inhibitory_neuron_densities_helper.py` & `atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_densities_helper.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_inhibitory_neuron_density.py` & `atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_inhibitory_neuron_density_optimization.py` & `atlas-densities-0.1.4/tests/densities/test_inhibitory_neuron_density_optimization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_measurement_to_density.py` & `atlas-densities-0.1.4/tests/densities/test_measurement_to_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_mtype_densities_from_composition.py` & `atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_composition.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_mtype_densities_from_map.py` & `atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_map.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_mtype_densities_from_profiles.py` & `atlas-densities-0.1.4/tests/densities/test_mtype_densities_from_profiles.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_optimization_initialization.py` & `atlas-densities-0.1.4/tests/densities/test_optimization_initialization.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_refined_inhibitory_neuron_density.py` & `atlas-densities-0.1.4/tests/densities/test_refined_inhibitory_neuron_density.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/densities/test_utils.py` & `atlas-densities-0.1.4/tests/densities/test_utils.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/markers_config.yaml` & `atlas-densities-0.1.4/tests/markers_config.yaml`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/mocking_tools.py` & `atlas-densities-0.1.4/tests/mocking_tools.py`

 * *Files identical despite different names*

### Comparing `atlas-densities-0.1.3/tests/test_utils.py` & `atlas-densities-0.1.4/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,44 +71,14 @@
 
     # True RegionMap object
     region_map = RegionMap.load_json(str(Path(TEST_PATH, "1.json")))
     mask = tested.get_region_mask("Isocortex", annotation, region_map)
     npt.assert_array_equal(mask, expected)
 
 
-def test_split_into_halves():
-    volume = np.array(
-        [
-            [[0, 1, 2], [2, 3, 4]],
-            [[4, 5, 6], [7, 8, 9]],
-        ],
-        dtype=np.int64,
-    )
-    halves = tested.split_into_halves(volume)
-    npt.assert_array_equal(
-        halves[0],
-        np.array(
-            [
-                [[0, 0, 0], [2, 0, 0]],
-                [[4, 0, 0], [7, 0, 0]],
-            ],
-            dtype=np.int64,
-        ),
-    )
-    npt.assert_array_equal(
-        halves[1],
-        np.array(
-            [
-                [[0, 1, 2], [0, 3, 4]],
-                [[0, 5, 6], [0, 8, 9]],
-            ]
-        ),
-    )
-
-
 def test_is_obtuse_angle():
     vector_field_1 = np.array(
         [
             [
                 [[1.0, 0.0, -1.0], [10.3, 5.6, 9.0]],
                 [[0.0, 0.0, 0.0], [-1.0, -1.0, -1.0]],
             ],
```

### Comparing `atlas-densities-0.1.3/tox.ini` & `atlas-densities-0.1.4/tox.ini`

 * *Files identical despite different names*

