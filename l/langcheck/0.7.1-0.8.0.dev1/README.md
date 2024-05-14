# Comparing `tmp/langcheck-0.7.1.tar.gz` & `tmp/langcheck-0.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcheck-0.7.1.tar", last modified: Wed May  8 14:43:13 2024, max compression
+gzip compressed data, was "langcheck-0.8.0.dev1.tar", last modified: Tue May 14 05:37:38 2024, max compression
```

## Comparing `langcheck-0.7.1.tar` & `langcheck-0.8.0.dev1.tar`

### file list

```diff
@@ -1,133 +1,132 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.738261 langcheck-0.7.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-08-11 13:51:15.000000 langcheck-0.7.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10659 2024-05-08 14:43:13.736810 langcheck-0.7.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6957 2024-04-05 07:29:40.000000 langcheck-0.7.1/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2921 2024-05-08 14:42:28.000000 langcheck-0.7.1/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      160 2024-05-08 14:43:13.740365 langcheck-0.7.1/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.240353 langcheck-0.7.1/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.315610 langcheck-0.7.1/src/langcheck/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      103 2023-11-19 15:49:24.000000 langcheck-0.7.1/src/langcheck/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      486 2023-12-05 05:59:04.000000 langcheck-0.7.1/src/langcheck/_handle_logs.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.344792 langcheck-0.7.1/src/langcheck/augment/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      554 2024-04-03 12:24:40.000000 langcheck-0.7.1/src/langcheck/augment/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.387167 langcheck-0.7.1/src/langcheck/augment/en/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      523 2023-12-12 02:12:39.000000 langcheck-0.7.1/src/langcheck/augment/en/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1424 2023-12-05 05:59:05.000000 langcheck-0.7.1/src/langcheck/augment/en/_change_case.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.398234 langcheck-0.7.1/src/langcheck/augment/en/_gender/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-12-12 02:12:39.000000 langcheck-0.7.1/src/langcheck/augment/en/_gender/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4173 2024-03-02 15:56:50.000000 langcheck-0.7.1/src/langcheck/augment/en/_gender/_gender.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3851 2023-12-12 02:12:39.000000 langcheck-0.7.1/src/langcheck/augment/en/_gender/_gender_pronouns.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2697 2023-12-05 05:59:05.000000 langcheck-0.7.1/src/langcheck/augment/en/_keyboard_typo.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2364 2023-12-05 05:59:05.000000 langcheck-0.7.1/src/langcheck/augment/en/_ocr_typo.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1364 2023-12-05 05:59:05.000000 langcheck-0.7.1/src/langcheck/augment/en/_remove_punctuation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4276 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/augment/en/_rephrase.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1815 2023-12-05 05:59:05.000000 langcheck-0.7.1/src/langcheck/augment/en/_synonym.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.405617 langcheck-0.7.1/src/langcheck/augment/ja/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       73 2024-01-11 08:18:01.000000 langcheck-0.7.1/src/langcheck/augment/ja/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2076 2024-04-03 12:24:40.000000 langcheck-0.7.1/src/langcheck/augment/ja/_synonym.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.428670 langcheck-0.7.1/src/langcheck/metrics/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2124 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3798 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/_pairwise_text_quality_utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9754 2024-04-03 12:24:40.000000 langcheck-0.7.1/src/langcheck/metrics/_validation.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.448898 langcheck-0.7.1/src/langcheck/metrics/de/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      905 2024-02-24 16:17:52.000000 langcheck-0.7.1/src/langcheck/metrics/de/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      632 2024-02-24 16:17:52.000000 langcheck-0.7.1/src/langcheck/metrics/de/_tokenizers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2741 2024-03-22 04:27:03.000000 langcheck-0.7.1/src/langcheck/metrics/de/_translation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9336 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/de/reference_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21572 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/de/reference_free_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8115 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/de/source_based_text_quality.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.467775 langcheck-0.7.1/src/langcheck/metrics/en/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      858 2024-04-03 12:24:40.000000 langcheck-0.7.1/src/langcheck/metrics/en/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5046 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/en/pairwise_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9394 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/en/reference_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23239 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/en/reference_free_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11734 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/en/source_based_text_quality.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.489643 langcheck-0.7.1/src/langcheck/metrics/eval_clients/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      620 2024-05-08 10:14:25.000000 langcheck-0.7.1/src/langcheck/metrics/eval_clients/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7348 2024-05-08 10:14:25.000000 langcheck-0.7.1/src/langcheck/metrics/eval_clients/_anthropic.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4901 2024-05-08 13:24:50.000000 langcheck-0.7.1/src/langcheck/metrics/eval_clients/_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9366 2024-05-08 10:14:25.000000 langcheck-0.7.1/src/langcheck/metrics/eval_clients/_gemini.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8454 2024-05-03 02:46:01.000000 langcheck-0.7.1/src/langcheck/metrics/eval_clients/_google.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13970 2024-05-08 10:14:25.000000 langcheck-0.7.1/src/langcheck/metrics/eval_clients/_openai.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.513860 langcheck-0.7.1/src/langcheck/metrics/ja/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      857 2024-04-05 07:29:40.000000 langcheck-0.7.1/src/langcheck/metrics/ja/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3468 2023-11-29 01:09:25.000000 langcheck-0.7.1/src/langcheck/metrics/ja/_tokenizers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5047 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/ja/pairwise_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10028 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/ja/reference_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22556 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/ja/reference_free_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10034 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/ja/source_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11027 2024-04-03 12:24:40.000000 langcheck-0.7.1/src/langcheck/metrics/metric_value.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.524750 langcheck-0.7.1/src/langcheck/metrics/model_manager/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       70 2024-03-01 06:48:01.000000 langcheck-0.7.1/src/langcheck/metrics/model_manager/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4189 2024-03-22 04:27:03.000000 langcheck-0.7.1/src/langcheck/metrics/model_manager/_model_loader.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11909 2024-03-22 04:27:03.000000 langcheck-0.7.1/src/langcheck/metrics/model_manager/_model_management.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.527683 langcheck-0.7.1/src/langcheck/metrics/model_manager/config/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3596 2024-03-22 04:27:03.000000 langcheck-0.7.1/src/langcheck/metrics/model_manager/config/metric_config.yaml
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.531721 langcheck-0.7.1/src/langcheck/metrics/prompts/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      408 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/_utils.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.266696 langcheck-0.7.1/src/langcheck/metrics/prompts/de/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.538452 langcheck-0.7.1/src/langcheck/metrics/prompts/de/get_score/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2024-05-08 14:24:03.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/de/get_score/function_calling.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2024-05-08 14:24:03.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/de/get_score/plain_text.j2
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.559997 langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/answer_relevance.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      863 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/context_relevance.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1041 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/factual_consistency.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      849 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/fluency.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      589 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/sentiment.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/toxicity.j2
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.272149 langcheck-0.7.1/src/langcheck/metrics/prompts/en/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.567744 langcheck-0.7.1/src/langcheck/metrics/prompts/en/get_score/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      245 2024-05-08 10:14:25.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/get_score/function_calling.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      365 2024-05-08 10:14:25.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/get_score/plain_text.j2
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.593682 langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      737 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/answer_relevance.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      741 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/context_relevance.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      953 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/factual_consistency.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      761 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/fluency.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2189 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/pairwise_comparison.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      546 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/sentiment.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      336 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/toxicity.j2
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.277428 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.601144 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/get_score/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      278 2024-05-08 14:24:03.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/get_score/function_calling.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-05-08 14:24:03.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/get_score/plain_text.j2
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.656620 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      923 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/answer_relevance.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      968 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/context_relevance.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1527 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/factual_consistency.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      968 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/fluency.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2421 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/pairwise_comparison.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      706 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/sentiment.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)      518 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/toxicity.j2
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1814 2023-12-05 05:59:05.000000 langcheck-0.7.1/src/langcheck/metrics/reference_based_text_quality.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.668573 langcheck-0.7.1/src/langcheck/metrics/scorer/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4855 2024-03-22 04:27:03.000000 langcheck-0.7.1/src/langcheck/metrics/scorer/_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6481 2024-03-22 04:27:03.000000 langcheck-0.7.1/src/langcheck/metrics/scorer/detoxify_models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5656 2024-03-22 04:27:03.000000 langcheck-0.7.1/src/langcheck/metrics/scorer/hf_models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14772 2023-12-05 05:59:05.000000 langcheck-0.7.1/src/langcheck/metrics/text_structure.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.691726 langcheck-0.7.1/src/langcheck/metrics/zh/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      547 2024-03-01 06:48:01.000000 langcheck-0.7.1/src/langcheck/metrics/zh/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2024-03-01 06:48:01.000000 langcheck-0.7.1/src/langcheck/metrics/zh/_tokenizers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10273 2024-04-30 05:42:20.000000 langcheck-0.7.1/src/langcheck/metrics/zh/reference_based_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12361 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/zh/reference_free_text_quality.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4464 2024-04-26 01:26:17.000000 langcheck-0.7.1/src/langcheck/metrics/zh/source_based_text_quality.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.712550 langcheck-0.7.1/src/langcheck/plot/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      128 2023-09-26 12:28:25.000000 langcheck-0.7.1/src/langcheck/plot/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      538 2023-09-26 12:28:25.000000 langcheck-0.7.1/src/langcheck/plot/_css.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4112 2023-11-29 01:09:25.000000 langcheck-0.7.1/src/langcheck/plot/_histogram.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15343 2024-04-03 12:24:40.000000 langcheck-0.7.1/src/langcheck/plot/_scatter.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1303 2023-11-29 01:09:25.000000 langcheck-0.7.1/src/langcheck/plot/_utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1940 2023-09-26 12:28:25.000000 langcheck-0.7.1/src/langcheck/stats.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.724432 langcheck-0.7.1/src/langcheck/utils/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       66 2023-09-26 12:28:25.000000 langcheck-0.7.1/src/langcheck/utils/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      263 2023-09-26 12:28:25.000000 langcheck-0.7.1/src/langcheck/utils/io.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      460 2023-12-05 05:59:05.000000 langcheck-0.7.1/src/langcheck/utils/progess_bar.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.731233 langcheck-0.7.1/src/langcheck.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10659 2024-05-08 14:43:13.000000 langcheck-0.7.1/src/langcheck.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4627 2024-05-08 14:43:13.000000 langcheck-0.7.1/src/langcheck.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-08 14:43:13.000000 langcheck-0.7.1/src/langcheck.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      733 2024-05-08 14:43:13.000000 langcheck-0.7.1/src/langcheck.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2024-05-08 14:43:13.000000 langcheck-0.7.1/src/langcheck.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-08 14:43:13.727859 langcheck-0.7.1/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1119 2023-11-19 15:49:24.000000 langcheck-0.7.1/tests/test_stats.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:38.721119 langcheck-0.8.0.dev1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-10-10 09:38:20.000000 langcheck-0.8.0.dev1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10664 2024-05-14 05:37:38.706225 langcheck-0.8.0.dev1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6957 2024-04-07 14:19:34.000000 langcheck-0.8.0.dev1/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2926 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      160 2024-05-14 05:37:38.742902 langcheck-0.8.0.dev1/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:32.834708 langcheck-0.8.0.dev1/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:33.854785 langcheck-0.8.0.dev1/src/langcheck/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      103 2023-11-06 02:00:48.000000 langcheck-0.8.0.dev1/src/langcheck/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      486 2023-11-16 07:47:37.000000 langcheck-0.8.0.dev1/src/langcheck/_handle_logs.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:34.153989 langcheck-0.8.0.dev1/src/langcheck/augment/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      554 2024-04-03 02:39:44.000000 langcheck-0.8.0.dev1/src/langcheck/augment/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:34.410423 langcheck-0.8.0.dev1/src/langcheck/augment/en/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      523 2023-12-26 07:19:48.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1424 2023-11-16 07:47:37.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_change_case.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:34.553992 langcheck-0.8.0.dev1/src/langcheck/augment/en/_gender/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-12-26 07:19:48.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_gender/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4173 2024-03-02 07:03:11.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_gender/_gender.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3851 2023-12-26 07:19:49.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_gender/_gender_pronouns.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2697 2023-11-16 07:47:37.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_keyboard_typo.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2364 2023-11-16 07:47:37.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_ocr_typo.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1364 2023-11-16 07:47:37.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_remove_punctuation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4276 2024-05-03 09:15:20.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_rephrase.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1815 2023-11-16 07:47:37.000000 langcheck-0.8.0.dev1/src/langcheck/augment/en/_synonym.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:34.628123 langcheck-0.8.0.dev1/src/langcheck/augment/ja/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       73 2024-02-29 10:04:37.000000 langcheck-0.8.0.dev1/src/langcheck/augment/ja/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2076 2024-04-03 09:30:38.000000 langcheck-0.8.0.dev1/src/langcheck/augment/ja/_synonym.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:34.817741 langcheck-0.8.0.dev1/src/langcheck/metrics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2124 2024-05-03 09:15:20.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3798 2024-05-03 09:15:20.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/_pairwise_text_quality_utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9754 2024-04-02 00:47:28.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/_validation.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:35.471996 langcheck-0.8.0.dev1/src/langcheck/metrics/de/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      905 2024-02-29 10:04:38.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/de/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      632 2024-02-29 10:04:38.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/de/_tokenizers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2741 2024-03-18 09:06:28.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/de/_translation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9336 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/de/reference_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    21572 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/de/reference_free_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8115 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/de/source_based_text_quality.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:35.649127 langcheck-0.8.0.dev1/src/langcheck/metrics/en/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      858 2024-04-02 00:47:28.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/en/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5046 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/en/pairwise_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9394 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/en/reference_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    23239 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/en/reference_free_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11734 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/en/source_based_text_quality.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:35.824921 langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      620 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7348 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/_anthropic.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4901 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9366 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/_gemini.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13970 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:36.054249 langcheck-0.8.0.dev1/src/langcheck/metrics/ja/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      857 2024-04-07 14:19:34.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/ja/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3468 2023-11-16 07:47:37.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/ja/_tokenizers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5047 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/ja/pairwise_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10028 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/ja/reference_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22556 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/ja/reference_free_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10034 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/ja/source_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11027 2024-04-02 00:47:28.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/metric_value.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:36.152051 langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       70 2024-03-02 07:03:12.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4189 2024-03-18 09:06:29.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/_model_loader.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11909 2024-03-18 09:06:29.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/_model_management.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:36.184878 langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/config/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3596 2024-03-18 09:06:29.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/config/metric_config.yaml
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:36.225271 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      408 2024-05-03 09:15:21.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/_utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:33.024239 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:36.276975 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/get_score/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/get_score/function_calling.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/get_score/plain_text.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:36.447847 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      918 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/answer_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      953 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/context_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1131 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/factual_consistency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      939 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/fluency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      679 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/sentiment.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      476 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/toxicity.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:33.059676 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:36.496426 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/get_score/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      245 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/get_score/function_calling.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      365 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/get_score/plain_text.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:37.224812 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      808 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/answer_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      812 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/context_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1024 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/factual_consistency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      832 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/fluency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2260 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/pairwise_comparison.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      617 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/sentiment.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      407 2024-05-14 05:29:43.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/toxicity.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:33.094869 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:37.287668 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/get_score/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      278 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/get_score/function_calling.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      397 2024-05-08 14:48:07.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/get_score/plain_text.j2
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:37.545703 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1019 2024-05-14 05:29:44.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/answer_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1064 2024-05-14 05:29:44.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/context_relevance.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1623 2024-05-14 05:29:44.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/factual_consistency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1064 2024-05-14 05:29:44.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/fluency.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2517 2024-05-14 05:29:44.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/pairwise_comparison.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      802 2024-05-14 05:29:44.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/sentiment.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      615 2024-05-14 05:29:44.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/toxicity.j2
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1814 2023-12-07 09:44:42.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/reference_based_text_quality.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:37.641867 langcheck-0.8.0.dev1/src/langcheck/metrics/scorer/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4855 2024-04-03 02:48:06.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/scorer/_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6481 2024-03-18 09:06:30.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/scorer/detoxify_models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5656 2024-03-18 09:06:30.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/scorer/hf_models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14772 2023-12-07 09:44:42.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/text_structure.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:37.875110 langcheck-0.8.0.dev1/src/langcheck/metrics/zh/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      547 2024-03-02 07:03:12.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/zh/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2560 2024-03-02 07:03:12.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/zh/_tokenizers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10273 2024-05-03 09:15:24.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/zh/reference_based_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12361 2024-05-03 09:15:24.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/zh/reference_free_text_quality.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4464 2024-05-03 09:15:24.000000 langcheck-0.8.0.dev1/src/langcheck/metrics/zh/source_based_text_quality.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:38.036738 langcheck-0.8.0.dev1/src/langcheck/plot/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      128 2023-10-10 09:38:20.000000 langcheck-0.8.0.dev1/src/langcheck/plot/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      538 2023-10-10 09:38:20.000000 langcheck-0.8.0.dev1/src/langcheck/plot/_css.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4112 2023-11-06 02:01:01.000000 langcheck-0.8.0.dev1/src/langcheck/plot/_histogram.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15343 2024-04-02 00:47:28.000000 langcheck-0.8.0.dev1/src/langcheck/plot/_scatter.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1303 2023-11-06 02:01:01.000000 langcheck-0.8.0.dev1/src/langcheck/plot/_utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1940 2023-10-10 09:38:20.000000 langcheck-0.8.0.dev1/src/langcheck/stats.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:38.141749 langcheck-0.8.0.dev1/src/langcheck/utils/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       66 2023-10-10 09:38:20.000000 langcheck-0.8.0.dev1/src/langcheck/utils/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      263 2023-10-10 09:38:20.000000 langcheck-0.8.0.dev1/src/langcheck/utils/io.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      460 2023-12-26 05:12:57.000000 langcheck-0.8.0.dev1/src/langcheck/utils/progess_bar.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:38.661608 langcheck-0.8.0.dev1/src/langcheck.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10664 2024-05-14 05:37:32.000000 langcheck-0.8.0.dev1/src/langcheck.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4581 2024-05-14 05:37:32.000000 langcheck-0.8.0.dev1/src/langcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-14 05:37:32.000000 langcheck-0.8.0.dev1/src/langcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      733 2024-05-14 05:37:32.000000 langcheck-0.8.0.dev1/src/langcheck.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2024-05-14 05:37:32.000000 langcheck-0.8.0.dev1/src/langcheck.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-14 05:37:38.169034 langcheck-0.8.0.dev1/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1119 2023-10-25 04:25:55.000000 langcheck-0.8.0.dev1/tests/test_stats.py
```

### Comparing `langcheck-0.7.1/LICENSE` & `langcheck-0.8.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/PKG-INFO` & `langcheck-0.8.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcheck
-Version: 0.7.1
+Version: 0.8.0.dev1
 Summary: Simple, Pythonic building blocks to evaluate LLM-based applications
 Author-email: Citadel AI <info@citadel.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Citadel AI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `langcheck-0.7.1/README.md` & `langcheck-0.8.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/pyproject.toml` & `langcheck-0.8.0.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langcheck"
-version = "0.7.1"
+version = "0.8.0.dev1"
 description = "Simple, Pythonic building blocks to evaluate LLM-based applications"
 readme = "README.md"
 authors = [{ name = "Citadel AI", email = "info@citadel.co.jp" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `langcheck-0.7.1/src/langcheck/augment/__init__.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/__init__.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/_change_case.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/_change_case.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/_gender/_gender.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/_gender/_gender.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/_gender/_gender_pronouns.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/_gender/_gender_pronouns.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/_keyboard_typo.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/_keyboard_typo.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/_ocr_typo.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/_ocr_typo.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/_remove_punctuation.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/_remove_punctuation.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/_rephrase.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/_rephrase.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/en/_synonym.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/en/_synonym.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/augment/ja/_synonym.py` & `langcheck-0.8.0.dev1/src/langcheck/augment/ja/_synonym.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/__init__.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/_pairwise_text_quality_utils.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/_pairwise_text_quality_utils.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/_validation.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/_validation.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/de/__init__.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/de/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/de/_tokenizers.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/de/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/de/_translation.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/de/_translation.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/de/reference_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/de/reference_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/de/reference_free_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/de/reference_free_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/de/source_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/de/source_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/en/__init__.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/en/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/en/pairwise_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/en/pairwise_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/en/reference_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/en/reference_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/en/reference_free_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/en/reference_free_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/en/source_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/en/source_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/eval_clients/__init__.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/eval_clients/_anthropic.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/_anthropic.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/eval_clients/_base.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/_base.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/eval_clients/_gemini.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/_gemini.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/eval_clients/_openai.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/eval_clients/_openai.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/ja/__init__.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/ja/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/ja/_tokenizers.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/ja/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/ja/pairwise_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/ja/pairwise_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/ja/reference_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/ja/reference_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/ja/reference_free_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/ja/reference_free_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/ja/source_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/ja/source_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/metric_value.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/metric_value.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/model_manager/_model_loader.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/_model_loader.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/model_manager/_model_management.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/_model_management.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/model_manager/config/metric_config.yaml` & `langcheck-0.8.0.dev1/src/langcheck/metrics/model_manager/config/metric_config.yaml`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/answer_relevance.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/answer_relevance.j2`

 * *Files 16% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
 Bestimmen Sie, ob die Antwort eine relevante Reaktion auf die Benutzeranfrage ist.
 Die verfügbaren Bewertungen sind:
 `Fully Relevant` - Die Antwort ist vollständig relevant und beantwortet die Benutzeranfrage vollständig.
 `Partially Relevant` - Die Antwort ist teilweise relevant für die Benutzeranfrage, beantwortet sie jedoch nicht vollständig oder enthält einige irrelevante Informationen.
 `Not Relevant` - Die Antwort ist nicht relevant für die Benutzeranfrage oder geht nicht richtig auf die Benutzeranfrage ein.
 
