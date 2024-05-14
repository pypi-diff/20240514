# Comparing `tmp/blueapi-0.4.2a2.tar.gz` & `tmp/blueapi-0.4.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueapi-0.4.2a2.tar", last modified: Wed May  1 16:27:35 2024, max compression
+gzip compressed data, was "blueapi-0.4.3a1.tar", last modified: Tue May 14 12:20:22 2024, max compression
```

## Comparing `blueapi-0.4.2a2.tar` & `blueapi-0.4.3a1.tar`

### file list

```diff
@@ -1,202 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.132484 blueapi-0.4.2a2/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.096484 blueapi-0.4.2a2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2722 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_container.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/asyncapi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/backstage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/helm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.104484 blueapi-0.4.2a2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-05-01 16:27:35.132484 blueapi-0.4.2a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/codecov.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/container-startup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.108484 blueapi-0.4.2a2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.108484 blueapi-0.4.2a2/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.108484 blueapi-0.4.2a2/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/0003-no-queues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/0004-api-case.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations/type_validators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/genindex.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.108484 blueapi-0.4.2a2/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/add-plans-and-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/configure-app.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/run-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to/write-plans.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.112484 blueapi-0.4.2a2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   236122 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/blueapi-architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/blueapi-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   386340 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/blueapi.png
--rw-r--r--   0 runner    (1001) docker     (127)   304331 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/bluesky-events.png
--rw-r--r--   0 runner    (1001) docker     (127)    16967 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/images/debug-vscode.png
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.112484 blueapi-0.4.2a2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/asyncapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/messaging-spec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference/rest-spec.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.112484 blueapi-0.4.2a2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/tutorials/dev-run.rst
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/tutorials/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/docs/tutorials.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.100484 blueapi-0.4.2a2/helm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.112484 blueapi-0.4.2a2/helm/blueapi/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/.helmignore
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.116484 blueapi-0.4.2a2/helm/blueapi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.116484 blueapi-0.4.2a2/helm/blueapi/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/templates/tests/test-ping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/helm/blueapi/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:27:35.132484 blueapi-0.4.2a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.100484 blueapi-0.4.2a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.116484 blueapi-0.4.2a2/src/blueapi/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.116484 blueapi-0.4.2a2/src/blueapi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/amq.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/cli/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.120484 blueapi-0.4.2a2/src/blueapi/core/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/bluesky_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/bluesky_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/device_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/core/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.120484 blueapi-0.4.2a2/src/blueapi/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/messaging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.120484 blueapi-0.4.2a2/src/blueapi/service/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/handler_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/service/subprocess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.120484 blueapi-0.4.2a2/src/blueapi/startup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/startup/example_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/startup/example_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/startup/simmotor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/src/blueapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/invalid_config_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/ophyd_async_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/utils/thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/src/blueapi/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/reworker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/src/blueapi/worker/worker_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/src/blueapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 16:27:35.000000 blueapi-0.4.2a2/src/blueapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/fake_device_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/fake_plan_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/core/test_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.124484 blueapi-0.4.2a2/tests/example_yaml/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/override_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/rest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/valid_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/example_yaml/valid_stomp_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/tests/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/messaging/test_stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/messaging/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/tests/service/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/service/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/service/test_openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/service/test_rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/service/test_subprocess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/hasall.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/lacksall.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/test_ophyd_async_connect.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/utils/test_thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:27:35.128484 blueapi-0.4.2a2/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/worker/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-01 16:27:31.000000 blueapi-0.4.2a2/tests/worker/test_reworker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.770188 blueapi-0.4.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.742189 blueapi-0.4.3a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.742189 blueapi-0.4.3a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.738189 blueapi-0.4.3a1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.742189 blueapi-0.4.3a1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.742189 blueapi-0.4.3a1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2722 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.746189 blueapi-0.4.3a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/_container.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/asyncapi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/backstage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/helm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.746189 blueapi-0.4.3a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-14 12:20:22.770188 blueapi-0.4.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/codecov.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/container-startup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.746189 blueapi-0.4.3a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.746189 blueapi-0.4.3a1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.750189 blueapi-0.4.3a1/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/decisions/0003-no-queues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/decisions/0004-api-case.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations/type_validators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.750189 blueapi-0.4.3a1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/how-to/add-plans-and-devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/how-to/configure-app.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/how-to/run-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/how-to/write-plans.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.750189 blueapi-0.4.3a1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   236122 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/images/blueapi-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/images/blueapi-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   386340 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/images/blueapi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   304331 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/images/bluesky-events.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16967 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/images/debug-vscode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.754189 blueapi-0.4.3a1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/reference/asyncapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/reference/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/reference/messaging-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/reference/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/reference/rest-spec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.754189 blueapi-0.4.3a1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/tutorials/dev-run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/tutorials/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/docs/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.738189 blueapi-0.4.3a1/helm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.754189 blueapi-0.4.3a1/helm/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.754189 blueapi-0.4.3a1/helm/blueapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/templates/configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/templates/ingress.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.754189 blueapi-0.4.3a1/helm/blueapi/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/templates/tests/test-ping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/helm/blueapi/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 12:20:22.770188 blueapi-0.4.3a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.738189 blueapi-0.4.3a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.754189 blueapi-0.4.3a1/src/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-14 12:20:22.000000 blueapi-0.4.3a1/src/blueapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.758189 blueapi-0.4.3a1/src/blueapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/cli/event_bus_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/cli/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/cli/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.758189 blueapi-0.4.3a1/src/blueapi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/core/bluesky_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/core/bluesky_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/core/device_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/core/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.758189 blueapi-0.4.3a1/src/blueapi/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/messaging/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/messaging/stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/messaging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.762189 blueapi-0.4.3a1/src/blueapi/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/service/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/service/handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/service/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/service/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/service/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/service/subprocess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.762189 blueapi-0.4.3a1/src/blueapi/startup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/startup/example_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/startup/example_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/startup/simmotor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.762189 blueapi-0.4.3a1/src/blueapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/utils/invalid_config_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/utils/thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.762189 blueapi-0.4.3a1/src/blueapi/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/worker/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/worker/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/worker/reworker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/src/blueapi/worker/worker_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.770188 blueapi-0.4.3a1/src/blueapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-14 12:20:22.000000 blueapi-0.4.3a1/src/blueapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-14 12:20:22.000000 blueapi-0.4.3a1/src/blueapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 12:20:22.000000 blueapi-0.4.3a1/src/blueapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 12:20:22.000000 blueapi-0.4.3a1/src/blueapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-14 12:20:22.000000 blueapi-0.4.3a1/src/blueapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 12:20:22.000000 blueapi-0.4.3a1/src/blueapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.766188 blueapi-0.4.3a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.766188 blueapi-0.4.3a1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/core/fake_device_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/core/fake_plan_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/core/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/core/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.766188 blueapi-0.4.3a1/tests/example_yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/example_yaml/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/example_yaml/nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/example_yaml/override_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/example_yaml/rest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/example_yaml/valid_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/example_yaml/valid_stomp_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.766188 blueapi-0.4.3a1/tests/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/messaging/test_stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/messaging/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.766188 blueapi-0.4.3a1/tests/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/service/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/service/test_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/service/test_rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/service/test_subprocess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.766188 blueapi-0.4.3a1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/utils/hasall.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/utils/lacksall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/utils/test_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/utils/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/utils/test_thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 12:20:22.770188 blueapi-0.4.3a1/tests/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/worker/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-14 12:20:16.000000 blueapi-0.4.3a1/tests/worker/test_reworker.py
```

### Comparing `blueapi-0.4.2a2/.devcontainer/devcontainer.json` & `blueapi-0.4.3a1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/CONTRIBUTING.md` & `blueapi-0.4.3a1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/actions/install_requirements/action.yml` & `blueapi-0.4.3a1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/dependabot.yml` & `blueapi-0.4.3a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/pages/make_switcher.py` & `blueapi-0.4.3a1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/workflows/_check.yml` & `blueapi-0.4.3a1/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/workflows/_container.yml` & `blueapi-0.4.3a1/.github/workflows/_container.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/workflows/_dist.yml` & `blueapi-0.4.3a1/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/workflows/_docs.yml` & `blueapi-0.4.3a1/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/workflows/_release.yml` & `blueapi-0.4.3a1/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/workflows/_test.yml` & `blueapi-0.4.3a1/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/workflows/ci.yml` & `blueapi-0.4.3a1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.github/workflows/helm.yml` & `blueapi-0.4.3a1/.github/workflows/helm.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.gitignore` & `blueapi-0.4.3a1/.gitignore`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.pre-commit-config.yaml` & `blueapi-0.4.3a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/.vscode/launch.json` & `blueapi-0.4.3a1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/Dockerfile` & `blueapi-0.4.3a1/Dockerfile`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/LICENSE` & `blueapi-0.4.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/PKG-INFO` & `blueapi-0.4.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.4.2a2
+Version: 0.4.3a1
 Summary: Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -234,15 +234,15 @@
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
-Requires-Dist: sphinx-autobuild; extra == "dev"
+Requires-Dist: sphinx-autobuild==2024.2.4; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-click; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: sphinxcontrib-openapi; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
```

### Comparing `blueapi-0.4.2a2/README.md` & `blueapi-0.4.3a1/README.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/catalog-info.yaml` & `blueapi-0.4.3a1/catalog-info.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/conf.py` & `blueapi-0.4.3a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/explanations/architecture.rst` & `blueapi-0.4.3a1/docs/explanations/architecture.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `blueapi-0.4.3a1/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/explanations/decisions/0003-no-queues.rst` & `blueapi-0.4.3a1/docs/explanations/decisions/0003-no-queues.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/explanations/decisions/0004-api-case.rst` & `blueapi-0.4.3a1/docs/explanations/decisions/0004-api-case.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/explanations/events.rst` & `blueapi-0.4.3a1/docs/explanations/events.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/explanations/lifecycle.rst` & `blueapi-0.4.3a1/docs/explanations/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/explanations/type_validators.rst` & `blueapi-0.4.3a1/docs/explanations/type_validators.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/how-to/add-plans-and-devices.rst` & `blueapi-0.4.3a1/docs/how-to/add-plans-and-devices.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/how-to/configure-app.rst` & `blueapi-0.4.3a1/docs/how-to/configure-app.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/how-to/run-cli.rst` & `blueapi-0.4.3a1/docs/how-to/run-cli.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/how-to/run-container.rst` & `blueapi-0.4.3a1/docs/how-to/run-container.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/how-to/write-plans.rst` & `blueapi-0.4.3a1/docs/how-to/write-plans.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/images/blueapi-architecture.png` & `blueapi-0.4.3a1/docs/images/blueapi-architecture.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/images/blueapi-logo.svg` & `blueapi-0.4.3a1/docs/images/blueapi-logo.svg`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/images/blueapi.png` & `blueapi-0.4.3a1/docs/images/blueapi.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/images/bluesky-events.png` & `blueapi-0.4.3a1/docs/images/bluesky-events.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/images/debug-vscode.png` & `blueapi-0.4.3a1/docs/images/debug-vscode.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/index.md` & `blueapi-0.4.3a1/docs/index.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/reference/asyncapi.yaml` & `blueapi-0.4.3a1/docs/reference/asyncapi.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/reference/openapi.yaml` & `blueapi-0.4.3a1/docs/reference/openapi.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/tutorials/dev-run.rst` & `blueapi-0.4.3a1/docs/tutorials/dev-run.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/tutorials/installation.md` & `blueapi-0.4.3a1/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/docs/tutorials/quickstart.rst` & `blueapi-0.4.3a1/docs/tutorials/quickstart.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/helm/blueapi/Chart.yaml` & `blueapi-0.4.3a1/helm/blueapi/Chart.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/helm/blueapi/templates/_helpers.tpl` & `blueapi-0.4.3a1/helm/blueapi/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/helm/blueapi/templates/deployment.yaml` & `blueapi-0.4.3a1/helm/blueapi/templates/deployment.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 spec:
   replicas: {{ .Values.replicaCount }}
   selector:
     matchLabels:
       {{- include "blueapi.selectorLabels" . | nindent 6 }}
   template:
     metadata:
