# Comparing `tmp/pygmalion-0.1.2.tar.gz` & `tmp/pygmalion-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmalion-0.1.2.tar", last modified: Fri Mar 31 19:14:13 2023, max compression
+gzip compressed data, was "pygmalion-0.1.3.tar", last modified: Tue Apr 11 19:59:20 2023, max compression
```

## Comparing `pygmalion-0.1.2.tar` & `pygmalion-0.1.3.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.586082 pygmalion-0.1.2/
--rw-rw-rw-   0        0        0     1085 2023-02-19 10:00:21.000000 pygmalion-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     7481 2023-03-31 19:14:13.586082 pygmalion-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6942 2023-03-27 11:47:38.000000 pygmalion-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.539205 pygmalion-0.1.2/pygmalion/
--rw-rw-rw-   0        0        0      179 2023-02-26 08:55:42.000000 pygmalion-0.1.2/pygmalion/__init__.py
--rw-rw-rw-   0        0        0       53 2023-03-31 19:10:58.000000 pygmalion-0.1.2/pygmalion/_info.py
--rw-rw-rw-   0        0        0     2923 2023-03-31 18:32:27.000000 pygmalion-0.1.2/pygmalion/_model_base.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.554831 pygmalion-0.1.2/pygmalion/datasets/
--rw-rw-rw-   0        0        0      336 2023-03-31 17:34:26.000000 pygmalion-0.1.2/pygmalion/datasets/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-31 18:29:54.000000 pygmalion-0.1.2/pygmalion/datasets/_airline_tweets.py
--rw-rw-rw-   0        0        0      334 2023-03-31 18:29:58.000000 pygmalion-0.1.2/pygmalion/datasets/_boston_housing.py
--rw-rw-rw-   0        0        0      323 2023-03-31 18:30:04.000000 pygmalion-0.1.2/pygmalion/datasets/_cityscapes.py
--rw-rw-rw-   0        0        0     2733 2023-03-31 18:30:07.000000 pygmalion-0.1.2/pygmalion/datasets/_download.py
--rw-rw-rw-   0        0        0      322 2023-03-31 18:30:14.000000 pygmalion-0.1.2/pygmalion/datasets/_fashion_mnist.py
--rw-rw-rw-   0        0        0      304 2023-03-31 18:30:16.000000 pygmalion-0.1.2/pygmalion/datasets/_iris.py
--rw-rw-rw-   0        0        0      366 2023-03-31 18:30:19.000000 pygmalion-0.1.2/pygmalion/datasets/_sentence_pairs.py
--rw-rw-rw-   0        0        0      313 2023-03-31 18:30:22.000000 pygmalion-0.1.2/pygmalion/datasets/_titanic.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.554831 pygmalion-0.1.2/pygmalion/datasets/generators/
--rw-rw-rw-   0        0        0      111 2023-03-11 18:35:23.000000 pygmalion-0.1.2/pygmalion/datasets/generators/__init__.py
--rw-rw-rw-   0        0        0     3698 2023-02-26 08:07:23.000000 pygmalion-0.1.2/pygmalion/datasets/generators/_circles_generator.py
--rw-rw-rw-   0        0        0     2335 2023-03-18 11:53:06.000000 pygmalion-0.1.2/pygmalion/datasets/generators/_roman_numerals_generator.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.554831 pygmalion-0.1.2/pygmalion/neural_networks/
--rw-rw-rw-   0        0        0      376 2023-03-28 12:20:13.000000 pygmalion-0.1.2/pygmalion/neural_networks/__init__.py
--rw-rw-rw-   0        0        0    17360 2023-03-27 11:08:39.000000 pygmalion-0.1.2/pygmalion/neural_networks/_conversions.py
--rw-rw-rw-   0        0        0     3132 2023-03-24 13:39:04.000000 pygmalion-0.1.2/pygmalion/neural_networks/_dense_classifier.py
--rw-rw-rw-   0        0        0     4037 2023-03-24 13:37:40.000000 pygmalion-0.1.2/pygmalion/neural_networks/_dense_regressor.py
--rw-rw-rw-   0        0        0     2863 2023-03-24 13:39:04.000000 pygmalion-0.1.2/pygmalion/neural_networks/_image_classifier.py
--rw-rw-rw-   0        0        0     4251 2023-03-24 13:39:04.000000 pygmalion-0.1.2/pygmalion/neural_networks/_image_segmenter.py
--rw-rw-rw-   0        0        0     7936 2023-03-27 11:46:39.000000 pygmalion-0.1.2/pygmalion/neural_networks/_loss_functions.py
--rw-rw-rw-   0        0        0    10905 2023-03-31 17:35:17.000000 pygmalion-0.1.2/pygmalion/neural_networks/_neural_network.py
--rw-rw-rw-   0        0        0     8281 2023-02-19 10:00:21.000000 pygmalion-0.1.2/pygmalion/neural_networks/_object_detector.py
--rw-rw-rw-   0        0        0     6422 2023-03-28 16:59:24.000000 pygmalion-0.1.2/pygmalion/neural_networks/_text_classifier.py
--rw-rw-rw-   0        0        0     6565 2023-03-28 17:00:06.000000 pygmalion-0.1.2/pygmalion/neural_networks/_text_segmenter.py
--rw-rw-rw-   0        0        0    18158 2023-03-27 11:43:01.000000 pygmalion-0.1.2/pygmalion/neural_networks/_text_translator.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.570457 pygmalion-0.1.2/pygmalion/neural_networks/layers/
--rw-rw-rw-   0        0        0      602 2023-03-11 11:30:46.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/__init__.py
--rw-rw-rw-   0        0        0     1570 2023-03-10 14:00:14.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/_activation.py
--rw-rw-rw-   0        0        0     2328 2023-03-05 11:05:58.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/_conv_block.py
--rw-rw-rw-   0        0        0     3451 2023-03-05 10:47:16.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/_normalizer.py
--rw-rw-rw-   0        0        0     3167 2023-02-24 14:25:21.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/_padded_conv.py
--rw-rw-rw-   0        0        0     2375 2023-03-14 15:30:15.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/_positional_encoding.py
--rw-rw-rw-   0        0        0     1791 2023-02-24 15:48:47.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/_upsampling.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.570457 pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/
--rw-rw-rw-   0        0        0      108 2023-03-12 12:44:54.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/__init__.py
--rw-rw-rw-   0        0        0    11373 2023-03-18 18:53:35.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_attention.py
--rw-rw-rw-   0        0        0     4689 2023-03-18 18:52:48.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_multihead_attention.py
--rw-rw-rw-   0        0        0     4887 2023-03-14 08:58:05.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_stack.py
--rw-rw-rw-   0        0        0     6934 2023-03-14 13:01:02.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_stages.py
--rw-rw-rw-   0        0        0     1333 2023-03-13 14:05:17.000000 pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.586082 pygmalion-0.1.2/pygmalion/tokenizers/
--rw-rw-rw-   0        0        0      188 2023-03-11 22:05:58.000000 pygmalion-0.1.2/pygmalion/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     1452 2023-03-27 11:23:04.000000 pygmalion-0.1.2/pygmalion/tokenizers/_ascii_char_tokenizer.py
--rw-rw-rw-   0        0        0     9824 2023-03-10 17:17:04.000000 pygmalion-0.1.2/pygmalion/tokenizers/_byte_pair_encoder.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.586082 pygmalion-0.1.2/pygmalion/tokenizers/_utilities/
--rw-rw-rw-   0        0        0      181 2023-03-10 17:16:48.000000 pygmalion-0.1.2/pygmalion/tokenizers/_utilities/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-03-03 15:19:46.000000 pygmalion-0.1.2/pygmalion/tokenizers/_utilities/_bytes_tree.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 17:57:11.000000 pygmalion-0.1.2/pygmalion/tokenizers/_utilities/_functions.py
--rw-rw-rw-   0        0        0      483 2023-02-26 09:01:48.000000 pygmalion-0.1.2/pygmalion/tokenizers/_utilities/_special_token.py
--rw-rw-rw-   0        0        0     3722 2023-03-19 01:46:23.000000 pygmalion-0.1.2/pygmalion/tokenizers/_utilities/_tokenizer_base.py
--rw-rw-rw-   0        0        0     3004 2023-03-10 17:17:36.000000 pygmalion-0.1.2/pygmalion/tokenizers/_words_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.586082 pygmalion-0.1.2/pygmalion/unsupervised/
--rw-rw-rw-   0        0        0       22 2023-02-26 08:42:10.000000 pygmalion-0.1.2/pygmalion/unsupervised/__init__.py
--rw-rw-rw-   0        0        0     3465 2023-02-26 11:23:20.000000 pygmalion-0.1.2/pygmalion/unsupervised/pca.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.586082 pygmalion-0.1.2/pygmalion/utilities/
--rw-rw-rw-   0        0        0      240 2023-02-26 08:56:05.000000 pygmalion-0.1.2/pygmalion/utilities/__init__.py
--rw-rw-rw-   0        0        0     2677 2023-02-19 10:02:35.000000 pygmalion-0.1.2/pygmalion/utilities/_cross_validation.py
--rw-rw-rw-   0        0        0     3775 2023-02-19 10:00:21.000000 pygmalion-0.1.2/pygmalion/utilities/_decorators.py
--rw-rw-rw-   0        0        0     6453 2023-02-19 10:02:35.000000 pygmalion-0.1.2/pygmalion/utilities/_metrics.py
--rw-rw-rw-   0        0        0     6533 2023-03-27 11:19:38.000000 pygmalion-0.1.2/pygmalion/utilities/_ploting.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.539205 pygmalion-0.1.2/pygmalion.egg-info/
--rw-rw-rw-   0        0        0     7481 2023-03-31 19:14:13.000000 pygmalion-0.1.2/pygmalion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2658 2023-03-31 19:14:13.000000 pygmalion-0.1.2/pygmalion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 19:14:13.000000 pygmalion-0.1.2/pygmalion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-03-31 19:14:13.000000 pygmalion-0.1.2/pygmalion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-31 19:14:13.000000 pygmalion-0.1.2/pygmalion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 19:14:13.586082 pygmalion-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1262 2023-03-31 19:08:49.000000 pygmalion-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 19:14:13.586082 pygmalion-0.1.2/test/
--rw-rw-rw-   0        0        0      596 2023-03-14 13:51:25.000000 pygmalion-0.1.2/test/test_decoder_stage.py
--rw-rw-rw-   0        0        0     5062 2023-03-12 12:47:08.000000 pygmalion-0.1.2/test/test_kernelized_attention.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.602047 pygmalion-0.1.3/
+-rw-rw-rw-   0        0        0     1085 2023-02-19 10:00:21.000000 pygmalion-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     7481 2023-04-11 19:59:20.601045 pygmalion-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6942 2023-03-27 11:47:38.000000 pygmalion-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.409871 pygmalion-0.1.3/pygmalion/
+-rw-rw-rw-   0        0        0      179 2023-02-26 08:55:42.000000 pygmalion-0.1.3/pygmalion/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-04-01 08:40:05.000000 pygmalion-0.1.3/pygmalion/_info.py
+-rw-rw-rw-   0        0        0     1858 2023-04-08 20:30:29.000000 pygmalion-0.1.3/pygmalion/_model.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.451909 pygmalion-0.1.3/pygmalion/datasets/
+-rw-rw-rw-   0        0        0      330 2023-04-08 21:42:29.000000 pygmalion-0.1.3/pygmalion/datasets/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-08 21:42:37.000000 pygmalion-0.1.3/pygmalion/datasets/_airline_tweets.py
+-rw-rw-rw-   0        0        0      334 2023-04-08 21:42:48.000000 pygmalion-0.1.3/pygmalion/datasets/_aquarium.py
+-rw-rw-rw-   0        0        0      353 2023-04-08 21:42:46.000000 pygmalion-0.1.3/pygmalion/datasets/_boston_housing.py
+-rw-rw-rw-   0        0        0      342 2023-04-08 21:42:51.000000 pygmalion-0.1.3/pygmalion/datasets/_cityscapes.py
+-rw-rw-rw-   0        0        0      341 2023-04-08 21:43:00.000000 pygmalion-0.1.3/pygmalion/datasets/_fashion_mnist.py
+-rw-rw-rw-   0        0        0      323 2023-04-08 21:43:03.000000 pygmalion-0.1.3/pygmalion/datasets/_iris.py
+-rw-rw-rw-   0        0        0      385 2023-04-08 21:43:06.000000 pygmalion-0.1.3/pygmalion/datasets/_sentence_pairs.py
+-rw-rw-rw-   0        0        0      332 2023-04-08 21:43:09.000000 pygmalion-0.1.3/pygmalion/datasets/_titanic.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.466923 pygmalion-0.1.3/pygmalion/datasets/generators/
+-rw-rw-rw-   0        0        0      159 2023-04-08 20:29:21.000000 pygmalion-0.1.3/pygmalion/datasets/generators/__init__.py
+-rw-rw-rw-   0        0        0     3698 2023-02-26 08:07:23.000000 pygmalion-0.1.3/pygmalion/datasets/generators/_circles_generator.py
+-rw-rw-rw-   0        0        0     2335 2023-03-18 11:53:06.000000 pygmalion-0.1.3/pygmalion/datasets/generators/_roman_numerals_generator.py
+-rw-rw-rw-   0        0        0     4063 2023-04-11 18:11:29.000000 pygmalion-0.1.3/pygmalion/datasets/generators/_shapes_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.500954 pygmalion-0.1.3/pygmalion/neural_networks/
+-rw-rw-rw-   0        0        0      383 2023-04-09 11:47:43.000000 pygmalion-0.1.3/pygmalion/neural_networks/__init__.py
+-rw-rw-rw-   0        0        0     9292 2023-04-09 13:28:07.000000 pygmalion-0.1.3/pygmalion/neural_networks/_conversions.py
+-rw-rw-rw-   0        0        0     3132 2023-03-24 13:39:04.000000 pygmalion-0.1.3/pygmalion/neural_networks/_dense_classifier.py
+-rw-rw-rw-   0        0        0     4037 2023-03-24 13:37:40.000000 pygmalion-0.1.3/pygmalion/neural_networks/_dense_regressor.py
+-rw-rw-rw-   0        0        0     2863 2023-03-24 13:39:04.000000 pygmalion-0.1.3/pygmalion/neural_networks/_image_classifier.py
+-rw-rw-rw-   0        0        0    15902 2023-04-11 18:30:31.000000 pygmalion-0.1.3/pygmalion/neural_networks/_image_object_detector.py
+-rw-rw-rw-   0        0        0     4251 2023-03-24 13:39:04.000000 pygmalion-0.1.3/pygmalion/neural_networks/_image_segmenter.py
+-rw-rw-rw-   0        0        0     4598 2023-04-10 17:40:55.000000 pygmalion-0.1.3/pygmalion/neural_networks/_loss_functions.py
+-rw-rw-rw-   0        0        0    10521 2023-04-08 21:56:10.000000 pygmalion-0.1.3/pygmalion/neural_networks/_neural_network.py
+-rw-rw-rw-   0        0        0     6422 2023-03-28 16:59:24.000000 pygmalion-0.1.3/pygmalion/neural_networks/_text_classifier.py
+-rw-rw-rw-   0        0        0     6565 2023-03-28 17:00:06.000000 pygmalion-0.1.3/pygmalion/neural_networks/_text_segmenter.py
+-rw-rw-rw-   0        0        0    18376 2023-04-09 09:44:05.000000 pygmalion-0.1.3/pygmalion/neural_networks/_text_translator.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.527978 pygmalion-0.1.3/pygmalion/neural_networks/layers/
+-rw-rw-rw-   0        0        0      602 2023-03-11 11:30:46.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     1218 2023-04-08 21:26:11.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/_activation.py
+-rw-rw-rw-   0        0        0     2328 2023-04-06 12:15:33.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/_conv_block.py
+-rw-rw-rw-   0        0        0     3451 2023-03-05 10:47:16.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/_normalizer.py
+-rw-rw-rw-   0        0        0     3167 2023-02-24 14:25:21.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/_padded_conv.py
+-rw-rw-rw-   0        0        0     2375 2023-03-14 15:30:15.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/_positional_encoding.py
+-rw-rw-rw-   0        0        0     1791 2023-02-24 15:48:47.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/_upsampling.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.547996 pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/
+-rw-rw-rw-   0        0        0      108 2023-03-12 12:44:54.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/__init__.py
+-rw-rw-rw-   0        0        0    11373 2023-03-18 18:53:35.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_attention.py
+-rw-rw-rw-   0        0        0     4689 2023-03-18 18:52:48.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_multihead_attention.py
+-rw-rw-rw-   0        0        0     4887 2023-03-14 08:58:05.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_stack.py
+-rw-rw-rw-   0        0        0     6934 2023-03-14 13:01:02.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_stages.py
+-rw-rw-rw-   0        0        0     1333 2023-03-13 14:05:17.000000 pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.560007 pygmalion-0.1.3/pygmalion/tokenizers/
+-rw-rw-rw-   0        0        0      188 2023-03-11 22:05:58.000000 pygmalion-0.1.3/pygmalion/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     1452 2023-03-27 11:23:04.000000 pygmalion-0.1.3/pygmalion/tokenizers/_ascii_char_tokenizer.py
+-rw-rw-rw-   0        0        0     9881 2023-04-08 22:43:59.000000 pygmalion-0.1.3/pygmalion/tokenizers/_byte_pair_encoder.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.575021 pygmalion-0.1.3/pygmalion/tokenizers/_utilities/
+-rw-rw-rw-   0        0        0      176 2023-04-08 21:17:04.000000 pygmalion-0.1.3/pygmalion/tokenizers/_utilities/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-03-03 15:19:46.000000 pygmalion-0.1.3/pygmalion/tokenizers/_utilities/_bytes_tree.py
+-rw-rw-rw-   0        0        0     1334 2023-02-26 17:57:11.000000 pygmalion-0.1.3/pygmalion/tokenizers/_utilities/_functions.py
+-rw-rw-rw-   0        0        0      483 2023-02-26 09:01:48.000000 pygmalion-0.1.3/pygmalion/tokenizers/_utilities/_special_token.py
+-rw-rw-rw-   0        0        0     3709 2023-04-08 21:17:06.000000 pygmalion-0.1.3/pygmalion/tokenizers/_utilities/_tokenizer.py
+-rw-rw-rw-   0        0        0     3004 2023-03-10 17:17:36.000000 pygmalion-0.1.3/pygmalion/tokenizers/_words_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.580026 pygmalion-0.1.3/pygmalion/unsupervised/
+-rw-rw-rw-   0        0        0       22 2023-02-26 08:42:10.000000 pygmalion-0.1.3/pygmalion/unsupervised/__init__.py
+-rw-rw-rw-   0        0        0     3469 2023-04-08 20:31:17.000000 pygmalion-0.1.3/pygmalion/unsupervised/pca.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.593038 pygmalion-0.1.3/pygmalion/utilities/
+-rw-rw-rw-   0        0        0      277 2023-04-08 21:44:23.000000 pygmalion-0.1.3/pygmalion/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2677 2023-02-19 10:02:35.000000 pygmalion-0.1.3/pygmalion/utilities/_cross_validation.py
+-rw-rw-rw-   0        0        0     3775 2023-02-19 10:00:21.000000 pygmalion-0.1.3/pygmalion/utilities/_decorators.py
+-rw-rw-rw-   0        0        0     2215 2023-04-09 11:51:21.000000 pygmalion-0.1.3/pygmalion/utilities/_download.py
+-rw-rw-rw-   0        0        0     1754 2023-04-08 22:35:58.000000 pygmalion-0.1.3/pygmalion/utilities/_load_model.py
+-rw-rw-rw-   0        0        0     6453 2023-02-19 10:02:35.000000 pygmalion-0.1.3/pygmalion/utilities/_metrics.py
+-rw-rw-rw-   0        0        0     6916 2023-04-10 18:08:54.000000 pygmalion-0.1.3/pygmalion/utilities/_ploting.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.423884 pygmalion-0.1.3/pygmalion.egg-info/
+-rw-rw-rw-   0        0        0     7481 2023-04-11 19:59:19.000000 pygmalion-0.1.3/pygmalion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2773 2023-04-11 19:59:20.000000 pygmalion-0.1.3/pygmalion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:59:19.000000 pygmalion-0.1.3/pygmalion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-04-11 19:59:20.000000 pygmalion-0.1.3/pygmalion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-11 19:59:20.000000 pygmalion-0.1.3/pygmalion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 19:59:20.602047 pygmalion-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1262 2023-03-31 19:08:49.000000 pygmalion-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:59:20.600044 pygmalion-0.1.3/test/
+-rw-rw-rw-   0        0        0      596 2023-03-14 13:51:25.000000 pygmalion-0.1.3/test/test_decoder_stage.py
+-rw-rw-rw-   0        0        0     5062 2023-03-12 12:47:08.000000 pygmalion-0.1.3/test/test_kernelized_attention.py
```

### Comparing `pygmalion-0.1.2/LICENSE` & `pygmalion-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/PKG-INFO` & `pygmalion-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmalion
-Version: 0.1.2
+Version: 0.1.3
 Summary: A machine learning package
 Home-page: https://github.com/BFavier/Pygmalion
 Author: Benoit Favier
 Author-email: benoitfamillefavier@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmalion-0.1.2/README.md` & `pygmalion-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/_model_base.py` & `pygmalion-0.1.3/pygmalion/_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,18 @@
 import json
 import pathlib
 import io
 from typing import Union
 
 
