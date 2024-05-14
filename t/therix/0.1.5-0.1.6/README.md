# Comparing `tmp/therix-0.1.5.tar.gz` & `tmp/therix-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "therix-0.1.5.tar", max compression
+gzip compressed data, was "therix-0.1.6.tar", max compression
```

## Comparing `therix-0.1.5.tar` & `therix-0.1.6.tar`

### file list

```diff
@@ -1,114 +1,118 @@
--rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.5/LICENSE
--rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.5/README.md
--rw-r--r--   0        0        0     1048 2024-05-13 10:00:57.830665 therix-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.5/therix/__init__.py
--rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.5/therix/alembic/README
--rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.5/therix/alembic/env.py
--rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.5/therix/alembic/script.py.mako
--rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.5/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
--rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.5/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
--rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.5/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
--rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.5/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
--rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.5/therix/alembic.ini
--rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.5/therix/core/JSONLoader.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.5/therix/core/__init__.py
--rw-r--r--   0        0        0     2737 2024-05-13 10:00:13.299373 therix-0.1.5/therix/core/cache.py
--rw-r--r--   0        0        0     1399 2024-05-13 10:00:13.301278 therix-0.1.5/therix/core/chat_history/base_chat_history.py
--rw-r--r--   0        0        0     1649 2024-05-13 10:00:13.301411 therix-0.1.5/therix/core/constants.py
--rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.5/therix/core/data_sources.py
--rw-r--r--   0        0        0     1676 2024-04-16 12:12:31.276049 therix-0.1.5/therix/core/embedding_models.py
--rw-r--r--   0        0        0     2374 2024-05-13 10:00:13.301910 therix-0.1.5/therix/core/inference_models.py
--rw-r--r--   0        0        0      317 2024-05-13 10:00:13.302010 therix-0.1.5/therix/core/output_parser.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.5/therix/core/output_source.py
--rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.5/therix/core/pii_filter_config.py
--rw-r--r--   0        0        0     6171 2024-05-13 10:00:13.302291 therix-0.1.5/therix/core/pipeline.py
--rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.5/therix/core/pipeline_component.py
--rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.5/therix/core/response.py
--rw-r--r--   0        0        0      594 2024-05-13 10:00:13.302774 therix-0.1.5/therix/core/summarizer_config.py
--rw-r--r--   0        0        0       98 2024-05-13 10:00:13.302847 therix-0.1.5/therix/core/summarizer_output_model.py
--rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.5/therix/core/trace.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.5/therix/db/__init__.py
--rw-r--r--   0        0        0     3757 2024-04-29 11:17:18.463868 therix-0.1.5/therix/db/db_manager.py
--rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.5/therix/db/session.py
--rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.5/therix/db/tests/__init__.py
--rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.5/therix/db/tests/test_db_manager.py
--rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.5/therix/docs/.gitignore
--rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.5/therix/docs/README.md
--rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.5/therix/docs/babel.config.js
--rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.5/therix/docs/blog/2019-05-28-first-blog-post.md
--rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.5/therix/docs/blog/2019-05-29-long-blog-post.md
--rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.5/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
--rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.5/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.5/therix/docs/blog/2021-08-26-welcome/index.md
--rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.5/therix/docs/blog/authors.yml
--rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.5/therix/docs/docs/LLM-Proxy/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.5/therix/docs/docs/LLM-Proxy/index.md
--rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.5/therix/docs/docs/core-components/_category_.json
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/_category_.json
--rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/caching.md
--rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
--rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
--rw-r--r--   0        0        0     5428 2024-05-13 10:00:13.303279 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
--rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
--rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
--rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/trace.md
--rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations.md
--rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.5/therix/docs/docs/core-components/pipeline-templates.md
--rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.5/therix/docs/docs/core-components/pipeline.md
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.5/therix/docs/docs/introduction/_category_.json
--rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.5/therix/docs/docs/introduction/getting-started.md
--rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.5/therix/docs/docs/introduction/index.md
--rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.5/therix/docs/docs/introduction/installation.md
--rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.5/therix/docs/docs/observability/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.5/therix/docs/docs/observability/index.md
--rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.5/therix/docs/docs/squad/_category_.json
--rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.5/therix/docs/docs/squad/index.md
--rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.5/therix/docs/docs/usage/_category_.json
--rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.5/therix/docs/docs/usage/index.md
--rw-r--r--   0        0        0     3717 2024-05-13 10:00:13.303378 therix-0.1.5/therix/docs/docs/use-cases/Keyword Search.md
--rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.5/therix/docs/docs/use-cases/_category_.json
--rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.5/therix/docs/docs/use-cases/faq.md
--rw-r--r--   0        0        0     3579 2024-05-13 10:00:13.303497 therix-0.1.5/therix/docs/docs/use-cases/pii_filer.md
--rw-r--r--   0        0        0     4177 2024-05-13 10:00:13.303673 therix-0.1.5/therix/docs/docs/use-cases/summarizer.md
--rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.5/therix/docs/docusaurus.config.js
--rw-r--r--   0        0        0      133 2024-05-13 10:00:13.303753 therix-0.1.5/therix/docs/firebase.json
--rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.5/therix/docs/package-lock.json
--rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.5/therix/docs/package.json
--rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.5/therix/docs/sidebars.js
--rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.5/therix/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.5/therix/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.5/therix/docs/src/css/custom.css
--rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.5/therix/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.5/therix/docs/src/pages/markdown-page.md
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.5/therix/docs/static/.nojekyll
--rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.5/therix/docs/static/img/coditas.png
--rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.5/therix/docs/static/img/coditasLogo.svg
--rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.5/therix/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.5/therix/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.5/therix/docs/static/img/favicon.ico
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.5/therix/docs/static/img/icon.svg
--rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.5/therix/docs/static/img/logo.png
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.5/therix/docs/static/img/logo.svg
--rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.5/therix/docs/static/img/therix-logo.png
--rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.5/therix/docs/static/img/undraw_docusaurus_mountain.svg
--rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.5/therix/docs/static/img/undraw_docusaurus_react.svg
--rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.5/therix/docs/static/img/undraw_docusaurus_tree.svg
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.5/therix/entities/__init__.py
--rw-r--r--   0        0        0     2535 2024-05-03 12:50:17.297755 therix-0.1.5/therix/entities/models.py
--rw-r--r--   0        0        0     2489 2024-05-13 10:00:13.304041 therix-0.1.5/therix/examples/cache_config_example.py
--rw-r--r--   0        0        0     2720 2024-05-13 10:00:13.304169 therix-0.1.5/therix/examples/keyword_search_examples.py
--rw-r--r--   0        0        0     3231 2024-05-13 10:00:13.304273 therix-0.1.5/therix/examples/main.py
--rw-r--r--   0        0        0     1839 2024-05-13 10:00:13.304440 therix-0.1.5/therix/examples/pii_filter_example.py
--rw-r--r--   0        0        0     6424 2024-05-13 10:00:13.304598 therix-0.1.5/therix/examples/summarizer_example.py
--rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.5/therix/pylintrc
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.5/therix/services/__init__.py
--rw-r--r--   0        0        0     7209 2024-05-13 10:00:13.304760 therix-0.1.5/therix/services/pipeline_service.py
--rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.5/therix/services/web_crawling.py
--rw-r--r--   0        0        0     2077 2024-05-13 10:00:13.304865 therix-0.1.5/therix/tests/test_cache.py
--rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.5/therix/tests/test_pii_filter.py
--rw-r--r--   0        0        0     8197 2024-05-13 10:00:13.305133 therix-0.1.5/therix/tests/test_summarizer.py
--rw-r--r--   0        0        0     3304 2024-05-13 10:00:13.305224 therix-0.1.5/therix/utils/keyword_search.py
--rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.5/therix/utils/pii_filter.py
--rw-r--r--   0        0        0    10981 2024-05-13 10:00:13.305523 therix-0.1.5/therix/utils/rag.py
--rw-r--r--   0        0        0     4591 2024-05-13 10:00:13.305701 therix-0.1.5/therix/utils/summarizer.py
--rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 therix-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.6/README.md
+-rw-r--r--   0        0        0     1048 2024-05-14 09:29:48.115395 therix-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.6/therix/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.6/therix/alembic/README
+-rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.6/therix/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.6/therix/alembic/script.py.mako
+-rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.6/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
+-rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.6/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
+-rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.6/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
+-rw-r--r--   0        0        0     2614 2024-05-14 09:23:25.311332 therix-0.1.6/therix/alembic/versions/2024_05_13_1842-f5c4562bcd86_added_config_type_for_system_prompt.py
+-rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.6/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
+-rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.6/therix/alembic.ini
+-rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.6/therix/core/JSONLoader.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.6/therix/core/__init__.py
+-rw-r--r--   0        0        0     2737 2024-05-13 10:00:13.299373 therix-0.1.6/therix/core/cache.py
+-rw-r--r--   0        0        0     1399 2024-05-13 10:00:13.301278 therix-0.1.6/therix/core/chat_history/base_chat_history.py
+-rw-r--r--   0        0        0     1649 2024-05-13 10:00:13.301411 therix-0.1.6/therix/core/constants.py
+-rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.6/therix/core/data_sources.py
+-rw-r--r--   0        0        0     1676 2024-04-16 12:12:31.276049 therix-0.1.6/therix/core/embedding_models.py
+-rw-r--r--   0        0        0     2374 2024-05-13 10:00:13.301910 therix-0.1.6/therix/core/inference_models.py
+-rw-r--r--   0        0        0      317 2024-05-13 10:00:13.302010 therix-0.1.6/therix/core/output_parser.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.6/therix/core/output_source.py
+-rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.6/therix/core/pii_filter_config.py
+-rw-r--r--   0        0        0     6884 2024-05-14 09:23:25.312293 therix-0.1.6/therix/core/pipeline.py
+-rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.6/therix/core/pipeline_component.py
+-rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.6/therix/core/response.py
+-rw-r--r--   0        0        0      594 2024-05-13 10:00:13.302774 therix-0.1.6/therix/core/summarizer_config.py
+-rw-r--r--   0        0        0       98 2024-05-13 10:00:13.302847 therix-0.1.6/therix/core/summarizer_output_model.py
+-rw-r--r--   0        0        0      328 2024-05-14 09:23:25.312543 therix-0.1.6/therix/core/system_prompt_config.py
+-rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.6/therix/core/trace.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.6/therix/db/__init__.py
+-rw-r--r--   0        0        0     3812 2024-05-14 09:23:25.313336 therix-0.1.6/therix/db/db_manager.py
+-rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.6/therix/db/session.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.6/therix/db/tests/__init__.py
+-rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.6/therix/db/tests/test_db_manager.py
+-rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.6/therix/docs/.gitignore
+-rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.6/therix/docs/README.md
+-rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.6/therix/docs/babel.config.js
+-rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.6/therix/docs/blog/2019-05-28-first-blog-post.md
+-rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.6/therix/docs/blog/2019-05-29-long-blog-post.md
+-rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.6/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
+-rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.6/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.6/therix/docs/blog/2021-08-26-welcome/index.md
+-rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.6/therix/docs/blog/authors.yml
+-rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.6/therix/docs/docs/LLM-Proxy/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.6/therix/docs/docs/LLM-Proxy/index.md
+-rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.6/therix/docs/docs/core-components/_category_.json
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/_category_.json
+-rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/caching.md
+-rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
+-rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
+-rw-r--r--   0        0        0     5428 2024-05-13 10:00:13.303279 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
+-rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
+-rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
+-rw-r--r--   0        0        0     1409 2024-05-14 09:23:25.313707 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/system-prompt.md
+-rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/trace.md
+-rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations.md
+-rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.6/therix/docs/docs/core-components/pipeline-templates.md
+-rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.6/therix/docs/docs/core-components/pipeline.md
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.6/therix/docs/docs/introduction/_category_.json
+-rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.6/therix/docs/docs/introduction/getting-started.md
+-rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.6/therix/docs/docs/introduction/index.md
+-rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.6/therix/docs/docs/introduction/installation.md
+-rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.6/therix/docs/docs/observability/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.6/therix/docs/docs/observability/index.md
+-rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.6/therix/docs/docs/squad/_category_.json
+-rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.6/therix/docs/docs/squad/index.md
+-rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.6/therix/docs/docs/usage/_category_.json
+-rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.6/therix/docs/docs/usage/index.md
+-rw-r--r--   0        0        0     3717 2024-05-13 10:00:13.303378 therix-0.1.6/therix/docs/docs/use-cases/Keyword Search.md
+-rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.6/therix/docs/docs/use-cases/_category_.json
+-rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.6/therix/docs/docs/use-cases/faq.md
+-rw-r--r--   0        0        0     3579 2024-05-13 10:00:13.303497 therix-0.1.6/therix/docs/docs/use-cases/pii_filer.md
+-rw-r--r--   0        0        0     4861 2024-05-14 09:23:25.314499 therix-0.1.6/therix/docs/docs/use-cases/summarizer.md
+-rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.6/therix/docs/docusaurus.config.js
+-rw-r--r--   0        0        0      133 2024-05-13 10:00:13.303753 therix-0.1.6/therix/docs/firebase.json
+-rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.6/therix/docs/package-lock.json
+-rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.6/therix/docs/package.json
+-rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.6/therix/docs/sidebars.js
+-rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.6/therix/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.6/therix/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.6/therix/docs/src/css/custom.css
+-rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.6/therix/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.6/therix/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.6/therix/docs/static/.nojekyll
+-rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.6/therix/docs/static/img/coditas.png
+-rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.6/therix/docs/static/img/coditasLogo.svg
+-rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.6/therix/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.6/therix/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.6/therix/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.6/therix/docs/static/img/icon.svg
+-rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.6/therix/docs/static/img/logo.png
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.6/therix/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.6/therix/docs/static/img/therix-logo.png
+-rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.6/therix/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.6/therix/docs/static/img/undraw_docusaurus_react.svg
+-rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.6/therix/docs/static/img/undraw_docusaurus_tree.svg
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.6/therix/entities/__init__.py
+-rw-r--r--   0        0        0     2572 2024-05-14 09:23:25.315163 therix-0.1.6/therix/entities/models.py
+-rw-r--r--   0        0        0     2489 2024-05-13 10:00:13.304041 therix-0.1.6/therix/examples/cache_config_example.py
+-rw-r--r--   0        0        0     2720 2024-05-13 10:00:13.304169 therix-0.1.6/therix/examples/keyword_search_examples.py
+-rw-r--r--   0        0        0     2549 2024-05-14 09:23:25.315461 therix-0.1.6/therix/examples/main.py
+-rw-r--r--   0        0        0     1839 2024-05-13 10:00:13.304440 therix-0.1.6/therix/examples/pii_filter_example.py
+-rw-r--r--   0        0        0     6380 2024-05-14 09:23:25.315855 therix-0.1.6/therix/examples/summarizer_example.py
+-rw-r--r--   0        0        0     6978 2024-05-14 09:23:25.316196 therix-0.1.6/therix/examples/system_prompt_example.py
+-rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.6/therix/pylintrc
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.6/therix/services/__init__.py
+-rw-r--r--   0        0        0     7305 2024-05-14 09:23:25.316581 therix-0.1.6/therix/services/pipeline_service.py
+-rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.6/therix/services/web_crawling.py
+-rw-r--r--   0        0        0     2077 2024-05-13 10:00:13.304865 therix-0.1.6/therix/tests/test_cache.py
+-rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.6/therix/tests/test_pii_filter.py
+-rw-r--r--   0        0        0     8197 2024-05-13 10:00:13.305133 therix-0.1.6/therix/tests/test_summarizer.py
+-rw-r--r--   0        0        0     3304 2024-05-13 10:00:13.305224 therix-0.1.6/therix/utils/keyword_search.py
+-rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.6/therix/utils/pii_filter.py
+-rw-r--r--   0        0        0    11283 2024-05-14 09:23:25.316980 therix-0.1.6/therix/utils/rag.py
+-rw-r--r--   0        0        0     4921 2024-05-14 09:23:25.317276 therix-0.1.6/therix/utils/summarizer.py
+-rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 therix-0.1.6/PKG-INFO
```

### Comparing `therix-0.1.5/LICENSE` & `therix-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/README.md` & `therix-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/pyproject.toml` & `therix-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "therix"
-version = "0.1.5"
+version = "0.1.6"
 description = "Therix is the SDK for langchain based applications."
 authors = ["Ajinath"]
 license = "MIT"
 readme = "README.md"
 include = ["alembic/**/*", "alembic.ini"]
 
 [tool.poetry.dependencies]
