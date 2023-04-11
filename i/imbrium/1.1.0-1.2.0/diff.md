# Comparing `tmp/imbrium-1.1.0.tar.gz` & `tmp/imbrium-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbrium-1.1.0.tar", last modified: Thu Mar  9 01:23:27 2023, max compression
+gzip compressed data, was "imbrium-1.2.0.tar", last modified: Tue Apr 11 21:05:07 2023, max compression
```

## Comparing `imbrium-1.1.0.tar` & `imbrium-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 01:23:27.782472 imbrium-1.1.0/
--rw-rw-rw-   0        0        0     1622 2023-03-09 00:12:02.000000 imbrium-1.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1096 2022-10-31 01:25:26.000000 imbrium-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 imbrium-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    30690 2023-03-09 01:23:27.778352 imbrium-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    29937 2023-03-08 23:29:11.000000 imbrium-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 01:23:27.639529 imbrium-1.1.0/imbrium/
--rw-rw-rw-   0        0        0       91 2023-02-21 01:19:25.000000 imbrium-1.1.0/imbrium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-09 01:23:27.672377 imbrium-1.1.0/imbrium/architectures/
--rw-rw-rw-   0        0        0       44 2022-10-31 01:25:26.000000 imbrium-1.1.0/imbrium/architectures/__init__.py
--rw-rw-rw-   0        0        0    28490 2023-03-08 23:42:08.000000 imbrium-1.1.0/imbrium/architectures/models.py
-drwxrwxrwx   0        0        0        0 2023-03-09 01:23:27.697184 imbrium-1.1.0/imbrium/blueprints/
--rw-rw-rw-   0        0        0        0 2022-10-31 01:25:26.000000 imbrium-1.1.0/imbrium/blueprints/__init__.py
--rw-rw-rw-   0        0        0     1706 2023-02-18 02:25:36.000000 imbrium-1.1.0/imbrium/blueprints/abstract_multivariate.py
--rw-rw-rw-   0        0        0     1702 2023-02-18 02:25:36.000000 imbrium-1.1.0/imbrium/blueprints/abstract_univariate.py
-drwxrwxrwx   0        0        0        0 2023-03-09 01:23:27.738288 imbrium-1.1.0/imbrium/predictors/
--rw-rw-rw-   0        0        0      296 2023-02-26 18:46:56.000000 imbrium-1.1.0/imbrium/predictors/__init__.py
--rw-rw-rw-   0        0        0    22977 2023-03-08 23:42:08.000000 imbrium-1.1.0/imbrium/predictors/multivarhybrid.py
--rw-rw-rw-   0        0        0    35394 2023-03-08 23:42:08.000000 imbrium-1.1.0/imbrium/predictors/multivarpure.py
--rw-rw-rw-   0        0        0    22328 2023-03-08 23:42:08.000000 imbrium-1.1.0/imbrium/predictors/univarhybrid.py
--rw-rw-rw-   0        0        0    35037 2023-03-08 23:42:08.000000 imbrium-1.1.0/imbrium/predictors/univarpure.py
-drwxrwxrwx   0        0        0        0 2023-03-09 01:23:27.762153 imbrium-1.1.0/imbrium/utils/
--rw-rw-rw-   0        0        0      129 2023-02-21 00:14:08.000000 imbrium-1.1.0/imbrium/utils/__init__.py
--rw-rw-rw-   0        0        0     1111 2023-02-21 00:14:08.000000 imbrium-1.1.0/imbrium/utils/optimization.py
--rw-rw-rw-   0        0        0      426 2023-03-08 23:42:08.000000 imbrium-1.1.0/imbrium/utils/scaler.py
--rw-rw-rw-   0        0        0    10584 2023-01-09 01:24:32.000000 imbrium-1.1.0/imbrium/utils/transformer.py
-drwxrwxrwx   0        0        0        0 2023-03-09 01:23:27.664313 imbrium-1.1.0/imbrium.egg-info/
--rw-rw-rw-   0        0        0    30690 2023-03-09 01:23:27.000000 imbrium-1.1.0/imbrium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2023-03-09 01:23:27.000000 imbrium-1.1.0/imbrium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 01:23:27.000000 imbrium-1.1.0/imbrium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-03-09 01:23:27.000000 imbrium-1.1.0/imbrium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-09 01:23:27.000000 imbrium-1.1.0/imbrium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-09 01:23:27.786496 imbrium-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1357 2023-02-21 01:18:49.000000 imbrium-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.321368 imbrium-1.2.0/
+-rw-rw-rw-   0        0        0     1732 2023-03-26 19:06:20.000000 imbrium-1.2.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1096 2022-10-31 01:25:26.000000 imbrium-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2022-10-31 01:25:26.000000 imbrium-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    48846 2023-04-11 21:05:07.321368 imbrium-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    48093 2023-04-11 20:47:03.000000 imbrium-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.164635 imbrium-1.2.0/imbrium/
+-rw-rw-rw-   0        0        0       91 2023-03-12 18:31:01.000000 imbrium-1.2.0/imbrium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.211564 imbrium-1.2.0/imbrium/architectures/
+-rw-rw-rw-   0        0        0       44 2022-10-31 01:25:26.000000 imbrium-1.2.0/imbrium/architectures/__init__.py
+-rw-rw-rw-   0        0        0    36327 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/architectures/models.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.227151 imbrium-1.2.0/imbrium/blueprints/
+-rw-rw-rw-   0        0        0        0 2022-10-31 01:25:26.000000 imbrium-1.2.0/imbrium/blueprints/__init__.py
+-rw-rw-rw-   0        0        0     1706 2023-02-18 02:25:36.000000 imbrium-1.2.0/imbrium/blueprints/abstract_multivariate.py
+-rw-rw-rw-   0        0        0     1702 2023-02-18 02:25:36.000000 imbrium-1.2.0/imbrium/blueprints/abstract_univariate.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.274491 imbrium-1.2.0/imbrium/predictors/
+-rw-rw-rw-   0        0        0      296 2023-02-26 18:46:56.000000 imbrium-1.2.0/imbrium/predictors/__init__.py
+-rw-rw-rw-   0        0        0    26529 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/predictors/multivarhybrid.py
+-rw-rw-rw-   0        0        0    44845 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/predictors/multivarpure.py
+-rw-rw-rw-   0        0        0    25879 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/predictors/univarhybrid.py
+-rw-rw-rw-   0        0        0    44457 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/predictors/univarpure.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.305818 imbrium-1.2.0/imbrium/utils/
+-rw-rw-rw-   0        0        0      129 2023-02-21 00:14:08.000000 imbrium-1.2.0/imbrium/utils/__init__.py
+-rw-rw-rw-   0        0        0     1111 2023-02-21 00:14:08.000000 imbrium-1.2.0/imbrium/utils/optimization.py
+-rw-rw-rw-   0        0        0      426 2023-04-11 19:14:21.000000 imbrium-1.2.0/imbrium/utils/scaler.py
+-rw-rw-rw-   0        0        0    10584 2023-01-09 01:24:32.000000 imbrium-1.2.0/imbrium/utils/transformer.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:05:07.195940 imbrium-1.2.0/imbrium.egg-info/
+-rw-rw-rw-   0        0        0    48846 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 21:05:06.000000 imbrium-1.2.0/imbrium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:05:07.321368 imbrium-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2023-03-12 18:30:22.000000 imbrium-1.2.0/setup.py
```

### Comparing `imbrium-1.1.0/CHANGELOG.md` & `imbrium-1.2.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,8 +63,14 @@
 
 - imbrium supports now:
   - python 3.7, 3.8, 3.9, 3.10
 
 ### 1.1.0
 
 - removed batch_size parameter from fit_model method
-- hyperparameter optimization added via the Optuna library
+- hyperparameter optimization added via the Optuna library
+
+
+### 1.2.0
+
+- added Tensorboard support
+- changed show_performance plot to show loss and metric values
```

### Comparing `imbrium-1.1.0/LICENSE` & `imbrium-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imbrium-1.1.0/imbrium/architectures/models.py` & `imbrium-1.2.0/imbrium/architectures/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import tensorflow as tf
 from tensorflow import keras
