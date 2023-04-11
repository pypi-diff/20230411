# Comparing `tmp/roof_mask-0.5.3.tar.gz` & `tmp/roof-mask-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roof_mask-0.5.3.tar", last modified: Tue Apr 11 13:37:40 2023, max compression
+gzip compressed data, was "roof-mask-0.5.4.tar", last modified: Tue Apr 11 18:20:32 2023, max compression
```

## Comparing `roof_mask-0.5.3.tar` & `roof-mask-0.5.4.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:06.732834 roof_mask-0.5.3/
--rwxrwxrwx   0 root         (0) root         (0)      525 2023-04-11 13:37:40.584944 roof_mask-0.5.3/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:06.784805 roof_mask-0.5.3/detectron2/
--rwxrwxrwx   0 root         (0) root         (0)      258 2023-03-20 23:41:43.000000 roof_mask-0.5.3/detectron2/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:06.895741 roof_mask-0.5.3/detectron2/checkpoint/
--rwxrwxrwx   0 root         (0) root         (0)      347 2023-03-20 23:41:48.000000 roof_mask-0.5.3/detectron2/checkpoint/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    17782 2023-03-20 23:41:48.000000 roof_mask-0.5.3/detectron2/checkpoint/c2_model_loading.py
--rwxrwxrwx   0 root         (0) root         (0)     5685 2023-03-20 23:41:48.000000 roof_mask-0.5.3/detectron2/checkpoint/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     5258 2023-03-20 23:41:48.000000 roof_mask-0.5.3/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:06.988688 roof_mask-0.5.3/detectron2/config/
--rwxrwxrwx   0 root         (0) root         (0)      599 2023-03-20 23:41:38.000000 roof_mask-0.5.3/detectron2/config/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7890 2023-03-20 23:41:38.000000 roof_mask-0.5.3/detectron2/config/compat.py
--rwxrwxrwx   0 root         (0) root         (0)     9211 2023-03-20 23:41:38.000000 roof_mask-0.5.3/detectron2/config/config.py
--rwxrwxrwx   0 root         (0) root         (0)    29512 2023-03-20 23:41:38.000000 roof_mask-0.5.3/detectron2/config/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)     2719 2023-03-20 23:41:38.000000 roof_mask-0.5.3/detectron2/config/instantiate.py
--rwxrwxrwx   0 root         (0) root         (0)    14944 2023-03-20 23:41:39.000000 roof_mask-0.5.3/detectron2/config/lazy.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.075638 roof_mask-0.5.3/detectron2/data/
--rwxrwxrwx   0 root         (0) root         (0)      644 2023-03-20 23:41:43.000000 roof_mask-0.5.3/detectron2/data/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7378 2023-03-20 23:41:44.000000 roof_mask-0.5.3/detectron2/data/benchmark.py
--rwxrwxrwx   0 root         (0) root         (0)    20605 2023-03-20 23:41:46.000000 roof_mask-0.5.3/detectron2/data/build.py
--rwxrwxrwx   0 root         (0) root         (0)     7224 2023-03-20 23:41:43.000000 roof_mask-0.5.3/detectron2/data/catalog.py
--rwxrwxrwx   0 root         (0) root         (0)     9164 2023-03-20 23:41:46.000000 roof_mask-0.5.3/detectron2/data/common.py
--rwxrwxrwx   0 root         (0) root         (0)     8169 2023-03-20 23:41:46.000000 roof_mask-0.5.3/detectron2/data/dataset_mapper.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.160588 roof_mask-0.5.3/detectron2/data/datasets/
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-03-20 23:41:44.000000 roof_mask-0.5.3/detectron2/data/datasets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10174 2023-03-20 23:41:45.000000 roof_mask-0.5.3/detectron2/data/datasets/builtin.py
--rwxrwxrwx   0 root         (0) root         (0)    21841 2023-03-20 23:41:44.000000 roof_mask-0.5.3/detectron2/data/datasets/builtin_meta.py
--rwxrwxrwx   0 root         (0) root         (0)    13167 2023-03-20 23:41:45.000000 roof_mask-0.5.3/detectron2/data/datasets/cityscapes.py
--rwxrwxrwx   0 root         (0) root         (0)     7821 2023-03-20 23:41:44.000000 roof_mask-0.5.3/detectron2/data/datasets/cityscapes_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)    23465 2023-03-20 23:41:45.000000 roof_mask-0.5.3/detectron2/data/datasets/coco.py
--rwxrwxrwx   0 root         (0) root         (0)     8977 2023-03-20 23:41:44.000000 roof_mask-0.5.3/detectron2/data/datasets/coco_panoptic.py
--rwxrwxrwx   0 root         (0) root         (0)     9623 2023-03-20 23:41:45.000000 roof_mask-0.5.3/detectron2/data/datasets/lvis.py
--rwxrwxrwx   0 root         (0) root         (0)   223757 2023-03-20 23:41:44.000000 roof_mask-0.5.3/detectron2/data/datasets/lvis_v0_5_categories.py
--rwxrwxrwx   0 root         (0) root         (0)   219177 2023-03-20 23:41:45.000000 roof_mask-0.5.3/detectron2/data/datasets/lvis_v1_categories.py
--rwxrwxrwx   0 root         (0) root         (0)    39414 2023-03-20 23:41:44.000000 roof_mask-0.5.3/detectron2/data/datasets/lvis_v1_category_image_count.py
--rwxrwxrwx   0 root         (0) root         (0)     3128 2023-03-20 23:41:45.000000 roof_mask-0.5.3/detectron2/data/datasets/pascal_voc.py
--rwxrwxrwx   0 root         (0) root         (0)      169 2023-03-20 23:41:45.000000 roof_mask-0.5.3/detectron2/data/datasets/register_coco.py
--rwxrwxrwx   0 root         (0) root         (0)    22841 2023-03-20 23:41:46.000000 roof_mask-0.5.3/detectron2/data/detection_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.231548 roof_mask-0.5.3/detectron2/data/samplers/
--rwxrwxrwx   0 root         (0) root         (0)      412 2023-03-20 23:41:47.000000 roof_mask-0.5.3/detectron2/data/samplers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11789 2023-03-20 23:41:47.000000 roof_mask-0.5.3/detectron2/data/samplers/distributed_sampler.py
--rwxrwxrwx   0 root         (0) root         (0)     1944 2023-03-20 23:41:47.000000 roof_mask-0.5.3/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.290514 roof_mask-0.5.3/detectron2/data/transforms/
--rwxrwxrwx   0 root         (0) root         (0)      466 2023-03-20 23:41:46.000000 roof_mask-0.5.3/detectron2/data/transforms/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14117 2023-03-20 23:41:46.000000 roof_mask-0.5.3/detectron2/data/transforms/augmentation.py
--rwxrwxrwx   0 root         (0) root         (0)    23069 2023-03-20 23:41:46.000000 roof_mask-0.5.3/detectron2/data/transforms/augmentation_impl.py
--rwxrwxrwx   0 root         (0) root         (0)    12629 2023-03-20 23:41:46.000000 roof_mask-0.5.3/detectron2/data/transforms/transform.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.335489 roof_mask-0.5.3/detectron2/engine/
--rwxrwxrwx   0 root         (0) root         (0)      340 2023-03-20 23:41:47.000000 roof_mask-0.5.3/detectron2/engine/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26868 2023-03-20 23:41:47.000000 roof_mask-0.5.3/detectron2/engine/defaults.py
--rwxrwxrwx   0 root         (0) root         (0)    25497 2023-03-20 23:41:48.000000 roof_mask-0.5.3/detectron2/engine/hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     4089 2023-03-20 23:41:47.000000 roof_mask-0.5.3/detectron2/engine/launch.py
--rwxrwxrwx   0 root         (0) root         (0)    14104 2023-03-20 23:41:47.000000 roof_mask-0.5.3/detectron2/engine/train_loop.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.391456 roof_mask-0.5.3/detectron2/evaluation/
--rwxrwxrwx   0 root         (0) root         (0)      671 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8369 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/cityscapes_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    30423 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8156 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/evaluator.py
--rwxrwxrwx   0 root         (0) root         (0)     5078 2023-03-20 23:41:55.000000 roof_mask-0.5.3/detectron2/evaluation/fast_eval_api.py
--rwxrwxrwx   0 root         (0) root         (0)    15018 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/lvis_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7500 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/panoptic_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)    10862 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/pascal_voc_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     7608 2023-03-20 23:41:55.000000 roof_mask-0.5.3/detectron2/evaluation/rotated_coco_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     8191 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/sem_seg_evaluation.py
--rwxrwxrwx   0 root         (0) root         (0)     2614 2023-03-20 23:41:54.000000 roof_mask-0.5.3/detectron2/evaluation/testing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.462416 roof_mask-0.5.3/detectron2/export/
--rwxrwxrwx   0 root         (0) root         (0)      336 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9280 2023-03-20 23:41:51.000000 roof_mask-0.5.3/detectron2/export/api.py
--rwxrwxrwx   0 root         (0) root         (0)    21035 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/c10.py
--rwxrwxrwx   0 root         (0) root         (0)     7803 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/caffe2_export.py
--rwxrwxrwx   0 root         (0) root         (0)     6674 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/caffe2_inference.py
--rwxrwxrwx   0 root         (0) root         (0)    17034 2023-03-20 23:41:51.000000 roof_mask-0.5.3/detectron2/export/caffe2_modeling.py
--rwxrwxrwx   0 root         (0) root         (0)     5033 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/caffe2_patch.py
--rwxrwxrwx   0 root         (0) root         (0)    11807 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/flatten.py
--rwxrwxrwx   0 root         (0) root         (0)    38071 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/shared.py
--rwxrwxrwx   0 root         (0) root         (0)     5008 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/torchscript.py
--rwxrwxrwx   0 root         (0) root         (0)    11526 2023-03-20 23:41:52.000000 roof_mask-0.5.3/detectron2/export/torchscript_patch.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.527378 roof_mask-0.5.3/detectron2/layers/
--rwxrwxrwx   0 root         (0) root         (0)      839 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5764 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/aspp.py
--rwxrwxrwx   0 root         (0) root         (0)    12131 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/batch_norm.py
--rwxrwxrwx   0 root         (0) root         (0)     3024 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/blocks.py
--rwxrwxrwx   0 root         (0) root         (0)    16978 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/deform_conv.py
--rwxrwxrwx   0 root         (0) root         (0)     4204 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/losses.py
--rwxrwxrwx   0 root         (0) root         (0)    10881 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/mask_ops.py
--rwxrwxrwx   0 root         (0) root         (0)     6490 2023-03-20 23:41:38.000000 roof_mask-0.5.3/detectron2/layers/nms.py
--rwxrwxrwx   0 root         (0) root         (0)     3098 2023-03-20 23:41:33.000000 roof_mask-0.5.3/detectron2/layers/roi_align.py
--rwxrwxrwx   0 root         (0) root         (0)     3302 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/roi_align_rotated.py
--rwxrwxrwx   0 root         (0) root         (0)      652 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/rotated_boxes.py
--rwxrwxrwx   0 root         (0) root         (0)      661 2023-03-20 23:41:38.000000 roof_mask-0.5.3/detectron2/layers/shape_spec.py
--rwxrwxrwx   0 root         (0) root         (0)     4893 2023-03-20 23:41:37.000000 roof_mask-0.5.3/detectron2/layers/wrappers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.601336 roof_mask-0.5.3/detectron2/modeling/
--rwxrwxrwx   0 root         (0) root         (0)     1475 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15443 2023-03-20 23:41:43.000000 roof_mask-0.5.3/detectron2/modeling/anchor_generator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.683289 roof_mask-0.5.3/detectron2/modeling/backbone/
--rwxrwxrwx   0 root         (0) root         (0)      475 2023-03-20 23:41:39.000000 roof_mask-0.5.3/detectron2/modeling/backbone/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1543 2023-03-20 23:41:39.000000 roof_mask-0.5.3/detectron2/modeling/backbone/backbone.py
--rwxrwxrwx   0 root         (0) root         (0)     1015 2023-03-20 23:41:39.000000 roof_mask-0.5.3/detectron2/modeling/backbone/build.py
--rwxrwxrwx   0 root         (0) root         (0)    10055 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/backbone/fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    16656 2023-03-20 23:41:39.000000 roof_mask-0.5.3/detectron2/modeling/backbone/regnet.py
--rwxrwxrwx   0 root         (0) root         (0)    23658 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/backbone/resnet.py
--rwxrwxrwx   0 root         (0) root         (0)    15123 2023-03-20 23:41:43.000000 roof_mask-0.5.3/detectron2/modeling/box_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     6264 2023-03-20 23:41:39.000000 roof_mask-0.5.3/detectron2/modeling/matcher.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.750250 roof_mask-0.5.3/detectron2/modeling/meta_arch/
--rwxrwxrwx   0 root         (0) root         (0)      508 2023-03-20 23:41:41.000000 roof_mask-0.5.3/detectron2/modeling/meta_arch/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      814 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/meta_arch/build.py
--rwxrwxrwx   0 root         (0) root         (0)    11550 2023-03-20 23:41:41.000000 roof_mask-0.5.3/detectron2/modeling/meta_arch/dense_detector.py
--rwxrwxrwx   0 root         (0) root         (0)    13213 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/meta_arch/fcos.py
--rwxrwxrwx   0 root         (0) root         (0)    10335 2023-03-20 23:41:41.000000 roof_mask-0.5.3/detectron2/modeling/meta_arch/panoptic_fpn.py
--rwxrwxrwx   0 root         (0) root         (0)    13710 2023-03-20 23:41:41.000000 roof_mask-0.5.3/detectron2/modeling/meta_arch/rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    18265 2023-03-20 23:41:41.000000 roof_mask-0.5.3/detectron2/modeling/meta_arch/retinanet.py
--rwxrwxrwx   0 root         (0) root         (0)     9720 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/meta_arch/semantic_seg.py
--rwxrwxrwx   0 root         (0) root         (0)    10832 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/mmdet_wrapper.py
--rwxrwxrwx   0 root         (0) root         (0)    11316 2023-03-20 23:41:43.000000 roof_mask-0.5.3/detectron2/modeling/poolers.py
--rwxrwxrwx   0 root         (0) root         (0)     4046 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/postprocessing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.809217 roof_mask-0.5.3/detectron2/modeling/proposal_generator/
--rwxrwxrwx   0 root         (0) root         (0)      231 2023-03-20 23:41:41.000000 roof_mask-0.5.3/detectron2/modeling/proposal_generator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      836 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/proposal_generator/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8128 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/proposal_generator/proposal_utils.py
--rwxrwxrwx   0 root         (0) root         (0)    23814 2023-03-20 23:41:41.000000 roof_mask-0.5.3/detectron2/modeling/proposal_generator/rpn.py
--rwxrwxrwx   0 root         (0) root         (0)     8807 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.868183 roof_mask-0.5.3/detectron2/modeling/roi_heads/
--rwxrwxrwx   0 root         (0) root         (0)      768 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/roi_heads/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4077 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/roi_heads/box_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12990 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/roi_heads/cascade_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    25274 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/roi_heads/fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)    11156 2023-03-20 23:41:43.000000 roof_mask-0.5.3/detectron2/modeling/roi_heads/keypoint_head.py
--rwxrwxrwx   0 root         (0) root         (0)    12169 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/roi_heads/mask_head.py
--rwxrwxrwx   0 root         (0) root         (0)    37701 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/roi_heads/roi_heads.py
--rwxrwxrwx   0 root         (0) root         (0)    11158 2023-03-20 23:41:42.000000 roof_mask-0.5.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rwxrwxrwx   0 root         (0) root         (0)     2334 2023-03-20 23:41:40.000000 roof_mask-0.5.3/detectron2/modeling/sampling.py
--rwxrwxrwx   0 root         (0) root         (0)    12416 2023-03-20 23:41:41.000000 roof_mask-0.5.3/detectron2/modeling/test_time_augmentation.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.915156 roof_mask-0.5.3/detectron2/solver/
--rwxrwxrwx   0 root         (0) root         (0)      298 2023-03-20 23:41:55.000000 roof_mask-0.5.3/detectron2/solver/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11127 2023-03-20 23:41:55.000000 roof_mask-0.5.3/detectron2/solver/build.py
--rwxrwxrwx   0 root         (0) root         (0)     8648 2023-03-20 23:41:55.000000 roof_mask-0.5.3/detectron2/solver/lr_scheduler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:07.987115 roof_mask-0.5.3/detectron2/structures/
--rwxrwxrwx   0 root         (0) root         (0)      645 2023-03-20 23:41:51.000000 roof_mask-0.5.3/detectron2/structures/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14429 2023-03-20 23:41:51.000000 roof_mask-0.5.3/detectron2/structures/boxes.py
--rwxrwxrwx   0 root         (0) root         (0)     4557 2023-03-20 23:41:51.000000 roof_mask-0.5.3/detectron2/structures/image_list.py
--rwxrwxrwx   0 root         (0) root         (0)     6542 2023-03-20 23:41:51.000000 roof_mask-0.5.3/detectron2/structures/instances.py
--rwxrwxrwx   0 root         (0) root         (0)     9030 2023-03-20 23:41:51.000000 roof_mask-0.5.3/detectron2/structures/keypoints.py
--rwxrwxrwx   0 root         (0) root         (0)    19802 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/structures/masks.py
--rwxrwxrwx   0 root         (0) root         (0)    18853 2023-03-20 23:41:51.000000 roof_mask-0.5.3/detectron2/structures/rotated_boxes.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.048080 roof_mask-0.5.3/detectron2/tracking/
--rwxrwxrwx   0 root         (0) root         (0)      580 2023-03-20 23:41:53.000000 roof_mask-0.5.3/detectron2/tracking/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2216 2023-03-20 23:41:53.000000 roof_mask-0.5.3/detectron2/tracking/base_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)    11858 2023-03-20 23:41:53.000000 roof_mask-0.5.3/detectron2/tracking/bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     7486 2023-03-20 23:41:53.000000 roof_mask-0.5.3/detectron2/tracking/hungarian_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     4142 2023-03-20 23:41:53.000000 roof_mask-0.5.3/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
--rwxrwxrwx   0 root         (0) root         (0)     1106 2023-03-20 23:41:53.000000 roof_mask-0.5.3/detectron2/tracking/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     5288 2023-03-20 23:41:53.000000 roof_mask-0.5.3/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.108046 roof_mask-0.5.3/detectron2/utils/
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6017 2023-03-20 23:41:49.000000 roof_mask-0.5.3/detectron2/utils/analysis.py
--rwxrwxrwx   0 root         (0) root         (0)     8391 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/utils/collect_env.py
--rwxrwxrwx   0 root         (0) root         (0)     4096 2023-03-20 23:41:49.000000 roof_mask-0.5.3/detectron2/utils/colormap.py
--rwxrwxrwx   0 root         (0) root         (0)     5610 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/utils/comm.py
--rwxrwxrwx   0 root         (0) root         (0)     1838 2023-03-20 23:41:49.000000 roof_mask-0.5.3/detectron2/utils/develop.py
--rwxrwxrwx   0 root         (0) root         (0)     5644 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/utils/env.py
--rwxrwxrwx   0 root         (0) root         (0)    17024 2023-03-20 23:41:49.000000 roof_mask-0.5.3/detectron2/utils/events.py
--rwxrwxrwx   0 root         (0) root         (0)     1189 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/utils/file_io.py
--rwxrwxrwx   0 root         (0) root         (0)     7807 2023-03-20 23:41:49.000000 roof_mask-0.5.3/detectron2/utils/logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2583 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/utils/memory.py
--rwxrwxrwx   0 root         (0) root         (0)     1874 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/utils/registry.py
--rwxrwxrwx   0 root         (0) root         (0)     1064 2023-03-20 23:41:48.000000 roof_mask-0.5.3/detectron2/utils/serialize.py
--rwxrwxrwx   0 root         (0) root         (0)     4833 2023-03-20 23:41:49.000000 roof_mask-0.5.3/detectron2/utils/testing.py
--rwxrwxrwx   0 root         (0) root         (0)    11319 2023-03-20 23:41:49.000000 roof_mask-0.5.3/detectron2/utils/video_visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    51159 2023-03-20 23:41:50.000000 roof_mask-0.5.3/detectron2/utils/visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)    52915 2023-03-20 23:41:49.000000 roof_mask-0.5.3/detectron2/utils/visualizer_new.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.155019 roof_mask-0.5.3/models/
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-03-20 23:41:58.000000 roof_mask-0.5.3/models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    41260 2023-03-20 23:41:58.000000 roof_mask-0.5.3/models/common.py
--rwxrwxrwx   0 root         (0) root         (0)     4319 2023-03-20 23:41:58.000000 roof_mask-0.5.3/models/experimental.py
--rwxrwxrwx   0 root         (0) root         (0)    25494 2023-03-20 23:41:57.000000 roof_mask-0.5.3/models/tf.py
--rwxrwxrwx   0 root         (0) root         (0)    22240 2023-03-20 23:41:58.000000 roof_mask-0.5.3/models/yolo.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.217982 roof_mask-0.5.3/roof_mask.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      525 2023-04-11 13:37:34.000000 roof_mask-0.5.3/roof_mask.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     6263 2023-04-11 13:37:06.000000 roof_mask-0.5.3/roof_mask.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-11 13:37:34.000000 roof_mask-0.5.3/roof_mask.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-11 13:37:34.000000 roof_mask-0.5.3/roof_mask.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.314927 roof_mask-0.5.3/roof_test/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 23:42:00.000000 roof_mask-0.5.3/roof_test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-04-10 17:56:52.000000 roof_mask-0.5.3/roof_test/a.py
--rwxrwxrwx   0 root         (0) root         (0)      191 2023-03-20 23:42:00.000000 roof_mask-0.5.3/roof_test/predict.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-11 13:37:40.728946 roof_mask-0.5.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      700 2023-04-10 16:56:16.000000 roof_mask-0.5.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.366897 roof_mask-0.5.3/tests/
--rwxrwxrwx   0 root         (0) root         (0)     2629 2023-04-11 13:37:35.000000 roof_mask-0.5.3/tests/test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.437857 roof_mask-0.5.3/utils/
--rwxrwxrwx   0 root         (0) root         (0)     1842 2023-03-20 23:42:04.000000 roof_mask-0.5.3/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3449 2023-03-20 23:42:02.000000 roof_mask-0.5.3/utils/activations.py
--rwxrwxrwx   0 root         (0) root         (0)    14782 2023-03-20 23:42:03.000000 roof_mask-0.5.3/utils/augmentations.py
--rwxrwxrwx   0 root         (0) root         (0)     7411 2023-03-20 23:42:03.000000 roof_mask-0.5.3/utils/autoanchor.py
--rwxrwxrwx   0 root         (0) root         (0)     2767 2023-03-20 23:42:04.000000 roof_mask-0.5.3/utils/autobatch.py
--rwxrwxrwx   0 root         (0) root         (0)     6958 2023-03-20 23:42:00.000000 roof_mask-0.5.3/utils/benchmarks.py
--rwxrwxrwx   0 root         (0) root         (0)     2661 2023-03-20 23:42:03.000000 roof_mask-0.5.3/utils/callbacks.py
--rwxrwxrwx   0 root         (0) root         (0)    51717 2023-03-20 23:42:02.000000 roof_mask-0.5.3/utils/dataloaders.py
--rwxrwxrwx   0 root         (0) root         (0)     7329 2023-03-20 23:42:03.000000 roof_mask-0.5.3/utils/downloads.py
--rwxrwxrwx   0 root         (0) root         (0)    48476 2023-03-20 23:42:02.000000 roof_mask-0.5.3/utils/general.py
--rwxrwxrwx   0 root         (0) root         (0)     9919 2023-03-20 23:42:03.000000 roof_mask-0.5.3/utils/loss.py
--rwxrwxrwx   0 root         (0) root         (0)    14706 2023-03-20 23:42:02.000000 roof_mask-0.5.3/utils/metrics.py
--rwxrwxrwx   0 root         (0) root         (0)    22815 2023-03-20 23:42:04.000000 roof_mask-0.5.3/utils/plots.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.499822 roof_mask-0.5.3/utils/segment/
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-03-20 23:42:02.000000 roof_mask-0.5.3/utils/segment/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3756 2023-03-20 23:42:01.000000 roof_mask-0.5.3/utils/segment/augmentations.py
--rwxrwxrwx   0 root         (0) root         (0)    13499 2023-03-20 23:42:02.000000 roof_mask-0.5.3/utils/segment/dataloaders.py
--rwxrwxrwx   0 root         (0) root         (0)     4480 2023-03-20 23:42:01.000000 roof_mask-0.5.3/utils/segment/general.py
--rwxrwxrwx   0 root         (0) root         (0)     8632 2023-03-20 23:42:00.000000 roof_mask-0.5.3/utils/segment/loss.py
--rwxrwxrwx   0 root         (0) root         (0)     5457 2023-03-20 23:42:02.000000 roof_mask-0.5.3/utils/segment/metrics.py
--rwxrwxrwx   0 root         (0) root         (0)     7859 2023-03-20 23:42:00.000000 roof_mask-0.5.3/utils/segment/plots.py
--rwxrwxrwx   0 root         (0) root         (0)    19970 2023-03-20 23:42:03.000000 roof_mask-0.5.3/utils/torch_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 13:37:08.547793 roof_mask-0.5.3/yolo_roof/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 23:42:04.000000 roof_mask-0.5.3/yolo_roof/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    27812 2023-04-10 20:09:08.000000 roof_mask-0.5.3/yolo_roof/detect_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    28494 2023-03-20 23:42:05.000000 roof_mask-0.5.3/yolo_roof/export.py
--rwxrwxrwx   0 root         (0) root         (0)    21374 2023-03-31 21:05:06.000000 roof_mask-0.5.3/yolo_roof/geo_functions.py
--rwxrwxrwx   0 root         (0) root         (0)    33193 2023-03-23 16:17:29.000000 roof_mask-0.5.3/yolo_roof/report_functions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:17.739408 roof-mask-0.5.4/
+-rwxrwxrwx   0 root         (0) root         (0)      548 2023-04-11 18:20:32.075026 roof-mask-0.5.4/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:17.797375 roof-mask-0.5.4/detectron2/
+-rwxrwxrwx   0 root         (0) root         (0)      258 2023-03-20 23:41:43.000000 roof-mask-0.5.4/detectron2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:17.942292 roof-mask-0.5.4/detectron2/checkpoint/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2023-03-20 23:41:48.000000 roof-mask-0.5.4/detectron2/checkpoint/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:20.742847 roof-mask-0.5.4/detectron2/checkpoint/c2_model_loading.py
+-rwxrwxrwx   0 root         (0) root         (0)     5685 2023-03-20 23:41:48.000000 roof-mask-0.5.4/detectron2/checkpoint/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     5258 2023-03-20 23:41:48.000000 roof-mask-0.5.4/detectron2/checkpoint/detection_checkpoint.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.050230 roof-mask-0.5.4/detectron2/config/
+-rwxrwxrwx   0 root         (0) root         (0)      599 2023-03-20 23:41:38.000000 roof-mask-0.5.4/detectron2/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7890 2023-03-20 23:41:38.000000 roof-mask-0.5.4/detectron2/config/compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     9211 2023-03-20 23:41:38.000000 roof-mask-0.5.4/detectron2/config/config.py
+-rwxrwxrwx   0 root         (0) root         (0)    29512 2023-03-20 23:41:38.000000 roof-mask-0.5.4/detectron2/config/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)     2719 2023-03-20 23:41:38.000000 roof-mask-0.5.4/detectron2/config/instantiate.py
+-rwxrwxrwx   0 root         (0) root         (0)    14944 2023-03-20 23:41:39.000000 roof-mask-0.5.4/detectron2/config/lazy.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.129184 roof-mask-0.5.4/detectron2/data/
+-rwxrwxrwx   0 root         (0) root         (0)      644 2023-03-20 23:41:43.000000 roof-mask-0.5.4/detectron2/data/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7378 2023-03-20 23:41:44.000000 roof-mask-0.5.4/detectron2/data/benchmark.py
+-rwxrwxrwx   0 root         (0) root         (0)    20605 2023-03-20 23:41:46.000000 roof-mask-0.5.4/detectron2/data/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     7224 2023-03-20 23:41:43.000000 roof-mask-0.5.4/detectron2/data/catalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     9164 2023-03-20 23:41:46.000000 roof-mask-0.5.4/detectron2/data/common.py
+-rwxrwxrwx   0 root         (0) root         (0)     8169 2023-03-20 23:41:46.000000 roof-mask-0.5.4/detectron2/data/dataset_mapper.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.247117 roof-mask-0.5.4/detectron2/data/datasets/
+-rwxrwxrwx   0 root         (0) root         (0)      523 2023-03-20 23:41:44.000000 roof-mask-0.5.4/detectron2/data/datasets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10174 2023-03-20 23:41:45.000000 roof-mask-0.5.4/detectron2/data/datasets/builtin.py
+-rwxrwxrwx   0 root         (0) root         (0)    21841 2023-03-20 23:41:44.000000 roof-mask-0.5.4/detectron2/data/datasets/builtin_meta.py
+-rwxrwxrwx   0 root         (0) root         (0)    13167 2023-03-20 23:41:45.000000 roof-mask-0.5.4/detectron2/data/datasets/cityscapes.py
+-rwxrwxrwx   0 root         (0) root         (0)     7821 2023-03-20 23:41:44.000000 roof-mask-0.5.4/detectron2/data/datasets/cityscapes_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)    23465 2023-03-20 23:41:45.000000 roof-mask-0.5.4/detectron2/data/datasets/coco.py
+-rwxrwxrwx   0 root         (0) root         (0)     8977 2023-03-20 23:41:44.000000 roof-mask-0.5.4/detectron2/data/datasets/coco_panoptic.py
+-rwxrwxrwx   0 root         (0) root         (0)     9623 2023-03-20 23:41:45.000000 roof-mask-0.5.4/detectron2/data/datasets/lvis.py
+-rwxrwxrwx   0 root         (0) root         (0)   223757 2023-03-20 23:41:44.000000 roof-mask-0.5.4/detectron2/data/datasets/lvis_v0_5_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)   219177 2023-03-20 23:41:45.000000 roof-mask-0.5.4/detectron2/data/datasets/lvis_v1_categories.py
+-rwxrwxrwx   0 root         (0) root         (0)    39414 2023-03-20 23:41:44.000000 roof-mask-0.5.4/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rwxrwxrwx   0 root         (0) root         (0)     3128 2023-03-20 23:41:45.000000 roof-mask-0.5.4/detectron2/data/datasets/pascal_voc.py
+-rwxrwxrwx   0 root         (0) root         (0)      169 2023-03-20 23:41:45.000000 roof-mask-0.5.4/detectron2/data/datasets/register_coco.py
+-rwxrwxrwx   0 root         (0) root         (0)    22841 2023-03-20 23:41:46.000000 roof-mask-0.5.4/detectron2/data/detection_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.333068 roof-mask-0.5.4/detectron2/data/samplers/
+-rwxrwxrwx   0 root         (0) root         (0)      412 2023-03-20 23:41:47.000000 roof-mask-0.5.4/detectron2/data/samplers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11789 2023-03-20 23:41:47.000000 roof-mask-0.5.4/detectron2/data/samplers/distributed_sampler.py
+-rwxrwxrwx   0 root         (0) root         (0)     1944 2023-03-20 23:41:47.000000 roof-mask-0.5.4/detectron2/data/samplers/grouped_batch_sampler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.391035 roof-mask-0.5.4/detectron2/data/transforms/
+-rwxrwxrwx   0 root         (0) root         (0)      466 2023-03-20 23:41:46.000000 roof-mask-0.5.4/detectron2/data/transforms/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14117 2023-03-20 23:41:46.000000 roof-mask-0.5.4/detectron2/data/transforms/augmentation.py
+-rwxrwxrwx   0 root         (0) root         (0)    23069 2023-03-20 23:41:46.000000 roof-mask-0.5.4/detectron2/data/transforms/augmentation_impl.py
+-rwxrwxrwx   0 root         (0) root         (0)    12629 2023-03-20 23:41:46.000000 roof-mask-0.5.4/detectron2/data/transforms/transform.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.472988 roof-mask-0.5.4/detectron2/engine/
+-rwxrwxrwx   0 root         (0) root         (0)      340 2023-03-20 23:41:47.000000 roof-mask-0.5.4/detectron2/engine/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26868 2023-03-20 23:41:47.000000 roof-mask-0.5.4/detectron2/engine/defaults.py
+-rwxrwxrwx   0 root         (0) root         (0)    25497 2023-03-20 23:41:48.000000 roof-mask-0.5.4/detectron2/engine/hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     4089 2023-03-20 23:41:47.000000 roof-mask-0.5.4/detectron2/engine/launch.py
+-rwxrwxrwx   0 root         (0) root         (0)    14104 2023-03-20 23:41:47.000000 roof-mask-0.5.4/detectron2/engine/train_loop.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.528955 roof-mask-0.5.4/detectron2/evaluation/
+-rwxrwxrwx   0 root         (0) root         (0)      671 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8369 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/cityscapes_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    30423 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8156 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/evaluator.py
+-rwxrwxrwx   0 root         (0) root         (0)     5078 2023-03-20 23:41:55.000000 roof-mask-0.5.4/detectron2/evaluation/fast_eval_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    15018 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/lvis_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7500 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/panoptic_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)    10862 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/pascal_voc_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     7608 2023-03-20 23:41:55.000000 roof-mask-0.5.4/detectron2/evaluation/rotated_coco_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     8191 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/sem_seg_evaluation.py
+-rwxrwxrwx   0 root         (0) root         (0)     2614 2023-03-20 23:41:54.000000 roof-mask-0.5.4/detectron2/evaluation/testing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.595917 roof-mask-0.5.4/detectron2/export/
+-rwxrwxrwx   0 root         (0) root         (0)      336 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9280 2023-03-20 23:41:51.000000 roof-mask-0.5.4/detectron2/export/api.py
+-rwxrwxrwx   0 root         (0) root         (0)    21035 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/c10.py
+-rwxrwxrwx   0 root         (0) root         (0)     7803 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/caffe2_export.py
+-rwxrwxrwx   0 root         (0) root         (0)     6674 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/caffe2_inference.py
+-rwxrwxrwx   0 root         (0) root         (0)    17034 2023-03-20 23:41:51.000000 roof-mask-0.5.4/detectron2/export/caffe2_modeling.py
+-rwxrwxrwx   0 root         (0) root         (0)     5033 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/caffe2_patch.py
+-rwxrwxrwx   0 root         (0) root         (0)    11807 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/flatten.py
+-rwxrwxrwx   0 root         (0) root         (0)    38071 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/shared.py
+-rwxrwxrwx   0 root         (0) root         (0)     5008 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/torchscript.py
+-rwxrwxrwx   0 root         (0) root         (0)    11526 2023-03-20 23:41:52.000000 roof-mask-0.5.4/detectron2/export/torchscript_patch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.675871 roof-mask-0.5.4/detectron2/layers/
+-rwxrwxrwx   0 root         (0) root         (0)      839 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5764 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/aspp.py
+-rwxrwxrwx   0 root         (0) root         (0)    12131 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/batch_norm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3024 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/blocks.py
+-rwxrwxrwx   0 root         (0) root         (0)    16978 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/deform_conv.py
+-rwxrwxrwx   0 root         (0) root         (0)     4204 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/losses.py
+-rwxrwxrwx   0 root         (0) root         (0)    10881 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/mask_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     6490 2023-03-20 23:41:38.000000 roof-mask-0.5.4/detectron2/layers/nms.py
+-rwxrwxrwx   0 root         (0) root         (0)     3098 2023-03-20 23:41:33.000000 roof-mask-0.5.4/detectron2/layers/roi_align.py
+-rwxrwxrwx   0 root         (0) root         (0)     3302 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/roi_align_rotated.py
+-rwxrwxrwx   0 root         (0) root         (0)      652 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/rotated_boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-03-20 23:41:38.000000 roof-mask-0.5.4/detectron2/layers/shape_spec.py
+-rwxrwxrwx   0 root         (0) root         (0)     4893 2023-03-20 23:41:37.000000 roof-mask-0.5.4/detectron2/layers/wrappers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.794803 roof-mask-0.5.4/detectron2/modeling/
+-rwxrwxrwx   0 root         (0) root         (0)     1475 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15443 2023-03-20 23:41:43.000000 roof-mask-0.5.4/detectron2/modeling/anchor_generator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.869760 roof-mask-0.5.4/detectron2/modeling/backbone/
+-rwxrwxrwx   0 root         (0) root         (0)      475 2023-03-20 23:41:39.000000 roof-mask-0.5.4/detectron2/modeling/backbone/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1543 2023-03-20 23:41:39.000000 roof-mask-0.5.4/detectron2/modeling/backbone/backbone.py
+-rwxrwxrwx   0 root         (0) root         (0)     1015 2023-03-20 23:41:39.000000 roof-mask-0.5.4/detectron2/modeling/backbone/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    10055 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/backbone/fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    16656 2023-03-20 23:41:39.000000 roof-mask-0.5.4/detectron2/modeling/backbone/regnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    23658 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/backbone/resnet.py
+-rwxrwxrwx   0 root         (0) root         (0)    15123 2023-03-20 23:41:43.000000 roof-mask-0.5.4/detectron2/modeling/box_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     6264 2023-03-20 23:41:39.000000 roof-mask-0.5.4/detectron2/modeling/matcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:18.943717 roof-mask-0.5.4/detectron2/modeling/meta_arch/
+-rwxrwxrwx   0 root         (0) root         (0)      508 2023-03-20 23:41:41.000000 roof-mask-0.5.4/detectron2/modeling/meta_arch/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      814 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/meta_arch/build.py
+-rwxrwxrwx   0 root         (0) root         (0)    11550 2023-03-20 23:41:41.000000 roof-mask-0.5.4/detectron2/modeling/meta_arch/dense_detector.py
+-rwxrwxrwx   0 root         (0) root         (0)    13213 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/meta_arch/fcos.py
+-rwxrwxrwx   0 root         (0) root         (0)    10335 2023-03-20 23:41:41.000000 roof-mask-0.5.4/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rwxrwxrwx   0 root         (0) root         (0)    13710 2023-03-20 23:41:41.000000 roof-mask-0.5.4/detectron2/modeling/meta_arch/rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    18265 2023-03-20 23:41:41.000000 roof-mask-0.5.4/detectron2/modeling/meta_arch/retinanet.py
+-rwxrwxrwx   0 root         (0) root         (0)     9720 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/meta_arch/semantic_seg.py
+-rwxrwxrwx   0 root         (0) root         (0)    10832 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/mmdet_wrapper.py
+-rwxrwxrwx   0 root         (0) root         (0)    11316 2023-03-20 23:41:43.000000 roof-mask-0.5.4/detectron2/modeling/poolers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4046 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/postprocessing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.038664 roof-mask-0.5.4/detectron2/modeling/proposal_generator/
+-rwxrwxrwx   0 root         (0) root         (0)      231 2023-03-20 23:41:41.000000 roof-mask-0.5.4/detectron2/modeling/proposal_generator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      836 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/proposal_generator/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8128 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/proposal_generator/proposal_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    23814 2023-03-20 23:41:41.000000 roof-mask-0.5.4/detectron2/modeling/proposal_generator/rpn.py
+-rwxrwxrwx   0 root         (0) root         (0)     8807 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/proposal_generator/rrpn.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.121616 roof-mask-0.5.4/detectron2/modeling/roi_heads/
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/roi_heads/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4077 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/roi_heads/box_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12990 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    25274 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/roi_heads/fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)    11156 2023-03-20 23:41:43.000000 roof-mask-0.5.4/detectron2/modeling/roi_heads/keypoint_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    12169 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/roi_heads/mask_head.py
+-rwxrwxrwx   0 root         (0) root         (0)    37701 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/roi_heads/roi_heads.py
+-rwxrwxrwx   0 root         (0) root         (0)    11158 2023-03-20 23:41:42.000000 roof-mask-0.5.4/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rwxrwxrwx   0 root         (0) root         (0)     2334 2023-03-20 23:41:40.000000 roof-mask-0.5.4/detectron2/modeling/sampling.py
+-rwxrwxrwx   0 root         (0) root         (0)    12416 2023-03-20 23:41:41.000000 roof-mask-0.5.4/detectron2/modeling/test_time_augmentation.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.195573 roof-mask-0.5.4/detectron2/solver/
+-rwxrwxrwx   0 root         (0) root         (0)      298 2023-03-20 23:41:55.000000 roof-mask-0.5.4/detectron2/solver/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11127 2023-03-20 23:41:55.000000 roof-mask-0.5.4/detectron2/solver/build.py
+-rwxrwxrwx   0 root         (0) root         (0)     8648 2023-03-20 23:41:55.000000 roof-mask-0.5.4/detectron2/solver/lr_scheduler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.276527 roof-mask-0.5.4/detectron2/structures/
+-rwxrwxrwx   0 root         (0) root         (0)      645 2023-03-20 23:41:51.000000 roof-mask-0.5.4/detectron2/structures/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14429 2023-03-20 23:41:51.000000 roof-mask-0.5.4/detectron2/structures/boxes.py
+-rwxrwxrwx   0 root         (0) root         (0)     4557 2023-03-20 23:41:51.000000 roof-mask-0.5.4/detectron2/structures/image_list.py
+-rwxrwxrwx   0 root         (0) root         (0)     6542 2023-03-20 23:41:51.000000 roof-mask-0.5.4/detectron2/structures/instances.py
+-rwxrwxrwx   0 root         (0) root         (0)     9030 2023-03-20 23:41:51.000000 roof-mask-0.5.4/detectron2/structures/keypoints.py
+-rwxrwxrwx   0 root         (0) root         (0)    19802 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/structures/masks.py
+-rwxrwxrwx   0 root         (0) root         (0)    18853 2023-03-20 23:41:51.000000 roof-mask-0.5.4/detectron2/structures/rotated_boxes.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.334494 roof-mask-0.5.4/detectron2/tracking/
+-rwxrwxrwx   0 root         (0) root         (0)      580 2023-03-20 23:41:53.000000 roof-mask-0.5.4/detectron2/tracking/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2216 2023-03-20 23:41:53.000000 roof-mask-0.5.4/detectron2/tracking/base_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)    11858 2023-03-20 23:41:53.000000 roof-mask-0.5.4/detectron2/tracking/bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     7486 2023-03-20 23:41:53.000000 roof-mask-0.5.4/detectron2/tracking/hungarian_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     4142 2023-03-20 23:41:53.000000 roof-mask-0.5.4/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)     1106 2023-03-20 23:41:53.000000 roof-mask-0.5.4/detectron2/tracking/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     5288 2023-03-20 23:41:53.000000 roof-mask-0.5.4/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.430438 roof-mask-0.5.4/detectron2/utils/
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6017 2023-03-20 23:41:49.000000 roof-mask-0.5.4/detectron2/utils/analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)     8391 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/utils/collect_env.py
+-rwxrwxrwx   0 root         (0) root         (0)     4096 2023-03-20 23:41:49.000000 roof-mask-0.5.4/detectron2/utils/colormap.py
+-rwxrwxrwx   0 root         (0) root         (0)     5610 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/utils/comm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1838 2023-03-20 23:41:49.000000 roof-mask-0.5.4/detectron2/utils/develop.py
+-rwxrwxrwx   0 root         (0) root         (0)     5644 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/utils/env.py
+-rwxrwxrwx   0 root         (0) root         (0)    17024 2023-03-20 23:41:49.000000 roof-mask-0.5.4/detectron2/utils/events.py
+-rwxrwxrwx   0 root         (0) root         (0)     1189 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/utils/file_io.py
+-rwxrwxrwx   0 root         (0) root         (0)     7807 2023-03-20 23:41:49.000000 roof-mask-0.5.4/detectron2/utils/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2583 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/utils/memory.py
+-rwxrwxrwx   0 root         (0) root         (0)     1874 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/utils/registry.py
+-rwxrwxrwx   0 root         (0) root         (0)     1064 2023-03-20 23:41:48.000000 roof-mask-0.5.4/detectron2/utils/serialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     4833 2023-03-20 23:41:49.000000 roof-mask-0.5.4/detectron2/utils/testing.py
+-rwxrwxrwx   0 root         (0) root         (0)    11319 2023-03-20 23:41:49.000000 roof-mask-0.5.4/detectron2/utils/video_visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    51159 2023-03-20 23:41:50.000000 roof-mask-0.5.4/detectron2/utils/visualizer.py
+-rwxrwxrwx   0 root         (0) root         (0)    52915 2023-03-20 23:41:49.000000 roof-mask-0.5.4/detectron2/utils/visualizer_new.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.536378 roof-mask-0.5.4/models/
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-03-20 23:41:58.000000 roof-mask-0.5.4/models/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    41260 2023-03-20 23:41:58.000000 roof-mask-0.5.4/models/common.py
+-rwxrwxrwx   0 root         (0) root         (0)     4319 2023-03-20 23:41:58.000000 roof-mask-0.5.4/models/experimental.py
+-rwxrwxrwx   0 root         (0) root         (0)    25494 2023-03-20 23:41:57.000000 roof-mask-0.5.4/models/tf.py
+-rwxrwxrwx   0 root         (0) root         (0)    22240 2023-03-20 23:41:58.000000 roof-mask-0.5.4/models/yolo.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.599341 roof-mask-0.5.4/roof_mask.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      548 2023-04-11 18:20:00.000000 roof-mask-0.5.4/roof_mask.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6263 2023-04-11 18:20:01.000000 roof-mask-0.5.4/roof_mask.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-11 18:20:00.000000 roof-mask-0.5.4/roof_mask.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       44 2023-04-11 18:20:00.000000 roof-mask-0.5.4/roof_mask.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.725269 roof-mask-0.5.4/roof_test/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 23:42:00.000000 roof-mask-0.5.4/roof_test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-04-10 17:56:52.000000 roof-mask-0.5.4/roof_test/a.py
+-rwxrwxrwx   0 root         (0) root         (0)      191 2023-03-20 23:42:00.000000 roof-mask-0.5.4/roof_test/predict.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-11 18:20:32.143027 roof-mask-0.5.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      724 2023-04-11 18:07:42.000000 roof-mask-0.5.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.898170 roof-mask-0.5.4/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     2629 2023-04-11 16:30:17.000000 roof-mask-0.5.4/tests/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:19.987119 roof-mask-0.5.4/utils/
+-rwxrwxrwx   0 root         (0) root         (0)     1842 2023-03-20 23:42:04.000000 roof-mask-0.5.4/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3449 2023-03-20 23:42:02.000000 roof-mask-0.5.4/utils/activations.py
+-rwxrwxrwx   0 root         (0) root         (0)    14782 2023-03-20 23:42:03.000000 roof-mask-0.5.4/utils/augmentations.py
+-rwxrwxrwx   0 root         (0) root         (0)     7411 2023-03-20 23:42:03.000000 roof-mask-0.5.4/utils/autoanchor.py
+-rwxrwxrwx   0 root         (0) root         (0)     2767 2023-03-20 23:42:04.000000 roof-mask-0.5.4/utils/autobatch.py
+-rwxrwxrwx   0 root         (0) root         (0)     6958 2023-03-20 23:42:00.000000 roof-mask-0.5.4/utils/benchmarks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2661 2023-03-20 23:42:03.000000 roof-mask-0.5.4/utils/callbacks.py
+-rwxrwxrwx   0 root         (0) root         (0)    51717 2023-03-20 23:42:02.000000 roof-mask-0.5.4/utils/dataloaders.py
+-rwxrwxrwx   0 root         (0) root         (0)     7329 2023-03-20 23:42:03.000000 roof-mask-0.5.4/utils/downloads.py
+-rwxrwxrwx   0 root         (0) root         (0)    48476 2023-03-20 23:42:02.000000 roof-mask-0.5.4/utils/general.py
+-rwxrwxrwx   0 root         (0) root         (0)     9919 2023-03-20 23:42:03.000000 roof-mask-0.5.4/utils/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)    14706 2023-03-20 23:42:02.000000 roof-mask-0.5.4/utils/metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)    22815 2023-03-20 23:42:04.000000 roof-mask-0.5.4/utils/plots.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:20.113047 roof-mask-0.5.4/utils/segment/
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-03-20 23:42:02.000000 roof-mask-0.5.4/utils/segment/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3756 2023-03-20 23:42:01.000000 roof-mask-0.5.4/utils/segment/augmentations.py
+-rwxrwxrwx   0 root         (0) root         (0)    13499 2023-03-20 23:42:02.000000 roof-mask-0.5.4/utils/segment/dataloaders.py
+-rwxrwxrwx   0 root         (0) root         (0)     4480 2023-03-20 23:42:01.000000 roof-mask-0.5.4/utils/segment/general.py
+-rwxrwxrwx   0 root         (0) root         (0)     8632 2023-03-20 23:42:00.000000 roof-mask-0.5.4/utils/segment/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)     5457 2023-03-20 23:42:02.000000 roof-mask-0.5.4/utils/segment/metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)     7859 2023-03-20 23:42:00.000000 roof-mask-0.5.4/utils/segment/plots.py
+-rwxrwxrwx   0 root         (0) root         (0)    19970 2023-03-20 23:42:03.000000 roof-mask-0.5.4/utils/torch_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-11 18:15:20.169015 roof-mask-0.5.4/yolo_roof/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-03-20 23:42:04.000000 roof-mask-0.5.4/yolo_roof/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    27812 2023-04-10 20:09:08.000000 roof-mask-0.5.4/yolo_roof/detect_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    28494 2023-03-20 23:42:05.000000 roof-mask-0.5.4/yolo_roof/export.py
+-rwxrwxrwx   0 root         (0) root         (0)    21398 2023-04-11 16:34:46.000000 roof-mask-0.5.4/yolo_roof/geo_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)    33193 2023-03-23 16:17:29.000000 roof-mask-0.5.4/yolo_roof/report_functions.py
```

### Comparing `roof_mask-0.5.3/PKG-INFO` & `roof-mask-0.5.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
-Name: roof_mask
-Version: 0.5.3
+Name: roof-mask
+Version: 0.5.4
 Summary: upload pip package test
 Home-page: https://github.com/lrxjason/roof_model_test/
 Author: Ruixu
 Author-email: lrxjason@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 v0.5.3: backend errors (coded as 11, 21, 31, and 41) from image vender and geo-coding vender are raised as exceptions and passed back to the caller.
