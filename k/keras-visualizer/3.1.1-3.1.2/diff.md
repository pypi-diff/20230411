# Comparing `tmp/keras-visualizer-3.1.1.tar.gz` & `tmp/keras-visualizer-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-visualizer-3.1.1.tar", last modified: Sat Mar 11 08:13:42 2023, max compression
+gzip compressed data, was "keras-visualizer-3.1.2.tar", last modified: Tue Apr 11 08:41:11 2023, max compression
```

## Comparing `keras-visualizer-3.1.1.tar` & `keras-visualizer-3.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 08:13:42.840330 keras-visualizer-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-11 08:13:29.000000 keras-visualizer-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-03-11 08:13:42.840330 keras-visualizer-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-03-11 08:13:29.000000 keras-visualizer-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 08:13:42.836330 keras-visualizer-3.1.1/keras_visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-03-11 08:13:29.000000 keras-visualizer-3.1.1/keras_visualizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-11 08:13:42.840330 keras-visualizer-3.1.1/keras_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-03-11 08:13:42.000000 keras-visualizer-3.1.1/keras_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-11 08:13:42.000000 keras-visualizer-3.1.1/keras_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-11 08:13:42.000000 keras-visualizer-3.1.1/keras_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-11 08:13:42.000000 keras-visualizer-3.1.1/keras_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-11 08:13:42.000000 keras-visualizer-3.1.1/keras_visualizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-11 08:13:42.840330 keras-visualizer-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-11 08:13:29.000000 keras-visualizer-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:41:11.708169 keras-visualizer-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 08:41:02.000000 keras-visualizer-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-11 08:41:11.704169 keras-visualizer-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-11 08:41:02.000000 keras-visualizer-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:41:11.704169 keras-visualizer-3.1.2/keras_visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-11 08:41:02.000000 keras-visualizer-3.1.2/keras_visualizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:41:11.704169 keras-visualizer-3.1.2/keras_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:41:11.708169 keras-visualizer-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 08:41:02.000000 keras-visualizer-3.1.2/setup.py
```

### Comparing `keras-visualizer-3.1.1/LICENSE` & `keras-visualizer-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keras-visualizer-3.1.1/PKG-INFO` & `keras-visualizer-3.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: keras-visualizer
-Version: 3.1.1
+Version: 3.1.2
 Summary: A Keras Model Visualizer
 Home-page: https://github.com/lordmahyar/keras-visualizer
 Author: Mahyar Amiri
 Author-email: mmaahhyyaarr@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Keras Visualizer
 
