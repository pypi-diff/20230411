# Comparing `tmp/hordelib-0.2.0.tar.gz` & `tmp/hordelib-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.2.0.tar", last modified: Sat Apr  8 17:41:21 2023, max compression
+gzip compressed data, was "hordelib-0.4.1.tar", last modified: Mon Apr 10 21:50:24 2023, max compression
```

## Comparing `hordelib-0.2.0.tar` & `hordelib-0.4.1.tar`

### file list

```diff
@@ -1,109 +1,616 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.546485 hordelib-0.2.0/
--rw-rw-rw-   0        0        0      158 2023-04-06 17:36:05.000000 hordelib-0.2.0/.coveragerc
--rw-rw-rw-   0        0        0       88 2023-04-03 21:13:26.000000 hordelib-0.2.0/.flake8
--rw-rw-rw-   0        0        0      162 2023-04-07 14:09:36.000000 hordelib-0.2.0/.git-blame-ignore-revs
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.464260 hordelib-0.2.0/.github/
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.475261 hordelib-0.2.0/.github/workflows/
--rw-rw-rw-   0        0        0     2270 2023-04-06 23:34:51.000000 hordelib-0.2.0/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0      615 2023-04-08 16:55:32.000000 hordelib-0.2.0/.github/workflows/tests.yaml
--rw-rw-rw-   0        0        0     2191 2023-04-08 16:59:24.000000 hordelib-0.2.0/.gitignore
--rw-rw-rw-   0        0        0     3260 2023-04-08 17:26:58.000000 hordelib-0.2.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35182 2023-04-05 20:05:31.000000 hordelib-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    47456 2023-04-08 17:41:21.546485 hordelib-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6314 2023-04-08 16:59:24.000000 hordelib-0.2.0/README.md
--rw-rw-rw-   0        0        0     1666 2023-04-06 23:36:10.000000 hordelib-0.2.0/build_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.482260 hordelib-0.2.0/hordelib/
--rw-rw-rw-   0        0        0       94 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.507485 hordelib-0.2.0/hordelib/cache/
--rw-rw-rw-   0        0        0       60 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/cache/__init__.py
--rw-rw-rw-   0        0        0     8739 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/cache/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.511485 hordelib-0.2.0/hordelib/clip/
--rw-rw-rw-   0        0        0      131 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/clip/__init__.py
--rw-rw-rw-   0        0        0     2481 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/clip/bulk.py
--rw-rw-rw-   0        0        0     1088 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/clip/coca.py
--rw-rw-rw-   0        0        0     4681 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/clip/image.py
--rw-rw-rw-   0        0        0    12260 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/clip/interrogate.py
--rw-rw-rw-   0        0        0     3034 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/clip/text.py
--rw-rw-rw-   0        0        0    12822 2023-04-08 10:08:14.000000 hordelib-0.2.0/hordelib/comfy_horde.py
--rw-rw-rw-   0        0        0      527 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/config_path.py
--rw-rw-rw-   0        0        0      569 2023-04-08 17:40:47.000000 hordelib-0.2.0/hordelib/consts.py
--rw-rw-rw-   0        0        0     8631 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/horde.py
--rw-rw-rw-   0        0        0      789 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/initialisation.py
--rw-rw-rw-   0        0        0     3773 2023-04-07 17:27:13.000000 hordelib-0.2.0/hordelib/install_comfy.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.520484 hordelib-0.2.0/hordelib/model_manager/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/model_manager/__init__.py
--rw-rw-rw-   0        0        0     7823 2023-04-07 15:47:10.000000 hordelib-0.2.0/hordelib/model_manager/aitemplate.py
--rw-rw-rw-   0        0        0    20616 2023-04-07 15:47:24.000000 hordelib-0.2.0/hordelib/model_manager/base.py
--rw-rw-rw-   0        0        0     4195 2023-04-07 15:47:35.000000 hordelib-0.2.0/hordelib/model_manager/blip.py
--rw-rw-rw-   0        0        0     6767 2023-04-07 15:47:41.000000 hordelib-0.2.0/hordelib/model_manager/clip.py
--rw-rw-rw-   0        0        0     2858 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/model_manager/codeformer.py
--rw-rw-rw-   0        0        0     2226 2023-04-07 15:47:53.000000 hordelib-0.2.0/hordelib/model_manager/compvis.py
--rw-rw-rw-   0        0        0     5500 2023-04-07 15:47:57.000000 hordelib-0.2.0/hordelib/model_manager/controlnet.py
--rw-rw-rw-   0        0        0     4719 2023-04-07 15:48:03.000000 hordelib-0.2.0/hordelib/model_manager/diffusers.py
--rw-rw-rw-   0        0        0     2431 2023-04-07 15:48:06.000000 hordelib-0.2.0/hordelib/model_manager/esrgan.py
--rw-rw-rw-   0        0        0     2409 2023-04-07 15:48:10.000000 hordelib-0.2.0/hordelib/model_manager/gfpgan.py
--rw-rw-rw-   0        0        0    15731 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/model_manager/hyper.py
--rw-rw-rw-   0        0        0     3380 2023-04-07 15:48:13.000000 hordelib-0.2.0/hordelib/model_manager/new.py
--rw-rw-rw-   0        0        0     3553 2023-04-07 15:48:16.000000 hordelib-0.2.0/hordelib/model_manager/safety_checker.py
--rw-rw-rw-   0        0        0     8699 2023-04-07 20:20:31.000000 hordelib-0.2.0/hordelib/model_manager/sdu.py
--rw-rw-rw-   0        0        0     7282 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/model_manager/torch_hijack.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.524484 hordelib-0.2.0/hordelib/nodes/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/nodes/__init__.py
--rw-rw-rw-   0        0        0     1449 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/nodes/node_clip_similarities.py
--rw-rw-rw-   0        0        0      947 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/nodes/node_image_loader.py
--rw-rw-rw-   0        0        0     1634 2023-04-06 14:10:46.000000 hordelib-0.2.0/hordelib/nodes/node_image_output.py
--rw-rw-rw-   0        0        0     1244 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/nodes/node_model_loader.py
--rw-rw-rw-   0        0        0     1065 2023-04-08 16:59:24.000000 hordelib-0.2.0/hordelib/nodes/node_upscale_model_loader.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.527484 hordelib-0.2.0/hordelib/pipeline_designs/
--rw-rw-rw-   0        0        0     2807 2023-04-07 08:03:23.000000 hordelib-0.2.0/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-rw-rw-   0        0        0     8264 2023-04-07 17:52:13.000000 hordelib-0.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-rw-rw-   0        0        0    11353 2023-04-07 19:35:03.000000 hordelib-0.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-rw-rw-   0        0        0     8478 2023-04-08 08:48:44.000000 hordelib-0.2.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.529483 hordelib-0.2.0/hordelib/pipelines/
--rw-rw-rw-   0        0        0      802 2023-04-07 08:03:55.000000 hordelib-0.2.0/hordelib/pipelines/pipeline_image_upscale.json
--rw-rw-rw-   0        0        0     2470 2023-04-07 17:51:47.000000 hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-rw-rw-   0        0        0     3507 2023-04-07 19:08:34.000000 hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-rw-rw-   0        0        0     2561 2023-04-08 09:41:56.000000 hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-rw-rw-   0        0        0      473 2023-04-07 16:38:47.000000 hordelib-0.2.0/hordelib/run_comfyui.patch
--rw-rw-rw-   0        0        0     1245 2023-04-07 17:27:31.000000 hordelib-0.2.0/hordelib/run_comfyui.py
--rw-rw-rw-   0        0        0      717 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/safety_checker.py
--rw-rw-rw-   0        0        0      505 2023-04-06 09:46:54.000000 hordelib-0.2.0/hordelib/settings.py
--rw-rw-rw-   0        0        0      926 2023-04-07 10:32:48.000000 hordelib-0.2.0/hordelib/shared_model_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.530483 hordelib-0.2.0/hordelib/utils/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.2.0/hordelib/utils/__init__.py
--rw-rw-rw-   0        0        0      655 2023-04-07 14:09:36.000000 hordelib-0.2.0/hordelib/utils/cast.py
--rw-rw-rw-   0        0        0      218 2023-04-06 09:46:54.000000 hordelib-0.2.0/hordelib/utils/switch.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.506484 hordelib-0.2.0/hordelib.egg-info/
--rw-rw-rw-   0        0        0    47456 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2662 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      225 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-08 17:41:21.000000 hordelib-0.2.0/hordelib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.533487 hordelib-0.2.0/images/
--rw-rw-rw-   0        0        0    36815 2023-04-06 23:19:06.000000 hordelib-0.2.0/images/test_db0.jpg
--rw-rw-rw-   0        0        0  1474994 2023-04-08 09:16:11.000000 hordelib-0.2.0/images/test_inpaint.png
--rw-rw-rw-   0        0        0  1467500 2023-04-08 09:41:06.000000 hordelib-0.2.0/images/test_outpaint.png
--rw-rw-rw-   0        0        0     2369 2023-04-08 17:41:15.000000 hordelib-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       71 2023-04-03 21:13:26.000000 hordelib-0.2.0/pytest.ini
--rw-rw-rw-   0        0        0       73 2023-04-07 14:09:36.000000 hordelib-0.2.0/requirements.dev.txt
--rw-rw-rw-   0        0        0      348 2023-04-08 17:41:15.000000 hordelib-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 17:41:21.546485 hordelib-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-08 17:41:21.545487 hordelib-0.2.0/tests/
--rw-rw-rw-   0        0        0      180 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_img2img.py
--rw-rw-rw-   0        0        0     1107 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_img2img_hires.py
--rw-rw-rw-   0        0        0     1136 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_img2img_inpaint.py
--rw-rw-rw-   0        0        0     1181 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_img2img_outpaint.py
--rw-rw-rw-   0        0        0     1016 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_txt2img.py
--rw-rw-rw-   0        0        0     1021 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/run_txt2img_hires.py
--rw-rw-rw-   0        0        0      930 2023-04-08 10:50:44.000000 hordelib-0.2.0/tests/run_upscale.py
--rw-rw-rw-   0        0        0     1786 2023-04-08 09:21:29.000000 hordelib-0.2.0/tests/test_clip.py
--rw-rw-rw-   0        0        0     5948 2023-04-08 10:19:21.000000 hordelib-0.2.0/tests/test_comfy.py
--rw-rw-rw-   0        0        0     1550 2023-04-06 13:25:34.000000 hordelib-0.2.0/tests/test_comfy_install.py
--rw-rw-rw-   0        0        0    12444 2023-04-08 16:59:24.000000 hordelib-0.2.0/tests/test_horde_inference.py
--rw-rw-rw-   0        0        0     4410 2023-04-08 17:01:41.000000 hordelib-0.2.0/tests/test_horde_pp.py
--rw-rw-rw-   0        0        0     6230 2023-04-07 15:57:33.000000 hordelib-0.2.0/tests/test_inference.py
--rw-rw-rw-   0        0        0      382 2023-04-06 12:47:28.000000 hordelib-0.2.0/tests/test_initialisation.py
--rw-rw-rw-   0        0        0     3328 2023-04-07 11:33:18.000000 hordelib-0.2.0/tests/test_model_manager.py
--rw-rw-rw-   0        0        0     1587 2023-04-08 09:21:33.000000 hordelib-0.2.0/tests/test_safety_checker.py
--rw-rw-rw-   0        0        0     1058 2023-04-07 14:09:36.000000 hordelib-0.2.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.624515 hordelib-0.4.1/
+-rw-rw-rw-   0        0        0       88 2023-04-03 21:13:26.000000 hordelib-0.4.1/.flake8
+-rw-rw-rw-   0        0        0      162 2023-04-07 14:09:36.000000 hordelib-0.4.1/.git-blame-ignore-revs
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.277056 hordelib-0.4.1/.github/
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.320055 hordelib-0.4.1/.github/workflows/
+-rw-rw-rw-   0        0        0     2393 2023-04-10 21:35:23.000000 hordelib-0.4.1/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1222 2023-04-10 21:26:28.000000 hordelib-0.4.1/.github/workflows/tests.yaml
+-rw-rw-rw-   0        0        0     2277 2023-04-10 19:50:25.000000 hordelib-0.4.1/.gitignore
+-rw-rw-rw-   0        0        0     7674 2023-04-10 21:49:36.000000 hordelib-0.4.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35182 2023-04-05 20:05:31.000000 hordelib-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0    48014 2023-04-10 21:50:24.624515 hordelib-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6872 2023-04-10 19:50:25.000000 hordelib-0.4.1/README.md
+-rw-rw-rw-   0        0        0     1666 2023-04-06 23:36:10.000000 hordelib-0.4.1/build_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.336059 hordelib-0.4.1/hordelib/
+-rw-rw-rw-   0        0        0       94 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.354515 hordelib-0.4.1/hordelib/cache/
+-rw-rw-rw-   0        0        0       60 2023-04-03 21:13:26.000000 hordelib-0.4.1/hordelib/cache/__init__.py
+-rw-rw-rw-   0        0        0     8739 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/cache/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.357515 hordelib-0.4.1/hordelib/clip/
+-rw-rw-rw-   0        0        0      131 2023-04-03 21:13:26.000000 hordelib-0.4.1/hordelib/clip/__init__.py
+-rw-rw-rw-   0        0        0     2481 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/clip/bulk.py
+-rw-rw-rw-   0        0        0     1088 2023-04-03 21:13:26.000000 hordelib-0.4.1/hordelib/clip/coca.py
+-rw-rw-rw-   0        0        0     4681 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/clip/image.py
+-rw-rw-rw-   0        0        0    12260 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/clip/interrogate.py
+-rw-rw-rw-   0        0        0     3034 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/clip/text.py
+-rw-rw-rw-   0        0        0    13057 2023-04-10 21:49:36.000000 hordelib-0.4.1/hordelib/comfy_horde.py
+-rw-rw-rw-   0        0        0      592 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/config_path.py
+-rw-rw-rw-   0        0        0      570 2023-04-10 21:49:36.000000 hordelib-0.4.1/hordelib/consts.py
+-rw-rw-rw-   0        0        0    11159 2023-04-10 21:49:36.000000 hordelib-0.4.1/hordelib/horde.py
+-rw-rw-rw-   0        0        0      789 2023-04-08 16:59:24.000000 hordelib-0.4.1/hordelib/initialisation.py
+-rw-rw-rw-   0        0        0     1759 2023-04-09 17:44:13.000000 hordelib-0.4.1/hordelib/install_comfy.patch
+-rw-rw-rw-   0        0        0     4689 2023-04-09 17:44:13.000000 hordelib-0.4.1/hordelib/install_comfy.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.358514 hordelib-0.4.1/hordelib/model_database/
+-rw-rw-rw-   0        0        0      751 2023-04-08 22:24:37.000000 hordelib-0.4.1/hordelib/model_database/diffusers.json
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.377514 hordelib-0.4.1/hordelib/model_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.4.1/hordelib/model_manager/__init__.py
+-rw-rw-rw-   0        0        0     7823 2023-04-07 15:47:10.000000 hordelib-0.4.1/hordelib/model_manager/aitemplate.py
+-rw-rw-rw-   0        0        0    20533 2023-04-08 22:24:37.000000 hordelib-0.4.1/hordelib/model_manager/base.py
+-rw-rw-rw-   0        0        0     4195 2023-04-07 15:47:35.000000 hordelib-0.4.1/hordelib/model_manager/blip.py
+-rw-rw-rw-   0        0        0     6767 2023-04-07 15:47:41.000000 hordelib-0.4.1/hordelib/model_manager/clip.py
+-rw-rw-rw-   0        0        0     2858 2023-04-08 16:59:24.000000 hordelib-0.4.1/hordelib/model_manager/codeformer.py
+-rw-rw-rw-   0        0        0     2226 2023-04-07 15:47:53.000000 hordelib-0.4.1/hordelib/model_manager/compvis.py
+-rw-rw-rw-   0        0        0     3688 2023-04-10 21:49:36.000000 hordelib-0.4.1/hordelib/model_manager/controlnet.py
+-rw-rw-rw-   0        0        0     3094 2023-04-08 22:24:37.000000 hordelib-0.4.1/hordelib/model_manager/diffusers.py
+-rw-rw-rw-   0        0        0     2431 2023-04-07 15:48:06.000000 hordelib-0.4.1/hordelib/model_manager/esrgan.py
+-rw-rw-rw-   0        0        0     2409 2023-04-07 15:48:10.000000 hordelib-0.4.1/hordelib/model_manager/gfpgan.py
+-rw-rw-rw-   0        0        0    15731 2023-04-08 16:59:24.000000 hordelib-0.4.1/hordelib/model_manager/hyper.py
+-rw-rw-rw-   0        0        0     3380 2023-04-07 15:48:13.000000 hordelib-0.4.1/hordelib/model_manager/new.py
+-rw-rw-rw-   0        0        0     3553 2023-04-07 15:48:16.000000 hordelib-0.4.1/hordelib/model_manager/safety_checker.py
+-rw-rw-rw-   0        0        0     8699 2023-04-07 20:20:31.000000 hordelib-0.4.1/hordelib/model_manager/sdu.py
+-rw-rw-rw-   0        0        0     7282 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/model_manager/torch_hijack.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.385515 hordelib-0.4.1/hordelib/nodes/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.4.1/hordelib/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.389516 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-rw-rw-   0        0        0       39 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-rw-rw-   0        0        0    11556 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-rw-rw-   0        0        0     5835 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-rw-rw-   0        0        0    13176 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.390515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-rw-rw-   0        0        0      656 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.390515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-rw-rw-   0        0        0      196 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.391514 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-rw-rw-   0        0        0      665 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.391514 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-rw-rw-   0        0        0     6837 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+-rw-rw-rw-   0        0        0     1576 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/install.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.392515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-rw-rw-   0        0        0     4398 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.396515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-rw-rw-   0        0        0     1154 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-rw-rw-   0        0        0     6440 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-rw-rw-   0        0        0     9064 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-rw-rw-   0        0        0    23535 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-rw-rw-   0        0        0     1152 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-rw-rw-   0        0        0     2055 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-rw-rw-   0        0        0    17304 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.396515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-rw-rw-   0        0        0     1241 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.399516 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-rw-rw-   0        0        0     3178 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-rw-rw-   0        0        0    11036 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-rw-rw-   0        0        0     1718 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-rw-rw-   0        0        0    29583 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-rw-rw-   0        0        0     7558 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.401516 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-rw-rw-   0        0        0      137 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-rw-rw-   0        0        0     9520 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-rw-rw-   0        0        0     1084 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.404518 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-rw-rw-   0        0        0       84 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-rw-rw-   0        0        0     1578 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-rw-rw-   0        0        0     3309 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-rw-rw-   0        0        0     2280 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-rw-rw-   0        0        0     3215 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-rw-rw-   0        0        0     7698 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.406517 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-rw-rw-   0        0        0     1529 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-rw-rw-   0        0        0     5427 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.409515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-rw-rw-   0        0        0        0 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-rw-rw-   0        0        0     9584 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-rw-rw-   0        0        0     3263 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-rw-rw-   0        0        0     2785 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-rw-rw-   0        0        0     5334 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8103 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-rw-rw-   0        0        0    15116 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-rw-rw-   0        0        0     4771 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.410551 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-rw-rw-   0        0        0     1584 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.411515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-rw-rw-   0        0        0     9969 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-rw-   0        0        0     9454 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-rw-   0        0        0    24685 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.412515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-rw-rw-   0        0        0     7009 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.412515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-rw-rw-   0        0        0     4240 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.415515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-rw-rw-   0        0        0     2030 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-rw-rw-   0        0        0    11257 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-rw-rw-   0        0        0     3497 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-rw-rw-   0        0        0     8964 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-rw-rw-   0        0        0     7671 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.416514 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-rw-rw-   0        0        0     1518 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-rw-rw-   0        0        0    21070 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-rw-rw-   0        0        0      169 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.416514 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-rw-rw-   0        0        0     1197 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.283056 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.417514 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.422514 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-rw-rw-   0        0        0     1898 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-rw-rw-   0        0        0     1983 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-rw-rw-   0        0        0     1834 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-rw-rw-   0        0        0     1316 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-rw-rw-   0        0        0     1974 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-rw-rw-   0        0        0     1974 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-rw-rw-   0        0        0     2058 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-rw-rw-   0        0        0     2084 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-rw-rw-   0        0        0     1987 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-rw-rw-   0        0        0      270 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-rw-rw-   0        0        0     1976 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-rw-rw-   0        0        0      335 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.435517 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-rw-rw-   0        0        0     1392 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-rw-rw-   0        0        0     1346 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-rw-rw-   0        0        0     1302 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-rw-rw-   0        0        0     1145 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-rw-rw-   0        0        0     1305 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-rw-rw-   0        0        0     1317 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-rw-rw-   0        0        0     1549 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-rw-rw-   0        0        0     1389 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-rw-rw-   0        0        0     1346 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-rw-rw-   0        0        0     1362 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-rw-rw-   0        0        0     1376 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-rw-rw-   0        0        0     1483 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-rw-rw-   0        0        0     1818 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-rw-rw-   0        0        0     1698 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-rw-rw-   0        0        0     1330 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-rw-rw-   0        0        0     1563 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-rw-rw-   0        0        0     1092 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-rw-rw-   0        0        0     1012 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-rw-rw-   0        0        0     1372 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-rw-rw-   0        0        0      791 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-rw-rw-   0        0        0     1361 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-rw-rw-   0        0        0     2264 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-rw-rw-   0        0        0     1432 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-rw-rw-   0        0        0     1760 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-rw-rw-   0        0        0     1455 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-rw-rw-   0        0        0     1315 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-rw-rw-   0        0        0     1547 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-rw-rw-   0        0        0     1345 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-rw-rw-   0        0        0     1277 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.437518 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-rw-rw-   0        0        0      391 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-rw-rw-   0        0        0      388 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-rw-rw-   0        0        0      388 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-rw-rw-   0        0        0      388 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.284055 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.440517 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-rw-rw-   0        0        0     1353 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-rw-rw-   0        0        0      392 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-rw-rw-   0        0        0      328 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-rw-rw-   0        0        0     1354 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-rw-rw-   0        0        0     1377 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-rw-rw-   0        0        0     1377 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.441517 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-rw-rw-   0        0        0      367 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.441517 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-rw-rw-   0        0        0      137 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-rw-rw-   0        0        0     1879 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.444517 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-rw-rw-   0        0        0     2479 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-rw-rw-   0        0        0     2051 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.456028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-rw-rw-   0        0        0     1767 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-rw-rw-   0        0        0     2621 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-rw-rw-   0        0        0     4806 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-rw-rw-   0        0        0     1490 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-rw-rw-   0        0        0     2576 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-rw-rw-   0        0        0     8987 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-rw-rw-   0        0        0     5565 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-rw-rw-   0        0        0     4238 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-rw-rw-   0        0        0     2258 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-rw-rw-   0        0        0    16411 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-rw-rw-   0        0        0     1131 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-rw-rw-   0        0        0      680 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-rw-rw-   0        0        0    11318 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-rw-rw-   0        0        0     5340 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-rw-rw-   0        0        0     1163 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-rw-rw-   0        0        0     2575 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-rw-rw-   0        0        0      695 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-rw-rw-   0        0        0      598 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-rw-rw-   0        0        0      510 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-rw-rw-   0        0        0    25381 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-rw-rw-   0        0        0     2964 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-rw-rw-   0        0        0     7141 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-rw-rw-   0        0        0     1119 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-rw-rw-   0        0        0    10271 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.458027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-rw-rw-   0        0        0     1042 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-rw-rw-   0        0        0    22724 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-rw-rw-   0        0        0     1940 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-rw-rw-   0        0        0     2407 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-rw-rw-   0        0        0    26732 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-rw-rw-   0        0        0     6228 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.459028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-rw-rw-   0        0        0      274 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-rw-rw-   0        0        0     7440 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.461027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-rw-rw-   0        0        0      489 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-rw-rw-   0        0        0    43144 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.463028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-rw-rw-   0        0        0      285 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1023 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-rw-rw-   0        0        0     1104 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-rw-rw-   0        0        0      845 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-rw-rw-   0        0        0      689 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-rw-rw-   0        0        0     5671 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-rw-rw-   0        0        0     3555 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.466027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-rw-rw-   0        0        0     1753 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-rw-rw-   0        0        0    10213 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-rw-rw-   0        0        0    25924 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-rw-rw-   0        0        0     9851 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-rw-rw-   0        0        0     1475 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-rw-rw-   0        0        0    15427 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.467027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-rw-rw-   0        0        0      223 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-rw-rw-   0        0        0     3721 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-rw-rw-   0        0        0     5231 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.488028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-rw-rw-   0        0        0     4587 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-rw-rw-   0        0        0     4467 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-rw-rw-   0        0        0     1750 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-rw-rw-   0        0        0     2580 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-rw-rw-   0        0        0     3834 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-rw-rw-   0        0        0     1654 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-rw-rw-   0        0        0    10160 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-rw-rw-   0        0        0     3145 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-rw-rw-   0        0        0     1844 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-rw-rw-   0        0        0     4858 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-rw-rw-   0        0        0     6893 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-rw-rw-   0        0        0    16029 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-rw-rw-   0        0        0     7614 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-rw-rw-   0        0        0     1510 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-rw-rw-   0        0        0     6794 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-rw-rw-   0        0        0     2633 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-rw-rw-   0        0        0    10299 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-rw-rw-   0        0        0     1664 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-rw-rw-   0        0        0     8359 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-rw-rw-   0        0        0      923 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-rw-rw-   0        0        0     3073 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-rw-rw-   0        0        0     2676 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-rw-rw-   0        0        0     3872 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-rw-rw-   0        0        0     5552 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-rw-rw-   0        0        0    10877 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-rw-rw-   0        0        0    15617 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-rw-rw-   0        0        0    16675 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-rw-rw-   0        0        0     3188 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-rw-rw-   0        0        0    12648 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-rw-rw-   0        0        0     5374 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-rw-rw-   0        0        0     6261 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-rw-rw-   0        0        0     2865 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-rw-rw-   0        0        0     8742 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-rw-rw-   0        0        0     6611 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-rw-rw-   0        0        0     2603 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-rw-rw-   0        0        0     4391 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-rw-rw-   0        0        0     3067 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-rw-rw-   0        0        0     6012 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-rw-rw-   0        0        0     5336 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-rw-rw-   0        0        0    11567 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-rw-rw-   0        0        0     2215 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-rw-rw-   0        0        0     1566 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-rw-rw-   0        0        0     2209 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-rw-rw-   0        0        0    12155 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-rw-rw-   0        0        0     5418 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.493027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-rw-rw-   0        0        0      518 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-rw-rw-   0        0        0     2909 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-rw-rw-   0        0        0     3749 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-rw-rw-   0        0        0     2454 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-rw-rw-   0        0        0     4001 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-rw-rw-   0        0        0     5011 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-rw-rw-   0        0        0     2928 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-rw-rw-   0        0        0      361 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-rw-rw-   0        0        0     2366 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-rw-rw-   0        0        0      728 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.500028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-rw-rw-   0        0        0     2906 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-rw-rw-   0        0        0     7739 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-rw-rw-   0        0        0    21409 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-rw-rw-   0        0        0      690 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-rw-rw-   0        0        0    25864 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-rw-rw-   0        0        0     1993 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-rw-rw-   0        0        0     5559 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-rw-rw-   0        0        0     7773 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-rw-rw-   0        0        0    16215 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.508029 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-rw-rw-   0        0        0     1425 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-rw-rw-   0        0        0     7505 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-rw-rw-   0        0        0      280 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-rw-rw-   0        0        0     3688 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-rw-rw-   0        0        0    23041 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-rw-rw-   0        0        0     2874 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-rw-rw-   0        0        0      464 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.512028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-rw-rw-   0        0        0      537 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-rw-rw-   0        0        0     5617 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-rw-rw-   0        0        0     1819 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-rw-rw-   0        0        0     2916 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-rw-rw-   0        0        0     3159 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-rw-rw-   0        0        0     4516 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-rw-rw-   0        0        0     2155 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-rw-rw-   0        0        0    11003 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-rw-rw-   0        0        0     1750 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-rw-rw-   0        0        0    26725 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-rw-rw-   0        0        0      682 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-rw-rw-   0        0        0    21810 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-rw-rw-   0        0        0    22183 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-rw-rw-   0        0        0     8221 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-rw-rw-   0        0        0      867 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-rw-rw-   0        0        0      729 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-rw-rw-   0        0        0    11356 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-rw-rw-   0        0        0     1233 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.514028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-rw-rw-   0        0        0      379 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-rw-rw-   0        0        0    12115 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-rw-rw-   0        0        0     1658 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-rw-rw-   0        0        0     3050 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.521028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-rw-rw-   0        0        0     3984 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-rw-rw-   0        0        0    26993 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-rw-rw-   0        0        0     3525 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-rw-rw-   0        0        0     2133 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-rw-rw-   0        0        0     4096 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-rw-rw-   0        0        0    11824 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-rw-rw-   0        0        0      940 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-rw-rw-   0        0        0     3643 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-rw-rw-   0        0        0     3515 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-rw-rw-   0        0        0     7313 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-rw-rw-   0        0        0    11356 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-rw-rw-   0        0        0     4429 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-rw-rw-   0        0        0     3153 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-rw-rw-   0        0        0      839 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-rw-rw-   0        0        0     2763 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-rw-rw-   0        0        0     1212 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.523027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-rw-rw-   0        0        0      581 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-rw-rw-   0        0        0    10569 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-rw-rw-   0        0        0    10045 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-rw-rw-   0        0        0     5472 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.525027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-rw-rw-   0        0        0      347 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1453 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-rw-rw-   0        0        0     5318 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-rw-rw-   0        0        0     3543 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.526029 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-rw-rw-   0        0        0       99 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-rw-rw-   0        0        0    19716 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.292054 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.528027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-rw-rw-   0        0        0      390 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-rw-rw-   0        0        0     4970 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-rw-rw-   0        0        0     8589 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-rw-rw-   0        0        0     4256 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.528027 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-rw-rw-   0        0        0      129 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.530028 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-rw-rw-   0        0        0      309 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     7478 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-rw-rw-   0        0        0     4108 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-rw-rw-   0        0        0    13426 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.531029 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-rw-rw-   0        0        0      176 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.533032 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-rw-rw-   0        0        0      154 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-rw-rw-   0        0        0      296 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-rw-rw-   0        0        0     3231 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.534032 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-rw-rw-   0        0        0       58 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-rw-rw-   0        0        0      388 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.540032 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-rw-rw-   0        0        0      817 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-rw-rw-   0        0        0     5269 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-rw-rw-   0        0        0     6204 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-rw-rw-   0        0        0      808 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-rw-rw-   0        0        0     8753 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-rw-rw-   0        0        0    15366 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-rw-rw-   0        0        0     1549 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-rw-rw-   0        0        0      798 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-rw-rw-   0        0        0      774 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-rw-rw-   0        0        0     5305 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.543034 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-rw-rw-   0        0        0      829 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     1556 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-rw-rw-   0        0        0     9606 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-rw-rw-   0        0        0     6075 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-rw-rw-   0        0        0     5355 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-rw-rw-   0        0        0    31924 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-rw-rw-   0        0        0      788 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-rw-rw-   0        0        0     1159 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.544033 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-rw-rw-   0        0        0      501 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.549515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-rw-rw-   0        0        0      549 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-rw-rw-   0        0        0    13634 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-rw-rw-   0        0        0    14874 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-rw-rw-   0        0        0    21907 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-rw-rw-   0        0        0     7203 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-rw-rw-   0        0        0    10729 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-rw-rw-   0        0        0    10445 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-rw-rw-   0        0        0    25103 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-rw-rw-   0        0        0     5348 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-rw-rw-   0        0        0    18782 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-rw-rw-   0        0        0    18940 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-rw-rw-   0        0        0    18628 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-rw-rw-   0        0        0     1293 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.560515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-rw-rw-   0        0        0      997 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-rw-rw-   0        0        0     9460 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-rw-rw-   0        0        0     5772 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-rw-rw-   0        0        0     3608 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-rw-rw-   0        0        0     2408 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-rw-rw-   0        0        0     1366 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-rw-rw-   0        0        0     5805 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-rw-rw-   0        0        0     9558 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-rw-rw-   0        0        0     5165 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-rw-rw-   0        0        0     4743 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-rw-rw-   0        0        0     5985 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-rw-rw-   0        0        0     7013 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-rw-rw-   0        0        0     2919 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-rw-rw-   0        0        0     2532 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-rw-rw-   0        0        0     1679 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-rw-rw-   0        0        0     3251 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-rw-rw-   0        0        0     1647 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-rw-rw-   0        0        0     4488 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-rw-rw-   0        0        0    15187 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-rw-rw-   0        0        0     7803 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-rw-rw-   0        0        0     3495 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-rw-rw-   0        0        0     3670 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-rw-rw-   0        0        0     2096 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-rw-rw-   0        0        0     4180 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.563515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-rw-rw-   0        0        0      541 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-rw-rw-   0        0        0     3048 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-rw-rw-   0        0        0     7635 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-rw-rw-   0        0        0     4358 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-rw-rw-   0        0        0    11743 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-rw-rw-   0        0        0     3860 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.564515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-rw-rw-   0        0        0      106 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-rw-rw-   0        0        0     9392 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-rw-rw-   0        0        0     2545 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.566515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-rw-rw-   0        0        0      212 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-rw-rw-   0        0        0    10713 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-rw-rw-   0        0        0     3848 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-rw-rw-   0        0        0    11684 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.570515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-rw-rw-   0        0        0      515 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-rw-rw-   0        0        0     7254 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-rw-rw-   0        0        0     1258 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-rw-rw-   0        0        0     3450 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-rw-rw-   0        0        0     2250 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-rw-rw-   0        0        0     6325 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-rw-rw-   0        0        0     4110 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-rw-rw-   0        0        0     2389 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.572515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-rw-rw-   0        0        0      120 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-rw-rw-   0        0        0     2862 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-rw-rw-   0        0        0     1877 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.573515 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-rw-rw-   0        0        0      123 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-rw-rw-   0        0        0      585 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-rw-rw-   0        0        0      967 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-rw-rw-   0        0        0     5096 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.574515 hordelib-0.4.1/hordelib/nodes/facerestore/
+-rw-rw-rw-   0        0        0     7618 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.574515 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/
+-rw-rw-rw-   0        0        0        0 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.576516 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/
+-rw-rw-rw-   0        0        0     4775 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-rw-rw-   0        0        0     8160 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-rw-rw-   0        0        0     8426 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.577516 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-rw-rw-   0        0        0    14360 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-rw-rw-   0        0        0     6477 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-rw-rw-   0        0        0    16873 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.578515 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-rw-rw-   0        0        0        0 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-rw-rw-   0        0        0     6601 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.581515 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-rw-rw-   0        0        0        0 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-rw-rw-   0        0        0    12840 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-rw-rw-   0        0        0     1885 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-rw-rw-   0        0        0    10919 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-rw-rw-   0        0        0     1390 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-rw-rw-   0        0        0     1380 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.583515 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-rw-rw-   0        0        0      472 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-rw-rw-   0        0        0     1550 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-rw-rw-   0        0        0      235 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-rw-rw-   0        0        0    10619 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-rw-rw-   0        0        0     1415 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.585515 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/parsing/
+-rw-rw-rw-   0        0        0     1051 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-rw-rw-   0        0        0     5330 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-rw-rw-   0        0        0     6671 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-rw-rw-   0        0        0     2426 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.587516 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/utils/
+-rw-rw-rw-   0        0        0      396 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-rw-rw-   0        0        0    23863 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-rw-rw-   0        0        0    10502 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-rw-rw-   0        0        0     5443 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-rw-rw-   0        0        0     1449 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/nodes/node_clip_similarities.py
+-rw-rw-rw-   0        0        0     1219 2023-04-10 21:49:36.000000 hordelib-0.4.1/hordelib/nodes/node_controlnet_model_loader.py
+-rw-rw-rw-   0        0        0      947 2023-04-09 10:33:42.000000 hordelib-0.4.1/hordelib/nodes/node_image_loader.py
+-rw-rw-rw-   0        0        0     1634 2023-04-06 14:10:46.000000 hordelib-0.4.1/hordelib/nodes/node_image_output.py
+-rw-rw-rw-   0        0        0     1244 2023-04-08 16:59:24.000000 hordelib-0.4.1/hordelib/nodes/node_model_loader.py
+-rw-rw-rw-   0        0        0     1065 2023-04-08 16:59:24.000000 hordelib-0.4.1/hordelib/nodes/node_upscale_model_loader.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.590515 hordelib-0.4.1/hordelib/pipeline_designs/
+-rw-rw-rw-   0        0        0    17076 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-rw-rw-   0        0        0     3050 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-rw-rw-   0        0        0     2979 2023-04-09 10:02:46.000000 hordelib-0.4.1/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-rw-rw-   0        0        0     8778 2023-04-09 10:02:46.000000 hordelib-0.4.1/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-rw-rw-   0        0        0    12056 2023-04-09 10:02:46.000000 hordelib-0.4.1/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-rw-rw-   0        0        0     9007 2023-04-09 10:02:46.000000 hordelib-0.4.1/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.593515 hordelib-0.4.1/hordelib/pipelines/
+-rw-rw-rw-   0        0        0     4666 2023-04-10 10:47:00.000000 hordelib-0.4.1/hordelib/pipelines/pipeline_controlnet.json
+-rw-rw-rw-   0        0        0      854 2023-04-10 12:29:19.000000 hordelib-0.4.1/hordelib/pipelines/pipeline_image_facefix.json
+-rw-rw-rw-   0        0        0      802 2023-04-09 10:02:46.000000 hordelib-0.4.1/hordelib/pipelines/pipeline_image_upscale.json
+-rw-rw-rw-   0        0        0     2470 2023-04-09 10:02:46.000000 hordelib-0.4.1/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-rw-rw-   0        0        0     3507 2023-04-09 10:02:46.000000 hordelib-0.4.1/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-rw-rw-   0        0        0     2561 2023-04-09 10:02:46.000000 hordelib-0.4.1/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-rw-rw-   0        0        0     1149 2023-04-09 17:44:13.000000 hordelib-0.4.1/hordelib/run_comfyui.py
+-rw-rw-rw-   0        0        0      717 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/safety_checker.py
+-rw-rw-rw-   0        0        0      505 2023-04-06 09:46:54.000000 hordelib-0.4.1/hordelib/settings.py
+-rw-rw-rw-   0        0        0      926 2023-04-07 10:32:48.000000 hordelib-0.4.1/hordelib/shared_model_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.594515 hordelib-0.4.1/hordelib/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:13:26.000000 hordelib-0.4.1/hordelib/utils/__init__.py
+-rw-rw-rw-   0        0        0      655 2023-04-07 14:09:36.000000 hordelib-0.4.1/hordelib/utils/cast.py
+-rw-rw-rw-   0        0        0      218 2023-04-06 09:46:54.000000 hordelib-0.4.1/hordelib/utils/switch.py
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.353516 hordelib-0.4.1/hordelib.egg-info/
+-rw-rw-rw-   0        0        0    48014 2023-04-10 21:50:23.000000 hordelib-0.4.1/hordelib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    37715 2023-04-10 21:50:24.000000 hordelib-0.4.1/hordelib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 21:50:23.000000 hordelib-0.4.1/hordelib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      397 2023-04-10 21:50:23.000000 hordelib-0.4.1/hordelib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-10 21:50:23.000000 hordelib-0.4.1/hordelib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.599515 hordelib-0.4.1/images/
+-rw-rw-rw-   0        0        0    36815 2023-04-06 23:19:06.000000 hordelib-0.4.1/images/test_db0.jpg
+-rw-rw-rw-   0        0        0   538159 2023-04-10 12:29:19.000000 hordelib-0.4.1/images/test_facefix.png
+-rw-rw-rw-   0        0        0  1474994 2023-04-08 09:16:11.000000 hordelib-0.4.1/images/test_inpaint.png
+-rw-rw-rw-   0        0        0   411844 2023-04-10 10:47:00.000000 hordelib-0.4.1/images/test_inpaint_alpha.png
+-rw-rw-rw-   0        0        0    11886 2023-04-10 10:47:00.000000 hordelib-0.4.1/images/test_inpaint_mask.png
+-rw-rw-rw-   0        0        0   407128 2023-04-10 10:47:00.000000 hordelib-0.4.1/images/test_inpaint_original.png
+-rw-rw-rw-   0        0        0  1467500 2023-04-08 09:41:06.000000 hordelib-0.4.1/images/test_outpaint.png
+-rw-rw-rw-   0        0        0     2590 2023-04-10 21:50:17.000000 hordelib-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       73 2023-04-07 14:09:36.000000 hordelib-0.4.1/requirements.dev.txt
+-rw-rw-rw-   0        0        0      590 2023-04-10 21:50:17.000000 hordelib-0.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 21:50:24.624515 hordelib-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 21:50:24.623515 hordelib-0.4.1/tests/
+-rw-rw-rw-   0        0        0      180 2023-04-08 18:58:50.000000 hordelib-0.4.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2672 2023-04-10 19:50:25.000000 hordelib-0.4.1/tests/make_index.py
+-rw-rw-rw-   0        0        0     1392 2023-04-10 10:47:00.000000 hordelib-0.4.1/tests/run_controlnet.py
+-rw-rw-rw-   0        0        0      942 2023-04-10 12:29:19.000000 hordelib-0.4.1/tests/run_facefix.py
+-rw-rw-rw-   0        0        0     1106 2023-04-10 11:04:35.000000 hordelib-0.4.1/tests/run_img2img.py
+-rw-rw-rw-   0        0        0     1119 2023-04-10 11:04:35.000000 hordelib-0.4.1/tests/run_img2img_hires.py
+-rw-rw-rw-   0        0        0     1160 2023-04-10 11:04:35.000000 hordelib-0.4.1/tests/run_img2img_inpaint.py
+-rw-rw-rw-   0        0        0     1207 2023-04-10 11:04:35.000000 hordelib-0.4.1/tests/run_img2img_outpaint.py
+-rw-rw-rw-   0        0        0     1191 2023-04-10 11:04:35.000000 hordelib-0.4.1/tests/run_inpainting.py
+-rw-rw-rw-   0        0        0     1033 2023-04-10 20:16:01.000000 hordelib-0.4.1/tests/run_txt2img.py
+-rw-rw-rw-   0        0        0     1044 2023-04-10 11:04:35.000000 hordelib-0.4.1/tests/run_txt2img_hires.py
+-rw-rw-rw-   0        0        0      950 2023-04-10 11:04:35.000000 hordelib-0.4.1/tests/run_upscale.py
+-rw-rw-rw-   0        0        0     1786 2023-04-08 09:21:29.000000 hordelib-0.4.1/tests/test_clip.py
+-rw-rw-rw-   0        0        0     5859 2023-04-10 10:47:00.000000 hordelib-0.4.1/tests/test_comfy.py
+-rw-rw-rw-   0        0        0     1550 2023-04-09 09:13:38.000000 hordelib-0.4.1/tests/test_comfy_install.py
+-rw-rw-rw-   0        0        0     2027 2023-04-10 17:03:35.000000 hordelib-0.4.1/tests/test_cuda.py
+-rw-rw-rw-   0        0        0    12437 2023-04-10 20:43:29.000000 hordelib-0.4.1/tests/test_horde_inference.py
+-rw-rw-rw-   0        0        0     2608 2023-04-10 21:49:36.000000 hordelib-0.4.1/tests/test_horde_inference_controlnet.py
+-rw-rw-rw-   0        0        0     6747 2023-04-10 10:47:00.000000 hordelib-0.4.1/tests/test_horde_inference_img2img.py
+-rw-rw-rw-   0        0        0     2004 2023-04-10 19:50:25.000000 hordelib-0.4.1/tests/test_horde_inference_painting.py
+-rw-rw-rw-   0        0        0     5063 2023-04-10 12:29:19.000000 hordelib-0.4.1/tests/test_horde_pp.py
+-rw-rw-rw-   0        0        0     6306 2023-04-10 11:04:35.000000 hordelib-0.4.1/tests/test_inference.py
+-rw-rw-rw-   0        0        0      382 2023-04-06 12:47:28.000000 hordelib-0.4.1/tests/test_initialisation.py
+-rw-rw-rw-   0        0        0     3555 2023-04-08 22:24:37.000000 hordelib-0.4.1/tests/test_model_manager.py
+-rw-rw-rw-   0        0        0     1587 2023-04-08 09:21:33.000000 hordelib-0.4.1/tests/test_safety_checker.py
+-rw-rw-rw-   0        0        0     1329 2023-04-10 10:47:00.000000 hordelib-0.4.1/tox.ini
```

### Comparing `hordelib-0.2.0/.github/workflows/pypi.yml` & `hordelib-0.4.1/.github/workflows/pypi.yml`

 * *Files 12% similar despite different names*

```diff
@@ -26,40 +26,41 @@
       if: ${{ steps.release.outputs.version != '' }}
       uses: heinrichreimer/github-changelog-generator-action@v2.3
       with:
         token: ${{ secrets.GITHUB_TOKEN }}
     - name: "💾 Commit new version"
       if: ${{ steps.release.outputs.version != '' }}
       run: |
