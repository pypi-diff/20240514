# Comparing `tmp/girder-slicer-cli-web-1.5.4.dev2.tar.gz` & `tmp/girder_slicer_cli_web-1.5.5.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-slicer-cli-web-1.5.4.dev2.tar", last modified: Fri Mar 22 19:53:51 2024, max compression
+gzip compressed data, was "girder_slicer_cli_web-1.5.5.dev2.tar", last modified: Tue May 14 19:17:16 2024, max compression
```

## Comparing `girder-slicer-cli-web-1.5.4.dev2.tar` & `girder_slicer_cli_web-1.5.5.dev2.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.665892 girder-slicer-cli-web-1.5.4.dev2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.637892 girder-slicer-cli-web-1.5.4.dev2/.circleci/
--rw-r--r--   0 root         (0) root         (0)     7477 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)     4000 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      406 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/.editorconfig
--rw-r--r--   0 root         (0) root         (0)     1734 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1645 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17374 2024-03-22 19:53:51.665892 girder-slicer-cli-web-1.5.4.dev2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15959 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/README.rst
--rw-r--r--   0 root         (0) root         (0)      460 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/codecov.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.637892 girder-slicer-cli-web-1.5.4.dev2/docs/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/docs/worker_management.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.641892 girder-slicer-cli-web-1.5.4.dev2/example-average-color/
--rw-r--r--   0 root         (0) root         (0)     4000 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-average-color/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      260 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-average-color/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      877 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-average-color/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.641892 girder-slicer-cli-web-1.5.4.dev2/example-average-color/average_color/
--rw-r--r--   0 root         (0) root         (0)     1515 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-average-color/average_color/average_color.py
--rw-r--r--   0 root         (0) root         (0)     1494 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-average-color/average_color/average_color.xml
--rw-r--r--   0 root         (0) root         (0)       50 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-average-color/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-average-color/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.641892 girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/
--rw-r--r--   0 root         (0) root         (0)      290 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      507 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/README.rst
--rw-r--r--   0 root         (0) root         (0)       52 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.641892 girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/girder_requests/
--rw-r--r--   0 root         (0) root         (0)      503 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/girder_requests/girder_requests.py
--rw-r--r--   0 root         (0) root         (0)     1223 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/girder_requests/girder_requests.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.665892 girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17374 2024-03-22 19:53:51.000000 girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6054 2024-03-22 19:53:51.000000 girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 19:53:51.000000 girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      184 2024-03-22 19:53:51.000000 girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 19:53:14.000000 girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-22 19:53:51.000000 girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-22 19:53:51.000000 girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-03-22 19:53:51.665892 girder-slicer-cli-web-1.5.4.dev2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2714 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.645892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/
--rw-r--r--   0 root         (0) root         (0)     1191 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3558 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/cli_list_entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2501 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)     3109 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/config.py
--rw-r--r--   0 root         (0) root         (0)     6649 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/ctk_cli_adjustment.py
--rw-r--r--   0 root         (0) root         (0)    15908 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/docker_resource.py
--rw-r--r--   0 root         (0) root         (0)     3055 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.645892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_worker_plugin/
--rw-r--r--   0 root         (0) root         (0)     1018 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_worker_plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2553 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_worker_plugin/cli_progress.py
--rw-r--r--   0 root         (0) root         (0)     3834 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_worker_plugin/direct_docker_run.py
--rw-r--r--   0 root         (0) root         (0)    12084 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/image_job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.645892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/
--rw-r--r--   0 root         (0) root         (0)      208 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10406 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/docker_image.py
--rw-r--r--   0 root         (0) root         (0)      810 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3045 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/json_to_xml.py
--rw-r--r--   0 root         (0) root         (0)     2340 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/parser.py
--rw-r--r--   0 root         (0) root         (0)    31703 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/schema.json
--rw-r--r--   0 root         (0) root         (0)    14268 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/prepare_task.py
--rw-r--r--   0 root         (0) root         (0)    25905 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/rest_slicer_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.649892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/
--rw-r--r--   0 root         (0) root         (0)      404 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/JobStatus.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.649892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/collections/
--rw-r--r--   0 root         (0) root         (0)     1537 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/collections/WidgetCollection.js
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/collections/index.js
--rw-r--r--   0 root         (0) root         (0)       78 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/events.js
--rw-r--r--   0 root         (0) root         (0)      299 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/index.js
--rw-r--r--   0 root         (0) root         (0)      343 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/main.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.649892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/models/
--rw-r--r--   0 root         (0) root         (0)     9697 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/models/WidgetModel.js
--rw-r--r--   0 root         (0) root         (0)       56 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/models/index.js
--rw-r--r--   0 root         (0) root         (0)     3996 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.649892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/
--rw-r--r--   0 root         (0) root         (0)      540 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/constraints.js
--rw-r--r--   0 root         (0) root         (0)      610 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/convert.js
--rw-r--r--   0 root         (0) root         (0)      671 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/defaultValue.js
--rw-r--r--   0 root         (0) root         (0)      894 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/group.js
--rw-r--r--   0 root         (0) root         (0)      384 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/index.js
--rw-r--r--   0 root         (0) root         (0)      506 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/panel.js
--rw-r--r--   0 root         (0) root         (0)     2543 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/param.js
--rw-r--r--   0 root         (0) root         (0)     1595 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/parse.js
--rw-r--r--   0 root         (0) root         (0)      921 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/widget.js
--rw-r--r--   0 root         (0) root         (0)      404 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/routes.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.649892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/
--rw-r--r--   0 root         (0) root         (0)       93 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/configView.styl
--rw-r--r--   0 root         (0) root         (0)      964 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/controlWidget.styl
--rw-r--r--   0 root         (0) root         (0)      112 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/controlsPanel.styl
--rw-r--r--   0 root         (0) root         (0)       85 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/outputParameterDialog.styl
--rw-r--r--   0 root         (0) root         (0)      662 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/panel.styl
--rw-r--r--   0 root         (0) root         (0)      197 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/panelGroup.styl
--rw-r--r--   0 root         (0) root         (0)      370 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/slicerUI.styl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.653892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/
--rw-r--r--   0 root         (0) root         (0)      256 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/booleanWidget.pug
--rw-r--r--   0 root         (0) root         (0)      115 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/colorWidget.pug
--rw-r--r--   0 root         (0) root         (0)     2165 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/configView.pug
--rw-r--r--   0 root         (0) root         (0)       42 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/controlsPanel.pug
--rw-r--r--   0 root         (0) root         (0)      136 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/enumerationWidget.pug
--rw-r--r--   0 root         (0) root         (0)     1305 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/fileWidget.pug
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/jobsListWidget.pug
--rw-r--r--   0 root         (0) root         (0)      336 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/outputParameterDialog.pug
--rw-r--r--   0 root         (0) root         (0)      408 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/panel.pug
--rw-r--r--   0 root         (0) root         (0)      529 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/panelGroup.pug
--rw-r--r--   0 root         (0) root         (0)      184 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/rangeWidget.pug
--rw-r--r--   0 root         (0) root         (0)     3623 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/regionWidget.pug
--rw-r--r--   0 root         (0) root         (0)      308 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/slicerUI.pug
--rw-r--r--   0 root         (0) root         (0)      735 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/uploadImageDialog.pug
--rw-r--r--   0 root         (0) root         (0)      569 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/widget.pug
--rw-r--r--   0 root         (0) root         (0)     1642 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/utils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.657892 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/
--rw-r--r--   0 root         (0) root         (0)     4761 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/CollectionView.js
--rw-r--r--   0 root         (0) root         (0)     7145 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ConfigView.js
--rw-r--r--   0 root         (0) root         (0)    17917 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ControlWidget.js
--rw-r--r--   0 root         (0) root         (0)     1542 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ControlsPanel.js
--rw-r--r--   0 root         (0) root         (0)    11455 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ItemSelectorWidget.js
--rw-r--r--   0 root         (0) root         (0)     4584 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ItemView.js
--rw-r--r--   0 root         (0) root         (0)     3798 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/JobsListWidget.js
--rw-r--r--   0 root         (0) root         (0)      799 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/JobsPanel.js
--rw-r--r--   0 root         (0) root         (0)      532 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/OutputParameterDialog.js
--rw-r--r--   0 root         (0) root         (0)     1150 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/Panel.js
--rw-r--r--   0 root         (0) root         (0)     8424 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/PanelGroup.js
--rw-r--r--   0 root         (0) root         (0)      394 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/index.js
--rw-r--r--   0 root         (0) root         (0)      872 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/utils.js
--rw-r--r--   0 root         (0) root         (0)     7792 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/worker_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.657892 girder-slicer-cli-web-1.5.4.dev2/small-docker/
--rw-r--r--   0 root         (0) root         (0)     4000 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/.dockerignore
--rw-r--r--   0 root         (0) root         (0)      720 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.657892 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/
--rw-r--r--   0 root         (0) root         (0)    11001 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/Example1.json
--rw-r--r--   0 root         (0) root         (0)      681 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/Example1.py
--rw-r--r--   0 root         (0) root         (0)    10702 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/Example1.xml
--rw-r--r--   0 root         (0) root         (0)     7535 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/Example1.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.657892 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/
--rw-r--r--   0 root         (0) root         (0)     1042 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/Example2.json
--rw-r--r--   0 root         (0) root         (0)      678 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/Example2.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/Example2.xml
--rw-r--r--   0 root         (0) root         (0)      639 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/Example2.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.657892 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/
--rw-r--r--   0 root         (0) root         (0)     1035 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/Example3.json
--rw-r--r--   0 root         (0) root         (0)      621 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/Example3.py
--rw-r--r--   0 root         (0) root         (0)     1001 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/Example3.xml
--rw-r--r--   0 root         (0) root         (0)      626 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/Example3.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.657892 girder-slicer-cli-web-1.5.4.dev2/small-docker/ExampleProgress/
--rw-r--r--   0 root         (0) root         (0)      855 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/ExampleProgress/ExampleProgress.json
--rw-r--r--   0 root         (0) root         (0)      884 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/ExampleProgress/ExampleProgress.py
--rw-r--r--   0 root         (0) root         (0)     1269 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/ExampleProgress/progress_helper.py
--rw-r--r--   0 root         (0) root         (0)      523 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/cli_list.json
--rw-r--r--   0 root         (0) root         (0)     1397 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/small-docker/cli_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.661892 girder-slicer-cli-web-1.5.4.dev2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10313 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.661892 girder-slicer-cli-web-1.5.4.dev2/tests/data/
--rw-r--r--   0 root         (0) root         (0)     3850 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/ExampleSpec.xml
--rw-r--r--   0 root         (0) root         (0)      301 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/girder_worker.cfg
--rw-r--r--   0 root         (0) root         (0)     1235 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_advanced.json
--rw-r--r--   0 root         (0) root         (0)     1183 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_advanced.xml
--rw-r--r--   0 root         (0) root         (0)      681 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_advanced.yaml
--rw-r--r--   0 root         (0) root         (0)      232 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_simple.json
--rw-r--r--   0 root         (0) root         (0)      218 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_simple.xml
--rw-r--r--   0 root         (0) root         (0)      109 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_simple.yaml
--rw-r--r--   0 root         (0) root         (0)      272 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_simple.json
--rw-r--r--   0 root         (0) root         (0)      319 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_simple.xml
--rw-r--r--   0 root         (0) root         (0)      152 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_simple.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.661892 girder-slicer-cli-web-1.5.4.dev2/tests/girder_worker_plugin/
--rw-r--r--   0 root         (0) root         (0)     2769 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/girder_worker_plugin/test_cli_progress.py
--rw-r--r--   0 root         (0) root         (0)     1799 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/girder_worker_plugin/test_direct_docker_run.py
--rw-r--r--   0 root         (0) root         (0)     4961 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/test_batch.py
--rw-r--r--   0 root         (0) root         (0)      762 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     6041 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/test_docker.py
--rwxr-xr-x   0 root         (0) root         (0)      931 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/test_load.py
--rw-r--r--   0 root         (0) root         (0)     5923 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/test_parser.py
--rw-r--r--   0 root         (0) root         (0)    10568 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/test_rest_slicer_cli.py
--rw-r--r--   0 root         (0) root         (0)      867 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/test_web_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.665892 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/
--rw-r--r--   0 root         (0) root         (0)      237 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/.eslintrc
--rw-r--r--   0 root         (0) root         (0)     2410 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/configViewSpec.js
--rw-r--r--   0 root         (0) root         (0)     4543 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/containerViewSpec.js
--rw-r--r--   0 root         (0) root         (0)     6091 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/dockerTaskSpec.js
--rw-r--r--   0 root         (0) root         (0)     9891 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/itemSelectorWidgetSpec.js
--rw-r--r--   0 root         (0) root         (0)     2503 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/panelGroupSpec.js
--rw-r--r--   0 root         (0) root         (0)    27360 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/parseSpec.js
--rw-r--r--   0 root         (0) root         (0)    43069 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/widgetSpec.js
--rw-r--r--   0 root         (0) root         (0)     2516 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 19:53:51.665892 girder-slicer-cli-web-1.5.4.dev2/utils/
--rw-r--r--   0 root         (0) root         (0)     3878 2024-03-22 19:53:01.000000 girder-slicer-cli-web-1.5.4.dev2/utils/xmltojson.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.882623 girder_slicer_cli_web-1.5.5.dev2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.858622 girder_slicer_cli_web-1.5.5.dev2/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     7477 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)     4000 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/.editorconfig
+-rw-r--r--   0 root         (0) root         (0)     1734 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1645 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    17374 2024-05-14 19:17:16.882623 girder_slicer_cli_web-1.5.5.dev2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15959 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.858622 girder_slicer_cli_web-1.5.5.dev2/docs/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/docs/worker_management.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.858622 girder_slicer_cli_web-1.5.5.dev2/example-average-color/
+-rw-r--r--   0 root         (0) root         (0)     4000 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-average-color/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      260 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-average-color/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      877 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-average-color/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.858622 girder_slicer_cli_web-1.5.5.dev2/example-average-color/average_color/
+-rw-r--r--   0 root         (0) root         (0)     1515 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-average-color/average_color/average_color.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-average-color/average_color/average_color.xml
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-average-color/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-average-color/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.858622 girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/
+-rw-r--r--   0 root         (0) root         (0)      290 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      507 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/README.rst
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.862623 girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/girder_requests/
+-rw-r--r--   0 root         (0) root         (0)      503 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/girder_requests/girder_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/girder_requests/girder_requests.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.882623 girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17374 2024-05-14 19:17:16.000000 girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6054 2024-05-14 19:17:16.000000 girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 19:17:16.000000 girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-14 19:17:16.000000 girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 19:16:44.000000 girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-14 19:17:16.000000 girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-14 19:17:16.000000 girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-14 19:17:16.882623 girder_slicer_cli_web-1.5.5.dev2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2714 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.862623 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/
+-rw-r--r--   0 root         (0) root         (0)     1191 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/cli_list_entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/config.py
+-rw-r--r--   0 root         (0) root         (0)     6649 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/ctk_cli_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)    15908 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/docker_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.862623 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_worker_plugin/
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_worker_plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_worker_plugin/cli_progress.py
+-rw-r--r--   0 root         (0) root         (0)     3834 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_worker_plugin/direct_docker_run.py
+-rw-r--r--   0 root         (0) root         (0)    12084 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/image_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.866623 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10406 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/docker_image.py
+-rw-r--r--   0 root         (0) root         (0)      810 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/json_to_xml.py
+-rw-r--r--   0 root         (0) root         (0)     2340 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/parser.py
+-rw-r--r--   0 root         (0) root         (0)    31703 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/schema.json
+-rw-r--r--   0 root         (0) root         (0)    14268 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/prepare_task.py
+-rw-r--r--   0 root         (0) root         (0)    25905 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/rest_slicer_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.866623 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/JobStatus.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.866623 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/collections/
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/collections/WidgetCollection.js
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/collections/index.js
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/events.js
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/index.js
+-rw-r--r--   0 root         (0) root         (0)      343 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/main.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.866623 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/models/
+-rw-r--r--   0 root         (0) root         (0)     9697 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/models/WidgetModel.js
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/models/index.js
+-rw-r--r--   0 root         (0) root         (0)     3996 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.866623 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/constraints.js
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/convert.js
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/defaultValue.js
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/group.js
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/index.js
+-rw-r--r--   0 root         (0) root         (0)      506 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/panel.js
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/param.js
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/parse.js
+-rw-r--r--   0 root         (0) root         (0)      921 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/widget.js
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/routes.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.870622 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/configView.styl
+-rw-r--r--   0 root         (0) root         (0)      964 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/controlWidget.styl
+-rw-r--r--   0 root         (0) root         (0)      112 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/controlsPanel.styl
+-rw-r--r--   0 root         (0) root         (0)       85 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/outputParameterDialog.styl
+-rw-r--r--   0 root         (0) root         (0)      662 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/panel.styl
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/panelGroup.styl
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/slicerUI.styl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.870622 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/booleanWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      115 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/colorWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     2165 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/configView.pug
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/controlsPanel.pug
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/enumerationWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/fileWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      621 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/jobsListWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      336 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/outputParameterDialog.pug
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/panel.pug
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/panelGroup.pug
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/rangeWidget.pug
+-rw-r--r--   0 root         (0) root         (0)     3623 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/regionWidget.pug
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/slicerUI.pug
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/uploadImageDialog.pug
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/widget.pug
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/utils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.874623 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/
+-rw-r--r--   0 root         (0) root         (0)     4761 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/CollectionView.js
+-rw-r--r--   0 root         (0) root         (0)     7145 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ConfigView.js
+-rw-r--r--   0 root         (0) root         (0)    17917 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ControlWidget.js
+-rw-r--r--   0 root         (0) root         (0)     1542 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ControlsPanel.js
+-rw-r--r--   0 root         (0) root         (0)    11455 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ItemSelectorWidget.js
+-rw-r--r--   0 root         (0) root         (0)     4584 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ItemView.js
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/JobsListWidget.js
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/JobsPanel.js
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/OutputParameterDialog.js
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/Panel.js
+-rw-r--r--   0 root         (0) root         (0)     8424 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/PanelGroup.js
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/index.js
+-rw-r--r--   0 root         (0) root         (0)      872 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/utils.js
+-rw-r--r--   0 root         (0) root         (0)     7792 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/worker_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.874623 girder_slicer_cli_web-1.5.5.dev2/small-docker/
+-rw-r--r--   0 root         (0) root         (0)     4000 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)      720 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.874623 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/
+-rw-r--r--   0 root         (0) root         (0)    11001 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/Example1.json
+-rw-r--r--   0 root         (0) root         (0)      681 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/Example1.py
+-rw-r--r--   0 root         (0) root         (0)    10702 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/Example1.xml
+-rw-r--r--   0 root         (0) root         (0)     7535 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/Example1.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.874623 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/Example2.json
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/Example2.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/Example2.xml
+-rw-r--r--   0 root         (0) root         (0)      639 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/Example2.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.874623 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/Example3.json
+-rw-r--r--   0 root         (0) root         (0)      621 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/Example3.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/Example3.xml
+-rw-r--r--   0 root         (0) root         (0)      626 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/Example3.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.878623 girder_slicer_cli_web-1.5.5.dev2/small-docker/ExampleProgress/
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/ExampleProgress/ExampleProgress.json
+-rw-r--r--   0 root         (0) root         (0)      884 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/ExampleProgress/ExampleProgress.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/ExampleProgress/progress_helper.py
+-rw-r--r--   0 root         (0) root         (0)      523 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/cli_list.json
+-rw-r--r--   0 root         (0) root         (0)     1397 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/small-docker/cli_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.878623 girder_slicer_cli_web-1.5.5.dev2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10313 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.878623 girder_slicer_cli_web-1.5.5.dev2/tests/data/
+-rw-r--r--   0 root         (0) root         (0)     3850 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/ExampleSpec.xml
+-rw-r--r--   0 root         (0) root         (0)      301 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/girder_worker.cfg
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_advanced.json
+-rw-r--r--   0 root         (0) root         (0)     1183 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_advanced.xml
+-rw-r--r--   0 root         (0) root         (0)      681 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_advanced.yaml
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_simple.json
+-rw-r--r--   0 root         (0) root         (0)      218 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_simple.xml
+-rw-r--r--   0 root         (0) root         (0)      109 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_simple.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_simple.json
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_simple.xml
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_simple.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.878623 girder_slicer_cli_web-1.5.5.dev2/tests/girder_worker_plugin/
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/girder_worker_plugin/test_cli_progress.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/girder_worker_plugin/test_direct_docker_run.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/test_batch.py
+-rw-r--r--   0 root         (0) root         (0)      762 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/test_docker.py
+-rwxr-xr-x   0 root         (0) root         (0)      931 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/test_load.py
+-rw-r--r--   0 root         (0) root         (0)     5923 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/test_parser.py
+-rw-r--r--   0 root         (0) root         (0)    10568 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/test_rest_slicer_cli.py
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/test_web_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.882623 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/
+-rw-r--r--   0 root         (0) root         (0)      237 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/.eslintrc
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/configViewSpec.js
+-rw-r--r--   0 root         (0) root         (0)     4543 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/containerViewSpec.js
+-rw-r--r--   0 root         (0) root         (0)     6091 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/dockerTaskSpec.js
+-rw-r--r--   0 root         (0) root         (0)     9891 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/itemSelectorWidgetSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2503 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/panelGroupSpec.js
+-rw-r--r--   0 root         (0) root         (0)    27360 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/parseSpec.js
+-rw-r--r--   0 root         (0) root         (0)    43069 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/widgetSpec.js
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 19:17:16.882623 girder_slicer_cli_web-1.5.5.dev2/utils/
+-rw-r--r--   0 root         (0) root         (0)     3878 2024-05-14 19:16:28.000000 girder_slicer_cli_web-1.5.5.dev2/utils/xmltojson.py
```

### Comparing `girder-slicer-cli-web-1.5.4.dev2/.circleci/config.yml` & `girder_slicer_cli_web-1.5.5.dev2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/.dockerignore` & `girder_slicer_cli_web-1.5.5.dev2/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/.gitignore` & `girder_slicer_cli_web-1.5.5.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/.pre-commit-config.yaml` & `girder_slicer_cli_web-1.5.5.dev2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/LICENSE` & `girder_slicer_cli_web-1.5.5.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/PKG-INFO` & `girder_slicer_cli_web-1.5.5.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-slicer-cli-web
-Version: 1.5.4.dev2
+Version: 1.5.5.dev2
 Summary: A girder plugin for exposing slicer CLIs over the web
 Home-page: https://github.com/girder/slicer_cli_web
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,slicer_cli_web
 Classifier: Development Status :: 5 - Production/Stable
