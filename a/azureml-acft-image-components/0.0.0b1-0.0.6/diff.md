# Comparing `tmp/azureml_acft_image_components-0.0.0b1-py3-none-any.whl.zip` & `tmp/azureml_acft_image_components-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,137 @@
-Zip file size: 2900 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      249 b- defN 20-Jun-24 20:49 azureml/__init__.py
--rw-rw-rw-  2.0 fat      249 b- defN 20-Jun-24 20:49 azureml/acft/__init__.py
--rw-rw-rw-  2.0 fat      249 b- defN 20-Jun-24 20:49 azureml/acft/common/__init__.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Mar-07 17:42 azureml_acft_image_components-0.0.0b1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      419 b- defN 23-Mar-07 17:42 azureml_acft_image_components-0.0.0b1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-07 17:42 azureml_acft_image_components-0.0.0b1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-07 17:42 azureml_acft_image_components-0.0.0b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      750 b- defN 23-Mar-07 17:42 azureml_acft_image_components-0.0.0b1.dist-info/RECORD
-8 files, 3037 bytes uncompressed, 1556 bytes compressed:  48.8%
+Zip file size: 298829 bytes, number of entries: 135
+-rw-rw-rw-  2.0 fat      251 b- defN 23-Apr-10 23:37 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      295 b- defN 23-Apr-10 23:37 azureml/acft/__init__.py
+-rw-rw-rw-  2.0 fat      822 b- defN 23-Apr-10 23:37 azureml/acft/image/__init__.py
+-rw-rw-rw-  2.0 fat   600282 b- defN 23-Apr-10 23:37 azureml/acft/image/components/NOTICE.txt
+-rw-rw-rw-  2.0 fat      297 b- defN 23-Apr-10 23:37 azureml/acft/image/components/__init__.py
+-rw-rw-rw-  2.0 fat       34 b- defN 23-Apr-10 23:44 azureml/acft/image/components/_version.py
+-rw-rw-rw-  2.0 fat      312 b- defN 23-Apr-10 23:37 azureml/acft/image/components/common/__init__.py
+-rw-rw-rw-  2.0 fat      583 b- defN 23-Apr-10 23:37 azureml/acft/image/components/common/utils.py
+-rw-rw-rw-  2.0 fat      320 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/__init__.py
+-rw-rw-rw-  2.0 fat     7891 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/finetune_runner.py
+-rw-rw-rw-  2.0 fat      466 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/__init__.py
+-rw-rw-rw-  2.0 fat      893 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/utils.py
+-rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/__init__.py
+-rw-rw-rw-  2.0 fat     9017 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py
+-rw-rw-rw-  2.0 fat    17791 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py
+-rw-rw-rw-  2.0 fat    10881 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/custom_augmentations.py
+-rw-rw-rw-  2.0 fat    26914 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py
+-rw-rw-rw-  2.0 fat      320 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py
+-rw-rw-rw-  2.0 fat     1929 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml
+-rw-rw-rw-  2.0 fat     2474 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml
+-rw-rw-rw-  2.0 fat     1314 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/augmentation/configs/hf_albumentations_classification.yaml
+-rw-rw-rw-  2.0 fat      309 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/constants/__init__.py
+-rw-rw-rw-  2.0 fat     1817 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/constants/augmentation_constants.py
+-rw-rw-rw-  2.0 fat     4475 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/constants/constants.py
+-rw-rw-rw-  2.0 fat      304 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/data/__init__.py
+-rw-rw-rw-  2.0 fat     4848 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/data/base_dataset.py
+-rw-rw-rw-  2.0 fat     8655 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/data/classification_dataset.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py
+-rw-rw-rw-  2.0 fat    10245 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/data/download_manager.py
+-rw-rw-rw-  2.0 fat     7569 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py
+-rw-rw-rw-  2.0 fat      338 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/__init__.py
+-rw-rw-rw-  2.0 fat     2333 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/common_constants.py
+-rw-rw-rw-  2.0 fat     6225 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/common_utils.py
+-rw-rw-rw-  2.0 fat     6194 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py
+-rw-rw-rw-  2.0 fat     3222 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/hf_utils.py
+-rw-rw-rw-  2.0 fat      102 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/mmdet-requirements.txt
+-rw-rw-rw-  2.0 fat     5123 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py
+-rw-rw-rw-  2.0 fat     6775 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py
+-rw-rw-rw-  2.0 fat     8293 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py
+-rw-rw-rw-  2.0 fat      329 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/defaults/__init__.py
+-rw-rw-rw-  2.0 fat     3091 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/defaults/classification_models_defaults.py
+-rw-rw-rw-  2.0 fat     3507 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/defaults/constants.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py
+-rw-rw-rw-  2.0 fat      823 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py
+-rw-rw-rw-  2.0 fat      808 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py
+-rw-rw-rw-  2.0 fat     2021 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/defaults/task_defaults.py
+-rw-rw-rw-  2.0 fat     7761 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/defaults/training_defaults.py
+-rw-rw-rw-  2.0 fat      333 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/factory/__init__.py
+-rw-rw-rw-  2.0 fat      764 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/factory/mappings.py
+-rw-rw-rw-  2.0 fat     1750 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/factory/model_factory.py
+-rw-rw-rw-  2.0 fat      548 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/factory/task_definitions.py
+-rw-rw-rw-  2.0 fat     5988 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/__init__.py
+-rw-rw-rw-  2.0 fat      347 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/classification/__init__.py
+-rw-rw-rw-  2.0 fat     8922 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/classification/data_cls.py
+-rw-rw-rw-  2.0 fat     2367 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py
+-rw-rw-rw-  2.0 fat     5355 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/classification/inference_cls.py
+-rw-rw-rw-  2.0 fat     1706 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/classification/trainer_classes.py
+-rw-rw-rw-  2.0 fat      339 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/common/__init__.py
+-rw-rw-rw-  2.0 fat      951 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/common/constants.py
+-rw-rw-rw-  2.0 fat    18975 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py
+-rw-rw-rw-  2.0 fat      350 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/mlflow/__init__.py
+-rw-rw-rw-  2.0 fat     8760 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/huggingface/mlflow/hf_test_predict.py
+-rw-rw-rw-  2.0 fat      265 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/interfaces/__init__.py
+-rw-rw-rw-  2.0 fat    10706 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/interfaces/azml_interface.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/__init__.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/__init__.py
+-rw-rw-rw-  2.0 fat      759 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/constants.py
+-rw-rw-rw-  2.0 fat     9959 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/data_class.py
+-rw-rw-rw-  2.0 fat     8592 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/dataset.py
+-rw-rw-rw-  2.0 fat     1108 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py
+-rw-rw-rw-  2.0 fat     3015 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/inference.py
+-rw-rw-rw-  2.0 fat    10173 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/metrics.py
+-rw-rw-rw-  2.0 fat     7234 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/model.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py
+-rw-rw-rw-  2.0 fat      264 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py
+-rw-rw-rw-  2.0 fat     7586 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py
+-rw-rw-rw-  2.0 fat      259 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py
+-rw-rw-rw-  2.0 fat    10810 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py
+-rw-rw-rw-  2.0 fat      337 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/classification/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/classification/common/__init__.py
+-rw-rw-rw-  2.0 fat    27116 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/classification/common/classification_utils.py
+-rw-rw-rw-  2.0 fat     7507 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/classification/common/constants.py
+-rw-rw-rw-  2.0 fat     2601 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/classification/common/transforms.py
+-rw-rw-rw-  2.0 fat      331 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/__init__.py
+-rw-rw-rw-  2.0 fat     1903 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/aml_dataset_base_wrapper.py
+-rw-rw-rw-  2.0 fat    10450 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/artifacts_utils.py
+-rw-rw-rw-  2.0 fat     2025 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/average_meter.py
+-rw-rw-rw-  2.0 fat     2233 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/base_model_factory.py
+-rw-rw-rw-  2.0 fat     1231 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/base_model_settings.py
+-rw-rw-rw-  2.0 fat    22490 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/constants.py
+-rw-rw-rw-  2.0 fat     2826 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/data_utils.py
+-rw-rw-rw-  2.0 fat     3200 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/dataloaders.py
+-rw-rw-rw-  2.0 fat    18975 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/dataset_helper.py
+-rw-rw-rw-  2.0 fat    21071 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/distributed_utils.py
+-rw-rw-rw-  2.0 fat      672 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/errors.py
+-rw-rw-rw-  2.0 fat     2379 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/exceptions.py
+-rw-rw-rw-  2.0 fat     2528 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/logging_utils.py
+-rw-rw-rw-  2.0 fat    25090 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/model_export_utils.py
+-rw-rw-rw-  2.0 fat    14792 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/parameters.py
+-rw-rw-rw-  2.0 fat    10358 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/prediction_dataset.py
+-rw-rw-rw-  2.0 fat    37139 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/pretrained_model_utilities.py
+-rw-rw-rw-  2.0 fat     3033 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/sku_validation.py
+-rw-rw-rw-  2.0 fat     9854 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/system_meter.py
+-rw-rw-rw-  2.0 fat     5482 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/tiling_dataset_element.py
+-rw-rw-rw-  2.0 fat     6632 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/tiling_utils.py
+-rw-rw-rw-  2.0 fat     1039 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/torch_utils.py
+-rw-rw-rw-  2.0 fat    65467 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/common/utils.py
+-rw-rw-rw-  2.0 fat      302 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/__init__.py
+-rw-rw-rw-  2.0 fat      311 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/__init__.py
+-rw-rw-rw-  2.0 fat     9651 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/augmentations.py
+-rw-rw-rw-  2.0 fat     7384 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/boundingbox.py
+-rw-rw-rw-  2.0 fat     3072 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/coco_eval_box_converter.py
+-rw-rw-rw-  2.0 fat    11010 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/constants.py
+-rw-rw-rw-  2.0 fat    11945 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/masktools.py
+-rw-rw-rw-  2.0 fat    27549 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/object_detection_utils.py
+-rw-rw-rw-  2.0 fat     5003 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/parameters.py
+-rw-rw-rw-  2.0 fat    25989 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/common/tiling_helper.py
+-rw-rw-rw-  2.0 fat      306 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/data/__init__.py
+-rw-rw-rw-  2.0 fat     5012 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/data/dataset_wrappers.py
+-rw-rw-rw-  2.0 fat    39886 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/data/datasets.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/data/loaders.py
+-rw-rw-rw-  2.0 fat    11905 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/data/object_annotation.py
+-rw-rw-rw-  2.0 fat     5041 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/data/tiling_distributed_sampler.py
+-rw-rw-rw-  2.0 fat    11382 b- defN 23-Apr-10 23:37 azureml/acft/image/components/finetune/runtime_common/object_detection/data/utils.py
+-rw-rw-rw-  2.0 fat      321 b- defN 23-Apr-10 23:37 azureml/acft/image/components/model_selector/__init__.py
+-rw-rw-rw-  2.0 fat    10217 b- defN 23-Apr-10 23:37 azureml/acft/image/components/model_selector/component.py
+-rw-rw-rw-  2.0 fat      494 b- defN 23-Apr-10 23:37 azureml/acft/image/components/model_selector/constants.py
+-rw-rw-rw-  2.0 fat      859 b- defN 23-Apr-10 23:44 azureml_acft_image_components-0.0.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1485 b- defN 23-Apr-10 23:44 azureml_acft_image_components-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-10 23:44 azureml_acft_image_components-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-10 23:44 azureml_acft_image_components-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    17555 b- defN 23-Apr-10 23:44 azureml_acft_image_components-0.0.6.dist-info/RECORD
+135 files, 1445119 bytes uncompressed, 268679 bytes compressed:  81.4%
```

## zipnote {}

```diff
@@ -1,25 +1,406 @@
 Filename: azureml/__init__.py
 Comment: 
 
 Filename: azureml/acft/__init__.py
 Comment: 
 