-Atmen Sie tief durch und bearbeiten Sie dieses Problem Schritt für Schritt.
+Atmen Sie tief durch und bearbeiten Sie dieses Problem Schritt für Schritt. Geben Sie zunächst Ihren Gedankengang aus und liefern Sie dann Ihre endgültige Antwort.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/context_relevance.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/context_relevance.j2`

 * *Files 9% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 Bestimmen Sie, ob die Quelle die relevanten und notwendigen Informationen enthält, um auf die Anfrage des Benutzers zu antworten.
 Die verfügbaren Bewertungen sind:
 `Fully Relevant` - Der Quelltext enthält die Informationen, die notwendig sind, um auf die Anfrage des Benutzers zu antworten.
 `Partially Relevant` - Der Quelltext ist teilweise relevant für die Anfrage des Benutzers, enthält aber nicht alle Informationen,
 die notwendig sind, um auf die Anfrage des Benutzers zu antworten.
 `Not Relevant` - Der Quelltext ist nicht relevant für die Anfrage des Benutzers.
 
-Atmen Sie tief durch und arbeiten Sie Schritt für Schritt an diesem Problem.
+Atmen Sie tief durch und arbeiten Sie Schritt für Schritt an diesem Problem. Geben Sie zunächst Ihren Gedankengang aus und liefern Sie dann Ihre endgültige Antwort.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/factual_consistency.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/factual_consistency.j2`

 * *Files 14% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 Bestimmen Sie, ob die eingereichte Behauptung faktisch konsistent mit der Quelle ist. Die verfügbaren Bewertungen sind:
 `Fully Consistent` - Die eingereichte Behauptung ist vollständig faktisch konsistent mit dem Quelltext.
 `Partially Consistent` - Die eingereichte Behauptung ist teilweise faktisch konsistent mit dem Quelltext.
 Es gibt einige Aspekte der Behauptung, die faktisch konsistent sind, aber auch einige, die es nicht sind.
 `Not Consistent` - Die eingereichte Behauptung ist nicht faktisch konsistent mit dem Quelltext.
 
