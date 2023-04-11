# Comparing `tmp/cpctools-0.1.0.tar.gz` & `tmp/cpctools-0.1.0rc0.tar.gz`

## Comparing `cpctools-0.1.0.tar` & `cpctools-0.1.0rc0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/__init__.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/analysis.py
--rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/classify.py
--rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/cli.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/distances.py
--rw-r--r--   0        0        0    17579 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/engine.py
--rw-r--r--   0        0        0    15439 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/saponify.py
--rw-r--r--   0        0        0    11916 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/utils.py
--rw-r--r--   0        0        0    11323 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/HDF5er/HDF5To.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/HDF5er/HDF5erUtils.py
--rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/HDF5er/ToHDF5.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/HDF5er/__init__.py
--rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/transitions/__init__.py
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 cpctools-0.1.0/SOAPify/transitions/tracker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/requirements.txt
--rw-r--r--   0        0        0    64343 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/testSupport.py
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_HDF5er.py
--rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_HDF5ertools.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_SOAPify.py
--rw-r--r--   0        0        0     8958 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_SOAPifyEngine.py
--rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_SOAPifySOAP.py
--rw-r--r--   0        0        0    16071 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_analysis.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_classification.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_transitions/__init__.py
--rw-r--r--   0        0        0    13111 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_transitions/test_tracker.py
--rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 cpctools-0.1.0/tests/test_transitions/test_transitions.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cpctools-0.1.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 cpctools-0.1.0/LICENSE
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 cpctools-0.1.0/Readme.md
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 cpctools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 cpctools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/__init__.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/analysis.py
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/classify.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/distances.py
+-rw-r--r--   0        0        0    17579 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/engine.py
+-rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/saponify.py
+-rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/utils.py
+-rw-r--r--   0        0        0    11237 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/HDF5er/HDF5To.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/HDF5er/HDF5erUtils.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/HDF5er/ToHDF5.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/HDF5er/__init__.py
+-rw-r--r--   0        0        0     8853 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/transitions/__init__.py
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/SOAPify/transitions/tracker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/conftest.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/requirements.txt
+-rw-r--r--   0        0        0    64298 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/testSupport.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_HDF5er.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_HDF5ertools.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_SOAPify.py
+-rw-r--r--   0        0        0     8958 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_SOAPifyEngine.py
+-rw-r--r--   0        0        0    13624 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_SOAPifySOAP.py
+-rw-r--r--   0        0        0    13478 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_analysis.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_classification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_transitions/__init__.py
+-rw-r--r--   0        0        0    13111 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_transitions/test_tracker.py
+-rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/tests/test_transitions/test_transitions.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/Readme.md
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 cpctools-0.1.0rc0/PKG-INFO
```

### Comparing `cpctools-0.1.0/SOAPify/analysis.py` & `cpctools-0.1.0rc0/SOAPify/analysis.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,41 @@
 """Module that contains various analysis routines"""
-
 import numpy
 from numpy import ndarray
+from .distances import simpleSOAPdistance
 from MDAnalysis import Universe, AtomGroup
 from MDAnalysis.lib.NeighborSearch import AtomNeighborSearch
