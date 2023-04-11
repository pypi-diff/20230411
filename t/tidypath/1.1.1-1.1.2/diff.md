# Comparing `tmp/tidypath-1.1.1.tar.gz` & `tmp/tidypath-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.1.1.tar", last modified: Mon Mar 20 15:50:06 2023, max compression
+gzip compressed data, was "tidypath-1.1.2.tar", last modified: Tue Apr 11 18:33:03 2023, max compression
```

## Comparing `tidypath-1.1.1.tar` & `tidypath-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-03-20 15:50:06.418320 tidypath-1.1.1/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-07 11:08:19.000000 tidypath-1.1.1/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2023-03-20 15:50:06.418320 tidypath-1.1.1/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2804 2022-11-25 17:30:15.000000 tidypath-1.1.1/README.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2023-03-20 15:50:06.422320 tidypath-1.1.1/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1176 2023-03-20 15:49:51.000000 tidypath-1.1.1/setup.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-03-20 15:50:06.402319 tidypath-1.1.1/tidypath/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2022-11-07 12:11:16.000000 tidypath-1.1.1/tidypath/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1629 2022-11-07 17:52:31.000000 tidypath-1.1.1/tidypath/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5054 2022-11-07 17:57:44.000000 tidypath-1.1.1/tidypath/config.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    10961 2023-03-20 15:49:30.000000 tidypath-1.1.1/tidypath/decorators.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5152 2023-03-12 11:20:40.000000 tidypath-1.1.1/tidypath/fmt.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     5197 2022-11-07 17:56:37.000000 tidypath-1.1.1/tidypath/inspection.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    12813 2022-11-10 08:22:24.000000 tidypath-1.1.1/tidypath/paths.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9844 2022-11-08 08:59:29.000000 tidypath-1.1.1/tidypath/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2023-03-20 15:50:06.414319 tidypath-1.1.1/tidypath.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3682 2023-03-20 15:50:06.000000 tidypath-1.1.1/tidypath.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      358 2023-03-20 15:50:06.000000 tidypath-1.1.1/tidypath.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2023-03-20 15:50:06.000000 tidypath-1.1.1/tidypath.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)       63 2023-03-20 15:50:06.000000 tidypath-1.1.1/tidypath.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        9 2023-03-20 15:50:06.000000 tidypath-1.1.1/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 18:33:03.442506 tidypath-1.1.2/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2022-11-08 08:37:56.000000 tidypath-1.1.2/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-04-11 18:33:03.442506 tidypath-1.1.2/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     2804 2023-01-17 19:01:52.000000 tidypath-1.1.2/README.md
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2023-04-11 18:33:03.442506 tidypath-1.1.2/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1161 2023-04-11 18:32:18.000000 tidypath-1.1.2/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 18:33:03.442506 tidypath-1.1.2/tidypath/
+-rw-r--r--   0 userx     (1000) wheel      (998)      302 2022-11-08 08:37:56.000000 tidypath-1.1.2/tidypath/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1629 2022-11-08 08:37:56.000000 tidypath-1.1.2/tidypath/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5054 2022-11-08 08:37:56.000000 tidypath-1.1.2/tidypath/config.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    11535 2023-04-11 18:31:19.000000 tidypath-1.1.2/tidypath/decorators.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5152 2023-04-11 18:24:26.000000 tidypath-1.1.2/tidypath/fmt.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     5197 2022-11-08 08:37:56.000000 tidypath-1.1.2/tidypath/inspection.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    12813 2023-01-17 19:01:52.000000 tidypath-1.1.2/tidypath/paths.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9844 2023-01-17 19:01:52.000000 tidypath-1.1.2/tidypath/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2023-04-11 18:33:03.442506 tidypath-1.1.2/tidypath.egg-info/
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)      358 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/SOURCES.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        1 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/dependency_links.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)       63 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/requires.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)        9 2023-04-11 18:33:03.000000 tidypath-1.1.2/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.1.1/LICENSE.md` & `tidypath-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.1/PKG-INFO` & `tidypath-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.1
+Version: 1.1.2
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.1.1/README.md` & `tidypath-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.1/setup.py` & `tidypath-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.1.1',
+    version='1.1.2',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords=['tidy', 'project organization', 'project', 'organization', 'path', 'storage'],
     classifiers=[
-        "Programming Language :: Python :: 3",            
+        "Programming Language :: Python :: 3",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU Affero General Public License v3",
-        "Operating System :: OS Independent",    
+        "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Office/Business",
         "Intended Audience :: Science/Research",
     ],
     python_requires=">=3",
     install_requires=[
         'numpy',
         'pandas',
     ],
     extras_require={
         "matplotlib": "matplotlib",
         "plotly": ["plotly", "kaleido"],
     },