-Atmen Sie tief durch und bearbeiten Sie dieses Problem Schritt für Schritt.
+Atmen Sie tief durch und bearbeiten Sie dieses Problem Schritt für Schritt. Geben Sie zunächst Ihren Gedankengang aus und liefern Sie dann Ihre endgültige Antwort.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/fluency.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/fluency.j2`

 * *Files 13% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 [ENDE DATEN]
 
 Bestimmen Sie die Flüssigkeit der eingereichten Aussage. Die verfügbaren Bewertungen sind:
 `Poor` - Die Aussage hat viele Fehler, die sie schwer verständlich oder unnatürlich wirken lassen.
 `Fair` - Die Aussage hat einige Fehler, die die Klarheit oder Flüssigkeit des Textes beeinträchtigen, aber die Hauptpunkte sind dennoch verständlich.
 `Good` - Die Aussage hat wenige oder keine Fehler und ist leicht zu lesen undmzu verstehen.
 
-Atmen Sie tief durch und bearbeiten Sie dieses Problem Schritt für Schritt.
+Atmen Sie tief durch und bearbeiten Sie dieses Problem Schritt für Schritt. Geben Sie zunächst Ihren Gedankengang aus und liefern Sie dann Ihre endgültige Antwort.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/de/metrics/sentiment.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/de/metrics/sentiment.j2`

 * *Files 11% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 [ENDE DATEN]
 
 Bestimmen Sie die vorherrschende Stimmung der eingereichten Aussage. Die verfügbaren Bewertungen sind:
 `Positive` - Die eingereichte Aussage hat überwiegend eine positive Stimmung
 `Negative` - Die eingereichte Aussage hat überwiegend eine negative Stimmung
 `Neutral` - Die eingereichte Aussage hat weder eine positive noch negative Stimmung
 