-      {{- with .Values.podAnnotations }}
       annotations:
+      {{- if .Values.restartOnConfigChange }}
+        checksum/config: {{ include (print $.Template.BasePath "/configmap.yaml") . | sha256sum }}
+      {{- end }}
+      {{- with .Values.podAnnotations }}
         {{- toYaml . | nindent 8 }}
       {{- end }}
       labels:
         {{- include "blueapi.selectorLabels" . | nindent 8 }}
     spec:
       hostNetwork: {{ .Values.hostNetwork }}
       {{- with .Values.imagePullSecrets }}
```

### Comparing `blueapi-0.4.2a2/helm/blueapi/templates/ingress.yaml` & `blueapi-0.4.3a1/helm/blueapi/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/helm/blueapi/templates/tests/test-ping.yaml` & `blueapi-0.4.3a1/helm/blueapi/templates/tests/test-ping.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/helm/blueapi/values.yaml` & `blueapi-0.4.3a1/helm/blueapi/values.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 
 tolerations: []
 
 affinity: {}
 
 hostNetwork: false # May be needed for talking to arcane protocols such as EPICS
 
+restartOnConfigChange: true
+
 listener:
   enabled: true
   resources: {}
 
 scratch:
   hostPath: "" # example: /usr/local/blueapi-software-scratch
   containerPath: /blueapi-plugins/scratch