-class ModelBase:
+class Model:
 
     def __repr__(self):
         return f"{type(self).__name__}()"
 
-    @classmethod
-    def load(cls, file_path: Union[str, pathlib.Path, io.IOBase]) -> "ModelBase":
-        """
-        Load a model from the disk (must be a .json)
-
-        Parameters
-        ----------
-        file : str or pathlib.Path or file like
-            path of the file to read
-        """
-        if not isinstance(file_path, io.IOBase):
-            file_path = pathlib.Path(file_path)
-            path = file_path.parent
-            suffix = file_path.suffix.lower()
-            if suffix != ".json":
-                raise ValueError(f"The file must be '.json' file, but got a '{suffix}'")
-            if not path.is_dir():
-                raise ValueError(f"The directory '{path}' does not exist")
-            if not file_path.is_file():
-                raise FileNotFoundError(f"The file '{file_path.name}' does not exist in '{path}'")
-            with open(file_path) as json_file:
-                dump = json.load(json_file)
-        else:
-            dump = json.load(file_path)
-        return cls.from_dump(dump)
-
     def save(self, file_path: Union[str, pathlib.Path, io.IOBase],
              overwrite: bool = False, create_dir: bool = False):
         """
         Saves the model to the disk as '.json' file
 
         Parameters
         ----------
@@ -66,13 +40,13 @@
                     f"The file '{file_path}' already exists, set 'overwrite=True' to overwrite.")
             with open(file_path, "w", encoding="utf-8") as json_file:
                 json.dump(self.dump, json_file, ensure_ascii=False)
         else:
             json.dump(self.dump, file_path, ensure_ascii=False)
 
     @classmethod
-    def from_dump(cls, dump: dict) -> "ModelBase":
+    def from_dump(cls, dump: dict) -> "Model":
         raise NotImplementedError()
     
     @property
     def dump(self) -> dict:
         raise NotImplementedError()
```

### Comparing `pygmalion-0.1.2/pygmalion/datasets/_download.py` & `pygmalion-0.1.3/pygmalion/utilities/_download.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import pathlib
 from io import IOBase, BytesIO
+from tqdm import tqdm
 
 
 def download(file_path: str, url: str):
     """
     Download google drive a file from the given url to the disk.
     If the directory does not exists raise an error.
     If the file already exists skip it.