```

### Comparing `therix-0.1.5/therix/alembic/env.py` & `therix-0.1.6/therix/alembic/env.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/alembic/script.py.mako` & `therix-0.1.6/therix/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py` & `therix-0.1.6/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py` & `therix-0.1.6/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py` & `therix-0.1.6/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py` & `therix-0.1.6/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/alembic.ini` & `therix-0.1.6/therix/alembic.ini`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/JSONLoader.py` & `therix-0.1.6/therix/core/JSONLoader.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/cache.py` & `therix-0.1.6/therix/core/cache.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/chat_history/base_chat_history.py` & `therix-0.1.6/therix/core/chat_history/base_chat_history.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/constants.py` & `therix-0.1.6/therix/core/constants.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/data_sources.py` & `therix-0.1.6/therix/core/data_sources.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/embedding_models.py` & `therix-0.1.6/therix/core/embedding_models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/inference_models.py` & `therix-0.1.6/therix/core/inference_models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/pipeline.py` & `therix-0.1.6/therix/core/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,31 +104,40 @@
             
             if(question == None and keyword_search_params == None):
                 return "Please provide the required Parameters to invoke the pipeline"
 
             pipeline_trace_config = self.pipeline_service.get_pipeline_configuraitons_by_type(
                 self.pipeline_data.id, ConfigType.TRACE_DETAILS
             )
+            pipeline_system_prompt = self.pipeline_service.get_pipeline_configuraitons_by_type(self.pipeline_data.id, ConfigType.SYSTEM_PROMPT)
             trace_details = pipeline_trace_config[0].config if pipeline_trace_config else None
 
             pipeline_type = self.pipeline_service.get_pipeline(self.pipeline_data.id).type.value
 
             if pipeline_type == PipelineTypeMaster.RAG.value:
                 if add_cache:
                     cached_response = therix_cache.lookup(question, inference_model[0].name, self.pipeline_data.id)
                 if cached_response:
                     return ModelResponse(cached_response, session_id).create_response()
                 if (keyword_search_params and question == None):
                     keyword_search_params['pipeline_id'] = self.pipeline_data.id
                     keyword_search_params['trace_details'] = trace_details
                     answer = self.pipeline_service.search_keywords(keyword_search_params)
                 else:
-                    answer = self.pipeline_service.invoke_pipeline(
-                        self.pipeline_data.id, question, session_id, trace_details
-                    )
+                    if(pipeline_system_prompt):
+                        answer = self.pipeline_service.invoke_pipeline(
+                            self.pipeline_data.id, question, session_id, trace_details, pipeline_system_prompt[0]
+                        )
+                    else:
+                        answer = self.pipeline_service.invoke_pipeline(
+                            self.pipeline_data.id, question, session_id, trace_details
+                        )                        
                 if add_cache:
                     therix_cache.update(question, inference_model[0].name, answer, self.pipeline_data.id)
             elif pipeline_type == PipelineTypeMaster.SUMMARIZER.value:
-                answer = self.pipeline_service.invoke_summarizer_pipeline(self.pipeline_data.id, text=question, trace_details=trace_details)
-            
+                if(pipeline_system_prompt):
+                    answer = self.pipeline_service.invoke_summarizer_pipeline(self.pipeline_data.id, text=question, trace_details=trace_details, system_prompt = pipeline_system_prompt[0])
+                else: 
+                    answer = self.pipeline_service.invoke_summarizer_pipeline(self.pipeline_data.id, text=question, trace_details=trace_details)
+
             return ModelResponse(answer, session_id).create_response()
```