+![LOGO](logo.png)
+
 [![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
 [![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
 [![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
 
 A Python Library for Visualizing Keras Models.
@@ -102,14 +104,16 @@
     'INPUT_DENSE_COLOR': '#2ecc71',
     'INPUT_EMBEDDING_COLOR': 'black',
     'INPUT_EMBEDDING_FONT': 'white',
     'INPUT_GRAYSCALE_COLOR': 'black:white',
     'INPUT_GRAYSCALE_FONT': 'white',
     'INPUT_RGB_COLOR': '#e74c3c:#3498db',
     'INPUT_RGB_FONT': 'white',
+    'INPUT_LAYER_COLOR': 'black',
+    'INPUT_LAYER_FONT': 'white',
     # HIDDEN LAYERS
     'HIDDEN_DENSE_COLOR': '#3498db',
     'HIDDEN_CONV_COLOR': '#5faad0',
     'HIDDEN_CONV_FONT': 'black',
     'HIDDEN_POOLING_COLOR': '#8e44ad',
     'HIDDEN_POOLING_FONT': 'white',
     'HIDDEN_FLATTEN_COLOR': '#2c3e50',
@@ -118,14 +122,16 @@
     'HIDDEN_DROPOUT_FONT': 'black',
     'HIDDEN_ACTIVATION_COLOR': '#00b894',
     'HIDDEN_ACTIVATION_FONT': 'black',
     'HIDDEN_LAYER_COLOR': 'black',
     'HIDDEN_LAYER_FONT': 'white',
     # OUTPUT LAYER
     'OUTPUT_DENSE_COLOR': '#e74c3c',
+    'OUTPUT_LAYER_COLOR': 'black',
+    'OUTPUT_LAYER_FONT': 'white',
 }
 ```
 
 **Note**:
 
 * set `'MAX_NEURONS': None` to disable max neurons constraint.
 * see list of color names [here](https://graphviz.org/doc/info/colors.html).
```

### Comparing `keras-visualizer-3.1.1/README.md` & `keras-visualizer-3.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Keras Visualizer
 
+![LOGO](logo.png)
+
 [![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
 [![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
 [![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
 
 A Python Library for Visualizing Keras Models.
@@ -87,14 +89,16 @@
     'INPUT_DENSE_COLOR': '#2ecc71',
     'INPUT_EMBEDDING_COLOR': 'black',
     'INPUT_EMBEDDING_FONT': 'white',
     'INPUT_GRAYSCALE_COLOR': 'black:white',
     'INPUT_GRAYSCALE_FONT': 'white',
     'INPUT_RGB_COLOR': '#e74c3c:#3498db',
     'INPUT_RGB_FONT': 'white',
+    'INPUT_LAYER_COLOR': 'black',
+    'INPUT_LAYER_FONT': 'white',
     # HIDDEN LAYERS
     'HIDDEN_DENSE_COLOR': '#3498db',
     'HIDDEN_CONV_COLOR': '#5faad0',
     'HIDDEN_CONV_FONT': 'black',
     'HIDDEN_POOLING_COLOR': '#8e44ad',
     'HIDDEN_POOLING_FONT': 'white',
     'HIDDEN_FLATTEN_COLOR': '#2c3e50',
@@ -103,14 +107,16 @@
     'HIDDEN_DROPOUT_FONT': 'black',
     'HIDDEN_ACTIVATION_COLOR': '#00b894',
     'HIDDEN_ACTIVATION_FONT': 'black',
     'HIDDEN_LAYER_COLOR': 'black',
     'HIDDEN_LAYER_FONT': 'white',
     # OUTPUT LAYER
     'OUTPUT_DENSE_COLOR': '#e74c3c',
+    'OUTPUT_LAYER_COLOR': 'black',
+    'OUTPUT_LAYER_FONT': 'white',
 }
 ```
 
 **Note**:
 
 * set `'MAX_NEURONS': None` to disable max neurons constraint.
 * see list of color names [here](https://graphviz.org/doc/info/colors.html).
```

### Comparing `keras-visualizer-3.1.1/keras_visualizer/__init__.py` & `keras-visualizer-3.1.2/keras_visualizer/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         'INPUT_DENSE_COLOR': '#2ecc71',
         'INPUT_EMBEDDING_COLOR': 'black',
         'INPUT_EMBEDDING_FONT': 'white',
         'INPUT_GRAYSCALE_COLOR': 'black:white',
         'INPUT_GRAYSCALE_FONT': 'white',
         'INPUT_RGB_COLOR': '#e74c3c:#3498db',
         'INPUT_RGB_FONT': 'white',
+        'INPUT_LAYER_COLOR': 'black',
+        'INPUT_LAYER_FONT': 'white',
         # HIDDEN LAYERS
         'HIDDEN_DENSE_COLOR': '#3498db',
         'HIDDEN_CONV_COLOR': '#5faad0',
         'HIDDEN_CONV_FONT': 'black',
         'HIDDEN_POOLING_COLOR': '#8e44ad',
         'HIDDEN_POOLING_FONT': 'white',
         'HIDDEN_FLATTEN_COLOR': '#2c3e50',
@@ -41,28 +43,30 @@
         'HIDDEN_DROPOUT_FONT': 'black',
         'HIDDEN_ACTIVATION_COLOR': '#00b894',
         'HIDDEN_ACTIVATION_FONT': 'black',
         'HIDDEN_LAYER_COLOR': 'black',
         'HIDDEN_LAYER_FONT': 'white',
         # OUTPUT LAYER
         'OUTPUT_DENSE_COLOR': '#e74c3c',
+        'OUTPUT_LAYER_COLOR': 'black',
+        'OUTPUT_LAYER_FONT': 'white',
     }
 
     settings = {**main_settings, **settings} if settings is not None else {**main_settings}
     max_neurons = settings['MAX_NEURONS']
 
     input_layer = 0
     hidden_layers_nr = 0
     layer_types = []
     hidden_layers = []
     output_layer = 0
 
     for num, layer in enumerate(model.layers, 1):
         if num == 1:
-            input_layer = layer.input_shape[1]
+            input_layer = layer.input_shape[1] if type(layer.input_shape) == tuple else layer.input_shape[0][1]
         if num == len(model.layers):
             output_layer = layer.output_shape[1]
         else:
             hidden_layers_nr += 1
             hidden_layers.append(layer.output_shape[1] if layer.__class__.__name__ == 'Dense' else 1)
             layer_types.append(f'{layer.__class__.__name__}')
 
@@ -82,37 +86,38 @@
             ranksep='2',  # Y-SPACE
             splines='false'
         )
 
         # Input Layer
         with graph.subgraph(name='cluster_input') as c:
             # DENSE LAYER INPUT
-            if model.layers[0].__class__.__name__ == 'Dense':
-                input_units = model.layers[0].input_shape[1]
+            layer = model.layers[0]
+            if layer.__class__.__name__ == 'Dense':
+                input_units = layer.input_shape[1]
                 label_dense_input = f'Input Units: {input_units}'
                 if max_neurons is not None and input_units > max_neurons:
                     label_dense_input += f' (+{input_units - max_neurons} more)'
                     input_layer = max_neurons
-                label_dense_input += f'\nActivation: {model.layers[0].get_config()["activation"]}'
+                label_dense_input += f'\nActivation: {layer.get_config()["activation"]}'
                 c.attr(color='white')
                 for i in range(0, input_layer):
                     n += 1
                     c.node(str(n))
                     c.attr(rank='same')
                     c.node_attr.update(shape='circle', style='filled', color=settings['INPUT_DENSE_COLOR'], fontcolor=settings['INPUT_DENSE_COLOR'])
                 c.node(str(n + 1) * 3, label_dense_input, shape='rectangle', fontsize='18', color='white', fontcolor='black')
             # EMBEDDING LAYER INPUT
-            elif model.layers[0].__class__.__name__ == 'Embedding':
-                input_dim = model.layers[0].input_dim
-                output_dim = model.layers[0].output_dim
+            elif layer.__class__.__name__ == 'Embedding':
+                input_dim = layer.input_dim
+                output_dim = layer.output_dim
                 n += 1
                 c.node(str(n), label=f'Embedding\nInput Dim: {input_dim}\nOutput Dim: {output_dim}', shape='square', style='filled', fillcolor=settings['INPUT_EMBEDDING_COLOR'], fontcolor=settings['INPUT_EMBEDDING_FONT'])
             # CONV2D LAYER INPUT (IMAGE)
-            elif 'Conv' in model.layers[0].__class__.__name__:
-                pxls = model.layers[0].input_shape
+            elif 'Conv' in layer.__class__.__name__:
+                pxls = layer.input_shape
                 clr = pxls[-1]
                 node_color = 'white'
                 node_font = 'black'
                 if clr == 1:
                     clrmap = 'Grayscale'
                     node_color = settings['INPUT_GRAYSCALE_COLOR']
                     node_font = settings['INPUT_GRAYSCALE_FONT']
@@ -121,15 +126,20 @@
                     node_color = settings['INPUT_RGB_COLOR']
                     node_font = settings['INPUT_RGB_FONT']
                 else:
                     clrmap = ''
                 n += 1
                 c.node(str(n), label=f'Image\n{pxls[-3]} x {pxls[-2]} pixels\n{clrmap}', shape='square', style='filled', fillcolor=node_color, fontcolor=node_font)
             else:
-                raise ValueError('[Keras Visualizer] Input Layer is not supported for visualizing')
+                # raise ValueError('[Keras Visualizer] Input Layer is not supported for visualizing')
+                c.attr(color='white')
+                n += 1
+                input_layer = layer.input_shape[1] if type(layer.input_shape) == tuple else layer.input_shape[0][1]
+                label_layer = f'{layer.__class__.__name__}\nshape= {input_layer}'
+                c.node(str(n), label=label_layer, shape='egg', style='filled', fillcolor=settings['INPUT_LAYER_COLOR'], fontcolor=settings['INPUT_LAYER_FONT'])
 
         # Hidden Layers
         for i in range(0, hidden_layers_nr):
             with graph.subgraph(name='cluster_' + str(i + 1)) as c:
                 # Dense Layer
                 if layer_types[i] == 'Dense':
                     c.attr(color='white')
@@ -232,15 +242,20 @@
                 for i in range(1, output_layer + 1):
                     n += 1
                     c.node(str(n), shape='circle', style='filled', color=settings['OUTPUT_DENSE_COLOR'], fontcolor=settings['OUTPUT_DENSE_COLOR'])
                     for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
                         graph.edge(str(h), str(n))
                 # c.node_attr.update(color='#2ecc71', style='filled', fontcolor='#2ecc71', shape='circle')
             else:
-                raise ValueError('[Keras Visualizer] Output layer is not supported for visualizing')
+                # raise ValueError('[Keras Visualizer] Output layer is not supported for visualizing')
+                c.attr(color='white')
+                n += 1
+                output_layer = layer.output_shape[1] if type(layer.output_shape) == tuple else layer.output_shape[0][1]
+                label_layer = f'{layer.__class__.__name__}\nshape= {output_layer}'
+                c.node(str(n), label=label_layer, shape='egg', style='filled', fillcolor=settings['OUTPUT_LAYER_COLOR'], fontcolor=settings['OUTPUT_LAYER_FONT'])
 
         graph.attr(arrowShape='none')
         graph.edge_attr.update(arrowhead='none', color=settings['ARROW_COLOR'])
 
     # SAVE GRAPH
     try:
         if file_format is not None:
```

### Comparing `keras-visualizer-3.1.1/keras_visualizer.egg-info/PKG-INFO` & `keras-visualizer-3.1.2/keras_visualizer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: keras-visualizer
-Version: 3.1.1
+Version: 3.1.2
 Summary: A Keras Model Visualizer
 Home-page: https://github.com/lordmahyar/keras-visualizer
 Author: Mahyar Amiri
 Author-email: mmaahhyyaarr@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Keras Visualizer
 
+![LOGO](logo.png)
+
 [![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
 [![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
 [![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
 
 A Python Library for Visualizing Keras Models.
@@ -102,14 +104,16 @@
     'INPUT_DENSE_COLOR': '#2ecc71',
     'INPUT_EMBEDDING_COLOR': 'black',
     'INPUT_EMBEDDING_FONT': 'white',
     'INPUT_GRAYSCALE_COLOR': 'black:white',
     'INPUT_GRAYSCALE_FONT': 'white',
     'INPUT_RGB_COLOR': '#e74c3c:#3498db',
     'INPUT_RGB_FONT': 'white',
+    'INPUT_LAYER_COLOR': 'black',
+    'INPUT_LAYER_FONT': 'white',
     # HIDDEN LAYERS
     'HIDDEN_DENSE_COLOR': '#3498db',
     'HIDDEN_CONV_COLOR': '#5faad0',
     'HIDDEN_CONV_FONT': 'black',
     'HIDDEN_POOLING_COLOR': '#8e44ad',
     'HIDDEN_POOLING_FONT': 'white',
     'HIDDEN_FLATTEN_COLOR': '#2c3e50',
@@ -118,14 +122,16 @@
     'HIDDEN_DROPOUT_FONT': 'black',
     'HIDDEN_ACTIVATION_COLOR': '#00b894',
     'HIDDEN_ACTIVATION_FONT': 'black',
     'HIDDEN_LAYER_COLOR': 'black',
     'HIDDEN_LAYER_FONT': 'white',
     # OUTPUT LAYER
     'OUTPUT_DENSE_COLOR': '#e74c3c',
+    'OUTPUT_LAYER_COLOR': 'black',
+    'OUTPUT_LAYER_FONT': 'white',
 }
 ```
 
 **Note**:
 
 * set `'MAX_NEURONS': None` to disable max neurons constraint.
 * see list of color names [here](https://graphviz.org/doc/info/colors.html).
```

### Comparing `keras-visualizer-3.1.1/setup.py` & `keras-visualizer-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-VERSION = '3.1.1'
+VERSION = '3.1.2'
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='keras-visualizer',
     version=VERSION,
```