-Atmen Sie tief durch und bearbeiten Sie dieses Problem Schritt für Schritt.
+Atmen Sie tief durch und bearbeiten Sie dieses Problem Schritt für Schritt. Geben Sie zunächst Ihren Gedankengang aus und liefern Sie dann Ihre endgültige Antwort.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/answer_relevance.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/answer_relevance.j2`

 * *Files 7% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
 Determine whether the answer is a relevant response to the user's query.
 The available assessments are:
 `Fully Relevant` - The answer is fully relevant to and fully addresses the user's query.
 `Partially Relevant` - The answer is partially relevant to the user's query, but either does not answer the user's query fully or includes some irrelevant information.
 `Not Relevant` - The answer is not relevant to the user's query, or does not address the user's query properly.
 
-Take a deep breath and work on this problem step-by-step.
+Take a deep breath and work on this problem step-by-step. Output your thought process first, and then provide your final answer.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/context_relevance.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/context_relevance.j2`

 * *Files 25% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 [END DATA]
 
 Determine whether the source contains the relevant and necessary information needed to respond to the user's query. The available assessments are:
 `Fully Relevant` - The source text contains the information necessary to respond to the user's query.
 `Partially Relevant` - The source text is partially relevant to the user's query, but does not contain all the information necessary to respond to the user's query.
 `Not Relevant` - The source text is not relevant to the user's query.
 