### Comparing `therix-0.1.5/therix/core/pipeline_component.py` & `therix-0.1.6/therix/core/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/core/summarizer_config.py` & `therix-0.1.6/therix/core/summarizer_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/db/db_manager.py` & `therix-0.1.6/therix/db/db_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,19 @@
     def _create_engine(cls):
         db_url = cls._construct_db_url()
         return create_engine(db_url)
 
     @classmethod
     def _construct_db_url(cls):
         drivername = os.getenv("THERIX_DB_TYPE", "postgresql")
-        username = os.getenv("THERIX_DB_USERNAME")
-        password = os.getenv("THERIX_DB_PASSWORD")
-        host = os.getenv("THERIX_DB_HOST")
-        port = os.getenv("THERIX_DB_PORT")
-        db_name = os.getenv("THERIX_DB_NAME")
+        username = os.getenv("THERIX_DB_USERNAME","postgres")
+        password = os.getenv("THERIX_DB_PASSWORD","Piyush1234")
+        host = os.getenv("THERIX_DB_HOST","localhost")
+        port = os.getenv("THERIX_DB_PORT","5432")
+        db_name = os.getenv("THERIX_DB_NAME","coditasAi")
         return URL.create(
             drivername=drivername,
             username=username,
             password=password,
             host=host,
             port=port,
             database=db_name,
```

### Comparing `therix-0.1.5/therix/db/tests/test_db_manager.py` & `therix-0.1.6/therix/db/tests/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/README.md` & `therix-0.1.6/therix/docs/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/blog/2019-05-29-long-blog-post.md` & `therix-0.1.6/therix/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `therix-0.1.6/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/blog/2021-08-26-welcome/index.md` & `therix-0.1.6/therix/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/caching.md` & `therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/caching.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/data-sources.md` & `therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/data-sources.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md` & `therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/inference-model.md` & `therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/inference-model.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG` & `therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG` & `therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations/trace.md` & `therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations/trace.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline-configurations.md` & `therix-0.1.6/therix/docs/docs/core-components/pipeline-configurations.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/core-components/pipeline.md` & `therix-0.1.6/therix/docs/docs/core-components/pipeline.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/introduction/getting-started.md` & `therix-0.1.6/therix/docs/docs/introduction/getting-started.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/introduction/index.md` & `therix-0.1.6/therix/docs/docs/introduction/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/introduction/installation.md` & `therix-0.1.6/therix/docs/docs/introduction/installation.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/use-cases/Keyword Search.md` & `therix-0.1.6/therix/docs/docs/use-cases/Keyword Search.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/use-cases/pii_filer.md` & `therix-0.1.6/therix/docs/docs/use-cases/pii_filer.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/docs/use-cases/summarizer.md` & `therix-0.1.6/therix/docs/docs/use-cases/summarizer.md`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 ```
 
 **Sample Output:**
 ```python
 {'answer': {"mainTopic": "Superfoods", "subTopic1": "Health Benefits", "subTopic2": "10 Superfoods"} , 'session_id': UUID('3f2d3cef-8091-4e0d-accd-71b6387938c7')}
 ```
 
+
+
 ## How you can integrate summarizer in your code:
 
 - Import Necessary Modules: Begin by importing the required modules for configuring the Summarizer.
 
 ```python
 from therix.summarizer import SummarizerConfig, SummarizerTypeMaster
 from therix.core.summarizer_output_model import SummarizerOutputModel  # Import SummarizerOutputModel if needed
@@ -58,14 +60,37 @@
 Create an instance of the SummarizerConfig class by specifying the type of summarizer and, optionally, the Pydantic model for structuring the JSON output.
 
 - **For Extractive Summarizer with custom Pydantic model**
 ```python
 summarizer_config = SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE, TopicModel)
 ```
 
+- **For Extractive Summarizer with custom system prompt**
+
+Use the same placeholders for `{context}` and `{response_schema_json}`
+
+```python
+#For example:
+sys_prompt = 
+        """
+        You are a doctor chatbot
+        Summarize the provided context below as a doctor:
+        {context}
+
+        ---
+
+        Craft your response with conciseness and accuracy, including only the information provided in the context. 
+        Use null values for any missing information.
+
+        Please structure your response in the following JSON format:
+        {response_schema_json}
+        """
+    ```
+
+
 - **For Abstractive Summarizer**
 ```python
 summarizer_config = SummarizerConfig(SummarizerTypeMaster.ABSTRACTIVE)
 ```
 
 - Add Summarizer Configuration to Pipeline: Use the .add() method to add the SummarizerConfig to your Therix pipeline.
 
@@ -75,15 +100,17 @@
 
 ## Example
 
 ```python
 pipeline = Pipeline(name="Summarizer Pipeline")
     (pipeline
     .add(SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE,TopicModel))
+    #custom-prompt
+    .add(SystemPromptConfig(config={"system_prompt" : sys_prompt}))
     .add(// Any other configuration you want to add)
     .save())
 
     pipeline.publish()
     answer = pipeline.invoke(text)
 ```
 
-By following these steps and adjusting the parameters as needed, you can seamlessly integrate the Summarizer into your Therix pipeline. Whether you require Extractive or Abstractive summarization, with or without a custom model, Therix provides the flexibility and functionality to meet your summarization needs effectively.
+By following these steps and adjusting the parameters as needed, you can seamlessly integrate the Summarizer into your Therix pipeline. Whether you require Extractive or Abstractive summarization, with or without a custom model, Therix provides the flexibility and functionality to meet your summarization needs effectively.
```

### Comparing `therix-0.1.5/therix/docs/docusaurus.config.js` & `therix-0.1.6/therix/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/package-lock.json` & `therix-0.1.6/therix/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/package.json` & `therix-0.1.6/therix/docs/package.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/sidebars.js` & `therix-0.1.6/therix/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/src/components/HomepageFeatures/index.js` & `therix-0.1.6/therix/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/src/css/custom.css` & `therix-0.1.6/therix/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/coditas.png` & `therix-0.1.6/therix/docs/static/img/coditas.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/coditasLogo.svg` & `therix-0.1.6/therix/docs/static/img/coditasLogo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/docusaurus-social-card.jpg` & `therix-0.1.6/therix/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/docusaurus.png` & `therix-0.1.6/therix/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/favicon.ico` & `therix-0.1.6/therix/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/icon.svg` & `therix-0.1.6/therix/docs/static/img/icon.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/logo.png` & `therix-0.1.6/therix/docs/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/logo.svg` & `therix-0.1.6/therix/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/therix-logo.png` & `therix-0.1.6/therix/docs/static/img/therix-logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/undraw_docusaurus_mountain.svg` & `therix-0.1.6/therix/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/undraw_docusaurus_react.svg` & `therix-0.1.6/therix/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/docs/static/img/undraw_docusaurus_tree.svg` & `therix-0.1.6/therix/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/entities/models.py` & `therix-0.1.6/therix/entities/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     INPUT_SOURCE = "INPUT_SOURCE"
     EMBEDDING_MODEL = "EMBEDDING_MODEL"
     INFERENCE_MODEL = "INFERENCE_MODEL"
     OUTPUT_SOURCE = "OUTPUT_SOURCE"
     TRACE_DETAILS = "TRACE_DETAILS"
     PII_FILTER = "PII_FILTER"
     SUMMARIZER = "SUMMARIZER"
-    CACHE_CONFIG = "CACHE_CONFIG"
+    CACHE_CONFIG = "CACHE_CONFIG",
+    SYSTEM_PROMPT = 'SYSTEM_PROMPT'
 
 
 class Pipeline(Base):
     __tablename__ = "pipelines"
 
     id = Column(
         UUID(as_uuid=True),
```

### Comparing `therix-0.1.5/therix/examples/cache_config_example.py` & `therix-0.1.6/therix/examples/cache_config_example.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/examples/keyword_search_examples.py` & `therix-0.1.6/therix/examples/keyword_search_examples.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/examples/pii_filter_example.py` & `therix-0.1.6/therix/examples/pii_filter_example.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/examples/summarizer_example.py` & `therix-0.1.6/therix/examples/summarizer_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     question = sys.argv[2]
     ans = pipeline.invoke(question)
     print(ans)
 else:
     pipeline = Pipeline(name="Summarizer Pipeline")
 
     (pipeline
-    .add(GroqMixtral87bInferenceModel(config={"groq_api_key": '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'}))
+    .add(GroqMixtral87bInferenceModel(config={"groq_api_key": "GROQ_API_KEY"}))
     .add(SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE,TopicModel))
     .add(Trace(config={
         'secret_key': 'sk-lf-e62aa7ce-c4c8-4c77-ad7d-9d76dfd96db1',
         'public_key': 'pk-lf-282ad728-c1d6-4247-b6cd-8022198591a9',
         'identifier': 'my own pipeline'
     }))
     .save())
```

### Comparing `therix-0.1.5/therix/pylintrc` & `therix-0.1.6/therix/pylintrc`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/services/pipeline_service.py` & `therix-0.1.6/therix/services/pipeline_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         if "website" in data_sources[0].config:
             os.remove(output_file)
         embedding_model = self.get_pipeline_configuraitons_by_type(
             pipeline_id, "EMBEDDING_MODEL"
         )
         return create_embeddings(data_sources, embedding_model[0], str(pipeline_id))
 
-    def invoke_pipeline(self, pipeline_id, question, session_id, trace_details=None):
+    def invoke_pipeline(self, pipeline_id, question, session_id, trace_details=None, system_prompt=None):
         embedding_model = self.get_pipeline_configuraitons_by_type(
             pipeline_id, "EMBEDDING_MODEL"
         )
         store = get_vectorstore(embedding_model[0], str(pipeline_id))
         retreiver = store.as_retriever()
 
         inference_model = self.get_pipeline_configuraitons_by_type(
@@ -89,27 +89,28 @@
             question,
             retreiver,
             inference_model[0],
             embedding_model,
             session_id,
             pipeline_id,
             trace_details,
+            system_prompt
         )
         pii_filter_config = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.PII_FILTER)
         if pii_filter_config:
             pii_filter_config = pii_filter_config[0].config
             entities = pii_filter_config['entities']
             return pii_filter(result,entities)
         else:
             return result
 
-    def invoke_summarizer_pipeline(self, pipeline_id, text, trace_details = None):
+    def invoke_summarizer_pipeline(self, pipeline_id, text, trace_details = None, system_prompt=None):
         inference_model = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.INFERENCE_MODEL)
         summarizer_config = self.get_pipeline_configuraitons_by_type(pipeline_id, ConfigType.SUMMARIZER)[0].config
-        return summarizer(summarizer_config,inference_model[0],text)
+        return summarizer(summarizer_config,inference_model[0],text, trace_details, system_prompt)
 
     def search_keywords(self, keyword_search_params):
         if(not keyword_search_params.get("pipeline_id") or not keyword_search_params.get("config_id") or not keyword_search_params.get("prompt") or not keyword_search_params.get("keywords") or not keyword_search_params.get("output_parser")):
             return "Request is missing required parameters, please provide all the parameters, i.e. pipeline_id, config_id, prompt, keywords, output_parser"
         inference_model = self.get_pipeline_configuraitons_by_type(keyword_search_params.get("pipeline_id"), ConfigType.INFERENCE_MODEL)[0]
         inference_model_name = inference_model.name
         infer_config = inference_model.config
```

### Comparing `therix-0.1.5/therix/services/web_crawling.py` & `therix-0.1.6/therix/services/web_crawling.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/tests/test_cache.py` & `therix-0.1.6/therix/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/tests/test_pii_filter.py` & `therix-0.1.6/therix/tests/test_pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/tests/test_summarizer.py` & `therix-0.1.6/therix/tests/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/utils/keyword_search.py` & `therix-0.1.6/therix/utils/keyword_search.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/utils/pii_filter.py` & `therix-0.1.6/therix/utils/pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.5/therix/utils/rag.py` & `therix-0.1.6/therix/utils/rag.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 from langchain.prompts import PromptTemplate
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.runnables import RunnablePassthrough
 from langchain_core.output_parsers import StrOutputParser
 from langchain_core.messages import get_buffer_string
 from langchain_core.prompts import format_document
 from langchain_core.runnables import RunnableParallel
+from langchain_text_splitters import  RecursiveCharacterTextSplitter
 from operator import itemgetter
 
-
 def sanitize_text(text):
     # Remove null characters (0x00) from the text
     sanitized_text = text.replace("\x00", "")
     return sanitized_text
 
 
 def get_loader(file_type, file_path, config):
@@ -155,30 +155,35 @@
     else:
         raise ValueError(f"Unknown inference model: {inference_model_name}")
 
 
 def create_embeddings(data_sources, embedding_model, collection_name):
 
     store = get_vectorstore(embedding_model, collection_name)
+    
     config_id = []
     for data_source in data_sources:
         config_id.append(uuid.uuid4())
         # data_source = {'name': 'PDF', 'config': {'files': ['path/to/file', 'path/to/file']}}
         for file_path in data_source.config["files"]:
             loader = get_loader(data_source.name, file_path, data_source.config)
             extra_metadata = [
                 ("configId", str(config_id)),
             ]
             pages = loader.load_and_split()
             for page_content in pages:
                 for key, value in extra_metadata:
                     page_content.metadata[key] = value
+            
             # document.text = mask_data(document.text)
-            # text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
-            store.add_documents(pages)
+            result=RecursiveCharacterTextSplitter(
+                 chunk_size=1000,
+                 chunk_overlap=200,
+                ).split_documents(pages)
+            store.add_documents(result)
     # config_id is a list, due to possibility of multiple data_source.
     return {"message" : "embedding created" , "config_id" : config_id}
 
 
 def get_vectorstore(embedding_model, collection_name):
     embeddings = get_embedding_model(embedding_model.name, embedding_model.config)
     store = PGVector(
@@ -193,14 +198,15 @@
     question,
     retriever,
     inference_model,
     embed_model,
     session_id,
     pipeline_id,
     trace_details=None,
+    system_prompt=None
 ):
 
     # print(trace_details)
     chain_callbacks = []
     if trace_details is not None:
         langfuse_handler = CallbackHandler(
             secret_key=trace_details["secret_key"],
@@ -214,20 +220,23 @@
         str(session_id),
         str(pipeline_id),
         SQLALCHEMY_DATABASE_URL,
         table_name="chat_history",
     )
     chat_history = history.messages
 
-    template = """Answer the question based only on the following context and do not reply anything that is out of context, reply with "I am sorry, I cannot help you with that" and do not add any more message to it.
-    Context: 
-    {context}
+    if(system_prompt):
+        template = system_prompt.config.get("system_prompt")
+    else : 
+        template = """Answer the question based only on the following context and do not reply anything that is out of context, reply with "I am sorry, I cannot help you with that" and do not add any more message to it.
+        Context: 
+        {context}
 
-    Question: {question}
-    """
+        Question: {question}
+        """
     ANSWER_PROMPT = ChatPromptTemplate.from_template(template)
     _template = """Given the following conversation and a follow up question, rephrase the follow up question to be a standalone question, in its original language.
                     Chat History:
                     {chat_history}
                     Follow Up Input: {question}
                     Standalone question:"""
```

### Comparing `therix-0.1.5/therix/utils/summarizer.py` & `therix-0.1.6/therix/utils/summarizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
         Please structure your response in the following JSON format:
         {response_schema_json}
         """,
     "ABSTRACTIVE": "Provide a concise summary for the following text using abstractive summarization:\n\n{context}."
 }
         
-def summarizer(summarizer_config,inference_model_details,text, trace_details):
+def summarizer(summarizer_config,inference_model_details,text, trace_details, system_prompt=None):
     
     chain_callbacks = []
     if trace_details is not None:
         langfuse_handler = CallbackHandler(
             secret_key=trace_details["secret_key"],
             public_key=trace_details["public_key"],
             host=trace_details["host"],
@@ -105,19 +105,28 @@
     split_docs = text_splitter.split_documents([docs])
 
     # Run the chain
     summary = map_reduce_chain.run(split_docs)
     
     parser = JsonOutputParser()
 
-    prompt = PromptTemplate(
-        template=PROMPT_TEMPLATE[summarization_type],
-        input_variables=["context"],
-        partial_variables={"response_schema_json": pydantic_prompt},
-    )
+    if(system_prompt and summarization_type=="EXTRACTIVE"):
+        prompt = PromptTemplate(
+            template=system_prompt.config.get("system_prompt"),
+            input_variables=["context"],
+            partial_variables={"response_schema_json": pydantic_prompt},
+    )
+    else: 
+        prompt = PromptTemplate(
+            template=PROMPT_TEMPLATE[summarization_type],
+            input_variables=["context"],
+            partial_variables={"response_schema_json": pydantic_prompt},
+        )
+
+
     
     if summarization_type == SummarizerTypeMaster.EXTRACTIVE.value:
         chain = prompt | llm | parser
         return json.dumps(chain.invoke({"context": summary},config={"callbacks": [langfuse_handler]}))
     else:
         chain = prompt | llm
         return  chain.invoke({"context": summary}, config={"callbacks": [langfuse_handler]}).content
```

### Comparing `therix-0.1.5/PKG-INFO` & `therix-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: therix
-Version: 0.1.5
+Version: 0.1.6
 Summary: Therix is the SDK for langchain based applications.
 License: MIT
 Author: Ajinath
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