@@ -40,38 +41,24 @@
     return stream
 
 
 def _download_to_stream(url: str, stream: IOBase, file_name: str="Download"):
     """
     Download the bytes of the give google drive file into the given IO stream
     """
-    # make the request
     session = requests.Session()
     response = session.get(_direct_url(url), stream=True)
     if response.status_code >= 400:
         raise RuntimeError(f"http error: {response.status_code}")
-    # get a confirmation token for large files
-    for key, value in response.cookies.items():
-        if key.startswith('download_warning'):
-            response = session.get(_direct_url(url), params={'confirm': value},
-                                   stream=True)
-            break
-    # save on disk
-    CHUNK_SIZE = 32768
-    print(f"{file_name}: 0. kB", end="", flush=True)
-    for i, chunk in enumerate(response.iter_content(CHUNK_SIZE)):
-        stream.write(chunk)
-        n_bytes = (i+1)*CHUNK_SIZE / 8.
-        for j, unit in enumerate(['Bytes', 'kB', 'MB', 'GB', 'TB']):
-            if n_bytes < 1024**(j+1):
-                break
-        progress = n_bytes / 10024**j
-        print(f"\r{file_name}: {progress:.1f} {unit}"+" "*10,
-                end="", flush=True)
-    print()
+    total_size = int(response.headers['content-length'])
+    CHUNK_SIZE = 4096
+    with tqdm(unit="B", total=total_size, unit_scale=True, unit_divisor=1000) as pbar:
+        for chunk in response.iter_content(CHUNK_SIZE):
+            stream.write(chunk)
+            pbar.update(len(chunk))
 
 
 def _direct_url(url: str) -> str:
     """
     Converts a googledrive 'share' url to a direct download url
 
     Parameters
```

### Comparing `pygmalion-0.1.2/pygmalion/datasets/generators/_circles_generator.py` & `pygmalion-0.1.3/pygmalion/datasets/generators/_circles_generator.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/datasets/generators/_roman_numerals_generator.py` & `pygmalion-0.1.3/pygmalion/datasets/generators/_roman_numerals_generator.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_dense_classifier.py` & `pygmalion-0.1.3/pygmalion/neural_networks/_dense_classifier.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_dense_regressor.py` & `pygmalion-0.1.3/pygmalion/neural_networks/_dense_regressor.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_image_classifier.py` & `pygmalion-0.1.3/pygmalion/neural_networks/_image_classifier.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_image_segmenter.py` & `pygmalion-0.1.3/pygmalion/neural_networks/_image_segmenter.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_loss_functions.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_stages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,199 +1,170 @@
 import torch
-import torch.nn.functional as F
-from typing import Union, Tuple
-
-
-def MSE(y_pred: torch.Tensor, y_target: torch.Tensor,
-        weights: Union[None, torch.Tensor] = None) -> torch.Tensor:
-    """
-    Returns the Root Mean Squared Error of the model.
-    Each observation can optionnaly be weighted
-
-    Parameters
-    ----------
-    y_pred : torch.Tensor
-        A Tensor of float of shape [N_observations]
-        The values predicted by the model for eahc observations
-    y_target : torch.Tensor
-        A Tensor of float of shape [N_observations]
-        The target values to be predicted by the model
-    weights : None or torch.Tensor
-        If None all observations are equally weighted
-        Otherwise the squared error of each observation
-        is multiplied by the given factor
-
-    Returns
-    -------
-    torch.Tensor :
-        the scalar value of the loss
-    """
-    y_target = y_target.to(y_pred.device)
-    if weights is None:
-        return F.mse_loss(y_pred, y_target)
-    else:
-        weights = weights.to(y_pred.device)
-        return torch.mean(weights * (y_pred - y_target)**2)
-
-
-def RMSE(*args, **kwargs):
-    """
-    Returns the Root Mean Squared Error of the model.
-
-    Parameters
-    ----------
-    *args, **kwargs :
-        similar to MSE
-
-    Returns
-    -------
-    torch.Tensor :
-        the scalar value of the loss
-    """
-    return torch.sqrt(MSE(*args, **kwargs))
-
-
-def cross_entropy(y_pred: torch.Tensor, y_target: torch.Tensor,
-                  weights: Union[None, torch.Tensor] = None,
-                  class_weights: Union[None, torch.Tensor] = None,
-                  label_smoothing: float = 0.
-                  ) -> torch.Tensor:
-    """
-    Returns the cross entropy error of the model.
-    Each observation and each class be optionnaly weighted
-
-    Parameters
-    ----------
-    y_pred : torch.Tensor
-        A Tensor of float of shape [N_observations, N_classes, ...]
-        The probability of each class for eahc observation
-    y_target : torch.Tensor
-        A Tensor of long of shape [N_observations, 1, ...]
-        The index of the class to be predicted
-    weights : None or torch.Tensor
-        The individual observation weights (ignored if None)
-    class_weights : None or torch.Tensor
-        If None, all classes are equally weighted
-        The class-wise weights (ignored if None)
-
-    Returns
-    -------
-    torch.Tensor :
-        the scalar value of the loss
-    """
-    y_target = y_target.to(y_pred.device)
-    if class_weights is not None:
-        class_weights = class_weights.to(y_pred.device)
-    if weights is None:
-        return F.cross_entropy(y_pred, y_target, weight=class_weights, label_smoothing=label_smoothing)
-    else:
-        weights = weights.to(y_pred.device)
-        return (F.cross_entropy(y_pred, y_target, weight=class_weights, label_smoothing=label_smoothing, reduction="none")
-                * weights) / weights.mean()
-
-
-def soft_dice_loss(y_pred: torch.Tensor, y_target: torch.Tensor,
-                   weights: Union[None, torch.Tensor] = None,
-                   class_weights: Union[None, torch.Tensor] = None
-                   ) -> torch.Tensor:
-    """
-    A soft Dice loss for segmentation
-
-    Parameters
-    ----------
-    y_pred : torch.Tensor
-        A Tensor of float of shape [N_observations, N_classes, ...]
-        The probability of each class for eahc observation
-    y_target : torch.Tensor
-        A Tensor of long of shape [N_observations, 1, ...]
-        The index of the class to be predicted
-    weights : None or torch.Tensor
-        The individual observation weights (ignored if None)
-    class_weights : None or torch.Tensor
-        If None, all classes are equally weighted
-        The class-wise weights (ignored if None)
-
-    Returns
-    -------
-    torch.Tensor :
-        the scalar value of the loss
-    """
-    if (weights is not None) or (class_weights is not None):
-        raise NotImplementedError("Weighting in soft_dice_loss is not implemented yet")
-    y_target = y_target.to(y_pred.device)
-    n_classes = y_pred.shape[1]
-    pred = F.softmax(y_pred, dim=1)
-    eps = 1.0E-5
-    target = F.one_hot(y_target, num_classes=n_classes).permute(0, 3, 1, 2)
-    intersect = torch.sum(pred * target, dim=[2, 3])
-    cardinality = torch.sum(pred + target, dim=[2, 3])
-    dice_coeff = (2.*intersect + eps) / (cardinality + eps)
-    loss = 1. - torch.mean(dice_coeff)
-    return loss
-
-
-def object_detector_loss(y_pred: torch.Tensor, y_target: Tuple[torch.Tensor],
-                         weights: Union[None, torch.Tensor] = None,
-                         class_weights: Union[None, torch.Tensor] = None,
-                         target_norm: Union[None, torch.nn.Module] = None
-                         ) -> torch.Tensor:
-    """
-    Parameters
-    ----------
-    y_pred : tuple of torch.Tensor
-        The predictions of the model
-        A tuple of (boxe_size, object_proba, class_proba) Where
-        * 'boxe_size' is a tensor of [x, y, width, height] of the bboxe
-        * 'object_proba' is the probability object presence in the bboxe
-        * 'class_proba' is the probability of the object beeing of each class
-        Each tensor has the shape (N, B, C, H, W) with
-        * N number of observations
-        * B number of bounding boxes predicted per grid cell
-        * C number of channels (specific for each tensor)
-        * H the height of the cell grid
-        * W the width of the cell grid
-    y_target : torch.Tensor
-        The target bounding boxes to predict
-        Similar to y_pred except that each tensor is of shape (N, C, H, W)
-
-    Returns
-    -------
-    torch.Tensor :
-        a scalar tensor representing the loss function
-    """
-    coords_pred, size_pred, object_pred, class_pred = y_pred
-    coords_target, size_target, object_mask, class_target = y_target
-    _, n, _, _ = class_pred.shape
-    # Calculating the loss part linked to bounding boxe position/size
-    index = object_mask.unsqueeze(0).expand(2, -1, -1, -1)
-    coords_pred = torch.transpose(coords_pred, 0, 1)[index].view(2, -1)
-    coords_target = torch.transpose(coords_target, 0, 1)[index].view(2, -1)
-    coords_loss = (coords_pred - coords_target)**2
-    size_pred = torch.transpose(size_pred, 0, 1)[index].view(2, -1)
-    size_target = torch.transpose(size_target, 0, 1)[index].view(2, -1)
-    if target_norm is not None:
-        size_target = target_norm(size_target.unsqueeze(0)).squeeze(0)
-    size_loss = (size_pred - size_target)**2
-    if weights is not None:
-        coords_loss = coords_loss * weights[object_mask]
-        size_loss = size_loss * weights[object_mask]
-    coords_loss = coords_loss.mean()
-    size_loss = size_loss.mean()
-    # Calculate the loss part linked to object presence
-    object_loss = -torch.log(object_pred[object_mask] + 1.0E-5)
-    non_object_loss = -torch.log(1 - object_pred[~object_mask] + 1.0E-5)
-    if weights is not None:
-        object_loss = object_loss * weights[object_mask]
-        non_object_loss = non_object_loss * weights[~object_mask]
-    object_loss = object_loss.mean()
-    non_object_loss = non_object_loss.mean()
-    # Calculate the loss part linked to detected class
-    index = object_mask.unsqueeze(3).expand(-1, -1, -1, n)
-    class_pred = class_pred.permute(0, 2, 3, 1)[index].view(-1, n)
-    class_target = class_target[object_mask].view(-1)
-    class_loss = F.nll_loss(F.log_softmax(class_pred, dim=1), class_target,
-                            weight=class_weights, reduction="none")
-    if weights is not None:
-        class_loss = class_loss * weights[object_mask]
-    class_loss = class_loss.mean()
-    # Returning the final loss
-    return coords_loss + size_loss + object_loss + non_object_loss + class_loss
+from typing import Optional
+from ._multihead_attention import MultiHeadAttention, ATTENTION_TYPE
+from torch.utils.checkpoint import checkpoint
+
+
+class TransformerEncoderStage(torch.nn.Module):
+
+    def __init__(self, projection_dim: int, n_heads: int,
+                 dropout: Optional[float] = None,
+                 activation: str = "relu", RPE_radius: Optional[int] = None,
+                 attention_type: ATTENTION_TYPE = "scaled dot product",
+                 **kwargs):
+        super().__init__()
+        dim = projection_dim * n_heads
+        self.activation = getattr(torch, activation)
+        self.self_attention = MultiHeadAttention(projection_dim, n_heads, False,
+                                                 RPE_radius=RPE_radius,
+                                                 attention_type=attention_type,
+                                                 **kwargs)
+        self.intermediate_norm = torch.nn.LayerNorm(dim)
+        self.intermediate_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.expand = torch.nn.Linear(dim, dim * 4)
+        self.contract = torch.nn.Linear(dim * 4, dim)
+        self.out_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.out_norm = torch.nn.LayerNorm(dim)
+
+    def forward(self, X: torch.Tensor,
+                padding_mask: Optional[torch.Tensor] = None):
+        """
+        Parameter
+        ---------
+        X : torch.Tensor
+            Tensor of shape (N, L, D) with
+            * N sentences count
+            * L sequence length
+            * D number of features
+
+        padding_mask : torch.tensor or None
+            tensor of booleans of shape (N, L) of tokens to ignore
+
+        Returns
+        -------
+        torch.Tensor
+            tensor of shape (N, L, D)
+        """
+        X = X.to(self.device)
+        N, L, _ = X.shape
+        input = X.reshape(N * L, -1)
+        X = self.self_attention(X, X, padding_mask, padding_mask).reshape(N * L, -1)
+        if self.intermediate_dropout is not None:
+            X = self.intermediate_dropout(X) + input
+        X = self.intermediate_norm(X)
+        input = X
+        X = self.contract(self.activation(self.expand(X)))
+        if self.out_dropout is not None:
+            X = self.out_dropout(X)
+        X = self.out_norm(X + input)
+        return X.reshape(N, L, -1)
+
+    @property
+    def device(self) -> torch.device:
+        return self.self_attention.key.weight.device
+
+
+class TransformerDecoderStage(torch.nn.Module):
+
+    def __init__(self, projection_dim: int, n_heads: int,
+                 dropout: Optional[float] = None, activation: str = "relu",
+                 RPE_radius: Optional[int] = None,
+                 attention_type: ATTENTION_TYPE = "scaled dot product",
+                 **kwargs):
+        super().__init__()
+        dim = projection_dim * n_heads
+        self.activation = getattr(torch, activation)
+        self.masked_self_attention = MultiHeadAttention(projection_dim, n_heads, True,
+                                                        RPE_radius=RPE_radius,
+                                                        attention_type=attention_type,
+                                                        **kwargs)
+        self.first_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.first_norm = torch.nn.LayerNorm(dim)
+        self.attention = MultiHeadAttention(projection_dim, n_heads, False,
+                                            RPE_radius=RPE_radius,
+                                            attention_type=attention_type)
+        self.second_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.second_norm = torch.nn.LayerNorm(dim)
+        self.expand = torch.nn.Linear(dim, 4 * dim)
+        self.contract = torch.nn.Linear(4 * dim, dim)
+        self.out_dropout = torch.nn.Dropout(dropout) if dropout is not None else None
+        self.out_norm = torch.nn.LayerNorm(dim)
+
+    def forward(self, Y, encoded,
+                encoded_padding_mask: Optional[torch.Tensor] = None):
+        """
+        Parameter
+        ---------
+        Y : torch.Tensor
+            Tensor of shape (N, Lq, D)
+        encoded : torch.Tensor
+            Tensor of shape (N, Lk, D)
+        encoded_padding_mask : torch.Tensor or None
+            mask of shape (N, Lk)
+
+        Returns
+        -------
+        torch.Tensor
+            tensor of shape (N, L, D)
+        """
+        encoded = encoded.to(self.device)
+        Y = Y.to(self.device)
+        N, L, _ = Y.shape
+        input = Y.reshape(N * L, -1)
+        Y = self.masked_self_attention(Y, Y).reshape(N * L, -1)
+        if self.first_dropout is not None:
+            Y = self.first_dropout(Y)
+        Y = self.first_norm(Y + input).reshape(N, L, -1)
+        input = Y.reshape(N * L, -1)
+        Y = self.attention(Y, encoded, query_padding_mask=None,
+                           key_padding_mask=encoded_padding_mask).reshape(N * L, -1)
+        if self.second_dropout is not None:
+            Y = self.second_dropout(Y)
+        Y = self.second_norm(Y + input)
+        input = Y
+        Y = self.contract(self.activation(self.expand(Y)))
+        if self.out_dropout is not None:
+            Y = self.out_dropout(Y)
+        Y = self.out_norm(Y + input)
+        return Y.reshape(N, L, -1)
+
+    def predict(self, Y, encoded,
+                encoded_padding_mask: Optional[torch.Tensor]):
+        """
+        Efficiently predict the next representation
+        of the last token in the Y sequence
+
+        Parameter
+        ---------
+        Y : torch.Tensor
+            Tensor of shape (N, Lq, D)
+        encoded : torch.Tensor
+            Tensor of shape (N, Lk, D)
+        encoded_padding_mask : torch.Tensor or None
+            mask of shape (N, Lk)
+
+        Returns
+        -------
+        torch.Tensor
+            tensor of shape (N, 1, D)
+        """
+        assert not self.training
+        encoded = encoded.to(self.device)
+        Y = Y.to(self.device)
+        N, L, _ = Y.shape
+        Q = Y[:, -1:, :]
+        input = Q.reshape(N, -1)
+        Q = self.masked_self_attention(Q, Y, mask_index_offset=L-1).reshape(N, -1)
+        Q = self.first_norm(Q + input).reshape(N, 1, -1)
+        input = Q.reshape(N, -1)
+        Q = self.attention(Q, encoded, query_padding_mask=None,
+                           key_padding_mask=encoded_padding_mask,
+                           mask_index_offset=L-1).reshape(N, -1)
+        Q = self.second_norm(Q + input)
+        input = Q
+        Q = self.contract(self.activation(self.expand(Q)))
+        Q = self.out_norm(Q + input)
+        return Q.reshape(N, 1, -1)
+
+    @property
+    def device(self) -> torch.device:
+        return self.masked_self_attention.key.weight.device
```

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_neural_network.py` & `pygmalion-0.1.3/pygmalion/neural_networks/_neural_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import io
 import copy
 import pathlib
 import torch
 from typing import Union, Sequence, Optional, Callable, Iterable, List
 from ._conversions import floats_to_tensor
-from pygmalion._model_base import ModelBase
-from pygmalion.datasets import download_bytes
+from pygmalion._model import Model
 
 
-class NeuralNetwork(torch.nn.Module, ModelBase):
+class NeuralNetwork(torch.nn.Module, Model):
     """
     Abstract class for neural networks
     Implemented as a simple wrapper around torch.nn.Module
     with 'fit' and 'predict' methods
     """
 
     def __init__(self):
         torch.nn.Module.__init__(self)
-        ModelBase.__init__(self)
-
-    @classmethod
-    def load(cls, file_path: Union[str, pathlib.Path, io.IOBase]) -> "NeuralNetwork":
-        file = download_bytes(file_path) if str(file_path).startswith("https://") else file_path
-        model = torch.load(file, map_location="cpu")
-        assert isinstance(model, cls)
-        return model
+        Model.__init__(self)
 
     def save(self, file_path: Union[str, pathlib.Path, io.IOBase],
              overwrite: bool = False, create_dir: bool = False):
         """
         Saves the model to the disk as '.pth' file
 
         Parameters