-Take a deep breath and work on this problem step-by-step.
+Take a deep breath and work on this problem step-by-step. Output your thought process first, and then provide your final answer.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/factual_consistency.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/factual_consistency.j2`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 Determine whether the submitted claim is factually consistent with the source. The available assessments are:
 `Fully Consistent` - The submitted claim is fully factually consistent with the source text.
 `Partially Consistent` - The submitted claim is partially factually consistent with the source text.
 There are some aspects of the claim that are factually consistent, but some aspects that are not.
 `Not Consistent` - The submitted claim is not factually consistent with the source text.
 
-Take a deep breath and work on this problem step-by-step.
+Take a deep breath and work on this problem step-by-step. Output your thought process first, and then provide your final answer.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/pairwise_comparison.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/pairwise_comparison.j2`

 * *Files 5% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 {% endif %}
 Do not allow the order in which the responses were presented to influence your assessment.
 Do not allow the length of the responses to influence your assessment. The available assessments are:
 `Response A` - Response A is a better response.
 `Response B` - Response B is a better response.
 `Tie` - The two responses are roughly equal in quality.
 
-Take a deep breath and work on this problem step-by-step.
+Take a deep breath and work on this problem step-by-step. Output your thought process first, and then provide your final answer.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/en/metrics/sentiment.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/en/metrics/sentiment.j2`

 * *Files 12% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 [END DATA]
 
 Determine the predominant sentiment of the submitted statement. The available assessments are:
 `Positive` - The submitted statement has a predominantly positive sentiment
 `Negative` - The submitted statement has a predominantly negative sentiment
 `Neutral` - The submitted statement has neither a positive nor negative sentiment
 
-Take a deep breath and work on this problem step-by-step.
+Take a deep breath and work on this problem step-by-step. Output your thought process first, and then provide your final answer.
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/answer_relevance.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/answer_relevance.j2`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 [END DATA]
 
 ユーザーの質問に対して回答が関連性のあるものかどうかを判断してください。利用可能な評価は以下の通りです:
 `Fully Relevant` - 回答はユーザーの質問に完全に関連し、十分に答えています。
 `Partially Relevant` - 回答はユーザーの質問に部分的に関連していますが、質問に完全に答えていないか、関連しない情報が含まれています。
 `Not Relevant` - 回答はユーザーの質問に関連していない、または質問に適切に対応していません。
 