-import h5py
-
-from .distances import simpleSOAPdistance
-from .utils import getSOAPSettings, normalizeArray, fillSOAPVectorFromdscribe
 
 
-def timeSOAP(
+def tempoSOAP(
     SOAPTrajectory: ndarray,
     window: int = 1,
     stride: int = None,
     backward: bool = False,
-    returnDiff: bool = True,
     distanceFunction: callable = simpleSOAPdistance,
 ) -> "tuple[ndarray, ndarray]":
-    """performs the 'timeSOAP' analysis on the given SOAP trajectory
+    """performs the 'tempoSOAP' analysis on the given SOAP trajectory
 
         * Original author: Cristina Caruso
         * Mantainer: Daniele Rapetti
     Args:
         SOAPTrajectory (int):
-            a trajectory of SOAP fingerprints, should have shape (nFrames,nAtoms,SOAPlenght)
+            an array containg a soap trajectory, the shape is (frames, atom, SOAPdim)
         window (int):
             the dimension of the windows between each state confrontations.
             Defaults to 1.
         stride (int):
             the stride in frames between each state confrontation. **NOT IN USE**.
             Defaults to None.
-        backward (bool):
-            If true the soap distance is referred to the previous frame.
-             **NOT IN USE**. Defaulst to True.
-        returnDiff (bool):
-            If true returns also the first derivative of timeSOAP. Defaults to True.
+        deltaT (int): number of frames to skip
         distanceFunction (callable, optional):
             the function that define the distance. Defaults to :func:`SOAPify.distances.simpleSOAPdistance`.
 
     Returns:
-        tuple[numpy.ndarray,numpy.ndarray]:
-            - **timedSOAP** the timeSOAP values, shape(frames-1,natoms)
-            - **deltaTimedSOAP** the derivatives of timeSOAP, shape(natoms, frames-2)
+        tuple[numpy.ndarray,numpy.ndarray]: _description_
     """
     if stride is None:
         stride = window
     if stride > window:
         raise ValueError("the window must be bigger than the stride")
     if window >= SOAPTrajectory.shape[0] or stride >= SOAPTrajectory.shape[0]:
         raise ValueError("stride and window must be smaller than simulation lenght")
@@ -59,71 +48,49 @@
             # fill the matrix (each molecule for each frame)
             timedSOAP[frame - window, molecule] = distanceFunction(x, y)
     # vectorizedDistanceFunction = numpy.vectorize(
     #     distanceFunction, signature="(n),(n)->(1)"
     # )
     # print(SOAPTrajectory.shape)
 
-    if returnDiff:
-        deltaTimedSOAP = numpy.diff(timedSOAP.T, axis=-1)
-        return timedSOAP, deltaTimedSOAP
-    return timedSOAP
+    expectedDeltaTimedSOAP = numpy.diff(timedSOAP, axis=-1)
 
+    return timedSOAP, expectedDeltaTimedSOAP
 
-def timeSOAPsimple(
+
+def tempoSOAPsimple(
     SOAPTrajectory: ndarray,
     window: int = 1,
     stride: int = None,
     backward: bool = False,
-    returnDiff: bool = True,
 ) -> "tuple[ndarray, ndarray]":
-    r"""performs the 'timeSOAP' analysis on the given **normalized** SOAP trajectory
+    """performs the 'tempoSOAP' analysis on the given SOAP trajectory
 
-        this is optimized to use :func:`SOAPify.distances.simpleSOAPdistance`,
-        without calling it.
+        this is optimized to use :func:`SOAPify.distances.simpleSOAPdistance`
+        without calling it
 
         .. warning:: this function works **only** with normalized numpy.float64
           soap vectors!
 
-            The SOAP distance is calculated with
-
-            .. math::
-                d(\vec{a},\vec{b})=\sqrt{2-2\frac{\vec{a}\cdot\vec{b}}{\left\|\vec{a}\right\|\left\|\vec{b}\right\|}}
-
-            That is equivalent to
-
-            .. math::
-                d(\vec{a},\vec{b})=\sqrt{2-2\hat{a}\cdot\hat{b}} = \sqrt{\hat{a}\cdot\hat{a}+\hat{b}\cdot\hat{b}-2\hat{a}\cdot\hat{b}} =
-
-                \sqrt{(\hat{a}-\hat{b})\cdot(\hat{a}-\hat{b})}
-
-            That is the euclidean distance between the versors
 
         * Original author: Cristina Caruso
         * Mantainer: Daniele Rapetti
     Args:
         SOAPTrajectory (int):
-            a **normalize ** trajectory of SOAP fingerprints, should have shape
-            (nFrames,nAtoms,SOAPlenght)
+            _description_
         window (int):
             the dimension of the windows between each state confrontations.
             Defaults to 1.
         stride (int):
             the stride in frames between each state confrontation. **NOT IN USE**.
             Defaults to None.
-        backward (bool):
-            If true the soap distance is referred to the previous frame.
-             **NOT IN USE**. Defaulst to True.
-        returnDiff (bool):
-            If true returns also the first derivative of timeSOAP. Defaults to True.
+        deltaT (int): number of frames to skip
 
     Returns:
-        tuple[numpy.ndarray,numpy.ndarray]:
-            - **timedSOAP** the timeSOAP values, shape(frames-1,natoms)
-            - **deltaTimedSOAP** the derivatives of timeSOAP, shape(natoms, frames-2)
+        tuple[numpy.ndarray,numpy.ndarray]: _description_
     """
     if stride is None:
         stride = window
     if stride > window:
         raise ValueError("the window must be bigger than the stride")
     if window >= SOAPTrajectory.shape[0] or stride >= SOAPTrajectory.shape[0]:
         raise ValueError("stride and window must be smaller than simulation lenght")
@@ -132,79 +99,17 @@
     prev = SOAPTrajectory[0]
     for frame in range(window, SOAPTrajectory.shape[0]):
         actual = SOAPTrajectory[frame]
         # this is equivalent to distance of two normalized SOAP vector
         timedSOAP[frame - window] = numpy.linalg.norm(actual - prev, axis=1)
         prev = actual
 
-    if returnDiff:
-        deltaTimedSOAP = numpy.diff(timedSOAP.T, axis=-1)
-        return timedSOAP, deltaTimedSOAP
-    return timedSOAP
-
-
-def getTimeSOAPSimple(
-    soapDataset: h5py.Dataset,
-    window: int = 1,
-    stride: int = None,
-    backward: bool = False,
-):
-    """Shortcut to extract the timeSOAP from large datasets.
-
-        This function is the equivalent to:
-
-        - loading a chunk of the trajectory from a h5py.Dataset with a SOAP fingerprints trajectory
-        - filling the vector with :func:`SOAPify.utils.fillSOAPVectorFromdscribe`
-        - normalizing it with :func:`SOAPify.utils.normalizeArray`
-        - calculating the timeSOAP with  :func:`timeSOAPsimple`
-        and then returning timeSOAP and the derivative
-
-
-    Args:
-        soapDataset (h5py.Dataset):
-            the dataset with the SOAP fingerprints
-        window (int):
-            the dimension of the windows between each state confrontations.
-            See :func:`timeSOAPsimple`
-            Defaults to 1.
-        stride (int):
-            the stride in frames between each state confrontation.
-            See :func:`timeSOAPsimple`
-            Defaults to None.
-        backward (bool):
-            If true the soap distance is referred to the previous frame.
-            See :func:`timeSOAPsimple` . Defaulst to True.
-
-    Returns:
-        tuple[numpy.ndarray,numpy.ndarray]:
-            - **timedSOAP** the timeSOAP values, shape(frames-1,natoms)
-            - **deltaTimedSOAP** the derivatives of timeSOAP, shape(natoms, frames-2)
-    """
-    fillSettings = getSOAPSettings(soapDataset)
-    timedSOAP = numpy.zeros((soapDataset.shape[0] - window, soapDataset.shape[1]))
-    # TODO: add a check to the window
-
-    slide = 0
-    # this looks a lot convoluted, but it is way faster than working one atom
-    # at a time
-    for c in soapDataset.iter_chunks():
-        theSlice = slice(c[0].start - slide, c[0].stop, c[0].step)
-        outSlice = slice(c[0].start - slide, c[0].stop - 1, c[0].step)
-        timedSOAP[outSlice] = timeSOAPsimple(
-            normalizeArray(
-                fillSOAPVectorFromdscribe(soapDataset[theSlice], **fillSettings)
-            ),
-            window=window,
-            stride=stride,
-            backward=backward,
-            returnDiff=False,
-        )
-        slide = 1
+    expectedDeltaTimedSOAP = numpy.diff(timedSOAP, axis=-1)
 
-    return timedSOAP, numpy.diff(timedSOAP.T, axis=-1)
+    return timedSOAP, expectedDeltaTimedSOAP
 
 
 def listNeighboursAlongTrajectory(
     inputUniverse: Universe, cutOff: float, trajSlice: slice = slice(None)
 ) -> "list[list[AtomGroup]]":
     """produce a per frame list of the neighbours, atom per atom
 
@@ -246,16 +151,16 @@
     Returns:
         tuple[numpy.ndarray,numpy.ndarray,numpy.ndarray,numpy.ndarray]:
             - **lensArray** The calculated LENS parameter
             - **numberOfNeighs** the count of neighbours per frame
             - **lensNumerators** the numerators used for calculating LENS parameter
             - **lensDenominators** the denominators used for calculating LENS parameter
     """
-    nAt = numpy.asarray(nnListPerFrame, dtype=object).shape[1]
-    nFrames = numpy.asarray(nnListPerFrame, dtype=object).shape[0]
+    nAt = numpy.shape(nnListPerFrame)[1]
+    nFrames = numpy.shape(nnListPerFrame)[0]
     # this is the number of common NN between frames
     lensArray = numpy.zeros((nAt, nFrames))
     # this is the number of NN at that frame
     numberOfNeighs = numpy.zeros((nAt, nFrames))
     # this is the numerator of LENS
     lensNumerators = numpy.zeros((nAt, nFrames))
     # this is the denominator of lens
```

### Comparing `cpctools-0.1.0/SOAPify/classify.py` & `cpctools-0.1.0rc0/SOAPify/classify.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/SOAPify/distances.py` & `cpctools-0.1.0rc0/SOAPify/distances.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/SOAPify/engine.py` & `cpctools-0.1.0rc0/SOAPify/engine.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/SOAPify/saponify.py` & `cpctools-0.1.0rc0/SOAPify/saponify.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 def _saponifyWorker(
     trajGroup: h5py.Group,
     SOAPoutDataset: h5py.Dataset,
     soapEngine: SOAPengineContainer,
     SOAPOutputChunkDim: int = 100,
     SOAPnJobs: int = 1,
-    verbose: bool = True,
 ):
     """Calculates the soap descriptor and store the result in the given dataset
 
     Args:
         trajGroup (h5py.Group):
             the group that contains the trajectory (must contain "Box",
             "Trajectory" and "Types" datasets)
@@ -32,17 +31,14 @@
             The soap engine already set up
         SOAPOutputChunkDim (int, optional):
             The dimension of the chunck of data in the SOAP results dataset.
             Defaults to 100.
         SOAPnJobs (int, optional):
             the number of concurrent SOAP calculations (option passed to the
             desired SOAP engine). Defaults to 1.
-        verbose (bool, optional):
-            regulates the verbosity of the step by step operations.
-            Defaults to True.
     """
     symbols = trajGroup["Types"].asstr()[:]
     SOAPoutDataset.attrs["SOAPengine"] = soapEngine.SOAPenginekind
     SOAPoutDataset.attrs["l_max"] = soapEngine.lmax
     SOAPoutDataset.attrs["n_max"] = soapEngine.nmax
     SOAPoutDataset.attrs["r_cut"] = soapEngine.rcut
     SOAPoutDataset.attrs["species"] = soapEngine.species
@@ -66,52 +62,47 @@
                 )
                 SOAPoutDataset.attrs[
                     f"species_location_{soapEngine.species[i]}-{soapEngine.species[j]}"
                 ] = (temp.start, temp.stop)
 
     for chunkTraj in trajGroup["Trajectory"].iter_chunks():
         chunkBox = (chunkTraj[0], slice(0, 6, 1))