+ v0.5.4: minor bugfix.
```

### Comparing `roof_mask-0.5.3/detectron2/checkpoint/catalog.py` & `roof-mask-0.5.4/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/checkpoint/detection_checkpoint.py` & `roof-mask-0.5.4/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/config/__init__.py` & `roof-mask-0.5.4/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/config/compat.py` & `roof-mask-0.5.4/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/config/config.py` & `roof-mask-0.5.4/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/config/defaults.py` & `roof-mask-0.5.4/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/config/instantiate.py` & `roof-mask-0.5.4/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/config/lazy.py` & `roof-mask-0.5.4/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/__init__.py` & `roof-mask-0.5.4/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/benchmark.py` & `roof-mask-0.5.4/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/build.py` & `roof-mask-0.5.4/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/catalog.py` & `roof-mask-0.5.4/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/common.py` & `roof-mask-0.5.4/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/dataset_mapper.py` & `roof-mask-0.5.4/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/__init__.py` & `roof-mask-0.5.4/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/builtin.py` & `roof-mask-0.5.4/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/builtin_meta.py` & `roof-mask-0.5.4/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/cityscapes.py` & `roof-mask-0.5.4/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/cityscapes_panoptic.py` & `roof-mask-0.5.4/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/coco.py` & `roof-mask-0.5.4/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/coco_panoptic.py` & `roof-mask-0.5.4/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/lvis.py` & `roof-mask-0.5.4/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/lvis_v0_5_categories.py` & `roof-mask-0.5.4/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/lvis_v1_categories.py` & `roof-mask-0.5.4/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/lvis_v1_category_image_count.py` & `roof-mask-0.5.4/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/datasets/pascal_voc.py` & `roof-mask-0.5.4/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/detection_utils.py` & `roof-mask-0.5.4/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/samplers/distributed_sampler.py` & `roof-mask-0.5.4/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/samplers/grouped_batch_sampler.py` & `roof-mask-0.5.4/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/transforms/augmentation.py` & `roof-mask-0.5.4/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/transforms/augmentation_impl.py` & `roof-mask-0.5.4/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/data/transforms/transform.py` & `roof-mask-0.5.4/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/engine/defaults.py` & `roof-mask-0.5.4/detectron2/engine/defaults.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/engine/hooks.py` & `roof-mask-0.5.4/detectron2/engine/hooks.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/engine/launch.py` & `roof-mask-0.5.4/detectron2/engine/launch.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/engine/train_loop.py` & `roof-mask-0.5.4/detectron2/engine/train_loop.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/__init__.py` & `roof-mask-0.5.4/detectron2/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/cityscapes_evaluation.py` & `roof-mask-0.5.4/detectron2/evaluation/cityscapes_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/coco_evaluation.py` & `roof-mask-0.5.4/detectron2/evaluation/coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/evaluator.py` & `roof-mask-0.5.4/detectron2/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/fast_eval_api.py` & `roof-mask-0.5.4/detectron2/evaluation/fast_eval_api.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/lvis_evaluation.py` & `roof-mask-0.5.4/detectron2/evaluation/lvis_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/panoptic_evaluation.py` & `roof-mask-0.5.4/detectron2/evaluation/panoptic_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/pascal_voc_evaluation.py` & `roof-mask-0.5.4/detectron2/evaluation/pascal_voc_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/rotated_coco_evaluation.py` & `roof-mask-0.5.4/detectron2/evaluation/rotated_coco_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/sem_seg_evaluation.py` & `roof-mask-0.5.4/detectron2/evaluation/sem_seg_evaluation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/evaluation/testing.py` & `roof-mask-0.5.4/detectron2/evaluation/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/api.py` & `roof-mask-0.5.4/detectron2/export/api.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/c10.py` & `roof-mask-0.5.4/detectron2/export/c10.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/caffe2_export.py` & `roof-mask-0.5.4/detectron2/export/caffe2_export.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/caffe2_inference.py` & `roof-mask-0.5.4/detectron2/export/caffe2_inference.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/caffe2_modeling.py` & `roof-mask-0.5.4/detectron2/export/caffe2_modeling.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/caffe2_patch.py` & `roof-mask-0.5.4/detectron2/export/caffe2_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/flatten.py` & `roof-mask-0.5.4/detectron2/export/flatten.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/shared.py` & `roof-mask-0.5.4/detectron2/export/shared.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/torchscript.py` & `roof-mask-0.5.4/detectron2/export/torchscript.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/export/torchscript_patch.py` & `roof-mask-0.5.4/detectron2/export/torchscript_patch.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/__init__.py` & `roof-mask-0.5.4/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/aspp.py` & `roof-mask-0.5.4/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/batch_norm.py` & `roof-mask-0.5.4/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/blocks.py` & `roof-mask-0.5.4/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/deform_conv.py` & `roof-mask-0.5.4/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/losses.py` & `roof-mask-0.5.4/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/mask_ops.py` & `roof-mask-0.5.4/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/nms.py` & `roof-mask-0.5.4/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/roi_align.py` & `roof-mask-0.5.4/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/roi_align_rotated.py` & `roof-mask-0.5.4/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/rotated_boxes.py` & `roof-mask-0.5.4/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/shape_spec.py` & `roof-mask-0.5.4/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/layers/wrappers.py` & `roof-mask-0.5.4/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/__init__.py` & `roof-mask-0.5.4/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/anchor_generator.py` & `roof-mask-0.5.4/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/backbone/backbone.py` & `roof-mask-0.5.4/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/backbone/build.py` & `roof-mask-0.5.4/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/backbone/fpn.py` & `roof-mask-0.5.4/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/backbone/regnet.py` & `roof-mask-0.5.4/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/backbone/resnet.py` & `roof-mask-0.5.4/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/box_regression.py` & `roof-mask-0.5.4/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/matcher.py` & `roof-mask-0.5.4/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/meta_arch/build.py` & `roof-mask-0.5.4/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/meta_arch/dense_detector.py` & `roof-mask-0.5.4/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/meta_arch/fcos.py` & `roof-mask-0.5.4/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/meta_arch/panoptic_fpn.py` & `roof-mask-0.5.4/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/meta_arch/rcnn.py` & `roof-mask-0.5.4/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/meta_arch/retinanet.py` & `roof-mask-0.5.4/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/meta_arch/semantic_seg.py` & `roof-mask-0.5.4/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/mmdet_wrapper.py` & `roof-mask-0.5.4/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/poolers.py` & `roof-mask-0.5.4/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/postprocessing.py` & `roof-mask-0.5.4/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/proposal_generator/build.py` & `roof-mask-0.5.4/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/proposal_generator/proposal_utils.py` & `roof-mask-0.5.4/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/proposal_generator/rpn.py` & `roof-mask-0.5.4/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/proposal_generator/rrpn.py` & `roof-mask-0.5.4/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/roi_heads/__init__.py` & `roof-mask-0.5.4/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/roi_heads/box_head.py` & `roof-mask-0.5.4/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/roi_heads/cascade_rcnn.py` & `roof-mask-0.5.4/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/roi_heads/fast_rcnn.py` & `roof-mask-0.5.4/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/roi_heads/keypoint_head.py` & `roof-mask-0.5.4/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/roi_heads/mask_head.py` & `roof-mask-0.5.4/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/roi_heads/roi_heads.py` & `roof-mask-0.5.4/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `roof-mask-0.5.4/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/sampling.py` & `roof-mask-0.5.4/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/modeling/test_time_augmentation.py` & `roof-mask-0.5.4/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/solver/build.py` & `roof-mask-0.5.4/detectron2/solver/build.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/solver/lr_scheduler.py` & `roof-mask-0.5.4/detectron2/solver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/structures/__init__.py` & `roof-mask-0.5.4/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/structures/boxes.py` & `roof-mask-0.5.4/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/structures/image_list.py` & `roof-mask-0.5.4/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/structures/instances.py` & `roof-mask-0.5.4/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/structures/keypoints.py` & `roof-mask-0.5.4/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/structures/masks.py` & `roof-mask-0.5.4/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/structures/rotated_boxes.py` & `roof-mask-0.5.4/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/tracking/__init__.py` & `roof-mask-0.5.4/detectron2/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/tracking/base_tracker.py` & `roof-mask-0.5.4/detectron2/tracking/base_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/tracking/bbox_iou_tracker.py` & `roof-mask-0.5.4/detectron2/tracking/bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/tracking/hungarian_tracker.py` & `roof-mask-0.5.4/detectron2/tracking/hungarian_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py` & `roof-mask-0.5.4/detectron2/tracking/iou_weighted_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/tracking/utils.py` & `roof-mask-0.5.4/detectron2/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py` & `roof-mask-0.5.4/detectron2/tracking/vanilla_hungarian_bbox_iou_tracker.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/analysis.py` & `roof-mask-0.5.4/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/collect_env.py` & `roof-mask-0.5.4/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/colormap.py` & `roof-mask-0.5.4/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/comm.py` & `roof-mask-0.5.4/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/develop.py` & `roof-mask-0.5.4/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/env.py` & `roof-mask-0.5.4/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/events.py` & `roof-mask-0.5.4/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/file_io.py` & `roof-mask-0.5.4/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/logger.py` & `roof-mask-0.5.4/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/memory.py` & `roof-mask-0.5.4/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/registry.py` & `roof-mask-0.5.4/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/serialize.py` & `roof-mask-0.5.4/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/testing.py` & `roof-mask-0.5.4/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/video_visualizer.py` & `roof-mask-0.5.4/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/visualizer.py` & `roof-mask-0.5.4/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/detectron2/utils/visualizer_new.py` & `roof-mask-0.5.4/detectron2/utils/visualizer_new.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/models/common.py` & `roof-mask-0.5.4/models/common.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/models/experimental.py` & `roof-mask-0.5.4/models/experimental.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/models/tf.py` & `roof-mask-0.5.4/models/tf.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/models/yolo.py` & `roof-mask-0.5.4/models/yolo.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/roof_mask.egg-info/PKG-INFO` & `roof-mask-0.5.4/roof_mask.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: roof-mask
-Version: 0.5.3
+Version: 0.5.4
 Summary: upload pip package test
 Home-page: https://github.com/lrxjason/roof_model_test/
 Author: Ruixu
 Author-email: lrxjason@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 v0.5.3: backend errors (coded as 11, 21, 31, and 41) from image vender and geo-coding vender are raised as exceptions and passed back to the caller.
+ v0.5.4: minor bugfix.
```

