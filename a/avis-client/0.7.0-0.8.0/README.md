# Comparing `tmp/avis_client-0.7.0.tar.gz` & `tmp/avis_client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avis_client-0.7.0.tar", max compression
+gzip compressed data, was "avis_client-0.8.0.tar", max compression
```

## Comparing `avis_client-0.7.0.tar` & `avis_client-0.8.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0    11364 2024-03-07 03:22:14.745539 avis_client-0.7.0/LICENSE
--rw-r--r--   0        0        0    21680 2024-04-09 13:30:25.744450 avis_client-0.7.0/README.md
--rw-r--r--   0        0        0     8054 2024-04-09 13:30:25.744450 avis_client-0.7.0/avis_client/__init__.py
--rw-r--r--   0        0        0     1018 2024-04-09 13:30:25.744450 avis_client-0.7.0/avis_client/api/__init__.py
--rw-r--r--   0        0        0    22842 2024-04-09 13:30:25.744450 avis_client-0.7.0/avis_client/api/api_keys_api.py
--rw-r--r--   0        0        0    75618 2024-04-09 13:30:25.744450 avis_client-0.7.0/avis_client/api/configuration_api.py
--rw-r--r--   0        0        0   105986 2024-04-09 13:30:25.748450 avis_client-0.7.0/avis_client/api/image_api.py
--rw-r--r--   0        0        0    75484 2024-04-09 13:30:25.748450 avis_client-0.7.0/avis_client/api/image_attribute_api.py
--rw-r--r--   0        0        0    77200 2024-04-09 13:30:25.748450 avis_client-0.7.0/avis_client/api/image_attribute_category_api.py
--rw-r--r--   0        0        0   113930 2024-04-09 13:30:25.748450 avis_client-0.7.0/avis_client/api/inspection_api.py
--rw-r--r--   0        0        0    63041 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/membership_api.py
--rw-r--r--   0        0        0    74160 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/metadata_api.py
--rw-r--r--   0        0        0    75484 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/metadata_schema_api.py
--rw-r--r--   0        0        0   143687 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/ml_api.py
--rw-r--r--   0        0        0    75912 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/product_api.py
--rw-r--r--   0        0        0    75680 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/product_category_api.py
--rw-r--r--   0        0        0    75680 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/quality_criteria_api.py
--rw-r--r--   0        0        0    73768 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/result_api.py
--rw-r--r--   0        0        0   109694 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/statistics_api.py
--rw-r--r--   0        0        0    62209 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/teams_api.py
--rw-r--r--   0        0        0    19541 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/user_api.py
--rw-r--r--   0        0        0    24532 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api_client.py
--rw-r--r--   0        0        0      674 2024-03-07 03:22:12.093504 avis_client-0.7.0/avis_client/api_response.py
--rw-r--r--   0        0        0    15507 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/configuration.py
--rw-r--r--   0        0        0     5910 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/exceptions.py
--rw-r--r--   0        0        0     6567 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/__init__.py
--rw-r--r--   0        0        0     3135 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/azure_ml_inference_request.py
--rw-r--r--   0        0        0      746 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/blank_enum.py
--rw-r--r--   0        0        0     4794 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/configuration_type.py
--rw-r--r--   0        0        0     3968 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/configuration_type_request.py
--rw-r--r--   0        0        0     2869 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/custom_user.py
--rw-r--r--   0        0        0     2757 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/custom_user_request.py
--rw-r--r--   0        0        0     2841 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/email_address.py
--rw-r--r--   0        0        0      947 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/format_enum.py
--rw-r--r--   0        0        0     4782 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image.py
--rw-r--r--   0        0        0     3897 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_attribute.py
--rw-r--r--   0        0        0     3953 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_attribute_category.py
--rw-r--r--   0        0        0     3021 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_attribute_category_request.py
--rw-r--r--   0        0        0     2965 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_attribute_request.py
--rw-r--r--   0        0        0     3919 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_request.py
--rw-r--r--   0        0        0     5778 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection.py
--rw-r--r--   0        0        0     2524 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_images_statistics.py
--rw-r--r--   0        0        0     2552 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_images_statistics_request.py
--rw-r--r--   0        0        0     4447 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_request.py
--rw-r--r--   0        0        0     2770 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_statistics.py
--rw-r--r--   0        0        0     2798 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_statistics_request.py
--rw-r--r--   0        0        0     2530 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_status.py
--rw-r--r--   0        0        0      845 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_status_enum.py
--rw-r--r--   0        0        0     2570 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_validation_status.py
--rw-r--r--   0        0        0     3841 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/membership.py
--rw-r--r--   0        0        0     2434 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/membership_request.py
--rw-r--r--   0        0        0     3804 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/metadata.py
--rw-r--r--   0        0        0     2872 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/metadata_request.py
--rw-r--r--   0        0        0     3630 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/metadata_schema.py
--rw-r--r--   0        0        0     2698 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/metadata_schema_request.py
--rw-r--r--   0        0        0     4120 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/ml_model.py
--rw-r--r--   0        0        0     3330 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/ml_model_request.py
--rw-r--r--   0        0        0     4641 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/ml_model_type.py
--rw-r--r--   0        0        0     3698 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/ml_model_type_request.py
--rw-r--r--   0        0        0     3602 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_configuration_type_list.py
--rw-r--r--   0        0        0     3643 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_image_attribute_category_list.py
--rw-r--r--   0        0        0     3578 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_image_attribute_list.py
--rw-r--r--   0        0        0     3505 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_image_list.py
--rw-r--r--   0        0        0     3675 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_images_statistics_list.py
--rw-r--r--   0        0        0     3545 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_list.py
--rw-r--r--   0        0        0     3626 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_statistics_list.py
--rw-r--r--   0        0        0     3594 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_status_list.py
--rw-r--r--   0        0        0     3675 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_validation_status_list.py
--rw-r--r--   0        0        0     3545 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_membership_list.py
--rw-r--r--   0        0        0     3529 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_metadata_list.py
--rw-r--r--   0        0        0     3578 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_metadata_schema_list.py
--rw-r--r--   0        0        0     3522 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_ml_model_list.py
--rw-r--r--   0        0        0     3555 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_ml_model_type_list.py
--rw-r--r--   0        0        0     3586 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_product_category_list.py
--rw-r--r--   0        0        0     3521 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_product_list.py
--rw-r--r--   0        0        0     3586 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_quality_criteria_list.py
--rw-r--r--   0        0        0     3635 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_quality_criteria_result_list.py
--rw-r--r--   0        0        0     3513 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_result_list.py
--rw-r--r--   0        0        0     3497 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_team_list.py
--rw-r--r--   0        0        0     4030 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_configuration_type_request.py
--rw-r--r--   0        0        0     3066 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_image_attribute_category_request.py
--rw-r--r--   0        0        0     3017 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_image_attribute_request.py
--rw-r--r--   0        0        0     3998 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_image_request.py
--rw-r--r--   0        0        0     4492 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_inspection_request.py
--rw-r--r--   0        0        0     2941 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_metadata_request.py
--rw-r--r--   0        0        0     2757 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_metadata_schema_request.py
--rw-r--r--   0        0        0     3382 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_ml_model_request.py
--rw-r--r--   0        0        0     3726 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_ml_model_type_request.py
--rw-r--r--   0        0        0     3219 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_product_category_request.py
--rw-r--r--   0        0        0     3532 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_product_request.py
--rw-r--r--   0        0        0     3198 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_quality_criteria_request.py
--rw-r--r--   0        0        0     4141 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_result_request.py
--rw-r--r--   0        0        0     5266 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_result_request_status.py
--rw-r--r--   0        0        0     4402 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/product.py
--rw-r--r--   0        0        0     4106 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/product_category.py
--rw-r--r--   0        0        0     3174 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/product_category_request.py
--rw-r--r--   0        0        0     3470 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/product_request.py
--rw-r--r--   0        0        0     3861 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/quality_criteria.py
--rw-r--r--   0        0        0     3102 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/quality_criteria_request.py
--rw-r--r--   0        0        0     2595 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/quality_criteria_result.py
--rw-r--r--   0        0        0      843 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/quality_enum.py
--rw-r--r--   0        0        0     5028 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/result.py
--rw-r--r--   0        0        0     4096 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/result_request.py
--rw-r--r--   0        0        0      857 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/status_enum.py
--rw-r--r--   0        0        0     4599 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/team.py
--rw-r--r--   0        0        0     3535 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/team_request.py
--rw-r--r--   0        0        0     3528 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/user_api_key_create.py
--rw-r--r--   0        0        0     2603 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/user_api_key_create_request.py
--rw-r--r--   0        0        0      896 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/validation_status_enum.py
--rw-r--r--   0        0        0        0 2024-03-07 03:22:12.085504 avis_client-0.7.0/avis_client/py.typed
--rw-r--r--   0        0        0     9749 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/rest.py
--rw-r--r--   0        0        0      904 2024-04-09 13:30:25.768449 avis_client-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    22666 1970-01-01 00:00:00.000000 avis_client-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11364 2024-05-14 13:59:08.245888 avis_client-0.8.0/LICENSE
+-rw-r--r--   0        0        0    22256 2024-05-14 13:59:03.762719 avis_client-0.8.0/README.md
+-rw-r--r--   0        0        0     8102 2024-05-14 13:59:03.778716 avis_client-0.8.0/avis_client/__init__.py
+-rw-r--r--   0        0        0     1018 2024-05-14 13:59:03.782715 avis_client-0.8.0/avis_client/api/__init__.py
+-rw-r--r--   0        0        0    22842 2024-05-14 13:59:03.414784 avis_client-0.8.0/avis_client/api/api_keys_api.py
+-rw-r--r--   0        0        0    75618 2024-05-14 13:59:03.434780 avis_client-0.8.0/avis_client/api/configuration_api.py
+-rw-r--r--   0        0        0    91977 2024-05-14 13:59:03.454776 avis_client-0.8.0/avis_client/api/image_api.py
+-rw-r--r--   0        0        0    75484 2024-05-14 13:59:03.478772 avis_client-0.8.0/avis_client/api/image_attribute_api.py
+-rw-r--r--   0        0        0    77200 2024-05-14 13:59:03.498768 avis_client-0.8.0/avis_client/api/image_attribute_category_api.py
+-rw-r--r--   0        0        0    99987 2024-05-14 13:59:03.518764 avis_client-0.8.0/avis_client/api/inspection_api.py
+-rw-r--r--   0        0        0    54026 2024-05-14 13:59:03.534761 avis_client-0.8.0/avis_client/api/membership_api.py
+-rw-r--r--   0        0        0    74160 2024-05-14 13:59:03.554758 avis_client-0.8.0/avis_client/api/metadata_api.py
+-rw-r--r--   0        0        0    75484 2024-05-14 13:59:03.570755 avis_client-0.8.0/avis_client/api/metadata_schema_api.py
+-rw-r--r--   0        0        0   143687 2024-05-14 13:59:03.590751 avis_client-0.8.0/avis_client/api/ml_api.py
+-rw-r--r--   0        0        0    75912 2024-05-14 13:59:03.614746 avis_client-0.8.0/avis_client/api/product_api.py
+-rw-r--r--   0        0        0    75680 2024-05-14 13:59:03.634743 avis_client-0.8.0/avis_client/api/product_category_api.py
+-rw-r--r--   0        0        0    75680 2024-05-14 13:59:03.658738 avis_client-0.8.0/avis_client/api/quality_criteria_api.py
+-rw-r--r--   0        0        0    73768 2024-05-14 13:59:03.686733 avis_client-0.8.0/avis_client/api/result_api.py
+-rw-r--r--   0        0        0   165716 2024-05-14 13:59:03.714728 avis_client-0.8.0/avis_client/api/statistics_api.py
+-rw-r--r--   0        0        0    53194 2024-05-14 13:59:03.734724 avis_client-0.8.0/avis_client/api/teams_api.py
+-rw-r--r--   0        0        0    19541 2024-05-14 13:59:03.750721 avis_client-0.8.0/avis_client/api/user_api.py
+-rw-r--r--   0        0        0    24532 2024-05-14 13:59:03.786714 avis_client-0.8.0/avis_client/api_client.py
+-rw-r--r--   0        0        0      674 2024-05-14 13:59:03.786714 avis_client-0.8.0/avis_client/api_response.py
+-rw-r--r--   0        0        0    15507 2024-05-14 13:59:03.778716 avis_client-0.8.0/avis_client/configuration.py
+-rw-r--r--   0        0        0     5910 2024-05-14 13:59:03.782715 avis_client-0.8.0/avis_client/exceptions.py
+-rw-r--r--   0        0        0     6615 2024-05-14 13:59:03.782715 avis_client-0.8.0/avis_client/models/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-14 13:59:02.231006 avis_client-0.8.0/avis_client/models/azure_ml_inference_request.py
+-rw-r--r--   0        0        0      746 2024-05-14 13:59:02.255002 avis_client-0.8.0/avis_client/models/blank_enum.py
+-rw-r--r--   0        0        0     2701 2024-05-14 13:59:02.278997 avis_client-0.8.0/avis_client/models/configuration_statistics.py
+-rw-r--r--   0        0        0     2729 2024-05-14 13:59:02.298994 avis_client-0.8.0/avis_client/models/configuration_statistics_request.py
+-rw-r--r--   0        0        0     4913 2024-05-14 13:59:02.322989 avis_client-0.8.0/avis_client/models/configuration_type.py
+-rw-r--r--   0        0        0     4087 2024-05-14 13:59:02.342985 avis_client-0.8.0/avis_client/models/configuration_type_request.py
+-rw-r--r--   0        0        0     2869 2024-05-14 13:59:02.354983 avis_client-0.8.0/avis_client/models/custom_user.py
+-rw-r--r--   0        0        0     2757 2024-05-14 13:59:02.362982 avis_client-0.8.0/avis_client/models/custom_user_request.py
+-rw-r--r--   0        0        0     2841 2024-05-14 13:59:02.374979 avis_client-0.8.0/avis_client/models/email_address.py
+-rw-r--r--   0        0        0      947 2024-05-14 13:59:02.378979 avis_client-0.8.0/avis_client/models/format_enum.py
+-rw-r--r--   0        0        0     4782 2024-05-14 13:59:02.390976 avis_client-0.8.0/avis_client/models/image.py
+-rw-r--r--   0        0        0     3897 2024-05-14 13:59:02.398975 avis_client-0.8.0/avis_client/models/image_attribute.py
+-rw-r--r--   0        0        0     3953 2024-05-14 13:59:02.406973 avis_client-0.8.0/avis_client/models/image_attribute_category.py
+-rw-r--r--   0        0        0     3021 2024-05-14 13:59:02.414972 avis_client-0.8.0/avis_client/models/image_attribute_category_request.py
+-rw-r--r--   0        0        0     2965 2024-05-14 13:59:02.426970 avis_client-0.8.0/avis_client/models/image_attribute_request.py
+-rw-r--r--   0        0        0     3919 2024-05-14 13:59:02.434968 avis_client-0.8.0/avis_client/models/image_request.py
+-rw-r--r--   0        0        0     5778 2024-05-14 13:59:02.446966 avis_client-0.8.0/avis_client/models/inspection.py
+-rw-r--r--   0        0        0     2524 2024-05-14 13:59:02.454964 avis_client-0.8.0/avis_client/models/inspection_images_statistics.py
+-rw-r--r--   0        0        0     2552 2024-05-14 13:59:02.466962 avis_client-0.8.0/avis_client/models/inspection_images_statistics_request.py
+-rw-r--r--   0        0        0     4447 2024-05-14 13:59:02.474960 avis_client-0.8.0/avis_client/models/inspection_request.py
+-rw-r--r--   0        0        0     2770 2024-05-14 13:59:02.494957 avis_client-0.8.0/avis_client/models/inspection_statistics.py
+-rw-r--r--   0        0        0     2798 2024-05-14 13:59:02.502955 avis_client-0.8.0/avis_client/models/inspection_statistics_request.py
+-rw-r--r--   0        0        0     2570 2024-05-14 13:59:02.510954 avis_client-0.8.0/avis_client/models/inspection_validation_status.py
+-rw-r--r--   0        0        0     3841 2024-05-14 13:59:02.562944 avis_client-0.8.0/avis_client/models/membership.py
+-rw-r--r--   0        0        0     2434 2024-05-14 13:59:02.570942 avis_client-0.8.0/avis_client/models/membership_request.py
+-rw-r--r--   0        0        0     3804 2024-05-14 13:59:02.578941 avis_client-0.8.0/avis_client/models/metadata.py
+-rw-r--r--   0        0        0     2872 2024-05-14 13:59:02.590939 avis_client-0.8.0/avis_client/models/metadata_request.py
+-rw-r--r--   0        0        0     3630 2024-05-14 13:59:02.598937 avis_client-0.8.0/avis_client/models/metadata_schema.py
+-rw-r--r--   0        0        0     2698 2024-05-14 13:59:02.606936 avis_client-0.8.0/avis_client/models/metadata_schema_request.py
+-rw-r--r--   0        0        0     4120 2024-05-14 13:59:02.518952 avis_client-0.8.0/avis_client/models/ml_model.py
+-rw-r--r--   0        0        0     3330 2024-05-14 13:59:02.530950 avis_client-0.8.0/avis_client/models/ml_model_request.py
+-rw-r--r--   0        0        0     4641 2024-05-14 13:59:02.542948 avis_client-0.8.0/avis_client/models/ml_model_type.py
+-rw-r--r--   0        0        0     3698 2024-05-14 13:59:02.550946 avis_client-0.8.0/avis_client/models/ml_model_type_request.py
+-rw-r--r--   0        0        0     3616 2024-05-14 13:59:02.618933 avis_client-0.8.0/avis_client/models/paginated_configuration_statistics_list.py
+-rw-r--r--   0        0        0     3568 2024-05-14 13:59:02.626932 avis_client-0.8.0/avis_client/models/paginated_configuration_type_list.py
+-rw-r--r--   0        0        0     3609 2024-05-14 13:59:02.634930 avis_client-0.8.0/avis_client/models/paginated_image_attribute_category_list.py
+-rw-r--r--   0        0        0     3544 2024-05-14 13:59:02.642929 avis_client-0.8.0/avis_client/models/paginated_image_attribute_list.py
+-rw-r--r--   0        0        0     3471 2024-05-14 13:59:02.650927 avis_client-0.8.0/avis_client/models/paginated_image_list.py
+-rw-r--r--   0        0        0     3641 2024-05-14 13:59:02.662925 avis_client-0.8.0/avis_client/models/paginated_inspection_images_statistics_list.py
+-rw-r--r--   0        0        0     3511 2024-05-14 13:59:02.670924 avis_client-0.8.0/avis_client/models/paginated_inspection_list.py
+-rw-r--r--   0        0        0     3592 2024-05-14 13:59:02.682921 avis_client-0.8.0/avis_client/models/paginated_inspection_statistics_list.py
+-rw-r--r--   0        0        0     3641 2024-05-14 13:59:02.690920 avis_client-0.8.0/avis_client/models/paginated_inspection_validation_status_list.py
+-rw-r--r--   0        0        0     3511 2024-05-14 13:59:02.722914 avis_client-0.8.0/avis_client/models/paginated_membership_list.py
+-rw-r--r--   0        0        0     3495 2024-05-14 13:59:02.730912 avis_client-0.8.0/avis_client/models/paginated_metadata_list.py
+-rw-r--r--   0        0        0     3544 2024-05-14 13:59:02.738911 avis_client-0.8.0/avis_client/models/paginated_metadata_schema_list.py
+-rw-r--r--   0        0        0     3488 2024-05-14 13:59:02.702917 avis_client-0.8.0/avis_client/models/paginated_ml_model_list.py
+-rw-r--r--   0        0        0     3521 2024-05-14 13:59:02.714915 avis_client-0.8.0/avis_client/models/paginated_ml_model_type_list.py
+-rw-r--r--   0        0        0     3552 2024-05-14 13:59:02.746909 avis_client-0.8.0/avis_client/models/paginated_product_category_list.py
+-rw-r--r--   0        0        0     3487 2024-05-14 13:59:02.754908 avis_client-0.8.0/avis_client/models/paginated_product_list.py
+-rw-r--r--   0        0        0     3552 2024-05-14 13:59:02.766905 avis_client-0.8.0/avis_client/models/paginated_quality_criteria_list.py
+-rw-r--r--   0        0        0     3601 2024-05-14 13:59:02.774904 avis_client-0.8.0/avis_client/models/paginated_quality_criteria_result_list.py
+-rw-r--r--   0        0        0     3479 2024-05-14 13:59:02.786902 avis_client-0.8.0/avis_client/models/paginated_result_list.py
+-rw-r--r--   0        0        0     3463 2024-05-14 13:59:02.794900 avis_client-0.8.0/avis_client/models/paginated_team_list.py
+-rw-r--r--   0        0        0     4149 2024-05-14 13:59:02.802899 avis_client-0.8.0/avis_client/models/patched_configuration_type_request.py
+-rw-r--r--   0        0        0     3066 2024-05-14 13:59:02.810897 avis_client-0.8.0/avis_client/models/patched_image_attribute_category_request.py
+-rw-r--r--   0        0        0     3017 2024-05-14 13:59:02.818896 avis_client-0.8.0/avis_client/models/patched_image_attribute_request.py
+-rw-r--r--   0        0        0     3998 2024-05-14 13:59:02.830893 avis_client-0.8.0/avis_client/models/patched_image_request.py
+-rw-r--r--   0        0        0     4492 2024-05-14 13:59:02.838892 avis_client-0.8.0/avis_client/models/patched_inspection_request.py
+-rw-r--r--   0        0        0     2941 2024-05-14 13:59:02.866887 avis_client-0.8.0/avis_client/models/patched_metadata_request.py
+-rw-r--r--   0        0        0     2757 2024-05-14 13:59:02.874885 avis_client-0.8.0/avis_client/models/patched_metadata_schema_request.py
+-rw-r--r--   0        0        0     3382 2024-05-14 13:59:02.850890 avis_client-0.8.0/avis_client/models/patched_ml_model_request.py
+-rw-r--r--   0        0        0     3726 2024-05-14 13:59:02.858888 avis_client-0.8.0/avis_client/models/patched_ml_model_type_request.py
+-rw-r--r--   0        0        0     3219 2024-05-14 13:59:02.882884 avis_client-0.8.0/avis_client/models/patched_product_category_request.py
+-rw-r--r--   0        0        0     3532 2024-05-14 13:59:02.890882 avis_client-0.8.0/avis_client/models/patched_product_request.py
+-rw-r--r--   0        0        0     3198 2024-05-14 13:59:02.898881 avis_client-0.8.0/avis_client/models/patched_quality_criteria_request.py
+-rw-r--r--   0        0        0     4141 2024-05-14 13:59:02.906879 avis_client-0.8.0/avis_client/models/patched_result_request.py
+-rw-r--r--   0        0        0     5266 2024-05-14 13:59:02.914878 avis_client-0.8.0/avis_client/models/patched_result_request_status.py
+-rw-r--r--   0        0        0     4402 2024-05-14 13:59:02.922876 avis_client-0.8.0/avis_client/models/product.py
+-rw-r--r--   0        0        0     4106 2024-05-14 13:59:02.930875 avis_client-0.8.0/avis_client/models/product_category.py
+-rw-r--r--   0        0        0     3174 2024-05-14 13:59:02.938873 avis_client-0.8.0/avis_client/models/product_category_request.py
+-rw-r--r--   0        0        0     3470 2024-05-14 13:59:02.942872 avis_client-0.8.0/avis_client/models/product_request.py
+-rw-r--r--   0        0        0     3861 2024-05-14 13:59:02.950871 avis_client-0.8.0/avis_client/models/quality_criteria.py
+-rw-r--r--   0        0        0     3102 2024-05-14 13:59:02.958869 avis_client-0.8.0/avis_client/models/quality_criteria_request.py
+-rw-r--r--   0        0        0     2595 2024-05-14 13:59:02.966868 avis_client-0.8.0/avis_client/models/quality_criteria_result.py
+-rw-r--r--   0        0        0      843 2024-05-14 13:59:02.970867 avis_client-0.8.0/avis_client/models/quality_enum.py
+-rw-r--r--   0        0        0     5028 2024-05-14 13:59:02.974866 avis_client-0.8.0/avis_client/models/result.py
+-rw-r--r--   0        0        0     4096 2024-05-14 13:59:02.982865 avis_client-0.8.0/avis_client/models/result_request.py
+-rw-r--r--   0        0        0      857 2024-05-14 13:59:02.986864 avis_client-0.8.0/avis_client/models/status_enum.py
+-rw-r--r--   0        0        0     4599 2024-05-14 13:59:02.994863 avis_client-0.8.0/avis_client/models/team.py
+-rw-r--r--   0        0        0     3535 2024-05-14 13:59:03.006860 avis_client-0.8.0/avis_client/models/team_request.py
+-rw-r--r--   0        0        0     3528 2024-05-14 13:59:03.014859 avis_client-0.8.0/avis_client/models/user_api_key_create.py
+-rw-r--r--   0        0        0     2603 2024-05-14 13:59:03.022857 avis_client-0.8.0/avis_client/models/user_api_key_create_request.py
+-rw-r--r--   0        0        0      896 2024-05-14 13:59:03.030856 avis_client-0.8.0/avis_client/models/validation_status_enum.py
+-rw-r--r--   0        0        0        0 2024-05-14 13:59:03.774716 avis_client-0.8.0/avis_client/py.typed
+-rw-r--r--   0        0        0     9749 2024-05-14 13:59:03.790713 avis_client-0.8.0/avis_client/rest.py
+-rw-r--r--   0        0        0      904 2024-05-14 13:59:08.213894 avis_client-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    23242 1970-01-01 00:00:00.000000 avis_client-0.8.0/PKG-INFO
```

### Comparing `avis_client-0.7.0/LICENSE` & `avis_client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avis_client-0.7.0/README.md` & `avis_client-0.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # avis-client
 VUE Autonomous Visual Inspection System (AVIS)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.7.0
