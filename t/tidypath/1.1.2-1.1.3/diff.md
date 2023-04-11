# Comparing `tmp/tidypath-1.1.2.tar.gz` & `tmp/tidypath-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.1.2.tar", last modified: Tue Apr 11 18:33:03 2023, max compression
+gzip compressed data, was "tidypath-1.1.3.tar", last modified: Tue Apr 11 21:39:48 2023, max compression
```

## Comparing `tidypath-1.1.2.tar` & `tidypath-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 18:33:03.442506 tidypath-1.1.2/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2022-11-08 08:37:56.000000 tidypath-1.1.2/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-04-11 18:33:03.442506 tidypath-1.1.2/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     2804 2023-01-17 19:01:52.000000 tidypath-1.1.2/README.md
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-04-11 18:33:03.442506 tidypath-1.1.2/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1161 2023-04-11 18:32:18.000000 tidypath-1.1.2/setup.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 18:33:03.442506 tidypath-1.1.2/tidypath/
--rw-r--r--   0 userx     (1000) wheel      (998)      302 2022-11-08 08:37:56.000000 tidypath-1.1.2/tidypath/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1629 2022-11-08 08:37:56.000000 tidypath-1.1.2/tidypath/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5054 2022-11-08 08:37:56.000000 tidypath-1.1.2/tidypath/config.py
--rw-r--r--   0 userx     (1000) wheel      (998)    11535 2023-04-11 18:31:19.000000 tidypath-1.1.2/tidypath/decorators.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5152 2023-04-11 18:24:26.000000 tidypath-1.1.2/tidypath/fmt.py
--rw-r--r--   0 userx     (1000) wheel      (998)     5197 2022-11-08 08:37:56.000000 tidypath-1.1.2/tidypath/inspection.py
--rw-r--r--   0 userx     (1000) wheel      (998)    12813 2023-01-17 19:01:52.000000 tidypath-1.1.2/tidypath/paths.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9844 2023-01-17 19:01:52.000000 tidypath-1.1.2/tidypath/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 18:33:03.442506 tidypath-1.1.2/tidypath.egg-info/
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)      358 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/SOURCES.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/dependency_links.txt
--rw-r--r--   0 userx     (1000) wheel      (998)       63 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/requires.txt
--rw-r--r--   0 userx     (1000) wheel      (998)        9 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 21:39:48.498314 tidypath-1.1.3/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2022-11-08 08:37:56.000000 tidypath-1.1.3/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-04-11 21:39:48.498314 tidypath-1.1.3/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     2804 2023-01-17 19:01:52.000000 tidypath-1.1.3/README.md
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-04-11 21:39:48.498314 tidypath-1.1.3/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1161 2023-04-11 21:39:36.000000 tidypath-1.1.3/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 21:39:48.498314 tidypath-1.1.3/tidypath/
+-rw-r--r--   0 userx     (1000) wheel      (998)      302 2022-11-08 08:37:56.000000 tidypath-1.1.3/tidypath/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1629 2022-11-08 08:37:56.000000 tidypath-1.1.3/tidypath/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5054 2022-11-08 08:37:56.000000 tidypath-1.1.3/tidypath/config.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    11478 2023-04-11 21:39:01.000000 tidypath-1.1.3/tidypath/decorators.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     6075 2023-04-11 21:32:52.000000 tidypath-1.1.3/tidypath/fmt.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5197 2022-11-08 08:37:56.000000 tidypath-1.1.3/tidypath/inspection.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    13081 2023-04-11 21:38:10.000000 tidypath-1.1.3/tidypath/paths.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9844 2023-01-17 19:01:52.000000 tidypath-1.1.3/tidypath/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 21:39:48.498314 tidypath-1.1.3/tidypath.egg-info/
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)      358 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/SOURCES.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/dependency_links.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)       63 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/requires.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        9 2023-04-11 21:39:48.000000 tidypath-1.1.3/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.1.2/LICENSE.md` & `tidypath-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.2/PKG-INFO` & `tidypath-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.2
+Version: 1.1.3
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.1.2/README.md` & `tidypath-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.2/setup.py` & `tidypath-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.1.2',
+    version='1.1.3',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.1.2/tidypath/_helper.py` & `tidypath-1.1.3/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.2/tidypath/config.py` & `tidypath-1.1.3/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.2/tidypath/decorators.py` & `tidypath-1.1.3/tidypath/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 if find_spec("matplotlib") is None:
     mpl_figure = NoFigure
 else:
     from matplotlib.figure import Figure as mpl_figure
     import matplotlib.pyplot as plt
 
 from . import storage, config