### Comparing `roof_mask-0.5.3/roof_mask.egg-info/SOURCES.txt` & `roof-mask-0.5.4/roof_mask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/setup.py` & `roof-mask-0.5.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ## test upload
 import setuptools
 
 setuptools.setup(
-    name = "roof_mask",
-    version = "0.5.3",
+    name = "roof-mask",
+    version = "0.5.4",
     author = "Ruixu",
     author_email = "lrxjason@gmail.com",
     description = "upload pip package test",
-    long_description = 'v0.5.3: backend errors (coded as 11, 21, 31, and 41) from image vender and geo-coding vender are raised as exceptions and passed back to the caller.',
+    long_description = 'v0.5.3: backend errors (coded as 11, 21, 31, and 41) from image vender and geo-coding vender are raised as exceptions and passed back to the caller.\n v0.5.4: minor bugfix.',
     long_description_content_type="text/markdown",
     url="https://github.com/lrxjason/roof_model_test/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `roof_mask-0.5.3/tests/test.py` & `roof-mask-0.5.4/tests/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,41 +27,41 @@
 yolo_damage_model = load_yolo_model("./best_damage.pt")
 yolo_equipment_model = load_yolo_model("./best_equipment.pt")
 
 #address="2232 Isle Royale Ln, Davis, CA 95616"
 addresses_generic = [
     # generic testcases
     #"2232 Isle Royale Ln, Davis, CA 95616",
-    #"1 E SIDE SQ, MACOMB, IL 61455-2213", 
     #"1 HEATHER HL, BOURBONNAIS, IL 60914-1622",
     #"1 INDIANA SQ STE 1200, INDIANAPOLIS, IN 46204-2066",
-    #"1 OAKBROOK CTR SPC 217, OAK BROOK, IL 60523-1809",
     #"1 S HARRISON ST, ASHLEY, OH 43003-7518",
     #"1 S WACKER DR STE 3250B, CHICAGO, IL 60606-4639",
     #"1 TOWNE SQ STE 800, SOUTHFIELD, MI 48076-3723",
     #"1 VIRGINIA AVE, INDIANAPOLIS, IN 46204-3644",
-    #"1 WOODCREST DR, HIGHLAND, IL 62249",
-    #"10 E 375 N, REYNOLDS, IN 47980-8025",
-    "10 N 3RD ST, LAFAYETTE, IN 47901-1296",
-    "10 N MARTINGALE RD STE 400, SCHAUMBURG, IL 60173-2411",
-    "100 MAPLE PARK BLVD, SAINT CLAIR SHORES, MI 48081-2200",
-    "100 N CHESTNUT ST, CHAMPAIGN, IL 61820-4856",
+    #"10 N 3RD ST, LAFAYETTE, IN 47901-1296",
+    #"10 N MARTINGALE RD STE 400, SCHAUMBURG, IL 60173-2411",
+    #"100 MAPLE PARK BLVD, SAINT CLAIR SHORES, MI 48081-2200",
+    #"100 N CHESTNUT ST, CHAMPAIGN, IL 61820-4856",
 ]
 
 addresses_special = [
     # special testcases
     "6200 South Gilmore Rd, Fairfield, OH",
     "1 Apple Park Way, Cupertino, CA 95014",
     "66 Bluff Ct Trout Valley, IL 60013"
+    "1 E SIDE SQ, MACOMB, IL 61455-2213", 
+    "1 OAKBROOK CTR SPC 217, OAK BROOK, IL 60523-1809",
+    "1 WOODCREST DR, HIGHLAND, IL 62249",
+    "10 E 375 N, REYNOLDS, IN 47980-8025",
 ]
 
 business_name="My home"
 email="qiang_wang@cinfin.com"
 
-for address in addresses_generic:
+for address in addresses_special:
     try:
         image_download(address, business_name, "./")
         roof_predict(yolo_roof_model, yolo_damage_model, yolo_equipment_model, "./")
         generate_report("./")
     except Exception as inst:
         backend_tester.error(f"{address} failed: {inst}")
     else:
```

### Comparing `roof_mask-0.5.3/utils/__init__.py` & `roof-mask-0.5.4/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/activations.py` & `roof-mask-0.5.4/utils/activations.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/augmentations.py` & `roof-mask-0.5.4/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/autoanchor.py` & `roof-mask-0.5.4/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/autobatch.py` & `roof-mask-0.5.4/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/benchmarks.py` & `roof-mask-0.5.4/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/callbacks.py` & `roof-mask-0.5.4/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/dataloaders.py` & `roof-mask-0.5.4/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/downloads.py` & `roof-mask-0.5.4/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/general.py` & `roof-mask-0.5.4/utils/general.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/loss.py` & `roof-mask-0.5.4/utils/loss.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/metrics.py` & `roof-mask-0.5.4/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/plots.py` & `roof-mask-0.5.4/utils/plots.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/segment/augmentations.py` & `roof-mask-0.5.4/utils/segment/augmentations.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/segment/dataloaders.py` & `roof-mask-0.5.4/utils/segment/dataloaders.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/segment/general.py` & `roof-mask-0.5.4/utils/segment/general.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/segment/loss.py` & `roof-mask-0.5.4/utils/segment/loss.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/segment/metrics.py` & `roof-mask-0.5.4/utils/segment/metrics.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/segment/plots.py` & `roof-mask-0.5.4/utils/segment/plots.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/utils/torch_utils.py` & `roof-mask-0.5.4/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/yolo_roof/detect_functions.py` & `roof-mask-0.5.4/yolo_roof/detect_functions.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/yolo_roof/export.py` & `roof-mask-0.5.4/yolo_roof/export.py`

 * *Files identical despite different names*

### Comparing `roof_mask-0.5.3/yolo_roof/geo_functions.py` & `roof-mask-0.5.4/yolo_roof/geo_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,10 +476,10 @@
     # Exception-throwing-catching is a more generic solution than passing the error message via and csv file, and I (qiang_wang)
     # plan to move away from the csv file(s)
     if 'Nearmap image is not available here.' in image_text:
         raise Exception(11, image_text) # 11 is the error code, image_text is the error message 
     elif 'image is too big' in image_text:
         raise Exception(21, image_text)
     elif 'Ecopia Geocoding is not accurate.' in image_text:
-        raise Exception(31)
+        raise Exception(31, image_text)
     elif 'The Ecopia Geocoding is not avaliable.' in image_text:
-        raise Exception(41)
+        raise Exception(41, image_text)
```

### Comparing `roof_mask-0.5.3/yolo_roof/report_functions.py` & `roof-mask-0.5.4/yolo_roof/report_functions.py`

 * *Files identical despite different names*