-- Package version: 0.7.0
+- API version: 0.8.0
+- Package version: 0.8.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -106,15 +106,14 @@
 *ConfigurationApi* | [**configuration_destroy**](docs/ConfigurationApi.md#configuration_destroy) | **DELETE** /api/configuration/{id}/ | 
 *ConfigurationApi* | [**configuration_list**](docs/ConfigurationApi.md#configuration_list) | **GET** /api/configuration/ | 
 *ConfigurationApi* | [**configuration_partial_update**](docs/ConfigurationApi.md#configuration_partial_update) | **PATCH** /api/configuration/{id}/ | 
 *ConfigurationApi* | [**configuration_retrieve**](docs/ConfigurationApi.md#configuration_retrieve) | **GET** /api/configuration/{id}/ | 
 *ConfigurationApi* | [**configuration_update**](docs/ConfigurationApi.md#configuration_update) | **PUT** /api/configuration/{id}/ | 
 *ImageApi* | [**image_create**](docs/ImageApi.md#image_create) | **POST** /api/image/ | 
 *ImageApi* | [**image_destroy**](docs/ImageApi.md#image_destroy) | **DELETE** /api/image/{id}/ | 
-*ImageApi* | [**image_inspection_status_list**](docs/ImageApi.md#image_inspection_status_list) | **GET** /api/image/inspection_status/ | 
 *ImageApi* | [**image_list**](docs/ImageApi.md#image_list) | **GET** /api/image/ | 
 *ImageApi* | [**image_partial_update**](docs/ImageApi.md#image_partial_update) | **PATCH** /api/image/{id}/ | 
 *ImageApi* | [**image_quality_list**](docs/ImageApi.md#image_quality_list) | **GET** /api/image/quality/ | 
 *ImageApi* | [**image_retrieve**](docs/ImageApi.md#image_retrieve) | **GET** /api/image/{id}/ | 
 *ImageApi* | [**image_update**](docs/ImageApi.md#image_update) | **PUT** /api/image/{id}/ | 
 *ImageAttributeApi* | [**image_attribute_create**](docs/ImageAttributeApi.md#image_attribute_create) | **POST** /api/image-attribute/ | 
 *ImageAttributeApi* | [**image_attribute_destroy**](docs/ImageAttributeApi.md#image_attribute_destroy) | **DELETE** /api/image-attribute/{id}/ | 
@@ -130,15 +129,14 @@
 *ImageAttributeCategoryApi* | [**image_attribute_category_update**](docs/ImageAttributeCategoryApi.md#image_attribute_category_update) | **PUT** /api/image-attribute-category/{id}/ | 
 *InspectionApi* | [**inspection_create**](docs/InspectionApi.md#inspection_create) | **POST** /api/inspection/ | 
 *InspectionApi* | [**inspection_destroy**](docs/InspectionApi.md#inspection_destroy) | **DELETE** /api/inspection/{id}/ | 
 *InspectionApi* | [**inspection_list**](docs/InspectionApi.md#inspection_list) | **GET** /api/inspection/ | 
 *InspectionApi* | [**inspection_partial_update**](docs/InspectionApi.md#inspection_partial_update) | **PATCH** /api/inspection/{id}/ | 
 *InspectionApi* | [**inspection_retrieve**](docs/InspectionApi.md#inspection_retrieve) | **GET** /api/inspection/{id}/ | 
 *InspectionApi* | [**inspection_send_validation_email_retrieve**](docs/InspectionApi.md#inspection_send_validation_email_retrieve) | **GET** /api/inspection/{id}/send_validation_email/ | 
-*InspectionApi* | [**inspection_status_list**](docs/InspectionApi.md#inspection_status_list) | **GET** /api/inspection/status/ | 
 *InspectionApi* | [**inspection_update**](docs/InspectionApi.md#inspection_update) | **PUT** /api/inspection/{id}/ | 
 *InspectionApi* | [**inspection_validation_status_list**](docs/InspectionApi.md#inspection_validation_status_list) | **GET** /api/inspection/validation_status/ | 
 *MembershipApi* | [**membership_create**](docs/MembershipApi.md#membership_create) | **POST** /api/membership/ | 
 *MembershipApi* | [**membership_destroy**](docs/MembershipApi.md#membership_destroy) | **DELETE** /api/membership/{id}/ | 
 *MembershipApi* | [**membership_list**](docs/MembershipApi.md#membership_list) | **GET** /api/membership/ | 
 *MembershipApi* | [**membership_retrieve**](docs/MembershipApi.md#membership_retrieve) | **GET** /api/membership/{id}/ | 
 *MembershipApi* | [**membership_update**](docs/MembershipApi.md#membership_update) | **PUT** /api/membership/{id}/ | 
@@ -187,14 +185,19 @@
 *QualityCriteriaApi* | [**quality_criteria_update**](docs/QualityCriteriaApi.md#quality_criteria_update) | **PUT** /api/quality-criteria/{id}/ | 
 *ResultApi* | [**result_create**](docs/ResultApi.md#result_create) | **POST** /api/result/ | 
 *ResultApi* | [**result_destroy**](docs/ResultApi.md#result_destroy) | **DELETE** /api/result/{id}/ | 
 *ResultApi* | [**result_list**](docs/ResultApi.md#result_list) | **GET** /api/result/ | 
 *ResultApi* | [**result_partial_update**](docs/ResultApi.md#result_partial_update) | **PATCH** /api/result/{id}/ | 
 *ResultApi* | [**result_retrieve**](docs/ResultApi.md#result_retrieve) | **GET** /api/result/{id}/ | 
 *ResultApi* | [**result_update**](docs/ResultApi.md#result_update) | **PUT** /api/result/{id}/ | 
+*StatisticsApi* | [**statistics_configuration_create**](docs/StatisticsApi.md#statistics_configuration_create) | **POST** /api/statistics/configuration/ | 
+*StatisticsApi* | [**statistics_configuration_destroy**](docs/StatisticsApi.md#statistics_configuration_destroy) | **DELETE** /api/statistics/configuration/{id}/ | 
+*StatisticsApi* | [**statistics_configuration_list**](docs/StatisticsApi.md#statistics_configuration_list) | **GET** /api/statistics/configuration/ | 
+*StatisticsApi* | [**statistics_configuration_retrieve**](docs/StatisticsApi.md#statistics_configuration_retrieve) | **GET** /api/statistics/configuration/{id}/ | 
+*StatisticsApi* | [**statistics_configuration_update**](docs/StatisticsApi.md#statistics_configuration_update) | **PUT** /api/statistics/configuration/{id}/ | 
 *StatisticsApi* | [**statistics_inspection_create**](docs/StatisticsApi.md#statistics_inspection_create) | **POST** /api/statistics/inspection/ | 
 *StatisticsApi* | [**statistics_inspection_destroy**](docs/StatisticsApi.md#statistics_inspection_destroy) | **DELETE** /api/statistics/inspection/{id}/ | 
 *StatisticsApi* | [**statistics_inspection_list**](docs/StatisticsApi.md#statistics_inspection_list) | **GET** /api/statistics/inspection/ | 
 *StatisticsApi* | [**statistics_inspection_retrieve**](docs/StatisticsApi.md#statistics_inspection_retrieve) | **GET** /api/statistics/inspection/{id}/ | 
 *StatisticsApi* | [**statistics_inspection_update**](docs/StatisticsApi.md#statistics_inspection_update) | **PUT** /api/statistics/inspection/{id}/ | 
 *StatisticsApi* | [**statistics_team_create**](docs/StatisticsApi.md#statistics_team_create) | **POST** /api/statistics/team/ | 
 *StatisticsApi* | [**statistics_team_destroy**](docs/StatisticsApi.md#statistics_team_destroy) | **DELETE** /api/statistics/team/{id}/ | 
@@ -210,14 +213,16 @@
 *UserApi* | [**user_whoami_retrieve**](docs/UserApi.md#user_whoami_retrieve) | **GET** /api/user/whoami/ | 
 
 
 ## Documentation For Models
 
  - [AzureMLInferenceRequest](docs/AzureMLInferenceRequest.md)
  - [BlankEnum](docs/BlankEnum.md)
+ - [ConfigurationStatistics](docs/ConfigurationStatistics.md)
+ - [ConfigurationStatisticsRequest](docs/ConfigurationStatisticsRequest.md)
  - [ConfigurationType](docs/ConfigurationType.md)
  - [ConfigurationTypeRequest](docs/ConfigurationTypeRequest.md)
  - [CustomUser](docs/CustomUser.md)
  - [CustomUserRequest](docs/CustomUserRequest.md)
  - [EmailAddress](docs/EmailAddress.md)
  - [FormatEnum](docs/FormatEnum.md)
  - [Image](docs/Image.md)
@@ -228,35 +233,33 @@
  - [ImageRequest](docs/ImageRequest.md)
  - [Inspection](docs/Inspection.md)
  - [InspectionImagesStatistics](docs/InspectionImagesStatistics.md)
  - [InspectionImagesStatisticsRequest](docs/InspectionImagesStatisticsRequest.md)
  - [InspectionRequest](docs/InspectionRequest.md)
  - [InspectionStatistics](docs/InspectionStatistics.md)
  - [InspectionStatisticsRequest](docs/InspectionStatisticsRequest.md)
- - [InspectionStatus](docs/InspectionStatus.md)
- - [InspectionStatusEnum](docs/InspectionStatusEnum.md)
  - [InspectionValidationStatus](docs/InspectionValidationStatus.md)
  - [MLModel](docs/MLModel.md)
  - [MLModelRequest](docs/MLModelRequest.md)
  - [MLModelType](docs/MLModelType.md)
  - [MLModelTypeRequest](docs/MLModelTypeRequest.md)
  - [Membership](docs/Membership.md)
  - [MembershipRequest](docs/MembershipRequest.md)
  - [Metadata](docs/Metadata.md)
  - [MetadataRequest](docs/MetadataRequest.md)
  - [MetadataSchema](docs/MetadataSchema.md)
  - [MetadataSchemaRequest](docs/MetadataSchemaRequest.md)
+ - [PaginatedConfigurationStatisticsList](docs/PaginatedConfigurationStatisticsList.md)
  - [PaginatedConfigurationTypeList](docs/PaginatedConfigurationTypeList.md)
  - [PaginatedImageAttributeCategoryList](docs/PaginatedImageAttributeCategoryList.md)
  - [PaginatedImageAttributeList](docs/PaginatedImageAttributeList.md)
  - [PaginatedImageList](docs/PaginatedImageList.md)
  - [PaginatedInspectionImagesStatisticsList](docs/PaginatedInspectionImagesStatisticsList.md)
  - [PaginatedInspectionList](docs/PaginatedInspectionList.md)
  - [PaginatedInspectionStatisticsList](docs/PaginatedInspectionStatisticsList.md)
- - [PaginatedInspectionStatusList](docs/PaginatedInspectionStatusList.md)
  - [PaginatedInspectionValidationStatusList](docs/PaginatedInspectionValidationStatusList.md)
  - [PaginatedMLModelList](docs/PaginatedMLModelList.md)
  - [PaginatedMLModelTypeList](docs/PaginatedMLModelTypeList.md)
  - [PaginatedMembershipList](docs/PaginatedMembershipList.md)
  - [PaginatedMetadataList](docs/PaginatedMetadataList.md)
  - [PaginatedMetadataSchemaList](docs/PaginatedMetadataSchemaList.md)
  - [PaginatedProductCategoryList](docs/PaginatedProductCategoryList.md)
```

### Comparing `avis_client-0.7.0/avis_client/__init__.py` & `avis_client-0.8.0/avis_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 # import apis into sdk package
 from avis_client.api.api_keys_api import ApiKeysApi
 from avis_client.api.configuration_api import ConfigurationApi
 from avis_client.api.image_api import ImageApi
 from avis_client.api.image_attribute_api import ImageAttributeApi
 from avis_client.api.image_attribute_category_api import ImageAttributeCategoryApi
@@ -45,14 +45,16 @@
 from avis_client.exceptions import ApiKeyError
 from avis_client.exceptions import ApiAttributeError
 from avis_client.exceptions import ApiException
 
 # import models into sdk package
 from avis_client.models.azure_ml_inference_request import AzureMLInferenceRequest
 from avis_client.models.blank_enum import BlankEnum
+from avis_client.models.configuration_statistics import ConfigurationStatistics
+from avis_client.models.configuration_statistics_request import ConfigurationStatisticsRequest
 from avis_client.models.configuration_type import ConfigurationType
 from avis_client.models.configuration_type_request import ConfigurationTypeRequest
 from avis_client.models.custom_user import CustomUser
 from avis_client.models.custom_user_request import CustomUserRequest
 from avis_client.models.email_address import EmailAddress
 from avis_client.models.format_enum import FormatEnum
 from avis_client.models.image import Image
@@ -63,35 +65,33 @@
 from avis_client.models.image_request import ImageRequest
 from avis_client.models.inspection import Inspection
 from avis_client.models.inspection_images_statistics import InspectionImagesStatistics
 from avis_client.models.inspection_images_statistics_request import InspectionImagesStatisticsRequest
 from avis_client.models.inspection_request import InspectionRequest
 from avis_client.models.inspection_statistics import InspectionStatistics
 from avis_client.models.inspection_statistics_request import InspectionStatisticsRequest
-from avis_client.models.inspection_status import InspectionStatus
-from avis_client.models.inspection_status_enum import InspectionStatusEnum
 from avis_client.models.inspection_validation_status import InspectionValidationStatus
 from avis_client.models.ml_model import MLModel
 from avis_client.models.ml_model_request import MLModelRequest
 from avis_client.models.ml_model_type import MLModelType
 from avis_client.models.ml_model_type_request import MLModelTypeRequest
 from avis_client.models.membership import Membership
 from avis_client.models.membership_request import MembershipRequest
 from avis_client.models.metadata import Metadata
 from avis_client.models.metadata_request import MetadataRequest
 from avis_client.models.metadata_schema import MetadataSchema
 from avis_client.models.metadata_schema_request import MetadataSchemaRequest
+from avis_client.models.paginated_configuration_statistics_list import PaginatedConfigurationStatisticsList
 from avis_client.models.paginated_configuration_type_list import PaginatedConfigurationTypeList
 from avis_client.models.paginated_image_attribute_category_list import PaginatedImageAttributeCategoryList
 from avis_client.models.paginated_image_attribute_list import PaginatedImageAttributeList
 from avis_client.models.paginated_image_list import PaginatedImageList
 from avis_client.models.paginated_inspection_images_statistics_list import PaginatedInspectionImagesStatisticsList
 from avis_client.models.paginated_inspection_list import PaginatedInspectionList
 from avis_client.models.paginated_inspection_statistics_list import PaginatedInspectionStatisticsList
-from avis_client.models.paginated_inspection_status_list import PaginatedInspectionStatusList
 from avis_client.models.paginated_inspection_validation_status_list import PaginatedInspectionValidationStatusList
 from avis_client.models.paginated_ml_model_list import PaginatedMLModelList
 from avis_client.models.paginated_ml_model_type_list import PaginatedMLModelTypeList
 from avis_client.models.paginated_membership_list import PaginatedMembershipList
 from avis_client.models.paginated_metadata_list import PaginatedMetadataList
 from avis_client.models.paginated_metadata_schema_list import PaginatedMetadataSchemaList
 from avis_client.models.paginated_product_category_list import PaginatedProductCategoryList
```

### Comparing `avis_client-0.7.0/avis_client/api/__init__.py` & `avis_client-0.8.0/avis_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `avis_client-0.7.0/avis_client/api/api_keys_api.py` & `avis_client-0.8.0/avis_client/api/api_keys_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/configuration_api.py` & `avis_client-0.8.0/avis_client/api/configuration_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/image_api.py` & `avis_client-0.8.0/avis_client/api/image_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -31,15 +31,14 @@
 
 from typing import List, Optional, Union
 
 from avis_client.models.format_enum import FormatEnum
 from avis_client.models.image import Image
 from avis_client.models.image_request import ImageRequest
 from avis_client.models.paginated_image_list import PaginatedImageList
-from avis_client.models.paginated_inspection_status_list import PaginatedInspectionStatusList
 from avis_client.models.paginated_quality_criteria_result_list import PaginatedQualityCriteriaResultList
 from avis_client.models.patched_image_request import PatchedImageRequest
 from avis_client.models.validation_status_enum import ValidationStatusEnum
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
@@ -692,327 +691,14 @@
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def image_inspection_status_list(
-        self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
-        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
-        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> PaginatedInspectionStatusList:
-        """image_inspection_status_list
-
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
-
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
-        :param ordering: Which field to use when ordering the results.
-        :type ordering: str
-        :param page: A page number within the paginated result set.
-        :type page: int
-        :param page_size: Number of results to return per page.
-        :type page_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._image_inspection_status_list_serialize(
-            id=id,
-            ordering=ordering,
-            page=page,
-            page_size=page_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedInspectionStatusList",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def image_inspection_status_list_with_http_info(
-        self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
-        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
-        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[PaginatedInspectionStatusList]:
-        """image_inspection_status_list
-
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
-
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
-        :param ordering: Which field to use when ordering the results.
-        :type ordering: str
-        :param page: A page number within the paginated result set.
-        :type page: int
-        :param page_size: Number of results to return per page.
-        :type page_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._image_inspection_status_list_serialize(
-            id=id,
-            ordering=ordering,
-            page=page,
-            page_size=page_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedInspectionStatusList",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def image_inspection_status_list_without_preload_content(
-        self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
-        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
-        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """image_inspection_status_list
-
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
-
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
-        :param ordering: Which field to use when ordering the results.
-        :type ordering: str
-        :param page: A page number within the paginated result set.
-        :type page: int
-        :param page_size: Number of results to return per page.
-        :type page_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._image_inspection_status_list_serialize(
-            id=id,
-            ordering=ordering,
-            page=page,
-            page_size=page_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedInspectionStatusList",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _image_inspection_status_list_serialize(
-        self,
-        id,
-        ordering,
-        page,
-        page_size,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> Tuple:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-            'id': 'csv',
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        if id is not None:
-            
-            _query_params.append(('id', id))
-            
-        if ordering is not None:
-            
-            _query_params.append(('ordering', ordering))
-            
-        if page is not None:
-            
-            _query_params.append(('page', page))
-            
-        if page_size is not None:
-            
-            _query_params.append(('page_size', page_size))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'cookieAuth', 
-            'ApiKeyAuth'
-        ]
-
-        return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/image/inspection_status/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `avis_client-0.7.0/avis_client/api/image_attribute_api.py` & `avis_client-0.8.0/avis_client/api/image_attribute_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/image_attribute_category_api.py` & `avis_client-0.8.0/avis_client/api/image_attribute_category_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/inspection_api.py` & `avis_client-0.8.0/avis_client/api/inspection_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -28,15 +28,14 @@
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
 from avis_client.models.inspection import Inspection
 from avis_client.models.inspection_request import InspectionRequest
 from avis_client.models.paginated_inspection_list import PaginatedInspectionList
-from avis_client.models.paginated_inspection_status_list import PaginatedInspectionStatusList
 from avis_client.models.paginated_inspection_validation_status_list import PaginatedInspectionValidationStatusList
 from avis_client.models.patched_inspection_request import PatchedInspectionRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
@@ -1723,327 +1722,14 @@
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
-    def inspection_status_list(
-        self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
-        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
-        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> PaginatedInspectionStatusList:
-        """inspection_status_list
-
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
-
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
-        :param ordering: Which field to use when ordering the results.
-        :type ordering: str
-        :param page: A page number within the paginated result set.
-        :type page: int
-        :param page_size: Number of results to return per page.
-        :type page_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._inspection_status_list_serialize(
-            id=id,
-            ordering=ordering,
-            page=page,
-            page_size=page_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedInspectionStatusList",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def inspection_status_list_with_http_info(
-        self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
-        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
-        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[PaginatedInspectionStatusList]:
-        """inspection_status_list
-
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
-
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
-        :param ordering: Which field to use when ordering the results.
-        :type ordering: str
-        :param page: A page number within the paginated result set.
-        :type page: int
-        :param page_size: Number of results to return per page.
-        :type page_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._inspection_status_list_serialize(
-            id=id,
-            ordering=ordering,
-            page=page,
-            page_size=page_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedInspectionStatusList",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def inspection_status_list_without_preload_content(
-        self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
-        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
-        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
-        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """inspection_status_list
-
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
-
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
-        :param ordering: Which field to use when ordering the results.
-        :type ordering: str
-        :param page: A page number within the paginated result set.
-        :type page: int
-        :param page_size: Number of results to return per page.
-        :type page_size: int
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._inspection_status_list_serialize(
-            id=id,
-            ordering=ordering,
-            page=page,
-            page_size=page_size,
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedInspectionStatusList",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _inspection_status_list_serialize(
-        self,
-        id,
-        ordering,
-        page,
-        page_size,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> Tuple:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-            'id': 'csv',
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        if id is not None:
-            
-            _query_params.append(('id', id))
-            
-        if ordering is not None:
-            
-            _query_params.append(('ordering', ordering))
-            
-        if page is not None:
-            
-            _query_params.append(('page', page))
-            
-        if page_size is not None:
-            
-            _query_params.append(('page_size', page_size))
-            
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'cookieAuth', 
-            'ApiKeyAuth'
-        ]
-
-        return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/inspection/status/',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
             collection_formats=_collection_formats,
             _host=_host,
             _request_auth=_request_auth
         )
```

### Comparing `avis_client-0.7.0/avis_client/api/membership_api.py` & `avis_client-0.8.0/avis_client/api/metadata_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -21,63 +21,64 @@
 try:
     from typing import Annotated
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
-from pydantic import StrictInt
+from pydantic import StrictInt, StrictStr
 
-from typing import Optional
+from typing import List, Optional
 
-from avis_client.models.membership import Membership
-from avis_client.models.membership_request import MembershipRequest
-from avis_client.models.paginated_membership_list import PaginatedMembershipList
+from avis_client.models.metadata import Metadata
+from avis_client.models.metadata_request import MetadataRequest
+from avis_client.models.paginated_metadata_list import PaginatedMetadataList
+from avis_client.models.patched_metadata_request import PatchedMetadataRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
-class MembershipApi:
+class MetadataApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def membership_create(
+    def metadata_create(
         self,
-        membership_request: MembershipRequest,
+        metadata_request: MetadataRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Membership:
-        """membership_create
+    ) -> Metadata:
+        """metadata_create
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param membership_request: (required)
-        :type membership_request: MembershipRequest
+        :param metadata_request: (required)
+        :type metadata_request: MetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -92,59 +93,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_create_serialize(
-            membership_request=membership_request,
+        _param = self._metadata_create_serialize(
+            metadata_request=metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Membership",
+            '201': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def membership_create_with_http_info(
+    def metadata_create_with_http_info(
         self,
-        membership_request: MembershipRequest,
+        metadata_request: MetadataRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Membership]:
-        """membership_create
+    ) -> ApiResponse[Metadata]:
+        """metadata_create
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param membership_request: (required)
-        :type membership_request: MembershipRequest
+        :param metadata_request: (required)
+        :type metadata_request: MetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -159,59 +160,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_create_serialize(
-            membership_request=membership_request,
+        _param = self._metadata_create_serialize(
+            metadata_request=metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Membership",
+            '201': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def membership_create_without_preload_content(
+    def metadata_create_without_preload_content(
         self,
-        membership_request: MembershipRequest,
+        metadata_request: MetadataRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """membership_create
+        """metadata_create
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param membership_request: (required)
-        :type membership_request: MembershipRequest
+        :param metadata_request: (required)
+        :type metadata_request: MetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -226,35 +227,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_create_serialize(
-            membership_request=membership_request,
+        _param = self._metadata_create_serialize(
+            metadata_request=metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Membership",
+            '201': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _membership_create_serialize(
+    def _metadata_create_serialize(
         self,
-        membership_request,
+        metadata_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -270,16 +271,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if membership_request is not None:
-            _body_params = membership_request
+        if metadata_request is not None:
+            _body_params = metadata_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -305,15 +306,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/api/membership/',
+            resource_path='/api/metadata/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -322,35 +323,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def membership_destroy(
+    def metadata_destroy(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """membership_destroy
+        """metadata_destroy
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -366,15 +367,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_destroy_serialize(
+        _param = self._metadata_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -389,35 +390,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def membership_destroy_with_http_info(
+    def metadata_destroy_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """membership_destroy
+        """metadata_destroy
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -433,15 +434,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_destroy_serialize(
+        _param = self._metadata_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -456,35 +457,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def membership_destroy_without_preload_content(
+    def metadata_destroy_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """membership_destroy
+        """metadata_destroy
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -500,15 +501,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_destroy_serialize(
+        _param = self._metadata_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -518,15 +519,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _membership_destroy_serialize(
+    def _metadata_destroy_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -558,15 +559,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/api/membership/{id}/',
+            resource_path='/api/metadata/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -575,35 +576,44 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def membership_list(
+    def metadata_list(
         self,
+        fields: Optional[StrictStr] = None,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> PaginatedMembershipList:
-        """membership_list
+    ) -> PaginatedMetadataList:
+        """metadata_list
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param fields:
+        :type fields: str
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -622,59 +632,71 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_list_serialize(
+        _param = self._metadata_list_serialize(
+            fields=fields,
+            id=id,
+            ordering=ordering,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedMembershipList",
+            '200': "PaginatedMetadataList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def membership_list_with_http_info(
+    def metadata_list_with_http_info(
         self,
+        fields: Optional[StrictStr] = None,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[PaginatedMembershipList]:
-        """membership_list
+    ) -> ApiResponse[PaginatedMetadataList]:
+        """metadata_list
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param fields:
+        :type fields: str
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -693,40 +715,46 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_list_serialize(
+        _param = self._metadata_list_serialize(
+            fields=fields,
+            id=id,
+            ordering=ordering,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedMembershipList",
+            '200': "PaginatedMetadataList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def membership_list_without_preload_content(
+    def metadata_list_without_preload_content(
         self,
+        fields: Optional[StrictStr] = None,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -734,18 +762,24 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """membership_list
+        """metadata_list
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param fields:
+        :type fields: str
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -764,57 +798,76 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_list_serialize(
+        _param = self._metadata_list_serialize(
+            fields=fields,
+            id=id,
+            ordering=ordering,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedMembershipList",
+            '200': "PaginatedMetadataList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _membership_list_serialize(
+    def _metadata_list_serialize(
         self,
+        fields,
+        id,
+        ordering,
         page,
         page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
+            'id': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if fields is not None:
+            
+            _query_params.append(('fields', fields))
+            
+        if id is not None:
+            
+            _query_params.append(('id', id))
+            
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
         if page is not None:
             
             _query_params.append(('page', page))
             
         if page_size is not None:
             
             _query_params.append(('page_size', page_size))
@@ -836,15 +889,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/membership/',
+            resource_path='/api/metadata/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -853,36 +906,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def membership_retrieve(
+    def metadata_partial_update(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        patched_metadata_request: Optional[PatchedMetadataRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Membership:
-        """membership_retrieve
+    ) -> Metadata:
+        """metadata_partial_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
+        :param patched_metadata_request:
+        :type patched_metadata_request: PatchedMetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -897,59 +953,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_retrieve_serialize(
+        _param = self._metadata_partial_update_serialize(
             id=id,
+            patched_metadata_request=patched_metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Membership",
+            '200': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def membership_retrieve_with_http_info(
+    def metadata_partial_update_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        patched_metadata_request: Optional[PatchedMetadataRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Membership]:
-        """membership_retrieve
+    ) -> ApiResponse[Metadata]:
+        """metadata_partial_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
+        :param patched_metadata_request:
+        :type patched_metadata_request: PatchedMetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -964,59 +1024,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_retrieve_serialize(
+        _param = self._metadata_partial_update_serialize(
             id=id,
+            patched_metadata_request=patched_metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Membership",
+            '200': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def membership_retrieve_without_preload_content(
+    def metadata_partial_update_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        patched_metadata_request: Optional[PatchedMetadataRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """membership_retrieve
+        """metadata_partial_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
+        :param patched_metadata_request:
+        :type patched_metadata_request: PatchedMetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1031,35 +1095,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_retrieve_serialize(
+        _param = self._metadata_partial_update_serialize(
             id=id,
+            patched_metadata_request=patched_metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Membership",
+            '200': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _membership_retrieve_serialize(
+    def _metadata_partial_update_serialize(
         self,
         id,
+        patched_metadata_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1077,14 +1143,307 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if patched_metadata_request is not None:
+            _body_params = patched_metadata_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'cookieAuth', 
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='PATCH',
+            resource_path='/api/metadata/{id}/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def metadata_retrieve(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        fields: Optional[StrictStr] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Metadata:
+        """metadata_retrieve
+
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+
+        :param id: A unique integer value identifying this metadata. (required)
+        :type id: int
+        :param fields:
+        :type fields: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._metadata_retrieve_serialize(
+            id=id,
+            fields=fields,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Metadata",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def metadata_retrieve_with_http_info(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        fields: Optional[StrictStr] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[Metadata]:
+        """metadata_retrieve
+
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+
+        :param id: A unique integer value identifying this metadata. (required)
+        :type id: int
+        :param fields:
+        :type fields: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._metadata_retrieve_serialize(
+            id=id,
+            fields=fields,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Metadata",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def metadata_retrieve_without_preload_content(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        fields: Optional[StrictStr] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """metadata_retrieve
+
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+
+        :param id: A unique integer value identifying this metadata. (required)
+        :type id: int
+        :param fields:
+        :type fields: str
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._metadata_retrieve_serialize(
+            id=id,
+            fields=fields,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Metadata",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _metadata_retrieve_serialize(
+        self,
+        id,
+        fields,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        if fields is not None:
+            
+            _query_params.append(('fields', fields))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1095,15 +1454,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/membership/{id}/',
+            resource_path='/api/metadata/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1112,39 +1471,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def membership_update(
+    def metadata_update(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
-        membership_request: MembershipRequest,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        metadata_request: MetadataRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Membership:
-        """membership_update
+    ) -> Metadata:
+        """metadata_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
-        :param membership_request: (required)
-        :type membership_request: MembershipRequest
+        :param metadata_request: (required)
+        :type metadata_request: MetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1159,63 +1518,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_update_serialize(
+        _param = self._metadata_update_serialize(
             id=id,
-            membership_request=membership_request,
+            metadata_request=metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Membership",
+            '200': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def membership_update_with_http_info(
+    def metadata_update_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
-        membership_request: MembershipRequest,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        metadata_request: MetadataRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Membership]:
-        """membership_update
+    ) -> ApiResponse[Metadata]:
+        """metadata_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
-        :param membership_request: (required)
-        :type membership_request: MembershipRequest
+        :param metadata_request: (required)
+        :type metadata_request: MetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1230,63 +1589,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_update_serialize(
+        _param = self._metadata_update_serialize(
             id=id,
-            membership_request=membership_request,
+            metadata_request=metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Membership",
+            '200': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def membership_update_without_preload_content(
+    def metadata_update_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this membership.")],
-        membership_request: MembershipRequest,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        metadata_request: MetadataRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """membership_update
+        """metadata_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this membership. (required)
+        :param id: A unique integer value identifying this metadata. (required)
         :type id: int
-        :param membership_request: (required)
-        :type membership_request: MembershipRequest
+        :param metadata_request: (required)
+        :type metadata_request: MetadataRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1301,37 +1660,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._membership_update_serialize(
+        _param = self._metadata_update_serialize(
             id=id,
-            membership_request=membership_request,
+            metadata_request=metadata_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Membership",
+            '200': "Metadata",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _membership_update_serialize(
+    def _metadata_update_serialize(
         self,
         id,
-        membership_request,
+        metadata_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1349,16 +1708,16 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if membership_request is not None:
-            _body_params = membership_request
+        if metadata_request is not None:
+            _body_params = metadata_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1384,15 +1743,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
-            resource_path='/api/membership/{id}/',
+            resource_path='/api/metadata/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `avis_client-0.7.0/avis_client/api/metadata_api.py` & `avis_client-0.8.0/avis_client/api/result_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -25,60 +25,60 @@
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
-from avis_client.models.metadata import Metadata
-from avis_client.models.metadata_request import MetadataRequest
-from avis_client.models.paginated_metadata_list import PaginatedMetadataList
-from avis_client.models.patched_metadata_request import PatchedMetadataRequest
+from avis_client.models.paginated_result_list import PaginatedResultList
+from avis_client.models.patched_result_request import PatchedResultRequest
+from avis_client.models.result import Result
+from avis_client.models.result_request import ResultRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
-class MetadataApi:
+class ResultApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def metadata_create(
+    def result_create(
         self,
-        metadata_request: MetadataRequest,
+        result_request: ResultRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Metadata:
-        """metadata_create
+    ) -> Result:
+        """result_create
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param metadata_request: (required)
-        :type metadata_request: MetadataRequest
+        :param result_request: (required)
+        :type result_request: ResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -93,59 +93,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_create_serialize(
-            metadata_request=metadata_request,
+        _param = self._result_create_serialize(
+            result_request=result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Metadata",
+            '201': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def metadata_create_with_http_info(
+    def result_create_with_http_info(
         self,
-        metadata_request: MetadataRequest,
+        result_request: ResultRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Metadata]:
-        """metadata_create
+    ) -> ApiResponse[Result]:
+        """result_create
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param metadata_request: (required)
-        :type metadata_request: MetadataRequest
+        :param result_request: (required)
+        :type result_request: ResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -160,59 +160,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_create_serialize(
-            metadata_request=metadata_request,
+        _param = self._result_create_serialize(
+            result_request=result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Metadata",
+            '201': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def metadata_create_without_preload_content(
+    def result_create_without_preload_content(
         self,
-        metadata_request: MetadataRequest,
+        result_request: ResultRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """metadata_create
+        """result_create
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param metadata_request: (required)
-        :type metadata_request: MetadataRequest
+        :param result_request: (required)
+        :type result_request: ResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -227,35 +227,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_create_serialize(
-            metadata_request=metadata_request,
+        _param = self._result_create_serialize(
+            result_request=result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Metadata",
+            '201': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _metadata_create_serialize(
+    def _result_create_serialize(
         self,
-        metadata_request,
+        result_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -271,16 +271,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if metadata_request is not None:
-            _body_params = metadata_request
+        if result_request is not None:
+            _body_params = result_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -306,15 +306,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/api/metadata/',
+            resource_path='/api/result/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -323,35 +323,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def metadata_destroy(
+    def result_destroy(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """metadata_destroy
+        """result_destroy
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -367,15 +367,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_destroy_serialize(
+        _param = self._result_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -390,35 +390,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def metadata_destroy_with_http_info(
+    def result_destroy_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """metadata_destroy
+        """result_destroy
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -434,15 +434,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_destroy_serialize(
+        _param = self._result_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -457,35 +457,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def metadata_destroy_without_preload_content(
+    def result_destroy_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """metadata_destroy
+        """result_destroy
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -501,15 +501,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_destroy_serialize(
+        _param = self._result_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -519,15 +519,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _metadata_destroy_serialize(
+    def _result_destroy_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -559,15 +559,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/api/metadata/{id}/',
+            resource_path='/api/result/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -576,15 +576,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def metadata_list(
+    def result_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
@@ -595,16 +595,16 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> PaginatedMetadataList:
-        """metadata_list
+    ) -> PaginatedResultList:
+        """result_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
@@ -632,42 +632,42 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_list_serialize(
+        _param = self._result_list_serialize(
             fields=fields,
             id=id,
             ordering=ordering,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedMetadataList",
+            '200': "PaginatedResultList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def metadata_list_with_http_info(
+    def result_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
@@ -678,16 +678,16 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[PaginatedMetadataList]:
-        """metadata_list
+    ) -> ApiResponse[PaginatedResultList]:
+        """result_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
@@ -715,42 +715,42 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_list_serialize(
+        _param = self._result_list_serialize(
             fields=fields,
             id=id,
             ordering=ordering,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedMetadataList",
+            '200': "PaginatedResultList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def metadata_list_without_preload_content(
+    def result_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
@@ -762,15 +762,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """metadata_list
+        """result_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
@@ -798,37 +798,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_list_serialize(
+        _param = self._result_list_serialize(
             fields=fields,
             id=id,
             ordering=ordering,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "PaginatedMetadataList",
+            '200': "PaginatedResultList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _metadata_list_serialize(
+    def _result_list_serialize(
         self,
         fields,
         id,
         ordering,
         page,
         page_size,
         _request_auth,
@@ -889,15 +889,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/metadata/',
+            resource_path='/api/result/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -906,39 +906,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def metadata_partial_update(
+    def result_partial_update(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
-        patched_metadata_request: Optional[PatchedMetadataRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
+        patched_result_request: Optional[PatchedResultRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Metadata:
-        """metadata_partial_update
+    ) -> Result:
+        """result_partial_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
-        :param patched_metadata_request:
-        :type patched_metadata_request: PatchedMetadataRequest
+        :param patched_result_request:
+        :type patched_result_request: PatchedResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -953,63 +953,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_partial_update_serialize(
+        _param = self._result_partial_update_serialize(
             id=id,
-            patched_metadata_request=patched_metadata_request,
+            patched_result_request=patched_result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def metadata_partial_update_with_http_info(
+    def result_partial_update_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
-        patched_metadata_request: Optional[PatchedMetadataRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
+        patched_result_request: Optional[PatchedResultRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Metadata]:
-        """metadata_partial_update
+    ) -> ApiResponse[Result]:
+        """result_partial_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
-        :param patched_metadata_request:
-        :type patched_metadata_request: PatchedMetadataRequest
+        :param patched_result_request:
+        :type patched_result_request: PatchedResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1024,63 +1024,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_partial_update_serialize(
+        _param = self._result_partial_update_serialize(
             id=id,
-            patched_metadata_request=patched_metadata_request,
+            patched_result_request=patched_result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def metadata_partial_update_without_preload_content(
+    def result_partial_update_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
-        patched_metadata_request: Optional[PatchedMetadataRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
+        patched_result_request: Optional[PatchedResultRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """metadata_partial_update
+        """result_partial_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
-        :param patched_metadata_request:
-        :type patched_metadata_request: PatchedMetadataRequest
+        :param patched_result_request:
+        :type patched_result_request: PatchedResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1095,37 +1095,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_partial_update_serialize(
+        _param = self._result_partial_update_serialize(
             id=id,
-            patched_metadata_request=patched_metadata_request,
+            patched_result_request=patched_result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _metadata_partial_update_serialize(
+    def _result_partial_update_serialize(
         self,
         id,
-        patched_metadata_request,
+        patched_result_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1143,16 +1143,16 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if patched_metadata_request is not None:
-            _body_params = patched_metadata_request
+        if patched_result_request is not None:
+            _body_params = patched_result_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1178,15 +1178,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PATCH',
-            resource_path='/api/metadata/{id}/',
+            resource_path='/api/result/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1195,36 +1195,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def metadata_retrieve(
+    def result_retrieve(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
         fields: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Metadata:
-        """metadata_retrieve
+    ) -> Result:
+        """result_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
         :param fields:
         :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1242,60 +1242,60 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_retrieve_serialize(
+        _param = self._result_retrieve_serialize(
             id=id,
             fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def metadata_retrieve_with_http_info(
+    def result_retrieve_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
         fields: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Metadata]:
-        """metadata_retrieve
+    ) -> ApiResponse[Result]:
+        """result_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
         :param fields:
         :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1313,60 +1313,60 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_retrieve_serialize(
+        _param = self._result_retrieve_serialize(
             id=id,
             fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def metadata_retrieve_without_preload_content(
+    def result_retrieve_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
         fields: Optional[StrictStr] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """metadata_retrieve
+        """result_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
         :param fields:
         :type fields: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1384,34 +1384,34 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_retrieve_serialize(
+        _param = self._result_retrieve_serialize(
             id=id,
             fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _metadata_retrieve_serialize(
+    def _result_retrieve_serialize(
         self,
         id,
         fields,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
@@ -1454,15 +1454,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/metadata/{id}/',
+            resource_path='/api/result/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1471,39 +1471,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def metadata_update(
+    def result_update(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
-        metadata_request: MetadataRequest,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
+        result_request: ResultRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Metadata:
-        """metadata_update
+    ) -> Result:
+        """result_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
-        :param metadata_request: (required)
-        :type metadata_request: MetadataRequest
+        :param result_request: (required)
+        :type result_request: ResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1518,63 +1518,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_update_serialize(
+        _param = self._result_update_serialize(
             id=id,
-            metadata_request=metadata_request,
+            result_request=result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def metadata_update_with_http_info(
+    def result_update_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
-        metadata_request: MetadataRequest,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
+        result_request: ResultRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Metadata]:
-        """metadata_update
+    ) -> ApiResponse[Result]:
+        """result_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
-        :param metadata_request: (required)
-        :type metadata_request: MetadataRequest
+        :param result_request: (required)
+        :type result_request: ResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1589,63 +1589,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_update_serialize(
+        _param = self._result_update_serialize(
             id=id,
-            metadata_request=metadata_request,
+            result_request=result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def metadata_update_without_preload_content(
+    def result_update_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this metadata.")],
-        metadata_request: MetadataRequest,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this result.")],
+        result_request: ResultRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """metadata_update
+        """result_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this metadata. (required)
+        :param id: A unique integer value identifying this result. (required)
         :type id: int
-        :param metadata_request: (required)
-        :type metadata_request: MetadataRequest
+        :param result_request: (required)
+        :type result_request: ResultRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1660,37 +1660,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._metadata_update_serialize(
+        _param = self._result_update_serialize(
             id=id,
-            metadata_request=metadata_request,
+            result_request=result_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Metadata",
+            '200': "Result",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _metadata_update_serialize(
+    def _result_update_serialize(
         self,
         id,
-        metadata_request,
+        result_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1708,16 +1708,16 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if metadata_request is not None:
-            _body_params = metadata_request
+        if result_request is not None:
+            _body_params = result_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1743,15 +1743,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
-            resource_path='/api/metadata/{id}/',
+            resource_path='/api/result/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `avis_client-0.7.0/avis_client/api/metadata_schema_api.py` & `avis_client-0.8.0/avis_client/api/metadata_schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/ml_api.py` & `avis_client-0.8.0/avis_client/api/ml_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/product_api.py` & `avis_client-0.8.0/avis_client/api/product_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/product_category_api.py` & `avis_client-0.8.0/avis_client/api/product_category_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/quality_criteria_api.py` & `avis_client-0.8.0/avis_client/api/quality_criteria_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api/statistics_api.py` & `avis_client-0.8.0/avis_client/api/statistics_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -21,22 +21,25 @@
 try:
     from typing import Annotated
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
-from pydantic import StrictInt
+from pydantic import StrictInt, StrictStr
 
-from typing import Optional
+from typing import List, Optional
 
+from avis_client.models.configuration_statistics import ConfigurationStatistics
+from avis_client.models.configuration_statistics_request import ConfigurationStatisticsRequest
 from avis_client.models.inspection_images_statistics import InspectionImagesStatistics
 from avis_client.models.inspection_images_statistics_request import InspectionImagesStatisticsRequest
 from avis_client.models.inspection_statistics import InspectionStatistics
 from avis_client.models.inspection_statistics_request import InspectionStatisticsRequest
+from avis_client.models.paginated_configuration_statistics_list import PaginatedConfigurationStatisticsList
 from avis_client.models.paginated_inspection_images_statistics_list import PaginatedInspectionImagesStatisticsList
 from avis_client.models.paginated_inspection_statistics_list import PaginatedInspectionStatisticsList
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
@@ -51,14 +54,1402 @@
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
+    def statistics_configuration_create(
+        self,
+        configuration_statistics_request: ConfigurationStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ConfigurationStatistics:
+        """statistics_configuration_create
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param configuration_statistics_request: (required)
+        :type configuration_statistics_request: ConfigurationStatisticsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_create_serialize(
+            configuration_statistics_request=configuration_statistics_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '201': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def statistics_configuration_create_with_http_info(
+        self,
+        configuration_statistics_request: ConfigurationStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[ConfigurationStatistics]:
+        """statistics_configuration_create
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param configuration_statistics_request: (required)
+        :type configuration_statistics_request: ConfigurationStatisticsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_create_serialize(
+            configuration_statistics_request=configuration_statistics_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '201': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def statistics_configuration_create_without_preload_content(
+        self,
+        configuration_statistics_request: ConfigurationStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """statistics_configuration_create
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param configuration_statistics_request: (required)
+        :type configuration_statistics_request: ConfigurationStatisticsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_create_serialize(
+            configuration_statistics_request=configuration_statistics_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '201': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _statistics_configuration_create_serialize(
+        self,
+        configuration_statistics_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if configuration_statistics_request is not None:
+            _body_params = configuration_statistics_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'cookieAuth', 
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='POST',
+            resource_path='/api/statistics/configuration/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def statistics_configuration_destroy(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> None:
+        """statistics_configuration_destroy
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_destroy_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '204': None,
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def statistics_configuration_destroy_with_http_info(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[None]:
+        """statistics_configuration_destroy
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_destroy_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '204': None,
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def statistics_configuration_destroy_without_preload_content(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """statistics_configuration_destroy
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_destroy_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '204': None,
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _statistics_configuration_destroy_serialize(
+        self,
+        id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'cookieAuth', 
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='DELETE',
+            resource_path='/api/statistics/configuration/{id}/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def statistics_configuration_list(
+        self,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> PaginatedConfigurationStatisticsList:
+        """statistics_configuration_list
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_list_serialize(
+            id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaginatedConfigurationStatisticsList",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def statistics_configuration_list_with_http_info(
+        self,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[PaginatedConfigurationStatisticsList]:
+        """statistics_configuration_list
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_list_serialize(
+            id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaginatedConfigurationStatisticsList",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def statistics_configuration_list_without_preload_content(
+        self,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """statistics_configuration_list
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_list_serialize(
+            id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "PaginatedConfigurationStatisticsList",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _statistics_configuration_list_serialize(
+        self,
+        id,
+        ordering,
+        page,
+        page_size,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+            'id': 'csv',
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        # process the query parameters
+        if id is not None:
+            
+            _query_params.append(('id', id))
+            
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'cookieAuth', 
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/api/statistics/configuration/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def statistics_configuration_retrieve(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ConfigurationStatistics:
+        """statistics_configuration_retrieve
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_retrieve_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def statistics_configuration_retrieve_with_http_info(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[ConfigurationStatistics]:
+        """statistics_configuration_retrieve
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_retrieve_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def statistics_configuration_retrieve_without_preload_content(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """statistics_configuration_retrieve
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_retrieve_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _statistics_configuration_retrieve_serialize(
+        self,
+        id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'cookieAuth', 
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/api/statistics/configuration/{id}/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def statistics_configuration_update(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        configuration_statistics_request: ConfigurationStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ConfigurationStatistics:
+        """statistics_configuration_update
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param configuration_statistics_request: (required)
+        :type configuration_statistics_request: ConfigurationStatisticsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_update_serialize(
+            id=id,
+            configuration_statistics_request=configuration_statistics_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def statistics_configuration_update_with_http_info(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        configuration_statistics_request: ConfigurationStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[ConfigurationStatistics]:
+        """statistics_configuration_update
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param configuration_statistics_request: (required)
+        :type configuration_statistics_request: ConfigurationStatisticsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_update_serialize(
+            id=id,
+            configuration_statistics_request=configuration_statistics_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def statistics_configuration_update_without_preload_content(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this configuration.")],
+        configuration_statistics_request: ConfigurationStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """statistics_configuration_update
+
+        A mixin that allows reading entities (listing and retrieving by id).
+
+        :param id: A unique integer value identifying this configuration. (required)
+        :type id: int
+        :param configuration_statistics_request: (required)
+        :type configuration_statistics_request: ConfigurationStatisticsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_configuration_update_serialize(
+            id=id,
+            configuration_statistics_request=configuration_statistics_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "ConfigurationStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _statistics_configuration_update_serialize(
+        self,
+        id,
+        configuration_statistics_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if configuration_statistics_request is not None:
+            _body_params = configuration_statistics_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'cookieAuth', 
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='PUT',
+            resource_path='/api/statistics/configuration/{id}/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
     def statistics_inspection_create(
         self,
         inspection_images_statistics_request: InspectionImagesStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -69,15 +1460,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> InspectionImagesStatistics:
         """statistics_inspection_create
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param inspection_images_statistics_request: (required)
         :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -136,15 +1527,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[InspectionImagesStatistics]:
         """statistics_inspection_create
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param inspection_images_statistics_request: (required)
         :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -203,15 +1594,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_inspection_create
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param inspection_images_statistics_request: (required)
         :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -343,15 +1734,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """statistics_inspection_destroy
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -410,15 +1801,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """statistics_inspection_destroy
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -477,15 +1868,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_inspection_destroy
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -597,15 +1988,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PaginatedInspectionImagesStatisticsList:
         """statistics_inspection_list
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -668,15 +2059,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PaginatedInspectionImagesStatisticsList]:
         """statistics_inspection_list
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -739,15 +2130,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_inspection_list
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -874,15 +2265,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> InspectionImagesStatistics:
         """statistics_inspection_retrieve
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -941,15 +2332,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[InspectionImagesStatistics]:
         """statistics_inspection_retrieve
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1008,15 +2399,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_inspection_retrieve
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1134,15 +2525,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> InspectionImagesStatistics:
         """statistics_inspection_update
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param inspection_images_statistics_request: (required)
         :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1205,15 +2596,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[InspectionImagesStatistics]:
         """statistics_inspection_update
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param inspection_images_statistics_request: (required)
         :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1276,15 +2667,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_inspection_update
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param inspection_images_statistics_request: (required)
         :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1422,15 +2813,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> InspectionStatistics:
         """statistics_team_create
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param inspection_statistics_request: (required)
         :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1489,15 +2880,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[InspectionStatistics]:
         """statistics_team_create
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param inspection_statistics_request: (required)
         :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1556,15 +2947,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_team_create
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param inspection_statistics_request: (required)
         :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1696,15 +3087,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """statistics_team_destroy
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1763,15 +3154,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """statistics_team_destroy
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1830,15 +3221,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_team_destroy
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1950,15 +3341,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PaginatedInspectionStatisticsList:
         """statistics_team_list
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2021,15 +3412,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PaginatedInspectionStatisticsList]:
         """statistics_team_list
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2092,15 +3483,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_team_list
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2227,15 +3618,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> InspectionStatistics:
         """statistics_team_retrieve
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2294,15 +3685,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[InspectionStatistics]:
         """statistics_team_retrieve
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2361,15 +3752,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_team_retrieve
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -2487,15 +3878,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> InspectionStatistics:
         """statistics_team_update
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param inspection_statistics_request: (required)
         :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2558,15 +3949,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[InspectionStatistics]:
         """statistics_team_update
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param inspection_statistics_request: (required)
         :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -2629,15 +4020,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """statistics_team_update
 
-        Allows a Google Partial Response query param like to prune results
+        A mixin that only allows retrieving entities by id.
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param inspection_statistics_request: (required)
         :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `avis_client-0.7.0/avis_client/api/teams_api.py` & `avis_client-0.8.0/avis_client/api/teams_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -66,15 +66,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Team:
         """teams_create
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -133,15 +133,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Team]:
         """teams_create
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -200,15 +200,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """teams_create
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -340,15 +340,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
         """teams_destroy
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -407,15 +407,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
         """teams_destroy
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -474,15 +474,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """teams_destroy
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -594,15 +594,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> PaginatedTeamList:
         """teams_list
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -665,15 +665,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[PaginatedTeamList]:
         """teams_list
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -736,15 +736,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """teams_list
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
         :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -871,15 +871,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Team:
         """teams_retrieve
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -938,15 +938,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Team]:
         """teams_retrieve
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1005,15 +1005,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """teams_retrieve
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1131,15 +1131,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Team:
         """teams_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1202,15 +1202,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Team]:
         """teams_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -1273,15 +1273,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """teams_update
 
-        A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
+        A mixin that allows reading entities (listing and retrieving by id).
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
```

### Comparing `avis_client-0.7.0/avis_client/api/user_api.py` & `avis_client-0.8.0/avis_client/api/user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/avis_client/api_client.py` & `avis_client-0.8.0/avis_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -82,15 +82,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.7.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.8.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `avis_client-0.7.0/avis_client/api_response.py` & `avis_client-0.8.0/avis_client/api_response.py`

 * *Files identical despite different names*

### Comparing `avis_client-0.7.0/avis_client/configuration.py` & `avis_client-0.8.0/avis_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -401,16 +401,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.7.0\n"\
-               "SDK Package Version: 0.7.0".\
+               "Version of the API: 0.8.0\n"\
+               "SDK Package Version: 0.8.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `avis_client-0.7.0/avis_client/exceptions.py` & `avis_client-0.8.0/avis_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `avis_client-0.7.0/avis_client/models/__init__.py` & `avis_client-0.8.0/avis_client/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 # flake8: noqa
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from avis_client.models.azure_ml_inference_request import AzureMLInferenceRequest
 from avis_client.models.blank_enum import BlankEnum
+from avis_client.models.configuration_statistics import ConfigurationStatistics
+from avis_client.models.configuration_statistics_request import ConfigurationStatisticsRequest
 from avis_client.models.configuration_type import ConfigurationType
 from avis_client.models.configuration_type_request import ConfigurationTypeRequest
 from avis_client.models.custom_user import CustomUser
 from avis_client.models.custom_user_request import CustomUserRequest
 from avis_client.models.email_address import EmailAddress
 from avis_client.models.format_enum import FormatEnum
 from avis_client.models.image import Image
@@ -30,35 +32,33 @@
 from avis_client.models.image_request import ImageRequest
 from avis_client.models.inspection import Inspection
 from avis_client.models.inspection_images_statistics import InspectionImagesStatistics
 from avis_client.models.inspection_images_statistics_request import InspectionImagesStatisticsRequest
 from avis_client.models.inspection_request import InspectionRequest
 from avis_client.models.inspection_statistics import InspectionStatistics
 from avis_client.models.inspection_statistics_request import InspectionStatisticsRequest
-from avis_client.models.inspection_status import InspectionStatus
-from avis_client.models.inspection_status_enum import InspectionStatusEnum
 from avis_client.models.inspection_validation_status import InspectionValidationStatus
 from avis_client.models.ml_model import MLModel
 from avis_client.models.ml_model_request import MLModelRequest
 from avis_client.models.ml_model_type import MLModelType
 from avis_client.models.ml_model_type_request import MLModelTypeRequest
 from avis_client.models.membership import Membership
 from avis_client.models.membership_request import MembershipRequest
 from avis_client.models.metadata import Metadata
 from avis_client.models.metadata_request import MetadataRequest
 from avis_client.models.metadata_schema import MetadataSchema
 from avis_client.models.metadata_schema_request import MetadataSchemaRequest
+from avis_client.models.paginated_configuration_statistics_list import PaginatedConfigurationStatisticsList
 from avis_client.models.paginated_configuration_type_list import PaginatedConfigurationTypeList
 from avis_client.models.paginated_image_attribute_category_list import PaginatedImageAttributeCategoryList
 from avis_client.models.paginated_image_attribute_list import PaginatedImageAttributeList
 from avis_client.models.paginated_image_list import PaginatedImageList
 from avis_client.models.paginated_inspection_images_statistics_list import PaginatedInspectionImagesStatisticsList
 from avis_client.models.paginated_inspection_list import PaginatedInspectionList
 from avis_client.models.paginated_inspection_statistics_list import PaginatedInspectionStatisticsList
-from avis_client.models.paginated_inspection_status_list import PaginatedInspectionStatusList
 from avis_client.models.paginated_inspection_validation_status_list import PaginatedInspectionValidationStatusList
 from avis_client.models.paginated_ml_model_list import PaginatedMLModelList
 from avis_client.models.paginated_ml_model_type_list import PaginatedMLModelTypeList
 from avis_client.models.paginated_membership_list import PaginatedMembershipList
 from avis_client.models.paginated_metadata_list import PaginatedMetadataList
 from avis_client.models.paginated_metadata_schema_list import PaginatedMetadataSchemaList
 from avis_client.models.paginated_product_category_list import PaginatedProductCategoryList
```

### Comparing `avis_client-0.7.0/avis_client/models/azure_ml_inference_request.py` & `avis_client-0.8.0/avis_client/models/azure_ml_inference_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/blank_enum.py` & `avis_client-0.8.0/avis_client/models/blank_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/configuration_type.py` & `avis_client-0.8.0/avis_client/models/configuration_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class ConfigurationType(BaseModel):
     """
@@ -35,15 +35,16 @@
     metadata_schema: Optional[StrictInt] = None
     quality_criteria: Optional[StrictInt] = None
     product_category: Optional[StrictInt] = None
     image_attribute_categories: Optional[List[StrictInt]] = None
     created_at: Optional[datetime]
     updated_at: Optional[datetime]
     description: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["id", "team", "name", "metadata_schema", "quality_criteria", "product_category", "image_attribute_categories", "created_at", "updated_at", "description"]
+    is_default: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["id", "team", "name", "metadata_schema", "quality_criteria", "product_category", "image_attribute_categories", "created_at", "updated_at", "description", "is_default"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -126,12 +127,13 @@
             "name": obj.get("name"),
             "metadata_schema": obj.get("metadata_schema"),
             "quality_criteria": obj.get("quality_criteria"),
             "product_category": obj.get("product_category"),
             "image_attribute_categories": obj.get("image_attribute_categories"),
             "created_at": obj.get("created_at"),
             "updated_at": obj.get("updated_at"),
-            "description": obj.get("description")
+            "description": obj.get("description"),
+            "is_default": obj.get("is_default")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/configuration_type_request.py` & `avis_client-0.8.0/avis_client/models/configuration_type_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
 from pydantic import Field
 from typing_extensions import Annotated
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
@@ -34,15 +34,16 @@
     team: StrictInt
     name: Annotated[str, Field(min_length=1, strict=True)]
     metadata_schema: Optional[StrictInt] = None
     quality_criteria: Optional[StrictInt] = None
     product_category: Optional[StrictInt] = None
     image_attribute_categories: Optional[List[StrictInt]] = None
     description: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["team", "name", "metadata_schema", "quality_criteria", "product_category", "image_attribute_categories", "description"]
+    is_default: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["team", "name", "metadata_schema", "quality_criteria", "product_category", "image_attribute_categories", "description", "is_default"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -106,12 +107,13 @@
         _obj = cls.model_validate({
             "team": obj.get("team"),
             "name": obj.get("name"),
             "metadata_schema": obj.get("metadata_schema"),
             "quality_criteria": obj.get("quality_criteria"),
             "product_category": obj.get("product_category"),
             "image_attribute_categories": obj.get("image_attribute_categories"),
-            "description": obj.get("description")
+            "description": obj.get("description"),
+            "is_default": obj.get("is_default")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/custom_user.py` & `avis_client-0.8.0/avis_client/models/custom_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/custom_user_request.py` & `avis_client-0.8.0/avis_client/models/custom_user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/email_address.py` & `avis_client-0.8.0/avis_client/models/email_address.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/format_enum.py` & `avis_client-0.8.0/avis_client/models/format_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/image.py` & `avis_client-0.8.0/avis_client/models/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/image_attribute.py` & `avis_client-0.8.0/avis_client/models/image_attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/image_attribute_category.py` & `avis_client-0.8.0/avis_client/models/image_attribute_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/image_attribute_category_request.py` & `avis_client-0.8.0/avis_client/models/image_attribute_category_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/image_attribute_request.py` & `avis_client-0.8.0/avis_client/models/image_attribute_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/image_request.py` & `avis_client-0.8.0/avis_client/models/image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection.py` & `avis_client-0.8.0/avis_client/models/inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection_images_statistics.py` & `avis_client-0.8.0/avis_client/models/inspection_images_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection_images_statistics_request.py` & `avis_client-0.8.0/avis_client/models/inspection_images_statistics_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection_request.py` & `avis_client-0.8.0/avis_client/models/inspection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection_statistics.py` & `avis_client-0.8.0/avis_client/models/inspection_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection_statistics_request.py` & `avis_client-0.8.0/avis_client/models/inspection_statistics_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection_status.py` & `avis_client-0.8.0/avis_client/models/inspection_validation_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List
 from pydantic import BaseModel, StrictInt
-from avis_client.models.inspection_status_enum import InspectionStatusEnum
+from avis_client.models.validation_status_enum import ValidationStatusEnum
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class InspectionStatus(BaseModel):
+class InspectionValidationStatus(BaseModel):
     """
-    InspectionStatus
+    InspectionValidationStatus
     """ # noqa: E501
     id: StrictInt
-    inspection_status: InspectionStatusEnum
-    __properties: ClassVar[List[str]] = ["id", "inspection_status"]
+    validation_status: ValidationStatusEnum
+    __properties: ClassVar[List[str]] = ["id", "validation_status"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of InspectionStatus from a JSON string"""
+        """Create an instance of InspectionValidationStatus from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +71,21 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of InspectionStatus from a dict"""
+        """Create an instance of InspectionValidationStatus from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "inspection_status": obj.get("inspection_status")
+            "validation_status": obj.get("validation_status")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection_status_enum.py` & `avis_client-0.8.0/avis_client/models/validation_status_enum.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -22,25 +22,25 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class InspectionStatusEnum(str, Enum):
+class ValidationStatusEnum(str, Enum):
     """
-    * `NONE` - None * `OK` - Ok * `DEFECT` - Defect
+    * `NONE` - None * `REQUESTED` - Validation Requested * `VALIDATED` - Validated
     """
 
     """
     allowed enum values
     """
     NONE = 'NONE'
-    OK = 'OK'
-    DEFECT = 'DEFECT'
+    REQUESTED = 'REQUESTED'
+    VALIDATED = 'VALIDATED'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of InspectionStatusEnum from a JSON string"""
+        """Create an instance of ValidationStatusEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `avis_client-0.7.0/avis_client/models/inspection_validation_status.py` & `avis_client-0.8.0/avis_client/models/metadata_schema_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, ClassVar, Dict, List
+from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt
-from avis_client.models.validation_status_enum import ValidationStatusEnum
+from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class InspectionValidationStatus(BaseModel):
+class MetadataSchemaRequest(BaseModel):
     """
-    InspectionValidationStatus
+    MetadataSchemaRequest
     """ # noqa: E501
-    id: StrictInt
-    validation_status: ValidationStatusEnum
-    __properties: ClassVar[List[str]] = ["id", "validation_status"]
+    team: StrictInt
+    var_json: Optional[Any] = Field(alias="json")
+    __properties: ClassVar[List[str]] = ["team", "json"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of InspectionValidationStatus from a JSON string"""
+        """Create an instance of MetadataSchemaRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,25 +67,30 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # set to None if var_json (nullable) is None
+        # and model_fields_set contains the field
+        if self.var_json is None and "var_json" in self.model_fields_set:
+            _dict['json'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of InspectionValidationStatus from a dict"""
+        """Create an instance of MetadataSchemaRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "validation_status": obj.get("validation_status")
+            "team": obj.get("team"),
+            "json": obj.get("json")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/membership.py` & `avis_client-0.8.0/avis_client/models/membership.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/membership_request.py` & `avis_client-0.8.0/avis_client/models/membership_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/metadata.py` & `avis_client-0.8.0/avis_client/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/metadata_request.py` & `avis_client-0.8.0/avis_client/models/patched_metadata_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -22,21 +22,21 @@
 from pydantic import BaseModel, StrictInt
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class MetadataRequest(BaseModel):
+class PatchedMetadataRequest(BaseModel):
     """
-    MetadataRequest
+    PatchedMetadataRequest
     """ # noqa: E501
-    team: StrictInt
+    team: Optional[StrictInt] = None
     configurations: Optional[List[StrictInt]] = None
-    var_schema: StrictInt = Field(alias="schema")
+    var_schema: Optional[StrictInt] = Field(default=None, alias="schema")
     data: Optional[Any] = None
     __properties: ClassVar[List[str]] = ["team", "configurations", "schema", "data"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of MetadataRequest from a JSON string"""
+        """Create an instance of PatchedMetadataRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,15 +78,15 @@
         if self.data is None and "data" in self.model_fields_set:
             _dict['data'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of MetadataRequest from a dict"""
+        """Create an instance of PatchedMetadataRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `avis_client-0.7.0/avis_client/models/metadata_schema.py` & `avis_client-0.8.0/avis_client/models/metadata_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/metadata_schema_request.py` & `avis_client-0.8.0/avis_client/models/patched_metadata_schema_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -22,20 +22,20 @@
 from pydantic import BaseModel, StrictInt
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class MetadataSchemaRequest(BaseModel):
+class PatchedMetadataSchemaRequest(BaseModel):
     """
-    MetadataSchemaRequest
+    PatchedMetadataSchemaRequest
     """ # noqa: E501
-    team: StrictInt
-    var_json: Optional[Any] = Field(alias="json")
+    team: Optional[StrictInt] = None
+    var_json: Optional[Any] = Field(default=None, alias="json")
     __properties: ClassVar[List[str]] = ["team", "json"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -48,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of MetadataSchemaRequest from a JSON string"""
+        """Create an instance of PatchedMetadataSchemaRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -76,15 +76,15 @@
         if self.var_json is None and "var_json" in self.model_fields_set:
             _dict['json'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of MetadataSchemaRequest from a dict"""
+        """Create an instance of PatchedMetadataSchemaRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `avis_client-0.7.0/avis_client/models/ml_model.py` & `avis_client-0.8.0/avis_client/models/ml_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/ml_model_request.py` & `avis_client-0.8.0/avis_client/models/ml_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/ml_model_type.py` & `avis_client-0.8.0/avis_client/models/ml_model_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/ml_model_type_request.py` & `avis_client-0.8.0/avis_client/models/ml_model_type_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_configuration_type_list.py` & `avis_client-0.8.0/avis_client/models/paginated_configuration_type_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedConfigurationTypeList(BaseModel):
     """
     PaginatedConfigurationTypeList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[ConfigurationType]] = None
+    results: List[ConfigurationType]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_image_attribute_category_list.py` & `avis_client-0.8.0/avis_client/models/paginated_image_attribute_category_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedImageAttributeCategoryList(BaseModel):
     """
     PaginatedImageAttributeCategoryList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[ImageAttributeCategory]] = None
+    results: List[ImageAttributeCategory]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_image_attribute_list.py` & `avis_client-0.8.0/avis_client/models/paginated_image_attribute_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedImageAttributeList(BaseModel):
     """
     PaginatedImageAttributeList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[ImageAttribute]] = None
+    results: List[ImageAttribute]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_image_list.py` & `avis_client-0.8.0/avis_client/models/paginated_team_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
-from avis_client.models.image import Image
+from avis_client.models.team import Team
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PaginatedImageList(BaseModel):
+class PaginatedTeamList(BaseModel):
     """
-    PaginatedImageList
+    PaginatedTeamList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[Image]] = None
+    results: List[Team]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaginatedImageList from a JSON string"""
+        """Create an instance of PaginatedTeamList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -90,23 +90,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaginatedImageList from a dict"""
+        """Create an instance of PaginatedTeamList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [Image.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
+            "results": [Team.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_inspection_images_statistics_list.py` & `avis_client-0.8.0/avis_client/models/paginated_inspection_images_statistics_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedInspectionImagesStatisticsList(BaseModel):
     """
     PaginatedInspectionImagesStatisticsList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[InspectionImagesStatistics]] = None
+    results: List[InspectionImagesStatistics]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_inspection_list.py` & `avis_client-0.8.0/avis_client/models/paginated_inspection_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedInspectionList(BaseModel):
     """
     PaginatedInspectionList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[Inspection]] = None
+    results: List[Inspection]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_inspection_statistics_list.py` & `avis_client-0.8.0/avis_client/models/paginated_inspection_statistics_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedInspectionStatisticsList(BaseModel):
     """
     PaginatedInspectionStatisticsList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[InspectionStatistics]] = None
+    results: List[InspectionStatistics]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_inspection_status_list.py` & `avis_client-0.8.0/avis_client/models/paginated_inspection_validation_status_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
-from avis_client.models.inspection_status import InspectionStatus
+from avis_client.models.inspection_validation_status import InspectionValidationStatus
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PaginatedInspectionStatusList(BaseModel):
+class PaginatedInspectionValidationStatusList(BaseModel):
     """
-    PaginatedInspectionStatusList
+    PaginatedInspectionValidationStatusList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[InspectionStatus]] = None
+    results: List[InspectionValidationStatus]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaginatedInspectionStatusList from a JSON string"""
+        """Create an instance of PaginatedInspectionValidationStatusList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -90,23 +90,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaginatedInspectionStatusList from a dict"""
+        """Create an instance of PaginatedInspectionValidationStatusList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [InspectionStatus.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
+            "results": [InspectionValidationStatus.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_inspection_validation_status_list.py` & `avis_client-0.8.0/avis_client/models/paginated_configuration_statistics_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
-from avis_client.models.inspection_validation_status import InspectionValidationStatus
+from avis_client.models.configuration_statistics import ConfigurationStatistics
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PaginatedInspectionValidationStatusList(BaseModel):
+class PaginatedConfigurationStatisticsList(BaseModel):
     """
-    PaginatedInspectionValidationStatusList
+    PaginatedConfigurationStatisticsList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[InspectionValidationStatus]] = None
+    results: List[ConfigurationStatistics]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaginatedInspectionValidationStatusList from a JSON string"""
+        """Create an instance of PaginatedConfigurationStatisticsList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -90,23 +90,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaginatedInspectionValidationStatusList from a dict"""
+        """Create an instance of PaginatedConfigurationStatisticsList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [InspectionValidationStatus.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
+            "results": [ConfigurationStatistics.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_membership_list.py` & `avis_client-0.8.0/avis_client/models/paginated_membership_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedMembershipList(BaseModel):
     """
     PaginatedMembershipList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[Membership]] = None
+    results: List[Membership]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_metadata_list.py` & `avis_client-0.8.0/avis_client/models/paginated_metadata_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedMetadataList(BaseModel):
     """
     PaginatedMetadataList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[Metadata]] = None
+    results: List[Metadata]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_metadata_schema_list.py` & `avis_client-0.8.0/avis_client/models/paginated_metadata_schema_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedMetadataSchemaList(BaseModel):
     """
     PaginatedMetadataSchemaList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[MetadataSchema]] = None
+    results: List[MetadataSchema]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_ml_model_list.py` & `avis_client-0.8.0/avis_client/models/paginated_ml_model_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedMLModelList(BaseModel):
     """
     PaginatedMLModelList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[MLModel]] = None
+    results: List[MLModel]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_ml_model_type_list.py` & `avis_client-0.8.0/avis_client/models/paginated_ml_model_type_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedMLModelTypeList(BaseModel):
     """
     PaginatedMLModelTypeList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[MLModelType]] = None
+    results: List[MLModelType]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_product_category_list.py` & `avis_client-0.8.0/avis_client/models/paginated_product_category_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -26,18 +26,18 @@
 except ImportError:
     from typing_extensions import Self
 
 class PaginatedProductCategoryList(BaseModel):
     """
     PaginatedProductCategoryList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[ProductCategory]] = None
+    results: List[ProductCategory]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_product_list.py` & `avis_client-0.8.0/avis_client/models/paginated_result_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
-from avis_client.models.product import Product
+from avis_client.models.result import Result
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PaginatedProductList(BaseModel):
+class PaginatedResultList(BaseModel):
     """
-    PaginatedProductList
+    PaginatedResultList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[Product]] = None
+    results: List[Result]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaginatedProductList from a JSON string"""
+        """Create an instance of PaginatedResultList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -90,23 +90,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaginatedProductList from a dict"""
+        """Create an instance of PaginatedResultList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [Product.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
+            "results": [Result.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_quality_criteria_list.py` & `avis_client-0.8.0/avis_client/models/paginated_quality_criteria_result_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
-from avis_client.models.quality_criteria import QualityCriteria
+from avis_client.models.quality_criteria_result import QualityCriteriaResult
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PaginatedQualityCriteriaList(BaseModel):
+class PaginatedQualityCriteriaResultList(BaseModel):
     """
-    PaginatedQualityCriteriaList
+    PaginatedQualityCriteriaResultList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[QualityCriteria]] = None
+    results: List[QualityCriteriaResult]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaginatedQualityCriteriaList from a JSON string"""
+        """Create an instance of PaginatedQualityCriteriaResultList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -90,23 +90,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaginatedQualityCriteriaList from a dict"""
+        """Create an instance of PaginatedQualityCriteriaResultList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [QualityCriteria.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
+            "results": [QualityCriteriaResult.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_quality_criteria_result_list.py` & `avis_client-0.8.0/avis_client/models/paginated_quality_criteria_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
-from avis_client.models.quality_criteria_result import QualityCriteriaResult
+from avis_client.models.quality_criteria import QualityCriteria
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PaginatedQualityCriteriaResultList(BaseModel):
+class PaginatedQualityCriteriaList(BaseModel):
     """
-    PaginatedQualityCriteriaResultList
+    PaginatedQualityCriteriaList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[QualityCriteriaResult]] = None
+    results: List[QualityCriteria]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaginatedQualityCriteriaResultList from a JSON string"""
+        """Create an instance of PaginatedQualityCriteriaList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -90,23 +90,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaginatedQualityCriteriaResultList from a dict"""
+        """Create an instance of PaginatedQualityCriteriaList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [QualityCriteriaResult.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
+            "results": [QualityCriteria.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_result_list.py` & `avis_client-0.8.0/avis_client/models/paginated_image_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel, StrictInt, StrictStr
-from avis_client.models.result import Result
+from avis_client.models.image import Image
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PaginatedResultList(BaseModel):
+class PaginatedImageList(BaseModel):
     """
-    PaginatedResultList
+    PaginatedImageList
     """ # noqa: E501
-    count: Optional[StrictInt] = None
+    count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: Optional[List[Result]] = None
+    results: List[Image]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaginatedResultList from a JSON string"""
+        """Create an instance of PaginatedImageList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -90,23 +90,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaginatedResultList from a dict"""
+        """Create an instance of PaginatedImageList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [Result.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
+            "results": [Image.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/paginated_team_list.py` & `avis_client-0.8.0/avis_client/models/team_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
-from avis_client.models.team import Team
+from pydantic import BaseModel, StrictInt, field_validator
+from pydantic import Field
+from typing_extensions import Annotated
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PaginatedTeamList(BaseModel):
+class TeamRequest(BaseModel):
     """
-    PaginatedTeamList
+    TeamRequest
     """ # noqa: E501
-    count: Optional[StrictInt] = None
-    next: Optional[StrictStr] = None
-    previous: Optional[StrictStr] = None
-    results: Optional[List[Team]] = None
-    __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
+    name: Annotated[str, Field(min_length=1, strict=True, max_length=100)]
+    slug: Annotated[str, Field(min_length=1, strict=True, max_length=50)]
+    customer: Optional[StrictInt] = None
+    subscription: Optional[StrictInt] = None
+    __properties: ClassVar[List[str]] = ["name", "slug", "customer", "subscription"]
+
+    @field_validator('slug')
+    def slug_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if not re.match(r"^[-a-zA-Z0-9_]+$", value):
+            raise ValueError(r"must validate the regular expression /^[-a-zA-Z0-9_]+$/")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -50,15 +58,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PaginatedTeamList from a JSON string"""
+        """Create an instance of TeamRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,44 +77,37 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in results (list)
-        _items = []
-        if self.results:
-            for _item in self.results:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['results'] = _items
-        # set to None if next (nullable) is None
+        # set to None if customer (nullable) is None
         # and model_fields_set contains the field
-        if self.next is None and "next" in self.model_fields_set:
-            _dict['next'] = None
+        if self.customer is None and "customer" in self.model_fields_set:
+            _dict['customer'] = None
 
-        # set to None if previous (nullable) is None
+        # set to None if subscription (nullable) is None
         # and model_fields_set contains the field
-        if self.previous is None and "previous" in self.model_fields_set:
-            _dict['previous'] = None
+        if self.subscription is None and "subscription" in self.model_fields_set:
+            _dict['subscription'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PaginatedTeamList from a dict"""
+        """Create an instance of TeamRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "count": obj.get("count"),
-            "next": obj.get("next"),
-            "previous": obj.get("previous"),
-            "results": [Team.from_dict(_item) for _item in obj.get("results")] if obj.get("results") is not None else None
+            "name": obj.get("name"),
+            "slug": obj.get("slug"),
+            "customer": obj.get("customer"),
+            "subscription": obj.get("subscription")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_configuration_type_request.py` & `avis_client-0.8.0/avis_client/models/patched_configuration_type_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
 from pydantic import Field
 from typing_extensions import Annotated
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
@@ -34,15 +34,16 @@
     team: Optional[StrictInt] = None
     name: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
     metadata_schema: Optional[StrictInt] = None
     quality_criteria: Optional[StrictInt] = None
     product_category: Optional[StrictInt] = None
     image_attribute_categories: Optional[List[StrictInt]] = None
     description: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["team", "name", "metadata_schema", "quality_criteria", "product_category", "image_attribute_categories", "description"]
+    is_default: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["team", "name", "metadata_schema", "quality_criteria", "product_category", "image_attribute_categories", "description", "is_default"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -106,12 +107,13 @@
         _obj = cls.model_validate({
             "team": obj.get("team"),
             "name": obj.get("name"),
             "metadata_schema": obj.get("metadata_schema"),
             "quality_criteria": obj.get("quality_criteria"),
             "product_category": obj.get("product_category"),
             "image_attribute_categories": obj.get("image_attribute_categories"),
-            "description": obj.get("description")
+            "description": obj.get("description"),
+            "is_default": obj.get("is_default")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_image_attribute_category_request.py` & `avis_client-0.8.0/avis_client/models/patched_image_attribute_category_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_image_attribute_request.py` & `avis_client-0.8.0/avis_client/models/patched_image_attribute_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_image_request.py` & `avis_client-0.8.0/avis_client/models/patched_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_inspection_request.py` & `avis_client-0.8.0/avis_client/models/patched_inspection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_metadata_request.py` & `avis_client-0.8.0/avis_client/models/metadata_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -22,21 +22,21 @@
 from pydantic import BaseModel, StrictInt
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PatchedMetadataRequest(BaseModel):
+class MetadataRequest(BaseModel):
     """
-    PatchedMetadataRequest
+    MetadataRequest
     """ # noqa: E501
-    team: Optional[StrictInt] = None
+    team: StrictInt
     configurations: Optional[List[StrictInt]] = None
-    var_schema: Optional[StrictInt] = Field(default=None, alias="schema")
+    var_schema: StrictInt = Field(alias="schema")
     data: Optional[Any] = None
     __properties: ClassVar[List[str]] = ["team", "configurations", "schema", "data"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
@@ -50,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PatchedMetadataRequest from a JSON string"""
+        """Create an instance of MetadataRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,15 +78,15 @@
         if self.data is None and "data" in self.model_fields_set:
             _dict['data'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PatchedMetadataRequest from a dict"""
+        """Create an instance of MetadataRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_metadata_schema_request.py` & `avis_client-0.8.0/avis_client/models/patched_ml_model_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt
+from pydantic import BaseModel, StrictInt, StrictStr
 from pydantic import Field
+from typing_extensions import Annotated
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PatchedMetadataSchemaRequest(BaseModel):
+class PatchedMLModelRequest(BaseModel):
     """
-    PatchedMetadataSchemaRequest
+    PatchedMLModelRequest
     """ # noqa: E501
-    team: Optional[StrictInt] = None
-    var_json: Optional[Any] = Field(default=None, alias="json")
-    __properties: ClassVar[List[str]] = ["team", "json"]
+    headers: Optional[Any] = None
+    model: Optional[StrictInt] = None
+    version: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None
+    url: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["headers", "model", "version", "url"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +51,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PatchedMetadataSchemaRequest from a JSON string"""
+        """Create an instance of PatchedMLModelRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,30 +70,42 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # set to None if var_json (nullable) is None
+        # set to None if headers (nullable) is None
         # and model_fields_set contains the field
-        if self.var_json is None and "var_json" in self.model_fields_set:
-            _dict['json'] = None
+        if self.headers is None and "headers" in self.model_fields_set:
+            _dict['headers'] = None
+
+        # set to None if version (nullable) is None
+        # and model_fields_set contains the field
+        if self.version is None and "version" in self.model_fields_set:
+            _dict['version'] = None
+
+        # set to None if url (nullable) is None
+        # and model_fields_set contains the field
+        if self.url is None and "url" in self.model_fields_set:
+            _dict['url'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PatchedMetadataSchemaRequest from a dict"""
+        """Create an instance of PatchedMLModelRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "team": obj.get("team"),
-            "json": obj.get("json")
+            "headers": obj.get("headers"),
+            "model": obj.get("model"),
+            "version": obj.get("version"),
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_ml_model_request.py` & `avis_client-0.8.0/avis_client/models/patched_product_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -23,23 +23,25 @@
 from pydantic import Field
 from typing_extensions import Annotated
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PatchedMLModelRequest(BaseModel):
+class PatchedProductRequest(BaseModel):
     """
-    PatchedMLModelRequest
+    PatchedProductRequest
     """ # noqa: E501
-    headers: Optional[Any] = None
-    model: Optional[StrictInt] = None
-    version: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None
-    url: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["headers", "model", "version", "url"]
+    team: Optional[StrictInt] = None
+    category: Optional[StrictInt] = None
+    inspections: Optional[List[StrictInt]] = None
+    identifier: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None
+    display_name: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None
+    description: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["team", "category", "inspections", "identifier", "display_name", "description"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -51,15 +53,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PatchedMLModelRequest from a JSON string"""
+        """Create an instance of PatchedProductRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,42 +72,39 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # set to None if headers (nullable) is None
+        # set to None if category (nullable) is None
         # and model_fields_set contains the field
-        if self.headers is None and "headers" in self.model_fields_set:
-            _dict['headers'] = None
+        if self.category is None and "category" in self.model_fields_set:
+            _dict['category'] = None
 
-        # set to None if version (nullable) is None
+        # set to None if display_name (nullable) is None
         # and model_fields_set contains the field
-        if self.version is None and "version" in self.model_fields_set:
-            _dict['version'] = None
-
-        # set to None if url (nullable) is None
-        # and model_fields_set contains the field
-        if self.url is None and "url" in self.model_fields_set:
-            _dict['url'] = None
+        if self.display_name is None and "display_name" in self.model_fields_set:
+            _dict['display_name'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PatchedMLModelRequest from a dict"""
+        """Create an instance of PatchedProductRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "headers": obj.get("headers"),
-            "model": obj.get("model"),
-            "version": obj.get("version"),
-            "url": obj.get("url")
+            "team": obj.get("team"),
+            "category": obj.get("category"),
+            "inspections": obj.get("inspections"),
+            "identifier": obj.get("identifier"),
+            "display_name": obj.get("display_name"),
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_ml_model_type_request.py` & `avis_client-0.8.0/avis_client/models/patched_ml_model_type_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_product_category_request.py` & `avis_client-0.8.0/avis_client/models/patched_product_category_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_product_request.py` & `avis_client-0.8.0/avis_client/models/product_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -23,22 +23,22 @@
 from pydantic import Field
 from typing_extensions import Annotated
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class PatchedProductRequest(BaseModel):
+class ProductRequest(BaseModel):
     """
-    PatchedProductRequest
+    ProductRequest
     """ # noqa: E501
-    team: Optional[StrictInt] = None
+    team: StrictInt
     category: Optional[StrictInt] = None
     inspections: Optional[List[StrictInt]] = None
-    identifier: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None
+    identifier: Annotated[str, Field(strict=True, max_length=255)]
     display_name: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None
     description: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["team", "category", "inspections", "identifier", "display_name", "description"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
@@ -53,15 +53,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of PatchedProductRequest from a JSON string"""
+        """Create an instance of ProductRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -86,15 +86,15 @@
         if self.display_name is None and "display_name" in self.model_fields_set:
             _dict['display_name'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of PatchedProductRequest from a dict"""
+        """Create an instance of ProductRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_quality_criteria_request.py` & `avis_client-0.8.0/avis_client/models/patched_quality_criteria_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_result_request.py` & `avis_client-0.8.0/avis_client/models/patched_result_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/patched_result_request_status.py` & `avis_client-0.8.0/avis_client/models/patched_result_request_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/product.py` & `avis_client-0.8.0/avis_client/models/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/product_category.py` & `avis_client-0.8.0/avis_client/models/product_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/product_category_request.py` & `avis_client-0.8.0/avis_client/models/product_category_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/product_request.py` & `avis_client-0.8.0/avis_client/models/configuration_statistics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, StrictStr
-from pydantic import Field
-from typing_extensions import Annotated
+from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, StrictInt
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class ProductRequest(BaseModel):
+class ConfigurationStatistics(BaseModel):
     """
-    ProductRequest
+    ConfigurationStatistics
     """ # noqa: E501
-    team: StrictInt
-    category: Optional[StrictInt] = None
-    inspections: Optional[List[StrictInt]] = None
-    identifier: Annotated[str, Field(strict=True, max_length=255)]
-    display_name: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None
-    description: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["team", "category", "inspections", "identifier", "display_name", "description"]
+    configuration: StrictInt
+    opened_inspections: StrictInt
+    inspections_marked_for_validation: StrictInt
+    __properties: ClassVar[List[str]] = ["configuration", "opened_inspections", "inspections_marked_for_validation"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -53,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ProductRequest from a JSON string"""
+        """Create an instance of ConfigurationStatistics from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,39 +67,26 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # set to None if category (nullable) is None
-        # and model_fields_set contains the field
-        if self.category is None and "category" in self.model_fields_set:
-            _dict['category'] = None
-
-        # set to None if display_name (nullable) is None
-        # and model_fields_set contains the field
-        if self.display_name is None and "display_name" in self.model_fields_set:
-            _dict['display_name'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of ProductRequest from a dict"""
+        """Create an instance of ConfigurationStatistics from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "team": obj.get("team"),
-            "category": obj.get("category"),
-            "inspections": obj.get("inspections"),
-            "identifier": obj.get("identifier"),
-            "display_name": obj.get("display_name"),
-            "description": obj.get("description")
+            "configuration": obj.get("configuration"),
+            "opened_inspections": obj.get("opened_inspections"),
+            "inspections_marked_for_validation": obj.get("inspections_marked_for_validation")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/quality_criteria.py` & `avis_client-0.8.0/avis_client/models/quality_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/quality_criteria_request.py` & `avis_client-0.8.0/avis_client/models/quality_criteria_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/quality_criteria_result.py` & `avis_client-0.8.0/avis_client/models/quality_criteria_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/quality_enum.py` & `avis_client-0.8.0/avis_client/models/quality_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/result.py` & `avis_client-0.8.0/avis_client/models/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/result_request.py` & `avis_client-0.8.0/avis_client/models/result_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/status_enum.py` & `avis_client-0.8.0/avis_client/models/status_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/team.py` & `avis_client-0.8.0/avis_client/models/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/team_request.py` & `avis_client-0.8.0/avis_client/models/user_api_key_create_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,42 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictInt, field_validator
+from pydantic import BaseModel
 from pydantic import Field
 from typing_extensions import Annotated
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class TeamRequest(BaseModel):
+class UserAPIKeyCreateRequest(BaseModel):
     """
-    TeamRequest
+    UserAPIKeyCreateRequest
     """ # noqa: E501
-    name: Annotated[str, Field(min_length=1, strict=True, max_length=100)]
-    slug: Annotated[str, Field(min_length=1, strict=True, max_length=50)]
-    customer: Optional[StrictInt] = None
-    subscription: Optional[StrictInt] = None
-    __properties: ClassVar[List[str]] = ["name", "slug", "customer", "subscription"]
-
-    @field_validator('slug')
-    def slug_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if not re.match(r"^[-a-zA-Z0-9_]+$", value):
-            raise ValueError(r"must validate the regular expression /^[-a-zA-Z0-9_]+$/")
-        return value
+    name: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=50)]] = Field(default=None, description="A free-form name for the API key. Need not be unique. 50 characters max.")
+    __properties: ClassVar[List[str]] = ["name"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -58,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TeamRequest from a JSON string"""
+        """Create an instance of UserAPIKeyCreateRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,37 +67,24 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
-        # set to None if customer (nullable) is None
-        # and model_fields_set contains the field
-        if self.customer is None and "customer" in self.model_fields_set:
-            _dict['customer'] = None
-
-        # set to None if subscription (nullable) is None
-        # and model_fields_set contains the field
-        if self.subscription is None and "subscription" in self.model_fields_set:
-            _dict['subscription'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of TeamRequest from a dict"""
+        """Create an instance of UserAPIKeyCreateRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "slug": obj.get("slug"),
-            "customer": obj.get("customer"),
-            "subscription": obj.get("subscription")
+            "name": obj.get("name")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/models/user_api_key_create.py` & `avis_client-0.8.0/avis_client/models/user_api_key_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.7.0/avis_client/models/user_api_key_create_request.py` & `avis_client-0.8.0/avis_client/models/configuration_statistics_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel
-from pydantic import Field
-from typing_extensions import Annotated
+from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, StrictInt
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class UserAPIKeyCreateRequest(BaseModel):
+class ConfigurationStatisticsRequest(BaseModel):
     """
-    UserAPIKeyCreateRequest
+    ConfigurationStatisticsRequest
     """ # noqa: E501
-    name: Optional[Annotated[str, Field(min_length=1, strict=True, max_length=50)]] = Field(default=None, description="A free-form name for the API key. Need not be unique. 50 characters max.")
-    __properties: ClassVar[List[str]] = ["name"]
+    configuration: StrictInt
+    opened_inspections: StrictInt
+    inspections_marked_for_validation: StrictInt
+    __properties: ClassVar[List[str]] = ["configuration", "opened_inspections", "inspections_marked_for_validation"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of UserAPIKeyCreateRequest from a JSON string"""
+        """Create an instance of ConfigurationStatisticsRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,20 +71,22 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of UserAPIKeyCreateRequest from a dict"""
+        """Create an instance of ConfigurationStatisticsRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name")
+            "configuration": obj.get("configuration"),
+            "opened_inspections": obj.get("opened_inspections"),
+            "inspections_marked_for_validation": obj.get("inspections_marked_for_validation")
         })
         return _obj
```

### Comparing `avis_client-0.7.0/avis_client/rest.py` & `avis_client-0.8.0/avis_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.7.0
+    The version of the OpenAPI document: 0.8.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.7.0/pyproject.toml` & `avis_client-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "avis_client"
-version = "0.7.0"
+version = "0.8.0"
 description = "AVIS Python client"
 authors = [ "VUEngineering <tech@vu.engineering>",]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/vuengineering/public/"
 keywords = [ "OpenAPI", "avis", "api client",]
 include = [ "avis_client/py.typed",]
```

### Comparing `avis_client-0.7.0/PKG-INFO` & `avis_client-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avis_client
-Version: 0.7.0
+Version: 0.8.0
 Summary: AVIS Python client
 Home-page: https://docs.vu.engineering/api/clients/python/avis_client/
 License: Apache-2.0
 Keywords: OpenAPI,avis,api client
 Author: VUEngineering
 Author-email: tech@vu.engineering
 Maintainer: Adriano Pagano
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # avis-client
 VUE Autonomous Visual Inspection System (AVIS)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.7.0
-- Package version: 0.7.0
+- API version: 0.8.0
+- Package version: 0.8.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -132,15 +132,14 @@
 *ConfigurationApi* | [**configuration_destroy**](docs/ConfigurationApi.md#configuration_destroy) | **DELETE** /api/configuration/{id}/ | 
 *ConfigurationApi* | [**configuration_list**](docs/ConfigurationApi.md#configuration_list) | **GET** /api/configuration/ | 
 *ConfigurationApi* | [**configuration_partial_update**](docs/ConfigurationApi.md#configuration_partial_update) | **PATCH** /api/configuration/{id}/ | 
 *ConfigurationApi* | [**configuration_retrieve**](docs/ConfigurationApi.md#configuration_retrieve) | **GET** /api/configuration/{id}/ | 
 *ConfigurationApi* | [**configuration_update**](docs/ConfigurationApi.md#configuration_update) | **PUT** /api/configuration/{id}/ | 
 *ImageApi* | [**image_create**](docs/ImageApi.md#image_create) | **POST** /api/image/ | 
 *ImageApi* | [**image_destroy**](docs/ImageApi.md#image_destroy) | **DELETE** /api/image/{id}/ | 
-*ImageApi* | [**image_inspection_status_list**](docs/ImageApi.md#image_inspection_status_list) | **GET** /api/image/inspection_status/ | 
 *ImageApi* | [**image_list**](docs/ImageApi.md#image_list) | **GET** /api/image/ | 
 *ImageApi* | [**image_partial_update**](docs/ImageApi.md#image_partial_update) | **PATCH** /api/image/{id}/ | 
 *ImageApi* | [**image_quality_list**](docs/ImageApi.md#image_quality_list) | **GET** /api/image/quality/ | 
 *ImageApi* | [**image_retrieve**](docs/ImageApi.md#image_retrieve) | **GET** /api/image/{id}/ | 
 *ImageApi* | [**image_update**](docs/ImageApi.md#image_update) | **PUT** /api/image/{id}/ | 
 *ImageAttributeApi* | [**image_attribute_create**](docs/ImageAttributeApi.md#image_attribute_create) | **POST** /api/image-attribute/ | 
 *ImageAttributeApi* | [**image_attribute_destroy**](docs/ImageAttributeApi.md#image_attribute_destroy) | **DELETE** /api/image-attribute/{id}/ | 
@@ -156,15 +155,14 @@
 *ImageAttributeCategoryApi* | [**image_attribute_category_update**](docs/ImageAttributeCategoryApi.md#image_attribute_category_update) | **PUT** /api/image-attribute-category/{id}/ | 
 *InspectionApi* | [**inspection_create**](docs/InspectionApi.md#inspection_create) | **POST** /api/inspection/ | 
 *InspectionApi* | [**inspection_destroy**](docs/InspectionApi.md#inspection_destroy) | **DELETE** /api/inspection/{id}/ | 
 *InspectionApi* | [**inspection_list**](docs/InspectionApi.md#inspection_list) | **GET** /api/inspection/ | 
 *InspectionApi* | [**inspection_partial_update**](docs/InspectionApi.md#inspection_partial_update) | **PATCH** /api/inspection/{id}/ | 
 *InspectionApi* | [**inspection_retrieve**](docs/InspectionApi.md#inspection_retrieve) | **GET** /api/inspection/{id}/ | 
 *InspectionApi* | [**inspection_send_validation_email_retrieve**](docs/InspectionApi.md#inspection_send_validation_email_retrieve) | **GET** /api/inspection/{id}/send_validation_email/ | 
-*InspectionApi* | [**inspection_status_list**](docs/InspectionApi.md#inspection_status_list) | **GET** /api/inspection/status/ | 
 *InspectionApi* | [**inspection_update**](docs/InspectionApi.md#inspection_update) | **PUT** /api/inspection/{id}/ | 
 *InspectionApi* | [**inspection_validation_status_list**](docs/InspectionApi.md#inspection_validation_status_list) | **GET** /api/inspection/validation_status/ | 
 *MembershipApi* | [**membership_create**](docs/MembershipApi.md#membership_create) | **POST** /api/membership/ | 
 *MembershipApi* | [**membership_destroy**](docs/MembershipApi.md#membership_destroy) | **DELETE** /api/membership/{id}/ | 
 *MembershipApi* | [**membership_list**](docs/MembershipApi.md#membership_list) | **GET** /api/membership/ | 
 *MembershipApi* | [**membership_retrieve**](docs/MembershipApi.md#membership_retrieve) | **GET** /api/membership/{id}/ | 
 *MembershipApi* | [**membership_update**](docs/MembershipApi.md#membership_update) | **PUT** /api/membership/{id}/ | 
@@ -213,14 +211,19 @@
 *QualityCriteriaApi* | [**quality_criteria_update**](docs/QualityCriteriaApi.md#quality_criteria_update) | **PUT** /api/quality-criteria/{id}/ | 
 *ResultApi* | [**result_create**](docs/ResultApi.md#result_create) | **POST** /api/result/ | 
 *ResultApi* | [**result_destroy**](docs/ResultApi.md#result_destroy) | **DELETE** /api/result/{id}/ | 
 *ResultApi* | [**result_list**](docs/ResultApi.md#result_list) | **GET** /api/result/ | 
 *ResultApi* | [**result_partial_update**](docs/ResultApi.md#result_partial_update) | **PATCH** /api/result/{id}/ | 
 *ResultApi* | [**result_retrieve**](docs/ResultApi.md#result_retrieve) | **GET** /api/result/{id}/ | 
 *ResultApi* | [**result_update**](docs/ResultApi.md#result_update) | **PUT** /api/result/{id}/ | 
+*StatisticsApi* | [**statistics_configuration_create**](docs/StatisticsApi.md#statistics_configuration_create) | **POST** /api/statistics/configuration/ | 
+*StatisticsApi* | [**statistics_configuration_destroy**](docs/StatisticsApi.md#statistics_configuration_destroy) | **DELETE** /api/statistics/configuration/{id}/ | 
+*StatisticsApi* | [**statistics_configuration_list**](docs/StatisticsApi.md#statistics_configuration_list) | **GET** /api/statistics/configuration/ | 
+*StatisticsApi* | [**statistics_configuration_retrieve**](docs/StatisticsApi.md#statistics_configuration_retrieve) | **GET** /api/statistics/configuration/{id}/ | 
+*StatisticsApi* | [**statistics_configuration_update**](docs/StatisticsApi.md#statistics_configuration_update) | **PUT** /api/statistics/configuration/{id}/ | 
 *StatisticsApi* | [**statistics_inspection_create**](docs/StatisticsApi.md#statistics_inspection_create) | **POST** /api/statistics/inspection/ | 
 *StatisticsApi* | [**statistics_inspection_destroy**](docs/StatisticsApi.md#statistics_inspection_destroy) | **DELETE** /api/statistics/inspection/{id}/ | 
 *StatisticsApi* | [**statistics_inspection_list**](docs/StatisticsApi.md#statistics_inspection_list) | **GET** /api/statistics/inspection/ | 
 *StatisticsApi* | [**statistics_inspection_retrieve**](docs/StatisticsApi.md#statistics_inspection_retrieve) | **GET** /api/statistics/inspection/{id}/ | 
 *StatisticsApi* | [**statistics_inspection_update**](docs/StatisticsApi.md#statistics_inspection_update) | **PUT** /api/statistics/inspection/{id}/ | 
 *StatisticsApi* | [**statistics_team_create**](docs/StatisticsApi.md#statistics_team_create) | **POST** /api/statistics/team/ | 
 *StatisticsApi* | [**statistics_team_destroy**](docs/StatisticsApi.md#statistics_team_destroy) | **DELETE** /api/statistics/team/{id}/ | 
@@ -236,14 +239,16 @@
 *UserApi* | [**user_whoami_retrieve**](docs/UserApi.md#user_whoami_retrieve) | **GET** /api/user/whoami/ | 
 
 
 ## Documentation For Models
 
  - [AzureMLInferenceRequest](docs/AzureMLInferenceRequest.md)
  - [BlankEnum](docs/BlankEnum.md)
+ - [ConfigurationStatistics](docs/ConfigurationStatistics.md)
+ - [ConfigurationStatisticsRequest](docs/ConfigurationStatisticsRequest.md)
  - [ConfigurationType](docs/ConfigurationType.md)
  - [ConfigurationTypeRequest](docs/ConfigurationTypeRequest.md)
  - [CustomUser](docs/CustomUser.md)
  - [CustomUserRequest](docs/CustomUserRequest.md)
  - [EmailAddress](docs/EmailAddress.md)
  - [FormatEnum](docs/FormatEnum.md)
  - [Image](docs/Image.md)
@@ -254,35 +259,33 @@
  - [ImageRequest](docs/ImageRequest.md)
  - [Inspection](docs/Inspection.md)
  - [InspectionImagesStatistics](docs/InspectionImagesStatistics.md)
  - [InspectionImagesStatisticsRequest](docs/InspectionImagesStatisticsRequest.md)
  - [InspectionRequest](docs/InspectionRequest.md)
  - [InspectionStatistics](docs/InspectionStatistics.md)
  - [InspectionStatisticsRequest](docs/InspectionStatisticsRequest.md)
- - [InspectionStatus](docs/InspectionStatus.md)
- - [InspectionStatusEnum](docs/InspectionStatusEnum.md)
  - [InspectionValidationStatus](docs/InspectionValidationStatus.md)
  - [MLModel](docs/MLModel.md)
  - [MLModelRequest](docs/MLModelRequest.md)
  - [MLModelType](docs/MLModelType.md)
  - [MLModelTypeRequest](docs/MLModelTypeRequest.md)
  - [Membership](docs/Membership.md)
  - [MembershipRequest](docs/MembershipRequest.md)
  - [Metadata](docs/Metadata.md)
  - [MetadataRequest](docs/MetadataRequest.md)
  - [MetadataSchema](docs/MetadataSchema.md)
  - [MetadataSchemaRequest](docs/MetadataSchemaRequest.md)
+ - [PaginatedConfigurationStatisticsList](docs/PaginatedConfigurationStatisticsList.md)
  - [PaginatedConfigurationTypeList](docs/PaginatedConfigurationTypeList.md)
  - [PaginatedImageAttributeCategoryList](docs/PaginatedImageAttributeCategoryList.md)
  - [PaginatedImageAttributeList](docs/PaginatedImageAttributeList.md)
  - [PaginatedImageList](docs/PaginatedImageList.md)
  - [PaginatedInspectionImagesStatisticsList](docs/PaginatedInspectionImagesStatisticsList.md)
  - [PaginatedInspectionList](docs/PaginatedInspectionList.md)
  - [PaginatedInspectionStatisticsList](docs/PaginatedInspectionStatisticsList.md)
- - [PaginatedInspectionStatusList](docs/PaginatedInspectionStatusList.md)
  - [PaginatedInspectionValidationStatusList](docs/PaginatedInspectionValidationStatusList.md)
  - [PaginatedMLModelList](docs/PaginatedMLModelList.md)
  - [PaginatedMLModelTypeList](docs/PaginatedMLModelTypeList.md)
  - [PaginatedMembershipList](docs/PaginatedMembershipList.md)
  - [PaginatedMetadataList](docs/PaginatedMetadataList.md)
  - [PaginatedMetadataSchemaList](docs/PaginatedMetadataSchemaList.md)
  - [PaginatedProductCategoryList](docs/PaginatedProductCategoryList.md)
```

