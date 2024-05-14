# Comparing `tmp/ai21-2.2.4.tar.gz` & `tmp/ai21-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-2.2.4.tar", max compression
+gzip compressed data, was "ai21-2.2.5.tar", max compression
```

## Comparing `ai21-2.2.4.tar` & `ai21-2.2.5.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    11357 2024-05-09 10:37:12.541003 ai21-2.2.4/LICENSE
--rw-r--r--   0        0        0    11868 2024-05-09 10:37:12.541003 ai21-2.2.4/README.md
--rw-r--r--   0        0        0     1575 2024-05-09 10:37:12.541003 ai21-2.2.4/ai21/__init__.py
--rw-r--r--   0        0        0     1014 2024-05-09 10:37:12.541003 ai21-2.2.4/ai21/ai21_env_config.py
--rw-r--r--   0        0        0     2626 2024-05-09 10:37:12.541003 ai21-2.2.4/ai21/ai21_http_client.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/__init__.py
--rw-r--r--   0        0        0      844 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/ai21_bedrock_client.py
--rw-r--r--   0        0        0       92 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/bedrock_model_id.py
--rw-r--r--   0        0        0     2414 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/bedrock_session.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/resources/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/resources/bedrock_completion.py
--rw-r--r--   0        0        0      522 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/resources/bedrock_resource.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/__init__.py
--rw-r--r--   0        0        0      857 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/answer_base.py
--rw-r--r--   0        0        0     3710 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/chat_base.py
--rw-r--r--   0        0        0     4216 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/completion_base.py
--rw-r--r--   0        0        0     1634 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/custom_model_base.py
--rw-r--r--   0        0        0     1886 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/dataset_base.py
--rw-r--r--   0        0        0      888 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/embed_base.py
--rw-r--r--   0        0        0      577 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/gec_base.py
--rw-r--r--   0        0        0      771 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/improvements_base.py
--rw-r--r--   0        0        0     1478 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/paraphrase_base.py
--rw-r--r--   0        0        0      806 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/segmentation_base.py
--rw-r--r--   0        0        0     1217 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/summarize_base.py
--rw-r--r--   0        0        0     1143 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/summarize_by_segment_base.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/__init__.py
--rw-r--r--   0        0        0     1545 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/ai21_sagemaker_client.py
--rw-r--r--   0        0        0      154 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/constants.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/__init__.py
--rw-r--r--   0        0        0      498 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_answer.py
--rw-r--r--   0        0        0     3194 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_completion.py
--rw-r--r--   0        0        0      399 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_gec.py
--rw-r--r--   0        0        0      789 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
--rw-r--r--   0        0        0      484 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_resource.py
--rw-r--r--   0        0        0      810 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_summarize.py
--rw-r--r--   0        0        0     2522 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/sagemaker_session.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/__init__.py
--rw-r--r--   0        0        0     3496 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/ai21_client.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/__init__.py
--rw-r--r--   0        0        0      101 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/chat/__init__.py
--rw-r--r--   0        0        0     2435 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/chat/chat_completions.py
--rw-r--r--   0        0        0      574 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_answer.py
--rw-r--r--   0        0        0     2061 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_chat.py
--rw-r--r--   0        0        0     1996 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_completion.py
--rw-r--r--   0        0        0     1290 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_custom_model.py
--rw-r--r--   0        0        0     1507 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_dataset.py
--rw-r--r--   0        0        0      584 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_embed.py
--rw-r--r--   0        0        0      472 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_gec.py
--rw-r--r--   0        0        0      739 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_improvements.py
--rw-r--r--   0        0        0     3670 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_library.py
--rw-r--r--   0        0        0      873 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_paraphrase.py
--rw-r--r--   0        0        0     1096 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_resource.py
--rw-r--r--   0        0        0      612 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_segmentation.py
--rw-r--r--   0        0        0      891 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_summarize.py
--rw-r--r--   0        0        0      782 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_summarize_by_segment.py
--rw-r--r--   0        0        0       64 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/constants.py
--rw-r--r--   0        0        0     2615 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/errors.py
--rw-r--r--   0        0        0     4868 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/http_client.py
--rw-r--r--   0        0        0      484 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/logger.py
--rw-r--r--   0        0        0     2633 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/__init__.py
--rw-r--r--   0        0        0      262 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/ai21_base_model_mixin.py
--rw-r--r--   0        0        0      343 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat/__init__.py
--rw-r--r--   0        0        0      592 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat/chat_completion_response.py
--rw-r--r--   0        0        0      219 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat/chat_message.py
--rw-r--r--   0        0        0       97 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat/role_type.py
--rw-r--r--   0        0        0      233 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat_message.py
--rw-r--r--   0        0        0       89 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/document_type.py
--rw-r--r--   0        0        0       96 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/embed_type.py
--rw-r--r--   0        0        0      286 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/improvement_type.py
--rw-r--r--   0        0        0      410 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/logprobs.py
--rw-r--r--   0        0        0      168 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/paraphrase_style_type.py
--rw-r--r--   0        0        0      503 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/penalty.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/__init__.py
--rw-r--r--   0        0        0      273 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/answer_response.py
--rw-r--r--   0        0        0      518 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/chat_response.py
--rw-r--r--   0        0        0      786 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/completion_response.py
--rw-r--r--   0        0        0      713 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/custom_model_response.py
--rw-r--r--   0        0        0      376 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/dataset_response.py
--rw-r--r--   0        0        0      300 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/embed_response.py
--rw-r--r--   0        0        0      550 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/file_response.py
--rw-r--r--   0        0        0      635 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/gec_response.py
--rw-r--r--   0        0        0      401 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/improvement_response.py
--rw-r--r--   0        0        0      469 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/library_answer_response.py
--rw-r--r--   0        0        0      450 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/library_search_response.py
--rw-r--r--   0        0        0      294 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/paraphrase_response.py
--rw-r--r--   0        0        0      317 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/segmentation_response.py
--rw-r--r--   0        0        0      564 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/summarize_by_segment_response.py
--rw-r--r--   0        0        0      187 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/summarize_response.py
--rw-r--r--   0        0        0      139 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/summary_method.py
--rw-r--r--   0        0        0      222 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/usage_info.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/py.typed
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/services/__init__.py
--rw-r--r--   0        0        0     2296 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/services/sagemaker.py
--rw-r--r--   0        0        0      123 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/tokenizers/__init__.py
--rw-r--r--   0        0        0      608 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/tokenizers/ai21_tokenizer.py
--rw-r--r--   0        0        0      628 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/tokenizers/factory.py
--rw-r--r--   0        0        0      722 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/types.py
--rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/utils/__init__.py
--rw-r--r--   0        0        0      668 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/utils/typing.py
--rw-r--r--   0        0        0       18 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/version.py
--rw-r--r--   0        0        0     2261 2024-05-09 10:37:12.549003 ai21-2.2.4/pyproject.toml
--rw-r--r--   0        0        0    12581 1970-01-01 00:00:00.000000 ai21-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 18:42:02.363846 ai21-2.2.5/LICENSE
+-rw-r--r--   0        0        0    11868 2024-05-14 18:42:02.363846 ai21-2.2.5/README.md
+-rw-r--r--   0        0        0     1575 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/__init__.py
+-rw-r--r--   0        0        0     1014 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/ai21_env_config.py
+-rw-r--r--   0        0        0     2626 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/ai21_http_client.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/__init__.py
+-rw-r--r--   0        0        0      844 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/ai21_bedrock_client.py
+-rw-r--r--   0        0        0       92 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/bedrock_model_id.py
+-rw-r--r--   0        0        0     2414 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/bedrock_session.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/resources/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/resources/bedrock_completion.py
+-rw-r--r--   0        0        0      522 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/bedrock/resources/bedrock_resource.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.363846 ai21-2.2.5/ai21/clients/common/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/answer_base.py
+-rw-r--r--   0        0        0     3710 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/chat_base.py
+-rw-r--r--   0        0        0     4216 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/completion_base.py
+-rw-r--r--   0        0        0     1634 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/custom_model_base.py
+-rw-r--r--   0        0        0     1886 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/dataset_base.py
+-rw-r--r--   0        0        0      888 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/embed_base.py
+-rw-r--r--   0        0        0      577 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/gec_base.py
+-rw-r--r--   0        0        0      771 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/improvements_base.py
+-rw-r--r--   0        0        0     1478 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/paraphrase_base.py
+-rw-r--r--   0        0        0      806 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/segmentation_base.py
+-rw-r--r--   0        0        0     1217 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/summarize_base.py
+-rw-r--r--   0        0        0     1143 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/common/summarize_by_segment_base.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/__init__.py
+-rw-r--r--   0        0        0     1545 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/ai21_sagemaker_client.py
+-rw-r--r--   0        0        0      154 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/constants.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_answer.py
+-rw-r--r--   0        0        0     3194 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_completion.py
+-rw-r--r--   0        0        0      399 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_gec.py
+-rw-r--r--   0        0        0      789 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
+-rw-r--r--   0        0        0      484 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_resource.py
+-rw-r--r--   0        0        0      810 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_summarize.py
+-rw-r--r--   0        0        0     2522 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/sagemaker/sagemaker_session.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/__init__.py
+-rw-r--r--   0        0        0     3496 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/ai21_client.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2435 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/chat/chat_completions.py
+-rw-r--r--   0        0        0      574 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_answer.py
+-rw-r--r--   0        0        0     2061 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_chat.py
+-rw-r--r--   0        0        0     1996 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_completion.py
+-rw-r--r--   0        0        0     1290 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_custom_model.py
+-rw-r--r--   0        0        0     1507 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_dataset.py
+-rw-r--r--   0        0        0      584 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_embed.py
+-rw-r--r--   0        0        0      472 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_gec.py
+-rw-r--r--   0        0        0      739 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_improvements.py
+-rw-r--r--   0        0        0     3670 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_library.py
+-rw-r--r--   0        0        0      873 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_paraphrase.py
+-rw-r--r--   0        0        0     1096 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_resource.py
+-rw-r--r--   0        0        0      612 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_segmentation.py
+-rw-r--r--   0        0        0      891 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_summarize.py
+-rw-r--r--   0        0        0      782 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/clients/studio/resources/studio_summarize_by_segment.py
+-rw-r--r--   0        0        0       64 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/constants.py
+-rw-r--r--   0        0        0     2615 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/errors.py
+-rw-r--r--   0        0        0     4868 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/http_client.py
+-rw-r--r--   0        0        0      484 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/logger.py
+-rw-r--r--   0        0        0     2633 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/ai21_base_model_mixin.py
+-rw-r--r--   0        0        0      343 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat/__init__.py
+-rw-r--r--   0        0        0      592 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat/chat_completion_response.py
+-rw-r--r--   0        0        0      219 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat/chat_message.py
+-rw-r--r--   0        0        0       97 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat/role_type.py
+-rw-r--r--   0        0        0      233 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/chat_message.py
+-rw-r--r--   0        0        0       89 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/document_type.py
+-rw-r--r--   0        0        0       96 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/embed_type.py
+-rw-r--r--   0        0        0      286 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/improvement_type.py
+-rw-r--r--   0        0        0      410 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/logprobs.py
+-rw-r--r--   0        0        0      168 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/paraphrase_style_type.py
+-rw-r--r--   0        0        0      503 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/penalty.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/answer_response.py
+-rw-r--r--   0        0        0      518 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/chat_response.py
+-rw-r--r--   0        0        0      786 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/completion_response.py
+-rw-r--r--   0        0        0      713 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/custom_model_response.py
+-rw-r--r--   0        0        0      376 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/dataset_response.py
+-rw-r--r--   0        0        0      300 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/embed_response.py
+-rw-r--r--   0        0        0      550 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/file_response.py
+-rw-r--r--   0        0        0      635 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/gec_response.py
+-rw-r--r--   0        0        0      401 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/improvement_response.py
+-rw-r--r--   0        0        0      469 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/library_answer_response.py
+-rw-r--r--   0        0        0      450 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/library_search_response.py
+-rw-r--r--   0        0        0      294 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/paraphrase_response.py
+-rw-r--r--   0        0        0      317 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/segmentation_response.py
+-rw-r--r--   0        0        0      564 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/summarize_by_segment_response.py
+-rw-r--r--   0        0        0      187 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/responses/summarize_response.py
+-rw-r--r--   0        0        0      139 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/summary_method.py
+-rw-r--r--   0        0        0      222 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/models/usage_info.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/py.typed
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/services/__init__.py
+-rw-r--r--   0        0        0     2296 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/services/sagemaker.py
+-rw-r--r--   0        0        0      123 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/tokenizers/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/tokenizers/ai21_tokenizer.py
+-rw-r--r--   0        0        0      628 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/tokenizers/factory.py
+-rw-r--r--   0        0        0      722 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/types.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/utils/__init__.py
+-rw-r--r--   0        0        0      668 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/utils/typing.py
+-rw-r--r--   0        0        0       18 2024-05-14 18:42:02.367846 ai21-2.2.5/ai21/version.py
+-rw-r--r--   0        0        0     2269 2024-05-14 18:42:02.371846 ai21-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0    12580 1970-01-01 00:00:00.000000 ai21-2.2.5/PKG-INFO
```

### Comparing `ai21-2.2.4/LICENSE` & `ai21-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/README.md` & `ai21-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/__init__.py` & `ai21-2.2.5/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/ai21_env_config.py` & `ai21-2.2.5/ai21/ai21_env_config.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/ai21_http_client.py` & `ai21-2.2.5/ai21/ai21_http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/bedrock/ai21_bedrock_client.py` & `ai21-2.2.5/ai21/clients/bedrock/ai21_bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/bedrock/bedrock_session.py` & `ai21-2.2.5/ai21/clients/bedrock/bedrock_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/bedrock/resources/bedrock_completion.py` & `ai21-2.2.5/ai21/clients/bedrock/resources/bedrock_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/bedrock/resources/bedrock_resource.py` & `ai21-2.2.5/ai21/clients/bedrock/resources/bedrock_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/answer_base.py` & `ai21-2.2.5/ai21/clients/common/answer_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/chat_base.py` & `ai21-2.2.5/ai21/clients/common/chat_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/completion_base.py` & `ai21-2.2.5/ai21/clients/common/completion_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/custom_model_base.py` & `ai21-2.2.5/ai21/clients/common/custom_model_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/dataset_base.py` & `ai21-2.2.5/ai21/clients/common/dataset_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/embed_base.py` & `ai21-2.2.5/ai21/clients/common/embed_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/gec_base.py` & `ai21-2.2.5/ai21/clients/common/gec_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/improvements_base.py` & `ai21-2.2.5/ai21/clients/common/improvements_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/paraphrase_base.py` & `ai21-2.2.5/ai21/clients/common/paraphrase_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/segmentation_base.py` & `ai21-2.2.5/ai21/clients/common/segmentation_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/summarize_base.py` & `ai21-2.2.5/ai21/clients/common/summarize_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/common/summarize_by_segment_base.py` & `ai21-2.2.5/ai21/clients/common/summarize_by_segment_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/sagemaker/ai21_sagemaker_client.py` & `ai21-2.2.5/ai21/clients/sagemaker/ai21_sagemaker_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_completion.py` & `ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py` & `ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_summarize.py` & `ai21-2.2.5/ai21/clients/sagemaker/resources/sagemaker_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/sagemaker/sagemaker_session.py` & `ai21-2.2.5/ai21/clients/sagemaker/sagemaker_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/ai21_client.py` & `ai21-2.2.5/ai21/clients/studio/ai21_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/chat/chat_completions.py` & `ai21-2.2.5/ai21/clients/studio/resources/chat/chat_completions.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_answer.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_answer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_chat.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_chat.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_completion.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_custom_model.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_dataset.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_embed.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_embed.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_improvements.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_library.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_library.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_paraphrase.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_resource.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_segmentation.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_summarize.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/clients/studio/resources/studio_summarize_by_segment.py` & `ai21-2.2.5/ai21/clients/studio/resources/studio_summarize_by_segment.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/errors.py` & `ai21-2.2.5/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/http_client.py` & `ai21-2.2.5/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/models/__init__.py` & `ai21-2.2.5/ai21/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/models/chat/chat_completion_response.py` & `ai21-2.2.5/ai21/models/chat/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/models/responses/chat_response.py` & `ai21-2.2.5/ai21/models/responses/chat_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/models/responses/completion_response.py` & `ai21-2.2.5/ai21/models/responses/completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/models/responses/custom_model_response.py` & `ai21-2.2.5/ai21/models/responses/custom_model_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/models/responses/file_response.py` & `ai21-2.2.5/ai21/models/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/models/responses/gec_response.py` & `ai21-2.2.5/ai21/models/responses/gec_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/models/responses/summarize_by_segment_response.py` & `ai21-2.2.5/ai21/models/responses/summarize_by_segment_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/services/sagemaker.py` & `ai21-2.2.5/ai21/services/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/tokenizers/ai21_tokenizer.py` & `ai21-2.2.5/ai21/tokenizers/ai21_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/tokenizers/factory.py` & `ai21-2.2.5/ai21/tokenizers/factory.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/types.py` & `ai21-2.2.5/ai21/types.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/ai21/utils/typing.py` & `ai21-2.2.5/ai21/utils/typing.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.4/pyproject.toml` & `ai21-2.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,26 +42,26 @@
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "if typing.TYPE_CHECKING:"
 ]
 
 [tool.poetry]
 name = "ai21"
