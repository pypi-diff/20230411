# Comparing `tmp/hello2-1.5.1.tar.gz` & `tmp/hello2-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello2-1.5.1.tar", last modified: Mon Apr  3 07:55:22 2023, max compression
+gzip compressed data, was "hello2-1.5.2.tar", last modified: Tue Apr 11 07:48:46 2023, max compression
```

## Comparing `hello2-1.5.1.tar` & `hello2-1.5.2.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0      550 2022-11-04 08:45:52.036893 hello2-1.5.1/.gitignore
--rw-r--r--   0        0        0      715 2022-11-04 17:06:29.116576 hello2-1.5.1/.readthedocs.yaml
--rw-r--r--   0        0        0    11357 2022-06-27 01:46:45.026108 hello2-1.5.1/LICENSE
--rw-r--r--   0        0        0      351 2022-12-20 05:58:10.658183 hello2-1.5.1/README.md
--rw-r--r--   0        0        0      638 2022-11-04 13:36:31.980929 hello2-1.5.1/docs/Makefile
--rw-r--r--   0        0        0      804 2022-11-04 13:36:31.980929 hello2-1.5.1/docs/make.bat
--rw-r--r--   0        0        0      163 2022-11-06 11:07:57.505182 hello2-1.5.1/docs/requirements.txt
--rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.5.1/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.5.1/docs/source/_templates/.gitkeep
--rw-r--r--   0        0        0     1365 2022-11-06 12:23:09.043638 hello2-1.5.1/docs/source/conf.py
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.770149 hello2-1.5.1/docs/source/hello.data.coco2yolo.rst
--rw-r--r--   0        0        0      231 2022-11-04 14:14:10.770149 hello2-1.5.1/docs/source/hello.data.rst
--rw-r--r--   0        0        0      187 2022-12-14 01:38:29.403883 hello2-1.5.1/docs/source/hello.experimental.albu.detection.rst
--rw-r--r--   0        0        0      283 2022-12-14 01:38:29.403883 hello2-1.5.1/docs/source/hello.experimental.albu.rst
--rw-r--r--   0        0        0      260 2022-12-14 01:38:29.393883 hello2-1.5.1/docs/source/hello.experimental.rst
--rw-r--r--   0        0        0      148 2022-12-14 09:04:35.414160 hello2-1.5.1/docs/source/hello.fiftyone.brain.rst
--rw-r--r--   0        0        0      160 2022-11-18 12:12:27.461051 hello2-1.5.1/docs/source/hello.fiftyone.copypaste.rst
--rw-r--r--   0        0        0      145 2022-11-04 14:14:10.780149 hello2-1.5.1/docs/source/hello.fiftyone.core.rst
--rw-r--r--   0        0        0      154 2022-11-04 14:14:10.780149 hello2-1.5.1/docs/source/hello.fiftyone.dataset.rst
--rw-r--r--   0        0        0      183 2022-11-04 14:14:10.780149 hello2-1.5.1/docs/source/hello.fiftyone.dataset_annotate.rst
--rw-r--r--   0        0        0      189 2022-11-04 14:14:10.780149 hello2-1.5.1/docs/source/hello.fiftyone.dataset_detections.rst
--rw-r--r--   0        0        0      198 2022-11-04 14:14:10.790149 hello2-1.5.1/docs/source/hello.fiftyone.dataset_segmentations.rst
--rw-r--r--   0        0        0      177 2022-11-04 14:14:10.790149 hello2-1.5.1/docs/source/hello.fiftyone.dataset_yolov5.rst
--rw-r--r--   0        0        0      168 2022-11-04 14:14:10.790149 hello2-1.5.1/docs/source/hello.fiftyone.dataset_zoo.rst
--rw-r--r--   0        0        0      157 2022-11-04 14:14:10.790149 hello2-1.5.1/docs/source/hello.fiftyone.evaluate.rst
--rw-r--r--   0        0        0      192 2022-11-04 14:14:10.790149 hello2-1.5.1/docs/source/hello.fiftyone.evaluate_detections.rst
--rw-r--r--   0        0        0      201 2022-11-04 14:14:10.790149 hello2-1.5.1/docs/source/hello.fiftyone.evaluate_segmentations.rst
--rw-r--r--   0        0        0      171 2022-11-18 12:12:27.481051 hello2-1.5.1/docs/source/hello.fiftyone.gen_examples.rst
--rw-r--r--   0        0        0      168 2022-11-18 12:12:27.481051 hello2-1.5.1/docs/source/hello.fiftyone.mask_ignore.rst
--rw-r--r--   0        0        0      145 2022-11-04 14:14:10.790149 hello2-1.5.1/docs/source/hello.fiftyone.miou.rst
--rw-r--r--   0        0        0      154 2022-11-18 12:12:27.481051 hello2-1.5.1/docs/source/hello.fiftyone.patches.rst
--rw-r--r--   0        0        0      833 2022-12-16 13:39:47.510383 hello2-1.5.1/docs/source/hello.fiftyone.rst
--rw-r--r--   0        0        0      154 2022-12-16 13:39:47.530383 hello2-1.5.1/docs/source/hello.fiftyone.tarinfo.rst
--rw-r--r--   0        0        0      151 2022-11-04 14:14:10.800149 hello2-1.5.1/docs/source/hello.fiftyone.unique.rst
--rw-r--r--   0        0        0      148 2022-11-22 16:10:13.239568 hello2-1.5.1/docs/source/hello.fiftyone.utils.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.800149 hello2-1.5.1/docs/source/hello.fiftyone.video.rst
--rw-r--r--   0        0        0      145 2022-11-22 16:10:13.239568 hello2-1.5.1/docs/source/hello.fiftyone.view.rst
--rw-r--r--   0        0        0      159 2022-11-04 15:41:25.788323 hello2-1.5.1/docs/source/hello.fvcore.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.800149 hello2-1.5.1/docs/source/hello.io.image.rst
--rw-r--r--   0        0        0      237 2022-11-04 14:14:10.800149 hello2-1.5.1/docs/source/hello.io.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.810149 hello2-1.5.1/docs/source/hello.io.utils.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.810149 hello2-1.5.1/docs/source/hello.mmdet.export.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.810149 hello2-1.5.1/docs/source/hello.mmdet.flop.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.820149 hello2-1.5.1/docs/source/hello.mmdet.infer.rst
--rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.5.1/docs/source/hello.mmdet.log.rst
--rw-r--r--   0        0        0      136 2022-11-25 07:45:47.915124 hello2-1.5.1/docs/source/hello.mmdet.plot.rst
--rw-r--r--   0        0        0      312 2022-11-25 07:45:47.915124 hello2-1.5.1/docs/source/hello.mmdet.rst
--rw-r--r--   0        0        0      139 2022-11-07 02:04:44.756679 hello2-1.5.1/docs/source/hello.mmseg.infer.rst
--rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.5.1/docs/source/hello.mmseg.log.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.820149 hello2-1.5.1/docs/source/hello.mmseg.lr.rst
--rw-r--r--   0        0        0      268 2022-11-07 02:04:44.756679 hello2-1.5.1/docs/source/hello.mmseg.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.830149 hello2-1.5.1/docs/source/hello.onnx.export.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.830149 hello2-1.5.1/docs/source/hello.onnx.infer.rst
--rw-r--r--   0        0        0      248 2022-11-04 14:14:10.830149 hello2-1.5.1/docs/source/hello.onnx.rst
--rw-r--r--   0        0        0      383 2022-12-14 01:38:29.383883 hello2-1.5.1/docs/source/hello.rst
--rw-r--r--   0        0        0      256 2022-11-04 14:14:10.840149 hello2-1.5.1/docs/source/hello.transforms.rst
--rw-r--r--   0        0        0      169 2022-11-04 14:14:10.840149 hello2-1.5.1/docs/source/hello.transforms.transforms.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.5.1/docs/source/hello.utils.colors.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.850149 hello2-1.5.1/docs/source/hello.utils.cuda.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.850149 hello2-1.5.1/docs/source/hello.utils.importer.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.850149 hello2-1.5.1/docs/source/hello.utils.plots.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.5.1/docs/source/hello.utils.points.rst
--rw-r--r--   0        0        0      342 2022-11-30 10:15:09.966399 hello2-1.5.1/docs/source/hello.utils.rst
--rw-r--r--   0        0        0      145 2022-11-30 10:15:09.976399 hello2-1.5.1/docs/source/hello.utils.strtime.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.860149 hello2-1.5.1/docs/source/hello.video.align.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.5.1/docs/source/hello.video.clip.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.5.1/docs/source/hello.video.frames.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.5.1/docs/source/hello.video.info.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.5.1/docs/source/hello.video.resize.rst
--rw-r--r--   0        0        0      424 2022-11-29 06:30:33.921961 hello2-1.5.1/docs/source/hello.video.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.870149 hello2-1.5.1/docs/source/hello.video.rtsp.rst
--rw-r--r--   0        0        0      153 2022-11-29 06:30:33.931961 hello2-1.5.1/docs/source/hello.video.rtsp_pull.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.5.1/docs/source/hello.video.split.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.870149 hello2-1.5.1/docs/source/hello.video.unwarp.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.5.1/docs/source/hello.video.utils.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.880149 hello2-1.5.1/docs/source/hello.x3m.config.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.5.1/docs/source/hello.x3m.preprocess.rst
--rw-r--r--   0        0        0      272 2022-11-04 14:14:10.870149 hello2-1.5.1/docs/source/hello.x3m.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.5.1/docs/source/hello.x3m.transforms.rst
--rw-r--r--   0        0        0      572 2022-11-04 15:19:50.508765 hello2-1.5.1/docs/source/index.rst
--rw-r--r--   0        0        0       52 2022-11-04 14:40:30.829573 hello2-1.5.1/docs/source/modules.rst
--rw-r--r--   0        0        0     3338 2023-02-22 04:02:31.469946 hello2-1.5.1/hello/README.md
--rw-r--r--   0        0        0      754 2023-04-03 07:52:26.586943 hello2-1.5.1/hello/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.1/hello/__main__.py
--rw-r--r--   0        0        0      471 2022-11-06 13:38:11.482015 hello2-1.5.1/hello/data/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.1/hello/data/__main__.py
--rw-r--r--   0        0        0     3426 2022-08-30 01:19:13.615222 hello2-1.5.1/hello/data/coco2yolo.py
--rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.5.1/hello/experimental/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.5.1/hello/experimental/albu/__init__.py
--rw-r--r--   0        0        0      111 2022-12-11 06:23:09.504528 hello2-1.5.1/hello/experimental/albu/detection.py
--rw-r--r--   0        0        0     1047 2022-11-06 13:38:17.442013 hello2-1.5.1/hello/fiftyone/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.1/hello/fiftyone/__main__.py
--rw-r--r--   0        0        0     4781 2023-03-15 05:39:13.846289 hello2-1.5.1/hello/fiftyone/annotate.py
--rw-r--r--   0        0        0     8329 2022-12-14 15:06:12.986153 hello2-1.5.1/hello/fiftyone/brain.py
--rw-r--r--   0        0        0       36 2022-11-18 04:25:30.455378 hello2-1.5.1/hello/fiftyone/copypaste.py
--rw-r--r--   0        0        0    16956 2023-03-30 13:19:40.433939 hello2-1.5.1/hello/fiftyone/core.py
--rw-r--r--   0        0        0    21141 2023-03-15 09:00:27.664680 hello2-1.5.1/hello/fiftyone/dataset.py
--rw-r--r--   0        0        0     7502 2022-12-30 03:41:16.092249 hello2-1.5.1/hello/fiftyone/dataset_detections.py
--rw-r--r--   0        0        0     5693 2022-12-30 03:45:01.362177 hello2-1.5.1/hello/fiftyone/dataset_segmentations.py
--rw-r--r--   0        0        0     1402 2022-11-30 01:50:37.091070 hello2-1.5.1/hello/fiftyone/dataset_yolov5.py
--rw-r--r--   0        0        0      889 2022-12-02 08:54:06.970245 hello2-1.5.1/hello/fiftyone/dataset_zoo.py
--rw-r--r--   0        0        0     1169 2022-07-18 00:56:40.761934 hello2-1.5.1/hello/fiftyone/evaluate.py
--rw-r--r--   0        0        0     5157 2023-03-07 04:04:15.369663 hello2-1.5.1/hello/fiftyone/evaluate_detections.py
--rw-r--r--   0        0        0     4544 2023-03-07 04:04:11.609664 hello2-1.5.1/hello/fiftyone/evaluate_segmentations.py
--rw-r--r--   0        0        0      103 2022-09-19 06:15:49.337504 hello2-1.5.1/hello/fiftyone/examples/README.md
--rw-r--r--   0        0        0     2975 2022-11-30 01:46:25.831120 hello2-1.5.1/hello/fiftyone/examples/examples.py
--rw-r--r--   0        0        0    12021 2023-01-09 09:33:51.046594 hello2-1.5.1/hello/fiftyone/examples/utils.py
--rw-r--r--   0        0        0     2133 2022-11-16 04:13:14.052375 hello2-1.5.1/hello/fiftyone/gen_examples.py
--rw-r--r--   0        0        0     1608 2022-11-18 03:16:41.036018 hello2-1.5.1/hello/fiftyone/mask_ignore.py
--rw-r--r--   0        0        0     5683 2022-12-30 03:42:18.702230 hello2-1.5.1/hello/fiftyone/miou.py
--rw-r--r--   0        0        0     2639 2022-11-18 06:29:39.594231 hello2-1.5.1/hello/fiftyone/patches.py
--rw-r--r--   0        0        0     7934 2023-03-22 02:58:26.970148 hello2-1.5.1/hello/fiftyone/tarinfo.py
--rw-r--r--   0        0        0     4094 2023-03-15 08:42:32.674825 hello2-1.5.1/hello/fiftyone/unique.py
--rw-r--r--   0        0        0     7621 2023-01-09 04:04:27.118496 hello2-1.5.1/hello/fiftyone/utils.py
--rw-r--r--   0        0        0      781 2022-12-01 14:14:43.560707 hello2-1.5.1/hello/fiftyone/video.py
--rw-r--r--   0        0        0     8010 2023-04-03 07:48:18.837028 hello2-1.5.1/hello/fiftyone/view.py
--rw-r--r--   0        0        0      435 2022-10-20 14:18:34.575285 hello2-1.5.1/hello/fvcore/README.md
--rw-r--r--   0        0        0        0 2022-11-04 14:49:06.729395 hello2-1.5.1/hello/fvcore/__init__.py
--rw-r--r--   0        0        0      135 2022-06-27 01:46:45.026108 hello2-1.5.1/hello/io/__init__.py
--rw-r--r--   0        0        0     1382 2022-08-23 09:20:12.751790 hello2-1.5.1/hello/io/image.py
--rw-r--r--   0        0        0      925 2022-10-24 06:29:25.755587 hello2-1.5.1/hello/io/utils.py
--rw-r--r--   0        0        0      851 2022-11-25 07:46:45.875120 hello2-1.5.1/hello/mmdet/__init__.py
--rw-r--r--   0        0        0       67 2022-10-17 07:49:46.479528 hello2-1.5.1/hello/mmdet/__main__.py
--rw-r--r--   0        0        0       97 2022-10-17 08:00:01.479443 hello2-1.5.1/hello/mmdet/export.py
--rw-r--r--   0        0        0     1736 2022-10-20 16:17:29.762828 hello2-1.5.1/hello/mmdet/flop.py
--rw-r--r--   0        0        0     5446 2023-03-03 15:16:46.611009 hello2-1.5.1/hello/mmdet/infer.py
--rw-r--r--   0        0        0     3283 2022-11-09 15:21:06.213089 hello2-1.5.1/hello/mmdet/log.py
--rw-r--r--   0        0        0     5871 2023-01-06 01:40:14.354697 hello2-1.5.1/hello/mmdet/plot.py
--rw-r--r--   0        0        0      645 2022-11-07 02:04:01.296693 hello2-1.5.1/hello/mmseg/__init__.py
--rw-r--r--   0        0        0       67 2022-10-31 01:39:47.674470 hello2-1.5.1/hello/mmseg/__main__.py
--rw-r--r--   0        0        0     6040 2022-11-09 01:29:31.447414 hello2-1.5.1/hello/mmseg/infer.py
--rw-r--r--   0        0        0     2368 2022-11-09 15:21:26.233085 hello2-1.5.1/hello/mmseg/log.py
--rw-r--r--   0        0        0     7006 2022-12-01 12:09:30.751861 hello2-1.5.1/hello/mmseg/lr.py
--rw-r--r--   0        0        0      462 2023-03-29 08:04:38.934968 hello2-1.5.1/hello/nanodet/__init__.py
--rw-r--r--   0        0        0       67 2023-03-29 08:03:09.784974 hello2-1.5.1/hello/nanodet/__main__.py
--rw-r--r--   0        0        0     7410 2023-03-30 04:26:27.357246 hello2-1.5.1/hello/nanodet/infer.py
--rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.5.1/hello/onnx/__init__.py
--rw-r--r--   0        0        0      213 2022-06-27 02:15:25.376085 hello2-1.5.1/hello/onnx/examples/README.md
--rw-r--r--   0        0        0     1879 2022-06-27 01:46:45.026108 hello2-1.5.1/hello/onnx/examples/test_sigmoid.py
--rw-r--r--   0        0        0     3024 2022-08-30 07:45:32.884923 hello2-1.5.1/hello/onnx/export.py
--rw-r--r--   0        0        0     1707 2022-08-22 07:09:07.802604 hello2-1.5.1/hello/onnx/infer.py
--rw-r--r--   0        0        0     1334 2022-11-21 14:14:37.239473 hello2-1.5.1/hello/transforms/README.md
--rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.5.1/hello/transforms/__init__.py
--rw-r--r--   0        0        0     2655 2022-11-21 15:01:54.364062 hello2-1.5.1/hello/transforms/transforms.py
--rw-r--r--   0        0        0        0 2022-07-20 06:21:09.967902 hello2-1.5.1/hello/utils/__init__.py
--rw-r--r--   0        0        0     1793 2022-12-06 09:45:32.879987 hello2-1.5.1/hello/utils/colors.py
--rw-r--r--   0        0        0     1815 2022-10-14 02:36:42.461531 hello2-1.5.1/hello/utils/cuda.py
--rw-r--r--   0        0        0      356 2022-07-20 06:43:22.727885 hello2-1.5.1/hello/utils/importer.py
--rw-r--r--   0        0        0      612 2022-08-23 06:44:50.231910 hello2-1.5.1/hello/utils/plots.py
--rw-r--r--   0        0        0     2999 2022-11-06 13:40:43.281966 hello2-1.5.1/hello/utils/points.py
--rw-r--r--   0        0        0      195 2022-11-30 01:25:21.821313 hello2-1.5.1/hello/utils/strtime.py
--rw-r--r--   0        0        0     1135 2023-02-20 08:24:47.078416 hello2-1.5.1/hello/video/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.1/hello/video/__main__.py
--rw-r--r--   0        0        0     3428 2022-11-06 13:15:37.862480 hello2-1.5.1/hello/video/align.py
--rw-r--r--   0        0        0     6233 2023-02-20 09:54:00.778138 hello2-1.5.1/hello/video/clip.py
--rw-r--r--   0        0        0     3290 2023-02-20 09:35:59.918194 hello2-1.5.1/hello/video/fisheye.py
--rw-r--r--   0        0        0     1565 2022-11-06 13:15:49.722478 hello2-1.5.1/hello/video/info.py
--rw-r--r--   0        0        0     3502 2022-11-06 13:15:55.532477 hello2-1.5.1/hello/video/resize.py
--rw-r--r--   0        0        0     4716 2022-11-29 07:15:17.421543 hello2-1.5.1/hello/video/rtsp.py
--rw-r--r--   0        0        0     5006 2022-11-29 08:00:32.141119 hello2-1.5.1/hello/video/rtsp_pull.py
--rw-r--r--   0        0        0     3048 2022-11-11 09:35:15.036742 hello2-1.5.1/hello/video/split.py
--rw-r--r--   0        0        0     4066 2023-02-20 08:27:40.638408 hello2-1.5.1/hello/video/unwarp.py
--rw-r--r--   0        0        0      968 2022-08-25 04:09:32.554890 hello2-1.5.1/hello/video/utils.py
--rw-r--r--   0        0        0      576 2022-11-06 13:41:08.801958 hello2-1.5.1/hello/x3m/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.1/hello/x3m/__main__.py
--rw-r--r--   0        0        0     4479 2022-11-06 13:41:19.251954 hello2-1.5.1/hello/x3m/config.py
--rw-r--r--   0        0        0     2592 2022-08-30 01:19:13.615222 hello2-1.5.1/hello/x3m/preprocess.py
--rw-r--r--   0        0        0     6928 2022-06-27 01:46:45.026108 hello2-1.5.1/hello/x3m/transforms.py
--rw-r--r--   0        0        0      808 2022-06-27 01:46:45.026108 hello2-1.5.1/hello_c/CMakeLists.txt
--rw-r--r--   0        0        0      776 2022-06-27 01:46:45.026108 hello2-1.5.1/hello_c/README.md
--rw-r--r--   0        0        0     1375 2022-06-27 01:46:45.026108 hello2-1.5.1/hello_c/main.cpp
--rw-r--r--   0        0        0      262 2022-06-27 01:46:45.026108 hello2-1.5.1/hello_c/trace_model.py
--rw-r--r--   0        0        0      754 2023-03-29 08:06:34.334946 hello2-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 hello2-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      550 2022-11-04 08:45:52.036893 hello2-1.5.2/.gitignore
+-rw-r--r--   0        0        0      715 2022-11-04 17:06:29.116576 hello2-1.5.2/.readthedocs.yaml
+-rw-r--r--   0        0        0    11357 2022-06-27 01:46:45.026108 hello2-1.5.2/LICENSE
+-rw-r--r--   0        0        0      351 2022-12-20 05:58:10.658183 hello2-1.5.2/README.md
+-rw-r--r--   0        0        0      638 2022-11-04 13:36:31.980929 hello2-1.5.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-11-04 13:36:31.980929 hello2-1.5.2/docs/make.bat
+-rw-r--r--   0        0        0      163 2022-11-06 11:07:57.505182 hello2-1.5.2/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.5.2/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.5.2/docs/source/_templates/.gitkeep
+-rw-r--r--   0        0        0     1365 2022-11-06 12:23:09.043638 hello2-1.5.2/docs/source/conf.py
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.770149 hello2-1.5.2/docs/source/hello.data.coco2yolo.rst
+-rw-r--r--   0        0        0      231 2022-11-04 14:14:10.770149 hello2-1.5.2/docs/source/hello.data.rst
+-rw-r--r--   0        0        0      187 2022-12-14 01:38:29.403883 hello2-1.5.2/docs/source/hello.experimental.albu.detection.rst
+-rw-r--r--   0        0        0      283 2022-12-14 01:38:29.403883 hello2-1.5.2/docs/source/hello.experimental.albu.rst
+-rw-r--r--   0        0        0      260 2022-12-14 01:38:29.393883 hello2-1.5.2/docs/source/hello.experimental.rst
+-rw-r--r--   0        0        0      148 2022-12-14 09:04:35.414160 hello2-1.5.2/docs/source/hello.fiftyone.brain.rst
+-rw-r--r--   0        0        0      160 2022-11-18 12:12:27.461051 hello2-1.5.2/docs/source/hello.fiftyone.copypaste.rst
+-rw-r--r--   0        0        0      145 2022-11-04 14:14:10.780149 hello2-1.5.2/docs/source/hello.fiftyone.core.rst
+-rw-r--r--   0        0        0      154 2022-11-04 14:14:10.780149 hello2-1.5.2/docs/source/hello.fiftyone.dataset.rst
+-rw-r--r--   0        0        0      183 2022-11-04 14:14:10.780149 hello2-1.5.2/docs/source/hello.fiftyone.dataset_annotate.rst
+-rw-r--r--   0        0        0      189 2022-11-04 14:14:10.780149 hello2-1.5.2/docs/source/hello.fiftyone.dataset_detections.rst
+-rw-r--r--   0        0        0      198 2022-11-04 14:14:10.790149 hello2-1.5.2/docs/source/hello.fiftyone.dataset_segmentations.rst
+-rw-r--r--   0        0        0      177 2022-11-04 14:14:10.790149 hello2-1.5.2/docs/source/hello.fiftyone.dataset_yolov5.rst
+-rw-r--r--   0        0        0      168 2022-11-04 14:14:10.790149 hello2-1.5.2/docs/source/hello.fiftyone.dataset_zoo.rst
+-rw-r--r--   0        0        0      157 2022-11-04 14:14:10.790149 hello2-1.5.2/docs/source/hello.fiftyone.evaluate.rst
+-rw-r--r--   0        0        0      192 2022-11-04 14:14:10.790149 hello2-1.5.2/docs/source/hello.fiftyone.evaluate_detections.rst
+-rw-r--r--   0        0        0      201 2022-11-04 14:14:10.790149 hello2-1.5.2/docs/source/hello.fiftyone.evaluate_segmentations.rst
+-rw-r--r--   0        0        0      171 2022-11-18 12:12:27.481051 hello2-1.5.2/docs/source/hello.fiftyone.gen_examples.rst
+-rw-r--r--   0        0        0      168 2022-11-18 12:12:27.481051 hello2-1.5.2/docs/source/hello.fiftyone.mask_ignore.rst
+-rw-r--r--   0        0        0      145 2022-11-04 14:14:10.790149 hello2-1.5.2/docs/source/hello.fiftyone.miou.rst
+-rw-r--r--   0        0        0      154 2022-11-18 12:12:27.481051 hello2-1.5.2/docs/source/hello.fiftyone.patches.rst
+-rw-r--r--   0        0        0      833 2022-12-16 13:39:47.510383 hello2-1.5.2/docs/source/hello.fiftyone.rst
+-rw-r--r--   0        0        0      154 2022-12-16 13:39:47.530383 hello2-1.5.2/docs/source/hello.fiftyone.tarinfo.rst
+-rw-r--r--   0        0        0      151 2022-11-04 14:14:10.800149 hello2-1.5.2/docs/source/hello.fiftyone.unique.rst
+-rw-r--r--   0        0        0      148 2022-11-22 16:10:13.239568 hello2-1.5.2/docs/source/hello.fiftyone.utils.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.800149 hello2-1.5.2/docs/source/hello.fiftyone.video.rst
+-rw-r--r--   0        0        0      145 2022-11-22 16:10:13.239568 hello2-1.5.2/docs/source/hello.fiftyone.view.rst
+-rw-r--r--   0        0        0      159 2022-11-04 15:41:25.788323 hello2-1.5.2/docs/source/hello.fvcore.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.800149 hello2-1.5.2/docs/source/hello.io.image.rst
+-rw-r--r--   0        0        0      237 2022-11-04 14:14:10.800149 hello2-1.5.2/docs/source/hello.io.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.810149 hello2-1.5.2/docs/source/hello.io.utils.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.810149 hello2-1.5.2/docs/source/hello.mmdet.export.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.810149 hello2-1.5.2/docs/source/hello.mmdet.flop.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.820149 hello2-1.5.2/docs/source/hello.mmdet.infer.rst
+-rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.5.2/docs/source/hello.mmdet.log.rst
+-rw-r--r--   0        0        0      136 2022-11-25 07:45:47.915124 hello2-1.5.2/docs/source/hello.mmdet.plot.rst
+-rw-r--r--   0        0        0      312 2022-11-25 07:45:47.915124 hello2-1.5.2/docs/source/hello.mmdet.rst
+-rw-r--r--   0        0        0      139 2022-11-07 02:04:44.756679 hello2-1.5.2/docs/source/hello.mmseg.infer.rst
+-rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.5.2/docs/source/hello.mmseg.log.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.820149 hello2-1.5.2/docs/source/hello.mmseg.lr.rst
+-rw-r--r--   0        0        0      268 2022-11-07 02:04:44.756679 hello2-1.5.2/docs/source/hello.mmseg.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.830149 hello2-1.5.2/docs/source/hello.onnx.export.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.830149 hello2-1.5.2/docs/source/hello.onnx.infer.rst
+-rw-r--r--   0        0        0      248 2022-11-04 14:14:10.830149 hello2-1.5.2/docs/source/hello.onnx.rst
+-rw-r--r--   0        0        0      383 2022-12-14 01:38:29.383883 hello2-1.5.2/docs/source/hello.rst
+-rw-r--r--   0        0        0      256 2022-11-04 14:14:10.840149 hello2-1.5.2/docs/source/hello.transforms.rst
+-rw-r--r--   0        0        0      169 2022-11-04 14:14:10.840149 hello2-1.5.2/docs/source/hello.transforms.transforms.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.5.2/docs/source/hello.utils.colors.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.850149 hello2-1.5.2/docs/source/hello.utils.cuda.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.850149 hello2-1.5.2/docs/source/hello.utils.importer.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.850149 hello2-1.5.2/docs/source/hello.utils.plots.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.5.2/docs/source/hello.utils.points.rst
+-rw-r--r--   0        0        0      342 2022-11-30 10:15:09.966399 hello2-1.5.2/docs/source/hello.utils.rst
+-rw-r--r--   0        0        0      145 2022-11-30 10:15:09.976399 hello2-1.5.2/docs/source/hello.utils.strtime.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.860149 hello2-1.5.2/docs/source/hello.video.align.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.5.2/docs/source/hello.video.clip.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.5.2/docs/source/hello.video.frames.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.5.2/docs/source/hello.video.info.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.5.2/docs/source/hello.video.resize.rst
+-rw-r--r--   0        0        0      424 2022-11-29 06:30:33.921961 hello2-1.5.2/docs/source/hello.video.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.870149 hello2-1.5.2/docs/source/hello.video.rtsp.rst
+-rw-r--r--   0        0        0      153 2022-11-29 06:30:33.931961 hello2-1.5.2/docs/source/hello.video.rtsp_pull.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.5.2/docs/source/hello.video.split.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.870149 hello2-1.5.2/docs/source/hello.video.unwarp.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.5.2/docs/source/hello.video.utils.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.880149 hello2-1.5.2/docs/source/hello.x3m.config.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.5.2/docs/source/hello.x3m.preprocess.rst
+-rw-r--r--   0        0        0      272 2022-11-04 14:14:10.870149 hello2-1.5.2/docs/source/hello.x3m.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.5.2/docs/source/hello.x3m.transforms.rst
+-rw-r--r--   0        0        0      572 2022-11-04 15:19:50.508765 hello2-1.5.2/docs/source/index.rst
+-rw-r--r--   0        0        0       52 2022-11-04 14:40:30.829573 hello2-1.5.2/docs/source/modules.rst
+-rw-r--r--   0        0        0     3338 2023-02-22 04:02:31.469946 hello2-1.5.2/hello/README.md
+-rw-r--r--   0        0        0      754 2023-04-11 07:08:26.654399 hello2-1.5.2/hello/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.2/hello/__main__.py
+-rw-r--r--   0        0        0      471 2022-11-06 13:38:11.482015 hello2-1.5.2/hello/data/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.2/hello/data/__main__.py
+-rw-r--r--   0        0        0     3426 2022-08-30 01:19:13.615222 hello2-1.5.2/hello/data/coco2yolo.py
+-rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.5.2/hello/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.5.2/hello/experimental/albu/__init__.py
+-rw-r--r--   0        0        0      111 2022-12-11 06:23:09.504528 hello2-1.5.2/hello/experimental/albu/detection.py
+-rw-r--r--   0        0        0     1047 2022-11-06 13:38:17.442013 hello2-1.5.2/hello/fiftyone/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.2/hello/fiftyone/__main__.py
+-rw-r--r--   0        0        0     4781 2023-03-15 05:39:13.846289 hello2-1.5.2/hello/fiftyone/annotate.py
+-rw-r--r--   0        0        0     8329 2022-12-14 15:06:12.986153 hello2-1.5.2/hello/fiftyone/brain.py
+-rw-r--r--   0        0        0       36 2022-11-18 04:25:30.455378 hello2-1.5.2/hello/fiftyone/copypaste.py
+-rw-r--r--   0        0        0    16956 2023-04-04 06:50:41.417819 hello2-1.5.2/hello/fiftyone/core.py
+-rw-r--r--   0        0        0    21141 2023-03-15 09:00:27.664680 hello2-1.5.2/hello/fiftyone/dataset.py
+-rw-r--r--   0        0        0     7502 2022-12-30 03:41:16.092249 hello2-1.5.2/hello/fiftyone/dataset_detections.py
+-rw-r--r--   0        0        0     5693 2022-12-30 03:45:01.362177 hello2-1.5.2/hello/fiftyone/dataset_segmentations.py
+-rw-r--r--   0        0        0     1402 2022-11-30 01:50:37.091070 hello2-1.5.2/hello/fiftyone/dataset_yolov5.py
+-rw-r--r--   0        0        0      889 2022-12-02 08:54:06.970245 hello2-1.5.2/hello/fiftyone/dataset_zoo.py
+-rw-r--r--   0        0        0     1169 2022-07-18 00:56:40.761934 hello2-1.5.2/hello/fiftyone/evaluate.py
+-rw-r--r--   0        0        0     5157 2023-03-07 04:04:15.369663 hello2-1.5.2/hello/fiftyone/evaluate_detections.py
+-rw-r--r--   0        0        0     4544 2023-03-07 04:04:11.609664 hello2-1.5.2/hello/fiftyone/evaluate_segmentations.py
+-rw-r--r--   0        0        0      103 2022-09-19 06:15:49.337504 hello2-1.5.2/hello/fiftyone/examples/README.md
+-rw-r--r--   0        0        0     2975 2022-11-30 01:46:25.831120 hello2-1.5.2/hello/fiftyone/examples/examples.py
+-rw-r--r--   0        0        0    12021 2023-01-09 09:33:51.046594 hello2-1.5.2/hello/fiftyone/examples/utils.py
+-rw-r--r--   0        0        0     2133 2022-11-16 04:13:14.052375 hello2-1.5.2/hello/fiftyone/gen_examples.py
+-rw-r--r--   0        0        0     1608 2022-11-18 03:16:41.036018 hello2-1.5.2/hello/fiftyone/mask_ignore.py
+-rw-r--r--   0        0        0     5683 2022-12-30 03:42:18.702230 hello2-1.5.2/hello/fiftyone/miou.py
+-rw-r--r--   0        0        0     2639 2022-11-18 06:29:39.594231 hello2-1.5.2/hello/fiftyone/patches.py
+-rw-r--r--   0        0        0     7934 2023-03-22 02:58:26.970148 hello2-1.5.2/hello/fiftyone/tarinfo.py
+-rw-r--r--   0        0        0     4094 2023-03-15 08:42:32.674825 hello2-1.5.2/hello/fiftyone/unique.py
+-rw-r--r--   0        0        0     7621 2023-01-09 04:04:27.118496 hello2-1.5.2/hello/fiftyone/utils.py
+-rw-r--r--   0        0        0      781 2022-12-01 14:14:43.560707 hello2-1.5.2/hello/fiftyone/video.py
+-rw-r--r--   0        0        0     8010 2023-04-03 07:48:18.837028 hello2-1.5.2/hello/fiftyone/view.py
+-rw-r--r--   0        0        0      435 2022-10-20 14:18:34.575285 hello2-1.5.2/hello/fvcore/README.md
+-rw-r--r--   0        0        0        0 2022-11-04 14:49:06.729395 hello2-1.5.2/hello/fvcore/__init__.py
+-rw-r--r--   0        0        0      135 2022-06-27 01:46:45.026108 hello2-1.5.2/hello/io/__init__.py
+-rw-r--r--   0        0        0     1382 2022-08-23 09:20:12.751790 hello2-1.5.2/hello/io/image.py
+-rw-r--r--   0        0        0      925 2022-10-24 06:29:25.755587 hello2-1.5.2/hello/io/utils.py
+-rw-r--r--   0        0        0      851 2022-11-25 07:46:45.875120 hello2-1.5.2/hello/mmdet/__init__.py
+-rw-r--r--   0        0        0       67 2022-10-17 07:49:46.479528 hello2-1.5.2/hello/mmdet/__main__.py
+-rw-r--r--   0        0        0       97 2022-10-17 08:00:01.479443 hello2-1.5.2/hello/mmdet/export.py
+-rw-r--r--   0        0        0     1736 2022-10-20 16:17:29.762828 hello2-1.5.2/hello/mmdet/flop.py
+-rw-r--r--   0        0        0     5446 2023-03-03 15:16:46.611009 hello2-1.5.2/hello/mmdet/infer.py
+-rw-r--r--   0        0        0     3273 2023-04-11 07:00:00.274582 hello2-1.5.2/hello/mmdet/log.py
+-rw-r--r--   0        0        0     5871 2023-04-11 07:12:30.594314 hello2-1.5.2/hello/mmdet/plot.py
+-rw-r--r--   0        0        0      645 2022-11-07 02:04:01.296693 hello2-1.5.2/hello/mmseg/__init__.py
+-rw-r--r--   0        0        0       67 2022-10-31 01:39:47.674470 hello2-1.5.2/hello/mmseg/__main__.py
+-rw-r--r--   0        0        0     6040 2022-11-09 01:29:31.447414 hello2-1.5.2/hello/mmseg/infer.py
+-rw-r--r--   0        0        0     2368 2023-04-11 07:03:55.124501 hello2-1.5.2/hello/mmseg/log.py
+-rw-r--r--   0        0        0     7006 2022-12-01 12:09:30.751861 hello2-1.5.2/hello/mmseg/lr.py
+-rw-r--r--   0        0        0      462 2023-03-29 08:04:38.934968 hello2-1.5.2/hello/nanodet/__init__.py
+-rw-r--r--   0        0        0       67 2023-03-29 08:03:09.784974 hello2-1.5.2/hello/nanodet/__main__.py
+-rw-r--r--   0        0        0     7410 2023-04-06 10:19:32.462564 hello2-1.5.2/hello/nanodet/infer.py
+-rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.5.2/hello/onnx/__init__.py
+-rw-r--r--   0        0        0      213 2022-06-27 02:15:25.376085 hello2-1.5.2/hello/onnx/examples/README.md
+-rw-r--r--   0        0        0     1879 2022-06-27 01:46:45.026108 hello2-1.5.2/hello/onnx/examples/test_sigmoid.py
+-rw-r--r--   0        0        0     3024 2022-08-30 07:45:32.884923 hello2-1.5.2/hello/onnx/export.py
+-rw-r--r--   0        0        0     1707 2022-08-22 07:09:07.802604 hello2-1.5.2/hello/onnx/infer.py
+-rw-r--r--   0        0        0     1334 2022-11-21 14:14:37.239473 hello2-1.5.2/hello/transforms/README.md
+-rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.5.2/hello/transforms/__init__.py
+-rw-r--r--   0        0        0     2655 2022-11-21 15:01:54.364062 hello2-1.5.2/hello/transforms/transforms.py
+-rw-r--r--   0        0        0        0 2022-07-20 06:21:09.967902 hello2-1.5.2/hello/utils/__init__.py
+-rw-r--r--   0        0        0     1793 2022-12-06 09:45:32.879987 hello2-1.5.2/hello/utils/colors.py
+-rw-r--r--   0        0        0     1815 2022-10-14 02:36:42.461531 hello2-1.5.2/hello/utils/cuda.py
+-rw-r--r--   0        0        0      356 2022-07-20 06:43:22.727885 hello2-1.5.2/hello/utils/importer.py
+-rw-r--r--   0        0        0      612 2022-08-23 06:44:50.231910 hello2-1.5.2/hello/utils/plots.py
+-rw-r--r--   0        0        0     2999 2022-11-06 13:40:43.281966 hello2-1.5.2/hello/utils/points.py
+-rw-r--r--   0        0        0      195 2022-11-30 01:25:21.821313 hello2-1.5.2/hello/utils/strtime.py
+-rw-r--r--   0        0        0     1135 2023-02-20 08:24:47.078416 hello2-1.5.2/hello/video/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.2/hello/video/__main__.py
+-rw-r--r--   0        0        0     3428 2022-11-06 13:15:37.862480 hello2-1.5.2/hello/video/align.py
+-rw-r--r--   0        0        0     6233 2023-02-20 09:54:00.778138 hello2-1.5.2/hello/video/clip.py
+-rw-r--r--   0        0        0     3290 2023-02-20 09:35:59.918194 hello2-1.5.2/hello/video/fisheye.py
+-rw-r--r--   0        0        0     1565 2022-11-06 13:15:49.722478 hello2-1.5.2/hello/video/info.py
+-rw-r--r--   0        0        0     3502 2022-11-06 13:15:55.532477 hello2-1.5.2/hello/video/resize.py
+-rw-r--r--   0        0        0     4716 2022-11-29 07:15:17.421543 hello2-1.5.2/hello/video/rtsp.py
+-rw-r--r--   0        0        0     5006 2022-11-29 08:00:32.141119 hello2-1.5.2/hello/video/rtsp_pull.py
+-rw-r--r--   0        0        0     3048 2022-11-11 09:35:15.036742 hello2-1.5.2/hello/video/split.py
+-rw-r--r--   0        0        0     4066 2023-02-20 08:27:40.638408 hello2-1.5.2/hello/video/unwarp.py
+-rw-r--r--   0        0        0      968 2022-08-25 04:09:32.554890 hello2-1.5.2/hello/video/utils.py
+-rw-r--r--   0        0        0      576 2022-11-06 13:41:08.801958 hello2-1.5.2/hello/x3m/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.5.2/hello/x3m/__main__.py
+-rw-r--r--   0        0        0     4479 2022-11-06 13:41:19.251954 hello2-1.5.2/hello/x3m/config.py
+-rw-r--r--   0        0        0     2592 2022-08-30 01:19:13.615222 hello2-1.5.2/hello/x3m/preprocess.py
+-rw-r--r--   0        0        0     6928 2022-06-27 01:46:45.026108 hello2-1.5.2/hello/x3m/transforms.py
+-rw-r--r--   0        0        0      808 2022-06-27 01:46:45.026108 hello2-1.5.2/hello_c/CMakeLists.txt
+-rw-r--r--   0        0        0      776 2022-06-27 01:46:45.026108 hello2-1.5.2/hello_c/README.md
+-rw-r--r--   0        0        0     1375 2022-06-27 01:46:45.026108 hello2-1.5.2/hello_c/main.cpp
+-rw-r--r--   0        0        0      262 2022-06-27 01:46:45.026108 hello2-1.5.2/hello_c/trace_model.py
+-rw-r--r--   0        0        0      754 2023-03-29 08:06:34.334946 hello2-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3739 1970-01-01 00:00:00.000000 hello2-1.5.2/PKG-INFO
```

### Comparing `hello2-1.5.1/.gitignore` & `hello2-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/.readthedocs.yaml` & `hello2-1.5.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/LICENSE` & `hello2-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/docs/Makefile` & `hello2-1.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/docs/make.bat` & `hello2-1.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/docs/source/conf.py` & `hello2-1.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/docs/source/hello.fiftyone.rst` & `hello2-1.5.2/docs/source/hello.fiftyone.rst`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/docs/source/index.rst` & `hello2-1.5.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/README.md` & `hello2-1.5.2/hello/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/__init__.py` & `hello2-1.5.2/hello/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "1.5.1"
+__version__ = "1.5.2"
 
 help_doc_str = """\
 usage: hello [--version] [--help]
 
 shell command:
     hello -h
     hello-data -h
```