@@ -108,15 +108,15 @@
 
 The XML must conform to the `Slicer Execution Schema <https://www.slicer.org/w/index.php?title=Documentation/Nightly/Developers/SlicerExecutionModel>`_, with a few minor additions:
 
 - Some types (``image``, ``file``, ``transform``, ``geometry``, ``table``, ``directory``, ``item``) can have a ``reference`` property.  When ``image``, ``file``, ``item``, ``directory`` are used with Girder, if the ``reference`` property is ``_girder_id_``, then value will be passed as a Girder ID string rather than converted to a Girder resource.
 
 - The ``region`` type can have a ``coordinateSystem`` property.
 
-- The ``region`` type has an optional ``shapes`` property that is a comma-separated list of values that can include ``default``, ``rectangle``, ``polygon``, ``line``, ``polyline``, and ``point``, plus ``multi`` and one of ``submit`` (or ``sibmitoff``), ``submiton``, or ``autosubmit``.
+- The ``region`` type has an optional ``shapes`` property that is a comma-separated list of values that can include ``default``, ``rectangle``, ``polygon``, ``line``, ``polyline``, and ``point``, plus ``multi`` and one of ``submit`` (or ``submitoff``), ``submiton``, or ``autosubmit``.
   In the official schema, region is a vector of six values of the form x,y,z,rx,ry,rz, defining a rectangle based on its center and radius in each of three dimensions.  This is the ``default`` shape.  The ``rectangle`` shape allows a vector of four values defining a rectangle of the form x,y,width,height, where x,y is the left and top of the rectangle in pixel coordinates.  Many algorithms that accept this value accept -1,-1,-1,-1 as a default to specify the whole conceptual space.  The ``polygon`` shape allows for a list of x,y values.  Polygons must always have at least four points so that the vector of values cannot be confused with the default; repeat the first vertex at the end to specify a triangle.  The ``line`` shape allows a two-vertex line.  To disambiguate this from a rectangle, the values -2,-2 are added after the line.  The ``polyline`` shape allows a multi vertex line, indicated again by a -2,-2 value after the line.  A ``point`` is a single vertex.
   ``multi`` allow multiple shapes, indicated by separating coordinates of each shape by -1,-1.  Note that neither -1,-1 nor -2,-2 are allowed as coordinates within a shape -- to use those, specify them with decimals (e.g., -1.0,-1.0).
   The submit options will add suggestions on how the UI should handle changes.  If present, the option to auto-run a job as soon as a valid shape is set should be present.  ``autosubmit`` means this should always happen.  ``submit`` or ``submitoff`` offers this as a setting but is default to not submit the job.  ``submiton`` offers this as a setting and defaults to submitting the job.
 
 - Some input types (``image``, ``file``, ``item``, ``directory``) can have ``defaultNameMatch``, ``defaultPathMatch``, and ``defaultRelativePath`` properties.  The first two are regular expressions designed to give a UI a value to match to prepopulate default values from files or paths that match the regex.  ``defaultNameMatch`` is intended to match the final path element, whereas ``defaultPathMatch`` is used on the entire path as a combined string.  ``defaultRelativePath`` is used to find a value that has a path relative to some base.  In the Girder UI, this might be from an item.
 
 - Input types can have a ``datalist`` property.  If this is present, when the CLI is first loaded or, possibly periodically after parameters have been changed, the CLI may be called with optional parameters.  The CLI is expected to return a new-line separated list of values that can be used as recommended inputs.  As an example, a ``string`` input might have a ``datalist`` of ``--enumerate-options``; the cli would be called with the existing parameters PLUS the extra parameter specified by ``datalist``.  If the result is sensible, the input control would expose this list to the user.  The ``datalist`` property is a json-encoded dictionary that overrides other parameters.  This should override parameters that aren't needed to be resolved to produce the datalist (e.g., input and output files) as that will speed up the call.  The CLI should respond to the modified call with a response that contains multiple ``<element>some text</element>`` values that will be the suggested data for the control.