-深呼吸をして、この問題にステップバイステップで取り組んでください。
+深呼吸をして、この問題にステップバイステップで取り組んでください。まずは考えているプロセスを出力し、最後に答えを提供してください。
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/context_relevance.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/context_relevance.j2`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 [END DATA]
 
 ユーザーの質問に対応するために必要な、関連性のある情報がソースに含まれているかを判断してください。利用可能な評価は以下の通りです:
 `Fully Relevant` - ソーステキストには、ユーザーの質問に対応するために必要な情報が含まれています。
 `Partially Relevant` - ソーステキストはユーザーの質問に部分的に関連していますが、質問に対応するために必要なすべての情報を含んでいません。
 `Not Relevant` - ソーステキストはユーザーの質問に関連していません。
 
-深呼吸をして、この問題にステップバイステップで取り組んでください。
+深呼吸をして、この問題にステップバイステップで取り組んでください。まずは考えているプロセスを出力し、最後に答えを提供してください。
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/factual_consistency.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/factual_consistency.j2`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 `Not Consistent` - 「生成文」は「ソース」と両立することのすることのできない、矛盾する部分を含んでいます。
 `Partially Consistent` - 2つの文章の間に矛盾はありませんが、「生成文」が「ソース」の内容のみからは論理的に導けない内容を含んでいます。
 `Fully Consistent` - 2つの文章の間に矛盾はなく、「生成文」の中の全ての記述が「ソース」の一部に基づいています。
 
 なお、「生成文」は「ソース」の内容を全て含んでいる必要はありません。「生成文」の文章が全て「ソース」の一部に基づいている場合、常に「Fully Consistent」と出力してください。
 逆に、「生成文」の記述が「ソース」に含まれていない場合、「Partially Consistent」または「Not Consistent」と判断する必要があることに注意してください。
 