-from .paths import datapath, figpath
+from .paths import datapath, figpath, hash_path
 from .inspection import classify_call_attrs, merge_wrapper_signatures
 from ._helper import merge_nested_dict
 
 
 def savedata(keys_or_function=None, include_classes="file",
              ext=config.EXT_DEFAULT_DATA, keys=config.KEYS_DEFAULT_DATA, funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_DATA,
              overwrite=False, save=True, load_opts_default_save=True,  #defaults for extra arguments
@@ -85,15 +85,15 @@
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, funcname_in_filename=funcname_in_filename, **kwargs):
             key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
             save_keys = merge_nested_dict(key_opts, keys, key_default="all")
             saving_path = datapath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename)
 
             if len(saving_path) > max_str_length:
-                saving_path = "{}.lzma".format(hash(os.path.splitext(saving_path)[0]))
+                saving_path = hash_path(saving_path)
                 warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
 
             if Path(saving_path).exists() and not overwrite:
                 try:
                     result = getattr(storage, f"load_{ext}")(saving_path, **load_opts)
                 except EOFError:
                     warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
@@ -171,15 +171,15 @@
             fig = func(*args, **kwargs)
             if isinstance(fig, (mpl_figure, plotly_figure)):
                 key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
                 save_keys = merge_nested_dict(key_opts, keys, key_default="all")
                 saving_path = figpath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename)
 
                 if len(saving_path) > max_str_length:
-                    saving_path = "{}.lzma".format(hash(os.path.splitext(saving_path)[0]))
+                    saving_path = hash_path(saving_path)
                     warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
 
                 if not Path(saving_path).exists() or overwrite:
                     if isinstance(fig, mpl_figure):
                         fig.savefig(saving_path, format=ext, **{**mpl_save_defaults, **save_opts})
                         plt.close(fig)
                     elif isinstance(fig, plotly_figure):
```

### Comparing `tidypath-1.1.2/tidypath/fmt.py` & `tidypath-1.1.3/tidypath/fmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Encode dictionaries in strings and decode them. Useful for automatically asigning filenames.
+Includes hashing.
 """
 import numpy as np
 import math
 import os
+import hashlib
 
 ##############################################################################################################################
 """                                                  I. Getopt utils                                                       """
 ##############################################################################################################################
 
 def encoder(x, ndigits=2, iterables=(list, tuple, np.ndarray), iterable_maxsize=3):
     """x -> string version of x"""
@@ -126,7 +128,31 @@
     for file in os.listdir(parentDir):
         if key is None or key in file:
             old_filename = os.path.join(parentDir, file)
             new_filename = id_updater(old_filename, update_dict, mode=mode)
             os.rename(old_filename, new_filename)
             r += 1
     return r
+
+
+##############################################################################################################################
+"""                                                     II. Other.                                                         """
+##############################################################################################################################
+
+def hash_file(filename, blocksize=65536):
+    """
+    Returns the SHA256 hash of the file.
+    Autogenerated by copilot. Do not trust it.
+    """
+    hasher = hashlib.sha256()
+    with open(filename, 'rb') as f:
+        buf = f.read(blocksize)
+        while len(buf) > 0:
+            hasher.update(buf)
+            buf = f.read(blocksize)
+    return hasher.hexdigest()
+
+def hash_string(s):
+    """
+    Returns the SHA256 hash of the string.
+    """
+    return hashlib.sha256(s.encode('utf-8')).hexdigest()
```

### Comparing `tidypath-1.1.2/tidypath/inspection.py` & `tidypath-1.1.3/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.2/tidypath/paths.py` & `tidypath-1.1.3/tidypath/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 """
-Creates paths for automatically organizing files. 
+Creates paths for automatically organizing files.
 Allows filename modification: If arg added (deleted) to func => add (delete) arg to stored function output files.
+Hash filename of long paths.
 
 Two schemes:
     1. By module => Module -> submodules -> class tree (until classes in module by default) -> func
     2. By class  => Class organization is a class to be inherited. Sets path: parentDir -> subfolder (optionally specified) -> inheritance_tree -> func_name.
 (1) is the most appropiate.
 """
 import os
 import sys
 import inspect
 import warnings
 import numpy as np
 from copy import deepcopy
 from collections.abc import Iterable
 from pathlib import Path
-from .fmt import dict_to_id, encoder
+from .fmt import dict_to_id, encoder, hash_string
 from .inspection import get_class_that_defined_method
 
 dataDir = "data"
 figDir = "figs"
 
+def hash_path(path):
+    """
+    Hashes the filename (keeping the extension and parentDir) of a path.
+    """
+    parentDir = os.path.dirname(path)
+    filename = os.path.basename(path)
+    filename, ext = os.path.splitext(filename)
+    filename = hash_string(filename)
+    return os.path.join(parentDir, f"{filename}{ext}")
+
 def module_path(func=None, depth=3, include_classes="file", skip=1):
     """
     returns module path and func_name.