```

### Comparing `blueapi-0.4.2a2/pyproject.toml` & `blueapi-0.4.3a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "pyepics",
     "aioca",
     "pydantic<2.0",
     "stomp-py",
     "aiohttp",
     "PyYAML",
     "click<8.1.4",
-    "fastapi[all]<0.99",
+    "fastapi[all]<0.99", # Later versions use a newer openapi schema, which is incompatible with swagger see https://github.com/swagger-api/swagger-codegen/issues/10446
     "uvicorn",
     "requests",
     "dls-bluesky-core",  #requires ophyd-async
     "dls-dodal",
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
@@ -40,15 +40,15 @@
     "pipdeptree",
     "pre-commit",
     "pydata-sphinx-theme>=0.12",
     "mypy",
     "pytest-cov",
     "pytest-asyncio",
     "ruff",
-    "sphinx-autobuild",
+    "sphinx-autobuild==2024.2.4", # Later versions have a clash with fastapi<0.99, remove pin when fastapi is a higher version
     "sphinx-copybutton",
     "sphinx-click",
     "sphinx-design",
     "sphinxcontrib-openapi",
     "tox-direct",
     "types-mock",
     "types-PyYAML",
```

### Comparing `blueapi-0.4.2a2/src/blueapi/cli/amq.py` & `blueapi-0.4.3a1/src/blueapi/cli/event_bus_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self, message: str) -> None:
         super().__init__(message)
 
 
 _Event = WorkerEvent | ProgressEvent | DataEvent
 
 