-Filename: azureml/acft/common/__init__.py
+Filename: azureml/acft/image/__init__.py
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.0b1.dist-info/LICENSE.txt
+Filename: azureml/acft/image/components/NOTICE.txt
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.0b1.dist-info/METADATA
+Filename: azureml/acft/image/components/__init__.py
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.0b1.dist-info/WHEEL
+Filename: azureml/acft/image/components/_version.py
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.0b1.dist-info/top_level.txt
+Filename: azureml/acft/image/components/common/__init__.py
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.0b1.dist-info/RECORD
+Filename: azureml/acft/image/components/common/utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/finetune_runner.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/custom_augmentations.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/augmentation/configs/hf_albumentations_classification.yaml
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/constants/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/constants/augmentation_constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/constants/constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/data/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/data/base_dataset.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/data/classification_dataset.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/data/download_manager.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/common_constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/common_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/hf_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet-requirements.txt
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/classification_models_defaults.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/task_defaults.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/defaults/training_defaults.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/factory/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/factory/mappings.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/factory/model_factory.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/factory/task_definitions.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/classification/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/classification/data_cls.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/classification/inference_cls.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/classification/trainer_classes.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/common/constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/mlflow/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/huggingface/mlflow/hf_test_predict.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/interfaces/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/interfaces/azml_interface.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/data_class.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/dataset.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/inference.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/metrics.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/model.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/classification/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/classification/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/classification/common/classification_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/classification/common/constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/classification/common/transforms.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/aml_dataset_base_wrapper.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/artifacts_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/average_meter.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/base_model_factory.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/base_model_settings.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/data_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/dataloaders.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/dataset_helper.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/distributed_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/errors.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/exceptions.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/logging_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/model_export_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/parameters.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/prediction_dataset.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/pretrained_model_utilities.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/sku_validation.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/system_meter.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/tiling_dataset_element.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/tiling_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/torch_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/common/utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/augmentations.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/boundingbox.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/coco_eval_box_converter.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/constants.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/masktools.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/object_detection_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/parameters.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/tiling_helper.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/dataset_wrappers.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/datasets.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/loaders.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/object_annotation.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/tiling_distributed_sampler.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/model_selector/__init__.py
+Comment: 
+
+Filename: azureml/acft/image/components/model_selector/component.py
+Comment: 
+
+Filename: azureml/acft/image/components/model_selector/constants.py
+Comment: 
+
+Filename: azureml_acft_image_components-0.0.6.dist-info/LICENSE.txt
+Comment: 
+
+Filename: azureml_acft_image_components-0.0.6.dist-info/METADATA
+Comment: 
+
+Filename: azureml_acft_image_components-0.0.6.dist-info/WHEEL
+Comment: 
+
+Filename: azureml_acft_image_components-0.0.6.dist-info/top_level.txt
+Comment: 
+
+Filename: azureml_acft_image_components-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/__init__.py