-          sed -i 's/VERSION = ".*"/VERSION = "${{ steps.release.outputs.version }}"/g' ./hordelib/consts.py
+          sed -i 's/^VERSION = ".*"/VERSION = "${{ steps.release.outputs.version }}"/g' ./hordelib/consts.py
           git config user.email github-actions@github.com
           git config user.name github-actions
-          git commit -am 'version incremented'
+          git commit -am 'build: version bump'
           git push
-    - name: "🐍 Set up Python 3.10"
-      if: ${{ steps.release.outputs.version != '' }}
-      uses: actions/setup-python@v3
-      with:
-        python-version: "3.10"
-    - name: "🛠 Install pypa/build"
-      if: ${{ steps.release.outputs.version != '' }}
-      run: >-
-        python -m
-        pip install
-        build
-        --user
-    - name: "🔧 Build a binary wheel and a source tarball"
-      if: ${{ steps.release.outputs.version != '' }}
-      run: >-
-        python build_helper.py
-    - name: "📦 Publish distribution to PyPI"
-      if: ${{ steps.release.outputs.version != '' }}
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        password: ${{ secrets.PYPI_API_TOKEN }}
-    # TODO: Once we make it official
+    ## FIXME: Disabled because build_helper.py is not working as expected yet
+    # - name: "🐍 Set up Python 3.10"
+    #   if: ${{ steps.release.outputs.version != '' }}
+    #   uses: actions/setup-python@v3
+    #   with:
+    #     python-version: "3.10"
+    # - name: "🛠 Install pypa/build"
+    #   if: ${{ steps.release.outputs.version != '' }}
+    #   run: >-
+    #     python -m
+    #     pip install
+    #     build
+    #     --user
+    # - name: "🔧 Build a binary wheel and a source tarball"
+    #   if: ${{ steps.release.outputs.version != '' }}
+    #   run: >-
+    #     python build_helper.py
+    # - name: "📦 Publish distribution to PyPI"
+    #   if: ${{ steps.release.outputs.version != '' }}
+    #   uses: pypa/gh-action-pypi-publish@release/v1
+    #   with:
+    #     password: ${{ secrets.PYPI_API_TOKEN }}
+    ## TODO: Once we make it official
     # - name: "Inform with Discord Webhook"
     #   if: ${{ steps.release.outputs.version != '' }}
     #   uses: tsickert/discord-webhook@v5.3.0
     #   with:
     #     webhook-url: ${{ secrets.DISCORD_WEBHOOK_URL }}
     #     content: "New version of hordelib has been published to pypi: ${{ steps.release.outputs.version }}"