### Comparing `hello2-1.5.1/hello/data/coco2yolo.py` & `hello2-1.5.2/hello/data/coco2yolo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/__init__.py` & `hello2-1.5.2/hello/fiftyone/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/annotate.py` & `hello2-1.5.2/hello/fiftyone/annotate.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/brain.py` & `hello2-1.5.2/hello/fiftyone/brain.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/core.py` & `hello2-1.5.2/hello/fiftyone/core.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/dataset.py` & `hello2-1.5.2/hello/fiftyone/dataset.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/dataset_detections.py` & `hello2-1.5.2/hello/fiftyone/dataset_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/dataset_segmentations.py` & `hello2-1.5.2/hello/fiftyone/dataset_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/dataset_yolov5.py` & `hello2-1.5.2/hello/fiftyone/dataset_yolov5.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/dataset_zoo.py` & `hello2-1.5.2/hello/fiftyone/dataset_zoo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/evaluate.py` & `hello2-1.5.2/hello/fiftyone/evaluate.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/evaluate_detections.py` & `hello2-1.5.2/hello/fiftyone/evaluate_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/evaluate_segmentations.py` & `hello2-1.5.2/hello/fiftyone/evaluate_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/examples/examples.py` & `hello2-1.5.2/hello/fiftyone/examples/examples.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/examples/utils.py` & `hello2-1.5.2/hello/fiftyone/examples/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/gen_examples.py` & `hello2-1.5.2/hello/fiftyone/gen_examples.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/mask_ignore.py` & `hello2-1.5.2/hello/fiftyone/mask_ignore.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/miou.py` & `hello2-1.5.2/hello/fiftyone/miou.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/patches.py` & `hello2-1.5.2/hello/fiftyone/patches.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/tarinfo.py` & `hello2-1.5.2/hello/fiftyone/tarinfo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/unique.py` & `hello2-1.5.2/hello/fiftyone/unique.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/utils.py` & `hello2-1.5.2/hello/fiftyone/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/video.py` & `hello2-1.5.2/hello/fiftyone/video.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/fiftyone/view.py` & `hello2-1.5.2/hello/fiftyone/view.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/io/image.py` & `hello2-1.5.2/hello/io/image.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/io/utils.py` & `hello2-1.5.2/hello/io/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/mmdet/__init__.py` & `hello2-1.5.2/hello/mmdet/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/mmdet/flop.py` & `hello2-1.5.2/hello/mmdet/flop.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/mmdet/infer.py` & `hello2-1.5.2/hello/mmdet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/mmdet/log.py` & `hello2-1.5.2/hello/mmdet/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 
-def func(json_logs, out_dir, metrics=["loss", "loss_cls", "loss_bbox"], mmdet_home="/workspace", format=".png"):
+def func(json_logs, out_dir, metrics, mmdet_home="/workspace", format=".png"):
     out_dir = Path(out_dir)
     shutil.rmtree(out_dir, ignore_errors=True)
     (out_dir / "images").mkdir(parents=True, exist_ok=False)
 
     if Path(json_logs[0]).is_dir():
         json_logs = [str(f) for f in Path(json_logs[0]).glob("*/*.log.json")]
         json_logs = sorted(json_logs)