```

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_text_classifier.py` & `pygmalion-0.1.3/pygmalion/neural_networks/_text_classifier.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_text_segmenter.py` & `pygmalion-0.1.3/pygmalion/neural_networks/_text_segmenter.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/_text_translator.py` & `pygmalion-0.1.3/pygmalion/neural_networks/_text_translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import numpy as np
 from typing import Union, List, Sequence, Optional, Literal
 from itertools import count
 from warnings import warn
 from .layers.transformers import TransformerEncoder, TransformerDecoder, ATTENTION_TYPE
 from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding
-from ._conversions import strings_to_tensor, tensor_to_sentences
+from ._conversions import strings_to_tensor, tensor_to_strings
 from ._conversions import floats_to_tensor
 from ._neural_network import NeuralNetwork
 from ._loss_functions import cross_entropy
 from pygmalion.tokenizers._utilities import Tokenizer, SpecialToken
 
 
 class TextTranslator(NeuralNetwork):
@@ -317,24 +317,28 @@
         else:
             data = (x, y)
         return data
 
     def _x_to_tensor(self, x: List[str],
                      device: Optional[torch.device] = None,
                      max_input_sequence_length: Optional[int] = None,
-                     raise_on_longer_sequences: bool = False):
+                     raise_on_longer_sequences: bool = False,
+                     progress_bar: bool = False):
         return strings_to_tensor(x, self.tokenizer_input, device,
                                  max_sequence_length=self.input_sequence_length or max_input_sequence_length,
                                  raise_on_longer_sequences=raise_on_longer_sequences,
-                                 add_start_end_tokens=False)
+                                 add_start_end_tokens=False,
+                                 progress_bar=progress_bar)
 
     def _y_to_tensor(self, y: List[str],
                      device: Optional[torch.device] = None,
                      max_output_sequence_length: Optional[int] = None,
-                     raise_on_longer_sequences: bool = False) -> torch.Tensor:
+                     raise_on_longer_sequences: bool = False,
+                     progress_bar: bool = False) -> torch.Tensor:
         return strings_to_tensor(y, self.tokenizer_output, device,
                                  max_sequence_length=self.output_sequence_length or max_output_sequence_length,
                                  raise_on_longer_sequences=raise_on_longer_sequences,
-                                 add_start_end_tokens=True)
+                                 add_start_end_tokens=True,
+                                 progress_bar=progress_bar)
 
     def _tensor_to_y(self, tensor: torch.Tensor) -> np.ndarray:
-        return tensor_to_sentences(tensor, self.tokenizer_output)
+        return tensor_to_strings(tensor, self.tokenizer_output)
```

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/__init__.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/_activation.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/_activation.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,14 @@
 
     Example
     -------
     >>> Activation("relu")
 
     """
 
-    def __new__(cls, activation: Union[str, Callable, torch.nn.Module],
-                *args, **kwargs) -> torch.nn.Module:
-        if isinstance(activation, torch.nn.Module):
-            return activation
-        else:
-            obj = super().__new__(cls)
-            cls.__init__(obj, activation, *args, **kwargs)
-            return obj
-
     def __init__(self, activation: Union[str, Callable]):
         super().__init__()
         assert isinstance(activation, str) or callable(activation)
         assert not isinstance(activation, LambdaType), "Lambda function cannot be pickled and saved on disk"
         self.function = self._as_callable(activation)
 
     def __repr__(self):
```

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/_conv_block.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/_conv_block.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/_normalizer.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/_normalizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/_padded_conv.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/_padded_conv.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/_positional_encoding.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/_upsampling.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/_upsampling.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_attention.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_attention.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_multihead_attention.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_multihead_attention.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_stack.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_stack.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/neural_networks/layers/transformers/_utilities.py` & `pygmalion-0.1.3/pygmalion/neural_networks/layers/transformers/_utilities.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/tokenizers/_ascii_char_tokenizer.py` & `pygmalion-0.1.3/pygmalion/tokenizers/_ascii_char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/tokenizers/_byte_pair_encoder.py` & `pygmalion-0.1.3/pygmalion/tokenizers/_byte_pair_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,16 @@
                 code[new_token] = [token_indexes[b] for b in best_pair]
                 new_token_bytes = b"".join(best_pair)
                 self._bytes_tree.push(new_token_bytes)
                 token_indexes[new_token_bytes] = new_token
                 if verbose:
                     print(f"\r\033[K\rMerge iteration {i}: "
                           f"{len(code)} tokens, "
-                          f"new token frequency={new_token_frequency:.3g}",
+                          f"new token frequency={new_token_frequency:.3g} "
+                          f"({pair_count} occurences)",
                           end="", flush=True)
         except KeyboardInterrupt:
             print("\nInterupted by the user", end="")
         finally:
             print("")
         self.code = code
```

### Comparing `pygmalion-0.1.2/pygmalion/tokenizers/_utilities/_bytes_tree.py` & `pygmalion-0.1.3/pygmalion/tokenizers/_utilities/_bytes_tree.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/tokenizers/_utilities/_functions.py` & `pygmalion-0.1.3/pygmalion/tokenizers/_utilities/_functions.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/tokenizers/_utilities/_tokenizer_base.py` & `pygmalion-0.1.3/pygmalion/tokenizers/_utilities/_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, List, Tuple, Union, Iterable
 from unidecode import unidecode
-from pygmalion._model_base import ModelBase
+from pygmalion._model import Model
 from ._special_token import SpecialToken
 
 
-class Tokenizer(ModelBase):
+class Tokenizer(Model):
     """
     Tokenizer base is a base class for tokenizers
 
     Atributes
     ---------
     _ascii : bool
         whether or not to convert input to acii before tokenizing
