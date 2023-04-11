# Comparing `tmp/regula.facesdk.webclient-5.1.0.tar.gz` & `tmp/regula.facesdk.webclient-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regula.facesdk.webclient-5.1.0.tar", last modified: Mon Mar 27 05:49:28 2023, max compression
+gzip compressed data, was "regula.facesdk.webclient-5.1.1.tar", last modified: Tue Apr 11 02:08:46 2023, max compression
```

## Comparing `regula.facesdk.webclient-5.1.0.tar` & `regula.facesdk.webclient-5.1.1.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.392353 regula.facesdk.webclient-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-27 05:49:28.392353 regula.facesdk.webclient-5.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.372354 regula.facesdk.webclient-5.1.0/regula/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.376354 regula.facesdk.webclient-5.1.0/regula/facesdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.376354 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.376354 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/
--rwxr-xr-x   0 runner    (1001) docker     (123)      309 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.376354 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/group_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2083 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/matching_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/person_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/search_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.376354 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/models/detect_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/models/match_image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/models/match_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.376354 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.380354 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47391 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/liveness_2_0_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/liveness_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/matching_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    68455 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/person_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27677 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.380354 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.392353 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detect_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detect_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detect_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detect_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detection_face.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detection_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_align_type_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_image_quality_align_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_image_quality_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_image_quality_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_quality_config_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_quality_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_quality_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_rectangular.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_sdk_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_sdk_result_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/faces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/faces_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group_page_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group_to_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_fields_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_page_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/liveness_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_request_all_of_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_response_all_of_detections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_image_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_image_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_response_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/operation_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/output_image_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person_with_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person_with_images_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/persons_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/persons_page_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/process_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_config_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_details_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/recognize_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/recognize_image_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_person_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_result_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/transaction_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/update_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    82471 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.392353 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:49:28.376354 regula.facesdk.webclient-5.1.0/regula.facesdk.webclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-27 05:49:28.000000 regula.facesdk.webclient-5.1.0/regula.facesdk.webclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-03-27 05:49:28.000000 regula.facesdk.webclient-5.1.0/regula.facesdk.webclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 05:49:28.000000 regula.facesdk.webclient-5.1.0/regula.facesdk.webclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-27 05:49:28.000000 regula.facesdk.webclient-5.1.0/regula.facesdk.webclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 05:49:28.000000 regula.facesdk.webclient-5.1.0/regula.facesdk.webclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 05:49:28.392353 regula.facesdk.webclient-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-03-27 05:48:43.000000 regula.facesdk.webclient-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.587455 regula.facesdk.webclient-5.1.1/regula/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      309 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/group_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2083 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/matching_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/person_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/search_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.591455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/detect_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      773 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/match_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/match_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.595455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.595455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47391 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/liveness_2_0_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/liveness_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19983 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/matching_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68455 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/person_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27677 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.595455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16633 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_align_type_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_align_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_config_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_rectangular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_sdk_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_sdk_result_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/faces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/faces_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_page_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_to_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_fields_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_page_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/liveness_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request_all_of_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response_all_of_detections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_response_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/operation_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/output_image_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_with_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_with_images_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/persons_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/persons_page_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/process_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_config_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_details_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/recognize_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/recognize_image_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_person_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_result_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/transaction_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/transaction_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/update_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82471 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:08:46.587455 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 02:08:46.000000 regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:08:46.611455 regula.facesdk.webclient-5.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-11 02:07:36.000000 regula.facesdk.webclient-5.1.1/setup.py
```

### Comparing `regula.facesdk.webclient-5.1.0/PKG-INFO` & `regula.facesdk.webclient-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regula.facesdk.webclient
-Version: 5.1.0
+Version: 5.1.1
 Summary: Regula's FaceSDK web python client
 Home-page: https://mobile.regulaforensics.com
 Author: Regula Forensics, Inc.
 Author-email: support@regulaforensics.com
 Keywords: face recognition,facesdk,regulaforensics,regula
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `regula.facesdk.webclient-5.1.0/README.md` & `regula.facesdk.webclient-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/__init__.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/group_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/group_api.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/matching_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/matching_api.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/person_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/person_api.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/sdk.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/sdk.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/api/search_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/api/search_api.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/models/detect_request.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/detect_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,10 +14,10 @@
         if not image:
             raise ApiValueError(f"image: expected <not empty> - obtained <{image}>", "image")
 
         if isinstance(image, bytes):
             image = bytes_to_base64(image)
 
         super().__init__(
-            image=image, only_central_face=only_central_face, attributes=attributes, thumbnails=thumbnails,
+            image=image, attributes=attributes, thumbnails=thumbnails,
             local_vars_configuration=local_vars_configuration, tag=tag
         )
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/models/match_image.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/match_image.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/ext/models/match_request.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/ext/models/match_request.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/__init__.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/group_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/group_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/liveness_2_0_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/liveness_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,166 +20,37 @@
 from regula.facesdk.webclient.gen.api_client import ApiClient
 from regula.facesdk.webclient.gen.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class Liveness20Api(object):
+class LivenessApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def get_liveness_transaction(self, transaction_id, **kwargs):  # noqa: E501
-        """liveness  # noqa: E501
+    def liveness_metadata(self, error_unknown, **kwargs):  # noqa: E501
+        """Liveness 2.0 metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_liveness_transaction(transaction_id, async_req=True)
+        >>> thread = api.liveness_metadata(error_unknown, async_req=True)
         >>> result = thread.get()
 
-        :param transaction_id: ID of the current liveness transaction. (required)
-        :type transaction_id: int
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: LivenessTransaction
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_liveness_transaction_with_http_info(transaction_id, **kwargs)  # noqa: E501
-
-    def get_liveness_transaction_with_http_info(self, transaction_id, **kwargs):  # noqa: E501
-        """liveness  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_liveness_transaction_with_http_info(transaction_id, async_req=True)
-        >>> result = thread.get()
-
-        :param transaction_id: ID of the current liveness transaction. (required)
-        :type transaction_id: int
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(LivenessTransaction, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'transaction_id'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_liveness_transaction" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-        # verify the required parameter 'transaction_id' is set
-        if self.api_client.client_side_validation and ('transaction_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['transaction_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `transaction_id` when calling `get_liveness_transaction`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-        if 'transaction_id' in local_var_params and local_var_params['transaction_id'] is not None:  # noqa: E501
-            query_params.append(('transactionId', local_var_params['transaction_id']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = []  # noqa: E501
-
-        return self.api_client.call_api(
-            '/api/v2/liveness', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='LivenessTransaction',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout'),
-            collection_formats=collection_formats,
-            _request_auth=local_var_params.get('_request_auth'))
-
-    def liveness_metadata(self, transaction_id, **kwargs):  # noqa: E501
-        """metadata  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.liveness_metadata(transaction_id, async_req=True)
-        >>> result = thread.get()
-
-        :param transaction_id: ID of the current liveness transaction. (required)
-        :type transaction_id: int
+        :param error_unknown: ID of the current liveness transaction. (required)
+        :type error_unknown: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -188,27 +59,27 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         kwargs['_return_http_data_only'] = True
-        return self.liveness_metadata_with_http_info(transaction_id, **kwargs)  # noqa: E501
+        return self.liveness_metadata_with_http_info(error_unknown, **kwargs)  # noqa: E501
 
-    def liveness_metadata_with_http_info(self, transaction_id, **kwargs):  # noqa: E501
-        """metadata  # noqa: E501
+    def liveness_metadata_with_http_info(self, error_unknown, **kwargs):  # noqa: E501
+        """Liveness 2.0 metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_metadata_with_http_info(transaction_id, async_req=True)
+        >>> thread = api.liveness_metadata_with_http_info(error_unknown, async_req=True)
         >>> result = thread.get()
 
-        :param transaction_id: ID of the current liveness transaction. (required)
-        :type transaction_id: int
+        :param error_unknown: ID of the current liveness transaction. (required)
+        :type error_unknown: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -227,15 +98,15 @@
                  returns the request thread.
         :rtype: tuple({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'transaction_id'
+            'error_unknown'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -247,26 +118,26 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method liveness_metadata" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'transaction_id' is set
-        if self.api_client.client_side_validation and ('transaction_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['transaction_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `transaction_id` when calling `liveness_metadata`")  # noqa: E501
+        # verify the required parameter 'error_unknown' is set
+        if self.api_client.client_side_validation and ('error_unknown' not in local_var_params or  # noqa: E501
+                                                        local_var_params['error_unknown'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `error_unknown` when calling `liveness_metadata`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'transaction_id' in local_var_params and local_var_params['transaction_id'] is not None:  # noqa: E501
-            query_params.append(('transactionId', local_var_params['transaction_id']))  # noqa: E501
+        if 'error_unknown' in local_var_params and local_var_params['error_unknown'] is not None:  # noqa: E501
+            query_params.append(('', local_var_params['error_unknown']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -290,25 +161,25 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def liveness_portrait(self, transaction_id, **kwargs):  # noqa: E501
-        """portrait  # noqa: E501
+    def liveness_portrait(self, error_unknown, **kwargs):  # noqa: E501
+        """Liveness 2.0 portrait  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_portrait(transaction_id, async_req=True)
+        >>> thread = api.liveness_portrait(error_unknown, async_req=True)
         >>> result = thread.get()
 
-        :param transaction_id: ID of the current liveness transaction. (required)
-        :type transaction_id: int
+        :param error_unknown: ID of the current liveness transaction. (required)
+        :type error_unknown: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -317,27 +188,27 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: file_type
         """
         kwargs['_return_http_data_only'] = True
-        return self.liveness_portrait_with_http_info(transaction_id, **kwargs)  # noqa: E501
+        return self.liveness_portrait_with_http_info(error_unknown, **kwargs)  # noqa: E501
 
-    def liveness_portrait_with_http_info(self, transaction_id, **kwargs):  # noqa: E501
-        """portrait  # noqa: E501
+    def liveness_portrait_with_http_info(self, error_unknown, **kwargs):  # noqa: E501
+        """Liveness 2.0 portrait  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_portrait_with_http_info(transaction_id, async_req=True)
+        >>> thread = api.liveness_portrait_with_http_info(error_unknown, async_req=True)
         >>> result = thread.get()
 
-        :param transaction_id: ID of the current liveness transaction. (required)
-        :type transaction_id: int
+        :param error_unknown: ID of the current liveness transaction. (required)
+        :type error_unknown: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -356,15 +227,15 @@
                  returns the request thread.
         :rtype: tuple(file_type, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'transaction_id'
+            'error_unknown'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -376,26 +247,26 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method liveness_portrait" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'transaction_id' is set
-        if self.api_client.client_side_validation and ('transaction_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['transaction_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `transaction_id` when calling `liveness_portrait`")  # noqa: E501
+        # verify the required parameter 'error_unknown' is set
+        if self.api_client.client_side_validation and ('error_unknown' not in local_var_params or  # noqa: E501
+                                                        local_var_params['error_unknown'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `error_unknown` when calling `liveness_portrait`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'transaction_id' in local_var_params and local_var_params['transaction_id'] is not None:  # noqa: E501
-            query_params.append(('transactionId', local_var_params['transaction_id']))  # noqa: E501
+        if 'error_unknown' in local_var_params and local_var_params['error_unknown'] is not None:  # noqa: E501
+            query_params.append(('', local_var_params['error_unknown']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -419,25 +290,25 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def liveness_video(self, transaction_id, **kwargs):  # noqa: E501
-        """video  # noqa: E501
+    def liveness_video(self, error_unknown, **kwargs):  # noqa: E501
+        """Liveness 2.0 video  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_video(transaction_id, async_req=True)
+        >>> thread = api.liveness_video(error_unknown, async_req=True)
         >>> result = thread.get()
 
-        :param transaction_id: ID of the current liveness transaction. (required)
-        :type transaction_id: int
+        :param error_unknown: ID of the current liveness transaction. (required)
+        :type error_unknown: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -446,27 +317,27 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: file_type
         """
         kwargs['_return_http_data_only'] = True
-        return self.liveness_video_with_http_info(transaction_id, **kwargs)  # noqa: E501
+        return self.liveness_video_with_http_info(error_unknown, **kwargs)  # noqa: E501
 
-    def liveness_video_with_http_info(self, transaction_id, **kwargs):  # noqa: E501
-        """video  # noqa: E501
+    def liveness_video_with_http_info(self, error_unknown, **kwargs):  # noqa: E501
+        """Liveness 2.0 video  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_video_with_http_info(transaction_id, async_req=True)
+        >>> thread = api.liveness_video_with_http_info(error_unknown, async_req=True)
         >>> result = thread.get()
 
-        :param transaction_id: ID of the current liveness transaction. (required)
-        :type transaction_id: int
+        :param error_unknown: ID of the current liveness transaction. (required)
+        :type error_unknown: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -485,15 +356,15 @@
                  returns the request thread.
         :rtype: tuple(file_type, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'transaction_id'
+            'error_unknown'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -505,26 +376,26 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method liveness_video" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'transaction_id' is set
-        if self.api_client.client_side_validation and ('transaction_id' not in local_var_params or  # noqa: E501
-                                                        local_var_params['transaction_id'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `transaction_id` when calling `liveness_video`")  # noqa: E501
+        # verify the required parameter 'error_unknown' is set
+        if self.api_client.client_side_validation and ('error_unknown' not in local_var_params or  # noqa: E501
+                                                        local_var_params['error_unknown'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `error_unknown` when calling `liveness_video`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'transaction_id' in local_var_params and local_var_params['transaction_id'] is not None:  # noqa: E501
-            query_params.append(('transactionId', local_var_params['transaction_id']))  # noqa: E501
+        if 'error_unknown' in local_var_params and local_var_params['error_unknown'] is not None:  # noqa: E501
+            query_params.append(('', local_var_params['error_unknown']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/liveness_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/matching_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -20,66 +20,70 @@
 from regula.facesdk.webclient.gen.api_client import ApiClient
 from regula.facesdk.webclient.gen.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class LivenessApi(object):
+class MatchingApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def liveness_metadata(self, error_unknown, **kwargs):  # noqa: E501
-        """Liveness 2.0 metadata  # noqa: E501
+    def detect(self, detect_request, **kwargs):  # noqa: E501
+        """Detect facial coordinates  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_metadata(error_unknown, async_req=True)
+        >>> thread = api.detect(detect_request, async_req=True)
         >>> result = thread.get()
 
-        :param error_unknown: ID of the current liveness transaction. (required)
-        :type error_unknown: int
+        :param detect_request: (required)
+        :type detect_request: DetectRequest
+        :param x_request_id:
+        :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :rtype: DetectResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.liveness_metadata_with_http_info(error_unknown, **kwargs)  # noqa: E501
+        return self.detect_with_http_info(detect_request, **kwargs)  # noqa: E501
 
-    def liveness_metadata_with_http_info(self, error_unknown, **kwargs):  # noqa: E501
-        """Liveness 2.0 metadata  # noqa: E501
+    def detect_with_http_info(self, detect_request, **kwargs):  # noqa: E501
+        """Detect facial coordinates  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_metadata_with_http_info(error_unknown, async_req=True)
+        >>> thread = api.detect_with_http_info(detect_request, async_req=True)
         >>> result = thread.get()
 
-        :param error_unknown: ID of the current liveness transaction. (required)
-        :type error_unknown: int
+        :param detect_request: (required)
+        :type detect_request: DetectRequest
+        :param x_request_id:
+        :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -92,21 +96,22 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(DetectResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'error_unknown'
+            'detect_request'
+            'x_request_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -114,101 +119,111 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method liveness_metadata" % key
+                    " to method detect" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'error_unknown' is set
-        if self.api_client.client_side_validation and ('error_unknown' not in local_var_params or  # noqa: E501
-                                                        local_var_params['error_unknown'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `error_unknown` when calling `liveness_metadata`")  # noqa: E501
+        # verify the required parameter 'detect_request' is set
+        if self.api_client.client_side_validation and ('detect_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['detect_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `detect_request` when calling `detect`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'error_unknown' in local_var_params and local_var_params['error_unknown'] is not None:  # noqa: E501
-            query_params.append(('', local_var_params['error_unknown']))  # noqa: E501
 
         header_params = {}
+        if 'x_request_id' in local_var_params:
+            header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'detect_request' in local_var_params:
+            body_params = local_var_params['detect_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json''application/octet-stream'])  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/v2/liveness/metadata', 'GET',
+            '/api/detect', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',  # noqa: E501
+            response_type='DetectResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def liveness_portrait(self, error_unknown, **kwargs):  # noqa: E501
-        """Liveness 2.0 portrait  # noqa: E501
+    def match(self, match_request, **kwargs):  # noqa: E501
+        """Compare provided face images in all combinations and return the similarity score for each pair.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_portrait(error_unknown, async_req=True)
+        >>> thread = api.match(match_request, async_req=True)
         >>> result = thread.get()
 
-        :param error_unknown: ID of the current liveness transaction. (required)
-        :type error_unknown: int
+        :param match_request: (required)
+        :type match_request: MatchRequest
+        :param x_request_id:
+        :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: file_type
+        :rtype: MatchResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.liveness_portrait_with_http_info(error_unknown, **kwargs)  # noqa: E501
+        return self.match_with_http_info(match_request, **kwargs)  # noqa: E501
 
-    def liveness_portrait_with_http_info(self, error_unknown, **kwargs):  # noqa: E501
-        """Liveness 2.0 portrait  # noqa: E501
+    def match_with_http_info(self, match_request, **kwargs):  # noqa: E501
+        """Compare provided face images in all combinations and return the similarity score for each pair.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_portrait_with_http_info(error_unknown, async_req=True)
+        >>> thread = api.match_with_http_info(match_request, async_req=True)
         >>> result = thread.get()
 
-        :param error_unknown: ID of the current liveness transaction. (required)
-        :type error_unknown: int
+        :param match_request: (required)
+        :type match_request: MatchRequest
+        :param x_request_id:
+        :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -221,21 +236,22 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(file_type, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(MatchResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'error_unknown'
+            'match_request'
+            'x_request_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -243,101 +259,111 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method liveness_portrait" % key
+                    " to method match" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'error_unknown' is set
-        if self.api_client.client_side_validation and ('error_unknown' not in local_var_params or  # noqa: E501
-                                                        local_var_params['error_unknown'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `error_unknown` when calling `liveness_portrait`")  # noqa: E501
+        # verify the required parameter 'match_request' is set
+        if self.api_client.client_side_validation and ('match_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['match_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `match_request` when calling `match`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'error_unknown' in local_var_params and local_var_params['error_unknown'] is not None:  # noqa: E501
-            query_params.append(('', local_var_params['error_unknown']))  # noqa: E501
 
         header_params = {}
+        if 'x_request_id' in local_var_params:
+            header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'match_request' in local_var_params:
+            body_params = local_var_params['match_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/octet-stream'])  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/v2/liveness/portrait', 'GET',
+            '/api/match', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='file_type',  # noqa: E501
+            response_type='MatchResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def liveness_video(self, error_unknown, **kwargs):  # noqa: E501
-        """Liveness 2.0 video  # noqa: E501
+    def match_and_search(self, match_and_search_request, **kwargs):  # noqa: E501
+        """Match and Search in one request  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_video(error_unknown, async_req=True)
+        >>> thread = api.match_and_search(match_and_search_request, async_req=True)
         >>> result = thread.get()
 
-        :param error_unknown: ID of the current liveness transaction. (required)
-        :type error_unknown: int
+        :param match_and_search_request: (required)
+        :type match_and_search_request: MatchAndSearchRequest
+        :param x_request_id:
+        :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: file_type
+        :rtype: MatchAndSearchResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self.liveness_video_with_http_info(error_unknown, **kwargs)  # noqa: E501
+        return self.match_and_search_with_http_info(match_and_search_request, **kwargs)  # noqa: E501
 
-    def liveness_video_with_http_info(self, error_unknown, **kwargs):  # noqa: E501
-        """Liveness 2.0 video  # noqa: E501
+    def match_and_search_with_http_info(self, match_and_search_request, **kwargs):  # noqa: E501
+        """Match and Search in one request  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.liveness_video_with_http_info(error_unknown, async_req=True)
+        >>> thread = api.match_and_search_with_http_info(match_and_search_request, async_req=True)
         >>> result = thread.get()
 
-        :param error_unknown: ID of the current liveness transaction. (required)
-        :type error_unknown: int
+        :param match_and_search_request: (required)
+        :type match_and_search_request: MatchAndSearchRequest
+        :param x_request_id:
+        :type x_request_id: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -350,21 +376,22 @@
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(file_type, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(MatchAndSearchResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
-            'error_unknown'
+            'match_and_search_request'
+            'x_request_id'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -372,53 +399,59 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method liveness_video" % key
+                    " to method match_and_search" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'error_unknown' is set
-        if self.api_client.client_side_validation and ('error_unknown' not in local_var_params or  # noqa: E501
-                                                        local_var_params['error_unknown'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `error_unknown` when calling `liveness_video`")  # noqa: E501
+        # verify the required parameter 'match_and_search_request' is set
+        if self.api_client.client_side_validation and ('match_and_search_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['match_and_search_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `match_and_search_request` when calling `match_and_search`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'error_unknown' in local_var_params and local_var_params['error_unknown'] is not None:  # noqa: E501
-            query_params.append(('', local_var_params['error_unknown']))  # noqa: E501
 
         header_params = {}
+        if 'x_request_id' in local_var_params:
+            header_params['X-RequestID'] = local_var_params['x_request_id']  # noqa: E501
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'match_and_search_request' in local_var_params:
+            body_params = local_var_params['match_and_search_request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/octet-stream'])  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         return self.api_client.call_api(
-            '/api/v2/liveness/video', 'GET',
+            '/api/match_and_search', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='file_type',  # noqa: E501
+            response_type='MatchAndSearchResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/person_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/person_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api/search_api.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api/search_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/api_client.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/apis/__init__.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/configuration.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -375,15 +375,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.1.3\n"\
+               "Version of the API: 5.1.0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/exceptions.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/crop.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/crop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detect_request.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -34,52 +34,47 @@
     """
     openapi_types = {
         'tag': 'str',
         'process_param': 'ProcessParam',
         'image': 'str',
         'thumbnails': 'bool',
         'attributes': 'bool',
-        'only_central_face': 'bool',
     }
 
     attribute_map = {
         'tag': 'tag',
         'process_param': 'processParam',
         'image': 'image',
         'thumbnails': 'thumbnails',
         'attributes': 'attributes',
-        'only_central_face': 'onlyCentralFace',
     }
 
-    def __init__(self, tag=None, process_param=None, image=None, thumbnails=False, attributes=False, only_central_face=False, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, tag=None, process_param=None, image=None, thumbnails=False, attributes=False, local_vars_configuration=None):  # noqa: E501
         """DetectRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._tag = None
         self._process_param = None
         self._image = None
         self._thumbnails = None
         self._attributes = None
-        self._only_central_face = None
         self.discriminator = None
 
         if tag is not None:
             self.tag = tag
         if process_param is not None:
             self.process_param = process_param
         if image is not None:
             self.image = image
         if thumbnails is not None:
             self.thumbnails = thumbnails
         if attributes is not None:
             self.attributes = attributes
-        if only_central_face is not None:
-            self.only_central_face = only_central_face
 
     @property
     def tag(self):
         """Gets the tag of this DetectRequest.  # noqa: E501
 
         Session identificator.  # noqa: E501
 
@@ -186,37 +181,14 @@
 
         :param attributes: The attributes of this DetectRequest.  # noqa: E501
         :type attributes: bool
         """
 
         self._attributes = attributes
 
-    @property
-    def only_central_face(self):
-        """Gets the only_central_face of this DetectRequest.  # noqa: E501
-
-        Whether to detect the only central face (true) or all the faces (false).  # noqa: E501
-
-        :return: The only_central_face of this DetectRequest.  # noqa: E501
-        :rtype: bool
-        """
-        return self._only_central_face
-
-    @only_central_face.setter
-    def only_central_face(self, only_central_face):
-        """Sets the only_central_face of this DetectRequest.
-
-        Whether to detect the only central face (true) or all the faces (false).  # noqa: E501
-
-        :param only_central_face: The only_central_face of this DetectRequest.  # noqa: E501
-        :type only_central_face: bool
-        """
-
-        self._only_central_face = only_central_face
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detect_response.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detect_response_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_response_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detect_result.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detect_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detection.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detection_face.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection_face.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/detection_quality.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/detection_quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_align_type_quality.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_align_type_quality.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_image_quality_align_type.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_align_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_image_quality_groups.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_image_quality_status.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_image_quality_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_quality_config_name.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_config_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_quality_scenarios.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_scenarios.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_quality_status.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_quality_status.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_rectangular.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_rectangular.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_sdk_result.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_sdk_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/face_sdk_result_code.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/face_sdk_result_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/faces_response.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/faces_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/faces_response_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/faces_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group_page.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group_page_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_page_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/group_to_create.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/group_to_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_fields.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_fields_image.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_fields_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_page.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_page_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_page_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/image_source.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/image_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/liveness_transaction.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/liveness_transaction.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_request.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_request_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_request_all_of_images.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_request_all_of_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_response.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_response_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_and_search_response_all_of_detections.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_and_search_response_all_of_detections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_image.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_image_detection.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_image_result.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_image_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_request.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_response.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/match_response_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/match_response_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/operation_log.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/operation_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/output_image_params.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/output_image_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/page.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person_fields.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person_with_images.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_with_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/person_with_images_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/person_with_images_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/persons_page.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/persons_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/persons_page_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/persons_page_all_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/process_param.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/process_param.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -33,43 +33,48 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'scenario': 'FaceQualityScenarios',
         'only_central_face': 'bool',
         'output_image_params': 'OutputImageParams',
         'quality': 'QualityRequest',
+        'attributes': 'bool',
     }
 
     attribute_map = {
         'scenario': 'scenario',
         'only_central_face': 'onlyCentralFace',
         'output_image_params': 'outputImageParams',
         'quality': 'quality',
+        'attributes': 'attributes',
     }
 
-    def __init__(self, scenario=None, only_central_face=None, output_image_params=None, quality=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, scenario=None, only_central_face=None, output_image_params=None, quality=None, attributes=False, local_vars_configuration=None):  # noqa: E501
         """ProcessParam - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._scenario = None
         self._only_central_face = None
         self._output_image_params = None
         self._quality = None
+        self._attributes = None
         self.discriminator = None
 
         if scenario is not None:
             self.scenario = scenario
         if only_central_face is not None:
             self.only_central_face = only_central_face
         if output_image_params is not None:
             self.output_image_params = output_image_params
         if quality is not None:
             self.quality = quality
+        if attributes is not None:
+            self.attributes = attributes
 
     @property
     def scenario(self):
         """Gets the scenario of this ProcessParam.  # noqa: E501
 
 
         :return: The scenario of this ProcessParam.  # noqa: E501
@@ -149,14 +154,37 @@
 
         :param quality: The quality of this ProcessParam.  # noqa: E501
         :type quality: QualityRequest
         """
 
         self._quality = quality
 
+    @property
+    def attributes(self):
+        """Gets the attributes of this ProcessParam.  # noqa: E501
+
+        Whether to evaluate attributes, such as age and emotions.  # noqa: E501
+
+        :return: The attributes of this ProcessParam.  # noqa: E501
+        :rtype: bool
+        """
+        return self._attributes
+
+    @attributes.setter
+    def attributes(self, attributes):
+        """Sets the attributes of this ProcessParam.
+
+        Whether to evaluate attributes, such as age and emotions.  # noqa: E501
+
+        :param attributes: The attributes of this ProcessParam.  # noqa: E501
+        :type attributes: bool
+        """
+
+        self._attributes = attributes
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_config.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_config_list.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/transaction_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class QualityConfigList(object):
+class TransactionConfig(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,15 +35,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """QualityConfigList - a model defined in OpenAPI"""  # noqa: E501
+        """TransactionConfig - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -75,18 +75,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, QualityConfigList):
+        if not isinstance(other, TransactionConfig):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, QualityConfigList):
+        if not isinstance(other, TransactionConfig):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_detail.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_details_groups.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_details_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/quality_request.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/recognize_image.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/recognize_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/recognize_image_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/recognize_image_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/rgb.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/rgb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_parameters.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_person.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_person.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_person_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_person_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_request.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_request_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_request_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_result.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/search_result_all_of.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/search_result_all_of.py`

 * *Files identical despite different names*

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/transaction_config.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/quality_config_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from regula.facesdk.webclient.gen.configuration import Configuration
 
 
-class TransactionConfig(object):
+class QualityConfigList(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,15 +35,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """TransactionConfig - a model defined in OpenAPI"""  # noqa: E501
+        """QualityConfigList - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -75,18 +75,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TransactionConfig):
+        if not isinstance(other, QualityConfigList):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, TransactionConfig):
+        if not isinstance(other, QualityConfigList):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model/update_group.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model/update_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/model_utils.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/models/__init__.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from regula.facesdk.webclient.gen.model.group_to_create import GroupToCreate
 from regula.facesdk.webclient.gen.model.image import Image
 from regula.facesdk.webclient.gen.model.image_fields import ImageFields
 from regula.facesdk.webclient.gen.model.image_fields_image import ImageFieldsImage
 from regula.facesdk.webclient.gen.model.image_page import ImagePage
 from regula.facesdk.webclient.gen.model.image_page_all_of import ImagePageAllOf
 from regula.facesdk.webclient.gen.model.image_source import ImageSource
-from regula.facesdk.webclient.gen.model.liveness_transaction import LivenessTransaction
 from regula.facesdk.webclient.gen.model.match_and_search_request import MatchAndSearchRequest
 from regula.facesdk.webclient.gen.model.match_and_search_request_all_of import MatchAndSearchRequestAllOf
 from regula.facesdk.webclient.gen.model.match_and_search_request_all_of_images import MatchAndSearchRequestAllOfImages
 from regula.facesdk.webclient.gen.model.match_and_search_response import MatchAndSearchResponse
 from regula.facesdk.webclient.gen.model.match_and_search_response_all_of import MatchAndSearchResponseAllOf
 from regula.facesdk.webclient.gen.model.match_and_search_response_all_of_detections import MatchAndSearchResponseAllOfDetections
 from regula.facesdk.webclient.gen.model.match_image import MatchImage
@@ -71,9 +70,9 @@
 from regula.facesdk.webclient.gen.model.recognize_image import RecognizeImage
 from regula.facesdk.webclient.gen.model.recognize_image_all_of import RecognizeImageAllOf
 from regula.facesdk.webclient.gen.model.search_parameters import SearchParameters
 from regula.facesdk.webclient.gen.model.search_person import SearchPerson
 from regula.facesdk.webclient.gen.model.search_person_all_of import SearchPersonAllOf
 from regula.facesdk.webclient.gen.model.search_request import SearchRequest
 from regula.facesdk.webclient.gen.model.search_result import SearchResult
-from regula.facesdk.webclient.gen.model.transaction_config import TransactionConfig
+from regula.facesdk.webclient.gen.model.transaction_info import TransactionInfo
 from regula.facesdk.webclient.gen.model.update_group import UpdateGroup
```

### Comparing `regula.facesdk.webclient-5.1.0/regula/facesdk/webclient/gen/rest.py` & `regula.facesdk.webclient-5.1.1/regula/facesdk/webclient/gen/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Regula FaceSDK Web API
 
     Regula FaceSDK Web API # Clients * [JavaScript](https://github.com/regulaforensics/FaceSDK-web-js-client) client for the browser and node.js based on axios * [Java](https://github.com/regulaforensics/FaceSDK-web-java-client) client compatible with jvm and android * [Python](https://github.com/regulaforensics/FaceSDK-web-python-client) 3.5+ client * [C#](https://github.com/regulaforensics/FaceSDK-web-csharp-client) client for .NET & .NET Core   # noqa: E501
 
-    The version of the OpenAPI document: 4.1.3
+    The version of the OpenAPI document: 5.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `regula.facesdk.webclient-5.1.0/regula.facesdk.webclient.egg-info/PKG-INFO` & `regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regula.facesdk.webclient
-Version: 5.1.0
+Version: 5.1.1
 Summary: Regula's FaceSDK web python client
 Home-page: https://mobile.regulaforensics.com
 Author: Regula Forensics, Inc.
 Author-email: support@regulaforensics.com
 Keywords: face recognition,facesdk,regulaforensics,regula
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `regula.facesdk.webclient-5.1.0/regula.facesdk.webclient.egg-info/SOURCES.txt` & `regula.facesdk.webclient-5.1.1/regula.facesdk.webclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -102,9 +102,10 @@
 regula/facesdk/webclient/gen/model/search_person.py
 regula/facesdk/webclient/gen/model/search_person_all_of.py
 regula/facesdk/webclient/gen/model/search_request.py
 regula/facesdk/webclient/gen/model/search_request_all_of.py
 regula/facesdk/webclient/gen/model/search_result.py
 regula/facesdk/webclient/gen/model/search_result_all_of.py
 regula/facesdk/webclient/gen/model/transaction_config.py
+regula/facesdk/webclient/gen/model/transaction_info.py
 regula/facesdk/webclient/gen/model/update_group.py
 regula/facesdk/webclient/gen/models/__init__.py
```

### Comparing `regula.facesdk.webclient-5.1.0/setup.py` & `regula.facesdk.webclient-5.1.1/setup.py`

 * *Files identical despite different names*