-    
+
     include_classes:   'file': path: module -> class tree contained in func file -> func_name.
                        'all': path: module -> full class tree -> func_name.
     """
     if func is None:
         frame = sys._getframe(depth)
         func_name = frame.f_code.co_name
         module = frame.f_globals["__name__"]
@@ -52,56 +63,56 @@
         class_tree = ""
     path = os.path.join(*module.split(".")[1:], class_tree, func_name)
     return path
 
 def saving_path(Dir, ext, keys={}, subfolder="", return_dir=False, funcname_in_filename=False, **kwargs):
     """Tree path: subfolder -> module -> (classes) -> func_name."""
     parentDir = os.path.join(Dir, subfolder, module_path(**kwargs))
-    Path(parentDir).mkdir(exist_ok=True, parents=True)   
+    Path(parentDir).mkdir(exist_ok=True, parents=True)
     if return_dir:
         return parentDir
     else:
         if funcname_in_filename:
             filename = parentDir.split("/")[-1] + f"_{dict_to_id(keys)}_.{ext}"
         else:
             filename = f"{dict_to_id(keys)}_.{ext}"
         return os.path.join(parentDir, filename)
-    
+
 def figpath(ext="png", **kwargs):
     return saving_path(figDir, ext, **kwargs)
 
 def datapath(ext="lzma", **kwargs):
     return saving_path(dataDir, ext, **kwargs)
 
 def filename_modifier(process_filename, func=None, directory=None, check_first=True, overwrite=False, **args):
     """
     Base function for adding/deleting/modifying function args encoded in the output filenames.
-    
+
     Attrs:
-        - process_filename:    function f(file, k_name, k, v) -> new_filename. 
+        - process_filename:    function f(file, k_name, k, v) -> new_filename.
                                - k, v are the key and value of an arg.
                                - k_name is the string encoding of k. (replace '_' -> '-')
         - func (callable):     function (wrapped by savedata or savefig) for retrieving the corresponding directory where the outputs are stored.
         - directory (str):     directory where files are to be modified. It is recommended to pass the function instead of the directory.
-        - check_first (bool):  whether to check the new filenames before applying any changes.   
+        - check_first (bool):  whether to check the new filenames before applying any changes.
         - overwrite (bool):    whether to overwrite files when in conflict.
                                Examples:   add/modify/delete an arg -> two filenames are the same -> one remains.
         - args (kwargs):       Arguments to add/delete/modify in the filename.
     """
     if func is not None:
         if directory is not None:
             raise RuntimeError("Please provide 'func' or 'directory' but not both.")
         else:
             if func.__out__ == "data":
                 directory = datapath(func=func, return_dir=True)
             else:
                 directory = figpath(func=func, return_dir=True)
     elif directory is None:
         raise RuntimeError("Provide 'func' (preferred) or 'directory'.")
-        
+
     args_sorted = {k: args[k] for k in sorted(args)}
     abort_changes = False
     avoid_files = [".ipynb_checkpoints", "__pycache__"]
     for k, v in args_sorted.items():
         check_first_k = deepcopy(check_first)
         if abort_changes:
             break
@@ -116,30 +127,30 @@
                             raise RuntimeError(f"'{new_filename}' already existing before modifying '{file}'. To delete repeated files pass 'overwrite=True'.")
                         else:
                             if check_first_k:
                                 update_file = 0
                                 while update_file not in ["y", "yes", "n", "no"]:
                                     update_file = input("Filename change example:\n\n'{}' -> '{}'\n\nProceed? [y/n]".format(file, new_filename)).lower()
                                 check_first_k = False
-                            if update_file in ["y", "yes"]:                    
-                                os.rename(os.path.join(directory, file), 
+                            if update_file in ["y", "yes"]:
+                                os.rename(os.path.join(directory, file),
                                           os.path.join(directory, new_filename))
                             else:
                                 warnings.warn("Aborted filename changes.", RuntimeWarning)
                                 abort_changes = True
                                 break
     return
 
 def add_arg(func=None, directory=None, check_first=True, overwrite=False, **args):
     """
     Encodes new function args into filename.
     Useful when:
         (1) Adding a new arg to a function wrapped by savedata. Allows loading the available data without recomputing.
         (2) Modifying figure names produced by a function.
-    
+
     Attrs:
         - args (kwargs):       new arguments to encode into filename.
         - func (callable):     function (wrapped by savedata or savefig) for retrieving the corresponding directory where the outputs are stored.
         - directory (str):     directory where files are to be modified. It is recommended to pass the function instead of the directory.
         - check_first (bool):  whether to check the new filenames before applying any changes.
         - overwrite (bool):    whether to overwrite files when in conflict.
                                Example:   add an arg -> two filenames are the same -> one remains.
