# Comparing `tmp/unravel-python-1.1.9.tar.gz` & `tmp/unravel-python-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.1.9.tar", last modified: Wed Mar 29 15:20:19 2023, max compression
+gzip compressed data, was "unravel-python-1.2.0.tar", last modified: Tue Apr 11 16:23:29 2023, max compression
```

## Comparing `unravel-python-1.1.9.tar` & `unravel-python-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 15:20:19.340000 unravel-python-1.1.9/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.1.9/LICENSE
--rw-rw-rw-   0        0        0     3894 2023-03-29 15:20:20.000000 unravel-python-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3436 2023-03-29 12:52:54.000000 unravel-python-1.1.9/README.md
--rw-rw-rw-   0        0        0       42 2023-03-29 15:20:20.000000 unravel-python-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 15:20:19.350000 unravel-python-1.1.9/unravel/
--rw-rw-rw-   0        0        0      358 2023-03-29 15:20:04.000000 unravel-python-1.1.9/unravel/__init__.py
--rw-rw-rw-   0        0        0    48038 2023-03-29 15:18:30.000000 unravel-python-1.1.9/unravel/core.py
--rw-rw-rw-   0        0        0     2627 2023-03-09 16:06:16.000000 unravel-python-1.1.9/unravel/example.py
--rw-rw-rw-   0        0        0     9538 2023-03-13 14:45:10.000000 unravel-python-1.1.9/unravel/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-29 15:20:19.350000 unravel-python-1.1.9/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     3894 2023-03-29 15:20:20.000000 unravel-python-1.1.9/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-03-29 15:20:20.000000 unravel-python-1.1.9/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 15:20:20.000000 unravel-python-1.1.9/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-03-29 15:20:20.000000 unravel-python-1.1.9/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-29 15:20:20.000000 unravel-python-1.1.9/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 16:23:29.570000 unravel-python-1.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3897 2023-04-11 16:23:30.000000 unravel-python-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3439 2023-04-05 09:30:36.000000 unravel-python-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-11 16:23:30.000000 unravel-python-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-03-10 13:34:14.000000 unravel-python-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 16:23:29.570000 unravel-python-1.2.0/unravel/
+-rw-rw-rw-   0        0        0      358 2023-04-11 16:23:06.000000 unravel-python-1.2.0/unravel/__init__.py
+-rw-rw-rw-   0        0        0    48173 2023-04-05 16:32:30.000000 unravel-python-1.2.0/unravel/core.py
+-rw-rw-rw-   0        0        0     4558 2023-04-05 16:37:44.000000 unravel-python-1.2.0/unravel/example.py
+-rw-rw-rw-   0        0        0    14119 2023-04-09 12:47:56.000000 unravel-python-1.2.0/unravel/utils.py
+-rw-rw-rw-   0        0        0     3746 2023-04-08 18:50:14.000000 unravel-python-1.2.0/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2023-04-11 16:23:29.580000 unravel-python-1.2.0/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     3897 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 16:23:30.000000 unravel-python-1.2.0/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.1.9/LICENSE` & `unravel-python-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.1.9/PKG-INFO` & `unravel-python-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.1.9
+Version: 1.2.0
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
@@ -22,15 +22,15 @@
 
 [![Documentation Status](https://readthedocs.org/projects/unravel/badge/?version=latest)](https://unravel.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/unravel-python?label=pypi%20package)](https://pypi.org/project/unravel-python/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/TIME-python)](https://pypi.org/project/unravel-python/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/unravel)
 [![DOI](https://zenodo.org/badge/455556787.svg)](https://zenodo.org/badge/latestdoi/455556787)
 
-The documentation of the code is available on [readthedocs](https://time.readthedocs.io/en/latest/)
+The documentation of the code is available on [readthedocs](https://unravel.readthedocs.io/en/latest/)
 
 ## Description
 
 To *unravel* has two meanings :
 
 * to disentangle the fibers of
 * to resolve the intricacy, complexity, or obscurity of
```

### Comparing `unravel-python-1.1.9/README.md` & `unravel-python-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [![Documentation Status](https://readthedocs.org/projects/unravel/badge/?version=latest)](https://unravel.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/unravel-python?label=pypi%20package)](https://pypi.org/project/unravel-python/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/TIME-python)](https://pypi.org/project/unravel-python/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/unravel)
 [![DOI](https://zenodo.org/badge/455556787.svg)](https://zenodo.org/badge/latestdoi/455556787)
 
-The documentation of the code is available on [readthedocs](https://time.readthedocs.io/en/latest/)
+The documentation of the code is available on [readthedocs](https://unravel.readthedocs.io/en/latest/)
 
 ## Description
 
 To *unravel* has two meanings :
 
 * to disentangle the fibers of
 * to resolve the intricacy, complexity, or obscurity of
```

### Comparing `unravel-python-1.1.9/setup.py` & `unravel-python-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.1.9/unravel/core.py` & `unravel-python-1.2.0/unravel/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1120,14 +1120,17 @@
                 mgtList.append(groundTruth_map[voxel])
 
         axs.plot(vList, mList, label=method)
 
     if groundTruth_map is not None:
         axs.plot(vList, mgtList, label='Ground truth')
     axs.legend()
+    axs.set_ylabel('Metric')
+    axs.set_xlabel('Streamline segment position')
+    axs.set_title('Microstructure along streamline')
 
 
 def plot_streamline_metrics_old(streamList: list, metric_maps: list,
                                 groundTruth_map=None, barplot: bool = True,
                                 method_list: list = ['ang'], fList: list = []):
     '''
     Plots the evolution of a metric along the course of a single streamline.
```

### Comparing `unravel-python-1.1.9/unravel/utils.py` & `unravel-python-1.2.0/unravel/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 import numpy as np
 from dipy.io.streamline import load_tractogram
 
 
 def tract_to_ROI(trk_file: str):
     '''
-    Returns a binary mask of each voxel containing a tractography node. The voxels containing streamlines segments but no nodes will not be selected.
+    Returns a binary mask of each voxel containing a tractography node.The
+    voxels containing streamlines segments but no nodes will not be selected.
 
     Parameters
     ----------
     trk_file : str
         Path to tractography file (.trk)
 
     Returns
@@ -57,95 +58,103 @@
         List of arrays of shape (x,y,z) containing the fiber volume fraction of
         each fixel. The default is None.
 
     Returns
     -------
     rgb : 4-D array of shape (x,y,z,3)
         RGB map of shape (x,y,z,3) representing the main direction of
-        of the peaks.
+        of the peaks. With type float64 [0,1].
 
     '''
 
     # Safety net
     if type(peaksList) != list:
         if len(peaksList.shape) == 5:
             peaksArray = peaksList.copy()
             peaksList = []
             for k in range(peaksArray.shape[4]):
                 peaksList.append(peaksArray[:, :, :, :, k])
         else:
             peaksList = [peaksList]
 
     K = len(peaksList)
+    dim = len(peaksList[0].shape[:-1])
+
+    len_ratio = np.ones(peaksList[0].shape[:-1])
 
     for k in range(K):
         peaksList[k] = np.nan_to_num(peaksList[k])
+        len_ratio += np.where(np.sum(peaksList[k], axis=dim) == 0, 1, 0)
 
     if fracList is None:
         fracList = []
         for k in range(K):
-            fracList.append(np.ones(peaksList[0].shape[:3]))
+            fracList.append(np.ones(peaksList[0].shape[:-1]))
 
     if fvfList is None:
         fvfList = []
         for k in range(K):
-            fvfList.append(np.ones(peaksList[0].shape[:3]))
+            fvfList.append(np.ones(peaksList[0].shape[:-1]))
 
     rgb = np.zeros(peaksList[0].shape)
 
-    for xyz in np.ndindex(peaksList[0].shape[:3]):
+    for xyz in np.ndindex(peaksList[0].shape[:-1]):
         for k in range(K):
             rgb[xyz] += abs(peaksList[k][xyz])*fracList[k][xyz]*fvfList[k][xyz]
 
+    # Normalize between [0,1] and by number of peaks per voxel
+    rgb *= np.repeat(1+len_ratio[(slice(None),) *
+                     dim + (np.newaxis,)]/K, 3, axis=dim)
+    rgb /= np.max(rgb)
+
     return rgb
 
 
 def peaks_to_peak(peaksList: list, fixel_weights, fracList: list = None,
                   fvfList: list = None):
     '''
     Fuse peaks into a single peak based on fixel weight and fvf, intensity
-    is then weighted with frac Mostly used for visualization purposes.
+    is then weighted with frac. Mostly used for visualization purposes.
 
     Parameters
     ----------
     peaksList : list of 4-D arrays
         List of arrays containing the peaks of shape (x,y,z,3)
     fixel_weights : 4-D array of shape (x,y,z,K)
         Array containing the relative weights of the K fixels in each voxel.
 
     Returns
     -------
-    None.
+    peak : 3-D array of shape (x,y,z,3)
 
     '''
 
     K = len(peaksList)
 
     for k in range(K):
         peaksList[k] = np.nan_to_num(peaksList[k])
 
     peak = np.zeros(peaksList[0].shape)
 
     if fracList is None:
         fracList = []
         for k in range(K):
-            fracList.append(np.ones(peaksList[0].shape[:3]))/k
+            fracList.append(np.ones(peaksList[0].shape[:-1])/(k+1))
 
     if fvfList is None:
         fvfList = []
         for k in range(K):
-            fvfList.append(np.ones(peaksList[0].shape[:3]))
+            fvfList.append(np.ones(peaksList[0].shape[:-1]))
 
-    fracTot = np.zeros(peaksList[0].shape[:3])
+    fracTot = np.zeros(peaksList[0].shape[:-1])
 
-    for xyz in np.ndindex(peaksList[0].shape[:3]):
+    for xyz in np.ndindex(peaksList[0].shape[:-1]):
         for k in range(K):
-            peak[xyz] += abs(peaksList[k][xyz]) * \
-                fixel_weights[xyz+(k,)]/np.sum(fixel_weights[xyz]) * \
-                fvfList[k][xyz]
+            peak[xyz] += (abs(peaksList[k][xyz])*fixel_weights[xyz+(k,)]
+                          / np.sum(fixel_weights[xyz])*fvfList[k][xyz])
 
     for k in range(K):
         fracTot += fracList[k]
 
     peak[..., 0] *= fracTot
     peak[..., 1] *= fracTot
     peak[..., 2] *= fracTot
@@ -222,62 +231,189 @@
     MD = MD.real.astype('float64')
 
     np.seterr(divide='warn', invalid='warn')
 
     return FA, AD, RD, MD
 
 
-def get_streamline_density(trk, resolution_increase: int = 1):
+def get_streamline_count(trk) -> int:
+    '''
+    Returns the number of streamlines in a tractogram.
+
+    Parameters
+    ----------
+    trk : tractogram
+        Content of a .trk file
+
+    Returns
+    -------
+    count : int
+        Number of streamlines in tractogram.
+
+    '''
+
+    # Safety net
+    if type(trk) == str:
+        trk = load_tractogram(trk, 'same')
+
+    count = len(trk.streamlines._offsets)
+
+    return count
+
+
+def get_streamline_angle(trk, resolution_increase: int = 1):
     '''
     Get the fixel weights from a tract specified in trk_file.
 
     Parameters
     ----------
     trk : tractogram
         Content of a .trk file
     resolution_increase : int, optional
-        Factor multuplying the resolution/dimensions of output array. The
+        Factor multiplying the resolution/dimensions of output array. The
         default is 1.
 
     Returns
     -------
     density : 3-D array of shape (x,y,z)
+        Array containing the mean angle of streamline segments in each voxel.
+    '''
+
+    from TIME.core import (tract_to_streamlines, compute_subsegments,
+                           angle_difference)
+    from tqdm import tqdm
+
+    num = np.zeros(trk._dimensions*resolution_increase)
+    angle = np.zeros(trk._dimensions*resolution_increase)
+
+    sList = tract_to_streamlines(trk)
+
+    for streamline in tqdm(sList):
+
+        previous_point = streamline[1, :]*resolution_increase
+        previous_dir = (previous_point-streamline[0, :]*resolution_increase)
+
+        for i in range(2, streamline.shape[0]):
+
+            point = streamline[i, :]*resolution_increase
+
+            voxList = compute_subsegments(previous_point, point)
+            vs = (point-previous_point)
+            ang = angle_difference(vs, previous_dir)
+
+            for x, y, z in voxList:
+
+                x, y, z = (int(x), int(y), int(z))
+
+                num[x, y, z] += 1
+                angle[x, y, z] += ang
+
+            previous_point = point
+            previous_dir = vs
+
+    angle[num != 0] /= num[num != 0]
+
+    return angle
+
+
+def get_streamline_density(trk, resolution_increase: int = 1,
+                           color: bool = False):
+    '''
+    Get the total segment length from a tract specified in trk.
+
+    Parameters
+    ----------
+    trk : tractogram
+        Content of a .trk file
+    resolution_increase : int, optional
+        Factor multiplying the resolution/dimensions of output array. The
+        default is 1.
+    color : bool, optional
+        If True, output a RGB volume with colors corresponding to the
+        directions of the streamlines, modulated by streamline density.
+        The default is False.
+
+    Returns
+    -------
+    density : 3-D array of shape (x,y,z)
         Array containing the streamline density in each voxel.
     '''
 
     from TIME.core import tract_to_streamlines, compute_subsegments
     from tqdm import tqdm
 
-    density = np.zeros(trk._dimensions*resolution_increase)
+    density = np.zeros(trk._dimensions*resolution_increase, dtype=np.float16)
+    rgb = np.zeros(tuple(trk._dimensions*resolution_increase)+(3,),
+                   dtype=np.float16)
 
     sList = tract_to_streamlines(trk)
 
     for streamline in tqdm(sList):
 
         previous_point = streamline[0, :]*resolution_increase
 
         for i in range(1, streamline.shape[0]):
 
             point = streamline[i, :]*resolution_increase
 
             voxList = compute_subsegments(previous_point, point)
+            vs = (point-previous_point)
 
             for x, y, z in voxList:
 
                 x, y, z = (int(x), int(y), int(z))
 
                 density[x, y, z] += voxList[(x, y, z)]
+                if color:
+                    rgb[x, y, z] += abs(vs)
 
             previous_point = point
 
+    if color:
+        return rgb
+
     return density
 
 
+def normalize_color(rgb, norm_all_voxels: bool = False):
+    '''
+    Sets values in RGB array (x,y,z,3) to be within [0,1].
+
+    TODO: increase speed when norm_all_voxels is set to True.
+
+    Parameters
+    ----------
+    rgb : 3-D array of shape (x,y,z,3)
+        RGB volume.
+    norm_all_voxels : bool, optional
+        If True, all voxel display maximum intensity. The default is False.
+
+    Returns
+    -------
+    norm : 3-D array of shape (x,y,z,3)
+        RGB volume.
+
+    '''
+
+    if norm_all_voxels:
+        norm = np.zeros(rgb.shape)
+
+        for xyz in np.ndindex(rgb.shape[:-1]):
+            if np.sum(rgb[xyz]) != 0:
+                norm[xyz] = rgb[xyz] / np.linalg.norm(rgb[xyz])
+    else:
+        norm = rgb/np.max(rgb)
+
+    return norm
+
+
 def plot_streamline_trajectory(trk, resolution_increase: int = 1,
-                               streamline_number: int = 0, axis: int = 1):
+                               streamline_number: int = 0, axis: int = 1,
+                               color: bool = False,
+                               norm_all_voxels: bool = False):
     '''
     Produces a grpah of the streamline density of tract 'trk', the streamline
     specified with 'streamline_number' is highlighted along 'axis'.
 
     Parameters
     ----------
     trk : tractogram
@@ -285,27 +421,38 @@
     resolution_increase : int, optional
         The dimensions of the volume are multiplied by this value to increase
         resolution. The default is 1.
     streamline_number : int, optional
         Number of the streamline to be highlighted. The default is 0.
     axis : int, optional
         Axis of inspection, [0:2] in 3D volumes. The default is 1.
+    color : bool, optional
+        If True, output a RGB volume with colors corresponding to the
+        directions of the streamlines, modulated by streamline density.
+        The default is False.
+    norm_all_voxels : bool, optional
+        If True, all RGB voxels display maximum intensity. Increases computation
+        time. The default is False.
 
     Returns
     -------
     None.
 
     '''
 
     import matplotlib.pyplot as plt
-    from TIME.core import tract_to_streamlines, compute_subsegments
+    from TIME.core import tract_to_streamlines
 
-    density = get_streamline_density(trk,
+    density = get_streamline_density(trk, color=color,
                                      resolution_increase=resolution_increase)
 
+    if color:
+        density = normalize_color(density, norm_all_voxels=norm_all_voxels)
+        density = (density*255).astype('uint8')
+
     sList = tract_to_streamlines(trk)
 
     streamline = sList[streamline_number]
 
     x = []
     y = []
     z = []
@@ -314,20 +461,27 @@
 
         point = streamline[i, :]*resolution_increase
 
         x.append(point[0])
         y.append(point[1])
         z.append(point[2])
 
+    transpose = [1, 0]
+    c = '#e69402ff'
+    if color:
+        transpose.append(2)
+        c = '#ffffffff'
+
     plt.figure()
     if axis == 0:
-        plt.imshow(density[int(sum(x)/len(x)), :, :].T,
+        plt.imshow(np.transpose(density[int(sum(x)/len(x)), :, :], transpose),
                    origin='lower', cmap='gray')
-        plt.plot(y, z, '.-', c='#e69402ff')
+        plt.plot(y, z, '.-', c=c)
     elif axis == 1:
-        plt.imshow(density[:, int(sum(y)/len(y)), :].T,
+        plt.imshow(np.transpose(density[:, int(sum(y)/len(y)), :], transpose),
                    origin='lower', cmap='gray')
-        plt.plot(x, z, '.-', c='#e69402ff')
+        plt.plot(x, z, '.-', c=c)
     else:
-        plt.imshow(density[:, :, int(sum(z)/len(z))].T,
+        plt.imshow(np.transpose(density[:, :, int(sum(z)/len(z))], transpose),
                    origin='lower', cmap='gray')
-        plt.plot(x, y, '.-', c='#e69402ff')
+        plt.plot(x, y, '.-', c=c)
+    plt.title('Streamline trajectory')
```

### Comparing `unravel-python-1.1.9/unravel_python.egg-info/PKG-INFO` & `unravel-python-1.2.0/unravel_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.1.9
+Version: 1.2.0
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
@@ -22,15 +22,15 @@
 
 [![Documentation Status](https://readthedocs.org/projects/unravel/badge/?version=latest)](https://unravel.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/unravel-python?label=pypi%20package)](https://pypi.org/project/unravel-python/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/TIME-python)](https://pypi.org/project/unravel-python/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/unravel)
 [![DOI](https://zenodo.org/badge/455556787.svg)](https://zenodo.org/badge/latestdoi/455556787)
 
-The documentation of the code is available on [readthedocs](https://time.readthedocs.io/en/latest/)
+The documentation of the code is available on [readthedocs](https://unravel.readthedocs.io/en/latest/)
 
 ## Description
 
 To *unravel* has two meanings :
 
 * to disentangle the fibers of
 * to resolve the intricacy, complexity, or obscurity of
```