```

### Comparing `girder-slicer-cli-web-1.5.4.dev2/README.rst` & `girder_slicer_cli_web-1.5.5.dev2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 The XML must conform to the `Slicer Execution Schema <https://www.slicer.org/w/index.php?title=Documentation/Nightly/Developers/SlicerExecutionModel>`_, with a few minor additions:
 
 - Some types (``image``, ``file``, ``transform``, ``geometry``, ``table``, ``directory``, ``item``) can have a ``reference`` property.  When ``image``, ``file``, ``item``, ``directory`` are used with Girder, if the ``reference`` property is ``_girder_id_``, then value will be passed as a Girder ID string rather than converted to a Girder resource.
 
 - The ``region`` type can have a ``coordinateSystem`` property.
 
-- The ``region`` type has an optional ``shapes`` property that is a comma-separated list of values that can include ``default``, ``rectangle``, ``polygon``, ``line``, ``polyline``, and ``point``, plus ``multi`` and one of ``submit`` (or ``sibmitoff``), ``submiton``, or ``autosubmit``.
+- The ``region`` type has an optional ``shapes`` property that is a comma-separated list of values that can include ``default``, ``rectangle``, ``polygon``, ``line``, ``polyline``, and ``point``, plus ``multi`` and one of ``submit`` (or ``submitoff``), ``submiton``, or ``autosubmit``.
   In the official schema, region is a vector of six values of the form x,y,z,rx,ry,rz, defining a rectangle based on its center and radius in each of three dimensions.  This is the ``default`` shape.  The ``rectangle`` shape allows a vector of four values defining a rectangle of the form x,y,width,height, where x,y is the left and top of the rectangle in pixel coordinates.  Many algorithms that accept this value accept -1,-1,-1,-1 as a default to specify the whole conceptual space.  The ``polygon`` shape allows for a list of x,y values.  Polygons must always have at least four points so that the vector of values cannot be confused with the default; repeat the first vertex at the end to specify a triangle.  The ``line`` shape allows a two-vertex line.  To disambiguate this from a rectangle, the values -2,-2 are added after the line.  The ``polyline`` shape allows a multi vertex line, indicated again by a -2,-2 value after the line.  A ``point`` is a single vertex.
   ``multi`` allow multiple shapes, indicated by separating coordinates of each shape by -1,-1.  Note that neither -1,-1 nor -2,-2 are allowed as coordinates within a shape -- to use those, specify them with decimals (e.g., -1.0,-1.0).
   The submit options will add suggestions on how the UI should handle changes.  If present, the option to auto-run a job as soon as a valid shape is set should be present.  ``autosubmit`` means this should always happen.  ``submit`` or ``submitoff`` offers this as a setting but is default to not submit the job.  ``submiton`` offers this as a setting and defaults to submitting the job.
 
 - Some input types (``image``, ``file``, ``item``, ``directory``) can have ``defaultNameMatch``, ``defaultPathMatch``, and ``defaultRelativePath`` properties.  The first two are regular expressions designed to give a UI a value to match to prepopulate default values from files or paths that match the regex.  ``defaultNameMatch`` is intended to match the final path element, whereas ``defaultPathMatch`` is used on the entire path as a combined string.  ``defaultRelativePath`` is used to find a value that has a path relative to some base.  In the Girder UI, this might be from an item.
 
 - Input types can have a ``datalist`` property.  If this is present, when the CLI is first loaded or, possibly periodically after parameters have been changed, the CLI may be called with optional parameters.  The CLI is expected to return a new-line separated list of values that can be used as recommended inputs.  As an example, a ``string`` input might have a ``datalist`` of ``--enumerate-options``; the cli would be called with the existing parameters PLUS the extra parameter specified by ``datalist``.  If the result is sensible, the input control would expose this list to the user.  The ``datalist`` property is a json-encoded dictionary that overrides other parameters.  This should override parameters that aren't needed to be resolved to produce the datalist (e.g., input and output files) as that will speed up the call.  The CLI should respond to the modified call with a response that contains multiple ``<element>some text</element>`` values that will be the suggested data for the control.