```

### Comparing `hordelib-0.2.0/.gitignore` & `hordelib-0.4.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -140,10 +140,16 @@
 ComfyUI
 model.ckpt
 coverage.lcov
 images/pip*.png
 images/test.png
 images/hor*.png
 images/hor*.webp
+images/pip*.webp
+images/test.webp
+images/run_*
 comfy-prompt*.json
+images/index.html
 
-.vscode
+.vscode
+*.ckpt
+*.pth
```

### Comparing `hordelib-0.2.0/LICENSE` & `hordelib-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/PKG-INFO` & `hordelib-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.2.0
+Version: 0.4.1
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -672,21 +672,29 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: <3.11,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hordelib
 
-`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed in ComfyUI. `hordelib` and ComfyUI are licensed under the terms of the GNU General Public License.
+[![PyPI version](https://badge.fury.io/py/hordelib.svg)](https://badge.fury.io/py/hordelib)
+[![Downloads](https://pepy.tech/badge/hordelib)](https://pepy.tech/project/hordelib)
+[![Build](https://github.com/jug-dev/hordelib/actions/workflows/tests.yaml/badge.svg)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
+
+![GitHub license](https://img.shields.io/github/license/jug-dev/hordelib)
+
+`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of this project can be found in the AI Horde Discord server: https://discord.gg/3DxrhksKznb
 