```

### Comparing `pygmalion-0.1.2/pygmalion/tokenizers/_words_tokenizer.py` & `pygmalion-0.1.3/pygmalion/tokenizers/_words_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/unsupervised/pca.py` & `pygmalion-0.1.3/pygmalion/unsupervised/pca.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from typing import Dict, Tuple, Optional
-from pygmalion._model_base import ModelBase
+from pygmalion._model import Model
 
 
-class PCA(ModelBase):
+class PCA(Model):
 
     @classmethod
-    def from_dump(cls, dump: dict):
+    def from_dump(cls, dump: dict) -> "PCA":
         """
         """
         assert dump["type"] == cls.__name__
         projection = {k: (np.array(v[0], dtype=float), v[1]) for k, v in
                       dump["projection"].items()}
         return PCA(dump["offset"], dump["scale"], projection)
 
@@ -76,15 +76,15 @@
         total = sum(eigen)
         y = [sum(eigen[:i])/total for i in x]
         ax.plot(x, y)
         ax.set_ylabel("explained variance")
         ax.set_xlabel("number of components")
 
     @property
-    def dump(self):
+    def dump(self) -> dict:
         offset = dict(self.offset)
         scale = dict(self.scale) if self.scale is not None else self.scale
         projection = {k: [v[0].tolist(), v[1]] for k, v in
                       self.projection.items()}
         return {"type": type(self).__name__,
                 "offset": offset,
                 "scale": scale,
```

### Comparing `pygmalion-0.1.2/pygmalion/utilities/_cross_validation.py` & `pygmalion-0.1.3/pygmalion/utilities/_cross_validation.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/utilities/_decorators.py` & `pygmalion-0.1.3/pygmalion/utilities/_decorators.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/utilities/_metrics.py` & `pygmalion-0.1.3/pygmalion/utilities/_metrics.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/pygmalion/utilities/_ploting.py` & `pygmalion-0.1.3/pygmalion/utilities/_ploting.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,45 +73,55 @@
                         class_colors: dict = {}, default_color: str = "r",
                         label_class: bool = True):
     """
     plot the image with given bounding boxes
 
     Parameters
     ----------
+
     bounding_boxes : dict
         A dict containing the following keys:
-        * x1, y1, x2, y2 : list of int
+        * x, y, w, h : list of int or float
             The coordinates in pixel of each bboxe corner
         * class : list of str
             The name of the class predicted for eahc bboxe
-        * [confidence : list of float]
+        * [bboxe confidence : list of float]
             The optional confidence of the bounding boxe
+        * [class confidence : list of float]
+            The optional confidence of detected classes
+
     ax : matplotlib.axes.Axes
         The matplotlib axes to draw on
+
     class_colors : dict
         A dictionary of {class: color} for the color of the boxes
         Can be any color format supported by matplotlib
+
     default_color : str or list
         the default color for classes that are not present in class_colors
+        Can be either a string ("#ff0000", "r", ...)
+        or a RGB/RGBA list ([255, 0, 0], [255, 0, 0, 255], ...)
     """