-        if verbose:
-            print(f'working on trajectory chunk "{chunkTraj}"')
-            print(f'   and working on box chunk "{repr(chunkBox)}"')
+        print(f'working on trajectory chunk "{chunkTraj}"')
+        print(f'   and working on box chunk "{repr(chunkBox)}"')
         # load in memory a chunk of data
         atoms = HDF2ase(trajGroup, chunkTraj, chunkBox, symbols)
         jobchunk = min(SOAPOutputChunkDim, len(atoms))
         jobStart = 0
         jobEnd = jobStart + jobchunk
         while jobStart < len(atoms):
             tStart = time.time()
             frameStart = jobStart + chunkTraj[0].start
             frameEnd = jobEnd + chunkTraj[0].start
-            if verbose:
-                print(f"working on frames: [{frameStart}:{frameEnd}]")
+            print(f"working on frames: [{frameStart}:{frameEnd}]")
             # TODO: dscribe1.2.1 return (nat,nsoap) instead of (1,nat,nsoap) with 1 frame input!
             SOAPoutDataset[frameStart:frameEnd] = soapEngine(
                 atoms[jobStart:jobEnd],
                 positions=[soapEngine.centersMask] * jobchunk,
                 n_jobs=SOAPnJobs,
             )
             tStop = time.time()
             jobchunk = min(SOAPOutputChunkDim, len(atoms) - jobEnd)
             jobStart = jobEnd
             jobEnd = jobStart + jobchunk
-            if verbose:
-                print(f"delta create= {tStop-tStart}")
+            print(f"delta create= {tStop-tStart}")
 
 
 def _applySOAP(
     trajContainer: h5py.Group,
     SOAPoutContainer: h5py.Group,
     key: str,
     soapEngine: SOAPengineContainer,
     SOAPOutputChunkDim: int = 100,
     SOAPnJobs: int = 1,
     doOverride: bool = False,
-    verbose: bool = True,
-    useType="float64",
 ):
     """helper function: applies the soap engine to the given trajectory within the trajContainer
 
     Args:
         trajContainer (h5py.Group):
             The group or the file that contains the trajectory, must have the
             following dataset in '/': "Box", "Trajectory" and "Types"
@@ -126,21 +117,15 @@
             if key is a new dataset will also be the size of the main chunck of
             data of the SOAP dataset . Defaults to 100.
         SOAPnJobs (int, optional):
             Number of concurrent SOAP calculations. Defaults to 1.
         doOverride (bool, optional):
             if False will raise and exception if the user ask to override an
             already existing DataSet. Defaults to False.
-        verbose (bool, optional):
-            regulates the verbosity of the step by step operations.
-            Defaults to True.
-        useType (str,optional):
-            The precision used to store the data. Defaults to "float64".
     """
-    useType = numpy.dtype(useType)
     nOfFeatures = soapEngine.features
     symbols = trajContainer["Types"].asstr()[:]
     nCenters = (
         len(symbols) if soapEngine.centersMask is None else len(soapEngine.centersMask)
     )
 
     if key in SOAPoutContainer.keys():