+NOTE: This project is in early development and is not yet in use by Stable Horde.
+
 ## Purpose
 
-The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically, in a manner ultimately suitable for use in stable horde.
+The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
 If being installed from pypi, use a requirements file of the form:
 ```
 --extra-index-url https://download.pytorch.org/whl/cu117
 hordelib
@@ -720,26 +728,30 @@
     "seed": 123456789,
     "height": 512,
     "width": 512,
     "karras": True,
     "tiling": False,
     "hires_fix": False,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "an ancient llamia monster",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
 }
 pil_image = generate.basic_inference(data)
 pil_image.save("test.png")
 ```
 
+Note that `hordelib.initialise()` will erase all command line arguments from argv. So make sure you parse them before you call that.
+
+See `tests/run_*.py` for more standalone examples.
+
 ## Development
 
 Requirements:
 - `git` (install git)
 - `tox` (`pip install tox`)
 - Set the environmental variable `AIWORKER_CACHE_HOME` to point to a model directory.
 
@@ -761,15 +773,15 @@
 
 ### Running the Tests
 
 Simply execute: `tox` (or `tox -q` for less noisy output)
 
 This will take a while the first time as it installs all the dependencies.
 
-If the tests run successfully images will be produced in the project with the name of each pipeline, for example, `pipeline_stable_diffusion.png` and likely some other .png files too.
+If the tests run successfully images will be produced in the `images/` folder.
 
 #### Running a specific test file
 
 `tox -- -k <filename>` for example `tox -- -k test_initialisation`
 
 ### Directory Structure
 
@@ -826,15 +838,18 @@
 1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
 Now ComfyUI is pinned to a new version.
 
 ### ComfyUI Patching
 
-It may be that we need to patch the ComfyUI source code. Currently this optional and only used for development helpers. However, the mechanisms to patch ComfyUI source code at runtime are also already in place.
+We need to patch the ComfyUI source code. It's only a small patch to:
+
+1. Allow ComfyUI to find our custom nodes without copying files and folder around.
+2. Allow make ComfyUI output some handy JSON we need for development purposes.
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
 
 Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
```

### Comparing `hordelib-0.2.0/README.md` & `hordelib-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 # hordelib
 
-`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed in ComfyUI. `hordelib` and ComfyUI are licensed under the terms of the GNU General Public License.
+[![PyPI version](https://badge.fury.io/py/hordelib.svg)](https://badge.fury.io/py/hordelib)
+[![Downloads](https://pepy.tech/badge/hordelib)](https://pepy.tech/project/hordelib)
+[![Build](https://github.com/jug-dev/hordelib/actions/workflows/tests.yaml/badge.svg)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
+
+![GitHub license](https://img.shields.io/github/license/jug-dev/hordelib)
+
+`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of this project can be found in the AI Horde Discord server: https://discord.gg/3DxrhksKznb
 
+NOTE: This project is in early development and is not yet in use by Stable Horde.
+
 ## Purpose
 
-The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically, in a manner ultimately suitable for use in stable horde.
+The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
 If being installed from pypi, use a requirements file of the form:
 ```
 --extra-index-url https://download.pytorch.org/whl/cu117
 hordelib
@@ -44,26 +52,30 @@
     "seed": 123456789,
     "height": 512,
     "width": 512,
     "karras": True,
     "tiling": False,
     "hires_fix": False,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "an ancient llamia monster",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
 }
 pil_image = generate.basic_inference(data)
 pil_image.save("test.png")
 ```
 
+Note that `hordelib.initialise()` will erase all command line arguments from argv. So make sure you parse them before you call that.
+
+See `tests/run_*.py` for more standalone examples.
+
 ## Development
 
 Requirements:
 - `git` (install git)
 - `tox` (`pip install tox`)
 - Set the environmental variable `AIWORKER_CACHE_HOME` to point to a model directory.
 
@@ -85,15 +97,15 @@
 
 ### Running the Tests
 
 Simply execute: `tox` (or `tox -q` for less noisy output)
 
 This will take a while the first time as it installs all the dependencies.
 
-If the tests run successfully images will be produced in the project with the name of each pipeline, for example, `pipeline_stable_diffusion.png` and likely some other .png files too.
+If the tests run successfully images will be produced in the `images/` folder.
 
 #### Running a specific test file
 
 `tox -- -k <filename>` for example `tox -- -k test_initialisation`
 
 ### Directory Structure
 
@@ -150,15 +162,18 @@
 1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
 Now ComfyUI is pinned to a new version.
 
 ### ComfyUI Patching
 
-It may be that we need to patch the ComfyUI source code. Currently this optional and only used for development helpers. However, the mechanisms to patch ComfyUI source code at runtime are also already in place.
+We need to patch the ComfyUI source code. It's only a small patch to:
+
+1. Allow ComfyUI to find our custom nodes without copying files and folder around.
+2. Allow make ComfyUI output some handy JSON we need for development purposes.
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
 
 Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
```

### Comparing `hordelib-0.2.0/build_helper.py` & `hordelib-0.4.1/build_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/cache/cache.py` & `hordelib-0.4.1/hordelib/cache/cache.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/clip/bulk.py` & `hordelib-0.4.1/hordelib/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/clip/coca.py` & `hordelib-0.4.1/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/clip/image.py` & `hordelib-0.4.1/hordelib/clip/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/clip/interrogate.py` & `hordelib-0.4.1/hordelib/clip/interrogate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/clip/text.py` & `hordelib-0.4.1/hordelib/clip/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/comfy_horde.py` & `hordelib-0.4.1/hordelib/comfy_horde.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,95 +2,72 @@
 # Wrapper around comfy to allow usage by the horde worker.
 import copy
 import glob
 import json
 import os
 import re
 from io import BytesIO
+from pprint import pformat
 
 from loguru import logger
 from PIL import Image
 
 from hordelib.config_path import get_comfyui_path
 
 # Do not change the order of these imports
-# fmt: off
+# isort: off
 import execution
-from comfy.sd import load_checkpoint_guess_config
+from comfy.sd import load_checkpoint_guess_config, load_controlnet
 from comfy.utils import load_torch_file
 from comfy_extras.chainner_models import model_loading
-# fmt: on
+
+# isort: on
 
 
 class Comfy_Horde:
     """Handles horde-specific behavior against ComfyUI."""
 
     # We save pipelines from the ComfyUI GUI. This is very convenient as it
-    # makes it super easy to load and edit them in the future. However standard
-    # ComfyUI's GUI doesn't know about our custom nodes, so we allow the pipeline
+    # makes it super easy to load and edit them in the future. We allow the pipeline
     # design with standard nodes, then at runtime we dynamically replace these
-    # node types with our own where we need to.
+    # node types with our own where we need to. This allows easy previewing in ComfyUI
+    # which our custom nodes don't allow.
     NODE_REPLACEMENTS = {
         "CheckpointLoaderSimple": "HordeCheckpointLoader",
         "UpscaleModelLoader": "HordeUpscaleModelLoader",
         "SaveImage": "HordeImageOutput",
         "LoadImage": "HordeImageLoader",
+        "DiffControlNetLoader": "HordeDiffControlNetLoader",
     }
 
     # We may wish some ComfyUI standard nodes had different names for consistency. Here
     # we can dynamically rename some node input parameter names.
     NODE_PARAMETER_REPLACEMENTS = {
         "HordeCheckpointLoader": {
             # We name this "model_name" as then we can use the same generic code in our model loaders
             "ckpt_name": "model_name"
         }
     }
 
     def __init__(self) -> None:
         self.client_id = None  # used for receiving comfyUI async events
         self.pipelines = {}
-        self.unit_testing = os.getenv("HORDELIB_TESTING", "")
 
         # Load our pipelines
         self._load_pipelines()
 
     def _this_dir(self, filename: str, subdir="") -> str:
         target_dir = os.path.dirname(os.path.realpath(__file__))
         if subdir:
             target_dir = os.path.join(target_dir, subdir)
         return os.path.join(target_dir, filename)
 
