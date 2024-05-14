# Comparing `tmp/OZI-1.6.4.tar.gz` & `tmp/OZI-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.6.4.tar", last modified: Mon May 13 19:59:22 2024, max compression
+gzip compressed data, was "OZI-1.6.5.tar", last modified: Mon May 13 23:06:58 2024, max compression
```

## Comparing `OZI-1.6.4.tar` & `OZI-1.6.5.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.095290 OZI-1.6.4/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.067290 OZI-1.6.4/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.063290 OZI-1.6.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.067290 OZI-1.6.4/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-13 19:55:42.000000 OZI-1.6.4/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-13 19:55:42.000000 OZI-1.6.4/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   307079 2024-05-13 19:55:42.000000 OZI-1.6.4/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-13 19:55:42.000000 OZI-1.6.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-13 19:58:59.851291 OZI-1.6.4/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-13 19:55:42.000000 OZI-1.6.4/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-13 19:55:42.000000 OZI-1.6.4/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-13 19:55:42.000000 OZI-1.6.4/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.091290 OZI-1.6.4/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.075290 OZI-1.6.4/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.075290 OZI-1.6.4/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.075290 OZI-1.6.4/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.075290 OZI-1.6.4/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3659 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.079290 OZI-1.6.4/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.079290 OZI-1.6.4/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.079290 OZI-1.6.4/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.079290 OZI-1.6.4/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.079290 OZI-1.6.4/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.079290 OZI-1.6.4/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.079290 OZI-1.6.4/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.079290 OZI-1.6.4/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.083290 OZI-1.6.4/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6765 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.083290 OZI-1.6.4/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.087290 OZI-1.6.4/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6245 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4484 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.087290 OZI-1.6.4/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.087290 OZI-1.6.4/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.087290 OZI-1.6.4/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.091290 OZI-1.6.4/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.091290 OZI-1.6.4/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-13 19:55:42.000000 OZI-1.6.4/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11109 2024-05-13 19:55:42.000000 OZI-1.6.4/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      206 2024-05-13 19:55:42.000000 OZI-1.6.4/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.091290 OZI-1.6.4/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-13 19:55:42.000000 OZI-1.6.4/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:59:00.095290 OZI-1.6.4/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-13 19:55:42.000000 OZI-1.6.4/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-13 19:55:42.000000 OZI-1.6.4/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14168 2024-05-13 19:55:42.000000 OZI-1.6.4/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-13 19:55:42.000000 OZI-1.6.4/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.034928 OZI-1.6.5/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.034928 OZI-1.6.5/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.034928 OZI-1.6.5/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-13 23:03:18.000000 OZI-1.6.5/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   307353 2024-05-13 23:03:18.000000 OZI-1.6.5/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-13 23:03:18.000000 OZI-1.6.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-13 23:06:35.830928 OZI-1.6.5/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-13 23:03:18.000000 OZI-1.6.5/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-13 23:03:18.000000 OZI-1.6.5/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-13 23:03:18.000000 OZI-1.6.5/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/restructuredtext-lint/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/restructuredtext-lint/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/restructuredtext-lint/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6765 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.054928 OZI-1.6.5/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6245 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4484 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11109 2024-05-13 23:03:18.000000 OZI-1.6.5/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      206 2024-05-13 23:03:18.000000 OZI-1.6.5/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-13 23:03:18.000000 OZI-1.6.5/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-13 23:03:18.000000 OZI-1.6.5/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-13 23:03:18.000000 OZI-1.6.5/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14168 2024-05-13 23:03:18.000000 OZI-1.6.5/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-13 23:03:18.000000 OZI-1.6.5/tests/test_tap.py
```

### Comparing `OZI-1.6.4/.github/CODEOWNERS` & `OZI-1.6.5/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/CODE_OF_CONDUCT.md` & `OZI-1.6.5/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/CONTRIBUTING.md` & `OZI-1.6.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.6.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.6.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/SECURITY.md` & `OZI-1.6.5/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/workflows/codeql.yml` & `OZI-1.6.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/workflows/dependency-review.yml` & `OZI-1.6.5/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/workflows/dev-workflow.yml` & `OZI-1.6.5/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/workflows/dist-workflow.yml` & `OZI-1.6.5/.github/workflows/dist-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.github/workflows/scorecard.yml` & `OZI-1.6.5/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/.gitignore` & `OZI-1.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/CHANGELOG.md` & `OZI-1.6.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,18 @@
 # CHANGELOG