@@ -157,25 +142,24 @@
         SOAPoutContainer.create_dataset(
             key,
             (0, nCenters, nOfFeatures),
             compression="gzip",
             compression_opts=9,
             chunks=(SOAPOutputChunkDim, nCenters, nOfFeatures),
             maxshape=(None, nCenters, nOfFeatures),
-            dtype=useType,
+            dtype=numpy.float64,
         )
     SOAPout = SOAPoutContainer[key]
     SOAPout.resize((len(trajContainer["Trajectory"]), nCenters, nOfFeatures))
     _saponifyWorker(
         trajContainer,
         SOAPout,
         soapEngine,
         SOAPOutputChunkDim,
         SOAPnJobs,
-        verbose=verbose,
     )
 
 
 def saponifyMultipleTrajectories(
     trajContainers: "h5py.Group|h5py.File",
     SOAPoutContainers: "h5py.Group|h5py.File",
     SOAPrcut: float,
@@ -185,16 +169,14 @@
     SOAPnJobs: int = 1,
     SOAPatomMask: "list[str]" = None,
     centersMask: Iterable = None,
     SOAP_respectPBC: bool = True,
     SOAPkwargs: dict = None,
     useSoapFrom: KNOWNSOAPENGINES = "dscribe",
     doOverride: bool = False,
-    verbose: bool = True,
-    useType="float64",
 ):
     """Calculates and stores the SOAP descriptor for all of the trajectories in
     the given group/file
 
     `saponifyMultipleTrajectories` checks if any of the group contained in
     `trajContainers` is a "trajectory group"
     (see :func:`SOAPify.HDF5er.HDF5erUtils.isTrajectoryGroup`) and then calculates
@@ -238,20 +220,20 @@
             Defaults to {}.
         useSoapFrom (KNOWNSOAPENGINES, optional)
             This string determines the selected SOAP engine for the calculations.
             Defaults to "dscribe".
         doOverride (bool, optional)
             if False will raise and exception if the user ask to override an
             already existing DataSet. Defaults to False.
-        verbose (bool, optional):
-            regulates the verbosity of the step by step operations.
-            Defaults to True.
-        useType (str,optional):
-            The precision used to store the data. Defaults to "float64".
     """
+    if SOAPkwargs is None:
+        SOAPkwargs = {}
+    print(f"using {useSoapFrom} to calculate SOAP")
+    print(SOAPkwargs)
+
     for key in trajContainers.keys():
         if isTrajectoryGroup(trajContainers[key]):
             saponifyTrajectory(
                 trajContainer=trajContainers[key],
                 SOAPoutContainer=SOAPoutContainers,
                 SOAPrcut=SOAPrcut,
                 SOAPnmax=SOAPnmax,
@@ -260,16 +242,14 @@
                 SOAPnJobs=SOAPnJobs,
                 SOAPatomMask=SOAPatomMask,
                 centersMask=centersMask,
                 SOAP_respectPBC=SOAP_respectPBC,
                 SOAPkwargs=SOAPkwargs,
                 useSoapFrom=useSoapFrom,
                 doOverride=doOverride,
-                verbose=verbose,
-                useType=useType,
             )
 
 
 def saponifyTrajectory(
     trajContainer: "h5py.Group|h5py.File",
     SOAPoutContainer: "h5py.Group|h5py.File",
     SOAPrcut: float,
@@ -279,16 +259,14 @@
     SOAPnJobs: int = 1,
     SOAPatomMask: str = None,
     centersMask: Iterable = None,
     SOAP_respectPBC: bool = True,
     SOAPkwargs: dict = None,
     useSoapFrom: KNOWNSOAPENGINES = "dscribe",
     doOverride: bool = False,
-    verbose: bool = True,
-    useType="float64",
 ):
     """Calculates the SOAP fingerprints for each atom in a given hdf5 trajectory
 
     Works exaclty as :func:`saponifyMultipleTrajectories` except for that it
     calculates the fingerprints only for the passed trajectory group
     (see :func:`SOAPify.HDF5er.HDF5erUtils.isTrajectoryGroup`).
 
@@ -331,23 +309,20 @@
             Defaults to {}.
         useSoapFrom (KNOWNSOAPENGINES, optional):
             This string determines the selected SOAP engine for the calculations.
             Defaults to "dscribe".
         doOverride (bool, optional):
             if False will raise and exception if the user ask to override an
             already existing DataSet. Defaults to False.
-        verbose (bool, optional):
-            regulates the verbosity of the step by step operations.
-            Defaults to True.
-        useType (str,optional):
-            The precision used to store the data. Defaults to "float64".
     """
+    if SOAPkwargs is None:
+        SOAPkwargs = {}
+    print(f"using {useSoapFrom} to calculate SOAP")
+    print(SOAPkwargs)
     if isTrajectoryGroup(trajContainer):
-        print(f'using "{useSoapFrom}" to calculate SOAP for "{trajContainer.name}"')
-        print("extra SOAP arguments:", SOAPkwargs)
         symbols = trajContainer["Types"].asstr()[:]
         soapEngine = getSoapEngine(
             atomNames=symbols,
             SOAPrcut=SOAPrcut,
             SOAPnmax=SOAPnmax,
             SOAPlmax=SOAPlmax,
             SOAPatomMask=SOAPatomMask,
@@ -361,12 +336,10 @@
             trajContainer,
             SOAPoutContainer,
             exportDatasetName,
             soapEngine,
             SOAPOutputChunkDim,
             SOAPnJobs,
             doOverride=doOverride,
-            verbose=verbose,
-            useType=useType,
         )
     else:
         raise ValueError("saponify: The input object is not a trajectory group.")
