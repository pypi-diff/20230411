# Comparing `tmp/simpleimageio-1.2.0.tar.gz` & `tmp/simpleimageio-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleimageio-1.2.0.tar", last modified: Thu Jan 12 13:56:54 2023, max compression
+gzip compressed data, was "simpleimageio-1.3.0.tar", last modified: Tue Apr 11 18:26:31 2023, max compression
```

## Comparing `simpleimageio-1.2.0.tar` & `simpleimageio-1.3.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:56:54.987461 simpleimageio-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:56:54.983461 simpleimageio-1.2.0/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:56:54.987461 simpleimageio-1.2.0/Core/External/
--rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/fpng.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/fpng.h
--rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/miniz.c
--rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/miniz.h
--rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/stb_image.h
--rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/stb_image_write.h
--rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/tiny_dng_loader.h
--rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/tiny_dng_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/External/tinyexr.h
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/error_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/filter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/image.h
--rw-r--r--   0 runner    (1001) docker     (123)    33647 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/imageio.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/manipulation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/tonemapping.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/Core/vec3.h
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-01-12 13:56:54.987461 simpleimageio-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:56:54.983461 simpleimageio-1.2.0/PyWrapper/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:56:54.987461 simpleimageio-1.2.0/PyWrapper/simpleimageio/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/corelib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/error_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/imageViewer.js
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/manip.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/tev.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/PyWrapper/simpleimageio/tonemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 13:56:54.987461 simpleimageio-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-01-12 13:56:28.000000 simpleimageio-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:56:54.987461 simpleimageio-1.2.0/simpleimageio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-01-12 13:56:54.000000 simpleimageio-1.2.0/simpleimageio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-01-12 13:56:54.000000 simpleimageio-1.2.0/simpleimageio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 13:56:54.000000 simpleimageio-1.2.0/simpleimageio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-12 13:56:54.000000 simpleimageio-1.2.0/simpleimageio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-12 13:56:54.000000 simpleimageio-1.2.0/simpleimageio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.339984 simpleimageio-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.331983 simpleimageio-1.3.0/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.335984 simpleimageio-1.3.0/Core/External/
+-rw-r--r--   0 runner    (1001) docker     (123)   114725 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/fpng.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/fpng.h
+-rw-r--r--   0 runner    (1001) docker     (123)   319839 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/miniz.c
+-rw-r--r--   0 runner    (1001) docker     (123)    69441 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/miniz.h
+-rw-r--r--   0 runner    (1001) docker     (123)   273149 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/stb_image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    69564 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/stb_image_write.h
+-rw-r--r--   0 runner    (1001) docker     (123)   163059 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/tiny_dng_loader.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/tiny_dng_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)   269883 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/External/tinyexr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/error_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11082 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/filter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/image.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33227 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/imageio.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/manipulation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/tonemapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/Core/vec3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-11 18:26:27.000000 simpleimageio-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-11 18:26:31.335984 simpleimageio-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.331983 simpleimageio-1.3.0/PyWrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.335984 simpleimageio-1.3.0/PyWrapper/simpleimageio/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/corelib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/error_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36113 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/imageViewer.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89794 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/jquery-3.6.4.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/manip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/tev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/PyWrapper/simpleimageio/tonemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:26:31.339984 simpleimageio-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-11 18:26:28.000000 simpleimageio-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:26:31.335984 simpleimageio-1.3.0/simpleimageio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 18:26:31.000000 simpleimageio-1.3.0/simpleimageio.egg-info/top_level.txt
```

### Comparing `simpleimageio-1.2.0/Core/CMakeLists.txt` & `simpleimageio-1.3.0/Core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/fpng.cpp` & `simpleimageio-1.3.0/Core/External/fpng.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/fpng.h` & `simpleimageio-1.3.0/Core/External/fpng.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/miniz.c` & `simpleimageio-1.3.0/Core/External/miniz.c`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/miniz.h` & `simpleimageio-1.3.0/Core/External/miniz.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/stb_image.h` & `simpleimageio-1.3.0/Core/External/stb_image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/stb_image_write.h` & `simpleimageio-1.3.0/Core/External/stb_image_write.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/tiny_dng_loader.h` & `simpleimageio-1.3.0/Core/External/tiny_dng_loader.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/tiny_dng_writer.h` & `simpleimageio-1.3.0/Core/External/tiny_dng_writer.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/External/tinyexr.h` & `simpleimageio-1.3.0/Core/External/tinyexr.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/error_metrics.cpp` & `simpleimageio-1.3.0/Core/error_metrics.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/filter.cpp` & `simpleimageio-1.3.0/Core/filter.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/image.h` & `simpleimageio-1.3.0/Core/image.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/imageio.cpp` & `simpleimageio-1.3.0/Core/imageio.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -291,100 +291,97 @@
     for (int i = 0; i < numLayers; ++i) totalChannels += numChannels[i];
 
     header.num_channels = totalChannels;
     image.num_channels = totalChannels;
     image.width = width;
     image.height = height;
 
-    // Sort the layer names in ASCII byte order because OpenEXR demands it so
-    std::vector<int> layerIndices;
-    for (int i = 0; i < numLayers; ++i) layerIndices.push_back(i);
-    std::sort(layerIndices.begin(), layerIndices.end(), [layerNames] (int a, int b) {
-        if (layerNames[a] == nullptr) {
-            if (layerNames[b] == nullptr) return false;
-            else return true;
-        }
-        else if (layerNames[b] == nullptr) return false;
-
-        return strcmp(layerNames[a], layerNames[b]) < 0;
-    });
-
     // Convert image data from AoS to SoA (i.e. one image per channel in each layer)
     std::vector<std::vector<float>> channelImages;
-    float** imagePtr = (float **) alloca(sizeof(float*) * image.num_channels);
     for (int layer = 0; layer < numLayers; ++layer) {
-        for (int chan = 0; chan < numChannels[layerIndices[layer]]; ++chan) {
+        for (int chan = 0; chan < numChannels[layer]; ++chan) {
             channelImages.emplace_back(width * height);
         }
 
-        size_t offset = channelImages.size() - numChannels[layerIndices[layer]];
+        size_t offset = channelImages.size() - numChannels[layer];
         for (int r = 0; r < height; ++r) {
             for (int c = 0; c < width; ++c) {
-                auto start = r * rowStrides[layerIndices[layer]] + c * numChannels[layerIndices[layer]];
-                for (int chan = 0; chan < numChannels[layerIndices[layer]]; ++chan) {
-                    channelImages[offset + chan][r * width + c] = layers[layerIndices[layer]][start + chan];
-
-                    // reverse channel order from RGB(A) to (A)BGR
-                    imagePtr[offset + numChannels[layerIndices[layer]] - chan - 1] = channelImages[offset + chan].data();
+                auto start = r * rowStrides[layer] + c * numChannels[layer];
+                for (int chan = 0; chan < numChannels[layer]; ++chan) {
+                    channelImages[offset + chan][r * width + c] = layers[layer][start + chan];
                 }
             }
         }
     }
-    image.images = (unsigned char**)imagePtr;
 
     // Set the channel names
-    std::vector<EXRChannelInfo> channels(header.num_channels);
-    header.channels = channels.data();
+    std::vector<EXRChannelInfo> channels(totalChannels);
     int offset = 0;
     for (int lay = 0; lay < numLayers; ++lay) {
         char namePrefix[256];
         size_t prefixLen = 0;
-        if (!layerNames || !layerNames[layerIndices[lay]] || layerNames[layerIndices[lay]][0] == 0) {
+        if (!layerNames || !layerNames[lay] || layerNames[lay][0] == 0) {
             prefixLen = 0;
             namePrefix[0] = 0;
         } else {
-            prefixLen = strlen(layerNames[layerIndices[lay]]) + 1;
-            strncpy(namePrefix, layerNames[layerIndices[lay]], 255);
+            prefixLen = strlen(layerNames[lay]) + 1;
+            strncpy(namePrefix, layerNames[lay], 255);
             namePrefix[prefixLen - 1] = '.';
         }
 
-        if (numChannels[layerIndices[lay]] == 1) {
-            strncpy(header.channels[offset + 0].name, namePrefix, 255);
-            strncpy(header.channels[offset + 0].name + prefixLen, "Y", 255 - prefixLen);
-        } else if (numChannels[layerIndices[lay]] == 3) {
-            strncpy(header.channels[offset + 0].name, namePrefix, 255);
-            strncpy(header.channels[offset + 0].name + prefixLen, "B", 255 - prefixLen);
-
-            strncpy(header.channels[offset + 1].name, namePrefix, 255);
-            strncpy(header.channels[offset + 1].name + prefixLen, "G", 255 - prefixLen);
-
-            strncpy(header.channels[offset + 2].name, namePrefix, 255);
-            strncpy(header.channels[offset + 2].name + prefixLen, "R", 255 - prefixLen);
-        } else if (numChannels[layerIndices[lay]] == 4) {
-            strncpy(header.channels[offset + 0].name, namePrefix, 255);
-            strncpy(header.channels[offset + 0].name + prefixLen, "A", 255 - prefixLen);
+        if (numChannels[lay] == 1) {
+            strncpy(channels[offset + 0].name, namePrefix, 255);
+            strncpy(channels[offset + 0].name + prefixLen, "Y", 255 - prefixLen);
+        } else if (numChannels[lay] == 3) {
+            strncpy(channels[offset + 0].name, namePrefix, 255);
+            strncpy(channels[offset + 0].name + prefixLen, "R", 255 - prefixLen);
+
+            strncpy(channels[offset + 1].name, namePrefix, 255);
+            strncpy(channels[offset + 1].name + prefixLen, "G", 255 - prefixLen);
+
+            strncpy(channels[offset + 2].name, namePrefix, 255);
+            strncpy(channels[offset + 2].name + prefixLen, "B", 255 - prefixLen);
+        } else if (numChannels[lay] == 4) {
+            strncpy(channels[offset + 0].name, namePrefix, 255);
+            strncpy(channels[offset + 0].name + prefixLen, "R", 255 - prefixLen);
 
-            strncpy(header.channels[offset + 1].name, namePrefix, 255);
-            strncpy(header.channels[offset + 1].name + prefixLen, "B", 255 - prefixLen);
+            strncpy(channels[offset + 1].name, namePrefix, 255);
+            strncpy(channels[offset + 1].name + prefixLen, "G", 255 - prefixLen);
 
-            strncpy(header.channels[offset + 2].name, namePrefix, 255);
-            strncpy(header.channels[offset + 2].name + prefixLen, "G", 255 - prefixLen);
+            strncpy(channels[offset + 2].name, namePrefix, 255);
+            strncpy(channels[offset + 2].name + prefixLen, "B", 255 - prefixLen);
 
-            strncpy(header.channels[offset + 3].name, namePrefix, 255);
-            strncpy(header.channels[offset + 3].name + prefixLen, "R", 255 - prefixLen);
+            strncpy(channels[offset + 3].name, namePrefix, 255);
+            strncpy(channels[offset + 3].name + prefixLen, "A", 255 - prefixLen);
         } else {
             std::cerr << "ERROR while writing " << filename
                     << ": images with " << numChannels << " channels are currently not supported. "
                     << "no file has been written." << std::endl;
             return;
         }
 
-        offset += numChannels[layerIndices[lay]];
+        offset += numChannels[lay];
     }
 
+    // Sort channels by the ASCII byte code of their names because thats what OpenEXR expects
+    std::vector<int> channelIndices;
+    for (int i = 0; i < totalChannels; ++i) channelIndices.emplace_back(i);
+    std::sort(channelIndices.begin(), channelIndices.end(), [&channels] (int a, int b) {
+        return strcmp(channels[a].name, channels[b].name) < 0;
+    });
+
+    std::vector<EXRChannelInfo> sortedChannels(totalChannels);
+    float** imagePtr = (float **) alloca(sizeof(float*) * image.num_channels);
+    for (int i = 0; i < totalChannels; ++i) {
+        sortedChannels[i] = channels[channelIndices[i]];
+        imagePtr[i] = channelImages[channelIndices[i]].data();
+    }
+    header.channels = sortedChannels.data();
+    image.images = (unsigned char**)imagePtr;
+
     // Define pixel type of the buffer and requested output pixel type in the file
     header.pixel_types = (int*) alloca(sizeof(int) * header.num_channels);
     header.requested_pixel_types = (int*) alloca(sizeof(int) * header.num_channels);
     for (int i = 0; i < header.num_channels; i++) {
         // From float to float
         header.pixel_types[i] = TINYEXR_PIXELTYPE_FLOAT;
         header.requested_pixel_types[i] = TINYEXR_PIXELTYPE_FLOAT;
```