```diff
@@ -1,4 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
+
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
```

## azureml/acft/__init__.py

```diff
@@ -1,4 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
+"""AzureML ACFT Image Components package."""
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
```

## Comparing `azureml_acft_image_components-0.0.0b1.dist-info/LICENSE.txt` & `azureml_acft_image_components-0.0.6.dist-info/LICENSE.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-This Preview is made available to you on the condition that you agree to the
-[Supplemental Terms of Use for Microsoft Azure Previews][1], which supplement
-[your agreement][2] governing your use of Azure.
+This software is made available to you on the condition that you agree to
+[your agreement][1] governing your use of Azure.
 If you do not have an existing agreement governing your use of Azure, you agree that 
-your agreement governing use of Azure is the [Microsoft Online Subscription Agreement][3]
-(which incorporates the [Online Services Terms][4]).
-By using the Preview you agree to these terms. This Preview may collect data
-that is transmitted to Microsoft. Please see the [Microsoft Privacy Statement][5]
+your agreement governing use of Azure is the [Microsoft Online Subscription Agreement][2]
+(which incorporates the [Online Services Terms][3]).
+By using the software you agree to these terms. This software may collect data
+that is transmitted to Microsoft. Please see the [Microsoft Privacy Statement][4]
 to learn more about how Microsoft processes personal data.
 
-[1]: https://azure.microsoft.com/en-us/support/legal/preview-supplemental-terms/
-[2]: https://azure.microsoft.com/en-us/support/legal/
-[3]: https://azure.microsoft.com/en-us/support/legal/subscription-agreement/
-[4]: http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=46
-[5]: http://go.microsoft.com/fwlink/?LinkId=248681 
+[1]: https://azure.microsoft.com/en-us/support/legal/
+[2]: https://azure.microsoft.com/en-us/support/legal/subscription-agreement/
+[3]: http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=46
+[4]: http://go.microsoft.com/fwlink/?LinkId=248681
```