```

### Comparing `cpctools-0.1.0/SOAPify/utils.py` & `cpctools-0.1.0rc0/SOAPify/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Utilities submodule, cointains unclassified support functions
 Author: Daniele Rapetti"""
 from itertools import combinations_with_replacement
 import numpy
 from ase.data import atomic_numbers
-import h5py
 
 
 def _SOAPpstr(l, Z, n, Zp, np) -> str:
     if atomic_numbers[Z] < atomic_numbers[Zp]:
         Z, Zp = Zp, Z
         n, np = np, n
     return f"{l}_{Z}{n}_{Zp}{np}"
@@ -318,36 +317,7 @@
         return soapFromdscribe[:, indexes]
     if len(soapFromdscribe.shape) == 3:
         return soapFromdscribe[:, :, indexes]
 
     raise ValueError(
         "fillSOAPVectorFromdscribe: cannot convert array with len(shape) >=3"
     )
-
-
-def getSOAPSettings(fitsetData: h5py.Dataset) -> dict:
-    """Gets the settings of the SOAP calculation
-
-        you can feed directly this output to :func:`fillSOAPVectorFromdscribe`
-
-        #TODO: make tests for this
-    Args:
-        fitsetData (h5py.Dataset): A soap dataset with attributes
-
-    Returns:
-        dict: a dictionary with the following components:
-            - **nMax**
-            - **lMax**
-            - **atomTypes**
-            - **atomicSlices**
-
-    """
-    lmax = fitsetData.attrs["l_max"]
-    nmax = fitsetData.attrs["n_max"]
-    symbols, atomicSlices = getSlicesFromAttrs(fitsetData.attrs)
-
-    return {
-        "nMax": nmax,
-        "lMax": lmax,
-        "atomTypes": symbols,
-        "atomicSlices": atomicSlices,
-    }
```

### Comparing `cpctools-0.1.0/SOAPify/HDF5er/HDF5To.py` & `cpctools-0.1.0rc0/SOAPify/HDF5er/HDF5To.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,29 +315,28 @@
             the asked slice from wich create an universe.
             Defaults to slice(None).
 
     Returns:
         MDAnalysis.Universe:
             an universe containing the wnated part of the trajectory
     """
-    # TODO: also add a slice for the atoms
     traj = trajectoryGroup["Trajectory"]
     box = trajectoryGroup["Box"]
-    atomNames = trajectoryGroup["Types"].asstr()
+    # atomNames = trajectoryGroup["Types"].asstr()
     nAt = traj.shape[1]
     # TODO add names
     toRet = MDAnalysis.Universe.empty(
         n_atoms=nAt,
         n_residues=nAt,
         n_segments=1,
         atom_resindex=numpy.arange(nAt),
         residue_segindex=[1] * nAt,
         trajectory=True,
     )
-    toRet.add_TopologyAttr("type", atomNames)
+
     toRet.load_new(
         traj[useSlice],
         format=MDAnalysis.coordinates.memory.MemoryReader,
         dimensions=box[useSlice],
     )
 
     return toRet
```

### Comparing `cpctools-0.1.0/SOAPify/HDF5er/HDF5erUtils.py` & `cpctools-0.1.0rc0/SOAPify/HDF5er/HDF5erUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
         trajGroup (h5py.Group): the group to check
 
     Returns:
         bool: True if the group is a trajectory group, False otherwise
     """
 
     if (
-        isinstance(trajGroup, h5py.Group)
-        and "Trajectory" in trajGroup.keys()
+        "Trajectory" in trajGroup.keys()
         and "Types" in trajGroup.keys()
         and "Box" in trajGroup.keys()
     ):
         check = True
         for key in ["Trajectory", "Types", "Box"]:
             check &= isinstance(trajGroup[key], h5py.Dataset)
         return check
```

### Comparing `cpctools-0.1.0/SOAPify/HDF5er/ToHDF5.py` & `cpctools-0.1.0rc0/SOAPify/HDF5er/ToHDF5.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,55 +10,52 @@
 
 
 def universe2HDF5(
     mdaTrajectory: "mdaUniverse | mdaAtomGroup",
     trajFolder: h5py.Group,
     trajChunkSize: int = 100,
     trajslice: slice = slice(None),
-    useType="float64",
 ):
     """Uploads an mda.Universe or an mda.AtomGroup to a h5py.Group in an hdf5 file
 
     Args:
         MDAUniverseOrSelection (MDAnalysis.Universe or MDAnalysis.AtomGroup):
             the container with the trajectory data
         trajFolder (h5py.Group):
             the group in which store the trajectory in the hdf5 file
         trajChunkSize (int, optional):
             The desired dimension of the chunks of data that are stored in the hdf5 file.
             Defaults to 100.
-        useType (str,optional):
-            The precision used to store the data. Defaults to "float64".
     """
 
     atoms = mdaTrajectory.atoms
     universe = mdaTrajectory.universe
     nat = len(atoms)
-    useType = numpy.dtype(useType)
+
     if "Types" not in list(trajFolder.keys()):
         trajFolder.create_dataset("Types", (nat), compression="gzip", data=atoms.types)
 
     if "Trajectory" not in list(trajFolder.keys()):
         trajFolder.create_dataset(
             "Trajectory",
             (0, nat, 3),
             compression="gzip",
             chunks=(trajChunkSize, nat, 3),
             maxshape=(None, nat, 3),
-            dtype=useType,
+            dtype=numpy.float64,
         )
 
     if "Box" not in list(trajFolder.keys()):
         trajFolder.create_dataset(
             "Box",
             (0, 6),
             compression="gzip",
             chunks=True,
             maxshape=(None, 6),
-            dtype=useType,
+            dtype=numpy.float64,
         )
 
     frameNum = 0
     first = 0
     boxes = []
     atomicframes = []
     for _ in universe.trajectory[trajslice]:
@@ -81,15 +78,14 @@
     mdaTrajectory: "mdaUniverse | mdaAtomGroup",
     targetHDF5File: str,
     groupName: str,
     trajChunkSize: int = 100,
     override: bool = False,
     attrs: dict = None,
     trajslice: slice = slice(None),
-    useType="float64",
 ):
     """Creates an HDF5 trajectory groupfrom an mda trajectory
 
         Opens or creates the given HDF5 file, request the user's chosen group,
         then uploads an mda.Universe or an mda.AtomGroup to a h5py.Group in an
         hdf5 file
 
@@ -106,25 +102,22 @@
             `targetHDF5File`
         trajChunkSize (int, optional):
             The desired dimension of the chunks of data that are stored in the
             hdf5 file. Defaults to 100.
         override (bool, optional):
             If true the hdf5 file will be completely overwritten.
             Defaults to False.