### Comparing `simpleimageio-1.2.0/Core/manipulation.cpp` & `simpleimageio-1.3.0/Core/manipulation.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/tonemapping.cpp` & `simpleimageio-1.3.0/Core/tonemapping.cpp`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/Core/vec3.h` & `simpleimageio-1.3.0/Core/vec3.h`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/LICENSE` & `simpleimageio-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/PKG-INFO` & `simpleimageio-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.2.0
+Version: 1.3.0
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.2.0 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.0 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
```

### Comparing `simpleimageio-1.2.0/PyWrapper/simpleimageio/corelib.py` & `simpleimageio-1.3.0/PyWrapper/simpleimageio/corelib.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/PyWrapper/simpleimageio/error_metrics.py` & `simpleimageio-1.3.0/PyWrapper/simpleimageio/error_metrics.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/PyWrapper/simpleimageio/image.py` & `simpleimageio-1.3.0/PyWrapper/simpleimageio/image.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/PyWrapper/simpleimageio/manip.py` & `simpleimageio-1.3.0/PyWrapper/simpleimageio/manip.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/PyWrapper/simpleimageio/tev.py` & `simpleimageio-1.3.0/PyWrapper/simpleimageio/tev.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/PyWrapper/simpleimageio/tonemap.py` & `simpleimageio-1.3.0/PyWrapper/simpleimageio/tonemap.py`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/README.md` & `simpleimageio-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `simpleimageio-1.2.0/setup.py` & `simpleimageio-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         os.chdir(str(cwd))
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='simpleimageio',
-    version='1.2.0',
+    version='1.3.0',
     author='Pascal Grittmann',
     url='https://github.com/pgrit/SimpleImageIO',
 
     description='A very simple Python wrapper to read and write various HDR and LDR image file formats.',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `simpleimageio-1.2.0/simpleimageio.egg-info/PKG-INFO` & `simpleimageio-1.3.0/simpleimageio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleimageio
-Version: 1.2.0
+Version: 1.3.0
 Summary: A very simple Python wrapper to read and write various HDR and LDR image file formats.
 Home-page: https://github.com/pgrit/SimpleImageIO
 Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simpleimageio Version: 1.2.0 Summary: A very simple
+Metadata-Version: 2.1 Name: simpleimageio Version: 1.3.0 Summary: A very simple
 Python wrapper to read and write various HDR and LDR image file formats. Home-
 page: https://github.com/pgrit/SimpleImageIO Author: Pascal Grittmann
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE ![Build](https://github.com/pgrit/SimpleImageIO/workflows/Build/
 badge.svg) [https://buildstats.info/nuget/SimpleImageIO] # Simple Image IO A
```

### Comparing `simpleimageio-1.2.0/simpleimageio.egg-info/SOURCES.txt` & `simpleimageio-1.3.0/simpleimageio.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 Core/External/tinyexr.h
 PyWrapper/simpleimageio/__init__.py
 PyWrapper/simpleimageio/corelib.py
 PyWrapper/simpleimageio/error_metrics.py
 PyWrapper/simpleimageio/flip.py
 PyWrapper/simpleimageio/image.py
 PyWrapper/simpleimageio/imageViewer.js
+PyWrapper/simpleimageio/jquery-3.6.4.min.js
 PyWrapper/simpleimageio/manip.py
 PyWrapper/simpleimageio/style.css
 PyWrapper/simpleimageio/tev.py
 PyWrapper/simpleimageio/tonemap.py
 simpleimageio.egg-info/PKG-INFO
 simpleimageio.egg-info/SOURCES.txt
 simpleimageio.egg-info/dependency_links.txt
```