-    def _load_node(self, filename: str) -> None:
-        try:
-            execution.nodes.load_custom_node(self._this_dir(filename, subdir="nodes"))
-        except Exception:
-            logger.error(f"Failed to load custom pipeline node: {filename}")
-            return
-        logger.debug(f"Loaded custom pipeline node: {filename}")
-
     def _load_custom_nodes(self) -> None:
-        # Load standard nodes stored in odd locations first
-        self._load_extra_nodes()
-        # Now load our own nodes
-        files = glob.glob(self._this_dir("node_*.py", subdir="nodes"))
-        for file in files:
-            self._load_node(os.path.basename(file))
-
-    def _load_comfy_node(self, filename: str) -> None:
-        try:
-            pathname = os.path.join(get_comfyui_path(), "comfy_extras", filename)
-            execution.nodes.load_custom_node(pathname)
-        except Exception:
-            logger.error(f"Failed to load comfy extra node: {filename}")
-            return
-        logger.debug(f"Loaded comfy extra node: {filename}")
-
-    # Load the comfy nodes that comfy stores in a different location from it's other nodes...
-    def _load_extra_nodes(self) -> None:
-        self._load_comfy_node("nodes_upscale_model.py")
+        execution.nodes.init_custom_nodes()
+        execution.nodes.load_custom_nodes(self._this_dir("nodes"))
 
     def _fix_pipeline_types(self, data: dict) -> dict:
         # We have a list of nodes and each node has a class type, which we may want to change
         for nodename, node in data.items():
             if ("class_type" in node) and (
                 node["class_type"] in Comfy_Horde.NODE_REPLACEMENTS
             ):
@@ -199,43 +176,59 @@
         return loaded_count
 
     # Inject parameters into a pre-configured pipeline
     # We allow "inputs" to be missing from the key name, if it is we insert it.
     def _set(self, dct, **kwargs) -> None:
         for key, value in kwargs.items():
             keys = key.split(".")
+            skip = False
             if "inputs" not in keys:
                 keys.insert(1, "inputs")
             current = dct
 
             for k in keys[:-1]:
                 if k not in current:
-                    logger.error(f"Attempt to set unknown pipeline parameter {key}")
+                    logger.warning(f"Attempt to set unknown pipeline parameter {key}")
+                    skip = True
                     break
 
                 current = current[k]
 
-            current[keys[-1]] = value
+            if not skip:
+                if not current.get(keys[-1]):
+                    logger.warning(
+                        f"Attempt to set parameter CREATED parameter '{key}'"
+                    )
+                current[keys[-1]] = value
 
     # Connect the named input to the named node (output).
     # Used for dynamic switching of pipeline graphs
     @classmethod
     def reconnect_input(cls, dct, input, output):
         logger.debug(f"Request to reconnect input {input} to output {output}")
+
+        # First check the output even exists
+        if output not in dct.keys():
+            logger.error(
+                f"Can not reconnect input {input} to {output} as {output} does not exist"
+            )
+            return None
+
         keys = input.split(".")
         if "inputs" not in keys:
             keys.insert(1, "inputs")
         current = dct
         for k in keys:
             if k not in current:
                 logger.error(f"Attempt to reconnect unknown input {input}")
                 return None
 
             current = current[k]
 
+        logger.debug(f"Request completed to reconnect input {input} to output {output}")
         current[0] = output
         return True
 
     # This is the callback handler for comfy async events. We only use it for debugging.
     def send_sync(self, p1, p2, p3):
         logger.debug(f"{p1}, {p2}, {p3}")
 
@@ -260,34 +253,44 @@
             params["model_loader.model_manager"] = SharedModelManager
 
         # If we have a source image, use that rather than noise (i.e. img2img)
         # XXX This probably shouldn't be here. But for the moment, it works.
         if "image_loader.image" in params:
             self.reconnect_input(pipeline, "sampler.latent_image", "vae_encode")
 
+        # XXX This shouldn't be here either, but it's not clear to me yet where the
+        # XXX correct place for dynamic connection of nodes is. Need to do a few more
+        # XXX pipelines to see.
+        if "control_type" in params:
+            # Inject control net model manager
+            if "controlnet_model_loader.model_manager" not in params:
+                logger.debug("Injecting controlnet model manager")
+                params["controlnet_model_loader.model_manager"] = SharedModelManager
+            # Connect to the correct pre-processor node
+            self.reconnect_input(
+                pipeline, "controlnet_apply.image", params["control_type"]
+            )
+
         # Set the pipeline parameters
         self._set(pipeline, **params)
 
-        # Fake it!
-        if self.unit_testing:
-            img = Image.new("RGB", (64, 64), (0, 0, 0))
-            byte_stream = BytesIO()
-            img.save(byte_stream, format="PNG", compress_level=4)
-            byte_stream.seek(0)
-
-            return {
-                "output_image": {"images": [{"imagedata": byte_stream, "type": "PNG"}]},
-            }
-
         # Run it!
         inference = execution.PromptExecutor(self)
         # Load our custom nodes
         self._load_custom_nodes()
+
+        # This is useful for dumping the entire pipeline to the terminal when
+        # developing and debugging new pipelines. A badly structured pipeline
+        # file just results in a cryptic error from comfy
+        pretty_pipeline = pformat(pipeline)
+        if False:  # This isn't here Tazlin :)
+            logger.error(pretty_pipeline)
+
         # The client_id parameter here is just so we receive comfy callbacks for debugging.
-        # We essential pretend we are a web client and want async callbacks.
+        # We pretend we are a web client and want async callbacks.
         inference.execute(pipeline, extra_data={"client_id": 1})
 
         return inference.outputs
 
     # Run a pipeline that returns an image in pixel space
     def run_image_pipeline(self, pipeline_name: str, params: dict) -> list[dict] | None:
         # From the horde point of view, let us assume the output we are interested in
```

### Comparing `hordelib-0.2.0/hordelib/config_path.py` & `hordelib-0.4.1/hordelib/config_path.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,7 +12,8 @@
     """Returns the path to ComfyUI that hordelib installs and manages."""
     return os.path.join(os.path.dirname(get_hordelib_path()), "ComfyUI")
 
 
 def set_system_path():
     """Adds ComfyUI to the python path, as it is not a proper library."""
     sys.path.append(get_comfyui_path())
+    sys.path.append(os.path.join(get_hordelib_path(), "nodes"))
```

### Comparing `hordelib-0.2.0/hordelib/consts.py` & `hordelib-0.4.1/hordelib/consts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # consts.py
 
 # hordelib version
-VERSION = "0.2.0"
+VERSION = "v0.4.1"
 
 # ComfyUI exact version we need
 COMFYUI_VERSION = "ebd7f9bf80213a44a8e2cadc75875a4b980991e5"
 
 # Default model managers to load
 DEFAULT_MODEL_MANAGERS = {
     "blip": True,
```

### Comparing `hordelib-0.2.0/hordelib/horde.py` & `hordelib-0.4.1/hordelib/horde.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         "k_dpm_adaptive": "dpm_adaptive",
         "k_dpmpp_2s_a": "dpmpp_2s_ancestral",
         "k_dpmpp_sde": "dpmpp_sde",
         "k_dpmpp_2m": "dpmpp_2m",
         "ddim": "ddim",
         "uni_pc": "uni_pc",
         "uni_pc_bh2": "uni_pc_bh2",
-        "plms": "<not supported>",
+        "plms": "euler",
     }
 
     # Horde to tex2img parameter mapping
     # XXX Items mapped to None are ignored for now
     BASIC_INFERENCE_PARAMS = {
         "sampler_name": "sampler.sampler_name",
         "cfg_scale": "sampler.cfg",
@@ -37,26 +37,47 @@
         "seed": "sampler.seed",
         "height": "empty_latent_image.height",
         "width": "empty_latent_image.width",
         # "karras": Handled below
         "tiling": None,
         # "hires_fix": Handled below
         "clip_skip": "clip_skip.stop_at_clip_layer",
-        "control_type": None,
+        # "control_type": Handled below
         "image_is_control": None,
         "return_control_map": None,
         # "prompt": Handled below
         "ddim_steps": "sampler.steps",
         "n_iter": "empty_latent_image.batch_size",
         "model": "model_loader.model_name",
         "source_image": "image_loader.image",
         "source_mask": None,
         "source_processing": "source_processing",
     }
 
+    # Horde names on the left, our node names on the right
+    # We use this to dynamically route the image through the
+    # right node by reconnect inputs.
+    CONTROLNET_IMAGE_PREPROCESSOR_MAP = {
+        "canny": "canny",
+        "hed": "hed",
+        "depth": "depth",
+        "normal": "normal",
+        "openpose": "openpose",
+        "seg": "seg",
+        "scribble": "scribble",
+        "fakescribbles": "fakescribble",
+        "hough": "mlsd",
+        # "<unused>": "MiDaS-DepthMapPreprocessor",
+        # "<unused>": "MediaPipe-HandPosePreprocessor",
+        # "<unused>": "MediaPipe-FaceMeshPreprocessor",
+        # "<unused>": "BinaryPreprocessor",
+        # "<unused>": "ColorPreprocessor",
+        # "<unused>": "PiDiNetPreprocessor",
+    }
+
     SOURCE_IMAGE_PROCESSING_OPTIONS = ["img2img", "inpainting", "outpainting"]
 
     def _parameter_remap(self, payload: dict[str, str | None]) -> dict[str, str | None]:
         params = {}
         # Extract from the payload things we understand
         for key, value in payload.items():
             newkey = HordeLib.BASIC_INFERENCE_PARAMS.get(key, None)