+from tensorflow.keras import regularizers
 from tensorflow.keras.layers import (GRU, LSTM, Bidirectional, Conv1D, Dense,
                                      Dropout, Flatten, MaxPooling1D,
                                      RepeatVector, SimpleRNN, TimeDistributed)
 
 
 def mlp(
     optimizer: str,
@@ -26,19 +27,34 @@
         model (object): Returns compiled Keras model.
     """
     model = keras.Sequential()
     model.add(
         Dense(
             layer_config["layer0"][0],
             activation=layer_config["layer0"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             input_dim=input_shape,
         )
     )
-    model.add(Dense(layer_config["layer1"][0], activation=layer_config["layer1"][1]))
-    model.add(Dense(layer_config["layer2"][0], activation=layer_config["layer2"][1]))
+    model.add(Dropout(layer_config["layer0"][3]))
+    model.add(
+        Dense(
+            layer_config["layer1"][0],
+            activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
+        )
+    )
+    model.add(Dropout(layer_config["layer1"][3]))
+    model.add(
+        Dense(
+            layer_config["layer2"][0],
+            activation=layer_config["layer2"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer2"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def rnn(
@@ -63,26 +79,34 @@
     """
     model = keras.Sequential()
     model.add(
         SimpleRNN(
             layer_config["layer0"][0],
             activation=layer_config["layer0"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][3]))
     model.add(
         SimpleRNN(
             layer_config["layer1"][0],
             activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
             return_sequences=True,
         )
     )
+    model.add(Dropout(layer_config["layer1"][3]))
     model.add(
-        SimpleRNN(layer_config["layer2"][0], activation=layer_config["layer2"][1])
+        SimpleRNN(
+            layer_config["layer2"][0],
+            activation=layer_config["layer2"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer2"][2]),
+        )
     )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
@@ -108,25 +132,35 @@
     """
     model = keras.Sequential()
     model.add(
         LSTM(
             layer_config["layer0"][0],
             activation=layer_config["layer0"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][3]))
     model.add(
         LSTM(
             layer_config["layer1"][0],
             activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
             return_sequences=True,
         )
     )
-    model.add(LSTM(layer_config["layer2"][0], activation=layer_config["layer2"][1]))
+    model.add(Dropout(layer_config["layer1"][3]))
+    model.add(
+        LSTM(
+            layer_config["layer2"][0],
+            activation=layer_config["layer2"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer2"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def cnn(
@@ -152,26 +186,36 @@
     model = keras.Sequential()
     model.add(
         Conv1D(
             filters=layer_config["layer0"][0],
             kernel_size=layer_config["layer0"][1],
             activation=layer_config["layer0"][2],
             input_shape=input_shape,
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][3]),
         )
     )
+    model.add(Dropout(layer_config["layer0"][4]))
     model.add(
         Conv1D(
             filters=layer_config["layer1"][0],
             kernel_size=layer_config["layer1"][1],
             activation=layer_config["layer1"][2],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][3]),
         )
     )
+    model.add(Dropout(layer_config["layer1"][4]))
     model.add(MaxPooling1D(pool_size=layer_config["layer2"]))
     model.add(Flatten())
-    model.add(Dense(layer_config["layer3"][0], activation=layer_config["layer3"][1]))
+    model.add(
+        Dense(
+            layer_config["layer3"][0],
+            activation=layer_config["layer3"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def gru(
@@ -196,25 +240,35 @@
     """
     model = keras.Sequential()
     model.add(
         GRU(
             layer_config["layer0"][0],
             activation=layer_config["layer0"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][3]))
     model.add(
         GRU(
             layer_config["layer1"][0],
             activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
             return_sequences=True,
         )
     )
-    model.add(GRU(layer_config["layer2"][0], activation=layer_config["layer2"][1]))
+    model.add(Dropout(layer_config["layer1"][3]))
+    model.add(
+        GRU(
+            layer_config["layer2"][0],
+            activation=layer_config["layer2"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer2"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def birnn(
@@ -240,20 +294,26 @@
     model = keras.Sequential()
     model.add(
         Bidirectional(
             SimpleRNN(
                 layer_config["layer0"][0],
                 activation=layer_config["layer0"][1],
                 return_sequences=True,
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             ),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][3]))
     model.add(
-        SimpleRNN(layer_config["layer1"][0], activation=layer_config["layer1"][1])
+        SimpleRNN(
+            layer_config["layer1"][0],
+            activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
+        )
     )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
@@ -280,19 +340,27 @@
     model = keras.Sequential()
     model.add(
         Bidirectional(
             LSTM(
                 layer_config["layer0"][0],
                 activation=layer_config["layer0"][1],
                 return_sequences=True,
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             ),
             input_shape=input_shape,
         )
     )
-    model.add(LSTM(layer_config["layer1"][0], activation=layer_config["layer1"][1]))
+    model.add(Dropout(layer_config["layer0"][3]))
+    model.add(
+        LSTM(
+            layer_config["layer1"][0],
+            activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
+        )
+    ),
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def bigru(
@@ -317,20 +385,28 @@
     """
     model = keras.Sequential()
     model.add(
         Bidirectional(
             GRU(
                 layer_config["layer0"][0],
                 activation=layer_config["layer0"][1],
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
                 return_sequences=True,
             ),
             input_shape=input_shape,
         )
     )
-    model.add(GRU(layer_config["layer1"][0], activation=layer_config["layer1"][1]))
+    model.add(Dropout(layer_config["layer0"][3]))
+    model.add(
+        GRU(
+            layer_config["layer1"][0],
+            activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def encdec_rnn(
@@ -356,33 +432,43 @@
     """
     model = keras.Sequential()
     model.add(
         SimpleRNN(
             layer_config["layer0"][0],
             activation=layer_config["layer0"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][3]))
     model.add(
-        SimpleRNN(layer_config["layer1"][0], activation=layer_config["layer1"][1])
+        SimpleRNN(
+            layer_config["layer1"][0],
+            activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
+        )
     )
+    model.add(Dropout(layer_config["layer1"][3]))
     model.add(RepeatVector(repeat))
     model.add(
         SimpleRNN(
             layer_config["layer2"][0],
             activation=layer_config["layer2"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer2"][2]),
         )
     )
+    model.add(Dropout(layer_config["layer2"][3]))
     model.add(
         SimpleRNN(
             layer_config["layer3"][0],
             activation=layer_config["layer3"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
         )
     )
     model.add(TimeDistributed(Dense(output_shape)))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
@@ -410,31 +496,43 @@
     """
     model = keras.Sequential()
     model.add(
         LSTM(
             layer_config["layer0"][0],
             activation=layer_config["layer0"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             input_shape=input_shape,
         )
     )
-    model.add(LSTM(layer_config["layer1"][0], activation=layer_config["layer1"][1]))
+    model.add(Dropout(layer_config["layer0"][3]))
+    model.add(
+        LSTM(
+            layer_config["layer1"][0],
+            activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
+        )
+    )
+    model.add(Dropout(layer_config["layer1"][3]))
     model.add(RepeatVector(repeat))
     model.add(
         LSTM(
             layer_config["layer2"][0],
             activation=layer_config["layer2"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
         )
     )
+    model.add(Dropout(layer_config["layer2"][3]))
     model.add(
         LSTM(
             layer_config["layer3"][0],
             activation=layer_config["layer3"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer2"][2]),
         )
     )
     model.add(TimeDistributed(Dense(output_shape)))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
@@ -463,38 +561,45 @@
     """
     model = keras.Sequential()
     model.add(
         Conv1D(
             layer_config["layer0"][0],
             kernel_size=layer_config["layer0"][1],
             activation=layer_config["layer0"][2],
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][3]),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][4]))
     model.add(
         Conv1D(
             filters=layer_config["layer1"][0],
             kernel_size=layer_config["layer1"][1],
-            activation=layer_config["layer0"][2],
+            activation=layer_config["layer1"][2],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][3]),
         )
     )
+    model.add(Dropout(layer_config["layer1"][4]))
     model.add(MaxPooling1D(pool_size=layer_config["layer2"]))
     model.add(Flatten())
     model.add(RepeatVector(repeat))
     model.add(
         GRU(
             layer_config["layer3"][0],
             activation=layer_config["layer3"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
             return_sequences=True,
         )
     )
+    model.add(Dropout(layer_config["layer3"][3]))
     model.add(
         GRU(
             layer_config["layer4"][0],
             activation=layer_config["layer4"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer4"][2]),
             return_sequences=True,
         )
     )
     model.add(TimeDistributed(Dense(output_shape)))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
@@ -523,30 +628,42 @@
     """
     model = keras.Sequential()
     model.add(
         GRU(
             layer_config["layer0"][0],
             activation=layer_config["layer0"][1],
             return_sequences=True,
+            kernel_regularizer=regularizers.L2(layer_config["layer0"][2]),
             input_shape=input_shape,
         )
     )
-    model.add(GRU(layer_config["layer1"][0], activation=layer_config["layer1"][1]))
+    model.add(Dropout(layer_config["layer0"][3]))
+    model.add(
+        GRU(
+            layer_config["layer1"][0],
+            activation=layer_config["layer1"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer1"][2]),
+        )
+    )
+    model.add(Dropout(layer_config["layer1"][3]))
     model.add(RepeatVector(repeat))
     model.add(
         GRU(
             layer_config["layer2"][0],
             activation=layer_config["layer2"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer2"][2]),
             return_sequences=True,
         )
     )
+    model.add(Dropout(layer_config["layer2"][3]))
     model.add(
         GRU(
             layer_config["layer3"][0],
             activation=layer_config["layer3"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
             return_sequences=True,
         )
     )
     model.add(TimeDistributed(Dense(output_shape)))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
@@ -575,38 +692,48 @@
     model = keras.Sequential()
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer0"][0],
                 kernel_size=layer_config["layer0"][1],
                 activation=layer_config["layer0"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][3]),
             ),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][4]))
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer1"][0],
                 kernel_size=layer_config["layer1"][1],
                 activation=layer_config["layer1"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer1"][3]),
             )
         )
     )
+    model.add(Dropout(layer_config["layer1"][4]))
     model.add(TimeDistributed(MaxPooling1D(pool_size=layer_config["layer2"])))
     model.add(TimeDistributed(Flatten()))
     model.add(
         SimpleRNN(
             layer_config["layer3"][0],
             activation=layer_config["layer3"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
             return_sequences=True,
         )
     )
+    model.add(Dropout(layer_config["layer3"][3]))
     model.add(
-        SimpleRNN(layer_config["layer4"][0], activation=layer_config["layer4"][1])
+        SimpleRNN(
+            layer_config["layer4"][0],
+            activation=layer_config["layer4"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer4"][2]),
+        )
     )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
@@ -633,37 +760,49 @@
     model = keras.Sequential()
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer0"][0],
                 kernel_size=layer_config["layer0"][1],
                 activation=layer_config["layer0"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][3]),
             ),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][4]))
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer1"][0],
                 kernel_size=layer_config["layer1"][1],
                 activation=layer_config["layer1"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer1"][3]),
             )
         )
     )
+    model.add(Dropout(layer_config["layer1"][4]))
     model.add(TimeDistributed(MaxPooling1D(pool_size=layer_config["layer2"])))
     model.add(TimeDistributed(Flatten()))
     model.add(
         LSTM(
             layer_config["layer3"][0],
             activation=layer_config["layer3"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
             return_sequences=True,
         )
     )
-    model.add(LSTM(layer_config["layer4"][0], activation=layer_config["layer4"][1]))
+    model.add(Dropout(layer_config["layer3"][3]))
+    model.add(
+        LSTM(
+            layer_config["layer4"][0],
+            activation=layer_config["layer4"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer4"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def cnngru(
@@ -689,37 +828,49 @@
     model = keras.Sequential()
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer0"][0],
                 kernel_size=layer_config["layer0"][1],
                 activation=layer_config["layer0"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][3]),
             ),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][4]))
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer1"][0],
                 kernel_size=layer_config["layer1"][1],
                 activation=layer_config["layer1"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer1"][3]),
             )
         )
     )
+    model.add(Dropout(layer_config["layer1"][4]))
     model.add(TimeDistributed(MaxPooling1D(pool_size=layer_config["layer2"])))
     model.add(TimeDistributed(Flatten()))
     model.add(
         GRU(
             layer_config["layer3"][0],
             activation=layer_config["layer3"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
             return_sequences=True,
         )
     )
-    model.add(GRU(layer_config["layer4"][0], activation=layer_config["layer4"][1]))
+    model.add(Dropout(layer_config["layer3"][3]))
+    model.add(
+        GRU(
+            layer_config["layer4"][0],
+            activation=layer_config["layer4"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer4"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def cnnbirnn(
@@ -745,40 +896,50 @@
     model = keras.Sequential()
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer0"][0],
                 kernel_size=layer_config["layer0"][1],
                 activation=layer_config["layer0"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][3]),
             ),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][4]))
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer1"][0],
                 kernel_size=layer_config["layer1"][1],
                 activation=layer_config["layer1"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer1"][3]),
             )
         )
     )
+    model.add(Dropout(layer_config["layer1"][4]))
     model.add(TimeDistributed(MaxPooling1D(pool_size=layer_config["layer2"])))
     model.add(TimeDistributed(Flatten()))
     model.add(
         Bidirectional(
             SimpleRNN(
                 layer_config["layer3"][0],
                 activation=layer_config["layer3"][1],
+                kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
                 return_sequences=True,
             )
         )
     )
+    model.add(Dropout(layer_config["layer3"][3]))
     model.add(
-        SimpleRNN(layer_config["layer4"][0], activation=layer_config["layer4"][1])
+        SimpleRNN(
+            layer_config["layer4"][0],
+            activation=layer_config["layer4"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer4"][2]),
+        )
     )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
@@ -805,39 +966,51 @@
     model = keras.Sequential()
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer0"][0],
                 kernel_size=layer_config["layer0"][1],
                 activation=layer_config["layer0"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][3]),
             ),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][4]))
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer1"][0],
                 kernel_size=layer_config["layer1"][1],
                 activation=layer_config["layer1"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer1"][3]),
             )
         )
     )
+    model.add(Dropout(layer_config["layer1"][4]))
     model.add(TimeDistributed(MaxPooling1D(pool_size=layer_config["layer2"])))
     model.add(TimeDistributed(Flatten()))
     model.add(
         Bidirectional(
             LSTM(
                 layer_config["layer3"][0],
                 activation=layer_config["layer3"][1],
+                kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
                 return_sequences=True,
             )
         )
     )
-    model.add(LSTM(layer_config["layer4"][0], activation=layer_config["layer4"][1]))
+    model.add(Dropout(layer_config["layer3"][3]))
+    model.add(
+        LSTM(
+            layer_config["layer4"][0],
+            activation=layer_config["layer4"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer4"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
 
 
 def cnnbigru(
@@ -863,36 +1036,48 @@
     model = keras.Sequential()
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer0"][0],
                 kernel_size=layer_config["layer0"][1],
                 activation=layer_config["layer0"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer0"][3]),
             ),
             input_shape=input_shape,
         )
     )
+    model.add(Dropout(layer_config["layer0"][4]))
     model.add(
         TimeDistributed(
             Conv1D(
                 filters=layer_config["layer1"][0],
                 kernel_size=layer_config["layer1"][1],
                 activation=layer_config["layer1"][2],
+                kernel_regularizer=regularizers.L2(layer_config["layer1"][3]),
             )
         )
     )
+    model.add(Dropout(layer_config["layer1"][4]))
     model.add(TimeDistributed(MaxPooling1D(pool_size=layer_config["layer2"])))
     model.add(TimeDistributed(Flatten()))
     model.add(
         Bidirectional(
             GRU(
                 layer_config["layer3"][0],
                 activation=layer_config["layer3"][1],
+                kernel_regularizer=regularizers.L2(layer_config["layer3"][2]),
                 return_sequences=True,
             )
         )
     )
-    model.add(GRU(layer_config["layer4"][0], activation=layer_config["layer4"][1]))
+    model.add(Dropout(layer_config["layer3"][3]))
+    model.add(
+        GRU(
+            layer_config["layer4"][0],
+            activation=layer_config["layer4"][1],
+            kernel_regularizer=regularizers.L2(layer_config["layer4"][2]),
+        )
+    )
     model.add(Dense(output_shape))
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
 
     return model
```

### Comparing `imbrium-1.1.0/imbrium/blueprints/abstract_multivariate.py` & `imbrium-1.2.0/imbrium/blueprints/abstract_multivariate.py`

 * *Files identical despite different names*

### Comparing `imbrium-1.1.0/imbrium/blueprints/abstract_univariate.py` & `imbrium-1.2.0/imbrium/blueprints/abstract_univariate.py`

 * *Files identical despite different names*

### Comparing `imbrium-1.1.0/imbrium/predictors/multivarhybrid.py` & `imbrium-1.2.0/imbrium/predictors/multivarhybrid.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import os
 
 import matplotlib.pyplot as plt
 import tensorflow as tf
 from numpy import array, empty, reshape
 from pandas import DataFrame
 from tensorflow import keras
@@ -176,19 +177,19 @@
 
     def create_cnnrnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
         """Creates CNN-RNN hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -214,19 +215,19 @@
 
     def create_cnnlstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
         """Creates CNN-LSTM hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -252,19 +253,19 @@
 
     def create_cnngru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
         """Creates CNN-GRU hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -290,19 +291,19 @@
 
     def create_cnnbirnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
         """Creates CNN-BI-RNN hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -328,19 +329,19 @@
 
     def create_cnnbilstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
         """Creates CNN-BI-LSTM hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -366,19 +367,19 @@
 
     def create_cnnbigru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
         """Creates CNN-BI-GRU hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -403,59 +404,126 @@
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             validation_split (float): Determines size of Validation data.
+            board (bool): Creates TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
-            self.details = self.model.fit(
-                self.input_x,
-                self.input_y,
-                validation_split=validation_split,
-                epochs=epochs,
-                verbose=show_progress,
-            )
+            if board == True:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback_board],
+                )
+            else:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                )
+
         else:
-            callback = EarlyStopping(**callback_setting)
-            self.details = self.model.fit(
-                self.input_x,
-                self.input_y,
-                validation_split=validation_split,
-                epochs=epochs,
-                verbose=show_progress,
-                callbacks=[callback],
-            )
+            if board == True:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                callback = EarlyStopping(**callback_setting)
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback, callback_board],
+                )
+            else:
+                callback = EarlyStopping(**callback_setting)
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback],
+                )
         return self.details
 
     def model_blueprint(self):
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
-    def show_performance(self):
-        """Plots model loss, validation loss over time."""
+    def show_performance(self, metric_name: str = ""):
+        """Plots model loss and a given metric over time."""
         information = self.details
 
-        plt.plot(information.history["loss"], color="black")
-        plt.plot(information.history["val_loss"], color="gold")
-        plt.title(self.model_id + " Model Loss")
-        plt.ylabel(self.loss)
-        plt.xlabel("Epoch")
-        plt.legend(["Train", "Test"], loc="upper right")
-        plt.tight_layout()
-        plt.show()
+        plt.style.use("dark_background")
+
+        colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+
+        if metric_name == "":
+
+            plt.plot(information.history["loss"], color=colors[0])
+            plt.plot(information.history["val_loss"], color=colors[1])
+            plt.title(self.model_id + " Model Loss")
+            plt.ylabel(self.loss)
+            plt.xlabel("Epoch")
+            plt.legend(["Train", "Test"], loc="upper right")
+            plt.tight_layout()
+            plt.show()
+        else:
+            plt.plot(information.history["loss"], color=colors[0])
+            plt.plot(information.history["val_loss"], color=colors[1])
+            plt.plot(information.history[metric_name], color=colors[2])
+            plt.plot(information.history["val_" + metric_name], color=colors[3])
+            plt.title(self.model_id + " Model Performance")
+            plt.ylabel(metric_name)
+            plt.xlabel("Epoch")
+            plt.legend(
+                [
+                    "Train Loss",
+                    "Test Loss",
+                    "Train " + metric_name,
+                    "Test " + metric_name,
+                ],
+                loc="upper right",
+            )
+            plt.tight_layout()
+            plt.show()
 
     def predict(self, data: array) -> DataFrame:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (DataFrame): Forecast for sequence provided.
@@ -490,192 +558,204 @@
 class OptimizeHybridMulti(HybridMulti):
     def create_fit_cnnrnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-RNN hybrid model."""
         self.create_cnnrnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnlstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-LSTM hybrid model."""
         self.create_cnnlstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnngru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-GRU hybrid model."""
         self.create_cnngru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbirnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiRNN hybrid model."""
         self.create_cnnbirnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbilstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiLSTM hybrid model."""
         self.create_cnnbilstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnnbigru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config={
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (25, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates CNN-BiGRU hybrid model."""
         self.create_cnnbigru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
```

### Comparing `imbrium-1.1.0/imbrium/predictors/multivarpure.py` & `imbrium-1.2.0/imbrium/predictors/univarhybrid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,135 @@
+import datetime
 import os
 
 import matplotlib.pyplot as plt
 import tensorflow as tf
-from numpy import array, empty, reshape
+from numpy import array, reshape
 from pandas import DataFrame
 from tensorflow import keras
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.layers import (GRU, LSTM, Bidirectional, Conv1D, Dense,
-                                     Dropout, Flatten, MaxPooling1D, SimpleRNN)
+                                     Dropout, Flatten, MaxPooling1D, SimpleRNN,
+                                     TimeDistributed)
 
 from imbrium.architectures.models import *
-from imbrium.blueprints.abstract_multivariate import MultiVariateMultiStep
+from imbrium.blueprints.abstract_univariate import UniVariateMultiStep
 from imbrium.utils.scaler import SCALER
-from imbrium.utils.transformer import data_prep_multi, multistep_prep_standard
+from imbrium.utils.transformer import data_prep_uni, sequence_prep_hybrid_uni
 
 
-class PureMulti(MultiVariateMultiStep):
-    """Implements deep neural networks based on multivariate multipstep
-    standard predictors.
-
-     Methods
-     -------
-     set_model_id(self, name: str):
-         Setter method to change model id name.
-     get_model_id(self) -> array:
-         Getter method to retrieve model id used.
-     get_X_input(self) -> array:
-         Getter method to retrieve transformed X input - training.
-     get_X_input_shape(self) -> tuple:
-         Getter method to retrieve transformed X shape.
-     get_y_input(self) -> array:
-         Getter method to retrieve transformed y input - target.
-     get_y_input_shape(self) -> array:
-         Getter method to retrieve transformed y input shape.
-     get_optimizer(self) -> str:
-         Getter method to retrieve model optimizer used.
-     get_loss(self) -> str:
-         Getter method to retrieve used model loss.
-     get_metrics(self) -> str:
-         Getter method to retrieve model evaluation metrics used.
-     create_mlp(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (50, 'relu'), 'layer1': (25,'relu'),
-     'layer2': (25, 'relu')}):
-         Builds MLP structure.
-     create_rnn(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (40, 'relu'), 'layer1': (50,'relu'),
-     'layer2': (50, 'relu')}):
-         Builds RNN structure.
-     create_lstm(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (40, 'relu'), 'layer1': (50,'relu'),
-     'layer2': (50, 'relu')}):
-         Builds LSTM structure.
-     create_cnn(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (64, 1, 'relu'), 'layer1': (32, 1, 'relu'),
-     'layer2': (2), 'layer3': (50, 'relu')}):
-         Builds CNN structure.
-     create_gru(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (40, 'relu'), 'layer1': (50,'relu'),
-     'layer2': (50, 'relu')}):
-         Builds GRU structure.
-     create_birnn(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (50, 'relu'), 'layer1': (50, 'relu')}):
-         Builds bidirectional RNN structure.
-     create_bilstm(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (50, 'relu'), 'layer1': (50, 'relu')}):
-         Builds bidirectional LSTM structure.
-     create_bigru(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (50, 'relu'), 'layer1': (50, 'relu')}):
-         Builds bidirectional GRU structure.
-     create_encdec_rnn(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (100, 'relu'), 'layer1': (50, 'relu'),
-     'layer2': (50, 'relu'), 'layer3': (100, 'relu')}):
-         Builds encoder decoder RNN structure.
-     create_encdec_lstm(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (100, 'relu'), 'layer1': (50, 'relu'),
-     'layer2': (50, 'relu'), 'layer3': (100, 'relu')}):
-         Builds encoder decoder LSTM structure.
-     create_encdec_gru(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (100, 'relu'), 'layer1': (50, 'relu'),
-     'layer2': (50, 'relu'), 'layer3': (100, 'relu')}):
-         Builds encoder decoder GRU structure.
-     create_encdec_cnn(self, optimizer: str = 'adam',
-     loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
-     layer_config: dict = {'layer0': (64, 1, 'relu'), 'layer1': (32, 1, 'relu'),
-     'layer2': (2), 'layer3': (50, 'relu'), 'layer4': (100, 'relu')}):
-         Builds encoder decoder CNN structure.
-     fit_model(self, epochs: int, show_progress: int = 1,
-     validation_split: float = 0.20,
-     **callback_setting: dict):
-         Fitting model onto provided data.
-     model_blueprint(self):
-         Print blueprint of layer structure.
-     show_performance(self):
-         Evaluate and plot model performance.
-     predict(self, data: array):
-         Takes in input data and outputs model forecasts.
-     save_model(self, absolute_path: str = CURRENT_PATH):
-         Saves current Keras model to current directory.
-     load_model(self, location: str):
-         Load model from location specified.
+class HybridUni(UniVariateMultiStep):
+    """Implements neural network based univariate multipstep hybrid predictors.
+
+    Methods
+    -------
+    set_model_id(self, name: str):
+        Setter method to change model id name.
+    get_model_id(self) -> array:
+        Getter method to retrieve model id used.
+    get_X_input(self) -> array:
+        Getter method to retrieve transformed X input - training.
+    get_X_input_shape(self) -> tuple:
+        Getter method to retrieve transformed X shape.
+    get_y_input(self) -> array:
+        Getter method to retrieve transformed y input - target.
+    get_y_input_shape(self) -> array:
+        Getter method to retrieve transformed y input shape.
+    get_optimizer(self) -> str:
+        Getter method to retrieve model optimizer used.
+    get_loss(self) -> str:
+        Getter method to retrieve used model loss.
+    get_metrics(self) -> str:
+        Getter method to retrieve model evaluation metrics used.
+    create_cnnrnn(self, optimizer: str = 'adam',
+    loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
+    layer_config = {'layer0': (64, 1, 'relu'), 'layer1': (32, 1, 'relu'),
+    'layer2': (2), 'layer3': (50, 'relu'), 'layer4': (25, 'relu')}):
+        Builds CNN-RNN structure.
+    create_cnnlstm(self, optimizer: str = 'adam',
+    loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
+    layer_config = {'layer0': (64, 1, 'relu'), 'layer1': (32, 1, 'relu'),
+    'layer2': (2), 'layer3': (50, 'relu'), 'layer4': (25, 'relu')}):
+        Builds CNN-LSTM structure.
+    create_cnngru(self, optimizer: str = 'adam',
+    loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
+    layer_config = {'layer0': (64, 1, 'relu'), 'layer1': (32, 1, 'relu'),
+    'layer2': (2), 'layer3': (50, 'relu'), 'layer4': (25, 'relu')}):
+        Builds CNN-GRU structure.
+    create_cnnbirnn(self, optimizer: str = 'adam',
+    loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
+    layer_config = {'layer0': (64, 1, 'relu'), 'layer1': (32, 1, 'relu'),
+    'layer2': (2), 'layer3': (50, 'relu'), 'layer4': (25, 'relu')}):
+        Buidls CNN bidirectional RNN structure.
+    create_cnnbilstm(self, optimizer: str = 'adam',
+    loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
+    layer_config = {'layer0': (64, 1, 'relu'), 'layer1': (32, 1, 'relu'),
+    'layer2': (2), 'layer3': (50, 'relu'), 'layer4': (25, 'relu')}):
+        Builds CNN bidirectional LSTM structure.
+    create_cnnbigru(self, optimizer: str = 'adam',
+    loss: str = 'mean_squared_error', metrics: str = 'mean_squared_error',
+    layer_config = {'layer0': (64, 1, 'relu'), 'layer1': (32, 1, 'relu'),
+    'layer2': (2), 'layer3': (50, 'relu'), 'layer4': (25, 'relu')}):
+        Builds CNN bidirectional GRU structure.
+    fit_model(self, epochs: int, show_progress: int = 1,
+    validation_split: float = 0.20,
+    **callback_setting: dict):
+        Fitting model onto provided data.
+    model_blueprint(self):
+        Print blueprint of layer structure.
+    show_performance(self):
+        Evaluate and plot model performance.
+    predict(self, data: array):
+        Takes in input data and outputs model forecasts.
+    save_model(self, absolute_path: str = CURRENT_PATH):
+        Saves current Keras model to current directory.
+    load_model(self, location: str):
+        Load model from location specified.
     """
 
     CURRENT_PATH = os.getcwd()
 
     def __init__(
         self,
+        sub_seq: int,
         steps_past: int,
         steps_future: int,
         data=DataFrame(),
-        features=[],
         scale: str = "",
     ) -> object:
         """
         Parameters:
+            sub_seq (int): Further division of given steps a predictor will
+            look backward.
             steps_past (int): Steps predictor will look backward.
             steps_future (int): Steps predictor will look forward.
-            data (DataFrame): Input data for model training.
-            features (list): List of features. First feature in list will be
-            set to the target variable.
+            data (array): Input data for model training. Default is empty to
+            enable loading pre-trained models.
             scale (str): How to scale the data before making predictions.
         """