```

### Comparing `girder-slicer-cli-web-1.5.4.dev2/docs/worker_management.rst` & `girder_slicer_cli_web-1.5.5.dev2/docs/worker_management.rst`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/example-average-color/.dockerignore` & `girder_slicer_cli_web-1.5.5.dev2/example-average-color/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/example-average-color/README.rst` & `girder_slicer_cli_web-1.5.5.dev2/example-average-color/README.rst`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/example-average-color/average_color/average_color.py` & `girder_slicer_cli_web-1.5.5.dev2/example-average-color/average_color/average_color.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/example-average-color/average_color/average_color.xml` & `girder_slicer_cli_web-1.5.5.dev2/example-average-color/average_color/average_color.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/example-average-color/cli_list.py` & `girder_slicer_cli_web-1.5.5.dev2/example-average-color/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/cli_list.py` & `girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/example-girder-requests/girder_requests/girder_requests.xml` & `girder_slicer_cli_web-1.5.5.dev2/example-girder-requests/girder_requests/girder_requests.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/PKG-INFO` & `girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-slicer-cli-web
-Version: 1.5.4.dev2
+Version: 1.5.5.dev2
 Summary: A girder plugin for exposing slicer CLIs over the web
 Home-page: https://github.com/girder/slicer_cli_web
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: girder-plugin,slicer_cli_web
 Classifier: Development Status :: 5 - Production/Stable
