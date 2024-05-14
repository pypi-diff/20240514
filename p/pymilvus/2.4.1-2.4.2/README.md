# Comparing `tmp/pymilvus-2.4.1.tar.gz` & `tmp/pymilvus-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilvus-2.4.1.tar", last modified: Mon Apr 29 11:33:42 2024, max compression
+gzip compressed data, was "pymilvus-2.4.2.tar", last modified: Tue May 14 12:59:56 2024, max compression
```

## Comparing `pymilvus-2.4.1.tar` & `pymilvus-2.4.2.tar`

### file list

```diff
@@ -1,224 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.742213 pymilvus-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.706213 pymilvus-2.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/enhancement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/ISSUE_TEMPLATE/general-question.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/mergify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/check_milvus_proto.yml
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/code_checker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/doc_update_event.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/nightly_ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/publish_dev_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/publish_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.github/workflows/release_event.yml
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-29 11:33:31.000000 pymilvus-2.4.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-29 11:33:31.000000 pymilvus-2.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-29 11:33:31.000000 pymilvus-2.4.1/CONTRIBUTING_CN.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 11:33:31.000000 pymilvus-2.4.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-29 11:33:31.000000 pymilvus-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-29 11:33:31.000000 pymilvus-2.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-29 11:33:31.000000 pymilvus-2.4.1/OWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-29 11:33:42.742213 pymilvus-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-29 11:33:31.000000 pymilvus-2.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-29 11:33:31.000000 pymilvus-2.4.1/_version_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-04-29 11:33:31.000000 pymilvus-2.4.1/check_proto_product.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.702213 pymilvus-2.4.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.702213 pymilvus-2.4.1/ci/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/ci/docker/milvus/
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-29 11:33:31.000000 pymilvus-2.4.1/ci/docker/milvus/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/ci/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7597 2024-04-29 11:33:31.000000 pymilvus-2.4.1/ci/scripts/docker_image_find_tag.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.710213 pymilvus-2.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.714213 pymilvus-2.4.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.714213 pymilvus-2.4.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/_templates/autosummaryclass.rst
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/about.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.714213 pymilvus-2.4.1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/collection.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/connections.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/future.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/milvus_index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/partition.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/search.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/api/utility.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/param.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.714213 pymilvus-2.4.1/docs/source/res/
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/res/Intro_to_Indexes.md
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/res/about_documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/results.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-29 11:33:31.000000 pymilvus-2.4.1/docs/source/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.722213 pymilvus-2.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/bfloat16_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/binary_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.722213 pymilvus-2.4.1/examples/cert/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/cert/ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/cert/client.key
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/cert/client.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/cert/server.pem
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.722213 pymilvus-2.4.1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1139866 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/data/train_embeddings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/dynamic_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_bulkinsert_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_bulkinsert_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_bulkwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_gpu_brute_force.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_gpu_cagra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_group_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_tls1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/example_tls2.py
--rw-r--r--   0 runner    (1001) docker     (127)  1070736 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/films.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/float16_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/fuzzy_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_hybrid_sparse_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_milvus.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_milvus_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_milvus_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hello_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/hybrid_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/inverted_index_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.726213 pymilvus-2.4.1/examples/milvus_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/customize_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/customize_schema_auto_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/index.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/index_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/non_ascii_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/rbac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/simple_auto_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/milvus_client/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/multithreading_hello_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/old_style_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/old_style_example_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/old_style_example_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/old_style_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/resource_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/resource_group_declarative_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/role_and_privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-29 11:33:31.000000 pymilvus-2.4.1/examples/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.726213 pymilvus-2.4.1/pymilvus/
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.730213 pymilvus-2.4.1/pymilvus/bulk_writer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/bulk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/local_bulk_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/bulk_writer/remote_bulk_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.734213 pymilvus-2.4.1/pymilvus/client/
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20301 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/asynch.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    22569 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/entity_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    72352 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/grpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    46903 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/singleton_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59505 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/ts_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23514 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.734213 pymilvus-2.4.1/pymilvus/grpc_gen/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    28792 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/feder_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/feder_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    89972 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   102932 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   136781 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/msg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/msg_pb2.pyi
--rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/python_gen.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/rg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/rg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/schema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/grpc_gen/schema_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.738213 pymilvus-2.4.1/pymilvus/milvus_client/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/milvus_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/milvus_client/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/milvus_client/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    35578 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/milvus_client/milvus_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.738213 pymilvus-2.4.1/pymilvus/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.738213 pymilvus-2.4.1/pymilvus/orm/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66166 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20047 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/future.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    23292 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23015 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    50438 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/orm/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pymilvus/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.742213 pymilvus-2.4.1/pymilvus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 11:33:42.000000 pymilvus-2.4.1/pymilvus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-04-29 11:33:31.000000 pymilvus-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-29 11:33:31.000000 pymilvus-2.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:33:42.742213 pymilvus-2.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:33:42.742213 pymilvus-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/mock_milvus.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/mock_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_create_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_grpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_ts_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-29 11:33:31.000000 pymilvus-2.4.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.998082 pymilvus-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.962081 pymilvus-2.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.962081 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/enhancement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/ISSUE_TEMPLATE/general-question.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/mergify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.962081 pymilvus-2.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/check_milvus_proto.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/code_checker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/doc_update_event.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/nightly_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/publish_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/publish_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.github/workflows/release_event.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 12:59:47.000000 pymilvus-2.4.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-14 12:59:47.000000 pymilvus-2.4.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-14 12:59:47.000000 pymilvus-2.4.2/CONTRIBUTING_CN.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-14 12:59:47.000000 pymilvus-2.4.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-14 12:59:47.000000 pymilvus-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-14 12:59:47.000000 pymilvus-2.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-14 12:59:47.000000 pymilvus-2.4.2/OWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-14 12:59:55.998082 pymilvus-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-14 12:59:47.000000 pymilvus-2.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-14 12:59:47.000000 pymilvus-2.4.2/_version_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-05-14 12:59:47.000000 pymilvus-2.4.2/check_proto_product.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.958081 pymilvus-2.4.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.958081 pymilvus-2.4.2/ci/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.962081 pymilvus-2.4.2/ci/docker/milvus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-14 12:59:47.000000 pymilvus-2.4.2/ci/docker/milvus/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.966081 pymilvus-2.4.2/ci/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7597 2024-05-14 12:59:47.000000 pymilvus-2.4.2/ci/scripts/docker_image_find_tag.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.966081 pymilvus-2.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.966081 pymilvus-2.4.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.966081 pymilvus-2.4.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/_templates/autosummaryclass.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/about.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.970081 pymilvus-2.4.2/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/collection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/future.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/milvus_index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/partition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/search.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/api/utility.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/param.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.970081 pymilvus-2.4.2/docs/source/res/
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/res/Intro_to_Indexes.md
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/res/about_documentation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-14 12:59:47.000000 pymilvus-2.4.2/docs/source/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.978081 pymilvus-2.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/bfloat16_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/binary_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.978081 pymilvus-2.4.2/examples/cert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/cert/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/cert/client.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/cert/client.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/cert/server.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.978081 pymilvus-2.4.2/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1139866 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/data/train_embeddings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/dynamic_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_bulkinsert_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_bulkinsert_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_bulkwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_gpu_brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_gpu_cagra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_tls1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/example_tls2.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1070736 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/films.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/float16_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/fuzzy_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_hybrid_sparse_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_milvus.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_milvus_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_milvus_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hello_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/hybrid_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/inverted_index_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.982082 pymilvus-2.4.2/examples/milvus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/customize_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/customize_schema_auto_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/index_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/non_ascii_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/simple_auto_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/milvus_client/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/multithreading_hello_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/old_style_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/old_style_example_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/old_style_example_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/old_style_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/resource_group_declarative_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/role_and_privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-14 12:59:47.000000 pymilvus-2.4.2/examples/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.982082 pymilvus-2.4.2/pymilvus/
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.982082 pymilvus-2.4.2/pymilvus/bulk_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/bulk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/local_bulk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/bulk_writer/remote_bulk_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.986081 pymilvus-2.4.2/pymilvus/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/asynch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20429 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/entity_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72991 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/grpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47348 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/singleton_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59505 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/ts_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24250 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8024 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.990082 pymilvus-2.4.2/pymilvus/grpc_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19238 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/feder_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/feder_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    91367 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104621 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   138400 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/msg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/msg_pb2.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2208 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/python_gen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/rg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/rg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/schema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/grpc_gen/schema_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.990082 pymilvus-2.4.2/pymilvus/milvus_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/milvus_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/milvus_client/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/milvus_client/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35578 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/milvus_client/milvus_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.990082 pymilvus-2.4.2/pymilvus/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.994082 pymilvus-2.4.2/pymilvus/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66019 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21066 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23291 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31276 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23015 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50438 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/orm/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pymilvus/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.998082 pymilvus-2.4.2/pymilvus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 12:59:55.000000 pymilvus-2.4.2/pymilvus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-05-14 12:59:47.000000 pymilvus-2.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 12:59:47.000000 pymilvus-2.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:59:55.998082 pymilvus-2.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:59:55.998082 pymilvus-2.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/mock_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/mock_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14886 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_create_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_grpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_milvus_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_ts_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-14 12:59:47.000000 pymilvus-2.4.2/tests/utils.py
```

### Comparing `pymilvus-2.4.1/.github/ISSUE_TEMPLATE/bug_report.yaml` & `pymilvus-2.4.2/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/ISSUE_TEMPLATE/enhancement.yaml` & `pymilvus-2.4.2/.github/ISSUE_TEMPLATE/enhancement.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/ISSUE_TEMPLATE/feature_request.yaml` & `pymilvus-2.4.2/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/ISSUE_TEMPLATE/general-question.yaml` & `pymilvus-2.4.2/.github/ISSUE_TEMPLATE/general-question.yaml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/mergify.yml` & `pymilvus-2.4.2/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/workflows/check_milvus_proto.yml` & `pymilvus-2.4.2/.github/workflows/check_milvus_proto.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/workflows/code_checker.yml` & `pymilvus-2.4.2/.github/workflows/code_checker.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/workflows/doc_update_event.yml` & `pymilvus-2.4.2/.github/workflows/doc_update_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/workflows/nightly_ci.yml` & `pymilvus-2.4.2/.github/workflows/nightly_ci.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/workflows/publish_dev_package.yml` & `pymilvus-2.4.2/.github/workflows/publish_dev_package.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/workflows/publish_on_release.yml` & `pymilvus-2.4.2/.github/workflows/publish_on_release.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/workflows/pull_request.yml` & `pymilvus-2.4.2/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/.github/workflows/release_event.yml` & `pymilvus-2.4.2/.github/workflows/release_event.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/CONTRIBUTING.md` & `pymilvus-2.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/CONTRIBUTING_CN.md` & `pymilvus-2.4.2/CONTRIBUTING_CN.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/LICENSE` & `pymilvus-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/Makefile` & `pymilvus-2.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/PKG-INFO` & `pymilvus-2.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.4.1
+Version: 2.4.2
 Summary: Python Sdk for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/pymilvus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,27 +12,28 @@
 Requires-Dist: setuptools>=67
 Requires-Dist: grpcio<=1.60.0,>=1.49.1
 Requires-Dist: protobuf>=3.20.0
 Requires-Dist: environs<=9.5.0
 Requires-Dist: ujson>=2.0.0
 Requires-Dist: pandas>=1.2.4
 Requires-Dist: numpy<1.25.0; python_version <= "3.8"
-Requires-Dist: requests
-Requires-Dist: minio>=7.0.0
-Requires-Dist: pyarrow>=12.0.0
-Requires-Dist: azure-storage-blob
-Requires-Dist: scipy
+Requires-Dist: milvus_lite<2.5.0,>=2.4.0
+Provides-Extra: bulk-writer
+Requires-Dist: requests; extra == "bulk-writer"
+Requires-Dist: minio>=7.0.0; extra == "bulk-writer"
+Requires-Dist: pyarrow>=12.0.0; extra == "bulk-writer"
+Requires-Dist: azure-storage-blob; extra == "bulk-writer"
 Provides-Extra: model
 Requires-Dist: milvus-model>=0.1.0; extra == "model"
 Provides-Extra: test
 Requires-Dist: pytest>=5.3.4; extra == "test"
 Requires-Dist: pytest-cov>=2.8.1; extra == "test"
 Requires-Dist: pytest-timeout>=1.3.4; extra == "test"
 Requires-Dist: grpcio-testing; extra == "test"
-Requires-Dist: ruff>=0.3.3; extra == "test"
+Requires-Dist: ruff>0.4.0; extra == "test"
 Requires-Dist: black; extra == "test"
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
 [![Downloads](https://static.pepy.tech/badge/pymilvus)](https://pepy.tech/project/pymilvus)
```

### Comparing `pymilvus-2.4.1/README.md` & `pymilvus-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/_version_helper.py` & `pymilvus-2.4.2/_version_helper.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/check_proto_product.sh` & `pymilvus-2.4.2/check_proto_product.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/ci/docker/milvus/docker-compose.yml` & `pymilvus-2.4.2/ci/docker/milvus/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/ci/scripts/docker_image_find_tag.sh` & `pymilvus-2.4.2/ci/scripts/docker_image_find_tag.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/Makefile` & `pymilvus-2.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/README.md` & `pymilvus-2.4.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/make.bat` & `pymilvus-2.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/api/collection.rst` & `pymilvus-2.4.2/docs/source/api/collection.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/api/connections.rst` & `pymilvus-2.4.2/docs/source/api/connections.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/api/future.rst` & `pymilvus-2.4.2/docs/source/api/future.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/api/milvus_index.rst` & `pymilvus-2.4.2/docs/source/api/milvus_index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/api/partition.rst` & `pymilvus-2.4.2/docs/source/api/partition.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/api/schema.rst` & `pymilvus-2.4.2/docs/source/api/schema.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/api/search.rst` & `pymilvus-2.4.2/docs/source/api/search.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/api/utility.rst` & `pymilvus-2.4.2/docs/source/api/utility.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/conf.py` & `pymilvus-2.4.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/contribute.rst` & `pymilvus-2.4.2/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/faq.rst` & `pymilvus-2.4.2/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/index.rst` & `pymilvus-2.4.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/install.rst` & `pymilvus-2.4.2/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/res/Intro_to_Indexes.md` & `pymilvus-2.4.2/docs/source/res/Intro_to_Indexes.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/res/about_documentation.md` & `pymilvus-2.4.2/docs/source/res/about_documentation.md`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/results.rst` & `pymilvus-2.4.2/docs/source/results.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/docs/source/tutorial.rst` & `pymilvus-2.4.2/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/bfloat16_example.py` & `pymilvus-2.4.2/examples/bfloat16_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/binary_example.py` & `pymilvus-2.4.2/examples/binary_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/cert/ca.pem` & `pymilvus-2.4.2/examples/cert/ca.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/cert/client.key` & `pymilvus-2.4.2/examples/cert/client.key`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/cert/client.pem` & `pymilvus-2.4.2/examples/cert/client.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/cert/server.pem` & `pymilvus-2.4.2/examples/cert/server.pem`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/collection.py` & `pymilvus-2.4.2/examples/collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/data/train_embeddings.csv` & `pymilvus-2.4.2/examples/data/train_embeddings.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/database.py` & `pymilvus-2.4.2/examples/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -129,14 +129,22 @@
 
     # verify read and write
     collection_read_write(col2_db1, "db1")
 
     # list collections within db1
     print("\nlist collections of database db1:")
     print(utility.list_collections())
+    
+    # set properties of db1
+    print("\nset properties of db1:")
+    db_info = db.describe_database(db_name="db1")
+    print(db_info)
+    db.set_properties(db_name="db1", properties={"key": "value"})
+    db_info = db.describe_database(db_name="db1")
+    print(db_info)
 
     print("\ndrop collection: col1_db2 from db1")
     col2_db1.drop()
     print("\ndrop database: db1")
     db.drop_database(db_name="db1")
 
     # list database
```

### Comparing `pymilvus-2.4.1/examples/dynamic_field.py` & `pymilvus-2.4.2/examples/dynamic_field.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example.py` & `pymilvus-2.4.2/examples/example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example_bulkinsert_json.py` & `pymilvus-2.4.2/examples/example_bulkinsert_json.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example_bulkinsert_numpy.py` & `pymilvus-2.4.2/examples/example_bulkinsert_numpy.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example_bulkwriter.py` & `pymilvus-2.4.2/examples/example_bulkwriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,21 +22,24 @@
 logging.basicConfig(level=logging.INFO)
 
 from pymilvus import (
     connections,
     FieldSchema, CollectionSchema, DataType,
     Collection,
     utility,
+    BulkInsertState,
+)
+
+from pymilvus.bulk_writer import (
     LocalBulkWriter,
     RemoteBulkWriter,
     BulkFileType,
     bulk_import,
     get_import_progress,
     list_import_jobs,
-    BulkInsertState,
 )
 
 # minio
 MINIO_ADDRESS = "0.0.0.0:9000"
 MINIO_SECRET_KEY = "minioadmin"
 MINIO_ACCESS_KEY = "minioadmin"
```

### Comparing `pymilvus-2.4.1/examples/example_gpu_brute_force.py` & `pymilvus-2.4.2/examples/example_gpu_brute_force.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example_gpu_cagra.py` & `pymilvus-2.4.2/examples/example_gpu_cagra.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example_group_by.py` & `pymilvus-2.4.2/examples/example_group_by.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example_index.py` & `pymilvus-2.4.2/examples/example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example_str.py` & `pymilvus-2.4.2/examples/example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/example_tls2.py` & `pymilvus-2.4.2/examples/example_tls2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import random
 
 from pymilvus import (
-    connections,
+    MilvusClient,
     FieldSchema, CollectionSchema, DataType,
-    Collection,
     utility
 )
 
 # This example shows how to:
 #   1. connect to Milvus server
 #   2. create a collection
 #   3. insert entities
 #   4. create index
 #   5. search
 
 
 _HOST = '127.0.0.1'
 _PORT = '19530'
+_URI = f"https://{_HOST}:{_PORT}"
 
 # Const names
 _COLLECTION_NAME = 'demo'
 _ID_FIELD_NAME = 'id_field'
 _VECTOR_FIELD_NAME = 'float_vector_field'
 
 # Vector parameters
@@ -31,136 +31,96 @@
 _METRIC_TYPE = 'L2'
 _INDEX_TYPE = 'IVF_FLAT'
 _NLIST = 1024
 _NPROBE = 16
 _TOPK = 3
 
 
-# Create a Milvus connection
-def create_connection():
+def main():
+    # create a connection
     print(f"\nCreate connection...")
-    connections.connect(host=_HOST, port=_PORT, secure=True, client_pem_path="cert/client.pem",
-                        client_key_path="cert/client.key",
-                        ca_pem_path="cert/ca.pem", server_name="localhost")
-    print(f"\nList connections:")
-    print(connections.list_connections())
+    milvus_client = MilvusClient(uri=_URI,
+                            secure=True,
+                            client_pem_path="cert/client.pem",
+                            client_key_path="cert/client.key",
+                            ca_pem_path="cert/ca.pem",
+                            server_name='localhost')
+    print(f"\nList connection:")
+    print(milvus_client._get_connection())
 
+    # drop collection if the collection exists
+    if milvus_client.has_collection(_COLLECTION_NAME):
+        milvus_client.drop_collection(_COLLECTION_NAME)
 
-# Create a collection named 'demo'
-def create_collection(name, id_field, vector_field):
-    field1 = FieldSchema(name=id_field, dtype=DataType.INT64, description="int64", is_primary=True)
-    field2 = FieldSchema(name=vector_field, dtype=DataType.FLOAT_VECTOR, description="float vector", dim=_DIM,
+    # create collection
+    field1 = FieldSchema(name=_ID_FIELD_NAME, dtype=DataType.INT64, description="int64", is_primary=True)
+    field2 = FieldSchema(name=_VECTOR_FIELD_NAME, dtype=DataType.FLOAT_VECTOR, description="float vector", dim=_DIM,
                          is_primary=False)
     schema = CollectionSchema(fields=[field1, field2], description="collection description")
-    collection = Collection(name=name, data=None, schema=schema)
-    print("\ncollection created:", name)
-    return collection
-
-
-def has_collection(name):
-    return utility.has_collection(name)
+    milvus_client.create_collection(collection_name=_COLLECTION_NAME,schema=schema)
+    milvus_client.describe_collection(collection_name=_COLLECTION_NAME)
 
+    print("\ncollection created:", _COLLECTION_NAME)
 
-# Drop a collection in Milvus
-def drop_collection(name):
-    collection = Collection(name)
-    collection.drop()
-    print("\nDrop collection: {}".format(name))
-
-
-# List all collections in Milvus
-def list_collections():
+    # show collections
     print("\nlist collections:")
-    print(utility.list_collections())
-
-
-def insert(collection, num, dim):
-    data = [
-        [i for i in range(num)],
-        [[random.random() for _ in range(dim)] for _ in range(num)],
-    ]
-    collection.insert(data)
-    return data[1]
-
-
-def get_entity_num(collection):
-    print("\nThe number of entity:")
-    print(collection.num_entities)
-
-
-def create_index(collection, filed_name):
-    index_param = {
-        "index_type": _INDEX_TYPE,
-        "params": {"nlist": _NLIST},
-        "metric_type": _METRIC_TYPE}
-    collection.create_index(filed_name, index_param)
-    print("\nCreated index:\n{}".format(collection.index().params))
-
-
-def drop_index(collection):
-    collection.drop_index()
-    print("\nDrop index sucessfully")
+    print(milvus_client.list_collections())
 
+    # insert 10000 vectors with 128 dimension
+    data_dict = []
+    for i in range(10000):
+        entity = {
+        "id_field": i+1,  # Assuming id_field is the _COLLECTION_NAME of the field corresponding to the ID
+        "float_vector_field": [random.random() for _ in range(_DIM)]
+        }
+        data_dict.append(entity)
+    insert_result = milvus_client.insert(collection_name=_COLLECTION_NAME,data=data_dict)
 
-def load_collection(collection):
-    collection.load()
+    # get the number of entities
+    print(f"\nThe number of entity: {insert_result['insert_count']}")
 
+    # create index
+    index_params = milvus_client.prepare_index_params()
 
-def release_collection(collection):
-    collection.release()
+    index_params.add_index(
+        field_name=_VECTOR_FIELD_NAME, 
+        index_type=_INDEX_TYPE,
+        metric_type=_METRIC_TYPE,
+        params={"nlist": _NLIST}
+    )
+
+    milvus_client.create_index(
+        collection_name=_COLLECTION_NAME,
+        index_params=index_params
+    )
+    print("\nCreated index")
 
+    # load data to memory
+    milvus_client.load_collection(_COLLECTION_NAME)
+    vector = data_dict[1]
+    vectors = [vector["float_vector_field"]]
 
-def search(collection, vector_field, id_field, search_vectors):
+    # search
     search_param = {
-        "data": search_vectors,
-        "anns_field": vector_field,
+        "anns_field": _VECTOR_FIELD_NAME,
         "param": {"metric_type": _METRIC_TYPE, "params": {"nprobe": _NPROBE}},
-        "limit": _TOPK,
-        "expr": "id_field > 0"}
-    results = collection.search(**search_param)
+        "expr": f"{_ID_FIELD_NAME} > 0"}
+    results = milvus_client.search(collection_name=_COLLECTION_NAME,data=vectors,limit= _TOPK,search_params=search_param)
     for i, result in enumerate(results):
         print("\nSearch result for {}th vector: ".format(i))
         for j, res in enumerate(result):
             print("Top {}: {}".format(j, res))
 
-
-def main():
-    # create a connection
-    create_connection()
-
-    # drop collection if the collection exists
-    if has_collection(_COLLECTION_NAME):
-        drop_collection(_COLLECTION_NAME)
-
-    # create collection
-    collection = create_collection(_COLLECTION_NAME, _ID_FIELD_NAME, _VECTOR_FIELD_NAME)
-
-    # show collections
-    list_collections()
-
-    # insert 10000 vectors with 128 dimension
-    vectors = insert(collection, 10000, _DIM)
-
-    # get the number of entities
-    get_entity_num(collection)
-
-    # create index
-    create_index(collection, _VECTOR_FIELD_NAME)
-
-    # load data to memory
-    load_collection(collection)
-
-    # search
-    search(collection, _VECTOR_FIELD_NAME, _ID_FIELD_NAME, vectors[:3])
-
     # release memory
-    release_collection(collection)
+    milvus_client.release_collection(_COLLECTION_NAME)
 
     # drop collection index
-    drop_index(collection)
+    milvus_client.drop_index(_COLLECTION_NAME,index_name=_VECTOR_FIELD_NAME)
+    print("\nDrop index sucessfully")
 
     # drop collection
-    drop_collection(_COLLECTION_NAME)
+    milvus_client.drop_collection(_COLLECTION_NAME)
+    print("\nDrop collection: {}".format(_COLLECTION_NAME))
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `pymilvus-2.4.1/examples/films.csv` & `pymilvus-2.4.2/examples/films.csv`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/float16_example.py` & `pymilvus-2.4.2/examples/float16_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/fuzzy_match.py` & `pymilvus-2.4.2/examples/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/hello_hybrid_sparse_dense.py` & `pymilvus-2.4.2/examples/hello_hybrid_sparse_dense.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/hello_milvus.ipynb` & `pymilvus-2.4.2/examples/hello_milvus.ipynb`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/hello_milvus.py` & `pymilvus-2.4.2/examples/hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/hello_milvus_array.py` & `pymilvus-2.4.2/examples/hello_milvus_array.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/hello_milvus_delete.py` & `pymilvus-2.4.2/examples/hello_milvus_delete.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/hello_model.py` & `pymilvus-2.4.2/examples/hello_model.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/hello_sparse.py` & `pymilvus-2.4.2/examples/hello_sparse.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 # 4. create index
 # 5. search, query, and hybrid search on entities
 # 6. delete entities by PK
 # 7. drop collection
 import time
 
 import numpy as np
-from scipy.sparse import rand
+import random
 from pymilvus import (
     connections,
     utility,
     FieldSchema, CollectionSchema, DataType,
     Collection,
 )
 
 fmt = "=== {:30} ==="
 search_latency_fmt = "search latency = {:.4f}s"
-num_entities, dim, density = 1000, 3000, 0.005
+num_entities, dim = 1000, 3000
+# non zero count of randomly generated sparse vectors
+nnz = 30
 
 def log(msg):
     print(time.strftime("%Y-%m-%d %H:%M:%S", time.localtime()) + " " + msg)
 
 # -----------------------------------------------------------------------------
 # connect to Milvus
 log(fmt.format("start connecting to Milvus"))
@@ -50,19 +52,24 @@
 
 log(f"hello_sparse has {hello_sparse.num_entities} entities({hello_sparse.num_entities/1000000}M), indexed {hello_sparse.has_index()}")
 
 # -----------------------------------------------------------------------------
 # insert
 log(fmt.format("Start creating entities to insert"))
 rng = np.random.default_rng(seed=19530)
-# this step is so damn slow
-matrix_csr = rand(num_entities, dim, density=density, format='csr')
+
+def generate_sparse_vector(dimension: int, non_zero_count: int) -> dict:
+    indices = random.sample(range(dimension), non_zero_count)
+    values = [random.random() for _ in range(non_zero_count)]
+    sparse_vector = {index: value for index, value in zip(indices, values)}
+    return sparse_vector
+
 entities = [
     rng.random(num_entities).tolist(),
-    matrix_csr,
+    [generate_sparse_vector(dim, nnz) for _ in range(num_entities)],
 ]
 
 log(fmt.format("Start inserting entities"))
 insert_result = hello_sparse.insert(entities)
 
 # -----------------------------------------------------------------------------
 # create index
```

### Comparing `pymilvus-2.4.1/examples/hybrid_search.py` & `pymilvus-2.4.2/examples/hybrid_search.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/inverted_index_example.py` & `pymilvus-2.4.2/examples/inverted_index_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/iterator.py` & `pymilvus-2.4.2/examples/iterator.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/alias.py` & `pymilvus-2.4.2/examples/milvus_client/alias.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/customize_schema.py` & `pymilvus-2.4.2/examples/milvus_client/customize_schema.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/customize_schema_auto_id.py` & `pymilvus-2.4.2/examples/milvus_client/customize_schema_auto_id.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/index.py` & `pymilvus-2.4.2/examples/milvus_client/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/index_params.py` & `pymilvus-2.4.2/examples/milvus_client/index_params.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/non_ascii_encode.py` & `pymilvus-2.4.2/examples/milvus_client/non_ascii_encode.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/partition.py` & `pymilvus-2.4.2/examples/milvus_client/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/rbac.py` & `pymilvus-2.4.2/examples/milvus_client/rbac.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/simple.py` & `pymilvus-2.4.2/examples/milvus_client/simple.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/simple_auto_id.py` & `pymilvus-2.4.2/examples/milvus_client/simple_auto_id.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/milvus_client/sparse.py` & `pymilvus-2.4.2/examples/milvus_client/sparse.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/multithreading_hello_milvus.py` & `pymilvus-2.4.2/examples/multithreading_hello_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/old_style_example.py` & `pymilvus-2.4.2/examples/old_style_example.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/old_style_example_index.py` & `pymilvus-2.4.2/examples/old_style_example_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/old_style_example_str.py` & `pymilvus-2.4.2/examples/old_style_example_str.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/old_style_query.py` & `pymilvus-2.4.2/examples/old_style_query.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/partition.py` & `pymilvus-2.4.2/examples/partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/resource_group.py` & `pymilvus-2.4.2/examples/resource_group.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/resource_group_declarative_api.py` & `pymilvus-2.4.2/examples/resource_group_declarative_api.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/role_and_privilege.py` & `pymilvus-2.4.2/examples/role_and_privilege.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/examples/user.py` & `pymilvus-2.4.2/examples/user.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/__init__.py` & `pymilvus-2.4.2/pymilvus/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,30 +6,14 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
-from .bulk_writer.bulk_import import (
-    bulk_import,
-    get_import_progress,
-    list_import_jobs,
-)
-
-# bulk writer
-from .bulk_writer.constants import (
-    BulkFileType,
-)
-from .bulk_writer.local_bulk_writer import (
-    LocalBulkWriter,
-)
-from .bulk_writer.remote_bulk_writer import (
-    RemoteBulkWriter,
-)
 from .client import __version__
 from .client.abstract import AnnSearchRequest, Hit, Hits, RRFRanker, SearchResult, WeightedRanker
 from .client.asynch import SearchFuture
 from .client.prepare import Prepare
 from .client.stub import Milvus
 from .client.types import (
     BulkInsertState,
@@ -139,17 +123,11 @@
     "DataType",
     "MilvusException",
     "__version__",
     "MilvusClient",
     "ResourceGroupInfo",
     "Connections",
     "IndexType",
-    "BulkFileType",
-    "LocalBulkWriter",
-    "RemoteBulkWriter",
-    "bulk_import",
-    "get_import_progress",
-    "list_import_jobs",
     "AnnSearchRequest",
     "RRFRanker",
     "WeightedRanker",
 ]
```

### Comparing `pymilvus-2.4.1/pymilvus/bulk_writer/buffer.py` & `pymilvus-2.4.2/pymilvus/bulk_writer/buffer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/bulk_writer/bulk_import.py` & `pymilvus-2.4.2/pymilvus/bulk_writer/bulk_import.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/bulk_writer/bulk_writer.py` & `pymilvus-2.4.2/pymilvus/bulk_writer/bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/bulk_writer/constants.py` & `pymilvus-2.4.2/pymilvus/bulk_writer/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/bulk_writer/local_bulk_writer.py` & `pymilvus-2.4.2/pymilvus/bulk_writer/local_bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/bulk_writer/remote_bulk_writer.py` & `pymilvus-2.4.2/pymilvus/bulk_writer/remote_bulk_writer.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/client/__init__.py` & `pymilvus-2.4.2/pymilvus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/client/abstract.py` & `pymilvus-2.4.2/pymilvus/client/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import ujson
 
 from pymilvus.exceptions import DataTypeNotMatchException, ExceptionsMessage, MilvusException
 from pymilvus.grpc_gen import schema_pb2
 from pymilvus.settings import Config
 
-from . import entity_helper
+from . import entity_helper, utils
 from .constants import DEFAULT_CONSISTENCY_LEVEL, RANKER_TYPE_RRF, RANKER_TYPE_WEIGHTED
 from .types import DataType
 
 
 class FieldSchema:
     def __init__(self, raw: Any):
         self._raw = raw
@@ -323,15 +323,15 @@
             "params": params,
         }
 
 
 class AnnSearchRequest:
     def __init__(
         self,
-        data: Union[List, entity_helper.SparseMatrixInputType],
+        data: Union[List, utils.SparseMatrixInputType],
         anns_field: str,
         param: Dict,
         limit: int,
         expr: Optional[str] = None,
     ):
         self._data = data
         self._anns_field = anns_field
```

### Comparing `pymilvus-2.4.1/pymilvus/client/asynch.py` & `pymilvus-2.4.2/pymilvus/client/asynch.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/client/check.py` & `pymilvus-2.4.2/pymilvus/client/check.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/client/entity_helper.py` & `pymilvus-2.4.2/pymilvus/client/entity_helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,31 @@
 import math
 import struct
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional
 
 import numpy as np
 import ujson
-from scipy import sparse
 
 from pymilvus.exceptions import (
     DataNotMatchException,
     ExceptionsMessage,
     MilvusException,
     ParamError,
 )
 from pymilvus.grpc_gen import schema_pb2 as schema_types
 from pymilvus.settings import Config
 
 from .types import DataType
+from .utils import SciPyHelper, SparseMatrixInputType, SparseRowOutputType
 
 CHECK_STR_ARRAY = True
 
-# in search results, if output fields includes a sparse float vector field, we
-# will return a SparseRowOutputType for each entity. Using Dict for readability.
-# TODO(SPARSE): to allow the user to specify output format.
-SparseRowOutputType = Dict[int, float]
-
-# we accept the following types as input for sparse matrix in user facing APIs
-# such as insert, search, etc.:
-# - scipy sparse array/matrix family: csr, csc, coo, bsr, dia, dok, lil
-# - iterable of iterables, each element(iterable) is a sparse vector with index
-#   as key and value as float.
-#   dict example: [{2: 0.33, 98: 0.72, ...}, {4: 0.45, 198: 0.52, ...}, ...]
-#   list of tuple example: [[(2, 0.33), (98, 0.72), ...], [(4, 0.45), ...], ...]
-#   both index/value can be str numbers: {'2': '3.1'}
-SparseMatrixInputType = Union[
-    Iterable[
-        Union[
-            SparseRowOutputType,
-            Iterable[Tuple[int, float]],  # only type hint, we accept int/float like types
-        ]
-    ],
-    sparse.csc_array,
-    sparse.coo_array,
-    sparse.bsr_array,
-    sparse.dia_array,
-    sparse.dok_array,
-    sparse.lil_array,
-    sparse.csr_array,
-    sparse.spmatrix,
-]
-
-
-def sparse_is_scipy_matrix(data: Any):
-    return isinstance(data, sparse.spmatrix)
-
-
-def sparse_is_scipy_array(data: Any):
-    # sparse.sparray, the common superclass of sparse.*_array, is introduced in
-    # scipy 1.11.0, which requires python 3.9, higher than pymilvus's current requirement.
-    return isinstance(
-        data,
-        (
-            sparse.bsr_array,
-            sparse.coo_array,
-            sparse.csc_array,
-            sparse.csr_array,
-            sparse.dia_array,
-            sparse.dok_array,
-            sparse.lil_array,
-        ),
-    )
-
-
-def sparse_is_scipy_format(data: Any):
-    return sparse_is_scipy_matrix(data) or sparse_is_scipy_array(data)
-
 
 def entity_is_sparse_matrix(entity: Any):
-    if sparse_is_scipy_format(entity):
+    if SciPyHelper.is_scipy_sparse(entity):
         return True
     try:
 
         def is_type_in_str(v: Any, t: Any):
             if not isinstance(v, str):
                 return False
             try:
@@ -110,89 +55,83 @@
         return False
     return True
 
 
 # parses plain bytes to a sparse float vector(SparseRowOutputType)
 def sparse_parse_single_row(data: bytes) -> SparseRowOutputType:
     if len(data) % 8 != 0:
-        msg = f"The length of data must be a multiple of 8, got {len(data)}"
-        raise ValueError(msg)
+        raise ParamError(message=f"The length of data must be a multiple of 8, got {len(data)}")
 
     return {
         struct.unpack("I", data[i : i + 4])[0]: struct.unpack("f", data[i + 4 : i + 8])[0]
         for i in range(0, len(data), 8)
     }
 
 
 # converts supported sparse matrix to schemapb.SparseFloatArray proto
 def sparse_rows_to_proto(data: SparseMatrixInputType) -> schema_types.SparseFloatArray:
     # converts a sparse float vector to plain bytes. the format is the same as how
     # milvus interprets/persists the data.
     def sparse_float_row_to_bytes(indices: Iterable[int], values: Iterable[float]):
         if len(indices) != len(values):
-            msg = f"length of indices and values must be the same, got {len(indices)} and {len(values)}"
-            raise ValueError(msg)
+            raise ParamError(
+                message=f"length of indices and values must be the same, got {len(indices)} and {len(values)}"
+            )
         data = b""
         for i, v in sorted(zip(indices, values), key=lambda x: x[0]):
             if not (0 <= i < 2**32 - 1):
-                msg = f"sparse vector index must be positive and less than 2^32-1: {i}"
-                raise ValueError(msg)
+                raise ParamError(
+                    message=f"sparse vector index must be positive and less than 2^32-1: {i}"
+                )
             if math.isnan(v):
-                msg = "sparse vector value must not be NaN"
-                raise ValueError(msg)
+                raise ParamError(message="sparse vector value must not be NaN")
             data += struct.pack("I", i)
             data += struct.pack("f", v)
         return data
 
-    def unify_sparse_input(data: SparseMatrixInputType) -> sparse.csr_array:
-        if isinstance(data, sparse.csr_array):
-            return data
-        if sparse_is_scipy_array(data):
-            return data.tocsr()
-        if sparse_is_scipy_matrix(data):
-            return sparse.csr_array(data.tocsr())
-        row_indices = []
-        col_indices = []
-        values = []
-        for row_id, row_data in enumerate(data):
-            row = row_data.items() if isinstance(row_data, dict) else row_data
-            row_indices.extend([row_id] * len(row))
-            col_indices.extend(
-                [int(col_id) if isinstance(col_id, str) else col_id for col_id, _ in row]
-            )
-            values.extend([float(value) if isinstance(value, str) else value for _, value in row])
-        return sparse.csr_array((values, (row_indices, col_indices)))
-
     if not entity_is_sparse_matrix(data):
-        msg = "input must be a sparse matrix in supported format"
-        raise TypeError(msg)
-    csr = unify_sparse_input(data)
+        raise ParamError(message="input must be a sparse matrix in supported format")
+
     result = schema_types.SparseFloatArray()
-    result.dim = csr.shape[1]
-    for start, end in zip(csr.indptr[:-1], csr.indptr[1:]):
-        result.contents.append(
-            sparse_float_row_to_bytes(csr.indices[start:end], csr.data[start:end])
-        )
+
+    if SciPyHelper.is_scipy_sparse(data):
+        csr = data.tocsr()
+        result.dim = csr.shape[1]
+        for start, end in zip(csr.indptr[:-1], csr.indptr[1:]):
+            result.contents.append(
+                sparse_float_row_to_bytes(csr.indices[start:end], csr.data[start:end])
+            )
+    else:
+        dim = 0
+        for _, row_data in enumerate(data):
+            indices = []
+            values = []
+            row = row_data.items() if isinstance(row_data, dict) else row_data
+            for index, value in row:
+                indices.append(index)
+                values.append(value)
+            result.contents.append(sparse_float_row_to_bytes(indices, values))
+            dim = max(dim, indices[-1] + 1)
+        result.dim = dim
     return result
 
 
 # converts schema_types.SparseFloatArray proto to Iterable[SparseRowOutputType]
 def sparse_proto_to_rows(
     sfv: schema_types.SparseFloatArray, start: Optional[int] = None, end: Optional[int] = None
 ) -> Iterable[SparseRowOutputType]:
     if not isinstance(sfv, schema_types.SparseFloatArray):
-        msg = "Vector must be a sparse float vector"
-        raise TypeError(msg)
+        raise ParamError(message="Vector must be a sparse float vector")
     start = start or 0
     end = end or len(sfv.contents)
     return [sparse_parse_single_row(row_bytes) for row_bytes in sfv.contents[start:end]]
 
 
 def get_input_num_rows(entity: Any) -> int:
-    if sparse_is_scipy_format(entity):
+    if SciPyHelper.is_scipy_sparse(entity):
         return entity.shape[0]
     return len(entity)
 
 
 def entity_type_to_dtype(entity_type: Any):
     if isinstance(entity_type, int):
         return entity_type
@@ -352,15 +291,15 @@
                 message="invalid input type for bfloat16 vector, expect np.ndarray with dtype=bfloat16"
             )
 
         field_data.vectors.dim = len(v_bytes) // 2
         field_data.vectors.bfloat16_vector += v_bytes
     elif field_type == DataType.SPARSE_FLOAT_VECTOR:
         # field_value is a single row of sparse float vector in user provided format