-class AmqClient:
+class EventBusClient:
     app: MessagingTemplate
     complete: threading.Event
     timed_out: bool | None
 
     def __init__(self, app: MessagingTemplate) -> None:
         self.app = app
         self.complete = threading.Event()
```

### Comparing `blueapi-0.4.2a2/src/blueapi/cli/cli.py` & `blueapi-0.4.3a1/src/blueapi/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from pprint import pprint
 
 import click
 from requests.exceptions import ConnectionError
 
 from blueapi import __version__
-from blueapi.cli.amq import AmqClient
+from blueapi.cli.event_bus_client import EventBusClient
 from blueapi.config import ApplicationConfig, ConfigLoader
 from blueapi.core import DataEvent
 from blueapi.messaging import MessageContext
 from blueapi.messaging.stomptemplate import StompMessagingTemplate
 from blueapi.service.main import start
 from blueapi.service.model import WorkerTask
 from blueapi.service.openapi import (
@@ -131,31 +131,33 @@
 @controller.command(name="listen")
 @check_connection
 @click.pass_obj
 def listen_to_events(obj: dict) -> None:
     """Listen to events output by blueapi"""
     config: ApplicationConfig = obj["config"]
     if config.stomp is not None:
-        amq_client = AmqClient(StompMessagingTemplate.autoconfigured(config.stomp))
+        event_bus_client = EventBusClient(
+            StompMessagingTemplate.autoconfigured(config.stomp)
+        )
     else:
         raise RuntimeError("Message bus needs to be configured")
 
     def on_event(
         context: MessageContext,
         event: WorkerEvent | ProgressEvent | DataEvent,
     ) -> None:
         converted = json.dumps(event.dict(), indent=2)
         print(converted)
 
     print(
         "Subscribing to all bluesky events from "
         f"{config.stomp.host}:{config.stomp.port}"
     )
-    with amq_client:
-        amq_client.subscribe_to_all_events(on_event)
+    with event_bus_client:
+        event_bus_client.subscribe_to_all_events(on_event)
         input("Press enter to exit")
 
 
 @controller.command(name="run")
 @click.argument("name", type=str)
 @click.argument("parameters", type=str, required=False)
 @click.option(
@@ -177,34 +179,34 @@
     logger = logging.getLogger(__name__)
     if config.stomp is not None:
         _message_template = StompMessagingTemplate.autoconfigured(config.stomp)
     else:
         raise RuntimeError(
             "Cannot run plans without Stomp configuration to track progress"
         )
-    amq_client = AmqClient(_message_template)
+    event_bus_client = EventBusClient(_message_template)
     finished_event: deque[WorkerEvent] = deque()
 
     def store_finished_event(event: WorkerEvent) -> None:
         if event.is_complete():
             finished_event.append(event)
 
     parameters = parameters or "{}"
     task = Task(name=name, params=json.loads(parameters))
 
     resp = client.create_task(task)
     task_id = resp.task_id
 
-    with amq_client:
-        amq_client.subscribe_to_topics(task_id, on_event=store_finished_event)
+    with event_bus_client:
+        event_bus_client.subscribe_to_topics(task_id, on_event=store_finished_event)
         updated = client.update_worker_task(WorkerTask(task_id=task_id))
 
-        amq_client.wait_for_complete(timeout=timeout)
+        event_bus_client.wait_for_complete(timeout=timeout)
 
-        if amq_client.timed_out:
+        if event_bus_client.timed_out:
             logger.error(f"Plan did not complete within {timeout} seconds")
             return
 
     process_event_after_finished(finished_event.pop(), logger)
     pprint(updated.dict())
```

### Comparing `blueapi-0.4.2a2/src/blueapi/cli/rest.py` & `blueapi-0.4.3a1/src/blueapi/cli/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     PlanModel,
     PlanResponse,
     TaskResponse,
     WorkerTask,
 )
 from blueapi.worker import Task, TrackableTask, WorkerState
 
-from .amq import BlueskyRemoteError
+from .event_bus_client import BlueskyRemoteError
 
 T = TypeVar("T")
 
 
 def _is_exception(response: requests.Response) -> bool:
     return response.status_code >= 400
```

### Comparing `blueapi-0.4.2a2/src/blueapi/cli/updates.py` & `blueapi-0.4.3a1/src/blueapi/cli/updates.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/config.py` & `blueapi-0.4.3a1/src/blueapi/config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/core/__init__.py` & `blueapi-0.4.3a1/src/blueapi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/core/bluesky_types.py` & `blueapi-0.4.3a1/src/blueapi/core/bluesky_types.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/core/context.py` & `blueapi-0.4.3a1/src/blueapi/core/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 from collections.abc import Callable
 from dataclasses import dataclass, field
 from importlib import import_module
 from inspect import Parameter, signature
 from types import ModuleType, UnionType
 from typing import Any, Generic, TypeVar, Union, get_args, get_origin, get_type_hints
 
-from bluesky.run_engine import RunEngine, call_in_bluesky_event_loop
+from bluesky.run_engine import RunEngine
 from pydantic import create_model
 from pydantic.fields import FieldInfo, ModelField
 
 from blueapi.config import EnvironmentConfig, SourceKind
 from blueapi.utils import (
     BlueapiPlanModelConfig,
-    connect_ophyd_async_devices,
     load_module_all,
 )
 
 from .bluesky_types import (
     BLUESKY_PROTOCOLS,
     Device,
     HasName,
@@ -41,15 +40,14 @@
 
     run_engine: RunEngine = field(
         default_factory=lambda: RunEngine(context_managers=[])
     )
     plans: dict[str, Plan] = field(default_factory=dict)
     devices: dict[str, Device] = field(default_factory=dict)
     plan_functions: dict[str, PlanGenerator] = field(default_factory=dict)
-    sim: bool = field(default=False)
 
     _reference_cache: dict[type, type] = field(default_factory=dict)
 
     def find_device(self, addr: str | list[str]) -> Device | None:
         """
         Find a device in this context, allows for recursive search.
 
@@ -74,21 +72,14 @@
             if source.kind is SourceKind.PLAN_FUNCTIONS:
                 self.with_plan_module(mod)
             elif source.kind is SourceKind.DEVICE_FUNCTIONS:
                 self.with_device_module(mod)
             elif source.kind is SourceKind.DODAL:
                 self.with_dodal_module(mod)
 
-        call_in_bluesky_event_loop(
-            connect_ophyd_async_devices(
-                self.devices.values(),
-                self.sim,
-            )
-        )
-
     def with_plan_module(self, module: ModuleType) -> None:
         """
         Register all functions in the module supplied as plans.
         Module should take the form:
 
         def plan_1(...) -> MsgGenerator:
             ...
```

### Comparing `blueapi-0.4.2a2/src/blueapi/core/device_lookup.py` & `blueapi-0.4.3a1/src/blueapi/core/device_lookup.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/core/event.py` & `blueapi-0.4.3a1/src/blueapi/core/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/messaging/base.py` & `blueapi-0.4.3a1/src/blueapi/messaging/base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/messaging/stomptemplate.py` & `blueapi-0.4.3a1/src/blueapi/messaging/stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/messaging/utils.py` & `blueapi-0.4.3a1/src/blueapi/messaging/utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/service/handler.py` & `blueapi-0.4.3a1/src/blueapi/service/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,17 +150,15 @@
 def setup_handler(
     config: ApplicationConfig | None = None,
 ) -> None:
     global HANDLER
 
     handler = Handler(
         config,
-        context=BlueskyContext(
-            sim=False,
-        ),
+        context=BlueskyContext(),
     )
     handler.start()
 
     HANDLER = handler
 
 
 def get_handler() -> Handler:
```

### Comparing `blueapi-0.4.2a2/src/blueapi/service/handler_base.py` & `blueapi-0.4.3a1/src/blueapi/service/handler_base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/service/main.py` & `blueapi-0.4.3a1/src/blueapi/service/main.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/service/model.py` & `blueapi-0.4.3a1/src/blueapi/service/model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/service/openapi.py` & `blueapi-0.4.3a1/src/blueapi/service/openapi.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/service/subprocess_handler.py` & `blueapi-0.4.3a1/src/blueapi/service/subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/startup/example_devices.py` & `blueapi-0.4.3a1/src/blueapi/startup/example_devices.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/startup/example_plans.py` & `blueapi-0.4.3a1/src/blueapi/startup/example_plans.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/startup/simmotor.py` & `blueapi-0.4.3a1/src/blueapi/startup/simmotor.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/utils/base_model.py` & `blueapi-0.4.3a1/src/blueapi/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/utils/modules.py` & `blueapi-0.4.3a1/src/blueapi/utils/modules.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/utils/serialization.py` & `blueapi-0.4.3a1/src/blueapi/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/utils/thread_exception.py` & `blueapi-0.4.3a1/src/blueapi/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/worker/__init__.py` & `blueapi-0.4.3a1/src/blueapi/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/worker/event.py` & `blueapi-0.4.3a1/src/blueapi/worker/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/worker/multithread.py` & `blueapi-0.4.3a1/src/blueapi/worker/multithread.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/worker/reworker.py` & `blueapi-0.4.3a1/src/blueapi/worker/reworker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/worker/task.py` & `blueapi-0.4.3a1/src/blueapi/worker/task.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi/worker/worker.py` & `blueapi-0.4.3a1/src/blueapi/worker/worker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/src/blueapi.egg-info/PKG-INFO` & `blueapi-0.4.3a1/src/blueapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.4.2a2
+Version: 0.4.3a1
 Summary: Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -234,15 +234,15 @@
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
-Requires-Dist: sphinx-autobuild; extra == "dev"
+Requires-Dist: sphinx-autobuild==2024.2.4; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-click; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: sphinxcontrib-openapi; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
```

### Comparing `blueapi-0.4.2a2/src/blueapi.egg-info/SOURCES.txt` & `blueapi-0.4.3a1/src/blueapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 src/blueapi.egg-info/SOURCES.txt
 src/blueapi.egg-info/dependency_links.txt
 src/blueapi.egg-info/entry_points.txt
 src/blueapi.egg-info/requires.txt
 src/blueapi.egg-info/top_level.txt
 src/blueapi/cli/__init__.py
 src/blueapi/cli/__main__.py
-src/blueapi/cli/amq.py
 src/blueapi/cli/cli.py
+src/blueapi/cli/event_bus_client.py
 src/blueapi/cli/rest.py
 src/blueapi/cli/updates.py
 src/blueapi/core/__init__.py
 src/blueapi/core/bluesky_event_loop.py
 src/blueapi/core/bluesky_types.py
 src/blueapi/core/context.py
 src/blueapi/core/device_lookup.py
@@ -117,15 +117,14 @@
 src/blueapi/startup/example_devices.py
 src/blueapi/startup/example_plans.py
 src/blueapi/startup/simmotor.py
 src/blueapi/utils/__init__.py
 src/blueapi/utils/base_model.py
 src/blueapi/utils/invalid_config_error.py
 src/blueapi/utils/modules.py
-src/blueapi/utils/ophyd_async_connect.py
 src/blueapi/utils/serialization.py
 src/blueapi/utils/thread_exception.py
 src/blueapi/worker/__init__.py
 src/blueapi/worker/event.py
 src/blueapi/worker/multithread.py
 src/blueapi/worker/reworker.py
 src/blueapi/worker/task.py
@@ -154,11 +153,10 @@
 tests/service/test_rest_api.py
 tests/service/test_subprocess_handler.py
 tests/utils/__init__.py
 tests/utils/hasall.py
 tests/utils/lacksall.py
 tests/utils/test_base_model.py
 tests/utils/test_modules.py
-tests/utils/test_ophyd_async_connect.py
 tests/utils/test_thread_exception.py
 tests/worker/devices.py
 tests/worker/test_reworker.py
```

### Comparing `blueapi-0.4.2a2/tests/conftest.py` & `blueapi-0.4.3a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/core/fake_device_module.py` & `blueapi-0.4.3a1/tests/core/fake_device_module.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/core/test_context.py` & `blueapi-0.4.3a1/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/core/test_event.py` & `blueapi-0.4.3a1/tests/core/test_event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/messaging/test_stomptemplate.py` & `blueapi-0.4.3a1/tests/messaging/test_stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/messaging/test_utils.py` & `blueapi-0.4.3a1/tests/messaging/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/service/test_handler.py` & `blueapi-0.4.3a1/tests/service/test_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/service/test_openapi.py` & `blueapi-0.4.3a1/tests/service/test_openapi.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/service/test_rest_api.py` & `blueapi-0.4.3a1/tests/service/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/service/test_subprocess_handler.py` & `blueapi-0.4.3a1/tests/service/test_subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/test_cli.py` & `blueapi-0.4.3a1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/test_config.py` & `blueapi-0.4.3a1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/utils/test_thread_exception.py` & `blueapi-0.4.3a1/tests/utils/test_thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/worker/devices.py` & `blueapi-0.4.3a1/tests/worker/devices.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.2a2/tests/worker/test_reworker.py` & `blueapi-0.4.3a1/tests/worker/test_reworker.py`

 * *Files identical despite different names*