-深呼吸をして、この問題にステップバイステップで取り組んでください。
+深呼吸をして、この問題にステップバイステップで取り組んでください。まずは考えているプロセスを出力し、最後に答えを提供してください。
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/fluency.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/fluency.j2`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 [END DATA]
 
 提出されたテキストの流暢さを判断してください。利用可能な評価は以下の通りです:
 `Poor` - テキストには多くのエラーがあり、理解が難しく、または不自然に聞こえます。
 `Fair` - テキストにはいくつかのエラーがあり、テキストの明瞭さや滑らかさに影響しますが、主要なポイントはまだ理解できます。
 `Good` - テキストにはほとんどエラーがなく、読みやすく、理解しやすいです。
 
-深呼吸をして、この問題にステップバイステップで取り組んでください。
+深呼吸をして、この問題にステップバイステップで取り組んでください。まずは考えているプロセスを出力し、最後に答えを提供してください。
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/pairwise_comparison.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/pairwise_comparison.j2`

 * *Files 16% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 有用性、正確さ、関連性などの要素を考慮して評価してください。
 {% endif %}
 回答が提示された順序に評価が影響されないようにしてください。回答の長さが評価に影響を与えないようにしてください。利用可能な評価は以下の通りです:
 `Response A` - Response Aがより良い回答です。
 `Response B` - Response Bがより良い回答です。
 `Tie` - 2つの回答は品質がほぼ同等です。
 