-    coords = zip(bboxes["x1"], bboxes["y1"], bboxes["x2"], bboxes["y2"])
-    for i, (x1, y1, x2, y2) in enumerate(coords):
+    coords = zip(bboxes["x"], bboxes["y"], bboxes["w"], bboxes["h"])
+    for i, (x, y, w, h) in enumerate(coords):
+        x1, x2 = x-w/2, x+w/2
+        y1, y2 = y-h/2, y+h/2
         boxe_class = bboxes["class"][i]
         boxe_color = class_colors.get(boxe_class, default_color)
-        xinf, yinf = min(x1, x2), min(y1, y2)
-        w, h = abs(x2-x1), abs(y2-y1)
-        rect = patches.Rectangle((xinf, yinf), w, h,
+        rect = patches.Rectangle((x1, y1), w, h,
                                  linewidth=1, edgecolor=boxe_color,
                                  facecolor='none')
         if label_class:
             s = boxe_class
-            confidence = bboxes.get("confidence", None)
-            if confidence is not None:
-                s += f": {confidence[i]*100:.1f}%"
-            ax.text(xinf, yinf-1, s, color=boxe_color)
+            bboxe_confidence = bboxes.get("bboxe confidence", None)
+            class_confidence = bboxes.get("class confidence", None)
+            if bboxe_confidence is not None and class_confidence is not None:
+                confidence = class_confidence[i] * bboxe_confidence[i]
+                s += f": {confidence:.1%}"
+            ax.text(x1, y1, s, color=boxe_color)
         ax.add_patch(rect)
     ax.set_xticks([])
     ax.set_yticks([])
 
 
 def plot_matrix(table: pd.DataFrame,
                 ax: Union[None, matplotlib.axes.Axes] = None,
```

### Comparing `pygmalion-0.1.2/pygmalion.egg-info/PKG-INFO` & `pygmalion-0.1.3/pygmalion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmalion
-Version: 0.1.2
+Version: 0.1.3
 Summary: A machine learning package
 Home-page: https://github.com/BFavier/Pygmalion
 Author: Benoit Favier
 Author-email: benoitfamillefavier@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygmalion-0.1.2/pygmalion.egg-info/SOURCES.txt` & `pygmalion-0.1.3/pygmalion.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 LICENSE
 README.md
 setup.py
 pygmalion/__init__.py
 pygmalion/_info.py
-pygmalion/_model_base.py
+pygmalion/_model.py
 pygmalion.egg-info/PKG-INFO
 pygmalion.egg-info/SOURCES.txt
 pygmalion.egg-info/dependency_links.txt
 pygmalion.egg-info/requires.txt
 pygmalion.egg-info/top_level.txt
 pygmalion/datasets/__init__.py
 pygmalion/datasets/_airline_tweets.py
+pygmalion/datasets/_aquarium.py
 pygmalion/datasets/_boston_housing.py
 pygmalion/datasets/_cityscapes.py
-pygmalion/datasets/_download.py
 pygmalion/datasets/_fashion_mnist.py
 pygmalion/datasets/_iris.py
 pygmalion/datasets/_sentence_pairs.py
 pygmalion/datasets/_titanic.py
 pygmalion/datasets/generators/__init__.py
 pygmalion/datasets/generators/_circles_generator.py
 pygmalion/datasets/generators/_roman_numerals_generator.py
+pygmalion/datasets/generators/_shapes_generator.py
 pygmalion/neural_networks/__init__.py
 pygmalion/neural_networks/_conversions.py
 pygmalion/neural_networks/_dense_classifier.py
 pygmalion/neural_networks/_dense_regressor.py
 pygmalion/neural_networks/_image_classifier.py
+pygmalion/neural_networks/_image_object_detector.py
 pygmalion/neural_networks/_image_segmenter.py
 pygmalion/neural_networks/_loss_functions.py
 pygmalion/neural_networks/_neural_network.py
-pygmalion/neural_networks/_object_detector.py
 pygmalion/neural_networks/_text_classifier.py
 pygmalion/neural_networks/_text_segmenter.py
 pygmalion/neural_networks/_text_translator.py
 pygmalion/neural_networks/layers/__init__.py
 pygmalion/neural_networks/layers/_activation.py
 pygmalion/neural_networks/layers/_conv_block.py
 pygmalion/neural_networks/layers/_normalizer.py
@@ -50,17 +51,19 @@
 pygmalion/tokenizers/_ascii_char_tokenizer.py
 pygmalion/tokenizers/_byte_pair_encoder.py
 pygmalion/tokenizers/_words_tokenizer.py
 pygmalion/tokenizers/_utilities/__init__.py
 pygmalion/tokenizers/_utilities/_bytes_tree.py
 pygmalion/tokenizers/_utilities/_functions.py
 pygmalion/tokenizers/_utilities/_special_token.py
-pygmalion/tokenizers/_utilities/_tokenizer_base.py
+pygmalion/tokenizers/_utilities/_tokenizer.py
 pygmalion/unsupervised/__init__.py
 pygmalion/unsupervised/pca.py
 pygmalion/utilities/__init__.py
 pygmalion/utilities/_cross_validation.py
 pygmalion/utilities/_decorators.py
+pygmalion/utilities/_download.py
+pygmalion/utilities/_load_model.py
 pygmalion/utilities/_metrics.py
 pygmalion/utilities/_ploting.py
 test/test_decoder_stage.py
 test/test_kernelized_attention.py
```

### Comparing `pygmalion-0.1.2/setup.py` & `pygmalion-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/test/test_decoder_stage.py` & `pygmalion-0.1.3/test/test_decoder_stage.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.2/test/test_kernelized_attention.py` & `pygmalion-0.1.3/test/test_kernelized_attention.py`

 * *Files identical despite different names*