@@ -108,15 +108,15 @@
 
 The XML must conform to the `Slicer Execution Schema <https://www.slicer.org/w/index.php?title=Documentation/Nightly/Developers/SlicerExecutionModel>`_, with a few minor additions:
 
 - Some types (``image``, ``file``, ``transform``, ``geometry``, ``table``, ``directory``, ``item``) can have a ``reference`` property.  When ``image``, ``file``, ``item``, ``directory`` are used with Girder, if the ``reference`` property is ``_girder_id_``, then value will be passed as a Girder ID string rather than converted to a Girder resource.
 
 - The ``region`` type can have a ``coordinateSystem`` property.
 
-- The ``region`` type has an optional ``shapes`` property that is a comma-separated list of values that can include ``default``, ``rectangle``, ``polygon``, ``line``, ``polyline``, and ``point``, plus ``multi`` and one of ``submit`` (or ``sibmitoff``), ``submiton``, or ``autosubmit``.
+- The ``region`` type has an optional ``shapes`` property that is a comma-separated list of values that can include ``default``, ``rectangle``, ``polygon``, ``line``, ``polyline``, and ``point``, plus ``multi`` and one of ``submit`` (or ``submitoff``), ``submiton``, or ``autosubmit``.
   In the official schema, region is a vector of six values of the form x,y,z,rx,ry,rz, defining a rectangle based on its center and radius in each of three dimensions.  This is the ``default`` shape.  The ``rectangle`` shape allows a vector of four values defining a rectangle of the form x,y,width,height, where x,y is the left and top of the rectangle in pixel coordinates.  Many algorithms that accept this value accept -1,-1,-1,-1 as a default to specify the whole conceptual space.  The ``polygon`` shape allows for a list of x,y values.  Polygons must always have at least four points so that the vector of values cannot be confused with the default; repeat the first vertex at the end to specify a triangle.  The ``line`` shape allows a two-vertex line.  To disambiguate this from a rectangle, the values -2,-2 are added after the line.  The ``polyline`` shape allows a multi vertex line, indicated again by a -2,-2 value after the line.  A ``point`` is a single vertex.
   ``multi`` allow multiple shapes, indicated by separating coordinates of each shape by -1,-1.  Note that neither -1,-1 nor -2,-2 are allowed as coordinates within a shape -- to use those, specify them with decimals (e.g., -1.0,-1.0).
   The submit options will add suggestions on how the UI should handle changes.  If present, the option to auto-run a job as soon as a valid shape is set should be present.  ``autosubmit`` means this should always happen.  ``submit`` or ``submitoff`` offers this as a setting but is default to not submit the job.  ``submiton`` offers this as a setting and defaults to submitting the job.
 
 - Some input types (``image``, ``file``, ``item``, ``directory``) can have ``defaultNameMatch``, ``defaultPathMatch``, and ``defaultRelativePath`` properties.  The first two are regular expressions designed to give a UI a value to match to prepopulate default values from files or paths that match the regex.  ``defaultNameMatch`` is intended to match the final path element, whereas ``defaultPathMatch`` is used on the entire path as a combined string.  ``defaultRelativePath`` is used to find a value that has a path relative to some base.  In the Girder UI, this might be from an item.
 
 - Input types can have a ``datalist`` property.  If this is present, when the CLI is first loaded or, possibly periodically after parameters have been changed, the CLI may be called with optional parameters.  The CLI is expected to return a new-line separated list of values that can be used as recommended inputs.  As an example, a ``string`` input might have a ``datalist`` of ``--enumerate-options``; the cli would be called with the existing parameters PLUS the extra parameter specified by ``datalist``.  If the result is sensible, the input control would expose this list to the user.  The ``datalist`` property is a json-encoded dictionary that overrides other parameters.  This should override parameters that aren't needed to be resolved to produce the datalist (e.g., input and output files) as that will speed up the call.  The CLI should respond to the modified call with a response that contains multiple ``<element>some text</element>`` values that will be the suggested data for the control.