-)
+)
```

### Comparing `tidypath-1.1.1/tidypath/_helper.py` & `tidypath-1.1.2/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.1/tidypath/config.py` & `tidypath-1.1.2/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.1/tidypath/decorators.py` & `tidypath-1.1.2/tidypath/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Main uses: save and cache data, save figures, change figure color, timing.
 """
 import math
 import inspect
 import warnings
+import os
 from pathlib import Path
 from functools import wraps
 from collections.abc import Iterable
 from importlib.util import find_spec
 from ._helper import NoFigure
 if find_spec("plotly") is None:
     plotly_figure = NoFigure
@@ -24,68 +25,77 @@
 from .inspection import classify_call_attrs, merge_wrapper_signatures
 from ._helper import merge_nested_dict
 
 
 def savedata(keys_or_function=None, include_classes="file",
              ext=config.EXT_DEFAULT_DATA, keys=config.KEYS_DEFAULT_DATA, funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_DATA,
              overwrite=False, save=True, load_opts_default_save=True,  #defaults for extra arguments
-             load_opts={}, **save_opts):    
+             max_str_length=255,
+             load_opts={}, **save_opts):
     """
     Decorator for automatically saving output and then loading cached data.
     Default behavior:
         1st function call:   stores the data with extension 'ext'.
         rest:                loads stored data if the key args passed to the function coincide.
-        
+
+    If filename is too long, it is shortened by hashing it.
+
+
     NOTE (!) decorated funcs will have extra arguments:
         - save (bool).                 whether to save the output of the function.
         - overwrite (bool).            whether to overwrite the saved version.
         - funcname_in_filename(bool)   whether to include funcname in the filename.
-        - keys (dict/str/iterable)   · dict:     specifies filename of the form k1-v1_k2-v2_...kn_vn. 
+        - keys (dict/str/iterable)   · dict:     specifies filename of the form k1-v1_k2-v2_...kn_vn.
                                                  k_i do not have to be arguments of the function.
                                      · str:       key of a keyword argument. Example: keys = 'x'.
                                                  "kwargs_defaults"  =>  default kwargs that were not modified.
                                                  "kwargs"           =>  kwargs passed during function call.
                                                  "kwargs_full"      =>  kws_defaults + kws.
                                                  "pos_only"         =>  length of *args
                                                  "args"             =>  attrs != **kwargs, *args.
                                                  "all"              if config.KEYS_ADD_POSONLY_TO_ALL  =>  all attrs
                                                                     else                               =>  all attrs except pos_only: kwargs_full + args
                                                  can combine options using "+" or "-". Example: "args+z", "x+y+kwargs", "all-y".
                                      · iterable: containing a combination of the available string keys (above). ["k1", "k2"] == "k1+k2".
-                                                 
+
     Attrs:
         - function:                function to which the decorator is applied
         - ext:                     storing extension. Selects 'storage' functions save_ext, load_ext.
                                    Supported: 'lzma' (default), 'bz2', 'json', 'csv', 'npz'.
         - include_classes:         include class tree in saving_path.
         - load_opts:               kws for storage.load_ext. default kws are those of 'saving_options', those specified update saving_options dict.
         - save_opts:               kws for storage.save_ext
         - load_opts_default_save:  use save_opts as default for load_opts.
+        - max_str_length:          max length of filename. If exceeded, filename is shortened by hashing it.
         - rest:                    default behavior for decorated funcs extra arguments (above).
-        
+
     Returns: Function decorator
     """
     if isinstance(keys_or_function, Iterable):
         keys = keys_or_function
         func = None
     elif callable(keys_or_function):
         func = keys_or_function
     else:
         func = None
-        
+
     if load_opts_default_save:
         load_opts = {**save_opts, **load_opts}
-        
-    def _savedata(func):  
+
+    def _savedata(func):
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, funcname_in_filename=funcname_in_filename, **kwargs):
             key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
-            save_keys = merge_nested_dict(key_opts, keys, key_default="all")                    
+            save_keys = merge_nested_dict(key_opts, keys, key_default="all")
             saving_path = datapath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename)
-            
+
+            if len(saving_path) > max_str_length:
+                saving_path = "{}.lzma".format(hash(os.path.splitext(saving_path)[0]))
+                warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
+
             if Path(saving_path).exists() and not overwrite:
                 try:
                     result = getattr(storage, f"load_{ext}")(saving_path, **load_opts)
                 except EOFError:
                     warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
                     result = func(*args, **kwargs)
                     getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
@@ -93,99 +103,107 @@
                 result = func(*args, **kwargs)
                 getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
             return result
 
         wrapper.__signature__ = merge_wrapper_signatures(wrapper, ["overwrite", "keys", "save", "funcname_in_filename"])
         wrapper.__out__ = "data"
         return wrapper
-        
+
     if func is None:
         return _savedata
     else:
         return _savedata(func)
-    
 
-def savefig(keys_or_function=None, include_classes="file", 
+
+def savefig(keys_or_function=None, include_classes="file",
             ext=config.EXT_DEFAULT_FIG, keys=config.KEYS_DEFAULT_FIG, funcname_in_filename=config.FUNCNAME_IN_FILENAME_DEFAULT_FIG, return_fig=config.RETURN_FIG_DEFAULT,
+            max_str_length=255,
             overwrite=True, save=True,  #defaults for extra arguments
-            **save_opts):    
+            **save_opts):
     """
     Generates figsaver decorator.
     Figure returned by function is automatically saved. Compatible with matplotlib and plotly.
     If None or NaN is returned, avoid figure saving.