-        self.scaler = SCALER[scale]
-        self.model_id = ""
+        self.sub_seq = sub_seq
+        self.steps_past = steps_past
+        self.steps_future = steps_future
         self.optimizer = ""
         self.loss = ""
         self.metrics = ""
 
+        self.scaler = SCALER[scale]
+
         if len(data) > 0:
-            self.data = data_prep_multi(data, features, self.scaler)
-            self.input_x, self.input_y = multistep_prep_standard(
-                self.data, steps_past, steps_future
+            self.data = array(data)
+            self.data = data_prep_uni(data, self.scaler)
+            self.input_x, self.input_y, self.modified_back = sequence_prep_hybrid_uni(
+                self.data, sub_seq, steps_past, steps_future
             )
         else:
             self.data = data
 
+        self.model_id = ""
+
     def set_model_id(self, name: str):
         """Setter method to change model id field.
         Parameters:
             name (str): Name for selected Model.
         """
         self.model_id = name
 
@@ -188,477 +169,353 @@
         return self.loss
 
     @property
     def get_metrics(self) -> str:
         """Get metrics."""
         return self.metrics
 
-    def create_mlp(
+    def create_cnnrnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (50, "relu"),
-            "layer1": (25, "relu"),
-            "layer2": (25, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
-        """Creates MLP model.
+        """Creates CNN-RNN hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
         """
-        self.set_model_id("MLP")
+        self.set_model_id("CNN-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
-        # necessary to account for hyperparameter optimization
-        try:
-            self.input_x = self.backup_input_x
-        except:
-            self.backup_input_x = self.input_x.copy()
-
-        self.dimension = self.input_x.shape[1] * self.input_x.shape[2]
-
-        self.input_x = self.input_x.reshape((self.input_x.shape[0], self.dimension))
-
-        self.model = mlp(
+        self.model = cnnrnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
-            input_shape=self.input_x.shape[1],
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
-    def create_rnn(
+    def create_cnnlstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
-        """Creates RNN model.
+        """Creates CNN-LSTM hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
         """
-        self.set_model_id("RNN")
+        self.set_model_id("CNN-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
-        self.model = rnn(
+        self.model = cnnlstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
-    def create_lstm(
+    def create_cnngru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
-        """Creates LSTM model.
+        """Creates CNN-GRU hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
         """
-        self.set_model_id("LSTM")
+        self.set_model_id("CNN-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
-        self.model = lstm(
+        self.model = cnngru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
-    def create_cnn(
+    def create_cnnbirnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
-        """Creates CNN model.
+        """Creates CNN-BI-RNN hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
         """
-        self.set_model_id("CNN")
+        self.set_model_id("CNN-BI-RNN")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
-        self.model = cnn(
+        self.model = cnnbirnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
-    def create_gru(
+    def create_cnnbilstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
-        """Creates GRU model.
-        Parameters:
-            optimizer (str): Optimization algorithm.
-            loss (str): Loss function.
-            metrics (str): Performance measurement.
-            layer_config (dict): Adjust neurons and acitivation functions.
-        """
-        self.set_model_id("GRU")
-        self.optimizer = optimizer
-        self.loss = loss
-        self.metrics = metrics
-
-        self.model = gru(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
-            output_shape=self.input_y.shape[1],
-        )
-
-    def create_birnn(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
-    ):
-        """Creates BI-RNN model.
-        Parameters:
-            optimizer (str): Optimization algorithm.
-            loss (str): Loss function.
-            metrics (str): Performance measurement.
-            layer_config (dict): Adjust neurons and acitivation functions.
-        """
-        self.set_model_id("BI-RNN")
-        self.optimizer = optimizer
-        self.loss = loss
-        self.metrics = metrics
-
-        self.model = birnn(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
-            output_shape=self.input_y.shape[1],
-        )
-
-    def create_bilstm(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
-    ):
-        """Creates BI-LSTM model.
-        Parameters:
-            optimizer (str): Optimization algorithm.
-            loss (str): Loss function.
-            metrics (str): Performance measurement.
-            layer_config (dict): Adjust neurons and acitivation functions.
-        """
-        self.set_model_id("BI-LSTM")
-        self.optimizer = optimizer
-        self.loss = loss
-        self.metrics = metrics
-
-        self.model = bilstm(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
-            output_shape=self.input_y.shape[1],
-        )
-
-    def create_bigru(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
-    ):
-        """Creates BI-GRU model.
+        """Creates CNN-BI-LSTM hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
         """
-        self.set_model_id("BI-GRU")
+        self.set_model_id("CNN-BI-LSTM")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
-        self.model = bigru(
+        self.model = cnnbilstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
+            input_shape=(None, self.modified_back, 1),
             output_shape=self.input_y.shape[1],
         )
 
-    def create_encdec_rnn(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
-        },
-    ):
-        """Creates Encoder-Decoder-RNN model model.
-        Parameters:
-            optimizer (str): Optimization algorithm.
-            loss (str): Loss function.
-            metrics (str): Performance measurement.
-            layer_config (dict): Adjust neurons and acitivation functions.
-        """
-        self.set_model_id("Encoder-Decoder-RNN")
-        self.optimizer = optimizer
-        self.loss = loss
-        self.metrics = metrics
-
-        self.model = encdec_rnn(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
-            output_shape=1,
-            repeat=self.input_y.shape[1],
-        )
-
-    def create_encdec_lstm(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
-        },
-    ):
-        """Creates Encoder-Decoder-LSTM model model.
-        Parameters:
-            optimizer (str): Optimization algorithm.
-            loss (str): Loss function.
-            metrics (str): Performance measurement.
-            layer_config (dict): Adjust neurons and acitivation functions.
-        """
-        self.set_model_id("Encoder-Decoder-LSTM")
-        self.optimizer = optimizer
-        self.loss = loss
-        self.metrics = metrics
-
-        self.model = encdec_lstm(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
-            output_shape=1,
-            repeat=self.input_y.shape[1],
-        )
-
-    def create_encdec_gru(
+    def create_cnnbigru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
-        },
-    ):
-        """Creates Encoder-Decoder-GRU model model.
-        Parameters:
-            optimizer (str): Optimization algorithm.
-            loss (str): Loss function.
-            metrics (str): Performance measurement.
-            layer_config (dict): Adjust neurons and acitivation functions.
-        """
-        self.set_model_id("Encoder-Decoder-GRU")
-        self.optimizer = optimizer
-        self.loss = loss
-        self.metrics = metrics
-
-        self.model = encdec_gru(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
-            output_shape=1,
-            repeat=self.input_y.shape[1],
-        )
-
-    def create_encdec_cnn(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (100, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
     ):
-        """Creates Encoder-Decoder-CNN model.
-        Encoding via CNN and Decoding via GRU.
+        """Creates CNN-BI-GRU hybrid model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
         """
-        self.set_model_id("Encoder(CNN)-Decoder(GRU)")
+        self.set_model_id("CNN-BI-GRU")
         self.optimizer = optimizer
         self.loss = loss
         self.metrics = metrics
 
-        self.model = encdec_cnn(
+        self.model = cnnbigru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
-            input_shape=(self.input_x.shape[1], self.input_x.shape[2]),
-            output_shape=1,
-            repeat=self.input_y.shape[1],
+            input_shape=(None, self.modified_back, 1),
+            output_shape=self.input_y.shape[1],
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             validation_split (float): Determines size of Validation data.
+            board (bool): Create TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
-            self.details = self.model.fit(
-                self.input_x,
-                self.input_y,
-                validation_split=validation_split,
-                epochs=epochs,
-                verbose=show_progress,
-            )
+            if board == True:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback_board],
+                )
+            else:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                )
+
         else:
-            callback = EarlyStopping(**callback_setting)
-            self.details = self.model.fit(
-                self.input_x,
-                self.input_y,
-                validation_split=validation_split,
-                epochs=epochs,
-                verbose=show_progress,
-                callbacks=[callback],
-            )
+            if board == True:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                callback = EarlyStopping(**callback_setting)
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback, callback_board],
+                )
+            else:
+                callback = EarlyStopping(**callback_setting)
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback],
+                )
         return self.details
 
     def model_blueprint(self):
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
-    def show_performance(self):
-        """Plots model loss, validation loss over time."""
+    def show_performance(self, metric_name: str = ""):
+        """Plots model loss and a given metric over time."""
         information = self.details
 
-        plt.plot(information.history["loss"], color="black")
-        plt.plot(information.history["val_loss"], color="green")
-        plt.title(self.model_id + " Model Loss")
-        plt.ylabel(self.loss)
-        plt.xlabel("Epoch")
-        plt.legend(["Train", "Test"], loc="upper right")
-        plt.tight_layout()
-        plt.show()
+        plt.style.use("dark_background")
+
+        colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+
+        if metric_name == "":
+
+            plt.plot(information.history["loss"], color=colors[0])
+            plt.plot(information.history["val_loss"], color=colors[1])
+            plt.title(self.model_id + " Model Loss")
+            plt.ylabel(self.loss)
+            plt.xlabel("Epoch")
+            plt.legend(["Train", "Test"], loc="upper right")
+            plt.tight_layout()
+            plt.show()
+        else:
+            plt.plot(information.history["loss"], color=colors[0])
+            plt.plot(information.history["val_loss"], color=colors[1])
+            plt.plot(information.history[metric_name], color=colors[2])
+            plt.plot(information.history["val_" + metric_name], color=colors[3])
+            plt.title(self.model_id + " Model Performance")
+            plt.ylabel(metric_name)
+            plt.xlabel("Epoch")
+            plt.legend(
+                [
+                    "Train Loss",
+                    "Test Loss",
+                    "Train " + metric_name,
+                    "Test " + metric_name,
+                ],
+                loc="upper right",
+            )
+            plt.tight_layout()
+            plt.show()
 
     def predict(self, data: array) -> DataFrame:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (DataFrame): Forecast for sequence provided.
         """
+        data = array(data)
+        data = data.reshape(-1, 1)
+
         self.scaler.fit(data)
         data = self.scaler.transform(data)
 
-        dimension = data.shape[0] * data.shape[1]  # MLP case
+        shape_ = int((data.shape[1] * self.steps_past) / self.sub_seq)
+        data = data.reshape(1, self.sub_seq, shape_, 1)
 
-        try:
-            data = data.reshape((1, data.shape[0], data.shape[1]))  # All other models
-            y_pred = self.model.predict(data, verbose=0)
-
-        except BaseException:
-            data = data.reshape((1, dimension))  # MLP case
-            y_pred = self.model.predict(data, verbose=0)
+        y_pred = self.model.predict(data, verbose=0)
 
         y_pred = y_pred.reshape(y_pred.shape[1], y_pred.shape[0])
 
         return DataFrame(y_pred, columns=[f"{self.model_id}"])
 
     def save_model(self, absolute_path: str = CURRENT_PATH):
         """Save the current model to the current directory.
@@ -671,360 +528,211 @@
         """Load a keras model from the path specified.
         Parameters:
             location (str): Path of keras model location.
         """
         self.model = keras.models.load_model(location)
 
 
-class OptimizePureMulti(PureMulti):
-    def create_fit_mlp(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (50, "relu"),
-            "layer1": (25, "relu"),
-            "layer2": (25, "relu"),
-        },
-        epochs: int = 100,
-        show_progress: int = 1,
-        validation_split: float = 0.20,
-        **callback_setting: dict,
-    ):
-        """Creates and trains a Multi-Layer-Perceptron model."""
-        self.create_mlp(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-        )
-        self.fit_model(
-            epochs=epochs,
-            show_progress=show_progress,
-            validation_split=validation_split,
-            **callback_setting,
-        )
-        return self.details.history[metrics][-1]
-
-    def create_fit_rnn(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-        },
-        epochs: int = 100,
-        show_progress: int = 1,
-        validation_split: float = 0.20,
-        **callback_setting: dict,
-    ):
-        """Creates and trains a RNN model."""
-        self.create_rnn(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-        )
-        self.fit_model(
-            epochs=epochs,
-            show_progress=show_progress,
-            validation_split=validation_split,
-            **callback_setting,
-        )
-        return self.details.history[metrics][-1]
-
-    def create_fit_lstm(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-        },
-        epochs: int = 100,
-        show_progress: int = 1,
-        validation_split: float = 0.20,
-        **callback_setting: dict,
-    ):
-        """Creates and trains a LSTM model."""
-        self.create_lstm(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-        )
-        self.fit_model(
-            epochs=epochs,
-            show_progress=show_progress,
-            validation_split=validation_split,
-            **callback_setting,
-        )
-        return self.details.history[metrics][-1]
-
-    def create_fit_cnn(
+class OptimizeHybridUni(HybridUni):
+    def create_fit_cnnrnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
-        """Creates and trains a CNN model."""
-        self.create_cnn(
+        """Creates CNN-RNN hybrid model."""
+        self.create_cnnrnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
-    def create_fit_gru(
+    def create_fit_cnnlstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
-        """Creates and trains a GRU model."""
-        self.create_gru(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-        )
-        self.fit_model(
-            epochs=epochs,
-            show_progress=show_progress,
-            validation_split=validation_split,
-            **callback_setting,
-        )
-        return self.details.history[metrics][-1]
-
-    def create_fit_birnn(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
-        epochs: int = 100,
-        show_progress: int = 1,
-        validation_split: float = 0.20,
-        **callback_setting: dict,
-    ):
-        """Creates and trains a BI-RNN model."""
-        self.create_birnn(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-        )
-        self.fit_model(
-            epochs=epochs,
-            show_progress=show_progress,
-            validation_split=validation_split,
-            **callback_setting,
-        )
-        return self.details.history[metrics][-1]
-
-    def create_fit_bilstm(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
-        epochs: int = 100,
-        show_progress: int = 1,
-        validation_split: float = 0.20,
-        **callback_setting: dict,
-    ):
-        """Creates and trains a BI-LSTM model."""
-        self.create_bilstm(
+        """Creates CNN-LSTM hybrid model."""
+        self.create_cnnlstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
-    def create_fit_bigru(
+    def create_fit_cnngru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
-        epochs: int = 100,
-        show_progress: int = 1,
-        validation_split: float = 0.20,
-        **callback_setting: dict,
-    ):
-        """Creates and trains a BI-GRU model."""
-        self.create_bigru(
-            optimizer=optimizer,
-            loss=loss,
-            metrics=metrics,
-            layer_config=layer_config,
-        )
-        self.fit_model(
-            epochs=epochs,
-            show_progress=show_progress,
-            validation_split=validation_split,
-            **callback_setting,
-        )
-        return self.details.history[metrics][-1]
-
-    def create_fit_encdec_rnn(
-        self,
-        optimizer: str = "adam",
-        loss: str = "mean_squared_error",
-        metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
-        """Creates and trains an encoder-decoder RNN model."""
-        self.create_encdec_rnn(
+        """Creates CNN-GRU hybrid model."""
+        self.create_cnngru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
-    def create_fit_encdec_lstm(
+    def create_fit_cnnbirnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
-        """Creates and trains an encoder-decoder LSTM model."""
-        self.create_encdec_lstm(
+        """Creates CNN-BiRNN hybrid model."""
+        self.create_cnnbirnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
-    def create_fit_encdec_gru(
+    def create_fit_cnnbilstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
-        """Creates and trains an encoder-decoder GRU model."""
-        self.create_encdec_gru(
+        """Creates CNN-BiLSTM hybrid model."""
+        self.create_cnnbilstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
-    def create_fit_encdec_cnn(
+    def create_fit_cnnbigru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+        layer_config={
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
+            "layer2": (2),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (25, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
-        """Creates and trains an encoder-decoder CNN model."""
-        self.create_encdec_cnn(
+        """Creates CNN-BiGRU hybrid model."""
+        self.create_cnnbigru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
```

### Comparing `imbrium-1.1.0/imbrium/predictors/univarpure.py` & `imbrium-1.2.0/imbrium/predictors/univarpure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import os
 
 import matplotlib.pyplot as plt
 import tensorflow as tf
 from numpy import array, empty, reshape
 from pandas import DataFrame
 from tensorflow import keras
@@ -188,17 +189,27 @@
 
     def create_mlp(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (50, "relu"),
-            "layer1": (25, "relu"),
-            "layer2": (25, "relu"),
+            "layer0": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                25,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (25, "relu", 0.0),  # (neurons, activation, regularization)
         },
     ):
         """Creates MLP model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -224,17 +235,27 @@
 
     def create_rnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+            "layer0": (
+                40,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (50, "relu", 0.0),  # (neurons, activation, regularization)
         },
     ):
         """Creates RNN model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -256,17 +277,27 @@
 
     def create_lstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+            "layer0": (
+                40,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (50, "relu", 0.0),  # (neurons, activation, regularization)
         },
     ):
         """Creates LSTM model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -288,18 +319,30 @@
 
     def create_cnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
-            "layer2": (2),
-            "layer3": (50, "relu"),
+            "layer0": (
+                64,
+                1,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, kernel_size, activation, regularization, dropout)
+            "layer1": (
+                32,
+                1,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, kernel_size, activation, regularization, dropout)
+            "layer2": (2),  # pooling
+            "layer3": (50, "relu", 0.0),  # (neurons, activation, regularization)
         },
     ):
         """Creates CNN model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -321,17 +364,27 @@
 
     def create_gru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+            "layer0": (
+                40,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (50, "relu", 0.0),  # (neurons, activation, regularization)
         },
     ):
         """Creates GRU model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -352,15 +405,18 @@
         )
 
     def create_birnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
+        layer_config: dict = {
+            "layer0": (50, "relu", 0.0, 0.0),
+            "layer1": (50, "relu", 0.0),
+        },  # (neurons, activation, regularization, dropout)
     ):
         """Creates BI-RNN model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
@@ -380,15 +436,18 @@
         )
 
     def create_bilstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
+        layer_config: dict = {
+            "layer0": (50, "relu", 0.0, 0.0),
+            "layer1": (50, "relu", 0.0),
+        },
     ):
         """Creates BI-LSTM model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
@@ -408,15 +467,18 @@
         )
 
     def create_bigru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
+        layer_config: dict = {
+            "layer0": (50, "relu", 0.0, 0.0),
+            "layer1": (50, "relu", 0.0),
+        },
     ):
         """Creates BI-GRU model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
             layer_config (dict): Adjust neurons and acitivation functions.
@@ -437,18 +499,33 @@
 
     def create_encdec_rnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+            "layer0": (
+                100,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer3": (100, "relu", 0.0),  # (neurons, activation, regularization)
         },
     ):
         """Creates Encoder-Decoder-RNN model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -471,18 +548,33 @@
 
     def create_encdec_lstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+            "layer0": (
+                100,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer3": (100, "relu", 0.0),  # (neurons, activation, regularization)
         },
     ):
         """Creates Encoder-Decoder-LSTM model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -505,18 +597,18 @@
 
     def create_encdec_gru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+            "layer0": (100, "relu", 0.0, 0.0),
+            "layer1": (50, "relu", 0.0, 0.0),
+            "layer2": (50, "relu", 0.0, 0.0),
+            "layer3": (100, "relu", 0.0),
         },
     ):
         """Creates Encoder-Decoder-GRU model.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
             metrics (str): Performance measurement.
@@ -539,19 +631,19 @@
 
     def create_encdec_cnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (100, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (100, "relu", 0.0),
         },
     ):
         """Creates Encoder-Decoder-CNN model.
         Encoding via CNN and Decoding via GRU.
         Parameters:
             optimizer (str): Optimization algorithm.
             loss (str): Loss function.
@@ -574,59 +666,126 @@
         )
 
     def fit_model(
         self,
         epochs: int,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Trains the model on data provided. Perfroms validation.
         Parameters:
             epochs (int): Number of epochs to train the model.
             show_progress (int): Prints training progress.
             validation_split (float): Determines size of Validation data.
+            board (bool): Creates TensorBoard.
             callback_settings (dict): Create a Keras EarlyStopping object.
         """
         if callback_setting == {}:
-            self.details = self.model.fit(
-                self.input_x,
-                self.input_y,
-                validation_split=validation_split,
-                epochs=epochs,
-                verbose=show_progress,
-            )
+            if board == True:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback_board],
+                )
+            else:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                )
+
         else:
-            callback = EarlyStopping(**callback_setting)
-            self.details = self.model.fit(
-                self.input_x,
-                self.input_y,
-                validation_split=validation_split,
-                epochs=epochs,
-                verbose=show_progress,
-                callbacks=[callback],
-            )
+            if board == True:
+                callback_board = tf.keras.callbacks.TensorBoard(
+                    log_dir="logs/fit/"
+                    + self.model_id
+                    + datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S"),
+                    histogram_freq=1,
+                )
+                callback = EarlyStopping(**callback_setting)
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback, callback_board],
+                )
+            else:
+                callback = EarlyStopping(**callback_setting)
+                self.details = self.model.fit(
+                    self.input_x,
+                    self.input_y,
+                    validation_split=validation_split,
+                    epochs=epochs,
+                    verbose=show_progress,
+                    callbacks=[callback],
+                )
         return self.details
 
     def model_blueprint(self):
         """Prints a summary of the models layer structure."""
         self.model.summary()
 
-    def show_performance(self):
-        """Plots model loss, validation loss over time."""
+    def show_performance(self, metric_name: str = ""):
+        """Plots model loss and a given metric over time."""
         information = self.details
 
-        plt.plot(information.history["loss"], color="black")
-        plt.plot(information.history["val_loss"], color="teal")
-        plt.title(self.model_id + " Model Loss")
-        plt.ylabel(self.loss)
-        plt.xlabel("Epoch")
-        plt.legend(["Train", "Test"], loc="upper right")
-        plt.tight_layout()
-        plt.show()
+        plt.style.use("dark_background")
+
+        colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
+
+        if metric_name == "":
+
+            plt.plot(information.history["loss"], color=colors[0])
+            plt.plot(information.history["val_loss"], color=colors[1])
+            plt.title(self.model_id + " Model Loss")
+            plt.ylabel(self.loss)
+            plt.xlabel("Epoch")
+            plt.legend(["Train", "Test"], loc="upper right")
+            plt.tight_layout()
+            plt.show()
+        else:
+            plt.plot(information.history["loss"], color=colors[0])
+            plt.plot(information.history["val_loss"], color=colors[1])
+            plt.plot(information.history[metric_name], color=colors[2])
+            plt.plot(information.history["val_" + metric_name], color=colors[3])
+            plt.title(self.model_id + " Model Performance")
+            plt.ylabel(metric_name)
+            plt.xlabel("Epoch")
+            plt.legend(
+                [
+                    "Train Loss",
+                    "Test Loss",
+                    "Train " + metric_name,
+                    "Test " + metric_name,
+                ],
+                loc="upper right",
+            )
+            plt.tight_layout()
+            plt.show()
 
     def predict(self, data: array) -> DataFrame:
         """Takes in a sequence of values and outputs a forecast.
         Parameters:
             data (array): Input sequence which needs to be forecasted.
         Returns:
             (DataFrame): Forecast for sequence provided.
@@ -669,354 +828,469 @@
 class OptimizePureUni(PureUni):
     def create_fit_mlp(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (50, "relu"),
-            "layer1": (25, "relu"),
-            "layer2": (25, "relu"),
+            "layer0": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                25,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (25, "relu", 0.0),  # (neurons, activation, regularization)
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Multi-Layer-Perceptron model."""
         self.create_mlp(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_rnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+            "layer0": (
+                40,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (50, "relu", 0.0),  # (neurons, activation, regularization)
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Recurrent Neural Network model."""
         self.create_rnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_lstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+            "layer0": (
+                40,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (50, "relu", 0.0),  # (neurons, activation, regularization)
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a LSTM model."""
         self.create_lstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_cnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
-            "layer2": (2),
-            "layer3": (50, "relu"),
+            "layer0": (
+                64,
+                1,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, kernel_size, activation, regularization, dropout)
+            "layer1": (
+                32,
+                1,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, kernel_size, activation, regularization, dropout)
+            "layer2": (2),  # pooling
+            "layer3": (50, "relu", 0.0),  # (neurons, activation, regularization)
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Convolutional Neural Network model."""
         self.create_cnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_gru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (40, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
+            "layer0": (
+                40,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (50, "relu", 0.0),  # (neurons, activation, regularization)
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a GRU model."""
         self.create_gru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_birnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
+        layer_config: dict = {
+            "layer0": (50, "relu", 0.0, 0.0),
+            "layer1": (50, "relu", 0.0),
+        },  # (neurons, activation, regularization, dropout)
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional RNN model."""
         self.create_birnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bilstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
+        layer_config: dict = {
+            "layer0": (50, "relu", 0.0, 0.0),
+            "layer1": (50, "relu", 0.0),
+        },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional LSTM model."""
         self.create_bilstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_bigru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
-        layer_config: dict = {"layer0": (50, "relu"), "layer1": (50, "relu")},
+        layer_config: dict = {
+            "layer0": (50, "relu", 0.0, 0.0),
+            "layer1": (50, "relu", 0.0),
+        },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Bidirectional GRU model."""
         self.create_bigru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_rnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+            "layer0": (
+                100,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer3": (100, "relu", 0.0),  # (neurons, activation, regularization)
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Encoder-Decoder RNN model."""
         self.create_encdec_rnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_lstm(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+            "layer0": (
+                100,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer1": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer2": (
+                50,
+                "relu",
+                0.0,
+                0.0,
+            ),  # (neurons, activation, regularization, dropout)
+            "layer3": (100, "relu", 0.0),  # (neurons, activation, regularization)
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Encoder-Decoder LSTM model."""
         self.create_encdec_lstm(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_gru(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (100, "relu"),
-            "layer1": (50, "relu"),
-            "layer2": (50, "relu"),
-            "layer3": (100, "relu"),
+            "layer0": (100, "relu", 0.0, 0.0),
+            "layer1": (50, "relu", 0.0, 0.0),
+            "layer2": (50, "relu", 0.0, 0.0),
+            "layer3": (100, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Encoder-Decoder GRU model."""
         self.create_encdec_gru(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
 
     def create_fit_encdec_cnn(
         self,
         optimizer: str = "adam",
         loss: str = "mean_squared_error",
         metrics: str = "mean_squared_error",
         layer_config: dict = {
-            "layer0": (64, 1, "relu"),
-            "layer1": (32, 1, "relu"),
+            "layer0": (64, 1, "relu", 0.0, 0.0),
+            "layer1": (32, 1, "relu", 0.0, 0.0),
             "layer2": (2),
-            "layer3": (50, "relu"),
-            "layer4": (100, "relu"),
+            "layer3": (50, "relu", 0.0, 0.0),
+            "layer4": (100, "relu", 0.0),
         },
         epochs: int = 100,
         show_progress: int = 1,
         validation_split: float = 0.20,
+        board: bool = False,
         **callback_setting: dict,
     ):
         """Creates and trains a Encoder-Decoder CNN model."""
         self.create_encdec_cnn(
             optimizer=optimizer,
             loss=loss,
             metrics=metrics,
             layer_config=layer_config,
         )
         self.fit_model(
             epochs=epochs,
             show_progress=show_progress,
             validation_split=validation_split,
+            board=board,
             **callback_setting,
         )
         return self.details.history[metrics][-1]
```

### Comparing `imbrium-1.1.0/imbrium/utils/optimization.py` & `imbrium-1.2.0/imbrium/utils/optimization.py`

 * *Files identical despite different names*

### Comparing `imbrium-1.1.0/imbrium/utils/transformer.py` & `imbrium-1.2.0/imbrium/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `imbrium-1.1.0/imbrium.egg-info/SOURCES.txt` & `imbrium-1.2.0/imbrium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imbrium-1.1.0/setup.py` & `imbrium-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author="Maximilian Mekiska",
     author_email="maxmekiska@gmail.com",
     url="https://github.com/maxmekiska/Imbrium",
     description="Standard and Hybrid Deep Learning Multivariate-Multi-Step & Univariate-Multi-Step Time Series Forecasting.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="imbrium",
-    version="1.1.0",
+    version="1.2.0",
     packages=find_packages(include=["imbrium", "imbrium.*"]),
     install_requires=[
         "setuptools >= 41.0.0",
         "tensorflow >= 2.11.0, < 2.12.0",
         "matplotlib >= 3.5.0, < 3.7.0",
         "pandas >= 1.3.3, < 1.6.0",
         "scikit-learn >= 1.0, < 1.3.0",
```

