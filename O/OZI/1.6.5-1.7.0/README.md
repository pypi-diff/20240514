# Comparing `tmp/OZI-1.6.5.tar.gz` & `tmp/OZI-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.6.5.tar", last modified: Mon May 13 23:06:58 2024, max compression
+gzip compressed data, was "OZI-1.7.0.tar", last modified: Tue May 14 08:44:39 2024, max compression
```

## Comparing `OZI-1.6.5.tar` & `OZI-1.7.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.034928 OZI-1.6.5/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.034928 OZI-1.6.5/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.034928 OZI-1.6.5/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-13 23:03:18.000000 OZI-1.6.5/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-13 23:03:18.000000 OZI-1.6.5/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   307353 2024-05-13 23:03:18.000000 OZI-1.6.5/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-13 23:03:18.000000 OZI-1.6.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-13 23:06:35.830928 OZI-1.6.5/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-13 23:03:18.000000 OZI-1.6.5/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16724 2024-05-13 23:03:18.000000 OZI-1.6.5/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7664 2024-05-13 23:03:18.000000 OZI-1.6.5/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6305 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.046928 OZI-1.6.5/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      553 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/lint/restructuredtext-lint/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/restructuredtext-lint/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       21 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/lint/restructuredtext-lint/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.050928 OZI-1.6.5/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6765 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2606 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.054928 OZI-1.6.5/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6245 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4484 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4572 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.058928 OZI-1.6.5/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-13 23:03:18.000000 OZI-1.6.5/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11109 2024-05-13 23:03:18.000000 OZI-1.6.5/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      206 2024-05-13 23:03:18.000000 OZI-1.6.5/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-13 23:03:18.000000 OZI-1.6.5/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:06:36.062928 OZI-1.6.5/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-13 23:03:18.000000 OZI-1.6.5/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-13 23:03:18.000000 OZI-1.6.5/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14168 2024-05-13 23:03:18.000000 OZI-1.6.5/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-13 23:03:18.000000 OZI-1.6.5/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.284503 OZI-1.7.0/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.256503 OZI-1.7.0/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.256503 OZI-1.7.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.256503 OZI-1.7.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-14 08:40:58.000000 OZI-1.7.0/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-14 08:40:58.000000 OZI-1.7.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   307793 2024-05-14 08:40:58.000000 OZI-1.7.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-14 08:40:58.000000 OZI-1.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-14 08:44:16.048501 OZI-1.7.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-14 08:40:58.000000 OZI-1.7.0/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    16774 2024-05-14 08:40:58.000000 OZI-1.7.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7660 2024-05-14 08:40:58.000000 OZI-1.7.0/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.280503 OZI-1.7.0/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.268503 OZI-1.7.0/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.268503 OZI-1.7.0/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.268503 OZI-1.7.0/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.268503 OZI-1.7.0/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6321 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.272503 OZI-1.7.0/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.268503 OZI-1.7.0/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.268503 OZI-1.7.0/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.268503 OZI-1.7.0/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.272503 OZI-1.7.0/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.272503 OZI-1.7.0/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.272503 OZI-1.7.0/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.272503 OZI-1.7.0/ozi/lint/readme-renderer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/readme-renderer/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       15 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/lint/readme-renderer/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.272503 OZI-1.7.0/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4813 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6940 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3128 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.276503 OZI-1.7.0/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.280503 OZI-1.7.0/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6233 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4480 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4564 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.280503 OZI-1.7.0/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.280503 OZI-1.7.0/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.280503 OZI-1.7.0/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.284503 OZI-1.7.0/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.284503 OZI-1.7.0/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-14 08:40:58.000000 OZI-1.7.0/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11225 2024-05-14 08:40:58.000000 OZI-1.7.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      206 2024-05-14 08:40:58.000000 OZI-1.7.0/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.284503 OZI-1.7.0/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-14 08:40:58.000000 OZI-1.7.0/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:44:16.284503 OZI-1.7.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-14 08:40:58.000000 OZI-1.7.0/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-14 08:40:58.000000 OZI-1.7.0/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14348 2024-05-14 08:40:58.000000 OZI-1.7.0/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-14 08:40:58.000000 OZI-1.7.0/tests/test_tap.py
```

### Comparing `OZI-1.6.5/.github/CODEOWNERS` & `OZI-1.7.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/CODE_OF_CONDUCT.md` & `OZI-1.7.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/CONTRIBUTING.md` & `OZI-1.7.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/SECURITY.md` & `OZI-1.7.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/workflows/codeql.yml` & `OZI-1.7.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/workflows/dependency-review.yml` & `OZI-1.7.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/workflows/dev-workflow.yml` & `OZI-1.7.0/.github/workflows/dev-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/workflows/dist-workflow.yml` & `OZI-1.7.0/.github/workflows/dist-workflow.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.github/workflows/scorecard.yml` & `OZI-1.7.0/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/.gitignore` & `OZI-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/CHANGELOG.md` & `OZI-1.7.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,22 @@
 # CHANGELOG