@@ -43,14 +43,15 @@
         _arg_out = " ".join(["--out"] + [str(out_dir / f"images/metric_{metric}{format}")])
         _arg_json_logs = " ".join(json_logs)
 
         command_line = f"python {py_script} plot_curve {_arg_keys} {_arg_title} {_arg_legend} {_arg_out} {_arg_json_logs}"
         result = subprocess.run(command_line, shell=True, stdout=subprocess.PIPE)
         if result.returncode != 0:
             print(f"[ERR]\n  {command_line}")
+    return str(out_dir)
 
 
 def parse_args(args=None):
     from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
     parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter)
 
     parser.add_argument("json_logs", type=str, nargs='+',
```

### Comparing `hello2-1.5.1/hello/mmdet/plot.py` & `hello2-1.5.2/hello/mmdet/plot.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/mmseg/__init__.py` & `hello2-1.5.2/hello/mmseg/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/mmseg/infer.py` & `hello2-1.5.2/hello/mmseg/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/mmseg/log.py` & `hello2-1.5.2/hello/mmseg/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 
-def func(json_logs, out_dir, metrics, mmdet_home="/workspace", format=".png"):
+def func(json_logs, out_dir, metrics, mmseg_home="/workspace", format=".png"):
     out_dir = Path(out_dir)
     shutil.rmtree(out_dir, ignore_errors=True)
     (out_dir / "images").mkdir(parents=True, exist_ok=False)
 
     if Path(json_logs[0]).is_dir():
         json_logs = [str(f) for f in Path(json_logs[0]).glob("*/*.log.json")]
         json_logs = sorted(json_logs)
 
-    py_script = str(Path(mmdet_home) / "tools/analyze_logs.py")
+    py_script = str(Path(mmseg_home) / "tools/analyze_logs.py")
 
     for metric in metrics + ["mIoU", "mAcc", "aAcc"]:
         run_name_list = [Path(f).parent.name for f in json_logs]
 
         _arg_keys = " ".join(["--keys"] + [metric])
         _arg_title = " ".join(["--title"] + [metric])
         _arg_legend = " ".join(["--legend"] + run_name_list)
@@ -38,16 +38,16 @@
     parser.add_argument("json_logs", type=str, nargs='+',
                         help="path of train log in json format or runs dir")
     parser.add_argument("-o", dest="out_dir", type=str,
                         help="save plotting curves to the dir")
     parser.add_argument("-m", dest="metrics", type=str, nargs='+',
                         default=["decode.loss_ce", "decode.acc_seg", "loss"],
                         help="the metric that you want to plot")
-    parser.add_argument("-b", dest="mmdet_home", type=str, default="/workspace",
-                        help="specify the mmdet home")
+    parser.add_argument("-b", dest="mmseg_home", type=str, default="/workspace",
+                        help="specify the mmseg home")
     parser.add_argument("-f", dest="format", type=str, default=".png",
                         help="image save format")
 
     args = parser.parse_args(args=args)
     return vars(args)
```

### Comparing `hello2-1.5.1/hello/mmseg/lr.py` & `hello2-1.5.2/hello/mmseg/lr.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/nanodet/infer.py` & `hello2-1.5.2/hello/nanodet/infer.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         height, width = img.shape[:2]
         img_info["height"] = height
         img_info["width"] = width
         meta = dict(img_info=img_info, raw_img=img, img=img)
         meta = self.pipeline(None, meta, self.cfg.data.val.input_size)
         meta["img"] = torch.from_numpy(meta["img"].transpose(2, 0, 1)).to(self.device)
         meta = naive_collate([meta])
-        meta["img"] = stack_batch_img(meta["img"], divisible=32)
+        meta["img"] = stack_batch_img(meta["img"], divisible=64)
         with torch.no_grad():
             results = self.model.inference(meta)
         return meta, results
 
     def test_images(self, images_or_dir, score_thr=0.3, out_dir=None):
         """Inference images with the predictor.
```

### Comparing `hello2-1.5.1/hello/onnx/examples/test_sigmoid.py` & `hello2-1.5.2/hello/onnx/examples/test_sigmoid.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/onnx/export.py` & `hello2-1.5.2/hello/onnx/export.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/onnx/infer.py` & `hello2-1.5.2/hello/onnx/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/transforms/README.md` & `hello2-1.5.2/hello/transforms/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/transforms/transforms.py` & `hello2-1.5.2/hello/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/utils/colors.py` & `hello2-1.5.2/hello/utils/colors.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/utils/cuda.py` & `hello2-1.5.2/hello/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/utils/plots.py` & `hello2-1.5.2/hello/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/utils/points.py` & `hello2-1.5.2/hello/utils/points.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/__init__.py` & `hello2-1.5.2/hello/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/align.py` & `hello2-1.5.2/hello/video/align.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/clip.py` & `hello2-1.5.2/hello/video/clip.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/fisheye.py` & `hello2-1.5.2/hello/video/fisheye.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/info.py` & `hello2-1.5.2/hello/video/info.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/resize.py` & `hello2-1.5.2/hello/video/resize.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/rtsp.py` & `hello2-1.5.2/hello/video/rtsp.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/rtsp_pull.py` & `hello2-1.5.2/hello/video/rtsp_pull.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/split.py` & `hello2-1.5.2/hello/video/split.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/unwarp.py` & `hello2-1.5.2/hello/video/unwarp.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/video/utils.py` & `hello2-1.5.2/hello/video/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/x3m/__init__.py` & `hello2-1.5.2/hello/x3m/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/x3m/config.py` & `hello2-1.5.2/hello/x3m/config.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/x3m/preprocess.py` & `hello2-1.5.2/hello/x3m/preprocess.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello/x3m/transforms.py` & `hello2-1.5.2/hello/x3m/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello_c/CMakeLists.txt` & `hello2-1.5.2/hello_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello_c/README.md` & `hello2-1.5.2/hello_c/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/hello_c/main.cpp` & `hello2-1.5.2/hello_c/main.cpp`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/pyproject.toml` & `hello2-1.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hello2-1.5.1/PKG-INFO` & `hello2-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello2
-Version: 1.5.1
+Version: 1.5.2
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: scikit-image
```