-        
+
+    If filename is too long, it is shortened by hashing it.
+
     NOTE (!) decorated funcs will have extra arguments:
         - return_fig (bool)            whether to return the figure (output of function).
         - save (bool).                 whether to save the figure.
         - overwrite (bool).            whether to overwrite the saved version.
         - funcname_in_filename(bool)   whether to include funcname in the filename.
-        - keys (dict/str/iterable)   · dict:     specifies filename of the form k1-v1_k2-v2_...kn_vn. 
+        - keys (dict/str/iterable)   · dict:     specifies filename of the form k1-v1_k2-v2_...kn_vn.
                                                  k_i do not have to be arguments of the function.
                                      · str:       key of a keyword argument. Example: keys = 'x'.
                                                  "kwargs_defaults"  =>  default kwargs that were not modified.
                                                  "kwargs"           =>  kwargs passed during function call.
                                                  "kwargs_full"      =>  kws_defaults + kws.
                                                  "pos_only"         =>  length of *args. Also self and cls are counted as pos_only arguments.
                                                  "args"             =>  attrs != **kwargs, *args.
                                                  "all"              if config.KEYS_ADD_POSONLY_TO_ALL  =>  all attrs
                                                                     else                               =>  all attrs except pos_only: kwargs_full + args
                                                  can combine options using "+" or "-". Example: "args+z", "x+y+kwargs", "all-y".
-                                     · iterable: containing a combination of the available string keys (above). ["k1", "k2"] == "k1+k2".                                         
-        
+                                     · iterable: containing a combination of the available string keys (above). ["k1", "k2"] == "k1+k2".
+
     Attrs:
         - function:                function to which the decorator is applied
         - ext:                     storing extension. 'eps' recommended for articles.
                                    Supported: any extension supported by matplotlib/plotly. Example: 'png', 'eps', 'html' (plotly), etc.
         - include_classes:         include class tree in saving_path.
         - save_opts:               kws for saving function.
+        - max_str_length:          max length of filename. If exceeded, filename is shortened by hashing it.
         - rest:                    default behavior for decorated funcs extra arguments (above).
-        
+
     Returns: Function decorator
     """
     if isinstance(keys_or_function, Iterable):
         keys = keys_or_function
         func = None
     elif callable(keys_or_function):
         func = keys_or_function
     else:
         func = None
-        
+
     mpl_save_defaults = dict(bbox_inches="tight")
-        
-    def _savefig(func):  
+
+    def _savefig(func):
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, return_fig=return_fig, funcname_in_filename=funcname_in_filename, **kwargs):
             fig = func(*args, **kwargs)
             if isinstance(fig, (mpl_figure, plotly_figure)):
                 key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
-                save_keys = merge_nested_dict(key_opts, keys, key_default="all")                    
+                save_keys = merge_nested_dict(key_opts, keys, key_default="all")
                 saving_path = figpath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename)
-                
+
+                if len(saving_path) > max_str_length:
+                    saving_path = "{}.lzma".format(hash(os.path.splitext(saving_path)[0]))
+                    warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
+
                 if not Path(saving_path).exists() or overwrite:
                     if isinstance(fig, mpl_figure):
                         fig.savefig(saving_path, format=ext, **{**mpl_save_defaults, **save_opts})
                         plt.close(fig)
                     elif isinstance(fig, plotly_figure):
                         if ext == "html":
                             fig.write_html(saving_path, **save_opts)
                         else:
                             fig.write_image(saving_path, format=ext, **save_opts)
                     else:
                         raise TypeError(f"fig type '{type(fig)}' not valid. Available: 'matplotlib.figure.Figure', 'plotly.grap_objs._figure.Figure'.")
-                        
+
                 if return_fig:
                     return fig
                 else:
                     return
             elif fig is None or math.isnan(fig):
                 warnings.warn("Expected output figure (plotly or matplotlib) and received None or NaN.", RuntimeWarning)
             else:
                 warnings.warn("Expected output figure (plotly, matplotlib) or a flag for figure error computation (None, NaN), but received {}".format(type(fig)), RuntimeWarning)
-            
+
         wrapper.__signature__ = merge_wrapper_signatures(wrapper, ["overwrite", "keys", "save", "funcname_in_filename", "return_fig"])
         wrapper.__out__ = "figure"
         return wrapper
-    
+
     if func is None:
         return _savefig
     else:
-        return _savefig(func)
+        return _savefig(func)
```

### Comparing `tidypath-1.1.1/tidypath/fmt.py` & `tidypath-1.1.2/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.1/tidypath/inspection.py` & `tidypath-1.1.2/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.1/tidypath/paths.py` & `tidypath-1.1.2/tidypath/paths.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.1/tidypath/storage.py` & `tidypath-1.1.2/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.1.1/tidypath.egg-info/PKG-INFO` & `tidypath-1.1.2/tidypath.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.1.1
+Version: 1.1.2
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