-        useType (str,optional):
-            The precision used to store the data. Defaults to "float64".
     """
     with h5py.File(targetHDF5File, "w" if override else "a") as newTraj:
         trajGroup = newTraj.require_group(f"Trajectories/{groupName}")
         universe2HDF5(
             mdaTrajectory,
             trajGroup,
             trajChunkSize=trajChunkSize,
             trajslice=trajslice,
-            useType=useType,
         )
         if attrs:
             for key in attrs.keys():
                 trajGroup.attrs.create(key, attrs[key])
 
 
 @deprecated('xyz2hdf5Converter is "legacy code" **not covered by unit tests**')
```

### Comparing `cpctools-0.1.0/SOAPify/transitions/__init__.py` & `cpctools-0.1.0rc0/SOAPify/transitions/__init__.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/SOAPify/transitions/tracker.py` & `cpctools-0.1.0rc0/SOAPify/transitions/tracker.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/tests/conftest.py` & `cpctools-0.1.0rc0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,14 @@
 
 @pytest.fixture(
     scope="module",
     params=[
         slice(None, None, None),  # no slice
         slice(1, None, 2),  # classic slice
         [0, 4],  # list-like slice
-        [0],  # list-like slice - single atom
     ],
 )
 def input_framesSlice(request):
     return request.param
 
 
 @pytest.fixture(
@@ -324,15 +323,15 @@
 
     return confFile, groupName, nMol
 
 
 @pytest.fixture(scope="session")
 def referencesTrajectory(tmp_path_factory):
     """Creates a base hdf5file to be used in various tests"""
-    u = giveUniverse(repeatFrames=10)
+    u = giveUniverse()
 
     fname = tmp_path_factory.mktemp("trajBase") / f"trajBase.hdf5"
     groupname = "trajBase"
     HDF5er.MDA2HDF5(u, fname, groupname, override=True)
     return fname, groupname
```

### Comparing `cpctools-0.1.0/tests/testSupport.py` & `cpctools-0.1.0rc0/tests/testSupport.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,26 +204,23 @@
         bonds.extend([(o, o + 1), (o, o + 2)])
 
     sol.add_TopologyAttr("bonds", bonds)
 
     return sol
 
 
-def giveUniverse(
-    angles: set = (90.0, 90.0, 90.0), repeatFrames=1
-) -> MDAnalysis.Universe:
+def giveUniverse(angles: set = (90.0, 90.0, 90.0)) -> MDAnalysis.Universe:
     traj = numpy.array(
         [
             [[0.0, 0.0, 0.0], [1.0, 1.0, 1.0], [2.0, 2.0, 2.0], [3.0, 3.0, 3.0]],
             [[0.1, 0.1, 0.1], [1.1, 1.1, 1.1], [2.1, 2.1, 2.1], [3.1, 3.1, 3.1]],
             [[0.2, 0.2, 0.2], [1.2, 1.2, 1.2], [2.2, 2.2, 2.2], [3.2, 3.2, 3.2]],
             [[0.3, 0.3, 0.3], [1.3, 1.3, 1.3], [2.3, 2.3, 2.3], [3.3, 3.3, 3.3]],
             [[0.4, 0.4, 0.4], [1.4, 1.4, 1.4], [2.4, 2.4, 2.4], [3.4, 3.4, 3.4]],
         ]
-        * repeatFrames
     )
     u = MDAnalysis.Universe.empty(
         4, trajectory=True, atom_resindex=[0, 0, 0, 0], residue_segindex=[0]
     )
 
     u.add_TopologyAttr("type", ["H"] * 4)
     u.atoms.positions = traj[0]
```

### Comparing `cpctools-0.1.0/tests/test_HDF5er.py` & `cpctools-0.1.0rc0/tests/test_HDF5er.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-"""Test for HDF5er"""
 import SOAPify.HDF5er as HDF5er
 import h5py
 import numpy
 from numpy.testing import assert_array_almost_equal
 
 
 def test_istTrajectoryGroupCheck(tmp_path):
@@ -10,25 +9,18 @@
     # Given an HDF5 group
     with h5py.File(fname, "w") as hdf5test:
         group = hdf5test.create_group("Trajectories/4Atoms3Frames")
         # empty group
         assert not HDF5er.isTrajectoryGroup(group)
         group.create_dataset("Trajectory", data=numpy.zeros((5, 4, 3)))
         assert not HDF5er.isTrajectoryGroup(group)
-        assert not HDF5er.isTrajectoryGroup(group["Trajectory"])
-
         group.create_dataset("Types", data=numpy.zeros((4)))
         assert not HDF5er.isTrajectoryGroup(group)
-        assert not HDF5er.isTrajectoryGroup(group["Types"])
-
         group.create_dataset("Box", data=numpy.zeros((5, 3)))
-        # now group contains a Box. a Types and  and a Trajectory Datasets
         assert HDF5er.isTrajectoryGroup(group)
-        assert not HDF5er.isTrajectoryGroup(group["Box"])
-
     with h5py.File(fname, "w") as hdf5test:
         group = hdf5test.create_group("Trajectories/4Atoms3Frames")
         # empty group
         assert not HDF5er.isTrajectoryGroup(group)
         # now trajectory is set as a group
         group.create_group("Trajectory")
         group.create_dataset("Types", data=numpy.zeros((4)))
```

### Comparing `cpctools-0.1.0/tests/test_HDF5ertools.py` & `cpctools-0.1.0rc0/tests/test_HDF5ertools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import SOAPify.HDF5er as HDF5er
 import h5py
 import pytest
 import numpy
-from numpy.testing import assert_array_almost_equal, assert_array_equal
+from numpy.testing import assert_array_almost_equal
 from io import StringIO
 from .testSupport import (
     giveUniverse,
     giveUniverse_ChangingBox,
     checkStringDataFromUniverse,
     getUniverseWithWaterMolecules,
     checkStringDataFromHDF5,
@@ -348,9 +348,7 @@
         for frameTraj, frameBox, ts in zip(
             group["Trajectory"][input_framesSlice],
             group["Box"][input_framesSlice],
             newUniverse.trajectory,
         ):
             assert_array_almost_equal(frameTraj, newUniverse.atoms.positions)
             assert_array_almost_equal(frameBox, newUniverse.dimensions)
-
-        assert_array_equal(group["Types"].asstr(), newUniverse.atoms.types)
```

### Comparing `cpctools-0.1.0/tests/test_SOAPify.py` & `cpctools-0.1.0rc0/tests/test_SOAPify.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/tests/test_SOAPifyEngine.py` & `cpctools-0.1.0rc0/tests/test_SOAPifyEngine.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/tests/test_SOAPifySOAP.py` & `cpctools-0.1.0rc0/tests/test_SOAPifySOAP.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/tests/test_analysis.py` & `cpctools-0.1.0rc0/tests/test_analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,17 @@
 import pytest
 import SOAPify.analysis as analysis
 import SOAPify
 import h5py
 import MDAnalysis
 from .testSupport import is_sorted, fewFrameUniverse
 
-# NB: the trueFalse fixture for the backward settings is here to anticipate the
-# implementation of that feature
 
-
-@pytest.mark.parametrize("window", [1, 2, 5, 7, 10])
-@pytest.mark.parametrize("backward", [True, False])
-def test_timeSOAP(referencesTrajectorySOAP, window, backward):
+def test_tempoSOAP(referencesTrajectorySOAP, inputWindows):
+    window = inputWindows
     stride = window
     confFile, groupName = referencesTrajectorySOAP
 
     with h5py.File(confFile, "r") as f:
         t = f[f"/SOAP/{groupName}"]
         fillArgs = {
             "soapFromdscribe": t[:],
@@ -32,15 +28,17 @@
     def isInvalidCombination(dataLen, stride, window):
         return (stride is not None and window < stride) or (
             (stride is not None and stride >= dataLen) or window >= dataLen
         )
 
     if isInvalidCombination(fillArgs["soapFromdscribe"].shape[0], stride, window):
         with pytest.raises(ValueError) as excinfo:
-            analysis.timeSOAP(fillArgs["soapFromdscribe"], stride=stride, window=window)
+            analysis.tempoSOAP(
+                fillArgs["soapFromdscribe"], stride=stride, window=window
+            )
         if stride is not None and window < stride:
             assert "window must be bigger" in str(excinfo.value)
             pytest.skip("Exception thrown correctly")
         if (
             stride is not None and stride >= fillArgs["soapFromdscribe"].shape[0]
         ) or window >= fillArgs["soapFromdscribe"].shape[0]:
             assert "window must be smaller" in str(excinfo.value)
@@ -56,93 +54,34 @@
     expectedTimedSOAP = numpy.zeros((SOAPTraj.shape[0] - window, SOAPTraj.shape[1]))
 
     for frame in range(window, SOAPTraj.shape[0]):
         for molecule in range(0, SOAPTraj.shape[1]):
             x = SOAPTraj[frame, molecule, :]
             y = SOAPTraj[frame - window, molecule, :]
             distance = SOAPify.simpleSOAPdistance(x, y)
-            # TODO:
-            # if backward:
-            # else:
             expectedTimedSOAP[
                 frame - window, molecule
             ] = distance  # fill the matrix (each molecule for each frame)
 
     expectedDeltaTimedSOAP = []
     for molecule in range(0, expectedTimedSOAP.shape[1]):
         derivative = numpy.diff(expectedTimedSOAP[:, molecule])
         expectedDeltaTimedSOAP.append(derivative)
 
-    timedSOAP, deltaTimedSOAP = analysis.timeSOAP(
-        SOAPTraj, stride=stride, window=window, backward=backward
-    )
-    # print(timedSOAP, expectedTimedSOAP)
-    print(deltaTimedSOAP.shape, timedSOAP.shape)
-    print(
-        numpy.asarray(expectedDeltaTimedSOAP).shape,
-        numpy.asarray(expectedTimedSOAP).shape,
-    )
-    assert_array_almost_equal(timedSOAP, expectedTimedSOAP)
-
-    assert_array_almost_equal(deltaTimedSOAP, expectedDeltaTimedSOAP)
-
-
-@pytest.mark.parametrize("window", [1, 2, 5, 7, 10])
-@pytest.mark.parametrize("backward", [True, False])
-def test_timeSOAPsimple(referencesTrajectorySOAP, window, backward):
-    stride = window
-    confFile, groupName = referencesTrajectorySOAP
-
-    with h5py.File(confFile, "r") as f:
-        t = f[f"/SOAP/{groupName}"]
-        fillArgs = {
-            "soapFromdscribe": t[:],
-            "lMax": t.attrs["l_max"],
-            "nMax": t.attrs["n_max"],
-        }
-        fillArgs["atomTypes"], fillArgs["atomicSlices"] = SOAPify.getSlicesFromAttrs(
-            t.attrs
-        )
-
-    def isInvalidCombination(dataLen, stride, window):
-        return (stride is not None and window < stride) or (
-            (stride is not None and stride >= dataLen) or window >= dataLen
-        )
-
-    if isInvalidCombination(fillArgs["soapFromdscribe"].shape[0], stride, window):
-        with pytest.raises(ValueError) as excinfo:
-            analysis.timeSOAP(fillArgs["soapFromdscribe"], stride=stride, window=window)
-        if stride is not None and window < stride:
-            assert "window must be bigger" in str(excinfo.value)
-            pytest.skip("Exception thrown correctly")
-        if (
-            stride is not None and stride >= fillArgs["soapFromdscribe"].shape[0]
-        ) or window >= fillArgs["soapFromdscribe"].shape[0]:
-            assert "window must be smaller" in str(excinfo.value)
-            pytest.skip("Exception thrown correctly")
-
-    SOAPTraj = SOAPify.fillSOAPVectorFromdscribe(**fillArgs)
-
-    SOAPTraj = SOAPify.normalizeArray(SOAPTraj)
-
-    expectedTimedSOAP, expectedDeltaTimedSOAP = analysis.timeSOAP(
-        SOAPTraj, stride=stride, window=window, backward=backward
-    )
-    timedSOAP, deltaTimedSOAP = analysis.timeSOAPsimple(
-        SOAPTraj, stride=stride, window=window, backward=backward
+    timedSOAP, deltaTimedSOAP = analysis.tempoSOAP(
+        SOAPTraj, stride=stride, window=window
     )
     print(timedSOAP, expectedTimedSOAP)
     assert_array_almost_equal(timedSOAP, expectedTimedSOAP)
 
     assert_array_almost_equal(deltaTimedSOAP, expectedDeltaTimedSOAP)
 
 
-@pytest.mark.parametrize("window", [1, 2, 5, 7, 10])
-@pytest.mark.parametrize("backward", [True, False])
-def test_getTimeSOAPsimple(referencesTrajectorySOAP, window, backward):
+def test_tempoSOAPsimple(referencesTrajectorySOAP, inputWindows):
+    window = inputWindows
     stride = window
     confFile, groupName = referencesTrajectorySOAP
 
     with h5py.File(confFile, "r") as f:
         t = f[f"/SOAP/{groupName}"]
         fillArgs = {
             "soapFromdscribe": t[:],
@@ -156,35 +95,36 @@
     def isInvalidCombination(dataLen, stride, window):
         return (stride is not None and window < stride) or (
             (stride is not None and stride >= dataLen) or window >= dataLen
         )
 
     if isInvalidCombination(fillArgs["soapFromdscribe"].shape[0], stride, window):
         with pytest.raises(ValueError) as excinfo:
-            analysis.timeSOAP(fillArgs["soapFromdscribe"], stride=stride, window=window)
+            analysis.tempoSOAP(
+                fillArgs["soapFromdscribe"], stride=stride, window=window
+            )
         if stride is not None and window < stride:
             assert "window must be bigger" in str(excinfo.value)
             pytest.skip("Exception thrown correctly")
         if (
             stride is not None and stride >= fillArgs["soapFromdscribe"].shape[0]
         ) or window >= fillArgs["soapFromdscribe"].shape[0]:
             assert "window must be smaller" in str(excinfo.value)
             pytest.skip("Exception thrown correctly")
 
     SOAPTraj = SOAPify.fillSOAPVectorFromdscribe(**fillArgs)
 
     SOAPTraj = SOAPify.normalizeArray(SOAPTraj)
 
-    expectedTimedSOAP, expectedDeltaTimedSOAP = analysis.timeSOAPsimple(
-        SOAPTraj, stride=stride, window=window, backward=backward
+    expectedTimedSOAP, expectedDeltaTimedSOAP = analysis.tempoSOAP(
+        SOAPTraj, stride=stride, window=window
+    )
+    timedSOAP, deltaTimedSOAP = analysis.tempoSOAPsimple(
+        SOAPTraj, stride=stride, window=window
     )
-    with h5py.File(confFile, "r") as f:
-        timedSOAP, deltaTimedSOAP = analysis.getTimeSOAPSimple(
-            f[f"/SOAP/{groupName}"], stride=stride, window=window, backward=backward
-        )
     print(timedSOAP, expectedTimedSOAP)
     assert_array_almost_equal(timedSOAP, expectedTimedSOAP)
 
     assert_array_almost_equal(deltaTimedSOAP, expectedDeltaTimedSOAP)
 
 
 @pytest.fixture(
```

### Comparing `cpctools-0.1.0/tests/test_classification.py` & `cpctools-0.1.0rc0/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/tests/test_transitions/test_tracker.py` & `cpctools-0.1.0rc0/tests/test_transitions/test_tracker.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/tests/test_transitions/test_transitions.py` & `cpctools-0.1.0rc0/tests/test_transitions/test_transitions.py`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/.gitignore` & `cpctools-0.1.0rc0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 *_script.py
 *.hdf5
 *.data
 *.bak
 *.png
 *.csv
 *.xyz
-*.lammpsdump
-*.zip*
 test.py
 log.lammps
 .vscode
 refSave.hdf5
 .secrets
 
 # Byte-compiled / optimized / DLL files
```

### Comparing `cpctools-0.1.0/LICENSE` & `cpctools-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/Readme.md` & `cpctools-0.1.0rc0/Readme.md`

 * *Files identical despite different names*

### Comparing `cpctools-0.1.0/pyproject.toml` & `cpctools-0.1.0rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 docs = [
     "sphinx<6,>=4",
     "docutils<0.18",
     "sphinx-rtd-theme==1.2.0",
     "myst-parser==0.18.1",
     "sphinx-autodoc-typehints==1.22",
     "nbsphinx==0.9.0",
-    "sphinx_gallery==0.12.2",
-    "ipython"
+    "sphinx_gallery==0.12.2"
 ]
 dscribe=["dscribe >1.2.0, <=12.2",]
 quippy=["quippy-ase==0.9.10",]
 tests = [
     "coverage[toml]",
     "pytest",
     "pytest-cov",
@@ -50,17 +49,16 @@
 Homepage = "https://github.com/GMPavanLab/SOAPify"
 Documentation = "https://gmpavanlab.github.io/SOAPify/"
 ReadTheDocs = "https://soapify.readthedocs.io/en/latest/"
 Issues = "https://github.com/GMPavanLab/SOAPify/issues"
 Source = "https://github.com/GMPavanLab/SOAPify"
 
 #TODO: define some cli scripts that can be useful!
-[project.scripts]
-SOAPify-prepareTrajectory = "SOAPify.cli:createTrajectory"
-SOAPify-traj2SOAP = "SOAPify.cli:traj2SOAP"
+#[project.scripts]
+#cli-name = "pkg.subpkg:func"
 
 [tool.hatch.version]
 path = "src/SOAPify/__init__.py"
 
 
 [tool.hatch.build]
 sources = ["src"]
```

### Comparing `cpctools-0.1.0/PKG-INFO` & `cpctools-0.1.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpctools
-Version: 0.1.0
+Version: 0.1.0rc0
 Summary: A package for creating and studying SOAP fingerprints
 Project-URL: Homepage, https://github.com/GMPavanLab/SOAPify
 Project-URL: Documentation, https://gmpavanlab.github.io/SOAPify/
 Project-URL: ReadTheDocs, https://soapify.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/GMPavanLab/SOAPify/issues
 Project-URL: Source, https://github.com/GMPavanLab/SOAPify
 Author-email: Daniele Rapetti <daniele.rapetti@polito.it>
@@ -20,15 +20,14 @@
 Requires-Dist: ase==3.22.1
 Requires-Dist: deprecated==1.2.13
 Requires-Dist: h5py==3.8.0
 Requires-Dist: mdanalysis==2.4.2
 Requires-Dist: numpy<1.24,>=1.18
 Provides-Extra: docs
 Requires-Dist: docutils<0.18; extra == 'docs'
-Requires-Dist: ipython; extra == 'docs'
 Requires-Dist: myst-parser==0.18.1; extra == 'docs'
 Requires-Dist: nbsphinx==0.9.0; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints==1.22; extra == 'docs'
 Requires-Dist: sphinx-gallery==0.12.2; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme==1.2.0; extra == 'docs'
 Requires-Dist: sphinx<6,>=4; extra == 'docs'
 Provides-Extra: dscribe
```