@@ -157,23 +168,23 @@
                 else:
                     insert_before = args_in_file[pos_new_arg + 1]
                 new_filename = file.replace(f"_{insert_before}", f"_{arg_val}_{insert_before}")
             return new_filename
         else:
             return None
     filename_modifier(process_filename, func=func, directory=directory, check_first=check_first, overwrite=overwrite, **args)
-    return 
+    return
 
 def delete_arg(func=None, arg=None, directory=None, check_first=True, overwrite=False):
     """
     Delete encoded function arg from filename.
     Useful when:
         (1) Deleting an arg from a function wrapped by savedata. Allows loading the available data without recomputing.
         (2) Modifying figure names produced by a function.
-    
+
     Attrs:
         - arg (str or iterable):       key of an arg (k in k=v) to be deleted, or an iterable containing keys.
         - func (callable):             function (wrapped by savedata or savefig) for retrieving the corresponding directory where the outputs are stored.
         - directory (str):             directory where files are to be modified. It is recommended to pass the function instead of the directory.
         - check_first (bool):          whether to check the new filenames before applying any changes.
         - overwrite (bool):            whether to overwrite files when in conflict.
                                        Examples:   Delete an arg -> two filenames are the same -> one remains.
@@ -183,35 +194,35 @@
     elif isinstance(arg, Iterable):
         if all(isinstance(a, str) for a in arg):
             arg_dict = {a: None for a in arg}
         else:
             raise ValueError(f"arg {arg} not valid. Must be a string or an iterable of strings.")
     else:
         raise ValueError(f"arg {arg} not valid. Must be a string or an iterable of strings.")
-        
+
     def process_filename(file, k_name, k, v):
         if file.startswith(f"{k_name}-"):
             return "_".join(file.split("_")[1:])
         else:
             mid_file_k_name = f"_{k_name}-"
             if mid_file_k_name in file:
                 arg_val_encoded = "{}{}".format(mid_file_k_name, file.split(mid_file_k_name)[1].split("_")[0])
                 return file.replace(arg_val_encoded, "")
             else:
                 return None
     filename_modifier(process_filename, func=func, directory=directory, check_first=check_first, overwrite=overwrite, **arg_dict)
-    return 
+    return
 
 def modify_arg(func=None, directory=None, check_first=True, overwrite=False, **args):
     """
     Modified encoded function arg from filename.
     Useful when:
         (1) Renaming an arg value with a more suitable one (more comprehensible, better defined...), leaving the func output unchanged. Allows loading the available data without recomputing.
         (2) Modifying figure names produced by a function.
-    
+
     Attrs:
         - args (kwargs):       arguments to modify in the filename.
         - func (callable):     function (wrapped by savedata or savefig) for retrieving the corresponding directory where the outputs are stored.
         - directory (str):     directory where files are to be modified. It is recommended to pass the function instead of the directory.
         - check_first (bool):  whether to check the new filenames before applying any changes.
         - overwrite (bool):    whether to overwrite files when in conflict.
                                Examples:   Modify an arg -> two filenames are the same -> one remains.
@@ -224,43 +235,42 @@
             if mid_file_k_name in file:
                 arg_val_encoded = "{}{}".format(mid_file_k_name, file.split(mid_file_k_name)[1].split("_")[0])
                 return file.replace(arg_val_encoded, "_{}".format(dict_to_id({k:v})))
             else:
                 return None
 
     filename_modifier(process_filename, func=func, directory=directory, check_first=check_first, overwrite=overwrite, **args)
-    return 
+    return
 
 class Organizer():
     dataDir = dataDir
     figDir = figDir
     subfolder = ""
-    
+
 class ClassPath(Organizer):
     """
     Updates fig and data dir of the class as follows:
     parentDir -> subfolder -> inheritance_tree -> func_name
     """
-    
+
     @classmethod
     def inheritance_path(cls, skip=2):
         return "/".join([c.__name__.lower() for c in cls.mro()[:-skip][::-1]])
-    
+
     @classmethod
     def create_dir(cls, dirKey, depth=2):
         """Creates tree: parentDir -> subfolder -> inheritance_tree -> func_name"""
         path = os.path.join(getattr(cls, f"{dirKey}Dir"),
                             cls.subfolder,
                             cls.inheritance_path(),
                             sys._getframe(depth).f_code.co_name
                            )
         Path(path).mkdir(exist_ok=True, parents=True)
         return path
-        
+
     @classmethod
     def create_figDir(cls):
         return cls.create_dir("fig")
-    
+
     @classmethod
     def create_dataDir(cls):
         return cls.create_dir("data")
-
```

### Comparing `tidypath-1.1.2/tidypath/storage.py` & `tidypath-1.1.3/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.2/tidypath.egg-info/PKG-INFO` & `tidypath-1.1.3/tidypath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.2
+Version: 1.1.3
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

