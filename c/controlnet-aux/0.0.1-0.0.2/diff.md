# Comparing `tmp/controlnet_aux-0.0.1.tar.gz` & `tmp/controlnet_aux-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/controlnet_aux-0.0.1.tar", last modified: Thu Mar  2 14:37:07 2023, max compression
+gzip compressed data, was "controlnet_aux-0.0.2.tar", last modified: Tue Apr 11 17:36:28 2023, max compression
```

## Comparing `controlnet_aux-0.0.1.tar` & `controlnet_aux-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,45 @@
-drwxr-xr-x   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     1187 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/PKG-INFO
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)      232 2023-03-02 14:33:46.000000 controlnet_aux-0.0.1/README.md
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)       38 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/setup.cfg
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     8478 2023-03-02 14:31:26.000000 controlnet_aux-0.0.1/setup.py
-drwxr-xr-x   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/
-drwxr-xr-x   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)      123 2023-03-02 14:35:45.000000 controlnet_aux-0.0.1/src/controlnet_aux/__init__.py
-drwxr-xr-x   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/hed/
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     7549 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/hed/__init__.py
-drwxr-xr-x   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/mlsd/
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     1989 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/mlsd/__init__.py
-drwxr-xr-x   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/mlsd/models/
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/mlsd/models/__init__.py
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     9678 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     9180 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)    24134 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/mlsd/utils.py
-drwxr-xr-x   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/open_pose/
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     3119 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/open_pose/__init__.py
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)    10909 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/open_pose/body.py
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     3389 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/open_pose/hand.py
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     8743 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/open_pose/model.py
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     8387 2023-03-02 14:31:07.000000 controlnet_aux-0.0.1/src/controlnet_aux/open_pose/util.py
-drwxr-xr-x   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        0 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux.egg-info/
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)     1187 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux.egg-info/PKG-INFO
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)      694 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux.egg-info/SOURCES.txt
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)        1 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux.egg-info/dependency_links.txt
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)       90 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux.egg-info/requires.txt
--rw-r--r--   0 patrick_huggingface_co (771153978) patrick_huggingface_co (771153978)       15 2023-03-02 14:37:07.000000 controlnet_aux-0.0.1/src/controlnet_aux.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1574 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      670 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/README.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8604 2023-04-11 17:33:24.000000 controlnet_aux-0.0.2/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.839497 controlnet_aux-0.0.2/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      189 2023-04-11 17:23:50.000000 controlnet_aux-0.0.2/src/controlnet_aux/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/canny/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      502 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/canny/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/hed/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7586 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/hed/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2272 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/api.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/blocks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/dpt_depth.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/midas_net.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/midas/vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/midas/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2026 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    24134 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/mlsd/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3156 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10883 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/body.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3389 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/hand.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8387 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/open_pose/util.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3742 2023-04-11 17:22:02.000000 controlnet_aux-0.0.2/src/controlnet_aux/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:36:28.843497 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1574 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1212 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      107 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-04-11 17:36:28.000000 controlnet_aux-0.0.2/src/controlnet_aux.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `controlnet_aux-0.0.1/setup.py` & `controlnet_aux-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,38 +69,41 @@
 
 import os
 import re
 from distutils.core import Command
 
 from setuptools import find_packages, setup
 
-
 # IMPORTANT:
 # 1. all dependencies should be listed here with their version requirements if any
 # 2. once modified, run: `make deps_table_update` to update src/diffusers/dependency_versions_table.py
 _deps = [
     "Pillow",
     "torch",
     "numpy",
     "filelock",
     "importlib_metadata",
     "opencv-python",
     "matplotlib",
     "scipy",
     "huggingface_hub",
-    "einops"
+    "einops",
+    "timm",
+    "torchvision"
 ]
 
 # this is a lookup table with items like:
 #
 # tokenizers: "huggingface-hub==0.8.0"
 # packaging: "packaging"
 #
 # some of the values are versioned whereas others aren't.
-deps = {b: a for a, b in (re.findall(r"^(([^!=<>~]+)(?:[!=<>~].*)?$)", x)[0] for x in _deps)}
+deps = {
+    b: a for a, b in (re.findall(r"^(([^!=<>~]+)(?:[!=<>~].*)?$)", x)[0] for x in _deps)
+}
 
 # since we save this data in src/diffusers/dependency_versions_table.py it can be easily accessed from
 # anywhere. If you need to quickly access the data from this table in a shell, you can do so easily with:
 #
 # python -c 'import sys; from diffusers.dependency_versions_table import deps; \
 # print(" ".join([ deps[x] for x in sys.argv[1:]]))' tokenizers datasets
 #
@@ -124,15 +127,19 @@
     A custom distutils command that updates the dependency table.
     usage: python setup.py deps_table_update
     """
 
     description = "build runtime dependency table"
     user_options = [
         # format: (long option, short option, description).
-        ("dep-table-update", None, "updates src/diffusers/dependency_versions_table.py"),
+        (
+            "dep-table-update",
+            None,
+            "updates src/diffusers/dependency_versions_table.py",
+        ),
     ]
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
@@ -165,19 +172,21 @@
     deps["huggingface_hub"],
     deps["scipy"],
     deps["opencv-python"],
     deps["filelock"],
     deps["numpy"],
     deps["Pillow"],
     deps["einops"],
+    deps["torchvision"],
+    deps["timm"],
 ]
 
 setup(
     name="controlnet_aux",
-    version="0.0.1",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.0.2",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Human Pose",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
```

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/hed/__init__.py` & `controlnet_aux-0.0.2/src/controlnet_aux/hed/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,17 +95,17 @@
 
 
 class HEDdetector:
     def __init__(self, netNetwork):
         self.netNetwork = netNetwork.eval()
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         filename = filename or "annotator/ckpts/network-bsds500.pth"
-        model_path = hf_hub_download(pretrained_model_or_path, filename)
+        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         netNetwork = Network(model_path)
 
         return cls(netNetwork)
 
     def __call__(self, input_image, detect_resolution=512, image_resolution=512, return_pil=True, scribble=False):
         device = next(iter(self.netNetwork.parameters())).device
