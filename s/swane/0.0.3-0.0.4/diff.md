# Comparing `tmp/swane-0.0.3.tar.gz` & `tmp/swane-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swane-0.0.3.tar", last modified: Tue Apr  4 03:40:44 2023, max compression
+gzip compressed data, was "swane-0.0.4.tar", last modified: Tue Apr 11 08:24:09 2023, max compression
```

## Comparing `swane-0.0.3.tar` & `swane-0.0.4.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.891767 swane-0.0.3/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1976 2023-03-29 17:07:54.000000 swane-0.0.3/LICENSE
--rw-rw-r--   0 mau       (1000) mau       (1000)      184 2023-03-29 17:07:54.000000 swane-0.0.3/MANIFEST.in
--rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-04 03:40:44.891767 swane-0.0.3/PKG-INFO
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.3/README.md
--rw-rw-r--   0 mau       (1000) mau       (1000)       38 2023-04-04 03:40:44.891767 swane-0.0.3/setup.cfg
--rw-rw-r--   0 mau       (1000) mau       (1000)     1202 2023-03-29 19:46:27.000000 swane-0.0.3/setup.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.875767 swane-0.0.3/swane/
--rw-rw-r--   0 mau       (1000) mau       (1000)       50 2023-03-31 09:42:52.000000 swane-0.0.3/swane/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1827 2023-03-29 17:07:54.000000 swane-0.0.3/swane/__main__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.879767 swane-0.0.3/swane/nipype_pipeline/
--rw-rw-r--   0 mau       (1000) mau       (1000)    18398 2023-03-30 15:50:36.000000 swane-0.0.3/swane/nipype_pipeline/MainWorkflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.879767 swane-0.0.3/swane/nipype_pipeline/engine/
--rw-rw-r--   0 mau       (1000) mau       (1000)     7531 2023-03-29 19:44:28.000000 swane-0.0.3/swane/nipype_pipeline/engine/CustomWorkflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)       85 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/engine/NodeListEntry.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/engine/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.883767 swane-0.0.3/swane/nipype_pipeline/nodes/
--rw-rw-r--   0 mau       (1000) mau       (1000)     2502 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/AsymmetryIndex.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2183 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1198 2023-04-04 03:05:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/CustomDcm2niix.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      414 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/CustomDilateImage.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      521 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/CustomLabel2Vol.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      798 2023-03-31 12:43:31.000000 swane-0.0.3/swane/nipype_pipeline/nodes/CustomProbTrackX2.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2345 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/CustomSliceTimer.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2637 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/DOmapOutliersMask.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2388 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/DeleteVolumes.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4446 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/FMRIGenSpec.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2474 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/ForceOrient.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      306 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/FslCluster.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1578 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/FslNVols.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1565 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/GetNiftiTR.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1617 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/MergeTargets.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1832 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/Orient.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1340 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/RandomSeedGenerator.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4257 2023-04-01 08:02:25.000000 swane-0.0.3/swane/nipype_pipeline/nodes/SegmentHA.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3201 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/SumMultiTracks.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2996 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/ThrROI.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2320 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/VenousCheck.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2615 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/Zscore.py
--rw-rw-r--   0 mau       (1000) mau       (1000)       25 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      179 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/nodes/utils.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.887767 swane-0.0.3/swane/nipype_pipeline/workflows/
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.3/swane/nipype_pipeline/workflows/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    13690 2023-03-31 12:25:20.000000 swane-0.0.3/swane/nipype_pipeline/workflows/domap_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     7922 2023-04-04 03:17:58.000000 swane-0.0.3/swane/nipype_pipeline/workflows/dti_preproc_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     7690 2023-04-01 08:02:25.000000 swane-0.0.3/swane/nipype_pipeline/workflows/freesurfer_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    10956 2023-04-04 03:17:58.000000 swane-0.0.3/swane/nipype_pipeline/workflows/func_map_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3504 2023-04-02 08:01:53.000000 swane-0.0.3/swane/nipype_pipeline/workflows/linear_reg_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3142 2023-03-29 20:08:41.000000 swane-0.0.3/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2180 2023-04-02 07:46:38.000000 swane-0.0.3/swane/nipype_pipeline/workflows/ref_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    19603 2023-04-02 08:03:23.000000 swane-0.0.3/swane/nipype_pipeline/workflows/task_fMRI_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    13745 2023-04-01 08:02:25.000000 swane-0.0.3/swane/nipype_pipeline/workflows/tractography_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     6335 2023-04-02 08:03:52.000000 swane-0.0.3/swane/nipype_pipeline/workflows/venous_workflow.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.887767 swane-0.0.3/swane/slicer/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1857 2023-03-29 17:07:54.000000 swane-0.0.3/swane/slicer/SlicerCheckWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1256 2023-03-29 17:07:54.000000 swane-0.0.3/swane/slicer/SlicerExportWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.3/swane/slicer/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      159 2023-03-29 17:07:54.000000 swane-0.0.3/swane/slicer/slicer_script_freesurfer_module_check.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     8841 2023-04-01 08:02:25.000000 swane-0.0.3/swane/slicer/slicer_script_result.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    12030 2023-03-31 12:17:40.000000 swane-0.0.3/swane/strings.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.891767 swane-0.0.3/swane/ui/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1378 2023-03-31 12:13:49.000000 swane-0.0.3/swane/ui/CustomTreeWidgetItem.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    20221 2023-03-29 17:07:54.000000 swane-0.0.3/swane/ui/MainWindow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      844 2023-03-29 17:07:54.000000 swane-0.0.3/swane/ui/PersistentProgressDialog.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    19160 2023-03-29 20:42:46.000000 swane-0.0.3/swane/ui/PreferencesWindow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    33668 2023-04-04 03:00:01.000000 swane-0.0.3/swane/ui/PtTab.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1001 2023-03-29 17:07:54.000000 swane-0.0.3/swane/ui/VerticalScrollArea.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.3/swane/ui/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.891767 swane-0.0.3/swane/ui/workers/
--rw-rw-r--   0 mau       (1000) mau       (1000)     4152 2023-03-29 17:07:54.000000 swane-0.0.3/swane/ui/workers/DicomSearchWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      725 2023-03-29 17:07:54.000000 swane-0.0.3/swane/ui/workers/WorkflowGeneratorWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      631 2023-03-29 17:07:54.000000 swane-0.0.3/swane/ui/workers/WorkflowMonitorWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3670 2023-04-04 02:58:13.000000 swane-0.0.3/swane/ui/workers/WorkflowProcess.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.3/swane/ui/workers/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.891767 swane-0.0.3/swane/utils/
--rw-rw-r--   0 mau       (1000) mau       (1000)     9139 2023-03-30 16:32:11.000000 swane-0.0.3/swane/utils/ConfigManager.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2514 2023-03-30 17:00:25.000000 swane-0.0.3/swane/utils/DataInput.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     5568 2023-03-29 17:07:54.000000 swane-0.0.3/swane/utils/PreferenceEntry.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.3/swane/utils/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1749 2023-03-29 17:07:54.000000 swane-0.0.3/swane/utils/check_dependency.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3267 2023-03-29 17:07:54.000000 swane-0.0.3/swane/utils/fsl_conflict_handler.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-04 03:40:44.879767 swane-0.0.3/swane.egg-info/
--rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-04 03:40:44.000000 swane-0.0.3/swane.egg-info/PKG-INFO
--rw-rw-r--   0 mau       (1000) mau       (1000)     2850 2023-04-04 03:40:44.000000 swane-0.0.3/swane.egg-info/SOURCES.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)        1 2023-04-04 03:40:44.000000 swane-0.0.3/swane.egg-info/dependency_links.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)       42 2023-04-04 03:40:44.000000 swane-0.0.3/swane.egg-info/entry_points.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)      109 2023-04-04 03:40:44.000000 swane-0.0.3/swane.egg-info/requires.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)        6 2023-04-04 03:40:44.000000 swane-0.0.3/swane.egg-info/top_level.txt
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.752565 swane-0.0.4/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1976 2023-03-29 17:07:54.000000 swane-0.0.4/LICENSE
+-rw-rw-r--   0 mau       (1000) mau       (1000)      184 2023-03-29 17:07:54.000000 swane-0.0.4/MANIFEST.in
+-rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-11 08:24:09.752565 swane-0.0.4/PKG-INFO
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/README.md
+-rw-rw-r--   0 mau       (1000) mau       (1000)       38 2023-04-11 08:24:09.752565 swane-0.0.4/setup.cfg
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1202 2023-04-11 08:22:48.000000 swane-0.0.4/setup.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.744566 swane-0.0.4/swane/
+-rw-rw-r--   0 mau       (1000) mau       (1000)       50 2023-04-05 07:58:56.000000 swane-0.0.4/swane/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1827 2023-03-29 17:07:54.000000 swane-0.0.4/swane/__main__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.744566 swane-0.0.4/swane/nipype_pipeline/
+-rw-rw-r--   0 mau       (1000) mau       (1000)    18398 2023-03-30 15:50:36.000000 swane-0.0.4/swane/nipype_pipeline/MainWorkflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/nipype_pipeline/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.744566 swane-0.0.4/swane/nipype_pipeline/engine/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7906 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/engine/CustomWorkflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      405 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/engine/NodeListEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/nipype_pipeline/engine/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/nipype_pipeline/nodes/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2537 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/AsymmetryIndex.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2263 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1245 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomDcm2niix.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      489 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomDilateImage.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      661 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomLabel2Vol.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      923 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomProbTrackX2.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2356 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomSliceTimer.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2737 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/DOmapOutliersMask.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2437 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/DeleteVolumes.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4520 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/FMRIGenSpec.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2506 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/ForceOrient.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      458 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/FslCluster.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1600 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/FslNVols.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1601 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/GetNiftiTR.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1650 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/MergeTargets.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1849 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/Orient.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1400 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/RandomSeedGenerator.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2741 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/SegmentHA.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3247 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/SumMultiTracks.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3025 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/ThrROI.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2378 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/VenousCheck.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2703 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/Zscore.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)       25 2023-03-29 17:07:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      178 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/utils.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/nipype_pipeline/workflows/
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/nipype_pipeline/workflows/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    13690 2023-03-31 12:25:20.000000 swane-0.0.4/swane/nipype_pipeline/workflows/domap_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7922 2023-04-04 03:17:58.000000 swane-0.0.4/swane/nipype_pipeline/workflows/dti_preproc_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7690 2023-04-01 08:02:25.000000 swane-0.0.4/swane/nipype_pipeline/workflows/freesurfer_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    10956 2023-04-04 03:17:58.000000 swane-0.0.4/swane/nipype_pipeline/workflows/func_map_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3504 2023-04-02 08:01:53.000000 swane-0.0.4/swane/nipype_pipeline/workflows/linear_reg_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3142 2023-03-29 20:08:41.000000 swane-0.0.4/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2180 2023-04-02 07:46:38.000000 swane-0.0.4/swane/nipype_pipeline/workflows/ref_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19603 2023-04-02 08:03:23.000000 swane-0.0.4/swane/nipype_pipeline/workflows/task_fMRI_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    13745 2023-04-01 08:02:25.000000 swane-0.0.4/swane/nipype_pipeline/workflows/tractography_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     6335 2023-04-02 08:03:52.000000 swane-0.0.4/swane/nipype_pipeline/workflows/venous_workflow.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/slicer/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1857 2023-03-29 17:07:54.000000 swane-0.0.4/swane/slicer/SlicerCheckWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1256 2023-03-29 17:07:54.000000 swane-0.0.4/swane/slicer/SlicerExportWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/slicer/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      159 2023-03-29 17:07:54.000000 swane-0.0.4/swane/slicer/slicer_script_freesurfer_module_check.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     8841 2023-04-01 08:02:25.000000 swane-0.0.4/swane/slicer/slicer_script_result.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    12032 2023-04-05 09:49:56.000000 swane-0.0.4/swane/strings.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/ui/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1378 2023-03-31 12:13:49.000000 swane-0.0.4/swane/ui/CustomTreeWidgetItem.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    18206 2023-04-05 07:58:18.000000 swane-0.0.4/swane/ui/MainWindow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      844 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/PersistentProgressDialog.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19160 2023-03-29 20:42:46.000000 swane-0.0.4/swane/ui/PreferencesWindow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    33668 2023-04-04 03:00:01.000000 swane-0.0.4/swane/ui/PtTab.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1001 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/VerticalScrollArea.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/ui/workers/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4152 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/workers/DicomSearchWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      725 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/workers/WorkflowGeneratorWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      631 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/workers/WorkflowMonitorWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3670 2023-04-04 02:58:13.000000 swane-0.0.4/swane/ui/workers/WorkflowProcess.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/workers/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.752565 swane-0.0.4/swane/utils/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     9139 2023-03-30 16:32:11.000000 swane-0.0.4/swane/utils/ConfigManager.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2514 2023-03-30 17:00:25.000000 swane-0.0.4/swane/utils/DataInput.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     5568 2023-03-29 17:07:54.000000 swane-0.0.4/swane/utils/PreferenceEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/utils/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1749 2023-03-29 17:07:54.000000 swane-0.0.4/swane/utils/check_dependency.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3267 2023-03-29 17:07:54.000000 swane-0.0.4/swane/utils/fsl_conflict_handler.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4385 2023-04-11 10:17:10.000000 swane-0.0.4/swane/utils/shortcut_manager.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.744566 swane-0.0.4/swane.egg-info/
+-rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/PKG-INFO
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2882 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/SOURCES.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)        1 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/dependency_links.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)       42 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/entry_points.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)      109 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/requires.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)        6 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/top_level.txt
```

### Comparing `swane-0.0.3/LICENSE` & `swane-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/setup.py` & `swane-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           "networkx<3",
           "nipype",
           "Pyside6",
           "pydicom",
           "configparser",
           "psutil",
           "pyshortcuts",