```

### Comparing `girder-slicer-cli-web-1.5.4.dev2/girder_slicer_cli_web.egg-info/SOURCES.txt` & `girder_slicer_cli_web-1.5.5.dev2/girder_slicer_cli_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/setup.py` & `girder_slicer_cli_web-1.5.5.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/__init__.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/cli_list_entrypoint.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/cli_list_entrypoint.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/cli_utils.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/cli_utils.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/config.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/config.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/ctk_cli_adjustment.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/ctk_cli_adjustment.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/docker_resource.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/docker_resource.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_plugin.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_plugin.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_worker_plugin/__init__.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_worker_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_worker_plugin/cli_progress.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_worker_plugin/cli_progress.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/girder_worker_plugin/direct_docker_run.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/girder_worker_plugin/direct_docker_run.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/image_job.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/image_job.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/docker_image.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/docker_image.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/exceptions.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/json_to_xml.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/json_to_xml.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/parser.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/parser.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/models/schema.json` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/models/schema.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/prepare_task.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/prepare_task.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/rest_slicer_cli.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/rest_slicer_cli.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/collections/WidgetCollection.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/collections/WidgetCollection.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/models/WidgetModel.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/models/WidgetModel.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/package.json` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/constraints.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/constraints.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/convert.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/convert.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/defaultValue.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/defaultValue.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/group.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/group.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/param.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/param.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/parse.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/parse.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/parser/widget.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/parser/widget.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/controlWidget.styl` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/controlWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/stylesheets/panel.styl` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/stylesheets/panel.styl`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/configView.pug` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/fileWidget.pug` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/fileWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/jobsListWidget.pug` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/jobsListWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/panelGroup.pug` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/panelGroup.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/regionWidget.pug` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/regionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/uploadImageDialog.pug` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/uploadImageDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/templates/widget.pug` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/templates/widget.pug`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/utils.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/utils.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/CollectionView.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/CollectionView.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ConfigView.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ControlWidget.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ControlWidget.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ControlsPanel.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ControlsPanel.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ItemSelectorWidget.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ItemSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/ItemView.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/JobsListWidget.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/JobsListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/JobsPanel.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/JobsPanel.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/OutputParameterDialog.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/OutputParameterDialog.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/Panel.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/Panel.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/PanelGroup.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/PanelGroup.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/web_client/views/utils.js` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/web_client/views/utils.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/slicer_cli_web/worker_tools.py` & `girder_slicer_cli_web-1.5.5.dev2/slicer_cli_web/worker_tools.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/.dockerignore` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/.dockerignore`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Dockerfile` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/Example1.json` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/Example1.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/Example1.py` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/Example1.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/Example1.xml` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/Example1.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example1/Example1.yaml` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example1/Example1.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/Example2.json` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/Example2.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/Example2.py` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/Example2.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/Example2.xml` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/Example2.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example2/Example2.yaml` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example2/Example2.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/Example3.json` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/Example3.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/Example3.py` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/Example3.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/Example3.xml` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/Example3.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/Example3/Example3.yaml` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/Example3/Example3.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/ExampleProgress/ExampleProgress.json` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/ExampleProgress/ExampleProgress.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/ExampleProgress/ExampleProgress.py` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/ExampleProgress/ExampleProgress.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/ExampleProgress/progress_helper.py` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/ExampleProgress/progress_helper.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/cli_list.json` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/cli_list.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/small-docker/cli_list.py` & `girder_slicer_cli_web-1.5.5.dev2/small-docker/cli_list.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/conftest.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/data/ExampleSpec.xml` & `girder_slicer_cli_web-1.5.5.dev2/tests/data/ExampleSpec.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_advanced.json` & `girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_advanced.json`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_advanced.xml` & `girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_advanced.xml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/data/parser_params_advanced.yaml` & `girder_slicer_cli_web-1.5.5.dev2/tests/data/parser_params_advanced.yaml`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/girder_worker_plugin/test_cli_progress.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/girder_worker_plugin/test_cli_progress.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/girder_worker_plugin/test_direct_docker_run.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/girder_worker_plugin/test_direct_docker_run.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/test_batch.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/test_config.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/test_docker.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/test_load.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/test_parser.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/test_rest_slicer_cli.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/test_rest_slicer_cli.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/test_web_client.py` & `girder_slicer_cli_web-1.5.5.dev2/tests/test_web_client.py`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/configViewSpec.js` & `girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/configViewSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/containerViewSpec.js` & `girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/containerViewSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/dockerTaskSpec.js` & `girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/dockerTaskSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/itemSelectorWidgetSpec.js` & `girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/itemSelectorWidgetSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/panelGroupSpec.js` & `girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/panelGroupSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/parseSpec.js` & `girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/parseSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tests/web_client_specs/widgetSpec.js` & `girder_slicer_cli_web-1.5.5.dev2/tests/web_client_specs/widgetSpec.js`

 * *Files identical despite different names*

### Comparing `girder-slicer-cli-web-1.5.4.dev2/tox.ini` & `girder_slicer_cli_web-1.5.5.dev2/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 [testenv]
 passenv =
   DOCKER_*
   PYTEST_*
 deps =
   coverage
   mock
-  pytest>=3.6
-  pytest-cov>=2.6
+  pytest
+  pytest-cov
   pytest-forked
-  pytest-girder>=3.1.25.dev9
+  pytest-girder
   pytest-mock
   pytest-xdist
   celery
-  urllib3<1.26
+  urllib3
 extras =
   girder
   worker
 allowlist_externals =
   mkdir
   npx
   rm
```

### Comparing `girder-slicer-cli-web-1.5.4.dev2/utils/xmltojson.py` & `girder_slicer_cli_web-1.5.5.dev2/utils/xmltojson.py`

 * *Files identical despite different names*