+## 1.7.0 (2024-05-14)
+
+### :sparkles:
+
+* :sparkles: markdown and plaintext readmes.
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`bf5f5ac`](https://github.com/OZI-Project/OZI/commit/bf5f5ac5c4824b82be8b29b496025b28a6b3ffce))
+
+### Other
+
+* Update pyproject.toml
+
+Signed-off-by: Eden Ross Duff, MSc &lt;ozi.project@outlook.com&gt; ([`2e4d278`](https://github.com/OZI-Project/OZI/commit/2e4d2781177aead20e41ea24cd9586e30113f361))
+
 ## 1.6.5 (2024-05-13)
 
 ### :bug:
 
 * :bug: Fix bug introduced in ``ozi-fix`` 1.6.4.
 
 missing target positional argument.
```

### Comparing `OZI-1.6.5/LICENSE.txt` & `OZI-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/PKG-INFO` & `OZI-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.6.5
+Version: 1.7.0
 Summary: Package Python projects with Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.6.5.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.7.0.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
-Requires-Dist: blastpipe~=2024.6.3
+Requires-Dist: blastpipe~=2024.7.4
 Requires-Dist: GitPython>=3
 Requires-Dist: dnspython
 Requires-Dist: idna>=2
 Requires-Dist: jinja2>=3
 Requires-Dist: meson>=1.1.0
 Requires-Dist: packaging~=24.0
 Requires-Dist: pyparsing~=3.1
```

### Comparing `OZI-1.6.5/README.rst` & `OZI-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/meson.build` & `OZI-1.7.0/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
     suite.enable_auto_if(dev.enabled())
     set_variable(name, suite)
     foreach command : command_names
         if suite.enabled()
             message('installing', command)
         endif
         if suite.enabled() and command in module_only
-            modules += [command]
+            modules += [command.underscorify()]  # we should collapse repeated `_`
         endif
         flag = disabler()
         if (
             (get_option('dev').enabled() or suite.enabled())
             and command not in plugin_only
         )
             run_command(
```

### Comparing `OZI-1.6.5/meson.options` & `OZI-1.7.0/meson.options`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         'flake8-bugbear',
         'flake8-datetimez',
         'flake8-no-pep420',
         'flake8-comprehensions',
         'flake8-leading-blank-lines',
         'flake8-tidy-imports',
         'flake8-pyi',
-        'restructuredtext-lint',
+        'readme-renderer',
     ],
 )
 option(
     'test-suite',
     type: 'array',
     description: '--setup=test',
     value: [
@@ -196,14 +196,15 @@
         'coverage',
         'flake8',
         'bandit',
         'black',
         'isort',
         'pyright',
         'mypy',
+        'readme-renderer',
     ],
 )
 # test application arguments
 option('args-sigstore', type: 'array', value: ['--version'], yield: true)
 option(
     'args-semantic_release',
     type: 'array',
@@ -273,17 +274,17 @@
       '--verbose',
       '@build_root@',
    ],
    yield: true
 )
 option('args-coverage', type: 'array', value: ['debug', 'config'], yield: true)
 option(
-    'args-restructuredtext-lint',
+    'args-readme-renderer',
     type: 'array',
-    value: ['--level=warning', 'README.rst'],
+    value: ['README.rst'],
     yield: true,
 )
 option(
     'args-flake8',
     type: 'array',
     value: [
         '--toml-config=pyproject.toml',
```

### Comparing `OZI-1.6.5/ozi/__main__.py` & `OZI-1.7.0/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/actions.py` & `OZI-1.7.0/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/comment.py` & `OZI-1.7.0/ozi/comment.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/fix/__main__.py` & `OZI-1.7.0/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/fix/build_definition.py` & `OZI-1.7.0/ozi/fix/build_definition.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/fix/meson.build` & `OZI-1.7.0/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/fix/missing.py` & `OZI-1.7.0/ozi/fix/missing.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """Render PKG-INFO as it would be produced during packaging."""
     with target.joinpath('pyproject.toml').open('rb') as f:
         setuptools_scm = toml.load(f).get('tool', {}).get('setuptools_scm', {})
         return message_from_string(
             setuptools_scm.get('version_file_template', '@README_TEXT@')
             .replace(
                 '@README_TEXT@',
-                target.joinpath('README.rst').read_text(),
+                target.joinpath('README').read_text(),
             )
             .replace('@PROJECT_NAME@', name)
             .replace('@LICENSE@', _license)
             .replace('@REQUIREMENTS_IN@\n', render_requirements(target))
             .replace('@SCM_VERSION@', '{version}'),
         )
 
@@ -122,15 +122,15 @@
             rel_path = Path(underscorify(name))
             expected_files = METADATA.spec.python.src.required.source
         case _:  # pragma: no cover
             rel_path = Path('.')
             expected_files = ()
     for file in expected_files:
         f = rel_path / file
-        if not target.joinpath(f).exists():
+        if not target.joinpath(f).exists():  # pragma: no cover
             TAP.not_ok('MISSING', str(f))
             continue  # pragma: defer to https://github.com/nedbat/coveragepy/issues/198
         TAP.ok(str(f))
         found_files.append(file)
     walk(target, rel_path, found_files=found_files, project_name=underscorify(name))
     return found_files
```

### Comparing `OZI-1.6.5/ozi/fix/parser.py` & `OZI-1.7.0/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/fix/rewrite_command.py` & `OZI-1.7.0/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/lint/meson.build` & `OZI-1.7.0/ozi/meson.build`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,36 @@
-# ozi/scripts/lint/meson.build
+# ozi/meson.build
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
-source_child_lint_children = [
-    'bandit',
-    'black',
-    'flake8',
-    'isort',
-    'mypy',
-    'pyright',
-    'restructuredtext-lint',
+source_files = [
+    '__init__.py',
+    '__main__.py',
+    'actions.py',
+    'comment.py',
+    'meson.py',
+    'pkg_extra.py',
+    'py.typed',
+    'render.py',
+    'spdx.py',
+    'tap.py',
+    'trove.py',
 ]
-if (get_option('dev').enabled() or get_option('lint').enabled())
-    foreach package : source_child_lint_children
-        message('configuring', package)
-        subdir(package)
-    endforeach
-endif
+foreach file : files(source_files)
+    fs.copyfile(file)
+    if not meson.is_subproject() or get_option('install-subprojects').enabled()
+        python.install_sources(file, pure: true, subdir: 'ozi')
+    endif
+endforeach
+source_children = [
+    'dist',
+    'fix',
+    'lint',
+    'new',
+    'scripts',
+    'spec',
+    'test',
+    'vendor',
+]
+foreach child: source_children
+    subdir(child)
+endforeach
```

### Comparing `OZI-1.6.5/ozi/lint/pyright/meson.build` & `OZI-1.7.0/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/meson.py` & `OZI-1.7.0/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/new/__main__.py` & `OZI-1.7.0/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/new/meson.build` & `OZI-1.7.0/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/new/parser.py` & `OZI-1.7.0/ozi/new/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -210,14 +210,21 @@
     '--status',
     '--development-status',
     action=CloseMatch,
     default=METADATA.spec.python.pkg.info.classifiers.development_status,
     help='Classifier: Development Status (Single Use)(default: "1 - Planning")',
     type=str,
 )
+defaults.add_argument(
+    '--long-description-content-type',
+    '--readme-type',
+    default='rst',
+    choices=('rst', 'md', 'txt'),
+    help='Description-Content-Type',
+)
 optional.add_argument(
     '-r',
     '--dist-requires',
     help='Dist-Requires (Multiple Use)',
     action='append',
     type=str,
     nargs='?',
```

### Comparing `OZI-1.6.5/ozi/new/validate.py` & `OZI-1.7.0/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/pkg_extra.py` & `OZI-1.7.0/ozi/pkg_extra.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,28 +19,50 @@
 
 from ozi.spdx import spdx_license_expression
 
 sspace = Suppress(White(' ', exact=1))
 dcolon = sspace + Suppress(Literal('::')) + sspace
 classifier = Suppress(White(' ', min=2)) + Suppress(Literal('Classifier:')) + sspace
 pep639_headers = Forward()
+pep639_headers_md = Forward()
 license_expression = classifier + (
     Keyword('License-Expression')
     + dcolon
     + Combine(spdx_license_expression, join_string=' ')
 ).set_parse_action(lambda t: {str(t[0]): str(t[1])})
 license_file = classifier + (
     Keyword('License-File') + dcolon + oneOf(['LICENSE', 'LICENSE.txt'])
 ).set_parse_action(lambda t: {str(t[0]): str(t[1])})
 pep639_headers <<= license_expression + license_file
+pep639_headers_md <<= (
+    Suppress(
+        Keyword('[comment]') + Literal('#') + Literal('('),
+    )
+    + license_expression
+    + Suppress(Literal(')'))
+    + Suppress(
+        Keyword('[comment]') + Literal('#') + Literal('('),
+    )
+    + license_file
+    + Suppress(Literal(')'))
+)
 extra_classifiers_comment = (
     Suppress(
         Keyword('..') + CaselessKeyword('ozi'),
     )
     + pep639_headers
+    | Suppress(
+        Keyword('[comment]')
+        + Keyword('#')
+        + Literal('(')
+        + Keyword('..')
+        + CaselessKeyword('ozi')
+        + Literal(')'),
+    )
+    + pep639_headers_md
 )
 
 
 def _str_dict_union(toks: ParseResults) -> Any | ParseResults:
     """Parse-time union of dict[str, str]."""
     if len(toks) >= 2:
         return dict(toks[0]) | dict(toks[1])
```

### Comparing `OZI-1.6.5/ozi/render.py` & `OZI-1.7.0/ozi/render.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/core_metadata_template.py` & `OZI-1.7.0/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/meson.build` & `OZI-1.7.0/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.7.0/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.7.0/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/render_requirements.py` & `OZI-1.7.0/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.7.0/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/scm_version_snip.py` & `OZI-1.7.0/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/to_distribution_template.py` & `OZI-1.7.0/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/scripts/version_metadata_template.py` & `OZI-1.7.0/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/spdx.py` & `OZI-1.7.0/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/spec/_license.py` & `OZI-1.7.0/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/spec/_spec.py` & `OZI-1.7.0/ozi/spec/_spec.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/spec/base.py` & `OZI-1.7.0/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/spec/ci.py` & `OZI-1.7.0/ozi/spec/ci.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         default_factory=lambda: {
             'bandit': 'bandit[toml]',
             'black': 'black>=24.3',
             'flake8': 'flake8',
             'isort': 'isort',
             'mypy': 'mypy',
             'pyright': 'pyright',
-            'restructuredtext-lint': 'restructuredtext-lint',
+            'readme-renderer': 'readme-renderer',
         },
     )
     plugin: Mapping[str, str] = field(
         default_factory=lambda: {
             'Flake8-pyproject': 'Flake8-pyproject',
             'flake8-annotations': 'flake8-annotations',
             'flake8-broken-line': 'flake8-broken-line',
```

### Comparing `OZI-1.6.5/ozi/spec/meson.build` & `OZI-1.7.0/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/spec/pkg.py` & `OZI-1.7.0/ozi/spec/pkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class PkgRequired(Default):
     """Required files for OZI project publishing."""
 
     root: tuple[str, ...] = (
-        'README.rst',
+        'README',
         'CHANGELOG.md',
         'pyproject.toml',
         'LICENSE.txt',
         'requirements.in',
     )
 
     source: tuple[str, ...] = ('__init__.py',)
```

### Comparing `OZI-1.6.5/ozi/spec/project.py` & `OZI-1.7.0/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/spec/python.py` & `OZI-1.7.0/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/spec/src.py` & `OZI-1.7.0/ozi/spec/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class SrcRequired(Default):
     """Required files for OZI to output with ``ozi-new``."""
 
     root: tuple[str, ...] = (
-        'README.rst',
+        'README',
         '.gitignore',
         'pyproject.toml',
         'meson.build',
         'meson.options',
         'LICENSE.txt',
         'requirements.in',
         'CHANGELOG.md',
@@ -73,15 +73,15 @@
     """
 
     root: tuple[str, ...] = (
         '.gitignore',
         'meson.build',
         'meson.options',
         'pyproject.toml',
-        'README.rst',
+        'README',
         'LICENSE.txt',
         'requirements.in',
         'CHANGELOG.md',
     )
     source: tuple[str, ...] = (
         'project.name/__init__.py',
         'project.name/meson.build',
```

### Comparing `OZI-1.6.5/ozi/tap.py` & `OZI-1.7.0/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/trove.py` & `OZI-1.7.0/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/email_validator/__init__.py` & `OZI-1.7.0/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/email_validator/__main__.py` & `OZI-1.7.0/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/email_validator/deliverability.py` & `OZI-1.7.0/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.7.0/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/email_validator/meson.build` & `OZI-1.7.0/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.7.0/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/email_validator/syntax.py` & `OZI-1.7.0/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/email_validator/validate_email.py` & `OZI-1.7.0/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/ozi/vendor/meson.build` & `OZI-1.7.0/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/pyproject.toml` & `OZI-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -316,14 +316,19 @@
 prerelease = false
 
 [tool.semantic_release.branches."release/1.6"]
 match = "release/1.6"
 prerelease_token = "alpha"
 prerelease = false
 
+[tool.semantic_release.branches."release/1.7"]
+match = "release/1.7"
+prerelease_token = "alpha"
+prerelease = false
+
 [tool.semantic_release.commit_parser_options]
 major_tags = [":boom:"]
 minor_tags = [
     ":sparkles:",
 ]
 patch_tags = [
     ":adhesive_bandage:",
```

### Comparing `OZI-1.6.5/templates/CHANGELOG.md.j2` & `OZI-1.7.0/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/tests/meson.build` & `OZI-1.7.0/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/tests/test_ozi_fix.py` & `OZI-1.7.0/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.6.5/tests/test_ozi_new.py` & `OZI-1.7.0/tests/test_ozi_new.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
             'license': st.one_of(
                 [
                     st.just(k)
                     for k in METADATA.spec.python.pkg.license.ambiguous.keys()
                     if k not in ['Private']
                 ],
             ),
+            'long_description_content_type': st.sampled_from(['rst', 'md', 'txt']),
         },
     ),
     license_expression=st.data(),
     license_id=st.data(),
 )
 def test_fuzz_new_project_good_namespace(  # noqa: DC102, RUF100
     tmp_path_factory: pytest.TempPathFactory,
@@ -215,14 +216,15 @@
         'topic': ['Utilities'],
         'audience': ['Developers'],
         'framework': ['Pytest'],
         'environment': ['No Input/Output (Daemon)'],
         'status': ['1 - Planning'],
         'dist_requires': [],
         'allow_file': [],
+        'long_description_content_type': 'rst',
     }
     project_dict.update(item)
     namespace = argparse.Namespace(**project_dict)
     with pytest.raises(RuntimeWarning):
         ozi.new.__main__.postprocess_arguments(
             ozi.new.__main__.preprocess_arguments(namespace),
         )
@@ -254,14 +256,15 @@
         'topic': ['Utilities'],
         'audience': ['Developers'],
         'framework': ['Pytest'],
         'environment': ['No Input/Output (Daemon)'],
         'status': ['1 - Planning'],
         'dist_requires': [],
         'allow_file': [],
+        'long_description_content_type': 'rst',
     }
     (project_dict['target'] / 'foobar').touch()  # type: ignore
     namespace = argparse.Namespace(**project_dict)
     with pytest.raises(RuntimeWarning):
         ozi.new.__main__.postprocess_arguments(
             ozi.new.__main__.preprocess_arguments(namespace),
         )
```

### Comparing `OZI-1.6.5/tests/test_tap.py` & `OZI-1.7.0/tests/test_tap.py`

 * *Files identical despite different names*