-        if not sparse_is_scipy_format(field_value):
+        if not SciPyHelper.is_scipy_sparse(field_value):
             field_value = [field_value]
         elif field_value.shape[0] != 1:
             raise ParamError(message="invalid input for sparse float vector: expect 1 row")
         if not entity_is_sparse_matrix(field_value):
             raise ParamError(message="invalid input for sparse float vector")
         field_data.vectors.sparse_float_vector.contents.append(
             sparse_rows_to_proto(field_value).contents[0]
```

### Comparing `pymilvus-2.4.1/pymilvus/client/grpc_handler.py` & `pymilvus-2.4.2/pymilvus/client/grpc_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     MilvusException,
     ParamError,
 )
 from pymilvus.grpc_gen import common_pb2, milvus_pb2_grpc
 from pymilvus.grpc_gen import milvus_pb2 as milvus_types
 from pymilvus.settings import Config
 
-from . import entity_helper, interceptor, ts_utils
+from . import entity_helper, interceptor, ts_utils, utils
 from .abstract import AnnSearchRequest, BaseRanker, CollectionSchema, MutationResult, SearchResult
 from .asynch import (
     CreateIndexFuture,
     FlushFuture,
     LoadPartitionsFuture,
     MutationFuture,
     SearchFuture,
@@ -38,14 +38,15 @@
     is_legal_port,
 )
 from .prepare import Prepare
 from .types import (
     BulkInsertState,
     CompactionPlans,
     CompactionState,
+    DatabaseInfo,
     DataType,
     GrantInfo,
     Group,
     IndexState,
     LoadState,
     Plan,
     Replica,
@@ -757,15 +758,15 @@
                 return SearchFuture(None, None, e)
             raise e from e
 
     @retry_on_rpc_failure(retry_on_inconsistent_requery=True)
     def search(
         self,
         collection_name: str,
-        data: Union[List[List[float]], entity_helper.SparseMatrixInputType],
+        data: Union[List[List[float]], utils.SparseMatrixInputType],
         anns_field: str,
         param: Dict,
         limit: int,
         expression: Optional[str] = None,
         partition_names: Optional[List[str]] = None,
         output_fields: Optional[List[str]] = None,
         round_decimal: int = -1,
@@ -1285,14 +1286,29 @@
     def list_database(self, timeout: Optional[float] = None):
         request = Prepare.list_database_req()
         response = self._stub.ListDatabases(request, timeout=timeout)
         check_status(response.status)
         return list(response.db_names)
 
     @retry_on_rpc_failure()
+    def alter_database(
+        self, db_name: str, properties: dict, timeout: Optional[float] = None, **kwargs
+    ):
+        request = Prepare.alter_database_req(db_name, properties)
+        status = self._stub.AlterDatabase(request, timeout=timeout)
+        check_status(status)
+
+    @retry_on_rpc_failure()
+    def describe_database(self, db_name: str, timeout: Optional[float] = None):
+        request = Prepare.describe_database_req(db_name=db_name)
+        resp = self._stub.DescribeDatabase(request, timeout=timeout)
+        check_status(resp.status)
+        return DatabaseInfo(resp)
+
+    @retry_on_rpc_failure()
     def get_load_state(
         self,
         collection_name: str,
         partition_names: Optional[List[str]] = None,
         timeout: Optional[float] = None,
     ):
         request = Prepare.get_load_state(collection_name, partition_names)
```

### Comparing `pymilvus-2.4.1/pymilvus/client/interceptor.py` & `pymilvus-2.4.2/pymilvus/client/interceptor.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/client/prepare.py` & `pymilvus-2.4.2/pymilvus/client/prepare.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import base64
 import datetime
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Union
 
 import numpy as np
 
-from pymilvus.client import __version__, entity_helper
 from pymilvus.exceptions import DataNotMatchException, ExceptionsMessage, ParamError
 from pymilvus.grpc_gen import common_pb2 as common_types
 from pymilvus.grpc_gen import milvus_pb2 as milvus_types
 from pymilvus.grpc_gen import schema_pb2 as schema_types
 from pymilvus.orm.schema import CollectionSchema
 
-from . import blob, ts_utils, utils
+from . import __version__, blob, entity_helper, ts_utils, utils
 from .check import check_pass_param, is_legal_collection_properties
 from .constants import (
     DEFAULT_CONSISTENCY_LEVEL,
     GROUP_BY_FIELD,
     ITERATOR_FIELD,
     REDUCE_STOP_FOR_BEST,
 )
@@ -622,15 +621,15 @@
             common_types.PlaceholderGroup(placeholders=[pl])
         )
 
     @classmethod
     def search_requests_with_expr(
         cls,
         collection_name: str,
-        data: Union[List, entity_helper.SparseMatrixInputType],
+        data: Union[List, utils.SparseMatrixInputType],
         anns_field: str,
         param: Dict,
         limit: int,
         expr: Optional[str] = None,
         partition_names: Optional[List[str]] = None,
         output_fields: Optional[List[str]] = None,
         round_decimal: int = -1,
@@ -1234,7 +1233,18 @@
     def drop_database_req(cls, db_name: str):
         check_pass_param(db_name=db_name)
         return milvus_types.DropDatabaseRequest(db_name=db_name)
 
     @classmethod
     def list_database_req(cls):
         return milvus_types.ListDatabasesRequest()
+
+    @classmethod
+    def alter_database_req(cls, db_name: str, properties: Dict):
+        check_pass_param(db_name=db_name)
+        kvs = [common_types.KeyValuePair(key=k, value=str(v)) for k, v in properties.items()]
+        return milvus_types.AlterDatabaseRequest(db_name=db_name, properties=kvs)
+
+    @classmethod
+    def describe_database_req(cls, db_name: str):
+        check_pass_param(db_name=db_name)
+        return milvus_types.DescribeDatabaseRequest(db_name=db_name)
```

### Comparing `pymilvus-2.4.1/pymilvus/client/stub.py` & `pymilvus-2.4.2/pymilvus/client/stub.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/client/ts_utils.py` & `pymilvus-2.4.2/pymilvus/client/ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/client/types.py` & `pymilvus-2.4.2/pymilvus/client/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -884,7 +884,36 @@
 
 ResourceGroupTransfer = rg_pb2.ResourceGroupTransfer
 """
 Represents the transfer config of a resource group.
 Attributes:
     resource_group (str): The name of the resource group that can be transferred to or from.
 """
+
+
+class DatabaseInfo:
+    """
+    Represents the information of a database.
+    Atributes:
+        name (str): The name of the database.
+        properties (dict): The properties of the database.
+    Example:
+        DatabaseInfo(name="test_db", id=1, properties={"key": "value"})
+    """
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def properties(self) -> Dict:
+        return self._properties
+
+    def __init__(self, info: Any) -> None:
+        self._name = info.db_name
+        self._properties = {}
+
+        for p in info.properties:
+            self.properties[p.key] = p.value
+
+    def __str__(self) -> str:
+        return f"DatabaseInfo(name={self.name}, properties={self.properties})"
```

### Comparing `pymilvus-2.4.1/pymilvus/decorators.py` & `pymilvus-2.4.2/pymilvus/decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/exceptions.py` & `pymilvus-2.4.2/pymilvus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/common_pb2.py` & `pymilvus-2.4.2/pymilvus/grpc_gen/common_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x13milvus.proto.common\x1a google/protobuf/descriptor.proto\"\xf3\x01\n\x06Status\x12\x36\n\nerror_code\x18\x01 \x01(\x0e\x32\x1e.milvus.proto.common.ErrorCodeB\x02\x18\x01\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\x05\x12\x11\n\tretriable\x18\x04 \x01(\x08\x12\x0e\n\x06\x64\x65tail\x18\x05 \x01(\t\x12>\n\nextra_info\x18\x06 \x03(\x0b\x32*.milvus.proto.common.Status.ExtraInfoEntry\x1a\x30\n\x0e\x45xtraInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"*\n\x0cKeyValuePair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0bKeyDataPair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x15\n\x04\x42lob\x12\r\n\x05value\x18\x01 \x01(\x0c\"c\n\x10PlaceholderValue\x12\x0b\n\x03tag\x18\x01 \x01(\t\x12\x32\n\x04type\x18\x02 \x01(\x0e\x32$.milvus.proto.common.PlaceholderType\x12\x0e\n\x06values\x18\x03 \x03(\x0c\"O\n\x10PlaceholderGroup\x12;\n\x0cplaceholders\x18\x01 \x03(\x0b\x32%.milvus.proto.common.PlaceholderValue\"#\n\x07\x41\x64\x64ress\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\"\xaf\x02\n\x07MsgBase\x12.\n\x08msg_type\x18\x01 \x01(\x0e\x32\x1c.milvus.proto.common.MsgType\x12\r\n\x05msgID\x18\x02 \x01(\x03\x12\x11\n\ttimestamp\x18\x03 \x01(\x04\x12\x10\n\x08sourceID\x18\x04 \x01(\x03\x12\x10\n\x08targetID\x18\x05 \x01(\x03\x12@\n\nproperties\x18\x06 \x03(\x0b\x32,.milvus.proto.common.MsgBase.PropertiesEntry\x12\x39\n\rreplicateInfo\x18\x07 \x01(\x0b\x32\".milvus.proto.common.ReplicateInfo\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\":\n\rReplicateInfo\x12\x13\n\x0bisReplicate\x18\x01 \x01(\x08\x12\x14\n\x0cmsgTimestamp\x18\x02 \x01(\x04\"7\n\tMsgHeader\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"M\n\x0c\x44MLMsgHeader\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x11\n\tshardName\x18\x02 \x01(\t\"\xbb\x01\n\x0cPrivilegeExt\x12\x34\n\x0bobject_type\x18\x01 \x01(\x0e\x32\x1f.milvus.proto.common.ObjectType\x12>\n\x10object_privilege\x18\x02 \x01(\x0e\x32$.milvus.proto.common.ObjectPrivilege\x12\x19\n\x11object_name_index\x18\x03 \x01(\x05\x12\x1a\n\x12object_name_indexs\x18\x04 \x01(\x05\"2\n\x0cSegmentStats\x12\x11\n\tSegmentID\x18\x01 \x01(\x03\x12\x0f\n\x07NumRows\x18\x02 \x01(\x03\"\xd5\x01\n\nClientInfo\x12\x10\n\x08sdk_type\x18\x01 \x01(\t\x12\x13\n\x0bsdk_version\x18\x02 \x01(\t\x12\x12\n\nlocal_time\x18\x03 \x01(\t\x12\x0c\n\x04user\x18\x04 \x01(\t\x12\x0c\n\x04host\x18\x05 \x01(\t\x12?\n\x08reserved\x18\x06 \x03(\x0b\x32-.milvus.proto.common.ClientInfo.ReservedEntry\x1a/\n\rReservedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe3\x01\n\nServerInfo\x12\x12\n\nbuild_tags\x18\x01 \x01(\t\x12\x12\n\nbuild_time\x18\x02 \x01(\t\x12\x12\n\ngit_commit\x18\x03 \x01(\t\x12\x12\n\ngo_version\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65ploy_mode\x18\x05 \x01(\t\x12?\n\x08reserved\x18\x06 \x03(\x0b\x32-.milvus.proto.common.ServerInfo.ReservedEntry\x1a/\n\rReservedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\">\n\x08NodeInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\x03\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08hostname\x18\x03 \x01(\t*\xc7\n\n\tErrorCode\x12\x0b\n\x07Success\x10\x00\x12\x13\n\x0fUnexpectedError\x10\x01\x12\x11\n\rConnectFailed\x10\x02\x12\x14\n\x10PermissionDenied\x10\x03\x12\x17\n\x13\x43ollectionNotExists\x10\x04\x12\x13\n\x0fIllegalArgument\x10\x05\x12\x14\n\x10IllegalDimension\x10\x07\x12\x14\n\x10IllegalIndexType\x10\x08\x12\x19\n\x15IllegalCollectionName\x10\t\x12\x0f\n\x0bIllegalTOPK\x10\n\x12\x14\n\x10IllegalRowRecord\x10\x0b\x12\x13\n\x0fIllegalVectorID\x10\x0c\x12\x17\n\x13IllegalSearchResult\x10\r\x12\x10\n\x0c\x46ileNotFound\x10\x0e\x12\x0e\n\nMetaFailed\x10\x0f\x12\x0f\n\x0b\x43\x61\x63heFailed\x10\x10\x12\x16\n\x12\x43\x61nnotCreateFolder\x10\x11\x12\x14\n\x10\x43\x61nnotCreateFile\x10\x12\x12\x16\n\x12\x43\x61nnotDeleteFolder\x10\x13\x12\x14\n\x10\x43\x61nnotDeleteFile\x10\x14\x12\x13\n\x0f\x42uildIndexError\x10\x15\x12\x10\n\x0cIllegalNLIST\x10\x16\x12\x15\n\x11IllegalMetricType\x10\x17\x12\x0f\n\x0bOutOfMemory\x10\x18\x12\x11\n\rIndexNotExist\x10\x19\x12\x13\n\x0f\x45mptyCollection\x10\x1a\x12\x1b\n\x17UpdateImportTaskFailure\x10\x1b\x12\x1a\n\x16\x43ollectionNameNotFound\x10\x1c\x12\x1b\n\x17\x43reateCredentialFailure\x10\x1d\x12\x1b\n\x17UpdateCredentialFailure\x10\x1e\x12\x1b\n\x17\x44\x65leteCredentialFailure\x10\x1f\x12\x18\n\x14GetCredentialFailure\x10 \x12\x18\n\x14ListCredUsersFailure\x10!\x12\x12\n\x0eGetUserFailure\x10\"\x12\x15\n\x11\x43reateRoleFailure\x10#\x12\x13\n\x0f\x44ropRoleFailure\x10$\x12\x1a\n\x16OperateUserRoleFailure\x10%\x12\x15\n\x11SelectRoleFailure\x10&\x12\x15\n\x11SelectUserFailure\x10\'\x12\x19\n\x15SelectResourceFailure\x10(\x12\x1b\n\x17OperatePrivilegeFailure\x10)\x12\x16\n\x12SelectGrantFailure\x10*\x12!\n\x1dRefreshPolicyInfoCacheFailure\x10+\x12\x15\n\x11ListPolicyFailure\x10,\x12\x12\n\x0eNotShardLeader\x10-\x12\x16\n\x12NoReplicaAvailable\x10.\x12\x13\n\x0fSegmentNotFound\x10/\x12\r\n\tForceDeny\x10\x30\x12\r\n\tRateLimit\x10\x31\x12\x12\n\x0eNodeIDNotMatch\x10\x32\x12\x14\n\x10UpsertAutoIDTrue\x10\x33\x12\x1c\n\x18InsufficientMemoryToLoad\x10\x34\x12\x18\n\x14MemoryQuotaExhausted\x10\x35\x12\x16\n\x12\x44iskQuotaExhausted\x10\x36\x12\x15\n\x11TimeTickLongDelay\x10\x37\x12\x11\n\rNotReadyServe\x10\x38\x12\x1b\n\x17NotReadyCoordActivating\x10\x39\x12\x0f\n\x0b\x44\x61taCoordNA\x10\x64\x12\x12\n\rDDRequestRace\x10\xe8\x07\x1a\x02\x18\x01*c\n\nIndexState\x12\x12\n\x0eIndexStateNone\x10\x00\x12\x0c\n\x08Unissued\x10\x01\x12\x0e\n\nInProgress\x10\x02\x12\x0c\n\x08\x46inished\x10\x03\x12\n\n\x06\x46\x61iled\x10\x04\x12\t\n\x05Retry\x10\x05*\x82\x01\n\x0cSegmentState\x12\x14\n\x10SegmentStateNone\x10\x00\x12\x0c\n\x08NotExist\x10\x01\x12\x0b\n\x07Growing\x10\x02\x12\n\n\x06Sealed\x10\x03\x12\x0b\n\x07\x46lushed\x10\x04\x12\x0c\n\x08\x46lushing\x10\x05\x12\x0b\n\x07\x44ropped\x10\x06\x12\r\n\tImporting\x10\x07*\x94\x01\n\x0fPlaceholderType\x12\x08\n\x04None\x10\x00\x12\x10\n\x0c\x42inaryVector\x10\x64\x12\x0f\n\x0b\x46loatVector\x10\x65\x12\x11\n\rFloat16Vector\x10\x66\x12\x12\n\x0e\x42\x46loat16Vector\x10g\x12\x15\n\x11SparseFloatVector\x10h\x12\t\n\x05Int64\x10\x05\x12\x0b\n\x07VarChar\x10\x15*\xe0\x10\n\x07MsgType\x12\r\n\tUndefined\x10\x00\x12\x14\n\x10\x43reateCollection\x10\x64\x12\x12\n\x0e\x44ropCollection\x10\x65\x12\x11\n\rHasCollection\x10\x66\x12\x16\n\x12\x44\x65scribeCollection\x10g\x12\x13\n\x0fShowCollections\x10h\x12\x14\n\x10GetSystemConfigs\x10i\x12\x12\n\x0eLoadCollection\x10j\x12\x15\n\x11ReleaseCollection\x10k\x12\x0f\n\x0b\x43reateAlias\x10l\x12\r\n\tDropAlias\x10m\x12\x0e\n\nAlterAlias\x10n\x12\x13\n\x0f\x41lterCollection\x10o\x12\x14\n\x10RenameCollection\x10p\x12\x11\n\rDescribeAlias\x10q\x12\x0f\n\x0bListAliases\x10r\x12\x14\n\x0f\x43reatePartition\x10\xc8\x01\x12\x12\n\rDropPartition\x10\xc9\x01\x12\x11\n\x0cHasPartition\x10\xca\x01\x12\x16\n\x11\x44\x65scribePartition\x10\xcb\x01\x12\x13\n\x0eShowPartitions\x10\xcc\x01\x12\x13\n\x0eLoadPartitions\x10\xcd\x01\x12\x16\n\x11ReleasePartitions\x10\xce\x01\x12\x11\n\x0cShowSegments\x10\xfa\x01\x12\x14\n\x0f\x44\x65scribeSegment\x10\xfb\x01\x12\x11\n\x0cLoadSegments\x10\xfc\x01\x12\x14\n\x0fReleaseSegments\x10\xfd\x01\x12\x14\n\x0fHandoffSegments\x10\xfe\x01\x12\x18\n\x13LoadBalanceSegments\x10\xff\x01\x12\x15\n\x10\x44\x65scribeSegments\x10\x80\x02\x12\x1c\n\x17\x46\x65\x64\x65rListIndexedSegment\x10\x81\x02\x12\"\n\x1d\x46\x65\x64\x65rDescribeSegmentIndexData\x10\x82\x02\x12\x10\n\x0b\x43reateIndex\x10\xac\x02\x12\x12\n\rDescribeIndex\x10\xad\x02\x12\x0e\n\tDropIndex\x10\xae\x02\x12\x17\n\x12GetIndexStatistics\x10\xaf\x02\x12\x0f\n\nAlterIndex\x10\xb0\x02\x12\x0b\n\x06Insert\x10\x90\x03\x12\x0b\n\x06\x44\x65lete\x10\x91\x03\x12\n\n\x05\x46lush\x10\x92\x03\x12\x17\n\x12ResendSegmentStats\x10\x93\x03\x12\x0b\n\x06Upsert\x10\x94\x03\x12\x0b\n\x06Search\x10\xf4\x03\x12\x11\n\x0cSearchResult\x10\xf5\x03\x12\x12\n\rGetIndexState\x10\xf6\x03\x12\x1a\n\x15GetIndexBuildProgress\x10\xf7\x03\x12\x1c\n\x17GetCollectionStatistics\x10\xf8\x03\x12\x1b\n\x16GetPartitionStatistics\x10\xf9\x03\x12\r\n\x08Retrieve\x10\xfa\x03\x12\x13\n\x0eRetrieveResult\x10\xfb\x03\x12\x14\n\x0fWatchDmChannels\x10\xfc\x03\x12\x15\n\x10RemoveDmChannels\x10\xfd\x03\x12\x17\n\x12WatchQueryChannels\x10\xfe\x03\x12\x18\n\x13RemoveQueryChannels\x10\xff\x03\x12\x1d\n\x18SealedSegmentsChangeInfo\x10\x80\x04\x12\x17\n\x12WatchDeltaChannels\x10\x81\x04\x12\x14\n\x0fGetShardLeaders\x10\x82\x04\x12\x10\n\x0bGetReplicas\x10\x83\x04\x12\x13\n\x0eUnsubDmChannel\x10\x84\x04\x12\x14\n\x0fGetDistribution\x10\x85\x04\x12\x15\n\x10SyncDistribution\x10\x86\x04\x12\x10\n\x0bSegmentInfo\x10\xd8\x04\x12\x0f\n\nSystemInfo\x10\xd9\x04\x12\x14\n\x0fGetRecoveryInfo\x10\xda\x04\x12\x14\n\x0fGetSegmentState\x10\xdb\x04\x12\r\n\x08TimeTick\x10\xb0\t\x12\x13\n\x0eQueryNodeStats\x10\xb1\t\x12\x0e\n\tLoadIndex\x10\xb2\t\x12\x0e\n\tRequestID\x10\xb3\t\x12\x0f\n\nRequestTSO\x10\xb4\t\x12\x14\n\x0f\x41llocateSegment\x10\xb5\t\x12\x16\n\x11SegmentStatistics\x10\xb6\t\x12\x15\n\x10SegmentFlushDone\x10\xb7\t\x12\x0f\n\nDataNodeTt\x10\xb8\t\x12\x0c\n\x07\x43onnect\x10\xb9\t\x12\x14\n\x0fListClientInfos\x10\xba\t\x12\x13\n\x0e\x41llocTimestamp\x10\xbb\t\x12\x15\n\x10\x43reateCredential\x10\xdc\x0b\x12\x12\n\rGetCredential\x10\xdd\x0b\x12\x15\n\x10\x44\x65leteCredential\x10\xde\x0b\x12\x15\n\x10UpdateCredential\x10\xdf\x0b\x12\x16\n\x11ListCredUsernames\x10\xe0\x0b\x12\x0f\n\nCreateRole\x10\xc0\x0c\x12\r\n\x08\x44ropRole\x10\xc1\x0c\x12\x14\n\x0fOperateUserRole\x10\xc2\x0c\x12\x0f\n\nSelectRole\x10\xc3\x0c\x12\x0f\n\nSelectUser\x10\xc4\x0c\x12\x13\n\x0eSelectResource\x10\xc5\x0c\x12\x15\n\x10OperatePrivilege\x10\xc6\x0c\x12\x10\n\x0bSelectGrant\x10\xc7\x0c\x12\x1b\n\x16RefreshPolicyInfoCache\x10\xc8\x0c\x12\x0f\n\nListPolicy\x10\xc9\x0c\x12\x18\n\x13\x43reateResourceGroup\x10\xa4\r\x12\x16\n\x11\x44ropResourceGroup\x10\xa5\r\x12\x17\n\x12ListResourceGroups\x10\xa6\r\x12\x1a\n\x15\x44\x65scribeResourceGroup\x10\xa7\r\x12\x11\n\x0cTransferNode\x10\xa8\r\x12\x14\n\x0fTransferReplica\x10\xa9\r\x12\x19\n\x14UpdateResourceGroups\x10\xaa\r\x12\x13\n\x0e\x43reateDatabase\x10\x89\x0e\x12\x11\n\x0c\x44ropDatabase\x10\x8a\x0e\x12\x12\n\rListDatabases\x10\x8b\x0e*\"\n\x07\x44slType\x12\x07\n\x03\x44sl\x10\x00\x12\x0e\n\nBoolExprV1\x10\x01*B\n\x0f\x43ompactionState\x12\x11\n\rUndefiedState\x10\x00\x12\r\n\tExecuting\x10\x01\x12\r\n\tCompleted\x10\x02*X\n\x10\x43onsistencyLevel\x12\n\n\x06Strong\x10\x00\x12\x0b\n\x07Session\x10\x01\x12\x0b\n\x07\x42ounded\x10\x02\x12\x0e\n\nEventually\x10\x03\x12\x0e\n\nCustomized\x10\x04*\x9e\x01\n\x0bImportState\x12\x11\n\rImportPending\x10\x00\x12\x10\n\x0cImportFailed\x10\x01\x12\x11\n\rImportStarted\x10\x02\x12\x13\n\x0fImportPersisted\x10\x05\x12\x11\n\rImportFlushed\x10\x08\x12\x13\n\x0fImportCompleted\x10\x06\x12\x1a\n\x16ImportFailedAndCleaned\x10\x07*2\n\nObjectType\x12\x0e\n\nCollection\x10\x00\x12\n\n\x06Global\x10\x01\x12\x08\n\x04User\x10\x02*\xd6\n\n\x0fObjectPrivilege\x12\x10\n\x0cPrivilegeAll\x10\x00\x12\x1d\n\x19PrivilegeCreateCollection\x10\x01\x12\x1b\n\x17PrivilegeDropCollection\x10\x02\x12\x1f\n\x1bPrivilegeDescribeCollection\x10\x03\x12\x1c\n\x18PrivilegeShowCollections\x10\x04\x12\x11\n\rPrivilegeLoad\x10\x05\x12\x14\n\x10PrivilegeRelease\x10\x06\x12\x17\n\x13PrivilegeCompaction\x10\x07\x12\x13\n\x0fPrivilegeInsert\x10\x08\x12\x13\n\x0fPrivilegeDelete\x10\t\x12\x1a\n\x16PrivilegeGetStatistics\x10\n\x12\x18\n\x14PrivilegeCreateIndex\x10\x0b\x12\x18\n\x14PrivilegeIndexDetail\x10\x0c\x12\x16\n\x12PrivilegeDropIndex\x10\r\x12\x13\n\x0fPrivilegeSearch\x10\x0e\x12\x12\n\x0ePrivilegeFlush\x10\x0f\x12\x12\n\x0ePrivilegeQuery\x10\x10\x12\x18\n\x14PrivilegeLoadBalance\x10\x11\x12\x13\n\x0fPrivilegeImport\x10\x12\x12\x1c\n\x18PrivilegeCreateOwnership\x10\x13\x12\x17\n\x13PrivilegeUpdateUser\x10\x14\x12\x1a\n\x16PrivilegeDropOwnership\x10\x15\x12\x1c\n\x18PrivilegeSelectOwnership\x10\x16\x12\x1c\n\x18PrivilegeManageOwnership\x10\x17\x12\x17\n\x13PrivilegeSelectUser\x10\x18\x12\x13\n\x0fPrivilegeUpsert\x10\x19\x12 \n\x1cPrivilegeCreateResourceGroup\x10\x1a\x12\x1e\n\x1aPrivilegeDropResourceGroup\x10\x1b\x12\"\n\x1ePrivilegeDescribeResourceGroup\x10\x1c\x12\x1f\n\x1bPrivilegeListResourceGroups\x10\x1d\x12\x19\n\x15PrivilegeTransferNode\x10\x1e\x12\x1c\n\x18PrivilegeTransferReplica\x10\x1f\x12\x1f\n\x1bPrivilegeGetLoadingProgress\x10 \x12\x19\n\x15PrivilegeGetLoadState\x10!\x12\x1d\n\x19PrivilegeRenameCollection\x10\"\x12\x1b\n\x17PrivilegeCreateDatabase\x10#\x12\x19\n\x15PrivilegeDropDatabase\x10$\x12\x1a\n\x16PrivilegeListDatabases\x10%\x12\x15\n\x11PrivilegeFlushAll\x10&\x12\x1c\n\x18PrivilegeCreatePartition\x10\'\x12\x1a\n\x16PrivilegeDropPartition\x10(\x12\x1b\n\x17PrivilegeShowPartitions\x10)\x12\x19\n\x15PrivilegeHasPartition\x10*\x12\x1a\n\x16PrivilegeGetFlushState\x10+\x12\x18\n\x14PrivilegeCreateAlias\x10,\x12\x16\n\x12PrivilegeDropAlias\x10-\x12\x1a\n\x16PrivilegeDescribeAlias\x10.\x12\x18\n\x14PrivilegeListAliases\x10/\x12!\n\x1dPrivilegeUpdateResourceGroups\x10\x30\x12\x1a\n\x16PrivilegeAlterDatabase\x10\x31*S\n\tStateCode\x12\x10\n\x0cInitializing\x10\x00\x12\x0b\n\x07Healthy\x10\x01\x12\x0c\n\x08\x41\x62normal\x10\x02\x12\x0b\n\x07StandBy\x10\x03\x12\x0c\n\x08Stopping\x10\x04*c\n\tLoadState\x12\x15\n\x11LoadStateNotExist\x10\x00\x12\x14\n\x10LoadStateNotLoad\x10\x01\x12\x14\n\x10LoadStateLoading\x10\x02\x12\x13\n\x0fLoadStateLoaded\x10\x03:^\n\x11privilege_ext_obj\x12\x1f.google.protobuf.MessageOptions\x18\xe9\x07 \x01(\x0b\x32!.milvus.proto.common.PrivilegeExtBm\n\x0eio.milvus.grpcB\x0b\x43ommonProtoP\x01Z4github.com/milvus-io/milvus-proto/go-api/v2/commonpb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0c\x63ommon.proto\x12\x13milvus.proto.common\x1a google/protobuf/descriptor.proto\"\xf3\x01\n\x06Status\x12\x36\n\nerror_code\x18\x01 \x01(\x0e\x32\x1e.milvus.proto.common.ErrorCodeB\x02\x18\x01\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0c\n\x04\x63ode\x18\x03 \x01(\x05\x12\x11\n\tretriable\x18\x04 \x01(\x08\x12\x0e\n\x06\x64\x65tail\x18\x05 \x01(\t\x12>\n\nextra_info\x18\x06 \x03(\x0b\x32*.milvus.proto.common.Status.ExtraInfoEntry\x1a\x30\n\x0e\x45xtraInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"*\n\x0cKeyValuePair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0bKeyDataPair\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"\x15\n\x04\x42lob\x12\r\n\x05value\x18\x01 \x01(\x0c\"c\n\x10PlaceholderValue\x12\x0b\n\x03tag\x18\x01 \x01(\t\x12\x32\n\x04type\x18\x02 \x01(\x0e\x32$.milvus.proto.common.PlaceholderType\x12\x0e\n\x06values\x18\x03 \x03(\x0c\"O\n\x10PlaceholderGroup\x12;\n\x0cplaceholders\x18\x01 \x03(\x0b\x32%.milvus.proto.common.PlaceholderValue\"#\n\x07\x41\x64\x64ress\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x03\"\xaf\x02\n\x07MsgBase\x12.\n\x08msg_type\x18\x01 \x01(\x0e\x32\x1c.milvus.proto.common.MsgType\x12\r\n\x05msgID\x18\x02 \x01(\x03\x12\x11\n\ttimestamp\x18\x03 \x01(\x04\x12\x10\n\x08sourceID\x18\x04 \x01(\x03\x12\x10\n\x08targetID\x18\x05 \x01(\x03\x12@\n\nproperties\x18\x06 \x03(\x0b\x32,.milvus.proto.common.MsgBase.PropertiesEntry\x12\x39\n\rreplicateInfo\x18\x07 \x01(\x0b\x32\".milvus.proto.common.ReplicateInfo\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\":\n\rReplicateInfo\x12\x13\n\x0bisReplicate\x18\x01 \x01(\x08\x12\x14\n\x0cmsgTimestamp\x18\x02 \x01(\x04\"7\n\tMsgHeader\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"M\n\x0c\x44MLMsgHeader\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x11\n\tshardName\x18\x02 \x01(\t\"\xbb\x01\n\x0cPrivilegeExt\x12\x34\n\x0bobject_type\x18\x01 \x01(\x0e\x32\x1f.milvus.proto.common.ObjectType\x12>\n\x10object_privilege\x18\x02 \x01(\x0e\x32$.milvus.proto.common.ObjectPrivilege\x12\x19\n\x11object_name_index\x18\x03 \x01(\x05\x12\x1a\n\x12object_name_indexs\x18\x04 \x01(\x05\"2\n\x0cSegmentStats\x12\x11\n\tSegmentID\x18\x01 \x01(\x03\x12\x0f\n\x07NumRows\x18\x02 \x01(\x03\"\xd5\x01\n\nClientInfo\x12\x10\n\x08sdk_type\x18\x01 \x01(\t\x12\x13\n\x0bsdk_version\x18\x02 \x01(\t\x12\x12\n\nlocal_time\x18\x03 \x01(\t\x12\x0c\n\x04user\x18\x04 \x01(\t\x12\x0c\n\x04host\x18\x05 \x01(\t\x12?\n\x08reserved\x18\x06 \x03(\x0b\x32-.milvus.proto.common.ClientInfo.ReservedEntry\x1a/\n\rReservedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe3\x01\n\nServerInfo\x12\x12\n\nbuild_tags\x18\x01 \x01(\t\x12\x12\n\nbuild_time\x18\x02 \x01(\t\x12\x12\n\ngit_commit\x18\x03 \x01(\t\x12\x12\n\ngo_version\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65ploy_mode\x18\x05 \x01(\t\x12?\n\x08reserved\x18\x06 \x03(\x0b\x32-.milvus.proto.common.ServerInfo.ReservedEntry\x1a/\n\rReservedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\">\n\x08NodeInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\x03\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08hostname\x18\x03 \x01(\t*\xc7\n\n\tErrorCode\x12\x0b\n\x07Success\x10\x00\x12\x13\n\x0fUnexpectedError\x10\x01\x12\x11\n\rConnectFailed\x10\x02\x12\x14\n\x10PermissionDenied\x10\x03\x12\x17\n\x13\x43ollectionNotExists\x10\x04\x12\x13\n\x0fIllegalArgument\x10\x05\x12\x14\n\x10IllegalDimension\x10\x07\x12\x14\n\x10IllegalIndexType\x10\x08\x12\x19\n\x15IllegalCollectionName\x10\t\x12\x0f\n\x0bIllegalTOPK\x10\n\x12\x14\n\x10IllegalRowRecord\x10\x0b\x12\x13\n\x0fIllegalVectorID\x10\x0c\x12\x17\n\x13IllegalSearchResult\x10\r\x12\x10\n\x0c\x46ileNotFound\x10\x0e\x12\x0e\n\nMetaFailed\x10\x0f\x12\x0f\n\x0b\x43\x61\x63heFailed\x10\x10\x12\x16\n\x12\x43\x61nnotCreateFolder\x10\x11\x12\x14\n\x10\x43\x61nnotCreateFile\x10\x12\x12\x16\n\x12\x43\x61nnotDeleteFolder\x10\x13\x12\x14\n\x10\x43\x61nnotDeleteFile\x10\x14\x12\x13\n\x0f\x42uildIndexError\x10\x15\x12\x10\n\x0cIllegalNLIST\x10\x16\x12\x15\n\x11IllegalMetricType\x10\x17\x12\x0f\n\x0bOutOfMemory\x10\x18\x12\x11\n\rIndexNotExist\x10\x19\x12\x13\n\x0f\x45mptyCollection\x10\x1a\x12\x1b\n\x17UpdateImportTaskFailure\x10\x1b\x12\x1a\n\x16\x43ollectionNameNotFound\x10\x1c\x12\x1b\n\x17\x43reateCredentialFailure\x10\x1d\x12\x1b\n\x17UpdateCredentialFailure\x10\x1e\x12\x1b\n\x17\x44\x65leteCredentialFailure\x10\x1f\x12\x18\n\x14GetCredentialFailure\x10 \x12\x18\n\x14ListCredUsersFailure\x10!\x12\x12\n\x0eGetUserFailure\x10\"\x12\x15\n\x11\x43reateRoleFailure\x10#\x12\x13\n\x0f\x44ropRoleFailure\x10$\x12\x1a\n\x16OperateUserRoleFailure\x10%\x12\x15\n\x11SelectRoleFailure\x10&\x12\x15\n\x11SelectUserFailure\x10\'\x12\x19\n\x15SelectResourceFailure\x10(\x12\x1b\n\x17OperatePrivilegeFailure\x10)\x12\x16\n\x12SelectGrantFailure\x10*\x12!\n\x1dRefreshPolicyInfoCacheFailure\x10+\x12\x15\n\x11ListPolicyFailure\x10,\x12\x12\n\x0eNotShardLeader\x10-\x12\x16\n\x12NoReplicaAvailable\x10.\x12\x13\n\x0fSegmentNotFound\x10/\x12\r\n\tForceDeny\x10\x30\x12\r\n\tRateLimit\x10\x31\x12\x12\n\x0eNodeIDNotMatch\x10\x32\x12\x14\n\x10UpsertAutoIDTrue\x10\x33\x12\x1c\n\x18InsufficientMemoryToLoad\x10\x34\x12\x18\n\x14MemoryQuotaExhausted\x10\x35\x12\x16\n\x12\x44iskQuotaExhausted\x10\x36\x12\x15\n\x11TimeTickLongDelay\x10\x37\x12\x11\n\rNotReadyServe\x10\x38\x12\x1b\n\x17NotReadyCoordActivating\x10\x39\x12\x0f\n\x0b\x44\x61taCoordNA\x10\x64\x12\x12\n\rDDRequestRace\x10\xe8\x07\x1a\x02\x18\x01*c\n\nIndexState\x12\x12\n\x0eIndexStateNone\x10\x00\x12\x0c\n\x08Unissued\x10\x01\x12\x0e\n\nInProgress\x10\x02\x12\x0c\n\x08\x46inished\x10\x03\x12\n\n\x06\x46\x61iled\x10\x04\x12\t\n\x05Retry\x10\x05*\x82\x01\n\x0cSegmentState\x12\x14\n\x10SegmentStateNone\x10\x00\x12\x0c\n\x08NotExist\x10\x01\x12\x0b\n\x07Growing\x10\x02\x12\n\n\x06Sealed\x10\x03\x12\x0b\n\x07\x46lushed\x10\x04\x12\x0c\n\x08\x46lushing\x10\x05\x12\x0b\n\x07\x44ropped\x10\x06\x12\r\n\tImporting\x10\x07*\x94\x01\n\x0fPlaceholderType\x12\x08\n\x04None\x10\x00\x12\x10\n\x0c\x42inaryVector\x10\x64\x12\x0f\n\x0b\x46loatVector\x10\x65\x12\x11\n\rFloat16Vector\x10\x66\x12\x12\n\x0e\x42\x46loat16Vector\x10g\x12\x15\n\x11SparseFloatVector\x10h\x12\t\n\x05Int64\x10\x05\x12\x0b\n\x07VarChar\x10\x15*\x8b\x11\n\x07MsgType\x12\r\n\tUndefined\x10\x00\x12\x14\n\x10\x43reateCollection\x10\x64\x12\x12\n\x0e\x44ropCollection\x10\x65\x12\x11\n\rHasCollection\x10\x66\x12\x16\n\x12\x44\x65scribeCollection\x10g\x12\x13\n\x0fShowCollections\x10h\x12\x14\n\x10GetSystemConfigs\x10i\x12\x12\n\x0eLoadCollection\x10j\x12\x15\n\x11ReleaseCollection\x10k\x12\x0f\n\x0b\x43reateAlias\x10l\x12\r\n\tDropAlias\x10m\x12\x0e\n\nAlterAlias\x10n\x12\x13\n\x0f\x41lterCollection\x10o\x12\x14\n\x10RenameCollection\x10p\x12\x11\n\rDescribeAlias\x10q\x12\x0f\n\x0bListAliases\x10r\x12\x14\n\x0f\x43reatePartition\x10\xc8\x01\x12\x12\n\rDropPartition\x10\xc9\x01\x12\x11\n\x0cHasPartition\x10\xca\x01\x12\x16\n\x11\x44\x65scribePartition\x10\xcb\x01\x12\x13\n\x0eShowPartitions\x10\xcc\x01\x12\x13\n\x0eLoadPartitions\x10\xcd\x01\x12\x16\n\x11ReleasePartitions\x10\xce\x01\x12\x11\n\x0cShowSegments\x10\xfa\x01\x12\x14\n\x0f\x44\x65scribeSegment\x10\xfb\x01\x12\x11\n\x0cLoadSegments\x10\xfc\x01\x12\x14\n\x0fReleaseSegments\x10\xfd\x01\x12\x14\n\x0fHandoffSegments\x10\xfe\x01\x12\x18\n\x13LoadBalanceSegments\x10\xff\x01\x12\x15\n\x10\x44\x65scribeSegments\x10\x80\x02\x12\x1c\n\x17\x46\x65\x64\x65rListIndexedSegment\x10\x81\x02\x12\"\n\x1d\x46\x65\x64\x65rDescribeSegmentIndexData\x10\x82\x02\x12\x10\n\x0b\x43reateIndex\x10\xac\x02\x12\x12\n\rDescribeIndex\x10\xad\x02\x12\x0e\n\tDropIndex\x10\xae\x02\x12\x17\n\x12GetIndexStatistics\x10\xaf\x02\x12\x0f\n\nAlterIndex\x10\xb0\x02\x12\x0b\n\x06Insert\x10\x90\x03\x12\x0b\n\x06\x44\x65lete\x10\x91\x03\x12\n\n\x05\x46lush\x10\x92\x03\x12\x17\n\x12ResendSegmentStats\x10\x93\x03\x12\x0b\n\x06Upsert\x10\x94\x03\x12\x0b\n\x06Search\x10\xf4\x03\x12\x11\n\x0cSearchResult\x10\xf5\x03\x12\x12\n\rGetIndexState\x10\xf6\x03\x12\x1a\n\x15GetIndexBuildProgress\x10\xf7\x03\x12\x1c\n\x17GetCollectionStatistics\x10\xf8\x03\x12\x1b\n\x16GetPartitionStatistics\x10\xf9\x03\x12\r\n\x08Retrieve\x10\xfa\x03\x12\x13\n\x0eRetrieveResult\x10\xfb\x03\x12\x14\n\x0fWatchDmChannels\x10\xfc\x03\x12\x15\n\x10RemoveDmChannels\x10\xfd\x03\x12\x17\n\x12WatchQueryChannels\x10\xfe\x03\x12\x18\n\x13RemoveQueryChannels\x10\xff\x03\x12\x1d\n\x18SealedSegmentsChangeInfo\x10\x80\x04\x12\x17\n\x12WatchDeltaChannels\x10\x81\x04\x12\x14\n\x0fGetShardLeaders\x10\x82\x04\x12\x10\n\x0bGetReplicas\x10\x83\x04\x12\x13\n\x0eUnsubDmChannel\x10\x84\x04\x12\x14\n\x0fGetDistribution\x10\x85\x04\x12\x15\n\x10SyncDistribution\x10\x86\x04\x12\x10\n\x0bSegmentInfo\x10\xd8\x04\x12\x0f\n\nSystemInfo\x10\xd9\x04\x12\x14\n\x0fGetRecoveryInfo\x10\xda\x04\x12\x14\n\x0fGetSegmentState\x10\xdb\x04\x12\r\n\x08TimeTick\x10\xb0\t\x12\x13\n\x0eQueryNodeStats\x10\xb1\t\x12\x0e\n\tLoadIndex\x10\xb2\t\x12\x0e\n\tRequestID\x10\xb3\t\x12\x0f\n\nRequestTSO\x10\xb4\t\x12\x14\n\x0f\x41llocateSegment\x10\xb5\t\x12\x16\n\x11SegmentStatistics\x10\xb6\t\x12\x15\n\x10SegmentFlushDone\x10\xb7\t\x12\x0f\n\nDataNodeTt\x10\xb8\t\x12\x0c\n\x07\x43onnect\x10\xb9\t\x12\x14\n\x0fListClientInfos\x10\xba\t\x12\x13\n\x0e\x41llocTimestamp\x10\xbb\t\x12\x15\n\x10\x43reateCredential\x10\xdc\x0b\x12\x12\n\rGetCredential\x10\xdd\x0b\x12\x15\n\x10\x44\x65leteCredential\x10\xde\x0b\x12\x15\n\x10UpdateCredential\x10\xdf\x0b\x12\x16\n\x11ListCredUsernames\x10\xe0\x0b\x12\x0f\n\nCreateRole\x10\xc0\x0c\x12\r\n\x08\x44ropRole\x10\xc1\x0c\x12\x14\n\x0fOperateUserRole\x10\xc2\x0c\x12\x0f\n\nSelectRole\x10\xc3\x0c\x12\x0f\n\nSelectUser\x10\xc4\x0c\x12\x13\n\x0eSelectResource\x10\xc5\x0c\x12\x15\n\x10OperatePrivilege\x10\xc6\x0c\x12\x10\n\x0bSelectGrant\x10\xc7\x0c\x12\x1b\n\x16RefreshPolicyInfoCache\x10\xc8\x0c\x12\x0f\n\nListPolicy\x10\xc9\x0c\x12\x18\n\x13\x43reateResourceGroup\x10\xa4\r\x12\x16\n\x11\x44ropResourceGroup\x10\xa5\r\x12\x17\n\x12ListResourceGroups\x10\xa6\r\x12\x1a\n\x15\x44\x65scribeResourceGroup\x10\xa7\r\x12\x11\n\x0cTransferNode\x10\xa8\r\x12\x14\n\x0fTransferReplica\x10\xa9\r\x12\x19\n\x14UpdateResourceGroups\x10\xaa\r\x12\x13\n\x0e\x43reateDatabase\x10\x89\x0e\x12\x11\n\x0c\x44ropDatabase\x10\x8a\x0e\x12\x12\n\rListDatabases\x10\x8b\x0e\x12\x12\n\rAlterDatabase\x10\x8c\x0e\x12\x15\n\x10\x44\x65scribeDatabase\x10\x8d\x0e*\"\n\x07\x44slType\x12\x07\n\x03\x44sl\x10\x00\x12\x0e\n\nBoolExprV1\x10\x01*B\n\x0f\x43ompactionState\x12\x11\n\rUndefiedState\x10\x00\x12\r\n\tExecuting\x10\x01\x12\r\n\tCompleted\x10\x02*X\n\x10\x43onsistencyLevel\x12\n\n\x06Strong\x10\x00\x12\x0b\n\x07Session\x10\x01\x12\x0b\n\x07\x42ounded\x10\x02\x12\x0e\n\nEventually\x10\x03\x12\x0e\n\nCustomized\x10\x04*\x9e\x01\n\x0bImportState\x12\x11\n\rImportPending\x10\x00\x12\x10\n\x0cImportFailed\x10\x01\x12\x11\n\rImportStarted\x10\x02\x12\x13\n\x0fImportPersisted\x10\x05\x12\x11\n\rImportFlushed\x10\x08\x12\x13\n\x0fImportCompleted\x10\x06\x12\x1a\n\x16ImportFailedAndCleaned\x10\x07*2\n\nObjectType\x12\x0e\n\nCollection\x10\x00\x12\n\n\x06Global\x10\x01\x12\x08\n\x04User\x10\x02*\xf5\n\n\x0fObjectPrivilege\x12\x10\n\x0cPrivilegeAll\x10\x00\x12\x1d\n\x19PrivilegeCreateCollection\x10\x01\x12\x1b\n\x17PrivilegeDropCollection\x10\x02\x12\x1f\n\x1bPrivilegeDescribeCollection\x10\x03\x12\x1c\n\x18PrivilegeShowCollections\x10\x04\x12\x11\n\rPrivilegeLoad\x10\x05\x12\x14\n\x10PrivilegeRelease\x10\x06\x12\x17\n\x13PrivilegeCompaction\x10\x07\x12\x13\n\x0fPrivilegeInsert\x10\x08\x12\x13\n\x0fPrivilegeDelete\x10\t\x12\x1a\n\x16PrivilegeGetStatistics\x10\n\x12\x18\n\x14PrivilegeCreateIndex\x10\x0b\x12\x18\n\x14PrivilegeIndexDetail\x10\x0c\x12\x16\n\x12PrivilegeDropIndex\x10\r\x12\x13\n\x0fPrivilegeSearch\x10\x0e\x12\x12\n\x0ePrivilegeFlush\x10\x0f\x12\x12\n\x0ePrivilegeQuery\x10\x10\x12\x18\n\x14PrivilegeLoadBalance\x10\x11\x12\x13\n\x0fPrivilegeImport\x10\x12\x12\x1c\n\x18PrivilegeCreateOwnership\x10\x13\x12\x17\n\x13PrivilegeUpdateUser\x10\x14\x12\x1a\n\x16PrivilegeDropOwnership\x10\x15\x12\x1c\n\x18PrivilegeSelectOwnership\x10\x16\x12\x1c\n\x18PrivilegeManageOwnership\x10\x17\x12\x17\n\x13PrivilegeSelectUser\x10\x18\x12\x13\n\x0fPrivilegeUpsert\x10\x19\x12 \n\x1cPrivilegeCreateResourceGroup\x10\x1a\x12\x1e\n\x1aPrivilegeDropResourceGroup\x10\x1b\x12\"\n\x1ePrivilegeDescribeResourceGroup\x10\x1c\x12\x1f\n\x1bPrivilegeListResourceGroups\x10\x1d\x12\x19\n\x15PrivilegeTransferNode\x10\x1e\x12\x1c\n\x18PrivilegeTransferReplica\x10\x1f\x12\x1f\n\x1bPrivilegeGetLoadingProgress\x10 \x12\x19\n\x15PrivilegeGetLoadState\x10!\x12\x1d\n\x19PrivilegeRenameCollection\x10\"\x12\x1b\n\x17PrivilegeCreateDatabase\x10#\x12\x19\n\x15PrivilegeDropDatabase\x10$\x12\x1a\n\x16PrivilegeListDatabases\x10%\x12\x15\n\x11PrivilegeFlushAll\x10&\x12\x1c\n\x18PrivilegeCreatePartition\x10\'\x12\x1a\n\x16PrivilegeDropPartition\x10(\x12\x1b\n\x17PrivilegeShowPartitions\x10)\x12\x19\n\x15PrivilegeHasPartition\x10*\x12\x1a\n\x16PrivilegeGetFlushState\x10+\x12\x18\n\x14PrivilegeCreateAlias\x10,\x12\x16\n\x12PrivilegeDropAlias\x10-\x12\x1a\n\x16PrivilegeDescribeAlias\x10.\x12\x18\n\x14PrivilegeListAliases\x10/\x12!\n\x1dPrivilegeUpdateResourceGroups\x10\x30\x12\x1a\n\x16PrivilegeAlterDatabase\x10\x31\x12\x1d\n\x19PrivilegeDescribeDatabase\x10\x32*S\n\tStateCode\x12\x10\n\x0cInitializing\x10\x00\x12\x0b\n\x07Healthy\x10\x01\x12\x0c\n\x08\x41\x62normal\x10\x02\x12\x0b\n\x07StandBy\x10\x03\x12\x0c\n\x08Stopping\x10\x04*c\n\tLoadState\x12\x15\n\x11LoadStateNotExist\x10\x00\x12\x14\n\x10LoadStateNotLoad\x10\x01\x12\x14\n\x10LoadStateLoading\x10\x02\x12\x13\n\x0fLoadStateLoaded\x10\x03:^\n\x11privilege_ext_obj\x12\x1f.google.protobuf.MessageOptions\x18\xe9\x07 \x01(\x0b\x32!.milvus.proto.common.PrivilegeExtBm\n\x0eio.milvus.grpcB\x0b\x43ommonProtoP\x01Z4github.com/milvus-io/milvus-proto/go-api/v2/commonpb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\016io.milvus.grpcB\013CommonProtoP\001Z4github.com/milvus-io/milvus-proto/go-api/v2/commonpb\240\001\001\252\002\022Milvus.Client.Grpc'
@@ -40,31 +40,31 @@
   _globals['_INDEXSTATE']._serialized_start=3253
   _globals['_INDEXSTATE']._serialized_end=3352
   _globals['_SEGMENTSTATE']._serialized_start=3355
   _globals['_SEGMENTSTATE']._serialized_end=3485
   _globals['_PLACEHOLDERTYPE']._serialized_start=3488
   _globals['_PLACEHOLDERTYPE']._serialized_end=3636
   _globals['_MSGTYPE']._serialized_start=3639
-  _globals['_MSGTYPE']._serialized_end=5783
-  _globals['_DSLTYPE']._serialized_start=5785
-  _globals['_DSLTYPE']._serialized_end=5819
-  _globals['_COMPACTIONSTATE']._serialized_start=5821
-  _globals['_COMPACTIONSTATE']._serialized_end=5887
-  _globals['_CONSISTENCYLEVEL']._serialized_start=5889
-  _globals['_CONSISTENCYLEVEL']._serialized_end=5977
-  _globals['_IMPORTSTATE']._serialized_start=5980
-  _globals['_IMPORTSTATE']._serialized_end=6138
-  _globals['_OBJECTTYPE']._serialized_start=6140
-  _globals['_OBJECTTYPE']._serialized_end=6190
-  _globals['_OBJECTPRIVILEGE']._serialized_start=6193
-  _globals['_OBJECTPRIVILEGE']._serialized_end=7559
-  _globals['_STATECODE']._serialized_start=7561
-  _globals['_STATECODE']._serialized_end=7644
-  _globals['_LOADSTATE']._serialized_start=7646
-  _globals['_LOADSTATE']._serialized_end=7745
+  _globals['_MSGTYPE']._serialized_end=5826
+  _globals['_DSLTYPE']._serialized_start=5828
+  _globals['_DSLTYPE']._serialized_end=5862
+  _globals['_COMPACTIONSTATE']._serialized_start=5864
+  _globals['_COMPACTIONSTATE']._serialized_end=5930
+  _globals['_CONSISTENCYLEVEL']._serialized_start=5932
+  _globals['_CONSISTENCYLEVEL']._serialized_end=6020
+  _globals['_IMPORTSTATE']._serialized_start=6023
+  _globals['_IMPORTSTATE']._serialized_end=6181
+  _globals['_OBJECTTYPE']._serialized_start=6183
+  _globals['_OBJECTTYPE']._serialized_end=6233
+  _globals['_OBJECTPRIVILEGE']._serialized_start=6236
+  _globals['_OBJECTPRIVILEGE']._serialized_end=7633
+  _globals['_STATECODE']._serialized_start=7635
+  _globals['_STATECODE']._serialized_end=7718
+  _globals['_LOADSTATE']._serialized_start=7720
+  _globals['_LOADSTATE']._serialized_end=7819
   _globals['_STATUS']._serialized_start=72
   _globals['_STATUS']._serialized_end=315
   _globals['_STATUS_EXTRAINFOENTRY']._serialized_start=267
   _globals['_STATUS_EXTRAINFOENTRY']._serialized_end=315
   _globals['_KEYVALUEPAIR']._serialized_start=317
   _globals['_KEYVALUEPAIR']._serialized_end=359
   _globals['_KEYDATAPAIR']._serialized_start=361
```

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/common_pb2.pyi` & `pymilvus-2.4.2/pymilvus/grpc_gen/common_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,16 @@
     DescribeResourceGroup: _ClassVar[MsgType]
     TransferNode: _ClassVar[MsgType]
     TransferReplica: _ClassVar[MsgType]
     UpdateResourceGroups: _ClassVar[MsgType]
     CreateDatabase: _ClassVar[MsgType]
     DropDatabase: _ClassVar[MsgType]
     ListDatabases: _ClassVar[MsgType]
+    AlterDatabase: _ClassVar[MsgType]
+    DescribeDatabase: _ClassVar[MsgType]
 
 class DslType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     Dsl: _ClassVar[DslType]
     BoolExprV1: _ClassVar[DslType]
 
 class CompactionState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
@@ -288,14 +290,15 @@
     PrivilegeGetFlushState: _ClassVar[ObjectPrivilege]
     PrivilegeCreateAlias: _ClassVar[ObjectPrivilege]
     PrivilegeDropAlias: _ClassVar[ObjectPrivilege]
     PrivilegeDescribeAlias: _ClassVar[ObjectPrivilege]
     PrivilegeListAliases: _ClassVar[ObjectPrivilege]
     PrivilegeUpdateResourceGroups: _ClassVar[ObjectPrivilege]
     PrivilegeAlterDatabase: _ClassVar[ObjectPrivilege]
+    PrivilegeDescribeDatabase: _ClassVar[ObjectPrivilege]
 
 class StateCode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     Initializing: _ClassVar[StateCode]
     Healthy: _ClassVar[StateCode]
     Abnormal: _ClassVar[StateCode]
     StandBy: _ClassVar[StateCode]
@@ -486,14 +489,16 @@
 DescribeResourceGroup: MsgType
 TransferNode: MsgType
 TransferReplica: MsgType
 UpdateResourceGroups: MsgType
 CreateDatabase: MsgType
 DropDatabase: MsgType
 ListDatabases: MsgType
+AlterDatabase: MsgType
+DescribeDatabase: MsgType
 Dsl: DslType
 BoolExprV1: DslType
 UndefiedState: CompactionState
 Executing: CompactionState
 Completed: CompactionState
 Strong: ConsistencyLevel
 Session: ConsistencyLevel
@@ -556,14 +561,15 @@
 PrivilegeGetFlushState: ObjectPrivilege
 PrivilegeCreateAlias: ObjectPrivilege
 PrivilegeDropAlias: ObjectPrivilege
 PrivilegeDescribeAlias: ObjectPrivilege
 PrivilegeListAliases: ObjectPrivilege
 PrivilegeUpdateResourceGroups: ObjectPrivilege
 PrivilegeAlterDatabase: ObjectPrivilege
+PrivilegeDescribeDatabase: ObjectPrivilege
 Initializing: StateCode
 Healthy: StateCode
 Abnormal: StateCode
 StandBy: StateCode
 Stopping: StateCode
 LoadStateNotExist: LoadState
 LoadStateNotLoad: LoadState
```

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/feder_pb2.py` & `pymilvus-2.4.2/pymilvus/grpc_gen/feder_pb2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/feder_pb2.pyi` & `pymilvus-2.4.2/pymilvus/grpc_gen/feder_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2.py` & `pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from . import rg_pb2 as rg__pb2
 from . import schema_pb2 as schema__pb2
 from . import feder_pb2 as feder__pb2
 from . import msg_pb2 as msg__pb2
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cmilvus.proto\x12\x13milvus.proto.milvus\x1a\x0c\x63ommon.proto\x1a\x08rg.proto\x1a\x0cschema.proto\x1a\x0b\x66\x65\x64\x65r.proto\x1a\tmsg.proto\x1a google/protobuf/descriptor.proto\"\x8d\x01\n\x12\x43reateAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\r\n\x05\x61lias\x18\x04 \x01(\t:\x12\xca>\x0f\x08\x01\x10,\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"r\n\x10\x44ropAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10-\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x8c\x01\n\x11\x41lterAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\r\n\x05\x61lias\x18\x04 \x01(\t:\x12\xca>\x0f\x08\x01\x10,\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"v\n\x14\x44\x65scribeAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10.\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"x\n\x15\x44\x65scribeAliasResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t\x12\x12\n\ncollection\x18\x04 \x01(\t\"~\n\x12ListAliasesRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10/\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"}\n\x13ListAliasesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0f\n\x07\x61liases\x18\x04 \x03(\t\"\xb8\x02\n\x17\x43reateCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\x0c\x12\x12\n\nshards_num\x18\x05 \x01(\x05\x12@\n\x11\x63onsistency_level\x18\x06 \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x35\n\nproperties\x18\x07 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x16\n\x0enum_partitions\x18\x08 \x01(\x03:\x12\xca>\x0f\x08\x01\x10\x01\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x81\x01\n\x15\x44ropCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x02\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xcf\x01\n\x16\x41lterCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x35\n\nproperties\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x12\xca>\x0f\x08\x01\x10\x01\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x80\x01\n\x14HasCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\ntime_stamp\x18\x04 \x01(\x04\"J\n\x0c\x42oolResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05value\x18\x02 \x01(\x08\"L\n\x0eStringResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05value\x18\x02 \x01(\t\"\xaf\x01\n\x19\x44\x65scribeCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x12\n\ntime_stamp\x18\x05 \x01(\x04:\x12\xca>\x0f\x08\x01\x10\x03\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xb9\x04\n\x1a\x44\x65scribeCollectionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x35\n\x06schema\x18\x02 \x01(\x0b\x32%.milvus.proto.schema.CollectionSchema\x12\x14\n\x0c\x63ollectionID\x18\x03 \x01(\x03\x12\x1d\n\x15virtual_channel_names\x18\x04 \x03(\t\x12\x1e\n\x16physical_channel_names\x18\x05 \x03(\t\x12\x19\n\x11\x63reated_timestamp\x18\x06 \x01(\x04\x12\x1d\n\x15\x63reated_utc_timestamp\x18\x07 \x01(\x04\x12\x12\n\nshards_num\x18\x08 \x01(\x05\x12\x0f\n\x07\x61liases\x18\t \x03(\t\x12\x39\n\x0fstart_positions\x18\n \x03(\x0b\x32 .milvus.proto.common.KeyDataPair\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x17\n\x0f\x63ollection_name\x18\x0c \x01(\t\x12\x35\n\nproperties\x18\r \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x0f\n\x07\x64\x62_name\x18\x0e \x01(\t\x12\x16\n\x0enum_partitions\x18\x0f \x01(\x03\x12\r\n\x05\x64\x62_id\x18\x10 \x01(\x03\"\xb8\x01\n\x15LoadCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0ereplica_number\x18\x04 \x01(\x05\x12\x17\n\x0fresource_groups\x18\x05 \x03(\t\x12\x0f\n\x07refresh\x18\x06 \x01(\x08:\x07\xca>\x04\x10\x05\x18\x03\"y\n\x18ReleaseCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\x06\x18\x03\"\xab\x01\n\x14GetStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x1b\n\x13guarantee_timestamp\x18\x05 \x01(\x04:\x07\xca>\x04\x10\n\x18\x03\"v\n\x15GetStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\x7f\n\x1eGetCollectionStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\n\x18\x03\"\x80\x01\n\x1fGetCollectionStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb4\x01\n\x16ShowCollectionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x12\n\ntime_stamp\x18\x03 \x01(\x04\x12+\n\x04type\x18\x04 \x01(\x0e\x32\x1d.milvus.proto.milvus.ShowType\x12\x1c\n\x10\x63ollection_names\x18\x05 \x03(\tB\x02\x18\x01\"\xf7\x01\n\x17ShowCollectionsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x18\n\x10\x63ollection_names\x18\x02 \x03(\t\x12\x16\n\x0e\x63ollection_ids\x18\x03 \x03(\x03\x12\x1a\n\x12\x63reated_timestamps\x18\x04 \x03(\x04\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x03(\x04\x12 \n\x14inMemory_percentages\x18\x06 \x03(\x03\x42\x02\x18\x01\x12\x1f\n\x17query_service_available\x18\x07 \x03(\x08\"\x8f\x01\n\x16\x43reatePartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\'\x18\x03\"\x8d\x01\n\x14\x44ropPartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10(\x18\x03\"\x8c\x01\n\x13HasPartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10*\x18\x03\"\xd1\x01\n\x15LoadPartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x16\n\x0ereplica_number\x18\x05 \x01(\x05\x12\x17\n\x0fresource_groups\x18\x06 \x03(\t\x12\x0f\n\x07refresh\x18\x07 \x01(\x08:\x07\xca>\x04\x10\x05\x18\x03\"\x92\x01\n\x18ReleasePartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t:\x07\xca>\x04\x10\x06\x18\x03\"\x8d\x01\n\x1dGetPartitionStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\"\x7f\n\x1eGetPartitionStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xd6\x01\n\x15ShowPartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x17\n\x0fpartition_names\x18\x05 \x03(\t\x12/\n\x04type\x18\x06 \x01(\x0e\x32\x1d.milvus.proto.milvus.ShowTypeB\x02\x18\x01:\x07\xca>\x04\x10)\x18\x03\"\xd2\x01\n\x16ShowPartitionsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x17\n\x0fpartition_names\x18\x02 \x03(\t\x12\x14\n\x0cpartitionIDs\x18\x03 \x03(\x03\x12\x1a\n\x12\x63reated_timestamps\x18\x04 \x03(\x04\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x03(\x04\x12 \n\x14inMemory_percentages\x18\x06 \x03(\x03\x42\x02\x18\x01\"m\n\x16\x44\x65scribeSegmentRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x11\n\tsegmentID\x18\x03 \x01(\x03\"\x8f\x01\n\x17\x44\x65scribeSegmentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07indexID\x18\x02 \x01(\x03\x12\x0f\n\x07\x62uildID\x18\x03 \x01(\x03\x12\x14\n\x0c\x65nable_index\x18\x04 \x01(\x08\x12\x0f\n\x07\x66ieldID\x18\x05 \x01(\x03\"l\n\x13ShowSegmentsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\"W\n\x14ShowSegmentsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x12\n\nsegmentIDs\x18\x02 \x03(\x03\"\xd4\x01\n\x12\x43reateIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x37\n\x0c\x65xtra_params\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x12\n\nindex_name\x18\x06 \x01(\t:\x07\xca>\x04\x10\x0b\x18\x03\"\xbf\x01\n\x11\x41lterIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x37\n\x0c\x65xtra_params\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x07\xca>\x04\x10\x0b\x18\x03\"\xb0\x01\n\x14\x44\x65scribeIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\x04:\x07\xca>\x04\x10\x0c\x18\x03\"\x95\x02\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07indexID\x18\x02 \x01(\x03\x12\x31\n\x06params\x18\x03 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x14\n\x0cindexed_rows\x18\x05 \x01(\x03\x12\x12\n\ntotal_rows\x18\x06 \x01(\x03\x12.\n\x05state\x18\x07 \x01(\x0e\x32\x1f.milvus.proto.common.IndexState\x12\x1f\n\x17index_state_fail_reason\x18\x08 \x01(\t\x12\x1a\n\x12pending_index_rows\x18\t \x01(\x03\"\x87\x01\n\x15\x44\x65scribeIndexResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x41\n\x12index_descriptions\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.IndexDescription\"\xa5\x01\n\x1cGetIndexBuildProgressRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\x0c\x18\x03\"v\n\x1dGetIndexBuildProgressResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0cindexed_rows\x18\x02 \x01(\x03\x12\x12\n\ntotal_rows\x18\x03 \x01(\x03\"\x9d\x01\n\x14GetIndexStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\x0c\x18\x03\"\x89\x01\n\x15GetIndexStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12.\n\x05state\x18\x02 \x01(\x0e\x32\x1f.milvus.proto.common.IndexState\x12\x13\n\x0b\x66\x61il_reason\x18\x03 \x01(\t\"\x99\x01\n\x10\x44ropIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\r\x18\x03\"\xe0\x01\n\rInsertRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x33\n\x0b\x66ields_data\x18\x05 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12\x10\n\x08num_rows\x18\x07 \x01(\r:\x07\xca>\x04\x10\x08\x18\x03\"\xe0\x01\n\rUpsertRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x33\n\x0b\x66ields_data\x18\x05 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12\x10\n\x08num_rows\x18\x07 \x01(\r:\x07\xca>\x04\x10\x19\x18\x03\"\xf0\x01\n\x0eMutationResult\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12%\n\x03IDs\x18\x02 \x01(\x0b\x32\x18.milvus.proto.schema.IDs\x12\x12\n\nsucc_index\x18\x03 \x03(\r\x12\x11\n\terr_index\x18\x04 \x03(\r\x12\x14\n\x0c\x61\x63knowledged\x18\x05 \x01(\x08\x12\x12\n\ninsert_cnt\x18\x06 \x01(\x03\x12\x12\n\ndelete_cnt\x18\x07 \x01(\x03\x12\x12\n\nupsert_cnt\x18\x08 \x01(\x03\x12\x11\n\ttimestamp\x18\t \x01(\x04\"\xe9\x01\n\rDeleteRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x05 \x01(\t\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12@\n\x11\x63onsistency_level\x18\x07 \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel:\x07\xca>\x04\x10\t\x18\x03\"\xb0\x01\n\x10SubSearchRequest\x12\x0b\n\x03\x64sl\x18\x01 \x01(\t\x12\x19\n\x11placeholder_group\x18\x02 \x01(\x0c\x12.\n\x08\x64sl_type\x18\x03 \x01(\x0e\x32\x1c.milvus.proto.common.DslType\x12\x38\n\rsearch_params\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\n\n\x02nq\x18\x05 \x01(\x03\"\xcc\x04\n\rSearchRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x0b\n\x03\x64sl\x18\x05 \x01(\t\x12\x19\n\x11placeholder_group\x18\x06 \x01(\x0c\x12.\n\x08\x64sl_type\x18\x07 \x01(\x0e\x32\x1c.milvus.proto.common.DslType\x12\x15\n\routput_fields\x18\x08 \x03(\t\x12\x38\n\rsearch_params\x18\t \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x18\n\x10travel_timestamp\x18\n \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x0b \x01(\x04\x12\n\n\x02nq\x18\x0c \x01(\x03\x12\x1b\n\x13not_return_all_meta\x18\r \x01(\x08\x12@\n\x11\x63onsistency_level\x18\x0e \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0f \x01(\x08\x12\x1e\n\x16search_by_primary_keys\x18\x10 \x01(\x08\x12\x37\n\x08sub_reqs\x18\x11 \x03(\x0b\x32%.milvus.proto.milvus.SubSearchRequest:\x07\xca>\x04\x10\x0e\x18\x03\"5\n\x04Hits\x12\x0b\n\x03IDs\x18\x01 \x03(\x03\x12\x10\n\x08row_data\x18\x02 \x03(\x0c\x12\x0e\n\x06scores\x18\x03 \x03(\x02\"\x8d\x01\n\rSearchResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x36\n\x07results\x18\x02 \x01(\x0b\x32%.milvus.proto.schema.SearchResultData\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\"\xc9\x03\n\x13HybridSearchRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x34\n\x08requests\x18\x05 \x03(\x0b\x32\".milvus.proto.milvus.SearchRequest\x12\x36\n\x0brank_params\x18\x06 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x18\n\x10travel_timestamp\x18\x07 \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x08 \x01(\x04\x12\x1b\n\x13not_return_all_meta\x18\t \x01(\x08\x12\x15\n\routput_fields\x18\n \x03(\t\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0c \x01(\x08:\x07\xca>\x04\x10\x0e\x18\x03\"n\n\x0c\x46lushRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t:\x07\xca>\x04\x10\x0f \x03\"\x9b\x05\n\rFlushResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12G\n\x0b\x63oll_segIDs\x18\x03 \x03(\x0b\x32\x32.milvus.proto.milvus.FlushResponse.CollSegIDsEntry\x12R\n\x11\x66lush_coll_segIDs\x18\x04 \x03(\x0b\x32\x37.milvus.proto.milvus.FlushResponse.FlushCollSegIDsEntry\x12N\n\x0f\x63oll_seal_times\x18\x05 \x03(\x0b\x32\x35.milvus.proto.milvus.FlushResponse.CollSealTimesEntry\x12J\n\rcoll_flush_ts\x18\x06 \x03(\x0b\x32\x33.milvus.proto.milvus.FlushResponse.CollFlushTsEntry\x1aQ\n\x0f\x43ollSegIDsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.milvus.proto.schema.LongArray:\x02\x38\x01\x1aV\n\x14\x46lushCollSegIDsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.milvus.proto.schema.LongArray:\x02\x38\x01\x1a\x34\n\x12\x43ollSealTimesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\x1a\x32\n\x10\x43ollFlushTsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\"\x9b\x03\n\x0cQueryRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x04 \x01(\t\x12\x15\n\routput_fields\x18\x05 \x03(\t\x12\x17\n\x0fpartition_names\x18\x06 \x03(\t\x12\x18\n\x10travel_timestamp\x18\x07 \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x08 \x01(\x04\x12\x37\n\x0cquery_params\x18\t \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x1b\n\x13not_return_all_meta\x18\n \x01(\x08\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0c \x01(\x08:\x07\xca>\x04\x10\x10\x18\x03\"\xa0\x01\n\x0cQueryResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x0b\x66ields_data\x18\x02 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x15\n\routput_fields\x18\x04 \x03(\t\"}\n\tVectorIDs\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12*\n\x08id_array\x18\x03 \x01(\x0b\x32\x18.milvus.proto.schema.IDs\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\"\x83\x01\n\x0cVectorsArray\x12\x32\n\x08id_array\x18\x01 \x01(\x0b\x32\x1e.milvus.proto.milvus.VectorIDsH\x00\x12\x36\n\ndata_array\x18\x02 \x01(\x0b\x32 .milvus.proto.schema.VectorFieldH\x00\x42\x07\n\x05\x61rray\"\xdd\x01\n\x13\x43\x61lcDistanceRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x32\n\x07op_left\x18\x02 \x01(\x0b\x32!.milvus.proto.milvus.VectorsArray\x12\x33\n\x08op_right\x18\x03 \x01(\x0b\x32!.milvus.proto.milvus.VectorsArray\x12\x31\n\x06params\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb5\x01\n\x13\x43\x61lcDistanceResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x31\n\x08int_dist\x18\x02 \x01(\x0b\x32\x1d.milvus.proto.schema.IntArrayH\x00\x12\x35\n\nfloat_dist\x18\x03 \x01(\x0b\x32\x1f.milvus.proto.schema.FloatArrayH\x00\x42\x07\n\x05\x61rray\"b\n\x0f\x46lushAllRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10&\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"U\n\x10\x46lushAllResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0c\x66lush_all_ts\x18\x02 \x01(\x04\"\x99\x01\n\x15PersistentSegmentInfo\x12\x11\n\tsegmentID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\x12\x10\n\x08num_rows\x18\x04 \x01(\x03\x12\x30\n\x05state\x18\x05 \x01(\x0e\x32!.milvus.proto.common.SegmentState\"u\n\x1fGetPersistentSegmentInfoRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0e\n\x06\x64\x62Name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ollectionName\x18\x03 \x01(\t\"\x8a\x01\n GetPersistentSegmentInfoResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x39\n\x05infos\x18\x02 \x03(\x0b\x32*.milvus.proto.milvus.PersistentSegmentInfo\"\xf0\x01\n\x10QuerySegmentInfo\x12\x11\n\tsegmentID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\x12\x10\n\x08mem_size\x18\x04 \x01(\x03\x12\x10\n\x08num_rows\x18\x05 \x01(\x03\x12\x12\n\nindex_name\x18\x06 \x01(\t\x12\x0f\n\x07indexID\x18\x07 \x01(\x03\x12\x12\n\x06nodeID\x18\x08 \x01(\x03\x42\x02\x18\x01\x12\x30\n\x05state\x18\t \x01(\x0e\x32!.milvus.proto.common.SegmentState\x12\x0f\n\x07nodeIds\x18\n \x03(\x03\"p\n\x1aGetQuerySegmentInfoRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0e\n\x06\x64\x62Name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ollectionName\x18\x03 \x01(\t\"\x80\x01\n\x1bGetQuerySegmentInfoResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x34\n\x05infos\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.QuerySegmentInfo\"$\n\x0c\x44ummyRequest\x12\x14\n\x0crequest_type\x18\x01 \x01(\t\"!\n\rDummyResponse\x12\x10\n\x08response\x18\x01 \x01(\t\"\x15\n\x13RegisterLinkRequest\"r\n\x14RegisterLinkResponse\x12-\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.Address\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.milvus.proto.common.Status\"P\n\x11GetMetricsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07request\x18\x02 \x01(\t\"k\n\x12GetMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08response\x18\x02 \x01(\t\x12\x16\n\x0e\x63omponent_name\x18\x03 \x01(\t\"\x98\x01\n\rComponentInfo\x12\x0e\n\x06nodeID\x18\x01 \x01(\x03\x12\x0c\n\x04role\x18\x02 \x01(\t\x12\x32\n\nstate_code\x18\x03 \x01(\x0e\x32\x1e.milvus.proto.common.StateCode\x12\x35\n\nextra_info\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb2\x01\n\x0f\x43omponentStates\x12\x31\n\x05state\x18\x01 \x01(\x0b\x32\".milvus.proto.milvus.ComponentInfo\x12?\n\x13subcomponent_states\x18\x02 \x03(\x0b\x32\".milvus.proto.milvus.ComponentInfo\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.milvus.proto.common.Status\"\x1b\n\x19GetComponentStatesRequest\"\xb6\x01\n\x12LoadBalanceRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x12\n\nsrc_nodeID\x18\x02 \x01(\x03\x12\x13\n\x0b\x64st_nodeIDs\x18\x03 \x03(\x03\x12\x19\n\x11sealed_segmentIDs\x18\x04 \x03(\x03\x12\x16\n\x0e\x63ollectionName\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x06 \x01(\t:\x07\xca>\x04\x10\x11\x18\x05\"e\n\x17ManualCompactionRequest\x12\x14\n\x0c\x63ollectionID\x18\x01 \x01(\x03\x12\x12\n\ntimetravel\x18\x02 \x01(\x04\x12\x17\n\x0fmajorCompaction\x18\x03 \x01(\x08:\x07\xca>\x04\x10\x07\x18\x01\"z\n\x18ManualCompactionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0c\x63ompactionID\x18\x02 \x01(\x03\x12\x1b\n\x13\x63ompactionPlanCount\x18\x03 \x01(\x05\"1\n\x19GetCompactionStateRequest\x12\x14\n\x0c\x63ompactionID\x18\x01 \x01(\x03\"\xdd\x01\n\x1aGetCompactionStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x05state\x18\x02 \x01(\x0e\x32$.milvus.proto.common.CompactionState\x12\x17\n\x0f\x65xecutingPlanNo\x18\x03 \x01(\x03\x12\x15\n\rtimeoutPlanNo\x18\x04 \x01(\x03\x12\x17\n\x0f\x63ompletedPlanNo\x18\x05 \x01(\x03\x12\x14\n\x0c\x66\x61iledPlanNo\x18\x06 \x01(\x03\"1\n\x19GetCompactionPlansRequest\x12\x14\n\x0c\x63ompactionID\x18\x01 \x01(\x03\"\xbc\x01\n\x1aGetCompactionPlansResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x05state\x18\x02 \x01(\x0e\x32$.milvus.proto.common.CompactionState\x12<\n\nmergeInfos\x18\x03 \x03(\x0b\x32(.milvus.proto.milvus.CompactionMergeInfo\"6\n\x13\x43ompactionMergeInfo\x12\x0f\n\x07sources\x18\x01 \x03(\x03\x12\x0e\n\x06target\x18\x02 \x01(\x03\"o\n\x14GetFlushStateRequest\x12\x12\n\nsegmentIDs\x18\x01 \x03(\x03\x12\x10\n\x08\x66lush_ts\x18\x02 \x01(\x04\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t:\x07\xca>\x04\x10+\x18\x04\"U\n\x15GetFlushStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x66lushed\x18\x02 \x01(\x08\"l\n\x17GetFlushAllStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x66lush_all_ts\x18\x02 \x01(\x04\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\"X\n\x18GetFlushAllStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x66lushed\x18\x02 \x01(\x08\"\xe0\x01\n\rImportRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x16\n\x0epartition_name\x18\x02 \x01(\t\x12\x15\n\rchannel_names\x18\x03 \x03(\t\x12\x11\n\trow_based\x18\x04 \x01(\x08\x12\r\n\x05\x66iles\x18\x05 \x03(\t\x12\x32\n\x07options\x18\x06 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x0f\n\x07\x64\x62_name\x18\x07 \x01(\t\x12\x17\n\x0f\x63lustering_info\x18\x08 \x01(\x0c:\x07\xca>\x04\x10\x12\x18\x01\"L\n\x0eImportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05tasks\x18\x02 \x03(\x03\"%\n\x15GetImportStateRequest\x12\x0c\n\x04task\x18\x01 \x01(\x03\"\x97\x02\n\x16GetImportStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12/\n\x05state\x18\x02 \x01(\x0e\x32 .milvus.proto.common.ImportState\x12\x11\n\trow_count\x18\x03 \x01(\x03\x12\x0f\n\x07id_list\x18\x04 \x03(\x03\x12\x30\n\x05infos\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\n\n\x02id\x18\x06 \x01(\x03\x12\x15\n\rcollection_id\x18\x07 \x01(\x03\x12\x13\n\x0bsegment_ids\x18\x08 \x03(\x03\x12\x11\n\tcreate_ts\x18\t \x01(\x03\"Q\n\x16ListImportTasksRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\"\x82\x01\n\x17ListImportTasksResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12:\n\x05tasks\x18\x02 \x03(\x0b\x32+.milvus.proto.milvus.GetImportStateResponse\"\x9a\x01\n\x12GetReplicasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x18\n\x10with_shard_nodes\x18\x03 \x01(\x08\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x05 \x01(\t\"v\n\x13GetReplicasResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x32\n\x08replicas\x18\x02 \x03(\x0b\x32 .milvus.proto.milvus.ReplicaInfo\"\xc1\x02\n\x0bReplicaInfo\x12\x11\n\treplicaID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x15\n\rpartition_ids\x18\x03 \x03(\x03\x12\x39\n\x0eshard_replicas\x18\x04 \x03(\x0b\x32!.milvus.proto.milvus.ShardReplica\x12\x10\n\x08node_ids\x18\x05 \x03(\x03\x12\x1b\n\x13resource_group_name\x18\x06 \x01(\t\x12P\n\x11num_outbound_node\x18\x07 \x03(\x0b\x32\x35.milvus.proto.milvus.ReplicaInfo.NumOutboundNodeEntry\x1a\x36\n\x14NumOutboundNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"`\n\x0cShardReplica\x12\x10\n\x08leaderID\x18\x01 \x01(\x03\x12\x13\n\x0bleader_addr\x18\x02 \x01(\t\x12\x17\n\x0f\x64m_channel_name\x18\x03 \x01(\t\x12\x10\n\x08node_ids\x18\x04 \x03(\x03\"\xbe\x01\n\x17\x43reateCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x04 \x01(\x04\x12\x1f\n\x17modified_utc_timestamps\x18\x05 \x01(\x04:\x12\xca>\x0f\x08\x01\x10\x13\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xcd\x01\n\x17UpdateCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x13\n\x0boldPassword\x18\x03 \x01(\t\x12\x13\n\x0bnewPassword\x18\x04 \x01(\t\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x01(\x04\x12\x1f\n\x17modified_utc_timestamps\x18\x06 \x01(\x04:\t\xca>\x06\x08\x02\x10\x14\x18\x02\"k\n\x17\x44\x65leteCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x15\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"W\n\x15ListCredUsersResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\tusernames\x18\x02 \x03(\t\"V\n\x14ListCredUsersRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x1a\n\nRoleEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1a\n\nUserEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x01\n\x11\x43reateRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12/\n\x06\x65ntity\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity:\x12\xca>\x0f\x08\x01\x10\x13\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"d\n\x0f\x44ropRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x11\n\trole_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x15\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xb5\x01\n\x16OperateUserRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x11\n\trole_name\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.milvus.proto.milvus.OperateUserRoleType:\x12\xca>\x0f\x08\x01\x10\x17\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x9d\x01\n\x11SelectRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12-\n\x04role\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12\x19\n\x11include_user_info\x18\x03 \x01(\x08:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"k\n\nRoleResult\x12-\n\x04role\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12.\n\x05users\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\"s\n\x12SelectRoleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x07results\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.RoleResult\"\x94\x01\n\x11SelectUserRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12-\n\x04user\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12\x19\n\x11include_role_info\x18\x03 \x01(\x08:\t\xca>\x06\x08\x02\x10\x18\x18\x02\"k\n\nUserResult\x12-\n\x04user\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12.\n\x05roles\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\"s\n\x12SelectUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x07results\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.UserResult\"\x1c\n\x0cObjectEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1f\n\x0fPrivilegeEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"w\n\rGrantorEntity\x12-\n\x04user\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12\x37\n\tprivilege\x18\x02 \x01(\x0b\x32$.milvus.proto.milvus.PrivilegeEntity\"L\n\x14GrantPrivilegeEntity\x12\x34\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\".milvus.proto.milvus.GrantorEntity\"\xca\x01\n\x0bGrantEntity\x12-\n\x04role\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12\x31\n\x06object\x18\x02 \x01(\x0b\x32!.milvus.proto.milvus.ObjectEntity\x12\x13\n\x0bobject_name\x18\x03 \x01(\t\x12\x33\n\x07grantor\x18\x04 \x01(\x0b\x32\".milvus.proto.milvus.GrantorEntity\x12\x0f\n\x07\x64\x62_name\x18\x05 \x01(\t\"\x86\x01\n\x12SelectGrantRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x30\n\x06\x65ntity\x18\x02 \x01(\x0b\x32 .milvus.proto.milvus.GrantEntity:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"v\n\x13SelectGrantResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x32\n\x08\x65ntities\x18\x02 \x03(\x0b\x32 .milvus.proto.milvus.GrantEntity\"\xc4\x01\n\x17OperatePrivilegeRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x30\n\x06\x65ntity\x18\x02 \x01(\x0b\x32 .milvus.proto.milvus.GrantEntity\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).milvus.proto.milvus.OperatePrivilegeType:\x12\xca>\x0f\x08\x01\x10\x17\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x93\x01\n\x19GetLoadingProgressRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x17\n\x0fpartition_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64\x62_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\x05\x18\x02\"u\n\x1aGetLoadingProgressResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08progress\x18\x02 \x01(\x03\x12\x18\n\x10refresh_progress\x18\x03 \x01(\x03\"\x8d\x01\n\x13GetLoadStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x17\n\x0fpartition_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64\x62_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\x05\x18\x02\"r\n\x14GetLoadStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12-\n\x05state\x18\x02 \x01(\x0e\x32\x1e.milvus.proto.common.LoadState\"\x1c\n\tMilvusExt\x12\x0f\n\x07version\x18\x01 \x01(\t\"\x13\n\x11GetVersionRequest\"R\n\x12GetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x14\n\x12\x43heckHealthRequest\"\x9d\x01\n\x13\x43heckHealthResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\tisHealthy\x18\x02 \x01(\x08\x12\x0f\n\x07reasons\x18\x03 \x03(\t\x12\x35\n\x0cquota_states\x18\x04 \x03(\x0e\x32\x1f.milvus.proto.milvus.QuotaState\"\xaa\x01\n\x1a\x43reateResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t\x12\x34\n\x06\x63onfig\x18\x03 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig:\x12\xca>\x0f\x08\x01\x10\x1a\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x99\x02\n\x1bUpdateResourceGroupsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12]\n\x0fresource_groups\x18\x02 \x03(\x0b\x32\x44.milvus.proto.milvus.UpdateResourceGroupsRequest.ResourceGroupsEntry\x1a[\n\x13ResourceGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig:\x02\x38\x01:\x12\xca>\x0f\x08\x01\x10\x30\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"r\n\x18\x44ropResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1b\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xa5\x01\n\x13TransferNodeRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x1d\n\x15source_resource_group\x18\x02 \x01(\t\x12\x1d\n\x15target_resource_group\x18\x03 \x01(\t\x12\x10\n\x08num_node\x18\x04 \x01(\x05:\x12\xca>\x0f\x08\x01\x10\x1e\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xd5\x01\n\x16TransferReplicaRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x1d\n\x15source_resource_group\x18\x02 \x01(\t\x12\x1d\n\x15target_resource_group\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t\x12\x13\n\x0bnum_replica\x18\x05 \x01(\x03\x12\x0f\n\x07\x64\x62_name\x18\x06 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1f\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"[\n\x19ListResourceGroupsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10\x1d\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"b\n\x1aListResourceGroupsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x17\n\x0fresource_groups\x18\x02 \x03(\t\"v\n\x1c\x44\x65scribeResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1c\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x88\x01\n\x1d\x44\x65scribeResourceGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12:\n\x0eresource_group\x18\x02 \x01(\x0b\x32\".milvus.proto.milvus.ResourceGroup\"\xd6\x04\n\rResourceGroup\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61pacity\x18\x02 \x01(\x05\x12\x1a\n\x12num_available_node\x18\x03 \x01(\x05\x12T\n\x12num_loaded_replica\x18\x04 \x03(\x0b\x32\x38.milvus.proto.milvus.ResourceGroup.NumLoadedReplicaEntry\x12R\n\x11num_outgoing_node\x18\x05 \x03(\x0b\x32\x37.milvus.proto.milvus.ResourceGroup.NumOutgoingNodeEntry\x12R\n\x11num_incoming_node\x18\x06 \x03(\x0b\x32\x37.milvus.proto.milvus.ResourceGroup.NumIncomingNodeEntry\x12\x34\n\x06\x63onfig\x18\x07 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig\x12,\n\x05nodes\x18\x08 \x03(\x0b\x32\x1d.milvus.proto.common.NodeInfo\x1a\x37\n\x15NumLoadedReplicaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x36\n\x14NumOutgoingNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x36\n\x14NumIncomingNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x9f\x01\n\x17RenameCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x0f\n\x07oldName\x18\x03 \x01(\t\x12\x0f\n\x07newName\x18\x04 \x01(\t\x12\x11\n\tnewDBName\x18\x05 \x01(\t:\x12\xca>\x0f\x08\x01\x10\"\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xa1\x01\n\x19GetIndexStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x11\n\ttimestamp\x18\x05 \x01(\x04:\x07\xca>\x04\x10\x0c\x18\x03\"\x8c\x01\n\x1aGetIndexStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x41\n\x12index_descriptions\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.IndexDescription\"r\n\x0e\x43onnectRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x34\n\x0b\x63lient_info\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.common.ClientInfo\"\x88\x01\n\x0f\x43onnectResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x34\n\x0bserver_info\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.common.ServerInfo\x12\x12\n\nidentifier\x18\x03 \x01(\x03\"C\n\x15\x41llocTimestampRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"X\n\x16\x41llocTimestampResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\ttimestamp\x18\x02 \x01(\x04\"h\n\x15\x43reateDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10#\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"f\n\x13\x44ropDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10$\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"B\n\x14ListDatabasesRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"q\n\x15ListDatabasesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08\x64\x62_names\x18\x02 \x03(\t\x12\x19\n\x11\x63reated_timestamp\x18\x03 \x03(\x04\"\xad\x01\n\x14\x41lterDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x64\x62_id\x18\x03 \x01(\t\x12\x35\n\nproperties\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x12\xca>\x0f\x08\x01\x10\x31\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xf5\x01\n\x17ReplicateMessageRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x0f\n\x07\x42\x65ginTs\x18\x03 \x01(\x04\x12\r\n\x05\x45ndTs\x18\x04 \x01(\x04\x12\x0c\n\x04Msgs\x18\x05 \x03(\x0c\x12\x35\n\x0eStartPositions\x18\x06 \x03(\x0b\x32\x1d.milvus.proto.msg.MsgPosition\x12\x33\n\x0c\x45ndPositions\x18\x07 \x03(\x0b\x32\x1d.milvus.proto.msg.MsgPosition\"Y\n\x18ReplicateMessageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08position\x18\x02 \x01(\t\"b\n\x15ImportAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x16\n\x0epartition_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01\"<\n GetImportProgressAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01\"O\n\x1aListImportsAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01*%\n\x08ShowType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08InMemory\x10\x01\x1a\x02\x18\x01*@\n\x13OperateUserRoleType\x12\x11\n\rAddUserToRole\x10\x00\x12\x16\n\x12RemoveUserFromRole\x10\x01*-\n\x14OperatePrivilegeType\x12\t\n\x05Grant\x10\x00\x12\n\n\x06Revoke\x10\x01*]\n\nQuotaState\x12\x0b\n\x07Unknown\x10\x00\x12\x0f\n\x0bReadLimited\x10\x02\x12\x10\n\x0cWriteLimited\x10\x03\x12\x0e\n\nDenyToRead\x10\x04\x12\x0f\n\x0b\x44\x65nyToWrite\x10\x05\x32\xc7\x43\n\rMilvusService\x12_\n\x10\x43reateCollection\x12,.milvus.proto.milvus.CreateCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12[\n\x0e\x44ropCollection\x12*.milvus.proto.milvus.DropCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\rHasCollection\x12).milvus.proto.milvus.HasCollectionRequest\x1a!.milvus.proto.milvus.BoolResponse\"\x00\x12[\n\x0eLoadCollection\x12*.milvus.proto.milvus.LoadCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11ReleaseCollection\x12-.milvus.proto.milvus.ReleaseCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12\x44\x65scribeCollection\x12..milvus.proto.milvus.DescribeCollectionRequest\x1a/.milvus.proto.milvus.DescribeCollectionResponse\"\x00\x12\x86\x01\n\x17GetCollectionStatistics\x12\x33.milvus.proto.milvus.GetCollectionStatisticsRequest\x1a\x34.milvus.proto.milvus.GetCollectionStatisticsResponse\"\x00\x12n\n\x0fShowCollections\x12+.milvus.proto.milvus.ShowCollectionsRequest\x1a,.milvus.proto.milvus.ShowCollectionsResponse\"\x00\x12]\n\x0f\x41lterCollection\x12+.milvus.proto.milvus.AlterCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0f\x43reatePartition\x12+.milvus.proto.milvus.CreatePartitionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12Y\n\rDropPartition\x12).milvus.proto.milvus.DropPartitionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0cHasPartition\x12(.milvus.proto.milvus.HasPartitionRequest\x1a!.milvus.proto.milvus.BoolResponse\"\x00\x12[\n\x0eLoadPartitions\x12*.milvus.proto.milvus.LoadPartitionsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11ReleasePartitions\x12-.milvus.proto.milvus.ReleasePartitionsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x83\x01\n\x16GetPartitionStatistics\x12\x32.milvus.proto.milvus.GetPartitionStatisticsRequest\x1a\x33.milvus.proto.milvus.GetPartitionStatisticsResponse\"\x00\x12k\n\x0eShowPartitions\x12*.milvus.proto.milvus.ShowPartitionsRequest\x1a+.milvus.proto.milvus.ShowPartitionsResponse\"\x00\x12w\n\x12GetLoadingProgress\x12..milvus.proto.milvus.GetLoadingProgressRequest\x1a/.milvus.proto.milvus.GetLoadingProgressResponse\"\x00\x12\x65\n\x0cGetLoadState\x12(.milvus.proto.milvus.GetLoadStateRequest\x1a).milvus.proto.milvus.GetLoadStateResponse\"\x00\x12U\n\x0b\x43reateAlias\x12\'.milvus.proto.milvus.CreateAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12Q\n\tDropAlias\x12%.milvus.proto.milvus.DropAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\nAlterAlias\x12&.milvus.proto.milvus.AlterAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rDescribeAlias\x12).milvus.proto.milvus.DescribeAliasRequest\x1a*.milvus.proto.milvus.DescribeAliasResponse\"\x00\x12\x62\n\x0bListAliases\x12\'.milvus.proto.milvus.ListAliasesRequest\x1a(.milvus.proto.milvus.ListAliasesResponse\"\x00\x12U\n\x0b\x43reateIndex\x12\'.milvus.proto.milvus.CreateIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\nAlterIndex\x12&.milvus.proto.milvus.AlterIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rDescribeIndex\x12).milvus.proto.milvus.DescribeIndexRequest\x1a*.milvus.proto.milvus.DescribeIndexResponse\"\x00\x12w\n\x12GetIndexStatistics\x12..milvus.proto.milvus.GetIndexStatisticsRequest\x1a/.milvus.proto.milvus.GetIndexStatisticsResponse\"\x00\x12k\n\rGetIndexState\x12).milvus.proto.milvus.GetIndexStateRequest\x1a*.milvus.proto.milvus.GetIndexStateResponse\"\x03\x88\x02\x01\x12\x83\x01\n\x15GetIndexBuildProgress\x12\x31.milvus.proto.milvus.GetIndexBuildProgressRequest\x1a\x32.milvus.proto.milvus.GetIndexBuildProgressResponse\"\x03\x88\x02\x01\x12Q\n\tDropIndex\x12%.milvus.proto.milvus.DropIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\x06Insert\x12\".milvus.proto.milvus.InsertRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12S\n\x06\x44\x65lete\x12\".milvus.proto.milvus.DeleteRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12S\n\x06Upsert\x12\".milvus.proto.milvus.UpsertRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12R\n\x06Search\x12\".milvus.proto.milvus.SearchRequest\x1a\".milvus.proto.milvus.SearchResults\"\x00\x12^\n\x0cHybridSearch\x12(.milvus.proto.milvus.HybridSearchRequest\x1a\".milvus.proto.milvus.SearchResults\"\x00\x12P\n\x05\x46lush\x12!.milvus.proto.milvus.FlushRequest\x1a\".milvus.proto.milvus.FlushResponse\"\x00\x12O\n\x05Query\x12!.milvus.proto.milvus.QueryRequest\x1a!.milvus.proto.milvus.QueryResults\"\x00\x12\x64\n\x0c\x43\x61lcDistance\x12(.milvus.proto.milvus.CalcDistanceRequest\x1a(.milvus.proto.milvus.CalcDistanceResults\"\x00\x12Y\n\x08\x46lushAll\x12$.milvus.proto.milvus.FlushAllRequest\x1a%.milvus.proto.milvus.FlushAllResponse\"\x00\x12h\n\rGetFlushState\x12).milvus.proto.milvus.GetFlushStateRequest\x1a*.milvus.proto.milvus.GetFlushStateResponse\"\x00\x12q\n\x10GetFlushAllState\x12,.milvus.proto.milvus.GetFlushAllStateRequest\x1a-.milvus.proto.milvus.GetFlushAllStateResponse\"\x00\x12\x89\x01\n\x18GetPersistentSegmentInfo\x12\x34.milvus.proto.milvus.GetPersistentSegmentInfoRequest\x1a\x35.milvus.proto.milvus.GetPersistentSegmentInfoResponse\"\x00\x12z\n\x13GetQuerySegmentInfo\x12/.milvus.proto.milvus.GetQuerySegmentInfoRequest\x1a\x30.milvus.proto.milvus.GetQuerySegmentInfoResponse\"\x00\x12\x62\n\x0bGetReplicas\x12\'.milvus.proto.milvus.GetReplicasRequest\x1a(.milvus.proto.milvus.GetReplicasResponse\"\x00\x12P\n\x05\x44ummy\x12!.milvus.proto.milvus.DummyRequest\x1a\".milvus.proto.milvus.DummyResponse\"\x00\x12\x65\n\x0cRegisterLink\x12(.milvus.proto.milvus.RegisterLinkRequest\x1a).milvus.proto.milvus.RegisterLinkResponse\"\x00\x12_\n\nGetMetrics\x12&.milvus.proto.milvus.GetMetricsRequest\x1a\'.milvus.proto.milvus.GetMetricsResponse\"\x00\x12l\n\x12GetComponentStates\x12..milvus.proto.milvus.GetComponentStatesRequest\x1a$.milvus.proto.milvus.ComponentStates\"\x00\x12U\n\x0bLoadBalance\x12\'.milvus.proto.milvus.LoadBalanceRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12GetCompactionState\x12..milvus.proto.milvus.GetCompactionStateRequest\x1a/.milvus.proto.milvus.GetCompactionStateResponse\"\x00\x12q\n\x10ManualCompaction\x12,.milvus.proto.milvus.ManualCompactionRequest\x1a-.milvus.proto.milvus.ManualCompactionResponse\"\x00\x12\x80\x01\n\x1bGetCompactionStateWithPlans\x12..milvus.proto.milvus.GetCompactionPlansRequest\x1a/.milvus.proto.milvus.GetCompactionPlansResponse\"\x00\x12S\n\x06Import\x12\".milvus.proto.milvus.ImportRequest\x1a#.milvus.proto.milvus.ImportResponse\"\x00\x12k\n\x0eGetImportState\x12*.milvus.proto.milvus.GetImportStateRequest\x1a+.milvus.proto.milvus.GetImportStateResponse\"\x00\x12n\n\x0fListImportTasks\x12+.milvus.proto.milvus.ListImportTasksRequest\x1a,.milvus.proto.milvus.ListImportTasksResponse\"\x00\x12_\n\x10\x43reateCredential\x12,.milvus.proto.milvus.CreateCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\x10UpdateCredential\x12,.milvus.proto.milvus.UpdateCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\x10\x44\x65leteCredential\x12,.milvus.proto.milvus.DeleteCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rListCredUsers\x12).milvus.proto.milvus.ListCredUsersRequest\x1a*.milvus.proto.milvus.ListCredUsersResponse\"\x00\x12S\n\nCreateRole\x12&.milvus.proto.milvus.CreateRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12O\n\x08\x44ropRole\x12$.milvus.proto.milvus.DropRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0fOperateUserRole\x12+.milvus.proto.milvus.OperateUserRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\nSelectRole\x12&.milvus.proto.milvus.SelectRoleRequest\x1a\'.milvus.proto.milvus.SelectRoleResponse\"\x00\x12_\n\nSelectUser\x12&.milvus.proto.milvus.SelectUserRequest\x1a\'.milvus.proto.milvus.SelectUserResponse\"\x00\x12_\n\x10OperatePrivilege\x12,.milvus.proto.milvus.OperatePrivilegeRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x62\n\x0bSelectGrant\x12\'.milvus.proto.milvus.SelectGrantRequest\x1a(.milvus.proto.milvus.SelectGrantResponse\"\x00\x12_\n\nGetVersion\x12&.milvus.proto.milvus.GetVersionRequest\x1a\'.milvus.proto.milvus.GetVersionResponse\"\x00\x12\x62\n\x0b\x43heckHealth\x12\'.milvus.proto.milvus.CheckHealthRequest\x1a(.milvus.proto.milvus.CheckHealthResponse\"\x00\x12\x65\n\x13\x43reateResourceGroup\x12/.milvus.proto.milvus.CreateResourceGroupRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11\x44ropResourceGroup\x12-.milvus.proto.milvus.DropResourceGroupRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12g\n\x14UpdateResourceGroups\x12\x30.milvus.proto.milvus.UpdateResourceGroupsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12W\n\x0cTransferNode\x12(.milvus.proto.milvus.TransferNodeRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0fTransferReplica\x12+.milvus.proto.milvus.TransferReplicaRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12ListResourceGroups\x12..milvus.proto.milvus.ListResourceGroupsRequest\x1a/.milvus.proto.milvus.ListResourceGroupsResponse\"\x00\x12\x80\x01\n\x15\x44\x65scribeResourceGroup\x12\x31.milvus.proto.milvus.DescribeResourceGroupRequest\x1a\x32.milvus.proto.milvus.DescribeResourceGroupResponse\"\x00\x12_\n\x10RenameCollection\x12,.milvus.proto.milvus.RenameCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12u\n\x12ListIndexedSegment\x12-.milvus.proto.feder.ListIndexedSegmentRequest\x1a..milvus.proto.feder.ListIndexedSegmentResponse\"\x00\x12\x87\x01\n\x18\x44\x65scribeSegmentIndexData\x12\x33.milvus.proto.feder.DescribeSegmentIndexDataRequest\x1a\x34.milvus.proto.feder.DescribeSegmentIndexDataResponse\"\x00\x12V\n\x07\x43onnect\x12#.milvus.proto.milvus.ConnectRequest\x1a$.milvus.proto.milvus.ConnectResponse\"\x00\x12k\n\x0e\x41llocTimestamp\x12*.milvus.proto.milvus.AllocTimestampRequest\x1a+.milvus.proto.milvus.AllocTimestampResponse\"\x00\x12[\n\x0e\x43reateDatabase\x12*.milvus.proto.milvus.CreateDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12W\n\x0c\x44ropDatabase\x12(.milvus.proto.milvus.DropDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rListDatabases\x12).milvus.proto.milvus.ListDatabasesRequest\x1a*.milvus.proto.milvus.ListDatabasesResponse\"\x00\x12Y\n\rAlterDatabase\x12).milvus.proto.milvus.AlterDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12q\n\x10ReplicateMessage\x12,.milvus.proto.milvus.ReplicateMessageRequest\x1a-.milvus.proto.milvus.ReplicateMessageResponse\"\x00\x32u\n\x0cProxyService\x12\x65\n\x0cRegisterLink\x12(.milvus.proto.milvus.RegisterLinkRequest\x1a).milvus.proto.milvus.RegisterLinkResponse\"\x00:U\n\x0emilvus_ext_obj\x12\x1c.google.protobuf.FileOptions\x18\xe9\x07 \x01(\x0b\x32\x1e.milvus.proto.milvus.MilvusExtBm\n\x0eio.milvus.grpcB\x0bMilvusProtoP\x01Z4github.com/milvus-io/milvus-proto/go-api/v2/milvuspb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cmilvus.proto\x12\x13milvus.proto.milvus\x1a\x0c\x63ommon.proto\x1a\x08rg.proto\x1a\x0cschema.proto\x1a\x0b\x66\x65\x64\x65r.proto\x1a\tmsg.proto\x1a google/protobuf/descriptor.proto\"\x8d\x01\n\x12\x43reateAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\r\n\x05\x61lias\x18\x04 \x01(\t:\x12\xca>\x0f\x08\x01\x10,\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"r\n\x10\x44ropAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10-\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x8c\x01\n\x11\x41lterAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\r\n\x05\x61lias\x18\x04 \x01(\t:\x12\xca>\x0f\x08\x01\x10,\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"v\n\x14\x44\x65scribeAliasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10.\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"x\n\x15\x44\x65scribeAliasResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x61lias\x18\x03 \x01(\t\x12\x12\n\ncollection\x18\x04 \x01(\t\"~\n\x12ListAliasesRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10/\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"}\n\x13ListAliasesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0f\n\x07\x61liases\x18\x04 \x03(\t\"\xb8\x02\n\x17\x43reateCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0e\n\x06schema\x18\x04 \x01(\x0c\x12\x12\n\nshards_num\x18\x05 \x01(\x05\x12@\n\x11\x63onsistency_level\x18\x06 \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x35\n\nproperties\x18\x07 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x16\n\x0enum_partitions\x18\x08 \x01(\x03:\x12\xca>\x0f\x08\x01\x10\x01\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x81\x01\n\x15\x44ropCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x02\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xcf\x01\n\x16\x41lterCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x35\n\nproperties\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x12\xca>\x0f\x08\x01\x10\x01\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x80\x01\n\x14HasCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\ntime_stamp\x18\x04 \x01(\x04\"J\n\x0c\x42oolResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05value\x18\x02 \x01(\x08\"L\n\x0eStringResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05value\x18\x02 \x01(\t\"\xaf\x01\n\x19\x44\x65scribeCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x12\n\ntime_stamp\x18\x05 \x01(\x04:\x12\xca>\x0f\x08\x01\x10\x03\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xb9\x04\n\x1a\x44\x65scribeCollectionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x35\n\x06schema\x18\x02 \x01(\x0b\x32%.milvus.proto.schema.CollectionSchema\x12\x14\n\x0c\x63ollectionID\x18\x03 \x01(\x03\x12\x1d\n\x15virtual_channel_names\x18\x04 \x03(\t\x12\x1e\n\x16physical_channel_names\x18\x05 \x03(\t\x12\x19\n\x11\x63reated_timestamp\x18\x06 \x01(\x04\x12\x1d\n\x15\x63reated_utc_timestamp\x18\x07 \x01(\x04\x12\x12\n\nshards_num\x18\x08 \x01(\x05\x12\x0f\n\x07\x61liases\x18\t \x03(\t\x12\x39\n\x0fstart_positions\x18\n \x03(\x0b\x32 .milvus.proto.common.KeyDataPair\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x17\n\x0f\x63ollection_name\x18\x0c \x01(\t\x12\x35\n\nproperties\x18\r \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x0f\n\x07\x64\x62_name\x18\x0e \x01(\t\x12\x16\n\x0enum_partitions\x18\x0f \x01(\x03\x12\r\n\x05\x64\x62_id\x18\x10 \x01(\x03\"\xb8\x01\n\x15LoadCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0ereplica_number\x18\x04 \x01(\x05\x12\x17\n\x0fresource_groups\x18\x05 \x03(\t\x12\x0f\n\x07refresh\x18\x06 \x01(\x08:\x07\xca>\x04\x10\x05\x18\x03\"y\n\x18ReleaseCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\x06\x18\x03\"\xab\x01\n\x14GetStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x1b\n\x13guarantee_timestamp\x18\x05 \x01(\x04:\x07\xca>\x04\x10\n\x18\x03\"v\n\x15GetStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\x7f\n\x1eGetCollectionStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\n\x18\x03\"\x80\x01\n\x1fGetCollectionStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb4\x01\n\x16ShowCollectionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x12\n\ntime_stamp\x18\x03 \x01(\x04\x12+\n\x04type\x18\x04 \x01(\x0e\x32\x1d.milvus.proto.milvus.ShowType\x12\x1c\n\x10\x63ollection_names\x18\x05 \x03(\tB\x02\x18\x01\"\xf7\x01\n\x17ShowCollectionsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x18\n\x10\x63ollection_names\x18\x02 \x03(\t\x12\x16\n\x0e\x63ollection_ids\x18\x03 \x03(\x03\x12\x1a\n\x12\x63reated_timestamps\x18\x04 \x03(\x04\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x03(\x04\x12 \n\x14inMemory_percentages\x18\x06 \x03(\x03\x42\x02\x18\x01\x12\x1f\n\x17query_service_available\x18\x07 \x03(\x08\"\x8f\x01\n\x16\x43reatePartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\'\x18\x03\"\x8d\x01\n\x14\x44ropPartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10(\x18\x03\"\x8c\x01\n\x13HasPartitionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t:\x07\xca>\x04\x10*\x18\x03\"\xd1\x01\n\x15LoadPartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x16\n\x0ereplica_number\x18\x05 \x01(\x05\x12\x17\n\x0fresource_groups\x18\x06 \x03(\t\x12\x0f\n\x07refresh\x18\x07 \x01(\x08:\x07\xca>\x04\x10\x05\x18\x03\"\x92\x01\n\x18ReleasePartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t:\x07\xca>\x04\x10\x06\x18\x03\"\x8d\x01\n\x1dGetPartitionStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\"\x7f\n\x1eGetPartitionStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x05stats\x18\x02 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xd6\x01\n\x15ShowPartitionsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x14\n\x0c\x63ollectionID\x18\x04 \x01(\x03\x12\x17\n\x0fpartition_names\x18\x05 \x03(\t\x12/\n\x04type\x18\x06 \x01(\x0e\x32\x1d.milvus.proto.milvus.ShowTypeB\x02\x18\x01:\x07\xca>\x04\x10)\x18\x03\"\xd2\x01\n\x16ShowPartitionsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x17\n\x0fpartition_names\x18\x02 \x03(\t\x12\x14\n\x0cpartitionIDs\x18\x03 \x03(\x03\x12\x1a\n\x12\x63reated_timestamps\x18\x04 \x03(\x04\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x03(\x04\x12 \n\x14inMemory_percentages\x18\x06 \x03(\x03\x42\x02\x18\x01\"m\n\x16\x44\x65scribeSegmentRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x11\n\tsegmentID\x18\x03 \x01(\x03\"\x8f\x01\n\x17\x44\x65scribeSegmentResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07indexID\x18\x02 \x01(\x03\x12\x0f\n\x07\x62uildID\x18\x03 \x01(\x03\x12\x14\n\x0c\x65nable_index\x18\x04 \x01(\x08\x12\x0f\n\x07\x66ieldID\x18\x05 \x01(\x03\"l\n\x13ShowSegmentsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\"W\n\x14ShowSegmentsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x12\n\nsegmentIDs\x18\x02 \x03(\x03\"\xd4\x01\n\x12\x43reateIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x37\n\x0c\x65xtra_params\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x12\n\nindex_name\x18\x06 \x01(\t:\x07\xca>\x04\x10\x0b\x18\x03\"\xbf\x01\n\x11\x41lterIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x37\n\x0c\x65xtra_params\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x07\xca>\x04\x10\x0b\x18\x03\"\xb0\x01\n\x14\x44\x65scribeIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t\x12\x11\n\ttimestamp\x18\x06 \x01(\x04:\x07\xca>\x04\x10\x0c\x18\x03\"\x95\x02\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07indexID\x18\x02 \x01(\x03\x12\x31\n\x06params\x18\x03 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x14\n\x0cindexed_rows\x18\x05 \x01(\x03\x12\x12\n\ntotal_rows\x18\x06 \x01(\x03\x12.\n\x05state\x18\x07 \x01(\x0e\x32\x1f.milvus.proto.common.IndexState\x12\x1f\n\x17index_state_fail_reason\x18\x08 \x01(\t\x12\x1a\n\x12pending_index_rows\x18\t \x01(\x03\"\x87\x01\n\x15\x44\x65scribeIndexResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x41\n\x12index_descriptions\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.IndexDescription\"\xa5\x01\n\x1cGetIndexBuildProgressRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\x0c\x18\x03\"v\n\x1dGetIndexBuildProgressResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0cindexed_rows\x18\x02 \x01(\x03\x12\x12\n\ntotal_rows\x18\x03 \x01(\x03\"\x9d\x01\n\x14GetIndexStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\x0c\x18\x03\"\x89\x01\n\x15GetIndexStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12.\n\x05state\x18\x02 \x01(\x0e\x32\x1f.milvus.proto.common.IndexState\x12\x13\n\x0b\x66\x61il_reason\x18\x03 \x01(\t\"\x99\x01\n\x10\x44ropIndexRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nfield_name\x18\x04 \x01(\t\x12\x12\n\nindex_name\x18\x05 \x01(\t:\x07\xca>\x04\x10\r\x18\x03\"\xe0\x01\n\rInsertRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x33\n\x0b\x66ields_data\x18\x05 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12\x10\n\x08num_rows\x18\x07 \x01(\r:\x07\xca>\x04\x10\x08\x18\x03\"\xe0\x01\n\rUpsertRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x33\n\x0b\x66ields_data\x18\x05 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12\x10\n\x08num_rows\x18\x07 \x01(\r:\x07\xca>\x04\x10\x19\x18\x03\"\xf0\x01\n\x0eMutationResult\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12%\n\x03IDs\x18\x02 \x01(\x0b\x32\x18.milvus.proto.schema.IDs\x12\x12\n\nsucc_index\x18\x03 \x03(\r\x12\x11\n\terr_index\x18\x04 \x03(\r\x12\x14\n\x0c\x61\x63knowledged\x18\x05 \x01(\x08\x12\x12\n\ninsert_cnt\x18\x06 \x01(\x03\x12\x12\n\ndelete_cnt\x18\x07 \x01(\x03\x12\x12\n\nupsert_cnt\x18\x08 \x01(\x03\x12\x11\n\ttimestamp\x18\t \x01(\x04\"\xe9\x01\n\rDeleteRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x16\n\x0epartition_name\x18\x04 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x05 \x01(\t\x12\x11\n\thash_keys\x18\x06 \x03(\r\x12@\n\x11\x63onsistency_level\x18\x07 \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel:\x07\xca>\x04\x10\t\x18\x03\"\xb0\x01\n\x10SubSearchRequest\x12\x0b\n\x03\x64sl\x18\x01 \x01(\t\x12\x19\n\x11placeholder_group\x18\x02 \x01(\x0c\x12.\n\x08\x64sl_type\x18\x03 \x01(\x0e\x32\x1c.milvus.proto.common.DslType\x12\x38\n\rsearch_params\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\n\n\x02nq\x18\x05 \x01(\x03\"\xcc\x04\n\rSearchRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x0b\n\x03\x64sl\x18\x05 \x01(\t\x12\x19\n\x11placeholder_group\x18\x06 \x01(\x0c\x12.\n\x08\x64sl_type\x18\x07 \x01(\x0e\x32\x1c.milvus.proto.common.DslType\x12\x15\n\routput_fields\x18\x08 \x03(\t\x12\x38\n\rsearch_params\x18\t \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x18\n\x10travel_timestamp\x18\n \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x0b \x01(\x04\x12\n\n\x02nq\x18\x0c \x01(\x03\x12\x1b\n\x13not_return_all_meta\x18\r \x01(\x08\x12@\n\x11\x63onsistency_level\x18\x0e \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0f \x01(\x08\x12\x1e\n\x16search_by_primary_keys\x18\x10 \x01(\x08\x12\x37\n\x08sub_reqs\x18\x11 \x03(\x0b\x32%.milvus.proto.milvus.SubSearchRequest:\x07\xca>\x04\x10\x0e\x18\x03\"5\n\x04Hits\x12\x0b\n\x03IDs\x18\x01 \x03(\x03\x12\x10\n\x08row_data\x18\x02 \x03(\x0c\x12\x0e\n\x06scores\x18\x03 \x03(\x02\"\x8d\x01\n\rSearchResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x36\n\x07results\x18\x02 \x01(\x0b\x32%.milvus.proto.schema.SearchResultData\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\"\xc9\x03\n\x13HybridSearchRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\x12\x34\n\x08requests\x18\x05 \x03(\x0b\x32\".milvus.proto.milvus.SearchRequest\x12\x36\n\x0brank_params\x18\x06 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x18\n\x10travel_timestamp\x18\x07 \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x08 \x01(\x04\x12\x1b\n\x13not_return_all_meta\x18\t \x01(\x08\x12\x15\n\routput_fields\x18\n \x03(\t\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0c \x01(\x08:\x07\xca>\x04\x10\x0e\x18\x03\"n\n\x0c\x46lushRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t:\x07\xca>\x04\x10\x0f \x03\"\xb6\x06\n\rFlushResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12G\n\x0b\x63oll_segIDs\x18\x03 \x03(\x0b\x32\x32.milvus.proto.milvus.FlushResponse.CollSegIDsEntry\x12R\n\x11\x66lush_coll_segIDs\x18\x04 \x03(\x0b\x32\x37.milvus.proto.milvus.FlushResponse.FlushCollSegIDsEntry\x12N\n\x0f\x63oll_seal_times\x18\x05 \x03(\x0b\x32\x35.milvus.proto.milvus.FlushResponse.CollSealTimesEntry\x12J\n\rcoll_flush_ts\x18\x06 \x03(\x0b\x32\x33.milvus.proto.milvus.FlushResponse.CollFlushTsEntry\x12G\n\x0b\x63hannel_cps\x18\x07 \x03(\x0b\x32\x32.milvus.proto.milvus.FlushResponse.ChannelCpsEntry\x1aQ\n\x0f\x43ollSegIDsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.milvus.proto.schema.LongArray:\x02\x38\x01\x1aV\n\x14\x46lushCollSegIDsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.milvus.proto.schema.LongArray:\x02\x38\x01\x1a\x34\n\x12\x43ollSealTimesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\x1a\x32\n\x10\x43ollFlushTsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\x1aP\n\x0f\x43hannelCpsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.milvus.proto.msg.MsgPosition:\x02\x38\x01\"\x9b\x03\n\x0cQueryRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x0c\n\x04\x65xpr\x18\x04 \x01(\t\x12\x15\n\routput_fields\x18\x05 \x03(\t\x12\x17\n\x0fpartition_names\x18\x06 \x03(\t\x12\x18\n\x10travel_timestamp\x18\x07 \x01(\x04\x12\x1b\n\x13guarantee_timestamp\x18\x08 \x01(\x04\x12\x37\n\x0cquery_params\x18\t \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x1b\n\x13not_return_all_meta\x18\n \x01(\x08\x12@\n\x11\x63onsistency_level\x18\x0b \x01(\x0e\x32%.milvus.proto.common.ConsistencyLevel\x12\x1f\n\x17use_default_consistency\x18\x0c \x01(\x08:\x07\xca>\x04\x10\x10\x18\x03\"\xa0\x01\n\x0cQueryResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x0b\x66ields_data\x18\x02 \x03(\x0b\x32\x1e.milvus.proto.schema.FieldData\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x15\n\routput_fields\x18\x04 \x03(\t\"}\n\tVectorIDs\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12*\n\x08id_array\x18\x03 \x01(\x0b\x32\x18.milvus.proto.schema.IDs\x12\x17\n\x0fpartition_names\x18\x04 \x03(\t\"\x83\x01\n\x0cVectorsArray\x12\x32\n\x08id_array\x18\x01 \x01(\x0b\x32\x1e.milvus.proto.milvus.VectorIDsH\x00\x12\x36\n\ndata_array\x18\x02 \x01(\x0b\x32 .milvus.proto.schema.VectorFieldH\x00\x42\x07\n\x05\x61rray\"\xdd\x01\n\x13\x43\x61lcDistanceRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x32\n\x07op_left\x18\x02 \x01(\x0b\x32!.milvus.proto.milvus.VectorsArray\x12\x33\n\x08op_right\x18\x03 \x01(\x0b\x32!.milvus.proto.milvus.VectorsArray\x12\x31\n\x06params\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb5\x01\n\x13\x43\x61lcDistanceResults\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x31\n\x08int_dist\x18\x02 \x01(\x0b\x32\x1d.milvus.proto.schema.IntArrayH\x00\x12\x35\n\nfloat_dist\x18\x03 \x01(\x0b\x32\x1f.milvus.proto.schema.FloatArrayH\x00\x42\x07\n\x05\x61rray\"b\n\x0f\x46lushAllRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10&\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"U\n\x10\x46lushAllResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0c\x66lush_all_ts\x18\x02 \x01(\x04\"\x99\x01\n\x15PersistentSegmentInfo\x12\x11\n\tsegmentID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\x12\x10\n\x08num_rows\x18\x04 \x01(\x03\x12\x30\n\x05state\x18\x05 \x01(\x0e\x32!.milvus.proto.common.SegmentState\"u\n\x1fGetPersistentSegmentInfoRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0e\n\x06\x64\x62Name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ollectionName\x18\x03 \x01(\t\"\x8a\x01\n GetPersistentSegmentInfoResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x39\n\x05infos\x18\x02 \x03(\x0b\x32*.milvus.proto.milvus.PersistentSegmentInfo\"\xf0\x01\n\x10QuerySegmentInfo\x12\x11\n\tsegmentID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x13\n\x0bpartitionID\x18\x03 \x01(\x03\x12\x10\n\x08mem_size\x18\x04 \x01(\x03\x12\x10\n\x08num_rows\x18\x05 \x01(\x03\x12\x12\n\nindex_name\x18\x06 \x01(\t\x12\x0f\n\x07indexID\x18\x07 \x01(\x03\x12\x12\n\x06nodeID\x18\x08 \x01(\x03\x42\x02\x18\x01\x12\x30\n\x05state\x18\t \x01(\x0e\x32!.milvus.proto.common.SegmentState\x12\x0f\n\x07nodeIds\x18\n \x03(\x03\"p\n\x1aGetQuerySegmentInfoRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0e\n\x06\x64\x62Name\x18\x02 \x01(\t\x12\x16\n\x0e\x63ollectionName\x18\x03 \x01(\t\"\x80\x01\n\x1bGetQuerySegmentInfoResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x34\n\x05infos\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.QuerySegmentInfo\"$\n\x0c\x44ummyRequest\x12\x14\n\x0crequest_type\x18\x01 \x01(\t\"!\n\rDummyResponse\x12\x10\n\x08response\x18\x01 \x01(\t\"\x15\n\x13RegisterLinkRequest\"r\n\x14RegisterLinkResponse\x12-\n\x07\x61\x64\x64ress\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.Address\x12+\n\x06status\x18\x02 \x01(\x0b\x32\x1b.milvus.proto.common.Status\"P\n\x11GetMetricsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07request\x18\x02 \x01(\t\"k\n\x12GetMetricsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08response\x18\x02 \x01(\t\x12\x16\n\x0e\x63omponent_name\x18\x03 \x01(\t\"\x98\x01\n\rComponentInfo\x12\x0e\n\x06nodeID\x18\x01 \x01(\x03\x12\x0c\n\x04role\x18\x02 \x01(\t\x12\x32\n\nstate_code\x18\x03 \x01(\x0e\x32\x1e.milvus.proto.common.StateCode\x12\x35\n\nextra_info\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xb2\x01\n\x0f\x43omponentStates\x12\x31\n\x05state\x18\x01 \x01(\x0b\x32\".milvus.proto.milvus.ComponentInfo\x12?\n\x13subcomponent_states\x18\x02 \x03(\x0b\x32\".milvus.proto.milvus.ComponentInfo\x12+\n\x06status\x18\x03 \x01(\x0b\x32\x1b.milvus.proto.common.Status\"\x1b\n\x19GetComponentStatesRequest\"\xb6\x01\n\x12LoadBalanceRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x12\n\nsrc_nodeID\x18\x02 \x01(\x03\x12\x13\n\x0b\x64st_nodeIDs\x18\x03 \x03(\x03\x12\x19\n\x11sealed_segmentIDs\x18\x04 \x03(\x03\x12\x16\n\x0e\x63ollectionName\x18\x05 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x06 \x01(\t:\x07\xca>\x04\x10\x11\x18\x05\"e\n\x17ManualCompactionRequest\x12\x14\n\x0c\x63ollectionID\x18\x01 \x01(\x03\x12\x12\n\ntimetravel\x18\x02 \x01(\x04\x12\x17\n\x0fmajorCompaction\x18\x03 \x01(\x08:\x07\xca>\x04\x10\x07\x18\x01\"z\n\x18ManualCompactionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x14\n\x0c\x63ompactionID\x18\x02 \x01(\x03\x12\x1b\n\x13\x63ompactionPlanCount\x18\x03 \x01(\x05\"1\n\x19GetCompactionStateRequest\x12\x14\n\x0c\x63ompactionID\x18\x01 \x01(\x03\"\xdd\x01\n\x1aGetCompactionStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x05state\x18\x02 \x01(\x0e\x32$.milvus.proto.common.CompactionState\x12\x17\n\x0f\x65xecutingPlanNo\x18\x03 \x01(\x03\x12\x15\n\rtimeoutPlanNo\x18\x04 \x01(\x03\x12\x17\n\x0f\x63ompletedPlanNo\x18\x05 \x01(\x03\x12\x14\n\x0c\x66\x61iledPlanNo\x18\x06 \x01(\x03\"1\n\x19GetCompactionPlansRequest\x12\x14\n\x0c\x63ompactionID\x18\x01 \x01(\x03\"\xbc\x01\n\x1aGetCompactionPlansResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x33\n\x05state\x18\x02 \x01(\x0e\x32$.milvus.proto.common.CompactionState\x12<\n\nmergeInfos\x18\x03 \x03(\x0b\x32(.milvus.proto.milvus.CompactionMergeInfo\"6\n\x13\x43ompactionMergeInfo\x12\x0f\n\x07sources\x18\x01 \x03(\x03\x12\x0e\n\x06target\x18\x02 \x01(\x03\"o\n\x14GetFlushStateRequest\x12\x12\n\nsegmentIDs\x18\x01 \x03(\x03\x12\x10\n\x08\x66lush_ts\x18\x02 \x01(\x04\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t:\x07\xca>\x04\x10+\x18\x04\"U\n\x15GetFlushStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x66lushed\x18\x02 \x01(\x08\"l\n\x17GetFlushAllStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x66lush_all_ts\x18\x02 \x01(\x04\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\"X\n\x18GetFlushAllStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x66lushed\x18\x02 \x01(\x08\"\xe0\x01\n\rImportRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x16\n\x0epartition_name\x18\x02 \x01(\t\x12\x15\n\rchannel_names\x18\x03 \x03(\t\x12\x11\n\trow_based\x18\x04 \x01(\x08\x12\r\n\x05\x66iles\x18\x05 \x03(\t\x12\x32\n\x07options\x18\x06 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\x0f\n\x07\x64\x62_name\x18\x07 \x01(\t\x12\x17\n\x0f\x63lustering_info\x18\x08 \x01(\x0c:\x07\xca>\x04\x10\x12\x18\x01\"L\n\x0eImportResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\r\n\x05tasks\x18\x02 \x03(\x03\"%\n\x15GetImportStateRequest\x12\x0c\n\x04task\x18\x01 \x01(\x03\"\x97\x02\n\x16GetImportStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12/\n\x05state\x18\x02 \x01(\x0e\x32 .milvus.proto.common.ImportState\x12\x11\n\trow_count\x18\x03 \x01(\x03\x12\x0f\n\x07id_list\x18\x04 \x03(\x03\x12\x30\n\x05infos\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\x12\n\n\x02id\x18\x06 \x01(\x03\x12\x15\n\rcollection_id\x18\x07 \x01(\x03\x12\x13\n\x0bsegment_ids\x18\x08 \x03(\x03\x12\x11\n\tcreate_ts\x18\t \x01(\x03\"Q\n\x16ListImportTasksRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\"\x82\x01\n\x17ListImportTasksResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12:\n\x05tasks\x18\x02 \x03(\x0b\x32+.milvus.proto.milvus.GetImportStateResponse\"\x9a\x01\n\x12GetReplicasRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x18\n\x10with_shard_nodes\x18\x03 \x01(\x08\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x62_name\x18\x05 \x01(\t\"v\n\x13GetReplicasResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x32\n\x08replicas\x18\x02 \x03(\x0b\x32 .milvus.proto.milvus.ReplicaInfo\"\xc1\x02\n\x0bReplicaInfo\x12\x11\n\treplicaID\x18\x01 \x01(\x03\x12\x14\n\x0c\x63ollectionID\x18\x02 \x01(\x03\x12\x15\n\rpartition_ids\x18\x03 \x03(\x03\x12\x39\n\x0eshard_replicas\x18\x04 \x03(\x0b\x32!.milvus.proto.milvus.ShardReplica\x12\x10\n\x08node_ids\x18\x05 \x03(\x03\x12\x1b\n\x13resource_group_name\x18\x06 \x01(\t\x12P\n\x11num_outbound_node\x18\x07 \x03(\x0b\x32\x35.milvus.proto.milvus.ReplicaInfo.NumOutboundNodeEntry\x1a\x36\n\x14NumOutboundNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"`\n\x0cShardReplica\x12\x10\n\x08leaderID\x18\x01 \x01(\x03\x12\x13\n\x0bleader_addr\x18\x02 \x01(\t\x12\x17\n\x0f\x64m_channel_name\x18\x03 \x01(\t\x12\x10\n\x08node_ids\x18\x04 \x03(\x03\"\xbe\x01\n\x17\x43reateCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x04 \x01(\x04\x12\x1f\n\x17modified_utc_timestamps\x18\x05 \x01(\x04:\x12\xca>\x0f\x08\x01\x10\x13\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xcd\x01\n\x17UpdateCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x13\n\x0boldPassword\x18\x03 \x01(\t\x12\x13\n\x0bnewPassword\x18\x04 \x01(\t\x12\x1e\n\x16\x63reated_utc_timestamps\x18\x05 \x01(\x04\x12\x1f\n\x17modified_utc_timestamps\x18\x06 \x01(\x04:\t\xca>\x06\x08\x02\x10\x14\x18\x02\"k\n\x17\x44\x65leteCredentialRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x15\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"W\n\x15ListCredUsersResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\tusernames\x18\x02 \x03(\t\"V\n\x14ListCredUsersRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x1a\n\nRoleEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1a\n\nUserEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x84\x01\n\x11\x43reateRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12/\n\x06\x65ntity\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity:\x12\xca>\x0f\x08\x01\x10\x13\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"d\n\x0f\x44ropRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x11\n\trole_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x15\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xb5\x01\n\x16OperateUserRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x11\n\trole_name\x18\x03 \x01(\t\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.milvus.proto.milvus.OperateUserRoleType:\x12\xca>\x0f\x08\x01\x10\x17\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x9d\x01\n\x11SelectRoleRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12-\n\x04role\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12\x19\n\x11include_user_info\x18\x03 \x01(\x08:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"k\n\nRoleResult\x12-\n\x04role\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12.\n\x05users\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\"s\n\x12SelectRoleResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x07results\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.RoleResult\"\x94\x01\n\x11SelectUserRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12-\n\x04user\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12\x19\n\x11include_role_info\x18\x03 \x01(\x08:\t\xca>\x06\x08\x02\x10\x18\x18\x02\"k\n\nUserResult\x12-\n\x04user\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12.\n\x05roles\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\"s\n\x12SelectUserResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x30\n\x07results\x18\x02 \x03(\x0b\x32\x1f.milvus.proto.milvus.UserResult\"\x1c\n\x0cObjectEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1f\n\x0fPrivilegeEntity\x12\x0c\n\x04name\x18\x01 \x01(\t\"w\n\rGrantorEntity\x12-\n\x04user\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.UserEntity\x12\x37\n\tprivilege\x18\x02 \x01(\x0b\x32$.milvus.proto.milvus.PrivilegeEntity\"L\n\x14GrantPrivilegeEntity\x12\x34\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\".milvus.proto.milvus.GrantorEntity\"\xca\x01\n\x0bGrantEntity\x12-\n\x04role\x18\x01 \x01(\x0b\x32\x1f.milvus.proto.milvus.RoleEntity\x12\x31\n\x06object\x18\x02 \x01(\x0b\x32!.milvus.proto.milvus.ObjectEntity\x12\x13\n\x0bobject_name\x18\x03 \x01(\t\x12\x33\n\x07grantor\x18\x04 \x01(\x0b\x32\".milvus.proto.milvus.GrantorEntity\x12\x0f\n\x07\x64\x62_name\x18\x05 \x01(\t\"\x86\x01\n\x12SelectGrantRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x30\n\x06\x65ntity\x18\x02 \x01(\x0b\x32 .milvus.proto.milvus.GrantEntity:\x12\xca>\x0f\x08\x01\x10\x16\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"v\n\x13SelectGrantResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x32\n\x08\x65ntities\x18\x02 \x03(\x0b\x32 .milvus.proto.milvus.GrantEntity\"\xc4\x01\n\x17OperatePrivilegeRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x30\n\x06\x65ntity\x18\x02 \x01(\x0b\x32 .milvus.proto.milvus.GrantEntity\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).milvus.proto.milvus.OperatePrivilegeType:\x12\xca>\x0f\x08\x01\x10\x17\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x93\x01\n\x19GetLoadingProgressRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x17\n\x0fpartition_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64\x62_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\x05\x18\x02\"u\n\x1aGetLoadingProgressResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08progress\x18\x02 \x01(\x03\x12\x18\n\x10refresh_progress\x18\x03 \x01(\x03\"\x8d\x01\n\x13GetLoadStateRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x17\n\x0fpartition_names\x18\x03 \x03(\t\x12\x0f\n\x07\x64\x62_name\x18\x04 \x01(\t:\x07\xca>\x04\x10\x05\x18\x02\"r\n\x14GetLoadStateResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12-\n\x05state\x18\x02 \x01(\x0e\x32\x1e.milvus.proto.common.LoadState\"\x1c\n\tMilvusExt\x12\x0f\n\x07version\x18\x01 \x01(\t\"\x13\n\x11GetVersionRequest\"R\n\x12GetVersionResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07version\x18\x02 \x01(\t\"\x14\n\x12\x43heckHealthRequest\"\x9d\x01\n\x13\x43heckHealthResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\tisHealthy\x18\x02 \x01(\x08\x12\x0f\n\x07reasons\x18\x03 \x03(\t\x12\x35\n\x0cquota_states\x18\x04 \x03(\x0e\x32\x1f.milvus.proto.milvus.QuotaState\"\xaa\x01\n\x1a\x43reateResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t\x12\x34\n\x06\x63onfig\x18\x03 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig:\x12\xca>\x0f\x08\x01\x10\x1a\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x99\x02\n\x1bUpdateResourceGroupsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12]\n\x0fresource_groups\x18\x02 \x03(\x0b\x32\x44.milvus.proto.milvus.UpdateResourceGroupsRequest.ResourceGroupsEntry\x1a[\n\x13ResourceGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig:\x02\x38\x01:\x12\xca>\x0f\x08\x01\x10\x30\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"r\n\x18\x44ropResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1b\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xa5\x01\n\x13TransferNodeRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x1d\n\x15source_resource_group\x18\x02 \x01(\t\x12\x1d\n\x15target_resource_group\x18\x03 \x01(\t\x12\x10\n\x08num_node\x18\x04 \x01(\x05:\x12\xca>\x0f\x08\x01\x10\x1e\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xd5\x01\n\x16TransferReplicaRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x1d\n\x15source_resource_group\x18\x02 \x01(\t\x12\x1d\n\x15target_resource_group\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x04 \x01(\t\x12\x13\n\x0bnum_replica\x18\x05 \x01(\x03\x12\x0f\n\x07\x64\x62_name\x18\x06 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1f\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"[\n\x19ListResourceGroupsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase:\x12\xca>\x0f\x08\x01\x10\x1d\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"b\n\x1aListResourceGroupsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x17\n\x0fresource_groups\x18\x02 \x03(\t\"v\n\x1c\x44\x65scribeResourceGroupRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x16\n\x0eresource_group\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10\x1c\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\x88\x01\n\x1d\x44\x65scribeResourceGroupResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12:\n\x0eresource_group\x18\x02 \x01(\x0b\x32\".milvus.proto.milvus.ResourceGroup\"\xd6\x04\n\rResourceGroup\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x63\x61pacity\x18\x02 \x01(\x05\x12\x1a\n\x12num_available_node\x18\x03 \x01(\x05\x12T\n\x12num_loaded_replica\x18\x04 \x03(\x0b\x32\x38.milvus.proto.milvus.ResourceGroup.NumLoadedReplicaEntry\x12R\n\x11num_outgoing_node\x18\x05 \x03(\x0b\x32\x37.milvus.proto.milvus.ResourceGroup.NumOutgoingNodeEntry\x12R\n\x11num_incoming_node\x18\x06 \x03(\x0b\x32\x37.milvus.proto.milvus.ResourceGroup.NumIncomingNodeEntry\x12\x34\n\x06\x63onfig\x18\x07 \x01(\x0b\x32$.milvus.proto.rg.ResourceGroupConfig\x12,\n\x05nodes\x18\x08 \x03(\x0b\x32\x1d.milvus.proto.common.NodeInfo\x1a\x37\n\x15NumLoadedReplicaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x36\n\x14NumOutgoingNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x36\n\x14NumIncomingNodeEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"\x9f\x01\n\x17RenameCollectionRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x0f\n\x07oldName\x18\x03 \x01(\t\x12\x0f\n\x07newName\x18\x04 \x01(\t\x12\x11\n\tnewDBName\x18\x05 \x01(\t:\x12\xca>\x0f\x08\x01\x10\"\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"\xa1\x01\n\x19GetIndexStatisticsRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12\x12\n\nindex_name\x18\x04 \x01(\t\x12\x11\n\ttimestamp\x18\x05 \x01(\x04:\x07\xca>\x04\x10\x0c\x18\x03\"\x8c\x01\n\x1aGetIndexStatisticsResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x41\n\x12index_descriptions\x18\x02 \x03(\x0b\x32%.milvus.proto.milvus.IndexDescription\"r\n\x0e\x43onnectRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x34\n\x0b\x63lient_info\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.common.ClientInfo\"\x88\x01\n\x0f\x43onnectResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x34\n\x0bserver_info\x18\x02 \x01(\x0b\x32\x1f.milvus.proto.common.ServerInfo\x12\x12\n\nidentifier\x18\x03 \x01(\x03\"C\n\x15\x41llocTimestampRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"X\n\x16\x41llocTimestampResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x11\n\ttimestamp\x18\x02 \x01(\x04\"h\n\x15\x43reateDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10#\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"f\n\x13\x44ropDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t:\x12\xca>\x0f\x08\x01\x10$\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"B\n\x14ListDatabasesRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\"q\n\x15ListDatabasesResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08\x64\x62_names\x18\x02 \x03(\t\x12\x19\n\x11\x63reated_timestamp\x18\x03 \x03(\x04\"\xad\x01\n\x14\x41lterDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\r\n\x05\x64\x62_id\x18\x03 \x01(\t\x12\x35\n\nproperties\x18\x04 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair:\x12\xca>\x0f\x08\x01\x10\x31\x18\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01\"V\n\x17\x44\x65scribeDatabaseRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\"\xb8\x01\n\x18\x44\x65scribeDatabaseResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x0f\n\x07\x64\x62_name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x62ID\x18\x03 \x01(\x03\x12\x19\n\x11\x63reated_timestamp\x18\x04 \x01(\x04\x12\x35\n\nproperties\x18\x05 \x03(\x0b\x32!.milvus.proto.common.KeyValuePair\"\xf5\x01\n\x17ReplicateMessageRequest\x12*\n\x04\x62\x61se\x18\x01 \x01(\x0b\x32\x1c.milvus.proto.common.MsgBase\x12\x14\n\x0c\x63hannel_name\x18\x02 \x01(\t\x12\x0f\n\x07\x42\x65ginTs\x18\x03 \x01(\x04\x12\r\n\x05\x45ndTs\x18\x04 \x01(\x04\x12\x0c\n\x04Msgs\x18\x05 \x03(\x0c\x12\x35\n\x0eStartPositions\x18\x06 \x03(\x0b\x32\x1d.milvus.proto.msg.MsgPosition\x12\x33\n\x0c\x45ndPositions\x18\x07 \x03(\x0b\x32\x1d.milvus.proto.msg.MsgPosition\"Y\n\x18ReplicateMessageResponse\x12+\n\x06status\x18\x01 \x01(\x0b\x32\x1b.milvus.proto.common.Status\x12\x10\n\x08position\x18\x02 \x01(\t\"b\n\x15ImportAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\x12\x16\n\x0epartition_name\x18\x03 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01\"<\n GetImportProgressAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x01 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01\"O\n\x1aListImportsAuthPlaceholder\x12\x0f\n\x07\x64\x62_name\x18\x03 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t:\x07\xca>\x04\x10\x12\x18\x01*%\n\x08ShowType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08InMemory\x10\x01\x1a\x02\x18\x01*@\n\x13OperateUserRoleType\x12\x11\n\rAddUserToRole\x10\x00\x12\x16\n\x12RemoveUserFromRole\x10\x01*-\n\x14OperatePrivilegeType\x12\t\n\x05Grant\x10\x00\x12\n\n\x06Revoke\x10\x01*]\n\nQuotaState\x12\x0b\n\x07Unknown\x10\x00\x12\x0f\n\x0bReadLimited\x10\x02\x12\x10\n\x0cWriteLimited\x10\x03\x12\x0e\n\nDenyToRead\x10\x04\x12\x0f\n\x0b\x44\x65nyToWrite\x10\x05\x32\xba\x44\n\rMilvusService\x12_\n\x10\x43reateCollection\x12,.milvus.proto.milvus.CreateCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12[\n\x0e\x44ropCollection\x12*.milvus.proto.milvus.DropCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\rHasCollection\x12).milvus.proto.milvus.HasCollectionRequest\x1a!.milvus.proto.milvus.BoolResponse\"\x00\x12[\n\x0eLoadCollection\x12*.milvus.proto.milvus.LoadCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11ReleaseCollection\x12-.milvus.proto.milvus.ReleaseCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12\x44\x65scribeCollection\x12..milvus.proto.milvus.DescribeCollectionRequest\x1a/.milvus.proto.milvus.DescribeCollectionResponse\"\x00\x12\x86\x01\n\x17GetCollectionStatistics\x12\x33.milvus.proto.milvus.GetCollectionStatisticsRequest\x1a\x34.milvus.proto.milvus.GetCollectionStatisticsResponse\"\x00\x12n\n\x0fShowCollections\x12+.milvus.proto.milvus.ShowCollectionsRequest\x1a,.milvus.proto.milvus.ShowCollectionsResponse\"\x00\x12]\n\x0f\x41lterCollection\x12+.milvus.proto.milvus.AlterCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0f\x43reatePartition\x12+.milvus.proto.milvus.CreatePartitionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12Y\n\rDropPartition\x12).milvus.proto.milvus.DropPartitionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0cHasPartition\x12(.milvus.proto.milvus.HasPartitionRequest\x1a!.milvus.proto.milvus.BoolResponse\"\x00\x12[\n\x0eLoadPartitions\x12*.milvus.proto.milvus.LoadPartitionsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11ReleasePartitions\x12-.milvus.proto.milvus.ReleasePartitionsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x83\x01\n\x16GetPartitionStatistics\x12\x32.milvus.proto.milvus.GetPartitionStatisticsRequest\x1a\x33.milvus.proto.milvus.GetPartitionStatisticsResponse\"\x00\x12k\n\x0eShowPartitions\x12*.milvus.proto.milvus.ShowPartitionsRequest\x1a+.milvus.proto.milvus.ShowPartitionsResponse\"\x00\x12w\n\x12GetLoadingProgress\x12..milvus.proto.milvus.GetLoadingProgressRequest\x1a/.milvus.proto.milvus.GetLoadingProgressResponse\"\x00\x12\x65\n\x0cGetLoadState\x12(.milvus.proto.milvus.GetLoadStateRequest\x1a).milvus.proto.milvus.GetLoadStateResponse\"\x00\x12U\n\x0b\x43reateAlias\x12\'.milvus.proto.milvus.CreateAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12Q\n\tDropAlias\x12%.milvus.proto.milvus.DropAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\nAlterAlias\x12&.milvus.proto.milvus.AlterAliasRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rDescribeAlias\x12).milvus.proto.milvus.DescribeAliasRequest\x1a*.milvus.proto.milvus.DescribeAliasResponse\"\x00\x12\x62\n\x0bListAliases\x12\'.milvus.proto.milvus.ListAliasesRequest\x1a(.milvus.proto.milvus.ListAliasesResponse\"\x00\x12U\n\x0b\x43reateIndex\x12\'.milvus.proto.milvus.CreateIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\nAlterIndex\x12&.milvus.proto.milvus.AlterIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rDescribeIndex\x12).milvus.proto.milvus.DescribeIndexRequest\x1a*.milvus.proto.milvus.DescribeIndexResponse\"\x00\x12w\n\x12GetIndexStatistics\x12..milvus.proto.milvus.GetIndexStatisticsRequest\x1a/.milvus.proto.milvus.GetIndexStatisticsResponse\"\x00\x12k\n\rGetIndexState\x12).milvus.proto.milvus.GetIndexStateRequest\x1a*.milvus.proto.milvus.GetIndexStateResponse\"\x03\x88\x02\x01\x12\x83\x01\n\x15GetIndexBuildProgress\x12\x31.milvus.proto.milvus.GetIndexBuildProgressRequest\x1a\x32.milvus.proto.milvus.GetIndexBuildProgressResponse\"\x03\x88\x02\x01\x12Q\n\tDropIndex\x12%.milvus.proto.milvus.DropIndexRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12S\n\x06Insert\x12\".milvus.proto.milvus.InsertRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12S\n\x06\x44\x65lete\x12\".milvus.proto.milvus.DeleteRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12S\n\x06Upsert\x12\".milvus.proto.milvus.UpsertRequest\x1a#.milvus.proto.milvus.MutationResult\"\x00\x12R\n\x06Search\x12\".milvus.proto.milvus.SearchRequest\x1a\".milvus.proto.milvus.SearchResults\"\x00\x12^\n\x0cHybridSearch\x12(.milvus.proto.milvus.HybridSearchRequest\x1a\".milvus.proto.milvus.SearchResults\"\x00\x12P\n\x05\x46lush\x12!.milvus.proto.milvus.FlushRequest\x1a\".milvus.proto.milvus.FlushResponse\"\x00\x12O\n\x05Query\x12!.milvus.proto.milvus.QueryRequest\x1a!.milvus.proto.milvus.QueryResults\"\x00\x12\x64\n\x0c\x43\x61lcDistance\x12(.milvus.proto.milvus.CalcDistanceRequest\x1a(.milvus.proto.milvus.CalcDistanceResults\"\x00\x12Y\n\x08\x46lushAll\x12$.milvus.proto.milvus.FlushAllRequest\x1a%.milvus.proto.milvus.FlushAllResponse\"\x00\x12h\n\rGetFlushState\x12).milvus.proto.milvus.GetFlushStateRequest\x1a*.milvus.proto.milvus.GetFlushStateResponse\"\x00\x12q\n\x10GetFlushAllState\x12,.milvus.proto.milvus.GetFlushAllStateRequest\x1a-.milvus.proto.milvus.GetFlushAllStateResponse\"\x00\x12\x89\x01\n\x18GetPersistentSegmentInfo\x12\x34.milvus.proto.milvus.GetPersistentSegmentInfoRequest\x1a\x35.milvus.proto.milvus.GetPersistentSegmentInfoResponse\"\x00\x12z\n\x13GetQuerySegmentInfo\x12/.milvus.proto.milvus.GetQuerySegmentInfoRequest\x1a\x30.milvus.proto.milvus.GetQuerySegmentInfoResponse\"\x00\x12\x62\n\x0bGetReplicas\x12\'.milvus.proto.milvus.GetReplicasRequest\x1a(.milvus.proto.milvus.GetReplicasResponse\"\x00\x12P\n\x05\x44ummy\x12!.milvus.proto.milvus.DummyRequest\x1a\".milvus.proto.milvus.DummyResponse\"\x00\x12\x65\n\x0cRegisterLink\x12(.milvus.proto.milvus.RegisterLinkRequest\x1a).milvus.proto.milvus.RegisterLinkResponse\"\x00\x12_\n\nGetMetrics\x12&.milvus.proto.milvus.GetMetricsRequest\x1a\'.milvus.proto.milvus.GetMetricsResponse\"\x00\x12l\n\x12GetComponentStates\x12..milvus.proto.milvus.GetComponentStatesRequest\x1a$.milvus.proto.milvus.ComponentStates\"\x00\x12U\n\x0bLoadBalance\x12\'.milvus.proto.milvus.LoadBalanceRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12GetCompactionState\x12..milvus.proto.milvus.GetCompactionStateRequest\x1a/.milvus.proto.milvus.GetCompactionStateResponse\"\x00\x12q\n\x10ManualCompaction\x12,.milvus.proto.milvus.ManualCompactionRequest\x1a-.milvus.proto.milvus.ManualCompactionResponse\"\x00\x12\x80\x01\n\x1bGetCompactionStateWithPlans\x12..milvus.proto.milvus.GetCompactionPlansRequest\x1a/.milvus.proto.milvus.GetCompactionPlansResponse\"\x00\x12S\n\x06Import\x12\".milvus.proto.milvus.ImportRequest\x1a#.milvus.proto.milvus.ImportResponse\"\x00\x12k\n\x0eGetImportState\x12*.milvus.proto.milvus.GetImportStateRequest\x1a+.milvus.proto.milvus.GetImportStateResponse\"\x00\x12n\n\x0fListImportTasks\x12+.milvus.proto.milvus.ListImportTasksRequest\x1a,.milvus.proto.milvus.ListImportTasksResponse\"\x00\x12_\n\x10\x43reateCredential\x12,.milvus.proto.milvus.CreateCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\x10UpdateCredential\x12,.milvus.proto.milvus.UpdateCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\x10\x44\x65leteCredential\x12,.milvus.proto.milvus.DeleteCredentialRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rListCredUsers\x12).milvus.proto.milvus.ListCredUsersRequest\x1a*.milvus.proto.milvus.ListCredUsersResponse\"\x00\x12S\n\nCreateRole\x12&.milvus.proto.milvus.CreateRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12O\n\x08\x44ropRole\x12$.milvus.proto.milvus.DropRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0fOperateUserRole\x12+.milvus.proto.milvus.OperateUserRoleRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12_\n\nSelectRole\x12&.milvus.proto.milvus.SelectRoleRequest\x1a\'.milvus.proto.milvus.SelectRoleResponse\"\x00\x12_\n\nSelectUser\x12&.milvus.proto.milvus.SelectUserRequest\x1a\'.milvus.proto.milvus.SelectUserResponse\"\x00\x12_\n\x10OperatePrivilege\x12,.milvus.proto.milvus.OperatePrivilegeRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x62\n\x0bSelectGrant\x12\'.milvus.proto.milvus.SelectGrantRequest\x1a(.milvus.proto.milvus.SelectGrantResponse\"\x00\x12_\n\nGetVersion\x12&.milvus.proto.milvus.GetVersionRequest\x1a\'.milvus.proto.milvus.GetVersionResponse\"\x00\x12\x62\n\x0b\x43heckHealth\x12\'.milvus.proto.milvus.CheckHealthRequest\x1a(.milvus.proto.milvus.CheckHealthResponse\"\x00\x12\x65\n\x13\x43reateResourceGroup\x12/.milvus.proto.milvus.CreateResourceGroupRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12\x61\n\x11\x44ropResourceGroup\x12-.milvus.proto.milvus.DropResourceGroupRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12g\n\x14UpdateResourceGroups\x12\x30.milvus.proto.milvus.UpdateResourceGroupsRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12W\n\x0cTransferNode\x12(.milvus.proto.milvus.TransferNodeRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12]\n\x0fTransferReplica\x12+.milvus.proto.milvus.TransferReplicaRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12w\n\x12ListResourceGroups\x12..milvus.proto.milvus.ListResourceGroupsRequest\x1a/.milvus.proto.milvus.ListResourceGroupsResponse\"\x00\x12\x80\x01\n\x15\x44\x65scribeResourceGroup\x12\x31.milvus.proto.milvus.DescribeResourceGroupRequest\x1a\x32.milvus.proto.milvus.DescribeResourceGroupResponse\"\x00\x12_\n\x10RenameCollection\x12,.milvus.proto.milvus.RenameCollectionRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12u\n\x12ListIndexedSegment\x12-.milvus.proto.feder.ListIndexedSegmentRequest\x1a..milvus.proto.feder.ListIndexedSegmentResponse\"\x00\x12\x87\x01\n\x18\x44\x65scribeSegmentIndexData\x12\x33.milvus.proto.feder.DescribeSegmentIndexDataRequest\x1a\x34.milvus.proto.feder.DescribeSegmentIndexDataResponse\"\x00\x12V\n\x07\x43onnect\x12#.milvus.proto.milvus.ConnectRequest\x1a$.milvus.proto.milvus.ConnectResponse\"\x00\x12k\n\x0e\x41llocTimestamp\x12*.milvus.proto.milvus.AllocTimestampRequest\x1a+.milvus.proto.milvus.AllocTimestampResponse\"\x00\x12[\n\x0e\x43reateDatabase\x12*.milvus.proto.milvus.CreateDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12W\n\x0c\x44ropDatabase\x12(.milvus.proto.milvus.DropDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12h\n\rListDatabases\x12).milvus.proto.milvus.ListDatabasesRequest\x1a*.milvus.proto.milvus.ListDatabasesResponse\"\x00\x12Y\n\rAlterDatabase\x12).milvus.proto.milvus.AlterDatabaseRequest\x1a\x1b.milvus.proto.common.Status\"\x00\x12q\n\x10\x44\x65scribeDatabase\x12,.milvus.proto.milvus.DescribeDatabaseRequest\x1a-.milvus.proto.milvus.DescribeDatabaseResponse\"\x00\x12q\n\x10ReplicateMessage\x12,.milvus.proto.milvus.ReplicateMessageRequest\x1a-.milvus.proto.milvus.ReplicateMessageResponse\"\x00\x32u\n\x0cProxyService\x12\x65\n\x0cRegisterLink\x12(.milvus.proto.milvus.RegisterLinkRequest\x1a).milvus.proto.milvus.RegisterLinkResponse\"\x00:U\n\x0emilvus_ext_obj\x12\x1c.google.protobuf.FileOptions\x18\xe9\x07 \x01(\x0b\x32\x1e.milvus.proto.milvus.MilvusExtBm\n\x0eio.milvus.grpcB\x0bMilvusProtoP\x01Z4github.com/milvus-io/milvus-proto/go-api/v2/milvuspb\xa0\x01\x01\xaa\x02\x12Milvus.Client.Grpcb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'milvus_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\016io.milvus.grpcB\013MilvusProtoP\001Z4github.com/milvus-io/milvus-proto/go-api/v2/milvuspb\240\001\001\252\002\022Milvus.Client.Grpc'
@@ -104,14 +104,16 @@
   _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_options = b'8\001'
   _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._options = None
   _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_options = b'8\001'
   _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._options = None
   _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_options = b'8\001'
   _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._options = None
   _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_options = b'8\001'
+  _globals['_FLUSHRESPONSE_CHANNELCPSENTRY']._options = None
+  _globals['_FLUSHRESPONSE_CHANNELCPSENTRY']._serialized_options = b'8\001'
   _globals['_QUERYREQUEST']._options = None
   _globals['_QUERYREQUEST']._serialized_options = b'\312>\004\020\020\030\003'
   _globals['_FLUSHALLREQUEST']._options = None
   _globals['_FLUSHALLREQUEST']._serialized_options = b'\312>\017\010\001\020&\030\377\377\377\377\377\377\377\377\377\001'
   _globals['_QUERYSEGMENTINFO'].fields_by_name['nodeID']._options = None
   _globals['_QUERYSEGMENTINFO'].fields_by_name['nodeID']._serialized_options = b'\030\001'
   _globals['_LOADBALANCEREQUEST']._options = None
@@ -188,22 +190,22 @@
   _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_options = b'\312>\004\020\022\030\001'
   _globals['_LISTIMPORTSAUTHPLACEHOLDER']._options = None
   _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_options = b'\312>\004\020\022\030\001'
   _globals['_MILVUSSERVICE'].methods_by_name['GetIndexState']._options = None
   _globals['_MILVUSSERVICE'].methods_by_name['GetIndexState']._serialized_options = b'\210\002\001'
   _globals['_MILVUSSERVICE'].methods_by_name['GetIndexBuildProgress']._options = None
   _globals['_MILVUSSERVICE'].methods_by_name['GetIndexBuildProgress']._serialized_options = b'\210\002\001'
-  _globals['_SHOWTYPE']._serialized_start=24640
-  _globals['_SHOWTYPE']._serialized_end=24677
-  _globals['_OPERATEUSERROLETYPE']._serialized_start=24679
-  _globals['_OPERATEUSERROLETYPE']._serialized_end=24743
-  _globals['_OPERATEPRIVILEGETYPE']._serialized_start=24745
-  _globals['_OPERATEPRIVILEGETYPE']._serialized_end=24790
-  _globals['_QUOTASTATE']._serialized_start=24792
-  _globals['_QUOTASTATE']._serialized_end=24885
+  _globals['_SHOWTYPE']._serialized_start=25070
+  _globals['_SHOWTYPE']._serialized_end=25107
+  _globals['_OPERATEUSERROLETYPE']._serialized_start=25109
+  _globals['_OPERATEUSERROLETYPE']._serialized_end=25173
+  _globals['_OPERATEPRIVILEGETYPE']._serialized_start=25175
+  _globals['_OPERATEPRIVILEGETYPE']._serialized_end=25220
+  _globals['_QUOTASTATE']._serialized_start=25222
+  _globals['_QUOTASTATE']._serialized_end=25315
   _globals['_CREATEALIASREQUEST']._serialized_start=134
   _globals['_CREATEALIASREQUEST']._serialized_end=275
   _globals['_DROPALIASREQUEST']._serialized_start=277
   _globals['_DROPALIASREQUEST']._serialized_end=391
   _globals['_ALTERALIASREQUEST']._serialized_start=394
   _globals['_ALTERALIASREQUEST']._serialized_end=534
   _globals['_DESCRIBEALIASREQUEST']._serialized_start=536
@@ -309,241 +311,247 @@
   _globals['_SEARCHRESULTS']._serialized_start=9484
   _globals['_SEARCHRESULTS']._serialized_end=9625
   _globals['_HYBRIDSEARCHREQUEST']._serialized_start=9628
   _globals['_HYBRIDSEARCHREQUEST']._serialized_end=10085
   _globals['_FLUSHREQUEST']._serialized_start=10087
   _globals['_FLUSHREQUEST']._serialized_end=10197
   _globals['_FLUSHRESPONSE']._serialized_start=10200
-  _globals['_FLUSHRESPONSE']._serialized_end=10867
-  _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_start=10592
-  _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_end=10673
-  _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_start=10675
-  _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_end=10761
-  _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_start=10763
-  _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_end=10815
-  _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_start=10817
-  _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_end=10867
-  _globals['_QUERYREQUEST']._serialized_start=10870
-  _globals['_QUERYREQUEST']._serialized_end=11281
-  _globals['_QUERYRESULTS']._serialized_start=11284
-  _globals['_QUERYRESULTS']._serialized_end=11444
-  _globals['_VECTORIDS']._serialized_start=11446
-  _globals['_VECTORIDS']._serialized_end=11571
-  _globals['_VECTORSARRAY']._serialized_start=11574
-  _globals['_VECTORSARRAY']._serialized_end=11705
-  _globals['_CALCDISTANCEREQUEST']._serialized_start=11708
-  _globals['_CALCDISTANCEREQUEST']._serialized_end=11929
-  _globals['_CALCDISTANCERESULTS']._serialized_start=11932
-  _globals['_CALCDISTANCERESULTS']._serialized_end=12113
-  _globals['_FLUSHALLREQUEST']._serialized_start=12115
-  _globals['_FLUSHALLREQUEST']._serialized_end=12213
-  _globals['_FLUSHALLRESPONSE']._serialized_start=12215
-  _globals['_FLUSHALLRESPONSE']._serialized_end=12300
-  _globals['_PERSISTENTSEGMENTINFO']._serialized_start=12303
-  _globals['_PERSISTENTSEGMENTINFO']._serialized_end=12456
-  _globals['_GETPERSISTENTSEGMENTINFOREQUEST']._serialized_start=12458
-  _globals['_GETPERSISTENTSEGMENTINFOREQUEST']._serialized_end=12575
-  _globals['_GETPERSISTENTSEGMENTINFORESPONSE']._serialized_start=12578
-  _globals['_GETPERSISTENTSEGMENTINFORESPONSE']._serialized_end=12716
-  _globals['_QUERYSEGMENTINFO']._serialized_start=12719
-  _globals['_QUERYSEGMENTINFO']._serialized_end=12959
-  _globals['_GETQUERYSEGMENTINFOREQUEST']._serialized_start=12961
-  _globals['_GETQUERYSEGMENTINFOREQUEST']._serialized_end=13073
-  _globals['_GETQUERYSEGMENTINFORESPONSE']._serialized_start=13076
-  _globals['_GETQUERYSEGMENTINFORESPONSE']._serialized_end=13204
-  _globals['_DUMMYREQUEST']._serialized_start=13206
-  _globals['_DUMMYREQUEST']._serialized_end=13242
-  _globals['_DUMMYRESPONSE']._serialized_start=13244
-  _globals['_DUMMYRESPONSE']._serialized_end=13277
-  _globals['_REGISTERLINKREQUEST']._serialized_start=13279
-  _globals['_REGISTERLINKREQUEST']._serialized_end=13300
-  _globals['_REGISTERLINKRESPONSE']._serialized_start=13302
-  _globals['_REGISTERLINKRESPONSE']._serialized_end=13416
-  _globals['_GETMETRICSREQUEST']._serialized_start=13418
-  _globals['_GETMETRICSREQUEST']._serialized_end=13498
-  _globals['_GETMETRICSRESPONSE']._serialized_start=13500
-  _globals['_GETMETRICSRESPONSE']._serialized_end=13607
-  _globals['_COMPONENTINFO']._serialized_start=13610
-  _globals['_COMPONENTINFO']._serialized_end=13762
-  _globals['_COMPONENTSTATES']._serialized_start=13765
-  _globals['_COMPONENTSTATES']._serialized_end=13943
-  _globals['_GETCOMPONENTSTATESREQUEST']._serialized_start=13945
-  _globals['_GETCOMPONENTSTATESREQUEST']._serialized_end=13972
-  _globals['_LOADBALANCEREQUEST']._serialized_start=13975
-  _globals['_LOADBALANCEREQUEST']._serialized_end=14157
-  _globals['_MANUALCOMPACTIONREQUEST']._serialized_start=14159
-  _globals['_MANUALCOMPACTIONREQUEST']._serialized_end=14260
-  _globals['_MANUALCOMPACTIONRESPONSE']._serialized_start=14262
-  _globals['_MANUALCOMPACTIONRESPONSE']._serialized_end=14384
-  _globals['_GETCOMPACTIONSTATEREQUEST']._serialized_start=14386
-  _globals['_GETCOMPACTIONSTATEREQUEST']._serialized_end=14435
-  _globals['_GETCOMPACTIONSTATERESPONSE']._serialized_start=14438
-  _globals['_GETCOMPACTIONSTATERESPONSE']._serialized_end=14659
-  _globals['_GETCOMPACTIONPLANSREQUEST']._serialized_start=14661
-  _globals['_GETCOMPACTIONPLANSREQUEST']._serialized_end=14710
-  _globals['_GETCOMPACTIONPLANSRESPONSE']._serialized_start=14713
-  _globals['_GETCOMPACTIONPLANSRESPONSE']._serialized_end=14901
-  _globals['_COMPACTIONMERGEINFO']._serialized_start=14903
-  _globals['_COMPACTIONMERGEINFO']._serialized_end=14957
-  _globals['_GETFLUSHSTATEREQUEST']._serialized_start=14959
-  _globals['_GETFLUSHSTATEREQUEST']._serialized_end=15070
-  _globals['_GETFLUSHSTATERESPONSE']._serialized_start=15072
-  _globals['_GETFLUSHSTATERESPONSE']._serialized_end=15157
-  _globals['_GETFLUSHALLSTATEREQUEST']._serialized_start=15159
-  _globals['_GETFLUSHALLSTATEREQUEST']._serialized_end=15267
-  _globals['_GETFLUSHALLSTATERESPONSE']._serialized_start=15269
-  _globals['_GETFLUSHALLSTATERESPONSE']._serialized_end=15357
-  _globals['_IMPORTREQUEST']._serialized_start=15360
-  _globals['_IMPORTREQUEST']._serialized_end=15584
-  _globals['_IMPORTRESPONSE']._serialized_start=15586
-  _globals['_IMPORTRESPONSE']._serialized_end=15662
-  _globals['_GETIMPORTSTATEREQUEST']._serialized_start=15664
-  _globals['_GETIMPORTSTATEREQUEST']._serialized_end=15701
-  _globals['_GETIMPORTSTATERESPONSE']._serialized_start=15704
-  _globals['_GETIMPORTSTATERESPONSE']._serialized_end=15983
-  _globals['_LISTIMPORTTASKSREQUEST']._serialized_start=15985
-  _globals['_LISTIMPORTTASKSREQUEST']._serialized_end=16066
-  _globals['_LISTIMPORTTASKSRESPONSE']._serialized_start=16069
-  _globals['_LISTIMPORTTASKSRESPONSE']._serialized_end=16199
-  _globals['_GETREPLICASREQUEST']._serialized_start=16202
-  _globals['_GETREPLICASREQUEST']._serialized_end=16356
-  _globals['_GETREPLICASRESPONSE']._serialized_start=16358
-  _globals['_GETREPLICASRESPONSE']._serialized_end=16476
-  _globals['_REPLICAINFO']._serialized_start=16479
-  _globals['_REPLICAINFO']._serialized_end=16800
-  _globals['_REPLICAINFO_NUMOUTBOUNDNODEENTRY']._serialized_start=16746
-  _globals['_REPLICAINFO_NUMOUTBOUNDNODEENTRY']._serialized_end=16800
-  _globals['_SHARDREPLICA']._serialized_start=16802
-  _globals['_SHARDREPLICA']._serialized_end=16898
-  _globals['_CREATECREDENTIALREQUEST']._serialized_start=16901
-  _globals['_CREATECREDENTIALREQUEST']._serialized_end=17091
-  _globals['_UPDATECREDENTIALREQUEST']._serialized_start=17094
-  _globals['_UPDATECREDENTIALREQUEST']._serialized_end=17299
-  _globals['_DELETECREDENTIALREQUEST']._serialized_start=17301
-  _globals['_DELETECREDENTIALREQUEST']._serialized_end=17408
-  _globals['_LISTCREDUSERSRESPONSE']._serialized_start=17410
-  _globals['_LISTCREDUSERSRESPONSE']._serialized_end=17497
-  _globals['_LISTCREDUSERSREQUEST']._serialized_start=17499
-  _globals['_LISTCREDUSERSREQUEST']._serialized_end=17585
-  _globals['_ROLEENTITY']._serialized_start=17587
-  _globals['_ROLEENTITY']._serialized_end=17613
-  _globals['_USERENTITY']._serialized_start=17615
-  _globals['_USERENTITY']._serialized_end=17641
-  _globals['_CREATEROLEREQUEST']._serialized_start=17644
-  _globals['_CREATEROLEREQUEST']._serialized_end=17776
-  _globals['_DROPROLEREQUEST']._serialized_start=17778
-  _globals['_DROPROLEREQUEST']._serialized_end=17878
-  _globals['_OPERATEUSERROLEREQUEST']._serialized_start=17881
-  _globals['_OPERATEUSERROLEREQUEST']._serialized_end=18062
-  _globals['_SELECTROLEREQUEST']._serialized_start=18065
-  _globals['_SELECTROLEREQUEST']._serialized_end=18222
-  _globals['_ROLERESULT']._serialized_start=18224
-  _globals['_ROLERESULT']._serialized_end=18331
-  _globals['_SELECTROLERESPONSE']._serialized_start=18333
-  _globals['_SELECTROLERESPONSE']._serialized_end=18448
-  _globals['_SELECTUSERREQUEST']._serialized_start=18451
-  _globals['_SELECTUSERREQUEST']._serialized_end=18599
-  _globals['_USERRESULT']._serialized_start=18601
-  _globals['_USERRESULT']._serialized_end=18708
-  _globals['_SELECTUSERRESPONSE']._serialized_start=18710
-  _globals['_SELECTUSERRESPONSE']._serialized_end=18825
-  _globals['_OBJECTENTITY']._serialized_start=18827
-  _globals['_OBJECTENTITY']._serialized_end=18855
-  _globals['_PRIVILEGEENTITY']._serialized_start=18857
-  _globals['_PRIVILEGEENTITY']._serialized_end=18888
-  _globals['_GRANTORENTITY']._serialized_start=18890
-  _globals['_GRANTORENTITY']._serialized_end=19009
-  _globals['_GRANTPRIVILEGEENTITY']._serialized_start=19011
-  _globals['_GRANTPRIVILEGEENTITY']._serialized_end=19087
-  _globals['_GRANTENTITY']._serialized_start=19090
-  _globals['_GRANTENTITY']._serialized_end=19292
-  _globals['_SELECTGRANTREQUEST']._serialized_start=19295
-  _globals['_SELECTGRANTREQUEST']._serialized_end=19429
-  _globals['_SELECTGRANTRESPONSE']._serialized_start=19431
-  _globals['_SELECTGRANTRESPONSE']._serialized_end=19549
-  _globals['_OPERATEPRIVILEGEREQUEST']._serialized_start=19552
-  _globals['_OPERATEPRIVILEGEREQUEST']._serialized_end=19748
-  _globals['_GETLOADINGPROGRESSREQUEST']._serialized_start=19751
-  _globals['_GETLOADINGPROGRESSREQUEST']._serialized_end=19898
-  _globals['_GETLOADINGPROGRESSRESPONSE']._serialized_start=19900
-  _globals['_GETLOADINGPROGRESSRESPONSE']._serialized_end=20017
-  _globals['_GETLOADSTATEREQUEST']._serialized_start=20020
-  _globals['_GETLOADSTATEREQUEST']._serialized_end=20161
-  _globals['_GETLOADSTATERESPONSE']._serialized_start=20163
-  _globals['_GETLOADSTATERESPONSE']._serialized_end=20277
-  _globals['_MILVUSEXT']._serialized_start=20279
-  _globals['_MILVUSEXT']._serialized_end=20307
-  _globals['_GETVERSIONREQUEST']._serialized_start=20309
-  _globals['_GETVERSIONREQUEST']._serialized_end=20328
-  _globals['_GETVERSIONRESPONSE']._serialized_start=20330
-  _globals['_GETVERSIONRESPONSE']._serialized_end=20412
-  _globals['_CHECKHEALTHREQUEST']._serialized_start=20414
-  _globals['_CHECKHEALTHREQUEST']._serialized_end=20434
-  _globals['_CHECKHEALTHRESPONSE']._serialized_start=20437
-  _globals['_CHECKHEALTHRESPONSE']._serialized_end=20594
-  _globals['_CREATERESOURCEGROUPREQUEST']._serialized_start=20597
-  _globals['_CREATERESOURCEGROUPREQUEST']._serialized_end=20767
-  _globals['_UPDATERESOURCEGROUPSREQUEST']._serialized_start=20770
-  _globals['_UPDATERESOURCEGROUPSREQUEST']._serialized_end=21051
-  _globals['_UPDATERESOURCEGROUPSREQUEST_RESOURCEGROUPSENTRY']._serialized_start=20940
-  _globals['_UPDATERESOURCEGROUPSREQUEST_RESOURCEGROUPSENTRY']._serialized_end=21031
-  _globals['_DROPRESOURCEGROUPREQUEST']._serialized_start=21053
-  _globals['_DROPRESOURCEGROUPREQUEST']._serialized_end=21167
-  _globals['_TRANSFERNODEREQUEST']._serialized_start=21170
-  _globals['_TRANSFERNODEREQUEST']._serialized_end=21335
-  _globals['_TRANSFERREPLICAREQUEST']._serialized_start=21338
-  _globals['_TRANSFERREPLICAREQUEST']._serialized_end=21551
-  _globals['_LISTRESOURCEGROUPSREQUEST']._serialized_start=21553
-  _globals['_LISTRESOURCEGROUPSREQUEST']._serialized_end=21644
-  _globals['_LISTRESOURCEGROUPSRESPONSE']._serialized_start=21646
-  _globals['_LISTRESOURCEGROUPSRESPONSE']._serialized_end=21744
-  _globals['_DESCRIBERESOURCEGROUPREQUEST']._serialized_start=21746
-  _globals['_DESCRIBERESOURCEGROUPREQUEST']._serialized_end=21864
-  _globals['_DESCRIBERESOURCEGROUPRESPONSE']._serialized_start=21867
-  _globals['_DESCRIBERESOURCEGROUPRESPONSE']._serialized_end=22003
-  _globals['_RESOURCEGROUP']._serialized_start=22006
-  _globals['_RESOURCEGROUP']._serialized_end=22604
-  _globals['_RESOURCEGROUP_NUMLOADEDREPLICAENTRY']._serialized_start=22437
-  _globals['_RESOURCEGROUP_NUMLOADEDREPLICAENTRY']._serialized_end=22492
-  _globals['_RESOURCEGROUP_NUMOUTGOINGNODEENTRY']._serialized_start=22494
-  _globals['_RESOURCEGROUP_NUMOUTGOINGNODEENTRY']._serialized_end=22548
-  _globals['_RESOURCEGROUP_NUMINCOMINGNODEENTRY']._serialized_start=22550
-  _globals['_RESOURCEGROUP_NUMINCOMINGNODEENTRY']._serialized_end=22604
-  _globals['_RENAMECOLLECTIONREQUEST']._serialized_start=22607
-  _globals['_RENAMECOLLECTIONREQUEST']._serialized_end=22766
-  _globals['_GETINDEXSTATISTICSREQUEST']._serialized_start=22769
-  _globals['_GETINDEXSTATISTICSREQUEST']._serialized_end=22930
-  _globals['_GETINDEXSTATISTICSRESPONSE']._serialized_start=22933
-  _globals['_GETINDEXSTATISTICSRESPONSE']._serialized_end=23073
-  _globals['_CONNECTREQUEST']._serialized_start=23075
-  _globals['_CONNECTREQUEST']._serialized_end=23189
-  _globals['_CONNECTRESPONSE']._serialized_start=23192
-  _globals['_CONNECTRESPONSE']._serialized_end=23328
-  _globals['_ALLOCTIMESTAMPREQUEST']._serialized_start=23330
-  _globals['_ALLOCTIMESTAMPREQUEST']._serialized_end=23397
-  _globals['_ALLOCTIMESTAMPRESPONSE']._serialized_start=23399
-  _globals['_ALLOCTIMESTAMPRESPONSE']._serialized_end=23487
-  _globals['_CREATEDATABASEREQUEST']._serialized_start=23489
-  _globals['_CREATEDATABASEREQUEST']._serialized_end=23593
-  _globals['_DROPDATABASEREQUEST']._serialized_start=23595
-  _globals['_DROPDATABASEREQUEST']._serialized_end=23697
-  _globals['_LISTDATABASESREQUEST']._serialized_start=23699
-  _globals['_LISTDATABASESREQUEST']._serialized_end=23765
-  _globals['_LISTDATABASESRESPONSE']._serialized_start=23767
-  _globals['_LISTDATABASESRESPONSE']._serialized_end=23880
-  _globals['_ALTERDATABASEREQUEST']._serialized_start=23883
-  _globals['_ALTERDATABASEREQUEST']._serialized_end=24056
-  _globals['_REPLICATEMESSAGEREQUEST']._serialized_start=24059
-  _globals['_REPLICATEMESSAGEREQUEST']._serialized_end=24304
-  _globals['_REPLICATEMESSAGERESPONSE']._serialized_start=24306
-  _globals['_REPLICATEMESSAGERESPONSE']._serialized_end=24395
-  _globals['_IMPORTAUTHPLACEHOLDER']._serialized_start=24397
-  _globals['_IMPORTAUTHPLACEHOLDER']._serialized_end=24495
-  _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_start=24497
-  _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_end=24557
-  _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_start=24559
-  _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_end=24638
-  _globals['_MILVUSSERVICE']._serialized_start=24888
-  _globals['_MILVUSSERVICE']._serialized_end=33535
-  _globals['_PROXYSERVICE']._serialized_start=33537
-  _globals['_PROXYSERVICE']._serialized_end=33654
+  _globals['_FLUSHRESPONSE']._serialized_end=11022
+  _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_start=10665
+  _globals['_FLUSHRESPONSE_COLLSEGIDSENTRY']._serialized_end=10746
+  _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_start=10748
+  _globals['_FLUSHRESPONSE_FLUSHCOLLSEGIDSENTRY']._serialized_end=10834
+  _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_start=10836
+  _globals['_FLUSHRESPONSE_COLLSEALTIMESENTRY']._serialized_end=10888
+  _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_start=10890
+  _globals['_FLUSHRESPONSE_COLLFLUSHTSENTRY']._serialized_end=10940
+  _globals['_FLUSHRESPONSE_CHANNELCPSENTRY']._serialized_start=10942
+  _globals['_FLUSHRESPONSE_CHANNELCPSENTRY']._serialized_end=11022
+  _globals['_QUERYREQUEST']._serialized_start=11025
+  _globals['_QUERYREQUEST']._serialized_end=11436
+  _globals['_QUERYRESULTS']._serialized_start=11439
+  _globals['_QUERYRESULTS']._serialized_end=11599
+  _globals['_VECTORIDS']._serialized_start=11601
+  _globals['_VECTORIDS']._serialized_end=11726
+  _globals['_VECTORSARRAY']._serialized_start=11729
+  _globals['_VECTORSARRAY']._serialized_end=11860
+  _globals['_CALCDISTANCEREQUEST']._serialized_start=11863
+  _globals['_CALCDISTANCEREQUEST']._serialized_end=12084
+  _globals['_CALCDISTANCERESULTS']._serialized_start=12087
+  _globals['_CALCDISTANCERESULTS']._serialized_end=12268
+  _globals['_FLUSHALLREQUEST']._serialized_start=12270
+  _globals['_FLUSHALLREQUEST']._serialized_end=12368
+  _globals['_FLUSHALLRESPONSE']._serialized_start=12370
+  _globals['_FLUSHALLRESPONSE']._serialized_end=12455
+  _globals['_PERSISTENTSEGMENTINFO']._serialized_start=12458
+  _globals['_PERSISTENTSEGMENTINFO']._serialized_end=12611
+  _globals['_GETPERSISTENTSEGMENTINFOREQUEST']._serialized_start=12613
+  _globals['_GETPERSISTENTSEGMENTINFOREQUEST']._serialized_end=12730
+  _globals['_GETPERSISTENTSEGMENTINFORESPONSE']._serialized_start=12733
+  _globals['_GETPERSISTENTSEGMENTINFORESPONSE']._serialized_end=12871
+  _globals['_QUERYSEGMENTINFO']._serialized_start=12874
+  _globals['_QUERYSEGMENTINFO']._serialized_end=13114
+  _globals['_GETQUERYSEGMENTINFOREQUEST']._serialized_start=13116
+  _globals['_GETQUERYSEGMENTINFOREQUEST']._serialized_end=13228
+  _globals['_GETQUERYSEGMENTINFORESPONSE']._serialized_start=13231
+  _globals['_GETQUERYSEGMENTINFORESPONSE']._serialized_end=13359
+  _globals['_DUMMYREQUEST']._serialized_start=13361
+  _globals['_DUMMYREQUEST']._serialized_end=13397
+  _globals['_DUMMYRESPONSE']._serialized_start=13399
+  _globals['_DUMMYRESPONSE']._serialized_end=13432
+  _globals['_REGISTERLINKREQUEST']._serialized_start=13434
+  _globals['_REGISTERLINKREQUEST']._serialized_end=13455
+  _globals['_REGISTERLINKRESPONSE']._serialized_start=13457
+  _globals['_REGISTERLINKRESPONSE']._serialized_end=13571
+  _globals['_GETMETRICSREQUEST']._serialized_start=13573
+  _globals['_GETMETRICSREQUEST']._serialized_end=13653
+  _globals['_GETMETRICSRESPONSE']._serialized_start=13655
+  _globals['_GETMETRICSRESPONSE']._serialized_end=13762
+  _globals['_COMPONENTINFO']._serialized_start=13765
+  _globals['_COMPONENTINFO']._serialized_end=13917
+  _globals['_COMPONENTSTATES']._serialized_start=13920
+  _globals['_COMPONENTSTATES']._serialized_end=14098
+  _globals['_GETCOMPONENTSTATESREQUEST']._serialized_start=14100
+  _globals['_GETCOMPONENTSTATESREQUEST']._serialized_end=14127
+  _globals['_LOADBALANCEREQUEST']._serialized_start=14130
+  _globals['_LOADBALANCEREQUEST']._serialized_end=14312
+  _globals['_MANUALCOMPACTIONREQUEST']._serialized_start=14314
+  _globals['_MANUALCOMPACTIONREQUEST']._serialized_end=14415
+  _globals['_MANUALCOMPACTIONRESPONSE']._serialized_start=14417
+  _globals['_MANUALCOMPACTIONRESPONSE']._serialized_end=14539
+  _globals['_GETCOMPACTIONSTATEREQUEST']._serialized_start=14541
+  _globals['_GETCOMPACTIONSTATEREQUEST']._serialized_end=14590
+  _globals['_GETCOMPACTIONSTATERESPONSE']._serialized_start=14593
+  _globals['_GETCOMPACTIONSTATERESPONSE']._serialized_end=14814
+  _globals['_GETCOMPACTIONPLANSREQUEST']._serialized_start=14816
+  _globals['_GETCOMPACTIONPLANSREQUEST']._serialized_end=14865
+  _globals['_GETCOMPACTIONPLANSRESPONSE']._serialized_start=14868
+  _globals['_GETCOMPACTIONPLANSRESPONSE']._serialized_end=15056
+  _globals['_COMPACTIONMERGEINFO']._serialized_start=15058
+  _globals['_COMPACTIONMERGEINFO']._serialized_end=15112
+  _globals['_GETFLUSHSTATEREQUEST']._serialized_start=15114
+  _globals['_GETFLUSHSTATEREQUEST']._serialized_end=15225
+  _globals['_GETFLUSHSTATERESPONSE']._serialized_start=15227
+  _globals['_GETFLUSHSTATERESPONSE']._serialized_end=15312
+  _globals['_GETFLUSHALLSTATEREQUEST']._serialized_start=15314
+  _globals['_GETFLUSHALLSTATEREQUEST']._serialized_end=15422
+  _globals['_GETFLUSHALLSTATERESPONSE']._serialized_start=15424
+  _globals['_GETFLUSHALLSTATERESPONSE']._serialized_end=15512
+  _globals['_IMPORTREQUEST']._serialized_start=15515
+  _globals['_IMPORTREQUEST']._serialized_end=15739
+  _globals['_IMPORTRESPONSE']._serialized_start=15741
+  _globals['_IMPORTRESPONSE']._serialized_end=15817
+  _globals['_GETIMPORTSTATEREQUEST']._serialized_start=15819
+  _globals['_GETIMPORTSTATEREQUEST']._serialized_end=15856
+  _globals['_GETIMPORTSTATERESPONSE']._serialized_start=15859
+  _globals['_GETIMPORTSTATERESPONSE']._serialized_end=16138
+  _globals['_LISTIMPORTTASKSREQUEST']._serialized_start=16140
+  _globals['_LISTIMPORTTASKSREQUEST']._serialized_end=16221
+  _globals['_LISTIMPORTTASKSRESPONSE']._serialized_start=16224
+  _globals['_LISTIMPORTTASKSRESPONSE']._serialized_end=16354
+  _globals['_GETREPLICASREQUEST']._serialized_start=16357
+  _globals['_GETREPLICASREQUEST']._serialized_end=16511
+  _globals['_GETREPLICASRESPONSE']._serialized_start=16513
+  _globals['_GETREPLICASRESPONSE']._serialized_end=16631
+  _globals['_REPLICAINFO']._serialized_start=16634
+  _globals['_REPLICAINFO']._serialized_end=16955
+  _globals['_REPLICAINFO_NUMOUTBOUNDNODEENTRY']._serialized_start=16901
+  _globals['_REPLICAINFO_NUMOUTBOUNDNODEENTRY']._serialized_end=16955
+  _globals['_SHARDREPLICA']._serialized_start=16957
+  _globals['_SHARDREPLICA']._serialized_end=17053
+  _globals['_CREATECREDENTIALREQUEST']._serialized_start=17056
+  _globals['_CREATECREDENTIALREQUEST']._serialized_end=17246
+  _globals['_UPDATECREDENTIALREQUEST']._serialized_start=17249
+  _globals['_UPDATECREDENTIALREQUEST']._serialized_end=17454
+  _globals['_DELETECREDENTIALREQUEST']._serialized_start=17456
+  _globals['_DELETECREDENTIALREQUEST']._serialized_end=17563
+  _globals['_LISTCREDUSERSRESPONSE']._serialized_start=17565
+  _globals['_LISTCREDUSERSRESPONSE']._serialized_end=17652
+  _globals['_LISTCREDUSERSREQUEST']._serialized_start=17654
+  _globals['_LISTCREDUSERSREQUEST']._serialized_end=17740
+  _globals['_ROLEENTITY']._serialized_start=17742
+  _globals['_ROLEENTITY']._serialized_end=17768
+  _globals['_USERENTITY']._serialized_start=17770
+  _globals['_USERENTITY']._serialized_end=17796
+  _globals['_CREATEROLEREQUEST']._serialized_start=17799
+  _globals['_CREATEROLEREQUEST']._serialized_end=17931
+  _globals['_DROPROLEREQUEST']._serialized_start=17933
+  _globals['_DROPROLEREQUEST']._serialized_end=18033
+  _globals['_OPERATEUSERROLEREQUEST']._serialized_start=18036
+  _globals['_OPERATEUSERROLEREQUEST']._serialized_end=18217
+  _globals['_SELECTROLEREQUEST']._serialized_start=18220
+  _globals['_SELECTROLEREQUEST']._serialized_end=18377
+  _globals['_ROLERESULT']._serialized_start=18379
+  _globals['_ROLERESULT']._serialized_end=18486
+  _globals['_SELECTROLERESPONSE']._serialized_start=18488
+  _globals['_SELECTROLERESPONSE']._serialized_end=18603
+  _globals['_SELECTUSERREQUEST']._serialized_start=18606
+  _globals['_SELECTUSERREQUEST']._serialized_end=18754
+  _globals['_USERRESULT']._serialized_start=18756
+  _globals['_USERRESULT']._serialized_end=18863
+  _globals['_SELECTUSERRESPONSE']._serialized_start=18865
+  _globals['_SELECTUSERRESPONSE']._serialized_end=18980
+  _globals['_OBJECTENTITY']._serialized_start=18982
+  _globals['_OBJECTENTITY']._serialized_end=19010
+  _globals['_PRIVILEGEENTITY']._serialized_start=19012
+  _globals['_PRIVILEGEENTITY']._serialized_end=19043
+  _globals['_GRANTORENTITY']._serialized_start=19045
+  _globals['_GRANTORENTITY']._serialized_end=19164
+  _globals['_GRANTPRIVILEGEENTITY']._serialized_start=19166
+  _globals['_GRANTPRIVILEGEENTITY']._serialized_end=19242
+  _globals['_GRANTENTITY']._serialized_start=19245
+  _globals['_GRANTENTITY']._serialized_end=19447
+  _globals['_SELECTGRANTREQUEST']._serialized_start=19450
+  _globals['_SELECTGRANTREQUEST']._serialized_end=19584
+  _globals['_SELECTGRANTRESPONSE']._serialized_start=19586
+  _globals['_SELECTGRANTRESPONSE']._serialized_end=19704
+  _globals['_OPERATEPRIVILEGEREQUEST']._serialized_start=19707
+  _globals['_OPERATEPRIVILEGEREQUEST']._serialized_end=19903
+  _globals['_GETLOADINGPROGRESSREQUEST']._serialized_start=19906
+  _globals['_GETLOADINGPROGRESSREQUEST']._serialized_end=20053
+  _globals['_GETLOADINGPROGRESSRESPONSE']._serialized_start=20055
+  _globals['_GETLOADINGPROGRESSRESPONSE']._serialized_end=20172
+  _globals['_GETLOADSTATEREQUEST']._serialized_start=20175
+  _globals['_GETLOADSTATEREQUEST']._serialized_end=20316
+  _globals['_GETLOADSTATERESPONSE']._serialized_start=20318
+  _globals['_GETLOADSTATERESPONSE']._serialized_end=20432
+  _globals['_MILVUSEXT']._serialized_start=20434
+  _globals['_MILVUSEXT']._serialized_end=20462
+  _globals['_GETVERSIONREQUEST']._serialized_start=20464
+  _globals['_GETVERSIONREQUEST']._serialized_end=20483
+  _globals['_GETVERSIONRESPONSE']._serialized_start=20485
+  _globals['_GETVERSIONRESPONSE']._serialized_end=20567
+  _globals['_CHECKHEALTHREQUEST']._serialized_start=20569
+  _globals['_CHECKHEALTHREQUEST']._serialized_end=20589
+  _globals['_CHECKHEALTHRESPONSE']._serialized_start=20592
+  _globals['_CHECKHEALTHRESPONSE']._serialized_end=20749
+  _globals['_CREATERESOURCEGROUPREQUEST']._serialized_start=20752
+  _globals['_CREATERESOURCEGROUPREQUEST']._serialized_end=20922
+  _globals['_UPDATERESOURCEGROUPSREQUEST']._serialized_start=20925
+  _globals['_UPDATERESOURCEGROUPSREQUEST']._serialized_end=21206
+  _globals['_UPDATERESOURCEGROUPSREQUEST_RESOURCEGROUPSENTRY']._serialized_start=21095
+  _globals['_UPDATERESOURCEGROUPSREQUEST_RESOURCEGROUPSENTRY']._serialized_end=21186
+  _globals['_DROPRESOURCEGROUPREQUEST']._serialized_start=21208
+  _globals['_DROPRESOURCEGROUPREQUEST']._serialized_end=21322
+  _globals['_TRANSFERNODEREQUEST']._serialized_start=21325
+  _globals['_TRANSFERNODEREQUEST']._serialized_end=21490
+  _globals['_TRANSFERREPLICAREQUEST']._serialized_start=21493
+  _globals['_TRANSFERREPLICAREQUEST']._serialized_end=21706
+  _globals['_LISTRESOURCEGROUPSREQUEST']._serialized_start=21708
+  _globals['_LISTRESOURCEGROUPSREQUEST']._serialized_end=21799
+  _globals['_LISTRESOURCEGROUPSRESPONSE']._serialized_start=21801
+  _globals['_LISTRESOURCEGROUPSRESPONSE']._serialized_end=21899
+  _globals['_DESCRIBERESOURCEGROUPREQUEST']._serialized_start=21901
+  _globals['_DESCRIBERESOURCEGROUPREQUEST']._serialized_end=22019
+  _globals['_DESCRIBERESOURCEGROUPRESPONSE']._serialized_start=22022
+  _globals['_DESCRIBERESOURCEGROUPRESPONSE']._serialized_end=22158
+  _globals['_RESOURCEGROUP']._serialized_start=22161
+  _globals['_RESOURCEGROUP']._serialized_end=22759
+  _globals['_RESOURCEGROUP_NUMLOADEDREPLICAENTRY']._serialized_start=22592
+  _globals['_RESOURCEGROUP_NUMLOADEDREPLICAENTRY']._serialized_end=22647
+  _globals['_RESOURCEGROUP_NUMOUTGOINGNODEENTRY']._serialized_start=22649
+  _globals['_RESOURCEGROUP_NUMOUTGOINGNODEENTRY']._serialized_end=22703
+  _globals['_RESOURCEGROUP_NUMINCOMINGNODEENTRY']._serialized_start=22705
+  _globals['_RESOURCEGROUP_NUMINCOMINGNODEENTRY']._serialized_end=22759
+  _globals['_RENAMECOLLECTIONREQUEST']._serialized_start=22762
+  _globals['_RENAMECOLLECTIONREQUEST']._serialized_end=22921
+  _globals['_GETINDEXSTATISTICSREQUEST']._serialized_start=22924
+  _globals['_GETINDEXSTATISTICSREQUEST']._serialized_end=23085
+  _globals['_GETINDEXSTATISTICSRESPONSE']._serialized_start=23088
+  _globals['_GETINDEXSTATISTICSRESPONSE']._serialized_end=23228
+  _globals['_CONNECTREQUEST']._serialized_start=23230
+  _globals['_CONNECTREQUEST']._serialized_end=23344
+  _globals['_CONNECTRESPONSE']._serialized_start=23347
+  _globals['_CONNECTRESPONSE']._serialized_end=23483
+  _globals['_ALLOCTIMESTAMPREQUEST']._serialized_start=23485
+  _globals['_ALLOCTIMESTAMPREQUEST']._serialized_end=23552
+  _globals['_ALLOCTIMESTAMPRESPONSE']._serialized_start=23554
+  _globals['_ALLOCTIMESTAMPRESPONSE']._serialized_end=23642
+  _globals['_CREATEDATABASEREQUEST']._serialized_start=23644
+  _globals['_CREATEDATABASEREQUEST']._serialized_end=23748
+  _globals['_DROPDATABASEREQUEST']._serialized_start=23750
+  _globals['_DROPDATABASEREQUEST']._serialized_end=23852
+  _globals['_LISTDATABASESREQUEST']._serialized_start=23854
+  _globals['_LISTDATABASESREQUEST']._serialized_end=23920
+  _globals['_LISTDATABASESRESPONSE']._serialized_start=23922
+  _globals['_LISTDATABASESRESPONSE']._serialized_end=24035
+  _globals['_ALTERDATABASEREQUEST']._serialized_start=24038
+  _globals['_ALTERDATABASEREQUEST']._serialized_end=24211
+  _globals['_DESCRIBEDATABASEREQUEST']._serialized_start=24213
+  _globals['_DESCRIBEDATABASEREQUEST']._serialized_end=24299
+  _globals['_DESCRIBEDATABASERESPONSE']._serialized_start=24302
+  _globals['_DESCRIBEDATABASERESPONSE']._serialized_end=24486
+  _globals['_REPLICATEMESSAGEREQUEST']._serialized_start=24489
+  _globals['_REPLICATEMESSAGEREQUEST']._serialized_end=24734
+  _globals['_REPLICATEMESSAGERESPONSE']._serialized_start=24736
+  _globals['_REPLICATEMESSAGERESPONSE']._serialized_end=24825
+  _globals['_IMPORTAUTHPLACEHOLDER']._serialized_start=24827
+  _globals['_IMPORTAUTHPLACEHOLDER']._serialized_end=24925
+  _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_start=24927
+  _globals['_GETIMPORTPROGRESSAUTHPLACEHOLDER']._serialized_end=24987
+  _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_start=24989
+  _globals['_LISTIMPORTSAUTHPLACEHOLDER']._serialized_end=25068
+  _globals['_MILVUSSERVICE']._serialized_start=25318
+  _globals['_MILVUSSERVICE']._serialized_end=34080
+  _globals['_PROXYSERVICE']._serialized_start=34082
+  _globals['_PROXYSERVICE']._serialized_end=34199
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2.pyi` & `pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -827,15 +827,15 @@
     COLLECTION_NAMES_FIELD_NUMBER: _ClassVar[int]
     base: _common_pb2.MsgBase
     db_name: str
     collection_names: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, base: _Optional[_Union[_common_pb2.MsgBase, _Mapping]] = ..., db_name: _Optional[str] = ..., collection_names: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class FlushResponse(_message.Message):
-    __slots__ = ("status", "db_name", "coll_segIDs", "flush_coll_segIDs", "coll_seal_times", "coll_flush_ts")
+    __slots__ = ("status", "db_name", "coll_segIDs", "flush_coll_segIDs", "coll_seal_times", "coll_flush_ts", "channel_cps")
     class CollSegIDsEntry(_message.Message):
         __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: _schema_pb2.LongArray
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_schema_pb2.LongArray, _Mapping]] = ...) -> None: ...
@@ -856,27 +856,36 @@
     class CollFlushTsEntry(_message.Message):
         __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: int
         def __init__(self, key: _Optional[str] = ..., value: _Optional[int] = ...) -> None: ...
+    class ChannelCpsEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: _msg_pb2.MsgPosition
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_msg_pb2.MsgPosition, _Mapping]] = ...) -> None: ...
     STATUS_FIELD_NUMBER: _ClassVar[int]
     DB_NAME_FIELD_NUMBER: _ClassVar[int]
     COLL_SEGIDS_FIELD_NUMBER: _ClassVar[int]
     FLUSH_COLL_SEGIDS_FIELD_NUMBER: _ClassVar[int]
     COLL_SEAL_TIMES_FIELD_NUMBER: _ClassVar[int]
     COLL_FLUSH_TS_FIELD_NUMBER: _ClassVar[int]
+    CHANNEL_CPS_FIELD_NUMBER: _ClassVar[int]
     status: _common_pb2.Status
     db_name: str
     coll_segIDs: _containers.MessageMap[str, _schema_pb2.LongArray]
     flush_coll_segIDs: _containers.MessageMap[str, _schema_pb2.LongArray]
     coll_seal_times: _containers.ScalarMap[str, int]
     coll_flush_ts: _containers.ScalarMap[str, int]
-    def __init__(self, status: _Optional[_Union[_common_pb2.Status, _Mapping]] = ..., db_name: _Optional[str] = ..., coll_segIDs: _Optional[_Mapping[str, _schema_pb2.LongArray]] = ..., flush_coll_segIDs: _Optional[_Mapping[str, _schema_pb2.LongArray]] = ..., coll_seal_times: _Optional[_Mapping[str, int]] = ..., coll_flush_ts: _Optional[_Mapping[str, int]] = ...) -> None: ...
+    channel_cps: _containers.MessageMap[str, _msg_pb2.MsgPosition]
+    def __init__(self, status: _Optional[_Union[_common_pb2.Status, _Mapping]] = ..., db_name: _Optional[str] = ..., coll_segIDs: _Optional[_Mapping[str, _schema_pb2.LongArray]] = ..., flush_coll_segIDs: _Optional[_Mapping[str, _schema_pb2.LongArray]] = ..., coll_seal_times: _Optional[_Mapping[str, int]] = ..., coll_flush_ts: _Optional[_Mapping[str, int]] = ..., channel_cps: _Optional[_Mapping[str, _msg_pb2.MsgPosition]] = ...) -> None: ...
 
 class QueryRequest(_message.Message):
     __slots__ = ("base", "db_name", "collection_name", "expr", "output_fields", "partition_names", "travel_timestamp", "guarantee_timestamp", "query_params", "not_return_all_meta", "consistency_level", "use_default_consistency")
     BASE_FIELD_NUMBER: _ClassVar[int]
     DB_NAME_FIELD_NUMBER: _ClassVar[int]
     COLLECTION_NAME_FIELD_NUMBER: _ClassVar[int]
     EXPR_FIELD_NUMBER: _ClassVar[int]
@@ -1893,14 +1902,36 @@
     PROPERTIES_FIELD_NUMBER: _ClassVar[int]
     base: _common_pb2.MsgBase
     db_name: str
     db_id: str
     properties: _containers.RepeatedCompositeFieldContainer[_common_pb2.KeyValuePair]
     def __init__(self, base: _Optional[_Union[_common_pb2.MsgBase, _Mapping]] = ..., db_name: _Optional[str] = ..., db_id: _Optional[str] = ..., properties: _Optional[_Iterable[_Union[_common_pb2.KeyValuePair, _Mapping]]] = ...) -> None: ...
 
+class DescribeDatabaseRequest(_message.Message):
+    __slots__ = ("base", "db_name")
+    BASE_FIELD_NUMBER: _ClassVar[int]
+    DB_NAME_FIELD_NUMBER: _ClassVar[int]
+    base: _common_pb2.MsgBase
+    db_name: str
+    def __init__(self, base: _Optional[_Union[_common_pb2.MsgBase, _Mapping]] = ..., db_name: _Optional[str] = ...) -> None: ...
+
+class DescribeDatabaseResponse(_message.Message):
+    __slots__ = ("status", "db_name", "dbID", "created_timestamp", "properties")
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    DB_NAME_FIELD_NUMBER: _ClassVar[int]
+    DBID_FIELD_NUMBER: _ClassVar[int]
+    CREATED_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    PROPERTIES_FIELD_NUMBER: _ClassVar[int]
+    status: _common_pb2.Status
+    db_name: str
+    dbID: int
+    created_timestamp: int
+    properties: _containers.RepeatedCompositeFieldContainer[_common_pb2.KeyValuePair]
+    def __init__(self, status: _Optional[_Union[_common_pb2.Status, _Mapping]] = ..., db_name: _Optional[str] = ..., dbID: _Optional[int] = ..., created_timestamp: _Optional[int] = ..., properties: _Optional[_Iterable[_Union[_common_pb2.KeyValuePair, _Mapping]]] = ...) -> None: ...
+
 class ReplicateMessageRequest(_message.Message):
     __slots__ = ("base", "channel_name", "BeginTs", "EndTs", "Msgs", "StartPositions", "EndPositions")
     BASE_FIELD_NUMBER: _ClassVar[int]
     CHANNEL_NAME_FIELD_NUMBER: _ClassVar[int]
     BEGINTS_FIELD_NUMBER: _ClassVar[int]
     ENDTS_FIELD_NUMBER: _ClassVar[int]
     MSGS_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/milvus_pb2_grpc.py` & `pymilvus-2.4.2/pymilvus/grpc_gen/milvus_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,14 +432,19 @@
                 response_deserializer=milvus__pb2.ListDatabasesResponse.FromString,
                 )
         self.AlterDatabase = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/AlterDatabase',
                 request_serializer=milvus__pb2.AlterDatabaseRequest.SerializeToString,
                 response_deserializer=common__pb2.Status.FromString,
                 )
+        self.DescribeDatabase = channel.unary_unary(
+                '/milvus.proto.milvus.MilvusService/DescribeDatabase',
+                request_serializer=milvus__pb2.DescribeDatabaseRequest.SerializeToString,
+                response_deserializer=milvus__pb2.DescribeDatabaseResponse.FromString,
+                )
         self.ReplicateMessage = channel.unary_unary(
                 '/milvus.proto.milvus.MilvusService/ReplicateMessage',
                 request_serializer=milvus__pb2.ReplicateMessageRequest.SerializeToString,
                 response_deserializer=milvus__pb2.ReplicateMessageResponse.FromString,
                 )
 
 
@@ -953,14 +958,20 @@
 
     def AlterDatabase(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def DescribeDatabase(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ReplicateMessage(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
@@ -1382,14 +1393,19 @@
                     response_serializer=milvus__pb2.ListDatabasesResponse.SerializeToString,
             ),
             'AlterDatabase': grpc.unary_unary_rpc_method_handler(
                     servicer.AlterDatabase,
                     request_deserializer=milvus__pb2.AlterDatabaseRequest.FromString,
                     response_serializer=common__pb2.Status.SerializeToString,
             ),
+            'DescribeDatabase': grpc.unary_unary_rpc_method_handler(
+                    servicer.DescribeDatabase,
+                    request_deserializer=milvus__pb2.DescribeDatabaseRequest.FromString,
+                    response_serializer=milvus__pb2.DescribeDatabaseResponse.SerializeToString,
+            ),
             'ReplicateMessage': grpc.unary_unary_rpc_method_handler(
                     servicer.ReplicateMessage,
                     request_deserializer=milvus__pb2.ReplicateMessageRequest.FromString,
                     response_serializer=milvus__pb2.ReplicateMessageResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -2826,14 +2842,31 @@
         return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/AlterDatabase',
             milvus__pb2.AlterDatabaseRequest.SerializeToString,
             common__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def DescribeDatabase(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/milvus.proto.milvus.MilvusService/DescribeDatabase',
+            milvus__pb2.DescribeDatabaseRequest.SerializeToString,
+            milvus__pb2.DescribeDatabaseResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ReplicateMessage(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/msg_pb2.py` & `pymilvus-2.4.2/pymilvus/grpc_gen/msg_pb2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/msg_pb2.pyi` & `pymilvus-2.4.2/pymilvus/grpc_gen/msg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/python_gen.sh` & `pymilvus-2.4.2/pymilvus/grpc_gen/python_gen.sh`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/rg_pb2.py` & `pymilvus-2.4.2/pymilvus/grpc_gen/rg_pb2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/rg_pb2.pyi` & `pymilvus-2.4.2/pymilvus/grpc_gen/rg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/schema_pb2.py` & `pymilvus-2.4.2/pymilvus/grpc_gen/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/grpc_gen/schema_pb2.pyi` & `pymilvus-2.4.2/pymilvus/grpc_gen/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/milvus_client/index.py` & `pymilvus-2.4.2/pymilvus/milvus_client/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/milvus_client/milvus_client.py` & `pymilvus-2.4.2/pymilvus/milvus_client/milvus_client.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/model/__init__.py` & `pymilvus-2.4.2/pymilvus/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/__init__.py` & `pymilvus-2.4.2/pymilvus/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/collection.py` & `pymilvus-2.4.2/pymilvus/orm/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import copy
 import json
 from typing import Dict, List, Optional, Union
 
 import pandas as pd
 
-from pymilvus.client import entity_helper
+from pymilvus.client import entity_helper, utils
 from pymilvus.client.abstract import BaseRanker, SearchResult
 from pymilvus.client.constants import DEFAULT_CONSISTENCY_LEVEL
 from pymilvus.client.types import (
     CompactionPlans,
     CompactionState,
     Replica,
     cmp_consistency_level,
@@ -230,18 +230,18 @@
 
     @property
     def schema(self) -> CollectionSchema:
         """CollectionSchema: schema of the collection."""
         return self._schema
 
     @property
-    def aliases(self, **kwargs) -> list:
+    def aliases(self) -> list:
         """List[str]: all the aliases of the collection."""
         conn = self._get_connection()
-        resp = conn.describe_collection(self._name, **kwargs)
+        resp = conn.describe_collection(self._name)
         return resp["aliases"]
 
     @property
     def description(self) -> str:
         """str: a text description of the collection."""
         return self.schema.description
 
@@ -252,22 +252,22 @@
 
     @property
     def is_empty(self) -> bool:
         """bool: whether the collection is empty or not."""
         return self.num_entities == 0
 
     @property
-    def num_shards(self, **kwargs) -> int:
+    def num_shards(self) -> int:
         """int: number of shards used by the collection."""
         if self._num_shards is None:
-            self._num_shards = self.describe(timeout=kwargs.get("timeout")).get("num_shards")
+            self._num_shards = self.describe().get("num_shards")
         return self._num_shards
 
     @property
-    def num_entities(self, **kwargs) -> int:
+    def num_entities(self) -> int:
         """int: The number of entities in the collection, not real time.
 
         Examples:
             >>> from pymilvus import Collection, FieldSchema, CollectionSchema, DataType
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
@@ -279,15 +279,15 @@
             >>> collection.num_entities
             0
             >>> collection.flush()
             >>> collection.num_entities
             2
         """
         conn = self._get_connection()
-        stats = conn.get_collection_stats(collection_name=self._name, **kwargs)
+        stats = conn.get_collection_stats(collection_name=self._name)
         result = {stat.key: stat.value for stat in stats}
         result["row_count"] = int(result["row_count"])
         return result["row_count"]
 
     @property
     def primary_field(self) -> FieldSchema:
         """FieldSchema: the primary field of the collection."""
@@ -450,15 +450,15 @@
             >>> collection.release()
         """
         conn = self._get_connection()
         conn.release_collection(self._name, timeout=timeout, **kwargs)
 
     def insert(
         self,
-        data: Union[List, pd.DataFrame, Dict, entity_helper.SparseMatrixInputType],
+        data: Union[List, pd.DataFrame, Dict, utils.SparseMatrixInputType],
         partition_name: Optional[str] = None,
         timeout: Optional[float] = None,
         **kwargs,
     ) -> MutationResult:
         """Insert data into the collection.
 
         Args:
@@ -577,15 +577,15 @@
         res = conn.delete(self._name, expr, partition_name, timeout=timeout, **kwargs)
         if kwargs.get("_async", False):
             return MutationFuture(res)
         return MutationResult(res)
 
     def upsert(
         self,
-        data: Union[List, pd.DataFrame, Dict, entity_helper.SparseMatrixInputType],
+        data: Union[List, pd.DataFrame, Dict, utils.SparseMatrixInputType],
         partition_name: Optional[str] = None,
         timeout: Optional[float] = None,
         **kwargs,
     ) -> MutationResult:
         """Upsert data into the collection.
 
         Args:
@@ -651,15 +651,15 @@
             **kwargs,
         )
 
         return MutationFuture(res) if kwargs.get("_async", False) else MutationResult(res)
 
     def search(
         self,
-        data: Union[List, entity_helper.SparseMatrixInputType],
+        data: Union[List, utils.SparseMatrixInputType],
         anns_field: str,
         param: Dict,
         limit: int,
         expr: Optional[str] = None,
         partition_names: Optional[List[str]] = None,
         output_fields: Optional[List[str]] = None,
         timeout: Optional[float] = None,
@@ -786,15 +786,15 @@
             - Total hits: 2, hits ids: [8, 5]
             >>> print(f"- Top1 hit id: {hits[0].id}, score: {hits[0].score} ")
             - Top1 hit id: 8, score: 0.10143111646175385
         """
         if expr is not None and not isinstance(expr, str):
             raise DataTypeNotMatchException(message=ExceptionsMessage.ExprType % type(expr))
 
-        empty_scipy_sparse = entity_helper.sparse_is_scipy_format(data) and (data.shape[0] == 0)
+        empty_scipy_sparse = utils.SciPyHelper.is_scipy_sparse(data) and (data.shape[0] == 0)
         if (isinstance(data, list) and len(data) == 0) or empty_scipy_sparse:
             resp = SearchResult(schema_pb2.SearchResultData())
             return SearchFuture(None) if kwargs.get("_async", False) else resp
 
         conn = self._get_connection()
         resp = conn.search(
             self._name,
@@ -953,15 +953,15 @@
             **kwargs,
         )
 
         return SearchFuture(resp) if kwargs.get("_async", False) else resp
 
     def search_iterator(
         self,
-        data: Union[List, entity_helper.SparseMatrixInputType],
+        data: Union[List, utils.SparseMatrixInputType],
         anns_field: str,
         param: Dict,
         batch_size: Optional[int] = 1000,
         limit: Optional[int] = UNLIMITED,
         expr: Optional[str] = None,
         partition_names: Optional[List[str]] = None,
         output_fields: Optional[List[str]] = None,
@@ -1107,15 +1107,15 @@
             partition_names=partition_names,
             schema=self._schema_dict,
             timeout=timeout,
             **kwargs,
         )
 
     @property
-    def partitions(self, **kwargs) -> List[Partition]:
+    def partitions(self) -> List[Partition]:
         """List[Partition]: List of Partition object.
 
         Raises:
             MilvusException: If anything goes wrong.
 
         Examples:
             >>> from pymilvus import Collection, FieldSchema, CollectionSchema, DataType
@@ -1124,15 +1124,15 @@
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
             ... ])
             >>> collection = Collection("test_collection_partitions", schema)
             >>> collection.partitions
             [{"name": "_default", "description": "", "num_entities": 0}]
         """
         conn = self._get_connection()
-        partition_strs = conn.list_partitions(self._name, **kwargs)
+        partition_strs = conn.list_partitions(self._name)
         partitions = []
         for partition in partition_strs:
             partitions.append(Partition(self, partition, construct_only=True))
         return partitions
 
     def partition(self, partition_name: str, **kwargs) -> Partition:
         """Get the existing partition object according to name. Return None if not existed.
@@ -1248,30 +1248,30 @@
             >>> collection.has_partition("comedy")
             False
         """
         conn = self._get_connection()
         return conn.drop_partition(self._name, partition_name, timeout=timeout, **kwargs)
 
     @property
-    def indexes(self, **kwargs) -> List[Index]:
+    def indexes(self) -> List[Index]:
         """List[Index]: list of indexes of this collection.
 
         Examples:
             >>> from pymilvus import Collection, FieldSchema, CollectionSchema, DataType
             >>> schema = CollectionSchema([
             ...     FieldSchema("film_id", DataType.INT64, is_primary=True),
             ...     FieldSchema("films", dtype=DataType.FLOAT_VECTOR, dim=2)
             ... ])
             >>> collection = Collection("test_collection_indexes", schema)
             >>> collection.indexes
             []
         """
         conn = self._get_connection()
         indexes = []
-        tmp_index = conn.list_indexes(self._name, **kwargs)
+        tmp_index = conn.list_indexes(self._name)
         for index in tmp_index:
             if index is not None:
                 info_dict = {kv.key: kv.value for kv in index.params}
                 if info_dict.get("params"):
                     info_dict["params"] = json.loads(info_dict["params"])
 
                 index_info = Index(
```

### Comparing `pymilvus-2.4.1/pymilvus/orm/connections.py` & `pymilvus-2.4.2/pymilvus/orm/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import copy
 import logging
+import pathlib
 import threading
 import time
 from typing import Callable, Tuple, Union
 from urllib import parse
 
 from pymilvus.client.check import is_legal_address, is_legal_host, is_legal_port
 from pymilvus.client.grpc_handler import GrpcHandler
@@ -353,14 +354,38 @@
                            server.
 
         :example:
             >>> from pymilvus import connections
             >>> connections.connect("test", host="localhost", port="19530")
         """
 
+        if kwargs.get("uri") and parse.urlparse(kwargs["uri"]).scheme.lower() not in [
+            "unix",
+            "http",
+            "https",
+            "tcp",
+        ]:
+            # start and connect milvuslite
+            if kwargs["uri"].endswith("/"):
+                raise ConnectionConfigException(
+                    message=f"Open local milvus failed, {kwargs['uri']} is not a local file path"
+                )
+            parent_path = pathlib.Path(kwargs["uri"]).parent
+            if not parent_path.is_dir():
+                raise ConnectionConfigException(
+                    message=f"Open local milvus failed, dir: {parent_path} is not exists"
+                )
+
+            from milvus_lite.server_manager import server_manager_instance
+
+            local_uri = server_manager_instance.start_and_get_uri(kwargs["uri"])
+            if local_uri is None:
+                raise ConnectionConfigException(message="Open local milvus failed")
+            kwargs["uri"] = local_uri
+
         # kwargs_copy is used for auto reconnect
         kwargs_copy = copy.deepcopy(kwargs)
         kwargs_copy["user"] = user
         kwargs_copy["password"] = password
         kwargs_copy["db_name"] = db_name
         kwargs_copy["token"] = token
```

### Comparing `pymilvus-2.4.1/pymilvus/orm/constants.py` & `pymilvus-2.4.2/pymilvus/orm/constants.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/db.py` & `pymilvus-2.4.2/pymilvus/orm/db.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,7 +40,38 @@
 def list_database(using: str = "default", timeout: Optional[float] = None) -> list:
     """List databases
 
     :return list[str]:
         List of database names, return when operation is successful
     """
     return _get_connection(using).list_database(timeout=timeout)
+
+
+def set_properties(
+    db_name: str,
+    properties: dict,
+    using: str = "default",
+    timeout: Optional[float] = None,
+):
+    """Alter a database using provided database name
+
+    :param db_name: Database name
+    :type  db_name: str
+
+    :param properties: Properties to be set
+    :type  properties: dict
+
+    """
+    _get_connection(using).alter_database(db_name, properties=properties, timeout=timeout)
+
+
+def describe_database(db_name: str, using: str = "default", timeout: Optional[float] = None):
+    """Describe a database using provided database name
+
+    :param db_name: Database name
+    :type  db_name: str
+
+    :return dict:
+        Database information, return when operation is successful
+
+    """
+    return _get_connection(using).describe_database(db_name, timeout=timeout)
```

### Comparing `pymilvus-2.4.1/pymilvus/orm/future.py` & `pymilvus-2.4.2/pymilvus/orm/future.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/index.py` & `pymilvus-2.4.2/pymilvus/orm/index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/iterator.py` & `pymilvus-2.4.2/pymilvus/orm/iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, TypeVar, Union
 
-from pymilvus.client import entity_helper
+from pymilvus.client import entity_helper, utils
 from pymilvus.client.abstract import Hits, LoopBase
 from pymilvus.exceptions import (
     MilvusException,
     ParamError,
 )
 
 from .connections import Connections
@@ -279,15 +279,15 @@
 
 
 class SearchIterator:
     def __init__(
         self,
         connection: Connections,
         collection_name: str,
-        data: Union[List, entity_helper.SparseMatrixInputType],
+        data: Union[List, utils.SparseMatrixInputType],
         ann_field: str,
         param: Dict,
         batch_size: Optional[int] = 1000,
         limit: Optional[int] = UNLIMITED,
         expr: Optional[str] = None,
         partition_names: Optional[List[str]] = None,
         output_fields: Optional[List[str]] = None,
```

### Comparing `pymilvus-2.4.1/pymilvus/orm/mutation.py` & `pymilvus-2.4.2/pymilvus/orm/mutation.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/partition.py` & `pymilvus-2.4.2/pymilvus/orm/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # the License.
 
 from typing import Dict, List, Optional, TypeVar, Union
 
 import pandas as pd
 import ujson
 
-from pymilvus.client import entity_helper
+from pymilvus.client import utils
 from pymilvus.client.abstract import BaseRanker, SearchResult
 from pymilvus.client.types import Replica
 from pymilvus.exceptions import MilvusException
 
 from .mutation import MutationResult
 
 Collection = TypeVar("Collection")
@@ -105,15 +105,15 @@
             >>> partition = Partition(collection, "comedy", "comedy films")
             >>> partition.is_empty
             True
         """
         return self.num_entities == 0
 
     @property
-    def num_entities(self, **kwargs) -> int:
+    def num_entities(self) -> int:
         """int: number of entities in the partition
 
         Examples:
             >>> from pymilvus import connections
             >>> connections.connect()
             >>> from pymilvus import Collection, Partition, FieldSchema, CollectionSchema, DataType
             >>> schema = CollectionSchema([
@@ -128,15 +128,15 @@
             ... ]
             >>> partition.insert(data)
             >>> partition.num_entities
             10
         """
         conn = self._get_connection()
         stats = conn.get_partition_stats(
-            collection_name=self._collection.name, partition_name=self.name, **kwargs
+            collection_name=self._collection.name, partition_name=self.name
         )
         result = {stat.key: stat.value for stat in stats}
         result["row_count"] = int(result["row_count"])
         return result["row_count"]
 
     def flush(self, timeout: Optional[float] = None, **kwargs):
         """Seal all segment in the collection of this partition.
@@ -235,15 +235,15 @@
             partition_names=[self.name],
             timeout=timeout,
             **kwargs,
         )
 
     def insert(
         self,
-        data: Union[List, pd.DataFrame, entity_helper.SparseMatrixInputType],
+        data: Union[List, pd.DataFrame, utils.SparseMatrixInputType],
         timeout: Optional[float] = None,
         **kwargs,
     ) -> MutationResult:
         """Insert data into the partition, the same as Collection.insert(data, [partition])
 
         Args:
             data (``list/tuple/pandas.DataFrame/sparse types``): The specified data to insert
@@ -313,15 +313,15 @@
             >>> test_partition.delete("film_id in [0, 1]")
             (insert count: 0, delete count: 2, upsert count: 0, timestamp: 431044582560759811)
         """
         return self._collection.delete(expr, self.name, timeout=timeout, **kwargs)
 
     def upsert(
         self,
-        data: Union[List, pd.DataFrame, entity_helper.SparseMatrixInputType],
+        data: Union[List, pd.DataFrame, utils.SparseMatrixInputType],
         timeout: Optional[float] = None,
         **kwargs,
     ) -> MutationResult:
         """Upsert data into the collection.
 
         Args:
             data (``list/tuple/pandas.DataFrame/sparse types``): The specified data to upsert
@@ -353,15 +353,15 @@
             >>> res.upsert_count
             10
         """
         return self._collection.upsert(data, self.name, timeout=timeout, **kwargs)
 
     def search(
         self,
-        data: Union[List, entity_helper.SparseMatrixInputType],
+        data: Union[List, utils.SparseMatrixInputType],
         anns_field: str,
         param: Dict,
         limit: int,
         expr: Optional[str] = None,
         output_fields: Optional[List[str]] = None,
         timeout: Optional[float] = None,
         round_decimal: int = -1,
```

### Comparing `pymilvus-2.4.1/pymilvus/orm/prepare.py` & `pymilvus-2.4.2/pymilvus/orm/prepare.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import copy
 from typing import List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
-from pymilvus.client import entity_helper
+from pymilvus.client import utils
 from pymilvus.client.types import DataType
 from pymilvus.exceptions import (
     DataNotMatchException,
     DataTypeNotSupportException,
     ExceptionsMessage,
     ParamError,
     UpsertAutoIDTrueException,
@@ -152,14 +152,14 @@
             entities.append({"name": field.name, "type": field.dtype, "values": d})
 
         return entities
 
     @classmethod
     def prepare_upsert_data(
         cls,
-        data: Union[List, Tuple, pd.DataFrame, entity_helper.SparseMatrixInputType],
+        data: Union[List, Tuple, pd.DataFrame, utils.SparseMatrixInputType],
         schema: CollectionSchema,
     ) -> List:
         if schema.auto_id:
             raise UpsertAutoIDTrueException(message=ExceptionsMessage.UpsertAutoIDTrue)
 
         return cls.prepare_insert_data(data, schema)
```

### Comparing `pymilvus-2.4.1/pymilvus/orm/role.py` & `pymilvus-2.4.2/pymilvus/orm/role.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/schema.py` & `pymilvus-2.4.2/pymilvus/orm/schema.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/types.py` & `pymilvus-2.4.2/pymilvus/orm/types.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/orm/utility.py` & `pymilvus-2.4.2/pymilvus/orm/utility.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus/settings.py` & `pymilvus-2.4.2/pymilvus/settings.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/pymilvus.egg-info/PKG-INFO` & `pymilvus-2.4.2/pymilvus.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilvus
-Version: 2.4.1
+Version: 2.4.2
 Summary: Python Sdk for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/pymilvus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,27 +12,28 @@
 Requires-Dist: setuptools>=67
 Requires-Dist: grpcio<=1.60.0,>=1.49.1
 Requires-Dist: protobuf>=3.20.0
 Requires-Dist: environs<=9.5.0
 Requires-Dist: ujson>=2.0.0
 Requires-Dist: pandas>=1.2.4
 Requires-Dist: numpy<1.25.0; python_version <= "3.8"
-Requires-Dist: requests
-Requires-Dist: minio>=7.0.0
-Requires-Dist: pyarrow>=12.0.0
-Requires-Dist: azure-storage-blob
-Requires-Dist: scipy
+Requires-Dist: milvus_lite<2.5.0,>=2.4.0
+Provides-Extra: bulk-writer
+Requires-Dist: requests; extra == "bulk-writer"
+Requires-Dist: minio>=7.0.0; extra == "bulk-writer"
+Requires-Dist: pyarrow>=12.0.0; extra == "bulk-writer"
+Requires-Dist: azure-storage-blob; extra == "bulk-writer"
 Provides-Extra: model
 Requires-Dist: milvus-model>=0.1.0; extra == "model"
 Provides-Extra: test
 Requires-Dist: pytest>=5.3.4; extra == "test"
 Requires-Dist: pytest-cov>=2.8.1; extra == "test"
 Requires-Dist: pytest-timeout>=1.3.4; extra == "test"
 Requires-Dist: grpcio-testing; extra == "test"
-Requires-Dist: ruff>=0.3.3; extra == "test"
+Requires-Dist: ruff>0.4.0; extra == "test"
 Requires-Dist: black; extra == "test"
 
 # Milvus Python SDK
 
 [![version](https://img.shields.io/pypi/v/pymilvus.svg?color=blue)](https://pypi.org/project/pymilvus/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pymilvus?logo=python&logoColor=blue)](https://pypi.org/project/pymilvus/)
 [![Downloads](https://static.pepy.tech/badge/pymilvus)](https://pepy.tech/project/pymilvus)
```

### Comparing `pymilvus-2.4.1/pymilvus.egg-info/SOURCES.txt` & `pymilvus-2.4.2/pymilvus.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,15 @@
 tests/test_check.py
 tests/test_collection.py
 tests/test_connections.py
 tests/test_create_collection.py
 tests/test_decorators.py
 tests/test_grpc_handler.py
 tests/test_index.py
+tests/test_milvus_lite.py
 tests/test_partition.py
 tests/test_prepare.py
 tests/test_schema.py
 tests/test_ts_utils.py
 tests/test_types.py
 tests/test_utils.py
 tests/utils.py
```

### Comparing `pymilvus-2.4.1/pyproject.toml` & `pymilvus-2.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,42 +20,45 @@
     "setuptools >= 67", # python3.12 pkg_resources
     "grpcio>=1.49.1,<=1.60.0",
     "protobuf>=3.20.0",
     "environs<=9.5.0",
     "ujson>=2.0.0",
     "pandas>=1.2.4",
     "numpy<1.25.0;python_version<='3.8'",
-    "requests",
-    "minio>=7.0.0",
-    "pyarrow>=12.0.0",
-    "azure-storage-blob",
-    "scipy",
+    "milvus_lite>=2.4.0,<2.5.0",
 ]
 
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 "repository" = 'https://github.com/milvus-io/pymilvus'
 
 [project.optional-dependencies]
+bulk_writer = [
+    "requests",
+    "minio>=7.0.0",
+    "pyarrow>=12.0.0",
+    "azure-storage-blob",
+]
+
 model = [
     "milvus-model>=0.1.0",
 ]
 
 test = [
     "pytest>=5.3.4",
     "pytest-cov>=2.8.1",
     "pytest-timeout>=1.3.4",
     "grpcio-testing",
-    "ruff>=0.3.3",
+    "ruff>0.4.0",
     "black",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "_version_helper.version"}
 
 [tool.setuptools_scm]
@@ -109,14 +112,15 @@
     "E501", # black takes care of it
     "ARG005", # [ruff] ARG005 Unused lambda argument: `disable` [E]
     "TRY400",
     "PLR0912", # TODO
     "PLR0915", # To many statements TODO
     "C901", # TODO
     "PYI041", # TODO
+    "E402",
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 lint.fixable = [
     "A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W",
     "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT",
     "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH",
```

### Comparing `pymilvus-2.4.1/requirements.txt` & `pymilvus-2.4.2/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 pep517==0.10.0
 pyparsing==2.4.7
 six==1.16.0
 toml==0.10.2
 ujson>=2.0.0
 urllib3==1.26.18
 m2r==0.3.1
-scipy>=1.9.3
 Sphinx==4.0.0
 sphinx-copybutton
 sphinx-rtd-theme
 sphinxcontrib-applehelp
 sphinxcontrib-devhelp
 sphinxcontrib-htmlhelp
 sphinxcontrib-jsmath
@@ -34,7 +33,8 @@
 pytest-timeout>=1.3.4
 pandas>=1.1.5
 ruff>=0.2.0
 black
 requests
 minio
 azure-storage-blob
+milvus_lite>=2.4.0,<2.5.0
```

### Comparing `pymilvus-2.4.1/tests/conftest.py` & `pymilvus-2.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/mock_milvus.py` & `pymilvus-2.4.2/tests/mock_milvus.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/mock_result.py` & `pymilvus-2.4.2/tests/mock_result.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_abstract.py` & `pymilvus-2.4.2/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_check.py` & `pymilvus-2.4.2/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_collection.py` & `pymilvus-2.4.2/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_connections.py` & `pymilvus-2.4.2/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_create_collection.py` & `pymilvus-2.4.2/tests/test_create_collection.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_decorators.py` & `pymilvus-2.4.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_grpc_handler.py` & `pymilvus-2.4.2/tests/test_grpc_handler.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_index.py` & `pymilvus-2.4.2/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_partition.py` & `pymilvus-2.4.2/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_prepare.py` & `pymilvus-2.4.2/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_schema.py` & `pymilvus-2.4.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_ts_utils.py` & `pymilvus-2.4.2/tests/test_ts_utils.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/test_types.py` & `pymilvus-2.4.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pymilvus-2.4.1/tests/utils.py` & `pymilvus-2.4.2/tests/utils.py`

 * *Files identical despite different names*