-version = "2.2.4"
+version = "2.2.5"
 description = ""
 authors = ["AI21 Labs"]
 readme = "README.md"
 packages = [
     { include = "ai21" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
-ai21-tokenizer = "^0.9.0"
+ai21-tokenizer = ">=0.9.1,<1.0.0"
 boto3 = { version = "^1.28.82", optional = true }
 dataclasses-json = "^0.6.3"
 typing-extensions = "^4.9.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
```

### Comparing `ai21-2.2.4/PKG-INFO` & `ai21-2.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 2.2.4
+Version: 2.2.5
 Summary: 
 Author: AI21 Labs
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: aws
-Requires-Dist: ai21-tokenizer (>=0.9.0,<0.10.0)
+Requires-Dist: ai21-tokenizer (>=0.9.1,<1.0.0)
 Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: ai21 Version: 2.2.4 Summary: Author: AI21 Labs
+Metadata-Version: 2.1 Name: ai21 Version: 2.2.5 Summary: Author: AI21 Labs
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: aws Requires-Dist: ai21-tokenizer
-(>=0.9.0,<0.10.0) Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
+(>=0.9.1,<1.0.0) Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
                       ************ _AA_II_22_11_ _LL_aa_bb_ss_ _PP_yy_tt_hh_oo_nn_ _SS_DD_KK ************
 [//]: # "Add when public" [//]: # '_[_T_e_s_t_]' [//]: # '_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
 _v_e_r_s_i_o_n_s_]'
  _[_T_e_s_t_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_o_e_t_r_y_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
```