@@ -131,14 +152,30 @@
                 width = (int(final_width / first_pass_ratio) // 64) * 64
                 height = (int(final_height / first_pass_ratio) // 64) * 64
                 params["empty_latent_image.width"] = width
                 params["empty_latent_image.height"] = height
                 # Finally mark that we are using hires fix
                 params["hires_fix"] = True
 
+        # ControlNet?
+        if cnet := payload.get("control_type"):
+            # Determine the pre-processor that was requested
+            pre_processor = HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.get(cnet)
+
+            # The controlnet type becomes a direct parameter to the pipeline
+            # It is tranlated to its model as required my ComfyUI from the CN ModelManager
+            params["controlnet_model_loader.control_net_name"] = cnet
+
+            # For the pre-processor we dynamically reroute nodes in the pipeline later
+            params["control_type"] = pre_processor
+
+            # Remove the source_processing settings in case they conflict later
+            if "source_processing" in params:
+                del params["source_processing"]
+
         return params
 
     # Fix any nonsensical requests
     def _validate_BASIC_INFERENCE_PARAMS(self, payload):
         # Turn off hires fix if we're not generating a hires image
         if "hires_fix" in payload and (
             payload["width"] <= 512 or payload["height"] <= 512
@@ -159,39 +196,48 @@
         if "hires_fix" in payload and (
             img_proc == "inpainting" or img_proc == "outpainting"
         ):
             payload["hires_fix"] = False
 
     def _get_appropriate_pipeline(self, params):
         # Determine the correct pipeline based on the parameters we have
+        pipeline = None
 
         # Hires fix
         if "hires_fix" in params:
             del params["hires_fix"]
             pipeline = "stable_diffusion_hires_fix"
         else:
             pipeline = "stable_diffusion"
 
         # Source processing modes
         source_proc = params.get("source_processing")
         if source_proc:
             del params["source_processing"]
         if source_proc == "img2img":
-            pass  # doesn't impact pipeline
+            # FIXME: Probably will have a different name from BASIC_INFERENCE_PARAMS
+            if params.get("source_mask"):
+                pipeline = "stable_diffusion_paint"
+            elif len(params.get("image_loader.image").split()) == 4:
+                pipeline = "stable_diffusion_paint"
         elif source_proc == "inpainting":
             pipeline = "stable_diffusion_paint"
         elif source_proc == "outpainting":
             pipeline = "stable_diffusion_paint"
 
+        # ControlNet
+        if params.get("control_type"):
+            pipeline = "controlnet"
+
         return pipeline
 
     def basic_inference(self, payload: dict[str, str | None]) -> Image.Image | None:
         generator = Comfy_Horde()
         # Validate our payload parameters
-        params = self._validate_BASIC_INFERENCE_PARAMS(payload)
+        self._validate_BASIC_INFERENCE_PARAMS(payload)
         # Determine our parameters
         params = self._parameter_remap_basic_inference(payload)
         # Determine the correct pipeline
         pipeline = self._get_appropriate_pipeline(params)
         # Run the pipeline
         images = generator.run_image_pipeline(pipeline, params)
         if images is None:
@@ -207,7 +253,20 @@
         pipeline = "image_upscale"
         # Run the pipeline
         images = generator.run_image_pipeline(pipeline, params)
         if images is None:
             return None  # XXX Log error and/or raise Exception here
         # XXX Assumes the horde only asks for and wants 1 image
         return Image.open(images[0]["imagedata"])
+
+    def image_facefix(self, payload: dict[str, str | None]) -> Image.Image | None:
+        generator = Comfy_Horde()
+        # Determine our parameters
+        params = self._parameter_remap(payload)
+        # Determine the correct pipeline
+        pipeline = "image_facefix"
+        # Run the pipeline
+        images = generator.run_image_pipeline(pipeline, params)
+        if images is None:
+            return None  # XXX Log error and/or raise Exception here
+        # XXX Assumes the horde only asks for and wants 1 image
+        return Image.open(images[0]["imagedata"])
```

### Comparing `hordelib-0.2.0/hordelib/initialisation.py` & `hordelib-0.4.1/hordelib/initialisation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/install_comfy.py` & `hordelib-0.4.1/hordelib/install_comfy.py`

 * *Files 18% similar despite different names*

```diff
@@ -61,30 +61,42 @@
         if not os.path.exists(get_comfyui_path()):
             installdir = os.path.dirname(get_comfyui_path())
             cls._run(
                 "git clone https://github.com/comfyanonymous/ComfyUI.git",
                 installdir,
             )
             cls._run(f"git checkout {comfy_version}", get_comfyui_path())
+            # Apply our patches to comfyui
+            cls.apply_patch(os.path.join(get_hordelib_path(), "install_comfy.patch"))
             return
 
         # If it's installed, is it up to date?
         version = cls.get_commit_hash()
         if version == comfy_version:
             # Yes, all done
             return
 
         # Update comfyui
         logger.info(
             f"Current ComfyUI version {version[:8]} requires {comfy_version[:8]}",
         )
-        # Try hard to ensure we reset everything even if we have been
-        # hacking on ComfyUI or are in a weird repo state
+        cls.reset_comfyui_to_version(comfy_version)
+        # Apply our patches to comfyui
+        cls.apply_patch(os.path.join(get_hordelib_path(), "install_comfy.patch"))
+
+    @classmethod
+    def remove_local_comfyui_changes(cls):
         cls._run("git reset --hard", get_comfyui_path())
         cls._run("git clean -fd", get_comfyui_path())
+
+    @classmethod
+    def reset_comfyui_to_version(cls, comfy_version):
+        # Try hard to ensure we reset everything even if we have been
+        # hacking on ComfyUI or are in a weird repo state
+        cls.remove_local_comfyui_changes()
         cls._run("git checkout master", get_comfyui_path())
         cls._run("git pull", get_comfyui_path())
         cls._run(f"git checkout {comfy_version}", get_comfyui_path())
 
     @classmethod
     def apply_patch(cls, patchfile):
         # Check if the patch has already been applied
@@ -94,15 +106,23 @@
         could_apply = not result.returncode
         result = cls._run_get_result(
             f"git apply --reverse --check {patchfile}", get_comfyui_path()
         )
         could_reverse = not result.returncode
         if could_apply:
             # Apply the patch
-            logger.debug(f"Applying patch {patchfile}")
-            cls._run_get_result(f"git apply {patchfile}", get_comfyui_path())
+            logger.info(f"Applying patch {patchfile}")
+            result = cls._run_get_result(f"git apply {patchfile}", get_comfyui_path())
+            logger.debug(f"{result}")
         elif could_reverse:
             # Patch is already applied, all is well
-            logger.debug(f"Already applied patch {patchfile}")
+            logger.info(f"Already applied patch {patchfile}")
         else:
-            # Couldn't apply or reverse? That's not so good
-            logger.error(f"Could not apply patch {patchfile}")
+            # Couldn't apply or reverse? That's not so good, but maybe we are partially applied?
+            # Reset local changes
+            cls.remove_local_comfyui_changes()
+            # Try to apply the patch
+            logger.info(f"Applying patch {patchfile}")
+            result = cls._run_get_result(f"git apply {patchfile}", get_comfyui_path())
+            logger.debug(f"{result}")
+            if result.returncode:
+                logger.error(f"Could not apply patch {patchfile}")
```

### Comparing `hordelib-0.2.0/hordelib/model_manager/aitemplate.py` & `hordelib-0.4.1/hordelib/model_manager/aitemplate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/base.py` & `hordelib-0.4.1/hordelib/model_manager/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,14 @@
         return self.models.get(model_name)
 
     def get_model_files(self, model_name):
         """
         :param model_name: Name of the model
         Returns the files for a model
         """
-        if self.models[model_name]["type"] == "diffusers":
-            return []
         return self.models[model_name]["config"]["files"]
 
     def get_model_download(self, model_name):
         """
         :param model_name: Name of the model
         Returns the download details for a model
         """
```

### Comparing `hordelib-0.2.0/hordelib/model_manager/blip.py` & `hordelib-0.4.1/hordelib/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/clip.py` & `hordelib-0.4.1/hordelib/model_manager/clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/codeformer.py` & `hordelib-0.4.1/hordelib/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/compvis.py` & `hordelib-0.4.1/hordelib/model_manager/compvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/esrgan.py` & `hordelib-0.4.1/hordelib/model_manager/esrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/gfpgan.py` & `hordelib-0.4.1/hordelib/model_manager/gfpgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/hyper.py` & `hordelib-0.4.1/hordelib/model_manager/hyper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/new.py` & `hordelib-0.4.1/hordelib/model_manager/new.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/safety_checker.py` & `hordelib-0.4.1/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/sdu.py` & `hordelib-0.4.1/hordelib/model_manager/sdu.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/model_manager/torch_hijack.py` & `hordelib-0.4.1/hordelib/model_manager/torch_hijack.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/nodes/node_clip_similarities.py` & `hordelib-0.4.1/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/nodes/node_image_loader.py` & `hordelib-0.4.1/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/nodes/node_image_output.py` & `hordelib-0.4.1/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/nodes/node_model_loader.py` & `hordelib-0.4.1/hordelib/nodes/node_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-0.4.1/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-0.4.1/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-0.4.1/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.4.1/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-0.4.1/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/safety_checker.py` & `hordelib-0.4.1/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/shared_model_manager.py` & `hordelib-0.4.1/hordelib/shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib/utils/cast.py` & `hordelib-0.4.1/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/hordelib.egg-info/PKG-INFO` & `hordelib-0.4.1/hordelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.2.0
+Version: 0.4.1
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -672,21 +672,29 @@
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: <3.11,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hordelib
 
-`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed in ComfyUI. `hordelib` and ComfyUI are licensed under the terms of the GNU General Public License.
+[![PyPI version](https://badge.fury.io/py/hordelib.svg)](https://badge.fury.io/py/hordelib)
+[![Downloads](https://pepy.tech/badge/hordelib)](https://pepy.tech/project/hordelib)
+[![Build](https://github.com/jug-dev/hordelib/actions/workflows/tests.yaml/badge.svg)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
+
+![GitHub license](https://img.shields.io/github/license/jug-dev/hordelib)
+
+`hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of this project can be found in the AI Horde Discord server: https://discord.gg/3DxrhksKznb
 
+NOTE: This project is in early development and is not yet in use by Stable Horde.
+
 ## Purpose
 
-The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically, in a manner ultimately suitable for use in stable horde.
+The goal here is to be able to design inference pipelines in the excellent ComfyUI, and then call those inference pipelines programmatically. Whilst providing features that maintain compatibility with the existing horde implementation.
 
 ## Installation
 
 If being installed from pypi, use a requirements file of the form:
 ```
 --extra-index-url https://download.pytorch.org/whl/cu117
 hordelib
@@ -720,26 +728,30 @@
     "seed": 123456789,
     "height": 512,
     "width": 512,
     "karras": True,
     "tiling": False,
     "hires_fix": False,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "an ancient llamia monster",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
 }
 pil_image = generate.basic_inference(data)
 pil_image.save("test.png")
 ```
 
+Note that `hordelib.initialise()` will erase all command line arguments from argv. So make sure you parse them before you call that.
+
+See `tests/run_*.py` for more standalone examples.
+
 ## Development
 
 Requirements:
 - `git` (install git)
 - `tox` (`pip install tox`)
 - Set the environmental variable `AIWORKER_CACHE_HOME` to point to a model directory.
 
@@ -761,15 +773,15 @@
 
 ### Running the Tests
 
 Simply execute: `tox` (or `tox -q` for less noisy output)
 
 This will take a while the first time as it installs all the dependencies.
 
-If the tests run successfully images will be produced in the project with the name of each pipeline, for example, `pipeline_stable_diffusion.png` and likely some other .png files too.
+If the tests run successfully images will be produced in the `images/` folder.
 
 #### Running a specific test file
 
 `tox -- -k <filename>` for example `tox -- -k test_initialisation`
 
 ### Directory Structure
 
@@ -826,15 +838,18 @@
 1. `cd ..` _Get back to the hordelib project root_
 1. `tox` _See if everything still works_
 
 Now ComfyUI is pinned to a new version.
 
 ### ComfyUI Patching
 
-It may be that we need to patch the ComfyUI source code. Currently this optional and only used for development helpers. However, the mechanisms to patch ComfyUI source code at runtime are also already in place.
+We need to patch the ComfyUI source code. It's only a small patch to:
+
+1. Allow ComfyUI to find our custom nodes without copying files and folder around.
+2. Allow make ComfyUI output some handy JSON we need for development purposes.
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
 
 Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
```

### Comparing `hordelib-0.2.0/images/test_db0.jpg` & `hordelib-0.4.1/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/images/test_inpaint.png` & `hordelib-0.4.1/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/images/test_outpaint.png` & `hordelib-0.4.1/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/pyproject.toml` & `hordelib-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -36,35 +36,47 @@
 exclude = ["ComfyUI"]
 namespaces = false
 
 [options.index-client]
 extra-index-urls = ["https://download.pytorch.org/whl/cu117"]
 
 [tool.pytest.ini_options]
+minversion = "7.0"
 addopts = [
-    "--import-mode=importlib",
+    "--import-mode=prepend",
+    "--ignore=nodes"
+]
+filterwarnings = [
+    "ignore:::.*",
+    "default:::hordelib.*"
+]
+testpaths = [
+    "tests"
 ]
 
+
 [tool.black]
+# Exclude ComfyUI and any packages we have installed in nodes/
 exclude = '''
 /(
     ComfyUI
   | \.tox
+  | nodes[\\/].*
 )/
 '''
 
-[tool.ruff] # XXX this isn't part of CI yet 
+[tool.ruff] # XXX this isn't part of CI yet
 line-length=100 # XXX is this length settled on?
 ignore=[
     "E501", # XXX line too long (comments are the big offender right now)
     "F401", # imported but unused
-] 
+]
 select = [
     "A",    # flake8-builtins
-    "I",    # isort 
+    "I",    # isort
     # "S",    # Bandit
     "F",    # pyflakes
     "E",    # pycodestyle errors
     "W",    # pycodestyle warnings
 
 
     "YTT",  # flake8-2020
@@ -73,18 +85,18 @@
     "COM",  # flake8-commas
     "C4",   # flake8-comprehensions
     # "G",    # flake8-logging-format
     "INP",  # flake8-no-pep420
     "PIE",  # flake8-pie
     # "T20",  # flake8-print
     # "UP",   # pyupgrade
-    "RSE",  # flake8-raise 
+    "RSE",  # flake8-raise
     "RET",  # flake8-return
     # "SLF",  # flake8-self
     "SIM",  # flake8-simplify
     "ARG",  # flake8-unused-arguments
-    # "TRY",  # tryceratops 
+    # "TRY",  # tryceratops
     "RUF100"
 ]
 
 [tool.ruff.per-file-ignores]
 "comfy_horde.py" = ["I001", "F401"]
```

### Comparing `hordelib-0.2.0/tests/run_img2img.py` & `hordelib-0.4.1/tests/run_img2img.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     "seed": 250636385744582,
     "height": 512,
     "width": 512,
     "karras": False,
     "tiling": False,
     "hires_fix": False,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "a dinosaur",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
-    "source_image": Image.open("images/horde_text_to_image.png"),
+    "source_image": Image.open("images/test_db0.jpg"),
 }
 pil_image = generate.basic_inference(data)
-pil_image.save("images/test.png")
+pil_image.save("images/run_img2img.webp", quality=90)
```

### Comparing `hordelib-0.2.0/tests/run_img2img_hires.py` & `hordelib-0.4.1/tests/run_img2img_outpaint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_img2img_hires
+# Call with: python -m test.run_img2img_outpaint
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
 hordelib.initialise()
 
@@ -13,28 +13,29 @@
 from hordelib.shared_model_manager import SharedModelManager
 
 generate = HordeLib()
 SharedModelManager.loadModelManagers(compvis=True)
 SharedModelManager.manager.load("Deliberate")
 
 data = {
-    "sampler_name": "k_dpmpp_2m",
-    "cfg_scale": 7.5,
-    "denoising_strength": 0.3,
-    "seed": 250636385744582,
-    "height": 1024,
-    "width": 1024,
+    "sampler_name": "euler",
+    "cfg_scale": 8.0,
+    "denoising_strength": 1.0,
+    "seed": 836913938046008,
+    "height": 512,
+    "width": 512,
     "karras": False,
     "tiling": False,
-    "hires_fix": True,
+    "hires_fix": False,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
-    "prompt": "a dinosaur",
-    "ddim_steps": 25,
+    "prompt": "a river through the mountains, blue sky with clouds.",
+    "ddim_steps": 20,
     "n_iter": 1,
     "model": "Deliberate",
-    "source_image": Image.open("images/horde_text_to_image.png"),
+    "source_image": Image.open("images/test_outpaint.png"),
+    "source_processing": "outpainting",
 }
 pil_image = generate.basic_inference(data)
-pil_image.save("images/test.png")
+pil_image.save("images/run_img2img_outpaint.webp", quality=90)
```

### Comparing `hordelib-0.2.0/tests/run_img2img_inpaint.py` & `hordelib-0.4.1/tests/run_img2img_inpaint.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     "seed": 836913938046008,
     "height": 512,
     "width": 512,
     "karras": False,
     "tiling": False,
     "hires_fix": False,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "a dinosaur",
     "ddim_steps": 20,
     "n_iter": 1,
     "model": "Deliberate",
-    "source_image": Image.open("images/test_outpaint.png"),
+    "source_image": Image.open("images/test_inpaint.png"),
     "source_processing": "inpainting",
 }
 pil_image = generate.basic_inference(data)
-pil_image.save("images/test.png")
+pil_image.save("images/run_img2img_inpaint.webp", quality=90)
```

### Comparing `hordelib-0.2.0/tests/run_img2img_outpaint.py` & `hordelib-0.4.1/tests/run_txt2img.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_img2img_outpaint
+# Call with: python -m test.run_txt2img
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
 hordelib.initialise()
 
-from PIL import Image
-
 from hordelib.horde import HordeLib
 from hordelib.shared_model_manager import SharedModelManager
 
 generate = HordeLib()
 SharedModelManager.loadModelManagers(compvis=True)
 SharedModelManager.manager.load("Deliberate")
 
 data = {
-    "sampler_name": "euler",
-    "cfg_scale": 8.0,
+    "sampler_name": "k_dpmpp_2m",
+    "cfg_scale": 7.5,
     "denoising_strength": 1.0,
-    "seed": 836913938046008,
+    "seed": 123456789,
     "height": 512,
     "width": 512,
-    "karras": False,
+    "karras": True,
     "tiling": False,
     "hires_fix": False,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
-    "prompt": "a river through the mountains, blue sky with clouds.",
-    "ddim_steps": 20,
+    "prompt": "an ancient llamia monster",
+    "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
-    "source_image": Image.open("images/test_outpaint.png"),
-    "source_processing": "outpainting",
 }
 pil_image = generate.basic_inference(data)