-深呼吸をして、この問題にステップバイステップで取り組んでください。
+深呼吸をして、この問題にステップバイステップで取り組んでください。まずは考えているプロセスを出力し、最後に答えを提供してください。
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/prompts/ja/metrics/sentiment.j2` & `langcheck-0.8.0.dev1/src/langcheck/metrics/prompts/ja/metrics/sentiment.j2`

 * *Files 11% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 [END DATA]
 
 提出されたテキストの主要な感情を判断してください。利用可能な評価は以下の通りです:
 `Positive` - 提出されたテキストには主にポジティブな感情があります
 `Negative` - 提出されたテキストには主にネガティブな感情があります
 `Neutral` - 提出されたテキストにはポジティブでもネガティブでもない感情があります
 
-深呼吸をして、この問題にステップバイステップで取り組んでください。
+深呼吸をして、この問題にステップバイステップで取り組んでください。まずは考えているプロセスを出力し、最後に答えを提供してください。
```

### Comparing `langcheck-0.7.1/src/langcheck/metrics/reference_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/reference_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/scorer/_base.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/scorer/_base.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/scorer/detoxify_models.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/scorer/detoxify_models.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/scorer/hf_models.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/scorer/hf_models.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/text_structure.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/text_structure.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/zh/__init__.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/zh/__init__.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/zh/_tokenizers.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/zh/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/zh/reference_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/zh/reference_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/zh/reference_free_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/zh/reference_free_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/metrics/zh/source_based_text_quality.py` & `langcheck-0.8.0.dev1/src/langcheck/metrics/zh/source_based_text_quality.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/plot/_css.py` & `langcheck-0.8.0.dev1/src/langcheck/plot/_css.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/plot/_histogram.py` & `langcheck-0.8.0.dev1/src/langcheck/plot/_histogram.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/plot/_scatter.py` & `langcheck-0.8.0.dev1/src/langcheck/plot/_scatter.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/plot/_utils.py` & `langcheck-0.8.0.dev1/src/langcheck/plot/_utils.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck/stats.py` & `langcheck-0.8.0.dev1/src/langcheck/stats.py`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/src/langcheck.egg-info/PKG-INFO` & `langcheck-0.8.0.dev1/src/langcheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcheck
-Version: 0.7.1
+Version: 0.8.0.dev1
 Summary: Simple, Pythonic building blocks to evaluate LLM-based applications
 Author-email: Citadel AI <info@citadel.co.jp>
 License: MIT License
         
         Copyright (c) 2023 Citadel AI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `langcheck-0.7.1/src/langcheck.egg-info/SOURCES.txt` & `langcheck-0.8.0.dev1/src/langcheck.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 src/langcheck/metrics/en/reference_based_text_quality.py
 src/langcheck/metrics/en/reference_free_text_quality.py
 src/langcheck/metrics/en/source_based_text_quality.py
 src/langcheck/metrics/eval_clients/__init__.py
 src/langcheck/metrics/eval_clients/_anthropic.py
 src/langcheck/metrics/eval_clients/_base.py
 src/langcheck/metrics/eval_clients/_gemini.py
-src/langcheck/metrics/eval_clients/_google.py
 src/langcheck/metrics/eval_clients/_openai.py
 src/langcheck/metrics/ja/__init__.py
 src/langcheck/metrics/ja/_tokenizers.py
 src/langcheck/metrics/ja/pairwise_text_quality.py
 src/langcheck/metrics/ja/reference_based_text_quality.py
 src/langcheck/metrics/ja/reference_free_text_quality.py
 src/langcheck/metrics/ja/source_based_text_quality.py
```

### Comparing `langcheck-0.7.1/src/langcheck.egg-info/requires.txt` & `langcheck-0.8.0.dev1/src/langcheck.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `langcheck-0.7.1/tests/test_stats.py` & `langcheck-0.8.0.dev1/tests/test_stats.py`

 * *Files identical despite different names*