```

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/mlsd/__init__.py` & `controlnet_aux-0.0.2/src/controlnet_aux/mlsd/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 
 class MLSDdetector:
     def __init__(self, model):
         self.model = model.eval()
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         filename = filename or "annotator/ckpts/mlsd_large_512_fp32.pth"
-        model_path = hf_hub_download(pretrained_model_or_path, filename)
+        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         model = MobileV2_MLSD_Large()
         model.load_state_dict(torch.load(model_path), strict=True)
 
         return cls(model)
 
     def __call__(self, input_image, thr_v=0.1, thr_d=0.1, detect_resolution=512, image_resolution=512, return_pil=True):
```

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `controlnet_aux-0.0.2/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/mlsd/utils.py` & `controlnet_aux-0.0.2/src/controlnet_aux/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/open_pose/__init__.py` & `controlnet_aux-0.0.2/src/controlnet_aux/open_pose/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
             # load_file_from_url(hand_model_path, model_dir=annotator_ckpts_path)
 
         # self.body_estimation = Body(body_modelpath)
         # self.hand_estimation = Hand(hand_modelpath)
         self.body_estimation = body_estimation
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         filename = filename or "annotator/ckpts/body_pose_model.pth"
-        body_model_path = hf_hub_download(pretrained_model_or_path, filename)
+        body_model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         body_estimation = Body(body_model_path)
 
         return cls(body_estimation)
 
     def __call__(self, input_image, detect_resolution=512, image_resolution=512, return_pil=True):
         # hand = False
```

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/open_pose/body.py` & `controlnet_aux-0.0.2/src/controlnet_aux/open_pose/body.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from .model import bodypose_model
 
 class Body(object):
     def __init__(self, model_path):
         self.model = bodypose_model()
         if torch.cuda.is_available():
             self.model = self.model.cuda()
-            print('cuda')
         model_dict = util.transfer(self.model, torch.load(model_path))
         self.model.load_state_dict(model_dict)
         self.model.eval()
 
     def __call__(self, oriImg):
         # scale_search = [0.5, 1.0, 1.5, 2.0]
         scale_search = [0.5]
```

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/open_pose/hand.py` & `controlnet_aux-0.0.2/src/controlnet_aux/open_pose/hand.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/open_pose/model.py` & `controlnet_aux-0.0.2/src/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.1/src/controlnet_aux/open_pose/util.py` & `controlnet_aux-0.0.2/src/controlnet_aux/open_pose/util.py`

 * *Files identical despite different names*