-pil_image.save("images/test.png")
+pil_image.save("images/run_txt2img.webp", quality=90)
```

### Comparing `hordelib-0.2.0/tests/run_txt2img.py` & `hordelib-0.4.1/tests/run_txt2img_hires.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_txt2img
+# Call with: python -m test.run_txt2img_hires
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
 hordelib.initialise()
 
@@ -19,19 +19,19 @@
     "cfg_scale": 7.5,
     "denoising_strength": 1.0,
     "seed": 123456789,
     "height": 512,
     "width": 512,
     "karras": True,
     "tiling": False,
-    "hires_fix": False,
+    "hires_fix": True,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
     "prompt": "an ancient llamia monster",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
 }
 pil_image = generate.basic_inference(data)
-pil_image.save("images/test.png")
+pil_image.save("images/run_txt2img_hires.webp", quality=90)
```

### Comparing `hordelib-0.2.0/tests/run_txt2img_hires.py` & `hordelib-0.4.1/tests/run_img2img_hires.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_txt2img_hires
+# Call with: python -m test.run_img2img_hires
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
 hordelib.initialise()
 
+from PIL import Image
+
 from hordelib.horde import HordeLib
 from hordelib.shared_model_manager import SharedModelManager
 
 generate = HordeLib()
 SharedModelManager.loadModelManagers(compvis=True)
 SharedModelManager.manager.load("Deliberate")
 
 data = {
     "sampler_name": "k_dpmpp_2m",
     "cfg_scale": 7.5,
-    "denoising_strength": 1.0,
-    "seed": 123456789,
-    "height": 512,
-    "width": 512,
-    "karras": True,
+    "denoising_strength": 0.3,
+    "seed": 250636385744582,
+    "height": 1024,
+    "width": 1024,
+    "karras": False,
     "tiling": False,
     "hires_fix": True,
     "clip_skip": 1,
-    "control_type": "canny",
+    "control_type": None,
     "image_is_control": False,
     "return_control_map": False,
-    "prompt": "an ancient llamia monster",
+    "prompt": "a dinosaur",
     "ddim_steps": 25,
     "n_iter": 1,
     "model": "Deliberate",
+    "source_image": Image.open("images/test_db0.jpg"),
 }
 pil_image = generate.basic_inference(data)
-pil_image.save("images/test.png")
+pil_image.save("images/run_img2img_hires.webp", quality=90)
```

### Comparing `hordelib-0.2.0/tests/run_upscale.py` & `hordelib-0.4.1/tests/run_upscale.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 SharedModelManager.manager.load("RealESRGAN_x4plus")
 
 data = {
     "model": "RealESRGAN_x4plus",
     "source_image": Image.open("images/test_db0.jpg"),
 }
 pil_image = generate.image_upscale(data)
-pil_image.save("images/test.png")
+pil_image.save("images/run_upscale.webp", quality=90)
```

### Comparing `hordelib-0.2.0/tests/test_clip.py` & `hordelib-0.4.1/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/tests/test_comfy.py` & `hordelib-0.4.1/tests/test_comfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # test_setup.py
+import glob
 import pytest
 
 from hordelib.comfy_horde import Comfy_Horde
 
 
 class TestSetup:
-    NUMBER_OF_PIPELINES = 4
+    NUMBER_OF_PIPELINES = len(glob.glob("hordelib/pipelines/*.json"))
     comfy: Comfy_Horde
 
     @pytest.fixture(autouse=True)
     def setup_and_teardown(self):
         self.comfy = Comfy_Horde()
         yield
         del self.comfy
@@ -18,24 +19,20 @@
         loaded = self.comfy._load_pipelines()
         assert loaded == TestSetup.NUMBER_OF_PIPELINES
         # Check the built in pipelines
         assert "stable_diffusion" in self.comfy.pipelines
         assert "stable_diffusion_hires_fix" in self.comfy.pipelines
         assert "image_upscale" in self.comfy.pipelines
         assert "stable_diffusion_paint" in self.comfy.pipelines
+        assert "controlnet" in self.comfy.pipelines
 
     def test_load_invalid_pipeline(self):
         loaded = self.comfy._load_pipeline("no-such-pipeline")
         assert loaded is None
 
-    def test_load_invalid_node(self, capsys):
-        self.comfy._load_node("no-such-node")
-        captured = capsys.readouterr()
-        assert "No such file or directory" in str(captured)
-
     def test_load_custom_nodes(self):
         self.comfy._load_custom_nodes()
 
         # Look for our nodes in the ComfyUI nodes list
         import execution
 
         assert "HordeCheckpointLoader" in execution.nodes.NODE_CLASS_MAPPINGS
```

### Comparing `hordelib-0.2.0/tests/test_comfy_install.py` & `hordelib-0.4.1/tests/test_comfy_install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/tests/test_horde_inference.py` & `hordelib-0.4.1/tests/test_horde_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         self.default_model_manager_args = {
             # aitemplate
             # "blip": True,
             # "clip": True,
             # "codeformer": True,
             "compvis": True,
-            # "controlnet": True,
+            "controlnet": True,
             # "diffusers": True,
             # "esrgan": True,
             # "gfpgan": True,
             # "safety_checker": True,
         }
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
@@ -39,15 +39,15 @@
             "seed": "23113",
             "height": 512,
             "width": 512,
             "karras": True,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "a dog ### cat, mouse, lion",
             "ddim_steps": 30,
             "n_iter": 1,
             "model": "Deliberate",
         }
@@ -80,15 +80,15 @@
             "seed": "23113",
             "height": 512,
             "width": 512,
             "karras": False,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "a dog",
             "ddim_steps": 30,
             "n_iter": 1,
             "model": "Deliberate",
         }
@@ -121,15 +121,15 @@
             "seed": 123456789,
             "height": 512,
             "width": 512,
             "karras": True,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "an ancient llamia monster",
             "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
         }
@@ -140,25 +140,25 @@
 
     def test_text_to_image_small(self):
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
             "denoising_strength": 1.0,
             "seed": 123456789,
-            "height": 256,
-            "width": 256,
+            "height": 320,
+            "width": 320,
             "karras": True,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
-            "prompt": "dinosaur ### painting, drawing, artwork",
-            "ddim_steps": 12,
+            "prompt": "a photo of cute dinosaur ### painting, drawing, artwork, red border",
+            "ddim_steps": 20,
             "n_iter": 1,
             "model": "Deliberate",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
         assert pil_image is not None
         pil_image.save("images/horde_text_to_image_small.webp", quality=90)
@@ -171,15 +171,15 @@
             "seed": 123456789,
             "height": 512,
             "width": 512,
             "karras": True,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 2,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "an ancient llamia monster",
             "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
         }
@@ -196,15 +196,15 @@
             "seed": 123456789,
             "height": 768,
             "width": 768,
             "karras": True,
             "tiling": False,
             "hires_fix": True,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "an ancient llamia monster",
             "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
         }
@@ -221,15 +221,15 @@
             "seed": 250636385744582,
             "height": 512,
             "width": 512,
             "karras": False,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "a dinosaur",
             "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
             "source_image": Image.open("images/test_db0.jpg"),
@@ -248,15 +248,15 @@
             "seed": 250636385744582,
             "height": 512,
             "width": 512,
             "karras": False,
             "tiling": False,
             "hires_fix": True,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "a dinosaur",
             "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
             "source_image": Image.open("images/test_db0.jpg"),
@@ -275,15 +275,15 @@
             "seed": 250636385744582,
             "height": 768,
             "width": 768,
             "karras": False,
             "tiling": False,
             "hires_fix": True,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "a dinosaur",
             "ddim_steps": 25,
             "n_iter": 1,
             "model": "Deliberate",
             "source_image": Image.open("images/test_db0.jpg"),
@@ -302,15 +302,15 @@
             "seed": 836913938046008,
             "height": 512,
             "width": 512,
             "karras": False,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "a river through the mountains",
             "ddim_steps": 20,
             "n_iter": 1,
             "model": "Deliberate",
             "source_image": Image.open("images/test_inpaint.png"),
@@ -329,15 +329,15 @@
             "seed": 836913938046008,
             "height": 512,
             "width": 512,
             "karras": False,
             "tiling": False,
             "hires_fix": False,
             "clip_skip": 1,
-            "control_type": "canny",
+            "control_type": None,
             "image_is_control": False,
             "return_control_map": False,
             "prompt": "a river through the mountains, blue sky with clouds.",
             "ddim_steps": 20,
             "n_iter": 1,
             "model": "Deliberate",
             "source_image": Image.open("images/test_outpaint.png"),
```

### Comparing `hordelib-0.2.0/tests/test_horde_pp.py` & `hordelib-0.4.1/tests/test_horde_pp.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     def setup_and_teardown(self):
         self.horde = HordeLib()
 
         self.default_model_manager_args = {
             # aitemplate
             # "blip": True,
             # "clip": True,
-            # "codeformer": True,
+            "codeformer": True,
             # "compvis": True,
             # "controlnet": True,
             # "diffusers": True,
             "esrgan": True,
-            # "gfpgan": True,
+            "gfpgan": True,
             # "safety_checker": True,
         }
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
         self.image = Image.open("images/test_db0.jpg")
         self.width, self.height = self.image.size
         yield
@@ -113,7 +113,23 @@
         }
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         # assert width == self.width * 4
         # assert height == self.height * 4
         pil_image.save("images/horde_image_upscale_4x_AnimeSharp.webp", quality=90)