-          "swane_supplement>=0.1.1",
+          "swane_supplement>=0.1.2",
           "matplotlib",
           "nibabel"
       ],
       python_requires=">=3.7",
       entry_points={
           'gui_scripts': [
               "swane = swane.__main__:main"
```

### Comparing `swane-0.0.3/swane/__main__.py` & `swane-0.0.4/swane/__main__.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/MainWorkflow.py` & `swane-0.0.4/swane/nipype_pipeline/MainWorkflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/engine/CustomWorkflow.py` & `swane-0.0.4/swane/nipype_pipeline/engine/CustomWorkflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
 from nipype.pipeline.engine import Workflow
 from nipype import Node, logging
 from nipype.interfaces.utility import IdentityInterface
 from nipype.interfaces.io import DataSink
-from nipype.pipeline.engine.utils import get_print_name
 from swane.nipype_pipeline.engine.NodeListEntry import NodeListEntry
 from swane import strings
 
 logger = logging.getLogger("nipype.workflow")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.pipeline.engine.Workflow)  -*-
 class CustomWorkflow(Workflow):
+    """
+    Custom implementation of Workflow class with utility funcs.
 
+    """
+    
     @staticmethod
     def format_node_name(node):
+        """
+        Returns the explicit name of a Node.
+
+        """
+        
         default_node_name = None
         if hasattr(node, "interface") and type(node.interface).__name__ in strings.node_names:
             default_node_name = strings.node_names[type(node.interface).__name__]
         if hasattr(node, "long_name"):
             formatted_name = node.long_name
             if "%s" in node.long_name and default_node_name is not None:
                 formatted_name = node.long_name % default_node_name
@@ -28,30 +36,38 @@
         else:
             formatted_name = node.name
 
         formatted_name = formatted_name[0].upper() + formatted_name[1:]
         return formatted_name
 
     def get_node_array(self):
-        """List names of all nodes in a workflow"""
+        """
+        Returns a List of NodeListEntry objects for the Nodes in a Workflow.
+        
+        """
+        
         from networkx import topological_sort
 
         outlist = {}
         for node in topological_sort(self._graph):
             if hasattr(node, "interface") and isinstance(node.interface, IdentityInterface):
                 continue
 
             outlist[node.name] = NodeListEntry()
             outlist[node.name].long_name = self.format_node_name(node)
             if isinstance(node, Workflow):
                 outlist[node.name].node_list = node.get_node_array()
         return outlist
 
     def sink_result(self, save_path, result_node, result_name, sub_folder, regexp_substitutions=None):
-
+        """
+        Creates a sink_result Node to save the output files of a Workflow.
+        
+        """
+        
         if isinstance(result_node, str):
             result_node = self.get_node(result_node)
 
         data_sink = Node(DataSink(), name='SaveResults_' + result_node.name + "_" + result_name.replace(".", "_"))
         data_sink.long_name = "%s: " + result_name
         data_sink.inputs.base_directory = save_path
 
@@ -59,15 +75,19 @@
             data_sink.inputs.regexp_substitutions = regexp_substitutions
 
         self.connect(result_node, result_name, data_sink, sub_folder)
 
     def _get_dot(
             self, prefix=None, hierarchy=None, colored=False, simple_form=True, level=0
     ):
-        """Create a dot file with connection info"""
+        """
+        Custom implementation of _get_dot Nipype func to support the long_name Node attribute.
+        
+        """
+        
         import networkx as nx
 
         if prefix is None:
             prefix = "  "
         if hierarchy is None:
             hierarchy = []
         colorset = [
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/AsymmetryIndex.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/AsymmetryIndex.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 
 from os.path import abspath
 import os
 
 from nipype.interfaces.base import (BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File, isdefined)
 
 
-# NODO PER IL CALCOLO GENERICO DI UN ASIMMERY INDEX DATI I DUE FILE INVERTITI
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class AsymmetryIndexInputSpec(BaseInterfaceInputSpec):
+    
     in_file = File(exists=True, mandatory=True, desc='the input image')
     swapped_file = File(exists=True, mandatory=True, desc='the swapped input image')
     out_file = File(desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class AsymmetryIndexOutputSpec(TraitedSpec):
     out_file = File(desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class AsymmetryIndex(BaseInterface):
+    """
+    Generate Asymmetry Index Map from an image and its RL swapped as subtraction/sum.
+
+    """
+    
     input_spec = AsymmetryIndexInputSpec
     output_spec = AsymmetryIndexOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
 
         add = BinaryMaths()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/CustomDcm2niix.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/CustomDcm2niix.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
 from nipype.interfaces.dcm2nii import Dcm2niix, Dcm2niixInputSpec
 import os
 from nipype.interfaces.base import traits
 
 
-# REIMPLEMENTAZIONE DI DCM2NIIX PER RINOMINARE I FILE CROPPATI
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.dcm2nii.Dcm2niixInputSpec)  -*-
 class CustomDcm2niixInputSpec(Dcm2niixInputSpec):
     merge_imgs = traits.Enum(
         2,
         1,
         0,
         argstr="-m %d",
         usedefault=True)
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.dcm2nii.Dcm2niix)  -*-
 class CustomDcm2niix(Dcm2niix):
+    """
+    Custom implementation of Dcm2niix Nipype Node to support crop and merge parameters.
+
+    """
+    
     input_spec = CustomDcm2niixInputSpec
 
     def _run_interface(self, runtime):
         self.inputs.args = "-w 1"
         runtime = super(CustomDcm2niix, self)._run_interface(runtime)
         if self.inputs.crop is True and len(self.output_files) > 0 and os.path.exists(self.output_files[0].replace(".nii.gz", "_Crop_1.nii.gz")):
             os.remove(self.output_files[0])
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/CustomProbTrackX2.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/CustomProbTrackX2.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,8 +11,13 @@
     sample_random_points = traits.Float(
         argstr="--sampvox=%f", desc="sample random points within seed voxels"
     )
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.fsl.ProbTrackX2)  -*-
 class CustomProbTrackX2(ProbTrackX2):
+    """
+    Custom implementation of ProbTrackX2 Nipype Node to support --rseed as Int and --sampvox as Float.
+
+    """
+    
     input_spec = CustomProbTrackX2InputSpec
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/CustomSliceTimer.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/CustomSliceTimer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from nipype.interfaces.fsl import SliceTimer
 from nipype import Node
 from os.path import abspath
 import os
 from nipype.interfaces.base import (traits, TraitedSpec, BaseInterface, BaseInterfaceInputSpec, File)
 
 
-# APPLICA LA SLICE TIMING CORRECTION SE RICHIESTO
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class CustomSliceTimerInputSpec(BaseInterfaceInputSpec):
     in_file = File(exists=True, mandatory=True, desc='the input image')
     time_repetition = traits.Float(mandatory=True)
     slice_timing = traits.Enum(
         0,  # None
         1,  # Regular up
@@ -24,14 +23,19 @@
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class CustomSliceTimerOutputSpec(TraitedSpec):
     slice_time_corrected_file = File(desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class CustomSliceTimer(BaseInterface):
+    """
+    Applies a slice timing correction.
+
+    """
+    
     input_spec = CustomSliceTimerInputSpec
     output_spec = CustomSliceTimerOutputSpec
 
     def _run_interface(self, runtime):
         out_file = self._gen_outfilename()
         if self.inputs.slice_timing == 0:
             shutil.copy(self.inputs.in_file, out_file)
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/DOmapOutliersMask.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/DOmapOutliersMask.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class DOmapOutliersMaskOutputSpec(TraitedSpec):
     out_file = File(exists=True, desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class DOmapOutliersMask(BaseInterface):
+    """
+    Creates a mask that can be used to remove the outliers in DOmap workflow.
+
+    """
+    
     input_spec = DOmapOutliersMaskInputSpec
     output_spec = DOmapOutliersMaskOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
 
         mean = ImageStats()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/DeleteVolumes.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/DeleteVolumes.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from nipype.interfaces.fsl import ExtractROI
 from nipype import Node
 from os.path import abspath
 import os
 from nipype.interfaces.base import (traits, TraitedSpec, BaseInterface, BaseInterfaceInputSpec, File)
 
 
-# APPLICA LA SLICE TIMING CORRECTION SE RICHIESTO
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class DeleteVolumesInputSpec(BaseInterfaceInputSpec):
     in_file = File(exists=True, mandatory=True, desc='the input image')
     nvols = traits.Int(mandatory=True, desc='original file volumes')
     del_start_vols = traits.Int(mandatory=True, desc='volumes to delete from start')
     del_end_vols = traits.Int(mandatory=True, desc='volumes to delete from end')
 
@@ -21,14 +20,19 @@
 class DeleteVolumesOutputSpec(TraitedSpec):
     out_file = File(desc='the output image')
     nvols = traits.Int(desc='new number of volumes')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class DeleteVolumes(BaseInterface):
+    """
+    Removes specified num. of volumes from start and end of a 4d NIFTI file.
+
+    """
+    
     input_spec = DeleteVolumesInputSpec
     output_spec = DeleteVolumesOutputSpec
 
     def _run_interface(self, runtime):
         out_file = self._gen_outfilename()
         if self.inputs.del_start_vols == 0 and self.inputs.del_end_vols == 0:
             shutil.copy(self.inputs.in_file, out_file)
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/FMRIGenSpec.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/FMRIGenSpec.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     task_a_name = traits.String(desc="Task name")
     task_b_name = traits.String(desc="Task name")
     contrasts = traits.List(desc="T contrast array")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class FMRIGenSpec(BaseInterface):
+    """
+    Formats the fMRI parameters for FSL feat nodes.
+
+    """
+    
     input_spec = FMRIGenSpecInputSpec
     output_spec = FMRIGenSpecOutputSpec
 
     def _run_interface(self, runtime):
 
         if isdefined(self.inputs.hpcutoff):
             self.hpcutoff = self.inputs.hpcutoff
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/ForceOrient.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/ForceOrient.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 from nipype.interfaces.fsl import SwapDimensions
 from os.path import abspath
 import os
 from nipype.interfaces.base import (BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File, isdefined)
 from swane.nipype_pipeline.nodes.Orient import Orient
 
 
-# QUESTO NODO CONVERTE LE IMMAGINI IN RADIOLOGICAL E "RL","PA","IS"
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class ForceOrientInputSpec(BaseInterfaceInputSpec):
     in_file = File(exists=True, mandatory=True, desc='the input image')
     out_file = File(desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class ForceOrientOutputSpec(TraitedSpec):
     out_file = File(desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class ForceOrient(BaseInterface):
+    """
+    Converts an image in radiological convention and in RL PA IS orientation.
+
+    """
+    
     input_spec = ForceOrientInputSpec
     output_spec = ForceOrientOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
         shutil.copy(self.inputs.in_file, self.inputs.out_file)
         get_orient = Orient(in_file=self.inputs.out_file)
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/FslNVols.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/FslNVols.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
 from nipype.interfaces.fsl.base import FSLCommand, FSLCommandInputSpec
 from nipype.interfaces.base import (traits, TraitedSpec, File, isdefined)
 
 
-# QUESTO NODO LEGGE IL NUMERO DI VOLUMI DI UN NIFTI
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.fsl.base.FSLCommandInputSpec)  -*-
 class FslNVolsInputSpec(FSLCommandInputSpec):
     in_file = File(exists=True, mandatory=True, argstr="%s", position="1", desc='the input image')
     force_value = traits.Int(mandatory=False, desc='value forced by user')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class FslNVolsOutputSpec(TraitedSpec):
     nvols = traits.Int(desc="Number of EPI runs")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.FSLCommand)  -*-
 class FslNVols(FSLCommand):
+    """
+    Reads the num. of volumes from a 4d NIFTI file.
+
+    """
+    
     _cmd = 'fslnvols'
     input_spec = FslNVolsInputSpec
     output_spec = FslNVolsOutputSpec
 
     def aggregate_outputs(self, runtime=None, needed_outputs=None):
         outputs = self._outputs()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/GetNiftiTR.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/GetNiftiTR.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
 from nipype.interfaces.fsl.base import FSLCommand, FSLCommandInputSpec
 from nipype.interfaces.base import (traits, TraitedSpec, File, isdefined)
 
 
-# QUESTO NODO LEGGE IL TR DI UN NIFTI
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.fsl.base.FSLCommandInputSpec)  -*-
 class GetNiftiTRInputSpec(FSLCommandInputSpec):
     in_file = File(exists=True, mandatory=True, argstr="%s pixdim4", position="1", desc='the input image')
     force_value = traits.Float(mandatory=False, desc='value forced by user')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class GetNiftiTROutputSpec(TraitedSpec):
     TR = traits.Float(desc="Repetition Time")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.fsl.base.FSLCommand)  -*-
 class GetNiftiTR(FSLCommand):
+    """
+    Reads the time of repetition from a NIFTI file.
+
+    """
+    
     _cmd = 'fslval'
     input_spec = GetNiftiTRInputSpec
     output_spec = GetNiftiTROutputSpec
 
     def aggregate_outputs(self, runtime=None, needed_outputs=None):
         outputs = self._outputs()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/MergeTargets.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/MergeTargets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
 from os.path import abspath
 from nipype.interfaces.base import (BaseInterface, BaseInterfaceInputSpec, TraitedSpec, InputMultiPath, File, isdefined)
 
 
-# SOMMA UNA LISTA DI VOLUMI
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class MergeTargetsInputSpec(BaseInterfaceInputSpec):
     target_files = InputMultiPath(File(exists=True), mandatory=True, desc="list of path file to merge in txt")
     out_file = File(desc='the output file name')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class MergeTargetsOutputSpec(TraitedSpec):
     out_file = File(exists=True, desc='the output txt file')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class MergeTargets(BaseInterface):
+    """
+    Creates a .txt file from an array.
+
+    """
+    
     input_spec = MergeTargetsInputSpec
     output_spec = MergeTargetsOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
 
         lines = "\n".join(self.inputs.target_files)
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/Orient.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/Orient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
 from nipype.interfaces.fsl.base import FSLCommand, FSLCommandInputSpec
 from nipype.interfaces.base import (traits, TraitedSpec, File, isdefined)
 
 
-# QUESTO NODO RESTITUISCE L'ORIENTAMENTO DELLE IMMAGINI (NEUROLOGICAL/radiological)
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.fsl.base.FSLCommandInputSpec)  -*-
 class OrientInputSpec(FSLCommandInputSpec):
     in_file = File(exists=True, mandatory=True, argstr="%s", position="2", desc="input image")
     _options_xor = ['get_orient', "swap_orient"]
     get_orient = traits.Bool(argstr="-getorient", position="1", xor=_options_xor,
                              desc="gets FSL left-right orientation")
     swap_orient = traits.Bool(argstr="-swaporient", position="1", xor=_options_xor,
@@ -19,14 +18,19 @@
 class OrientOutputSpec(TraitedSpec):
     out_file = File(exists=True, desc="image with modified orientation")
     orient = traits.Str(desc="FSL left-right orientation")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.fsl.base.FSLCommand)  -*-
 class Orient(FSLCommand):
+    """
+    Returns the image orientation as neurological or radiological conventions.
+
+    """
+    
     _cmd = 'fslorient'
     input_spec = OrientInputSpec
     output_spec = OrientOutputSpec
 
     def aggregate_outputs(self, runtime=None, needed_outputs=None):
 
         outputs = self._outputs()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/RandomSeedGenerator.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/RandomSeedGenerator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- DISCLAIMER: this file contains code derived from Nipype (https://github.com/nipy/nipype/blob/master/LICENSE)  -*-
 
 from nipype.interfaces.base import (traits, BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File)
 
 
-# QUESO NODO GENERA UNA LISTA DI SEED RANDOM
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class RandomSeedGeneratorInputSpec(BaseInterfaceInputSpec):
     seeds_n = traits.Int(mandatory=True, desc="The number of needed seeds")
     mask = File(mandatory=True, exists=True, desc="Just for depend")
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class RandomSeedGeneratorOutputSpec(TraitedSpec):
     seeds = traits.List(desc='the list of seeds')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class RandomSeedGenerator(BaseInterface):
+    """
+    Generates a list of random integers. Used to obtains a series of random seeds.
+
+    """
+    
     input_spec = RandomSeedGeneratorInputSpec
     output_spec = RandomSeedGeneratorOutputSpec
     seed_list = []
 
     def _run_interface(self, runtime):
         from random import randrange
         for x in range(self.inputs.seeds_n):
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/SumMultiTracks.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/SumMultiTracks.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from os.path import abspath
 import os
 
 from nipype.interfaces.fsl import BinaryMaths
 from nipype.interfaces.base import (BaseInterface, BaseInterfaceInputSpec, TraitedSpec, InputMultiPath, File, isdefined)
 
 
-# SOMMA UNA LISTA DI VOLUMI
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class SumMultiTracksInputSpec(BaseInterfaceInputSpec):
     path_files = InputMultiPath(File(exists=True), mandatory=True, desc="list of path file to sum togheter")
     waytotal_files = InputMultiPath(File(exists=True), mandatory=True, desc="list of waytotal files to sum togheter")
     out_file = File(desc='the output image')
 
 
@@ -19,14 +18,19 @@
 class SumMultiTracksOutputSpec(TraitedSpec):
     out_file = File(exists=True, desc='the output image')
     waytotal_sum = File(exists=True, desc='the output waytotal file')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class SumMultiTracks(BaseInterface):
+    """
+    Merges results from multiple tractography runs.
+
+    """
+    
     input_spec = SumMultiTracksInputSpec
     output_spec = SumMultiTracksOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
         waytotal_sum_file = self._gen_waytotal_outfilename()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/ThrROI.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/ThrROI.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from nipype.interfaces.fsl import (UnaryMaths, Threshold)
 from os.path import abspath
 import os
 from nipype.interfaces.base import (traits, BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File, isdefined)
 
 
-# NODO PER ESTRARRE UNA ROI DA UNA SEGMENTAZIONE CON UN DATO VALORE
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class ThrROIInputSpec(BaseInterfaceInputSpec):
     in_file = File(exists=True, mandatory=True, desc='the input image')
     seg_val_min = traits.Float(mandatory=True, desc='the min value of interested segmentation')
     seg_val_max = traits.Float(mandatory=True, desc='the max value of interested segmentation')
     out_file = File(desc='the output image')
 
@@ -18,14 +17,19 @@
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class ThrROIOutputSpec(TraitedSpec):
     out_file = File(desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class ThrROI(BaseInterface):
+    """
+    Extracts a binary ROI from a segmentation using a min and a max value.
+
+    """
+    
     input_spec = ThrROIInputSpec
     output_spec = ThrROIOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
 
         below = Threshold()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/VenousCheck.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/VenousCheck.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import shutil
 from nipype.interfaces.base import InputMultiObject
 from nipype.interfaces.fsl import ImageStats
 from os.path import abspath
 from nipype.interfaces.base import (BaseInterface, BaseInterfaceInputSpec, TraitedSpec, File)
 
 
-# QUESO NODO DISCRIMINA LA FASE VENOSA DA QUELLA MORFOLOGICA DELLA PHASE CONTRAST
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterfaceInputSpec)  -*-
 class VenousCheckInputSpec(BaseInterfaceInputSpec):
     in_files = InputMultiObject(File(exists=True), desc="List of splitted file")
     out_file_veins = File(desc='the output venous image')
     out_file_anat = File(desc='the output anatomic image')
 
 
@@ -19,14 +18,19 @@
 class VenousCheckOutputSpec(TraitedSpec):
     out_file_veins = File(desc='the output venous image')
     out_file_anat = File(desc='the output anatomic image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class VenousCheck(BaseInterface):
+    """
+    Recognises the venous phase from the anatomic image of a phase contrast sequence based on its standard deviation.
+
+    """
+    
     input_spec = VenousCheckInputSpec
     output_spec = VenousCheckOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file_veins = abspath("veins.nii.gz")
         self.inputs.out_file_anat = abspath("veins_anat.nii.gz")
         s0 = ImageStats()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/nodes/Zscore.py` & `swane-0.0.4/swane/nipype_pipeline/nodes/Zscore.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.TraitedSpec)  -*-
 class ZscoreOutputSpec(TraitedSpec):
     out_file = File(exists=True, desc='the output image')
 
 
 # -*- DISCLAIMER: this class extends a Nipype class (nipype.interfaces.base.BaseInterface)  -*-
 class Zscore(BaseInterface):
+    """
+    Calculates the z-score index of an image compared with a ROI.
+
+    """
+    
     input_spec = ZscoreInputSpec
     output_spec = ZscoreOutputSpec
 
     def _run_interface(self, runtime):
         self.inputs.out_file = self._gen_outfilename()
 
         mask = ApplyMask()
```

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/domap_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/domap_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/dti_preproc_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/dti_preproc_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/freesurfer_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/freesurfer_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/func_map_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/func_map_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/linear_reg_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/linear_reg_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/ref_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/ref_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/task_fMRI_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/task_fMRI_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/tractography_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/tractography_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/nipype_pipeline/workflows/venous_workflow.py` & `swane-0.0.4/swane/nipype_pipeline/workflows/venous_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/slicer/SlicerCheckWorker.py` & `swane-0.0.4/swane/slicer/SlicerCheckWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/slicer/SlicerExportWorker.py` & `swane-0.0.4/swane/slicer/SlicerExportWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/slicer/slicer_script_result.py` & `swane-0.0.4/swane/slicer/slicer_script_result.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/strings.py` & `swane-0.0.4/swane/strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 mainwindow_shortcut_created = "Shortcut created!"
 mainwindow_shortcut_removed = "Shortcut removed!"
 mainwindow_home_tab_name = "Home"
 mainwindow_wf_executing_error_1 = "Cannot close a patient during workflow execution!"
 mainwindow_wf_executing_error_2 = "Cannot close " + APPNAME + " during workflow execution!"
 mainwindow_home_label1 = "Welcome to " + APPNAME + "!"
 mainwindow_home_label2 = APPNAME + " (" + app_acronym + ") is a graphic tools for modular neuroimaging processing. " \
-                        "With " + APPNAME + "you can easily import and organize DICOM files from multiple sources, " \
+                        "With " + APPNAME + " you can easily import and organize DICOM files from multiple sources, " \
                         "generate a pipeline based on available imaging modalities and export results in a " \
                         "multimodal scene."
-mainwindow_home_label3 = APPNAME + "does NOT implement processing software but integrates in a user-friendly " \
+mainwindow_home_label3 = APPNAME + " does NOT implement processing software but integrates in a user-friendly " \
                         "interface many external applications, so make sure the check the following dependencies."
 mainwindow_home_label4 = APPNAME + " is not meant for clinical use!\n"
 mainwindow_home_label5 = "\nExternal mandatory dependencies:"
 mainwindow_home_label6 = "\nExternal recommended dependencies:"
 mainwindow_home_label7 = "\nExternal optional dependencies:"
 
 mainwindow_dep_slicer_src = "Searching Slicer installation..."
```

### Comparing `swane-0.0.3/swane/ui/CustomTreeWidgetItem.py` & `swane-0.0.4/swane/ui/CustomTreeWidgetItem.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/ui/MainWindow.py` & `swane-0.0.4/swane/ui/MainWindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,21 @@
                                QSpacerItem, QWidget, QTabBar, QDialog)
 from swane.utils.check_dependency import (check_dcm2niix, check_fsl, check_freesurfer,
                                           check_graphviz)
 from PySide6.QtGui import QAction, QIcon, QPixmap, QFont
 from PySide6.QtCore import QCoreApplication, QThreadPool
 from PySide6.QtSvgWidgets import QSvgWidget
 import os
-import shutil
-import sys
-import pyshortcuts
-from pyshortcuts.shortcut import shortcut as shcdef
-from pyshortcuts.shortcut import Shortcut
 
 from swane.ui.PtTab import PtTab
 from swane.ui.PreferencesWindow import PreferencesWindow
 import swane_supplement
 from swane import __version__, EXIT_CODE_REBOOT, strings
 from swane.utils.DataInput import DataInputList
+from swane.utils.shortcut_manager import shortcut_manager
 from swane.slicer.SlicerCheckWorker import SlicerCheckWorker
 
 
 class MainWindow(QMainWindow):
     ptDirPath = ""
     tabWidget = None
 
@@ -232,46 +228,14 @@
                 return True
         return False
 
     def reset_workflows(self):
         for pt in self.pt_tabs_array:
             pt.reset_workflow()
 
-    def toggle_shortcut(self):
-        if self.global_config.get_shortcut_path() == "":
-
-            # brutal monkey patch
-            setattr(pyshortcuts.shortcut, "shortcut", my_shortcut)
-            
-            icon_file = swane_supplement.appIcon_file
-            setattr(pyshortcuts.linux, "shortcut", my_shortcut)
-
-            scut = pyshortcuts.make_shortcut(
-                strings.APPNAME, name=strings.APPNAME, icon=icon_file, terminal=False,
-                executable=sys.executable + " -m")
-            targets = [os.path.join(f, scut.target)
-                       for f in (scut.desktop_dir, scut.startmenu_dir)]
-            self.global_config.set_shortcut_path("|".join(targets))
-            msg_box = QMessageBox()
-            msg_box.setText(strings.mainwindow_shortcut_created)
-            msg_box.exec()
-        else:
-            targets = self.global_config.get_shortcut_path().split("|")
-            for fil in targets:
-                if strings.APPNAME in fil and os.path.exists(fil):
-                    if os.path.isdir(fil):
-                        shutil.rmtree(fil, ignore_errors=True)
-                    else:
-                        os.remove(fil)
-            self.global_config.set_shortcut_path("")
-            msg_box = QMessageBox()
-            msg_box.setText(strings.mainwindow_shortcut_removed)
-            msg_box.exec()
-        self.global_config.save()
-
     def about(self):
         about_dialog = QDialog(parent=self)
         layout = QGridLayout()
 
         bold_font = QFont()
         bold_font.setBold(True)
         title_font = QFont()
@@ -332,18 +296,18 @@
         menu.setNativeMenuBar(False)
         file_menu = menu.addMenu(strings.menu_file_name)
         file_menu.addAction(button_action)
         file_menu.addAction(button_action2)
         file_menu.addAction(button_action3)
         tool_menu = menu.addMenu(strings.menu_tools_name)
         tool_menu.addAction(button_action4)
-        if pyshortcuts.platform.startswith('linux'):
-            button_action5 = QAction(strings.menu_shortcut, self)
-            button_action5.triggered.connect(self.toggle_shortcut)
-            tool_menu.addAction(button_action5)
+        button_action5 = QAction(strings.menu_shortcut, self)
+        button_action5.triggered.connect(lambda checked=None, global_config=self.global_config: shortcut_manager(global_config))
+
+        tool_menu.addAction(button_action5)
         help_menu = menu.addMenu(strings.menu_help_name)
         help_menu.addAction(button_action6)
 
         self.main_tab = QTabWidget(parent=self)
         self.main_tab.setTabsClosable(True)
         self.main_tab.tabCloseRequested.connect(self.close_pt)
         self.setCentralWidget(self.main_tab)
@@ -490,18 +454,7 @@
         if found:
             self.global_config.set_slicer_path(cmd)
             self.global_config.save()
             self.slicerlabel_icon.load(self.OK_ICON_FILE)
         else:
             self.slicerlabel_icon.load(self.ERROR_ICON_FILE)
         self.slicerlabel.setText(msg)
-
-
-orig_shortcut = shcdef
-
-
-def my_shortcut(script, userfolders, name=None, description=None, folder=None, working_dir=None, icon=None):
-    r = orig_shortcut(script, userfolders, name=name, description=description,
-                      folder=folder, working_dir=working_dir, icon=icon)
-    return Shortcut(strings.APPNAME, strings.APPNAME, r.icon, r.target,
-                    working_dir, strings.APPNAME, strings.APPNAME, r.arguments,
-                    r.desktop_dir, r.startmenu_dir)
```

### Comparing `swane-0.0.3/swane/ui/PersistentProgressDialog.py` & `swane-0.0.4/swane/ui/PersistentProgressDialog.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/ui/PreferencesWindow.py` & `swane-0.0.4/swane/ui/PreferencesWindow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/ui/PtTab.py` & `swane-0.0.4/swane/ui/PtTab.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/ui/VerticalScrollArea.py` & `swane-0.0.4/swane/ui/VerticalScrollArea.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/ui/workers/DicomSearchWorker.py` & `swane-0.0.4/swane/ui/workers/DicomSearchWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/ui/workers/WorkflowGeneratorWorker.py` & `swane-0.0.4/swane/ui/workers/WorkflowGeneratorWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/ui/workers/WorkflowMonitorWorker.py` & `swane-0.0.4/swane/ui/workers/WorkflowMonitorWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/ui/workers/WorkflowProcess.py` & `swane-0.0.4/swane/ui/workers/WorkflowProcess.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/utils/ConfigManager.py` & `swane-0.0.4/swane/utils/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/utils/DataInput.py` & `swane-0.0.4/swane/utils/DataInput.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/utils/PreferenceEntry.py` & `swane-0.0.4/swane/utils/PreferenceEntry.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/utils/check_dependency.py` & `swane-0.0.4/swane/utils/check_dependency.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane/utils/fsl_conflict_handler.py` & `swane-0.0.4/swane/utils/fsl_conflict_handler.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.3/swane.egg-info/SOURCES.txt` & `swane-0.0.4/swane.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,8 +69,9 @@
 swane/ui/workers/WorkflowProcess.py
 swane/ui/workers/__init__.py
 swane/utils/ConfigManager.py
 swane/utils/DataInput.py
 swane/utils/PreferenceEntry.py
 swane/utils/__init__.py
 swane/utils/check_dependency.py
-swane/utils/fsl_conflict_handler.py
+swane/utils/fsl_conflict_handler.py
+swane/utils/shortcut_manager.py
```