+## 1.6.5 (2024-05-13)
+
+### :bug:
+
+* :bug: Fix bug introduced in ``ozi-fix`` 1.6.4.
+
+missing target positional argument.
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`335558d`](https://github.com/OZI-Project/OZI/commit/335558da5eda61d230990d4429d816455372e143))
+
 ## 1.6.4 (2024-05-13)
 
 ### :bug:
 
 * :bug: Parsers default to target the current working dir.
 
 Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`7628281`](https://github.com/OZI-Project/OZI/commit/7628281ade6849d747f797ad7e29816c0fa7561a))
```

### Comparing `OZI-1.6.4/LICENSE.txt` & `OZI-1.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/PKG-INFO` & `OZI-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.6.4
+Version: 1.6.5
 Summary: Package Python projects with Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.6.4.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.6.5.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
```

### Comparing `OZI-1.6.4/README.rst` & `OZI-1.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/meson.build` & `OZI-1.6.5/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/meson.options` & `OZI-1.6.5/meson.options`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/__main__.py` & `OZI-1.6.5/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/actions.py` & `OZI-1.6.5/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/comment.py` & `OZI-1.6.5/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/fix/__main__.py` & `OZI-1.6.5/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/fix/build_definition.py` & `OZI-1.6.5/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/fix/meson.build` & `OZI-1.6.5/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/fix/missing.py` & `OZI-1.6.5/ozi/fix/missing.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/fix/parser.py` & `OZI-1.6.5/ozi/fix/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,14 @@
 import sys
 from argparse import SUPPRESS
 from argparse import ArgumentParser
 from argparse import BooleanOptionalAction
 
 parser = ArgumentParser(description=sys.modules[__name__].__doc__, add_help=False)
 subparser = parser.add_subparsers(help='source & test fix', dest='fix')
-parser.add_argument(
-    'target',
-    type=str,
-    nargs='?',
-    default='.',
-    help='target OZI project directory',
-)
 
 helpers = parser.add_mutually_exclusive_group()
 helpers.add_argument('-h', '--help', action='help', help='show this help message and exit')
 missing_parser = subparser.add_parser(
     'missing',
     aliases=['m'],
     allow_abbrev=True,
@@ -49,14 +42,21 @@
 )
 missing_parser.add_argument(
     '--pretty',
     default=False,
     action=BooleanOptionalAction,
     help='pretty mode outputs indented json, default: --no-pretty',
 )
+missing_parser.add_argument(
+    'target',
+    type=str,
+    nargs='?',
+    default='.',
+    help='target OZI project directory',
+)
 source_parser = subparser.add_parser(
     'source',
     aliases=['s'],
     allow_abbrev=True,
     help='Create a new Python source in an OZI project.',
 )
 test_parser = subparser.add_parser(
@@ -84,14 +84,21 @@
 source_parser.add_argument(
     '--copyright-head',
     type=str,
     default='',
     help='copyright header string',
     metavar='Part of the NAME project.\\nSee LICENSE...',
 )
+source_parser.add_argument(
+    'target',
+    type=str,
+    nargs='?',
+    default='.',
+    help='target OZI project directory',
+)
 source_output = source_parser.add_argument_group('output')
 source_output.add_argument(
     '--strict',
     default=False,
     action=BooleanOptionalAction,
     help='strict mode raises warnings to errors.',
 )
@@ -120,14 +127,21 @@
 test_parser.add_argument(
     '--copyright-head',
     type=str,
     default='',
     help='copyright header string',
     metavar='Part of the NAME project.\\nSee LICENSE...',
 )
+test_parser.add_argument(
+    'target',
+    type=str,
+    nargs='?',
+    default='.',
+    help='target OZI project directory',
+)
 test_output = test_parser.add_argument_group('output')
 test_output.add_argument(
     '--strict',
     default=False,
     action=BooleanOptionalAction,
     help='strict mode raises warnings to errors.',
 )
```

### Comparing `OZI-1.6.4/ozi/fix/rewrite_command.py` & `OZI-1.6.5/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/lint/meson.build` & `OZI-1.6.5/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/lint/pyright/meson.build` & `OZI-1.6.5/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/meson.build` & `OZI-1.6.5/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/meson.py` & `OZI-1.6.5/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/new/__main__.py` & `OZI-1.6.5/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/new/meson.build` & `OZI-1.6.5/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/new/parser.py` & `OZI-1.6.5/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/new/validate.py` & `OZI-1.6.5/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/pkg_extra.py` & `OZI-1.6.5/ozi/pkg_extra.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/render.py` & `OZI-1.6.5/ozi/render.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/core_metadata_template.py` & `OZI-1.6.5/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/meson.build` & `OZI-1.6.5/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.6.5/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.6.5/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/render_requirements.py` & `OZI-1.6.5/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.6.5/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/scm_version_snip.py` & `OZI-1.6.5/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/to_distribution_template.py` & `OZI-1.6.5/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/scripts/version_metadata_template.py` & `OZI-1.6.5/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spdx.py` & `OZI-1.6.5/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/_license.py` & `OZI-1.6.5/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/_spec.py` & `OZI-1.6.5/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/base.py` & `OZI-1.6.5/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/ci.py` & `OZI-1.6.5/ozi/spec/ci.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/meson.build` & `OZI-1.6.5/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/pkg.py` & `OZI-1.6.5/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/project.py` & `OZI-1.6.5/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/python.py` & `OZI-1.6.5/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/spec/src.py` & `OZI-1.6.5/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/tap.py` & `OZI-1.6.5/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/trove.py` & `OZI-1.6.5/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/email_validator/__init__.py` & `OZI-1.6.5/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/email_validator/__main__.py` & `OZI-1.6.5/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/email_validator/deliverability.py` & `OZI-1.6.5/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.6.5/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/email_validator/meson.build` & `OZI-1.6.5/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.6.5/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/email_validator/syntax.py` & `OZI-1.6.5/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/email_validator/validate_email.py` & `OZI-1.6.5/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/ozi/vendor/meson.build` & `OZI-1.6.5/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/pyproject.toml` & `OZI-1.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/templates/CHANGELOG.md.j2` & `OZI-1.6.5/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/tests/meson.build` & `OZI-1.6.5/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/tests/test_ozi_fix.py` & `OZI-1.6.5/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/tests/test_ozi_new.py` & `OZI-1.6.5/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.4/tests/test_tap.py` & `OZI-1.6.5/tests/test_tap.py`

 * *Files identical despite different names*