+
+    def test_image_facefix_codeformers(self):
+        SharedModelManager.manager.load("CodeFormers")
+        assert (
+            SharedModelManager.manager.codeformer.is_model_loaded("CodeFormers") is True
+        )
+        data = {
+            "model": "CodeFormers",
+            "source_image": Image.open("images/test_facefix.png"),
+        }
+        pil_image = self.horde.image_facefix(data)
+        assert pil_image is not None
+        width, height = pil_image.size
+        # assert width == self.width * 4
+        # assert height == self.height * 4
+        pil_image.save("images/horde_image_facefix_codeformers.webp", quality=90)
```

### Comparing `hordelib-0.2.0/tests/test_inference.py` & `hordelib-0.4.1/tests/test_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             "model_loader.model_name": "Deliberate",
             "clip_skip.stop_at_clip_layer": -1,
         }
         images = self.comfy.run_image_pipeline("stable_diffusion", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
-        image.save("images/pipeline_stable_diffusion.png")
+        image.save("images/pipeline_stable_diffusion.webp", quality=90)
 
     def test_stable_diffusion_pipeline_clip_skip(self):
         params = {
             "sampler.sampler_name": "dpmpp_2m",
             "sampler.cfg": 7.5,
             "sampler.denoise": 1.0,
             "sampler.seed": 12345,
@@ -62,15 +62,15 @@
             "model_loader.model_name": "Deliberate",
             "clip_skip.stop_at_clip_layer": -2,
         }
         images = self.comfy.run_image_pipeline("stable_diffusion", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
-        image.save("images/pipeline_stable_diffusion_clip_skip_2.png")
+        image.save("images/pipeline_stable_diffusion_clip_skip_2.webp", quality=90)
 
     def test_stable_diffusion_hires_fix_pipeline(self):
         params = {
             "sampler.seed": 1003,
             "sampler.cfg": 7.5,
             "sampler.scheduler": "normal",
             "sampler.sampler_name": "dpmpp_sde",
@@ -98,15 +98,15 @@
             "upscale_sampler.denoise": 0.5,
             "clip_skip.stop_at_clip_layer": -1,
         }
         images = self.comfy.run_image_pipeline("stable_diffusion_hires_fix", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
-        image.save("images/pipeline_stable_diffusion_hires_fix.png")
+        image.save("images/pipeline_stable_diffusion_hires_fix.webp", quality=90)
 
     def test_stable_diffusion_hires_fix_pipeline_clip_skip_2(self):
         params = {
             "sampler.seed": 1003,
             "sampler.cfg": 7.5,
             "sampler.scheduler": "normal",
             "sampler.sampler_name": "dpmpp_sde",
@@ -134,8 +134,10 @@
             "upscale_sampler.denoise": 0.5,
             "clip_skip.stop_at_clip_layer": -1,
         }
         images = self.comfy.run_image_pipeline("stable_diffusion_hires_fix", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
-        image.save("images/pipeline_stable_diffusion_hires_fix_clip_skip_2.png")
+        image.save(
+            "images/pipeline_stable_diffusion_hires_fix_clip_skip_2.webp", quality=90
+        )
```

### Comparing `hordelib-0.2.0/tests/test_model_manager.py` & `hordelib-0.4.1/tests/test_model_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,21 @@
         SharedModelManager.loadModelManagers(**self.default_model_manager_args)
         assert SharedModelManager.manager is not None
         yield
         del self.horde
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
+    def test_diffusers(self):
+        from hordelib.model_manager.diffusers import DiffusersModelManager
+
+        difusersMM = DiffusersModelManager()
+        difusersMM.load("stable_diffusion_inpainting")
+        pass
+
     def test_compvis(self):
         from hordelib.model_manager.compvis import CompVisModelManager
 
         CompVisModelManager()
 
     def test_horde_model_manager_init(self):
         assert SharedModelManager.manager is not None
```

### Comparing `hordelib-0.2.0/tests/test_safety_checker.py` & `hordelib-0.4.1/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.2.0/tox.ini` & `hordelib-0.4.1/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,84 @@
 00000000: 5b74 6f78 5d0d 0a65 6e76 5f6c 6973 7420  [tox]..env_list 
 00000010: 3d0d 0a20 2020 2066 6f72 6d61 740d 0a20  =..    format.. 
-00000020: 2020 2074 6573 7473 0d0a 0d0a 5b74 6573     tests....[tes
-00000030: 7465 6e76 5d0d 0a64 6573 6372 6970 7469  tenv]..descripti
-00000040: 6f6e 203d 2062 6173 6520 6576 6972 6f6e  on = base eviron
-00000050: 6d65 6e74 2077 6974 6820 616c 6c20 6465  ment with all de
-00000060: 7065 6e64 616e 6369 6573 0d0a 7061 7373  pendancies..pass
-00000070: 656e 7620 3d0d 0a20 2020 2048 4f52 4445  env =..    HORDE
-00000080: 4c49 425f 5445 5354 494e 470d 0a20 2020  LIB_TESTING..   
-00000090: 2041 4957 4f52 4b45 525f 4341 4348 455f   AIWORKER_CACHE_
-000000a0: 484f 4d45 0d0a 6465 7073 203d 0d0a 2020  HOME..deps =..  
-000000b0: 2020 7079 7465 7374 3e3d 370d 0a20 2020    pytest>=7..   
-000000c0: 2070 7974 6573 742d 7375 6761 720d 0a20   pytest-sugar.. 
-000000d0: 2020 2070 7974 6573 742d 636f 760d 0a20     pytest-cov.. 
-000000e0: 2020 2072 6571 7565 7374 730d 0a20 2020     requests..   
-000000f0: 202d 7220 7265 7175 6972 656d 656e 7473   -r requirements
-00000100: 2e74 7874 0d0a 0d0a 5b74 6573 7465 6e76  .txt....[testenv
-00000110: 3a66 6f72 6d61 745d 0d0a 6465 7363 7269  :format]..descri
-00000120: 7074 696f 6e20 3d20 6368 6563 6b20 666f  ption = check fo
-00000130: 726d 6174 7469 6e67 2072 756c 6573 0d0a  rmatting rules..
-00000140: 6465 7073 203d 0d0a 2020 2020 626c 6163  deps =..    blac
-00000150: 6b3d 3d32 322e 332e 300d 0a73 6b69 705f  k==22.3.0..skip_
-00000160: 696e 7374 616c 6c20 3d20 7472 7565 0d0a  install = true..
-00000170: 636f 6d6d 616e 6473 203d 2062 6c61 636b  commands = black
-00000180: 202d 2d63 6865 636b 202e 0d0a 0d0a 5b74   --check .....[t
-00000190: 6573 7465 6e76 3a6c 696e 745d 0d0a 6465  estenv:lint]..de
-000001a0: 7363 7269 7074 696f 6e20 3d20 6368 6563  scription = chec
-000001b0: 6b20 6c69 6e74 696e 6720 7275 6c65 730d  k linting rules.
-000001c0: 0a64 6570 7320 3d0d 0a20 2020 2072 7566  .deps =..    ruf
-000001d0: 663d 3d30 2e30 2e32 3631 0d0a 736b 6970  f==0.0.261..skip
-000001e0: 5f69 6e73 7461 6c6c 203d 2074 7275 650d  _install = true.
-000001f0: 0a63 6f6d 6d61 6e64 7320 3d20 7275 6666  .commands = ruff
-00000200: 202e 0d0a 0d0a 5b74 6573 7465 6e76 3a73   .....[testenv:s
-00000210: 6f72 7469 6d70 6f72 7473 5d0d 0a64 6573  ortimports]..des
-00000220: 6372 6970 7469 6f6e 203d 2063 6865 636b  cription = check
-00000230: 206c 696e 7469 6e67 2072 756c 6573 0d0a   linting rules..
-00000240: 6465 7073 203d 0d0a 2020 2020 7275 6666  deps =..    ruff
-00000250: 3d3d 302e 302e 3236 310d 0a73 6b69 705f  ==0.0.261..skip_
-00000260: 696e 7374 616c 6c20 3d20 7472 7565 0d0a  install = true..
-00000270: 636f 6d6d 616e 6473 203d 2072 7566 6620  commands = ruff 
-00000280: 2d2d 6669 7820 2d2d 6578 636c 7564 6520  --fix --exclude 
-00000290: 636f 6d66 795f 686f 7264 652e 7079 202d  comfy_horde.py -
-000002a0: 2d73 656c 6563 7420 4930 3031 202e 0d0a  -select I001 ...
-000002b0: 0d0a 5b74 6573 7465 6e76 3a63 6f6d 6679  ..[testenv:comfy
-000002c0: 7569 5d0d 0a64 6573 6372 6970 7469 6f6e  ui]..description
-000002d0: 203d 2072 756e 2063 6f6d 6679 7569 0d0a   = run comfyui..
-000002e0: 736b 6970 5f69 6e73 7461 6c6c 203d 2074  skip_install = t
-000002f0: 7275 650d 0a63 6f6d 6d61 6e64 7320 3d0d  rue..commands =.
-00000300: 0a20 2020 207b 656e 7670 7974 686f 6e7d  .    {envpython}
-00000310: 202d 6d20 686f 7264 656c 6962 2e72 756e   -m hordelib.run
-00000320: 5f63 6f6d 6679 7569 0d0a 0d0a 5b74 6573  _comfyui....[tes
-00000330: 7465 6e76 3a74 6573 7473 5d0d 0a64 6573  tenv:tests]..des
-00000340: 6372 6970 7469 6f6e 203d 2069 6e73 7461  cription = insta
-00000350: 6c6c 2070 7974 6573 7420 696e 2061 2076  ll pytest in a v
-00000360: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
-00000370: 6e74 2061 6e64 2069 6e76 6f6b 6520 6974  nt and invoke it
-00000380: 206f 6e20 7468 6520 7465 7374 7320 666f   on the tests fo
-00000390: 6c64 6572 0d0a 7061 7373 656e 7620 3d0d  lder..passenv =.
-000003a0: 0a20 2020 2048 4f52 4445 4c49 425f 5445  .    HORDELIB_TE
-000003b0: 5354 494e 470d 0a20 2020 2041 4957 4f52  STING..    AIWOR
-000003c0: 4b45 525f 4341 4348 455f 484f 4d45 0d0a  KER_CACHE_HOME..
-000003d0: 636f 6d6d 616e 6473 203d 0d0a 2020 2020  commands =..    
-000003e0: 7079 7465 7374 2074 6573 7473 207b 706f  pytest tests {po
-000003f0: 7361 7267 737d 202d 2d63 6f76 202d 2d63  sargs} --cov --c
-00000400: 6f76 2d72 6570 6f72 743d 7465 726d 202d  ov-report=term -
-00000410: 2d63 6f76 2d72 6570 6f72 743d 6c63 6f76  -cov-report=lcov
-00000420: 0d0a                                     ..
+00000020: 2020 2074 6573 7473 0d0a 0d0a 5b63 6f76     tests....[cov
+00000030: 6572 6167 653a 7275 6e5d 0d0a 6f6d 6974  erage:run]..omit
+00000040: 203d 0d0a 2020 2020 436f 6d66 7955 492f   =..    ComfyUI/
+00000050: 2a0d 0a20 2020 202a 2f6e 6f64 6573 2f2a  *..    */nodes/*
+00000060: 0d0a 2020 2020 2a2f 636f 6e66 6967 2e70  ..    */config.p
+00000070: 790d 0a20 2020 202a 2f63 6f6e 6669 672d  y..    */config-
+00000080: 332e 7079 0d0a 0d0a 5b63 6f76 6572 6167  3.py....[coverag
+00000090: 653a 7061 7468 735d 0d0a 736f 7572 6365  e:paths]..source
+000000a0: 203d 0d0a 2020 2020 686f 7264 656c 6962   =..    hordelib
+000000b0: 2f0d 0a0d 0a5b 636f 7665 7261 6765 3a72  /....[coverage:r
+000000c0: 6570 6f72 745d 0d0a 6f6d 6974 203d 0d0a  eport]..omit =..
+000000d0: 2020 2020 436f 6d66 7955 492f 2a0d 0a20      ComfyUI/*.. 
+000000e0: 2020 202a 2f6e 6f64 6573 2f2a 0d0a 2020     */nodes/*..  
+000000f0: 2020 2a2f 636f 6e66 6967 2e70 790d 0a20    */config.py.. 
+00000100: 2020 202a 2f63 6f6e 6669 672d 332e 7079     */config-3.py
+00000110: 0d0a 6c63 6f76 5f72 6570 6f72 7420 3d20  ..lcov_report = 
+00000120: 7465 726d 2063 6f76 6572 6167 652e 6c63  term coverage.lc
+00000130: 6f76 0d0a 6967 6e6f 7265 5f65 7272 6f72  ov..ignore_error
+00000140: 7320 3d20 5472 7565 0d0a 736b 6970 5f65  s = True..skip_e
+00000150: 6d70 7479 203d 2054 7275 650d 0a0d 0a5b  mpty = True....[
+00000160: 7465 7374 656e 765d 0d0a 6465 7363 7269  testenv]..descri
+00000170: 7074 696f 6e20 3d20 6261 7365 2065 7669  ption = base evi
+00000180: 726f 6e6d 656e 7420 7769 7468 2061 6c6c  ronment with all
+00000190: 2064 6570 656e 6461 6e63 6965 730d 0a70   dependancies..p
+000001a0: 6173 7365 6e76 203d 0d0a 2020 2020 484f  assenv =..    HO
+000001b0: 5244 454c 4942 5f54 4553 5449 4e47 0d0a  RDELIB_TESTING..
+000001c0: 2020 2020 4149 574f 524b 4552 5f43 4143      AIWORKER_CAC
+000001d0: 4845 5f48 4f4d 450d 0a64 6570 7320 3d0d  HE_HOME..deps =.
+000001e0: 0a20 2020 2070 7974 6573 743e 3d37 0d0a  .    pytest>=7..
+000001f0: 2020 2020 7079 7465 7374 2d73 7567 6172      pytest-sugar
+00000200: 0d0a 2020 2020 7079 7465 7374 2d63 6f76  ..    pytest-cov
+00000210: 0d0a 2020 2020 7265 7175 6573 7473 0d0a  ..    requests..
+00000220: 2020 2020 2d72 2072 6571 7569 7265 6d65      -r requireme
+00000230: 6e74 732e 7478 740d 0a0d 0a5b 7465 7374  nts.txt....[test
+00000240: 656e 763a 666f 726d 6174 5d0d 0a64 6573  env:format]..des
+00000250: 6372 6970 7469 6f6e 203d 2063 6865 636b  cription = check
+00000260: 2066 6f72 6d61 7474 696e 6720 7275 6c65   formatting rule
+00000270: 730d 0a64 6570 7320 3d0d 0a20 2020 2062  s..deps =..    b
+00000280: 6c61 636b 3d3d 3232 2e33 2e30 0d0a 736b  lack==22.3.0..sk
+00000290: 6970 5f69 6e73 7461 6c6c 203d 2074 7275  ip_install = tru
+000002a0: 650d 0a63 6f6d 6d61 6e64 7320 3d20 626c  e..commands = bl
+000002b0: 6163 6b20 2d2d 6368 6563 6b20 2e0d 0a0d  ack --check ....
+000002c0: 0a5b 7465 7374 656e 763a 6c69 6e74 5d0d  .[testenv:lint].
+000002d0: 0a64 6573 6372 6970 7469 6f6e 203d 2063  .description = c
+000002e0: 6865 636b 206c 696e 7469 6e67 2072 756c  heck linting rul
+000002f0: 6573 0d0a 6465 7073 203d 0d0a 2020 2020  es..deps =..    
+00000300: 7275 6666 3d3d 302e 302e 3236 310d 0a73  ruff==0.0.261..s
+00000310: 6b69 705f 696e 7374 616c 6c20 3d20 7472  kip_install = tr
+00000320: 7565 0d0a 636f 6d6d 616e 6473 203d 2072  ue..commands = r
+00000330: 7566 6620 2e0d 0a0d 0a5b 7465 7374 656e  uff .....[testen
+00000340: 763a 736f 7274 696d 706f 7274 735d 0d0a  v:sortimports]..
+00000350: 6465 7363 7269 7074 696f 6e20 3d20 6368  description = ch
+00000360: 6563 6b20 6c69 6e74 696e 6720 7275 6c65  eck linting rule
+00000370: 730d 0a64 6570 7320 3d0d 0a20 2020 2072  s..deps =..    r
+00000380: 7566 663d 3d30 2e30 2e32 3631 0d0a 736b  uff==0.0.261..sk
+00000390: 6970 5f69 6e73 7461 6c6c 203d 2074 7275  ip_install = tru
+000003a0: 650d 0a63 6f6d 6d61 6e64 7320 3d20 7275  e..commands = ru
+000003b0: 6666 202d 2d66 6978 202d 2d65 7863 6c75  ff --fix --exclu
+000003c0: 6465 2063 6f6d 6679 5f68 6f72 6465 2e70  de comfy_horde.p
+000003d0: 7920 2d2d 7365 6c65 6374 2049 3030 3120  y --select I001 
+000003e0: 2e0d 0a0d 0a5b 7465 7374 656e 763a 636f  .....[testenv:co
+000003f0: 6d66 7975 695d 0d0a 6465 7363 7269 7074  mfyui]..descript
+00000400: 696f 6e20 3d20 7275 6e20 636f 6d66 7975  ion = run comfyu
+00000410: 690d 0a73 6b69 705f 696e 7374 616c 6c20  i..skip_install 
+00000420: 3d20 7472 7565 0d0a 636f 6d6d 616e 6473  = true..commands
+00000430: 203d 0d0a 2020 2020 7b65 6e76 7079 7468   =..    {envpyth
+00000440: 6f6e 7d20 2d6d 2068 6f72 6465 6c69 622e  on} -m hordelib.
+00000450: 7275 6e5f 636f 6d66 7975 690d 0a0d 0a5b  run_comfyui....[
+00000460: 7465 7374 656e 763a 7465 7374 735d 0d0a  testenv:tests]..
+00000470: 6465 7363 7269 7074 696f 6e20 3d20 696e  description = in
+00000480: 7374 616c 6c20 7079 7465 7374 2069 6e20  stall pytest in 
+00000490: 6120 7669 7274 7561 6c20 656e 7669 726f  a virtual enviro
+000004a0: 6e6d 656e 7420 616e 6420 696e 766f 6b65  nment and invoke
+000004b0: 2069 7420 6f6e 2074 6865 2074 6573 7473   it on the tests
+000004c0: 2066 6f6c 6465 720d 0a70 6173 7365 6e76   folder..passenv
+000004d0: 203d 0d0a 2020 2020 484f 5244 454c 4942   =..    HORDELIB
+000004e0: 5f54 4553 5449 4e47 0d0a 2020 2020 4149  _TESTING..    AI
+000004f0: 574f 524b 4552 5f43 4143 4845 5f48 4f4d  WORKER_CACHE_HOM
+00000500: 450d 0a63 6f6d 6d61 6e64 7320 3d0d 0a20  E..commands =.. 
+00000510: 2020 2070 7974 6573 7420 7465 7374 7320     pytest tests 
+00000520: 7b70 6f73 6172 6773 7d20 2d2d 636f 760d  {posargs} --cov.
+00000530: 0a                                       .
```

