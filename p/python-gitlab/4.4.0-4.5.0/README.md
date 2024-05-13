# Comparing `tmp/python-gitlab-4.4.0.tar.gz` & `tmp/python_gitlab-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-gitlab-4.4.0.tar", last modified: Mon Jan 15 08:15:09 2024, max compression
+gzip compressed data, was "python_gitlab-4.5.0.tar", last modified: Mon May 13 22:19:49 2024, max compression
```

## Comparing `python-gitlab-4.4.0.tar` & `python_gitlab-4.5.0.tar`

### file list

```diff
@@ -1,358 +1,359 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.669729 python-gitlab-4.4.0/
--rw-r--r--   0 root         (0) root         (0)      526 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)   688509 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     7651 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/COPYING
--rw-r--r--   0 root         (0) root         (0)      189 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7662 2024-01-15 08:15:09.669729 python-gitlab-4.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5911 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.605728 python-gitlab-4.4.0/docs/
--rw-r--r--   0 root         (0) root         (0)     6790 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.597728 python-gitlab-4.4.0/docs/_static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.605728 python-gitlab-4.4.0/docs/_static/js/
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/_static/js/gitter.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.605728 python-gitlab-4.4.0/docs/api/
--rw-r--r--   0 root         (0) root         (0)     1362 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/api/gitlab.rst
--rw-r--r--   0 root         (0) root         (0)      320 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/api/gitlab.v4.rst
--rw-r--r--   0 root         (0) root         (0)     4280 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/api-levels.rst
--rw-r--r--   0 root         (0) root         (0)     1702 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/api-objects.rst
--rw-r--r--   0 root         (0) root         (0)     6622 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/api-usage-advanced.rst
--rw-r--r--   0 root         (0) root         (0)    15100 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/api-usage.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/changelog.md
--rw-r--r--   0 root         (0) root         (0)     7676 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/cli-examples.rst
--rw-r--r--   0 root         (0) root         (0)      643 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/cli-objects.rst
--rw-r--r--   0 root         (0) root         (0)    11215 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/cli-usage.rst
--rw-r--r--   0 root         (0) root         (0)     9858 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.609728 python-gitlab-4.4.0/docs/ext/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/ext/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1722 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/ext/docstrings.py
--rw-r--r--   0 root         (0) root         (0)     1246 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/ext/manager_tmpl.j2
--rw-r--r--   0 root         (0) root         (0)     2927 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/faq.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.621729 python-gitlab-4.4.0/docs/gl_objects/
--rw-r--r--   0 root         (0) root         (0)     1487 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/access_requests.rst
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/appearance.rst
--rw-r--r--   0 root         (0) root         (0)      619 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/applications.rst
--rw-r--r--   0 root         (0) root         (0)     1088 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/badges.rst
--rw-r--r--   0 root         (0) root         (0)     2409 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/boards.rst
--rw-r--r--   0 root         (0) root         (0)      848 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/branches.rst
--rw-r--r--   0 root         (0) root         (0)     2142 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/bulk_imports.rst
--rw-r--r--   0 root         (0) root         (0)     1865 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/ci_lint.rst
--rw-r--r--   0 root         (0) root         (0)     1930 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/clusters.rst
--rw-r--r--   0 root         (0) root         (0)     3354 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/commits.rst
--rw-r--r--   0 root         (0) root         (0)     1247 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/deploy_keys.rst
--rw-r--r--   0 root         (0) root         (0)     4093 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/deploy_tokens.rst
--rw-r--r--   0 root         (0) root         (0)     1803 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/deployments.rst
--rw-r--r--   0 root         (0) root         (0)     3431 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/discussions.rst
--rw-r--r--   0 root         (0) root         (0)     1461 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/draft_notes.rst
--rw-r--r--   0 root         (0) root         (0)     1196 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/emojis.rst
--rw-r--r--   0 root         (0) root         (0)      984 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/environments.rst
--rw-r--r--   0 root         (0) root         (0)     1302 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/epics.rst
--rw-r--r--   0 root         (0) root         (0)     2206 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/events.rst
--rw-r--r--   0 root         (0) root         (0)      625 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/features.rst
--rw-r--r--   0 root         (0) root         (0)      718 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/geo_nodes.rst
--rw-r--r--   0 root         (0) root         (0)     1128 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/group_access_tokens.rst
--rw-r--r--   0 root         (0) root         (0)    10727 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/groups.rst
--rw-r--r--   0 root         (0) root         (0)     2057 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/invitations.rst
--rw-r--r--   0 root         (0) root         (0)     7003 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/issues.rst
--rw-r--r--   0 root         (0) root         (0)      694 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/iterations.rst
--rw-r--r--   0 root         (0) root         (0)     1348 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/job_token_scope.rst
--rw-r--r--   0 root         (0) root         (0)      490 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/keys.rst
--rw-r--r--   0 root         (0) root         (0)     2292 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/labels.rst
--rw-r--r--   0 root         (0) root         (0)     2923 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/merge_request_approvals.rst
--rw-r--r--   0 root         (0) root         (0)     5625 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/merge_requests.rst
--rw-r--r--   0 root         (0) root         (0)      625 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/merge_trains.rst
--rw-r--r--   0 root         (0) root         (0)      988 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/messages.rst
--rw-r--r--   0 root         (0) root         (0)     2671 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/milestones.rst
--rw-r--r--   0 root         (0) root         (0)      697 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/namespaces.rst
--rw-r--r--   0 root         (0) root         (0)     1675 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/notes.rst
--rw-r--r--   0 root         (0) root         (0)     1877 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/notifications.rst
--rw-r--r--   0 root         (0) root         (0)     3520 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/packages.rst
--rw-r--r--   0 root         (0) root         (0)     1240 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/pagesdomains.rst
--rw-r--r--   0 root         (0) root         (0)     2089 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/personal_access_tokens.rst
--rw-r--r--   0 root         (0) root         (0)     9572 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/pipelines_and_jobs.rst
--rw-r--r--   0 root         (0) root         (0)     1162 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/project_access_tokens.rst
--rw-r--r--   0 root         (0) root         (0)    22202 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/projects.rst
--rw-r--r--   0 root         (0) root         (0)     1369 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/protected_branches.rst
--rw-r--r--   0 root         (0) root         (0)     1061 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/protected_environments.rst
--rw-r--r--   0 root         (0) root         (0)     2038 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/releases.rst
--rw-r--r--   0 root         (0) root         (0)      901 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/remote_mirrors.rst
--rw-r--r--   0 root         (0) root         (0)      760 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/repositories.rst
--rw-r--r--   0 root         (0) root         (0)     1128 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/repository_tags.rst
--rw-r--r--   0 root         (0) root         (0)      970 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/resource_groups.rst
--rw-r--r--   0 root         (0) root         (0)     3906 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/runners.rst
--rw-r--r--   0 root         (0) root         (0)     2351 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/search.rst
--rw-r--r--   0 root         (0) root         (0)     1036 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/secure_files.rst
--rw-r--r--   0 root         (0) root         (0)      417 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/settings.rst
--rw-r--r--   0 root         (0) root         (0)      393 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/sidekiq.rst
--rw-r--r--   0 root         (0) root         (0)     1585 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/snippets.rst
--rw-r--r--   0 root         (0) root         (0)      357 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/statistics.rst
--rw-r--r--   0 root         (0) root         (0)      596 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/system_hooks.rst
--rw-r--r--   0 root         (0) root         (0)     2062 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/templates.rst
--rw-r--r--   0 root         (0) root         (0)      840 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/todos.rst
--rw-r--r--   0 root         (0) root         (0)      969 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/topics.rst
--rw-r--r--   0 root         (0) root         (0)    11029 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/users.rst
--rw-r--r--   0 root         (0) root         (0)     2513 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/variables.rst
--rw-r--r--   0 root         (0) root         (0)     2393 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/gl_objects/wikis.rst
--rw-r--r--   0 root         (0) root         (0)      337 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6715 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     8182 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/docs/release-notes.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.625728 python-gitlab-4.4.0/gitlab/
--rw-r--r--   0 root         (0) root         (0)     1382 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)       68 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.625728 python-gitlab-4.4.0/gitlab/_backends/
--rw-r--r--   0 root         (0) root         (0)      392 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/_backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)      858 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/_backends/protocol.py
--rw-r--r--   0 root         (0) root         (0)     5534 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/_backends/requests_backend.py
--rw-r--r--   0 root         (0) root         (0)      249 2024-01-15 08:15:03.000000 python-gitlab-4.4.0/gitlab/_version.py
--rw-r--r--   0 root         (0) root         (0)    13780 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/base.py
--rw-r--r--   0 root         (0) root         (0)    12443 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/cli.py
--rw-r--r--   0 root         (0) root         (0)    48756 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/client.py
--rw-r--r--   0 root         (0) root         (0)     9088 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/config.py
--rw-r--r--   0 root         (0) root         (0)     5352 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/const.py
--rw-r--r--   0 root         (0) root         (0)     8303 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    36350 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/mixins.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/py.typed
--rw-r--r--   0 root         (0) root         (0)     3312 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/types.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.625728 python-gitlab-4.4.0/gitlab/v4/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20962 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.641728 python-gitlab-4.4.0/gitlab/v4/objects/
--rw-r--r--   0 root         (0) root         (0)     1958 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/access_requests.py
--rw-r--r--   0 root         (0) root         (0)     1932 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/appearance.py
--rw-r--r--   0 root         (0) root         (0)      591 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/applications.py
--rw-r--r--   0 root         (0) root         (0)     5020 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1909 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/audit_events.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/award_emojis.py
--rw-r--r--   0 root         (0) root         (0)     1464 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/badges.py
--rw-r--r--   0 root         (0) root         (0)     2680 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/boards.py
--rw-r--r--   0 root         (0) root         (0)     1706 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/branches.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/broadcast_messages.py
--rw-r--r--   0 root         (0) root         (0)     1573 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/bulk_imports.py
--rw-r--r--   0 root         (0) root         (0)     2270 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/ci_lint.py
--rw-r--r--   0 root         (0) root         (0)     3750 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/clusters.py
--rw-r--r--   0 root         (0) root         (0)     8214 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/commits.py
--rw-r--r--   0 root         (0) root         (0)     3341 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     1875 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/custom_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1826 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/deploy_keys.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/deploy_tokens.py
--rw-r--r--   0 root         (0) root         (0)     2879 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/deployments.py
--rw-r--r--   0 root         (0) root         (0)     3457 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/discussions.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/draft_notes.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/environments.py
--rw-r--r--   0 root         (0) root         (0)     4150 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/epics.py
--rw-r--r--   0 root         (0) root         (0)     7067 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/events.py
--rw-r--r--   0 root         (0) root         (0)     1909 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/export_import.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/features.py
--rw-r--r--   0 root         (0) root         (0)    10283 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/files.py
--rw-r--r--   0 root         (0) root         (0)     3646 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/geo_nodes.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/group_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)    15672 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/groups.py
--rw-r--r--   0 root         (0) root         (0)     3598 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/hooks.py
--rw-r--r--   0 root         (0) root         (0)     9205 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/integrations.py
--rw-r--r--   0 root         (0) root         (0)     2734 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/invitations.py
--rw-r--r--   0 root         (0) root         (0)    10162 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/issues.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/iterations.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/job_token_scope.py
--rw-r--r--   0 root         (0) root         (0)     9025 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/jobs.py
--rw-r--r--   0 root         (0) root         (0)      882 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/keys.py
--rw-r--r--   0 root         (0) root         (0)     4736 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/labels.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/ldap.py
--rw-r--r--   0 root         (0) root         (0)     3836 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/members.py
--rw-r--r--   0 root         (0) root         (0)     8181 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/merge_request_approvals.py
--rw-r--r--   0 root         (0) root         (0)    17305 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/merge_requests.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/merge_trains.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/milestones.py
--rw-r--r--   0 root         (0) root         (0)     1502 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/namespaces.py
--rw-r--r--   0 root         (0) root         (0)     8588 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/notes.py
--rw-r--r--   0 root         (0) root         (0)     2061 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/notification_settings.py
--rw-r--r--   0 root         (0) root         (0)     7187 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/packages.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/pages.py
--rw-r--r--   0 root         (0) root         (0)     1315 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/personal_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)     9723 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/pipelines.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/project_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)    44126 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/projects.py
--rw-r--r--   0 root         (0) root         (0)     3041 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/push_rules.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/releases.py
--rw-r--r--   0 root         (0) root         (0)    11047 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/repositories.py
--rw-r--r--   0 root         (0) root         (0)     1427 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/resource_groups.py
--rw-r--r--   0 root         (0) root         (0)      517 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/reviewers.py
--rw-r--r--   0 root         (0) root         (0)     4883 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/runners.py
--rw-r--r--   0 root         (0) root         (0)     2510 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/secure_files.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/settings.py
--rw-r--r--   0 root         (0) root         (0)     2956 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/sidekiq.py
--rw-r--r--   0 root         (0) root         (0)     6018 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/snippets.py
--rw-r--r--   0 root         (0) root         (0)     2638 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/statistics.py
--rw-r--r--   0 root         (0) root         (0)     1453 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/tags.py
--rw-r--r--   0 root         (0) root         (0)     1726 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/templates.py
--rw-r--r--   0 root         (0) root         (0)     1826 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/todos.py
--rw-r--r--   0 root         (0) root         (0)     2199 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/topics.py
--rw-r--r--   0 root         (0) root         (0)      824 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/triggers.py
--rw-r--r--   0 root         (0) root         (0)    21280 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/users.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/variables.py
--rw-r--r--   0 root         (0) root         (0)     1775 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/gitlab/v4/objects/wikis.py
--rw-r--r--   0 root         (0) root         (0)     4018 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.669729 python-gitlab-4.4.0/python_gitlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7662 2024-01-15 08:15:09.000000 python-gitlab-4.4.0/python_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10621 2024-01-15 08:15:09.000000 python-gitlab-4.4.0/python_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-15 08:15:09.000000 python-gitlab-4.4.0/python_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-01-15 08:15:09.000000 python-gitlab-4.4.0/python_gitlab.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      106 2024-01-15 08:15:09.000000 python-gitlab-4.4.0/python_gitlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-01-15 08:15:09.000000 python-gitlab-4.4.0/python_gitlab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/requirements-docker.txt
--rw-r--r--   0 root         (0) root         (0)      116 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/requirements-docs.txt
--rw-r--r--   0 root         (0) root         (0)      249 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/requirements-lint.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/requirements-precommit.txt
--rw-r--r--   0 root         (0) root         (0)      204 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/requirements-test.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-15 08:15:09.669729 python-gitlab-4.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.641728 python-gitlab-4.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1090 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.641728 python-gitlab-4.4.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.649729 python-gitlab-4.4.0/tests/functional/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      476 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_boards.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_branches.py
--rw-r--r--   0 root         (0) root         (0)     1216 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_bulk_imports.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_current_user.py
--rw-r--r--   0 root         (0) root         (0)      444 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_deploy_keys.py
--rw-r--r--   0 root         (0) root         (0)     1385 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_deploy_tokens.py
--rw-r--r--   0 root         (0) root         (0)      777 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_epics.py
--rw-r--r--   0 root         (0) root         (0)     7874 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)     9817 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_groups.py
--rw-r--r--   0 root         (0) root         (0)     3061 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_import_export.py
--rw-r--r--   0 root         (0) root         (0)     3800 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_issues.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_keys.py
--rw-r--r--   0 root         (0) root         (0)     1198 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_lazy_objects.py
--rw-r--r--   0 root         (0) root         (0)     9078 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_merge_requests.py
--rw-r--r--   0 root         (0) root         (0)     3908 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_packages.py
--rw-r--r--   0 root         (0) root         (0)    10821 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_projects.py
--rw-r--r--   0 root         (0) root         (0)      710 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_push_rules.py
--rw-r--r--   0 root         (0) root         (0)     2066 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_releases.py
--rw-r--r--   0 root         (0) root         (0)     5708 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_repository.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_services.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_snippets.py
--rw-r--r--   0 root         (0) root         (0)      295 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_statistics.py
--rw-r--r--   0 root         (0) root         (0)     1003 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_topics.py
--rw-r--r--   0 root         (0) root         (0)     5014 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_users.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_variables.py
--rw-r--r--   0 root         (0) root         (0)     1728 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/api/test_wikis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.649729 python-gitlab-4.4.0/tests/functional/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/conftest.py
--rw-r--r--   0 root         (0) root         (0)     6787 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2386 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli_artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1320 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli_packages.py
--rw-r--r--   0 root         (0) root         (0)     1692 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli_projects.py
--rw-r--r--   0 root         (0) root         (0)     3448 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli_repository.py
--rw-r--r--   0 root         (0) root         (0)     1057 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli_resource_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli_users.py
--rw-r--r--   0 root         (0) root         (0)    16248 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli_v4.py
--rw-r--r--   0 root         (0) root         (0)     1416 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/cli/test_cli_variables.py
--rw-r--r--   0 root         (0) root         (0)    21320 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/conftest.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/ee-test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.653729 python-gitlab-4.4.0/tests/functional/fixtures/
--rw-r--r--   0 root         (0) root         (0)       53 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/.env
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      592 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/avatar.png
--rw-r--r--   0 root         (0) root         (0)     1892 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/create_license.rb
--rw-r--r--   0 root         (0) root         (0)     1717 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/docker.py
--rw-r--r--   0 root         (0) root         (0)       55 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/invalid_auth.cfg
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/invalid_version.cfg
--rw-r--r--   0 root         (0) root         (0)      322 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/fixtures/set_token.rb
--rw-r--r--   0 root         (0) root         (0)     1564 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/functional/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.653729 python-gitlab-4.4.0/tests/install/
--rw-r--r--   0 root         (0) root         (0)      125 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/install/test_install.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.653729 python-gitlab-4.4.0/tests/smoke/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/smoke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1461 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/smoke/test_dists.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.657729 python-gitlab-4.4.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.657729 python-gitlab-4.4.0/tests/unit/_backends/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/_backends/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1765 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/_backends/test_requests_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.657729 python-gitlab-4.4.0/tests/unit/base/
--rw-r--r--   0 root         (0) root         (0)      734 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/base/test_rest_manager.py
--rw-r--r--   0 root         (0) root         (0)    10861 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/base/test_rest_object.py
--rw-r--r--   0 root         (0) root         (0)     3194 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2695 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.657729 python-gitlab-4.4.0/tests/unit/meta/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4352 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/meta/test_ensure_type_hints.py
--rw-r--r--   0 root         (0) root         (0)     1242 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/meta/test_imports.py
--rw-r--r--   0 root         (0) root         (0)     4023 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/meta/test_mro.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.657729 python-gitlab-4.4.0/tests/unit/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/mixins/test_meta_mixins.py
--rw-r--r--   0 root         (0) root         (0)    16409 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/mixins/test_mixin_methods.py
--rw-r--r--   0 root         (0) root         (0)     1218 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/mixins/test_object_mixins_attributes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 08:15:09.669729 python-gitlab-4.4.0/tests/unit/objects/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2212 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/conftest.py
--rw-r--r--   0 root         (0) root         (0)     2063 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_appearance.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_applications.py
--rw-r--r--   0 root         (0) root         (0)     2928 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_audit_events.py
--rw-r--r--   0 root         (0) root         (0)     5723 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_badges.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_bridges.py
--rw-r--r--   0 root         (0) root         (0)     4437 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_bulk_imports.py
--rw-r--r--   0 root         (0) root         (0)     2699 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_ci_lint.py
--rw-r--r--   0 root         (0) root         (0)     3345 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_commits.py
--rw-r--r--   0 root         (0) root         (0)     1299 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_deploy_tokens.py
--rw-r--r--   0 root         (0) root         (0)     5437 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_deployments.py
--rw-r--r--   0 root         (0) root         (0)     5088 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_draft_notes.py
--rw-r--r--   0 root         (0) root         (0)     1721 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_environments.py
--rw-r--r--   0 root         (0) root         (0)     3914 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_group_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)    14054 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_groups.py
--rw-r--r--   0 root         (0) root         (0)     5269 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_hooks.py
--rw-r--r--   0 root         (0) root         (0)     4748 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_invitations.py
--rw-r--r--   0 root         (0) root         (0)     2999 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_issues.py
--rw-r--r--   0 root         (0) root         (0)     1210 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_iterations.py
--rw-r--r--   0 root         (0) root         (0)     1226 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_job_artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1786 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_job_token_scope.py
--rw-r--r--   0 root         (0) root         (0)     2364 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_jobs.py
--rw-r--r--   0 root         (0) root         (0)     1329 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_keys.py
--rw-r--r--   0 root         (0) root         (0)     2235 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_members.py
--rw-r--r--   0 root         (0) root         (0)     1644 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_merge_request_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     3640 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_merge_requests.py
--rw-r--r--   0 root         (0) root         (0)     2011 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_merge_trains.py
--rw-r--r--   0 root         (0) root         (0)    12877 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_packages.py
--rw-r--r--   0 root         (0) root         (0)     4464 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_personal_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)     3222 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_pipeline_schedules.py
--rw-r--r--   0 root         (0) root         (0)     5553 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_project_access_tokens.py
--rw-r--r--   0 root         (0) root         (0)     6453 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_project_import_export.py
--rw-r--r--   0 root         (0) root         (0)    10274 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_project_merge_request_approvals.py
--rw-r--r--   0 root         (0) root         (0)      823 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_project_statistics.py
--rw-r--r--   0 root         (0) root         (0)    21091 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_projects.py
--rw-r--r--   0 root         (0) root         (0)     2679 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_registry_repositories.py
--rw-r--r--   0 root         (0) root         (0)     4214 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_releases.py
--rw-r--r--   0 root         (0) root         (0)     2607 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_remote_mirrors.py
--rw-r--r--   0 root         (0) root         (0)     1382 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_repositories.py
--rw-r--r--   0 root         (0) root         (0)     2423 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_resource_groups.py
--rw-r--r--   0 root         (0) root         (0)     1717 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_resource_iteration_events.py
--rw-r--r--   0 root         (0) root         (0)     3424 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_resource_label_events.py
--rw-r--r--   0 root         (0) root         (0)     2458 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_resource_milestone_events.py
--rw-r--r--   0 root         (0) root         (0)     3195 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_resource_state_events.py
--rw-r--r--   0 root         (0) root         (0)     8133 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_runners.py
--rw-r--r--   0 root         (0) root         (0)     2942 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_secure_files.py
--rw-r--r--   0 root         (0) root         (0)     3169 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_services.py
--rw-r--r--   0 root         (0) root         (0)     2498 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_snippets.py
--rw-r--r--   0 root         (0) root         (0)     1334 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_statistics.py
--rw-r--r--   0 root         (0) root         (0)     1454 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_submodules.py
--rw-r--r--   0 root         (0) root         (0)     2192 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_todos.py
--rw-r--r--   0 root         (0) root         (0)     3298 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_topics.py
--rw-r--r--   0 root         (0) root         (0)     8576 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_users.py
--rw-r--r--   0 root         (0) root         (0)     5173 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/objects/test_variables.py
--rw-r--r--   0 root         (0) root         (0)     5216 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/test_cli.py
--rw-r--r--   0 root         (0) root         (0)    11083 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/test_config.py
--rw-r--r--   0 root         (0) root         (0)      800 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/test_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12171 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)     7347 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/test_gitlab_auth.py
--rw-r--r--   0 root         (0) root         (0)    25165 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/test_gitlab_http_methods.py
--rw-r--r--   0 root         (0) root         (0)     4011 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/test_types.py
--rw-r--r--   0 root         (0) root         (0)     6441 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tests/unit/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2972 2024-01-15 08:15:02.000000 python-gitlab-4.4.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.682675 python_gitlab-4.5.0/
+-rw-r--r--   0 root         (0) root         (0)      526 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)   704321 2024-05-13 22:19:43.000000 python_gitlab-4.5.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     7651 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8223 2024-05-13 22:19:49.682675 python_gitlab-4.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6472 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.618675 python_gitlab-4.5.0/docs/
+-rw-r--r--   0 root         (0) root         (0)     6790 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.606675 python_gitlab-4.5.0/docs/_static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.618675 python_gitlab-4.5.0/docs/_static/js/
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/_static/js/gitter.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.618675 python_gitlab-4.5.0/docs/api/
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api/gitlab.rst
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api/gitlab.v4.rst
+-rw-r--r--   0 root         (0) root         (0)     4280 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api-levels.rst
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api-objects.rst
+-rw-r--r--   0 root         (0) root         (0)     6622 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api-usage-advanced.rst
+-rw-r--r--   0 root         (0) root         (0)    15176 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/api-usage.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/changelog.md
+-rw-r--r--   0 root         (0) root         (0)     7780 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/cli-examples.rst
+-rw-r--r--   0 root         (0) root         (0)      643 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/cli-objects.rst
+-rw-r--r--   0 root         (0) root         (0)    11215 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/cli-usage.rst
+-rw-r--r--   0 root         (0) root         (0)     9858 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.618675 python_gitlab-4.5.0/docs/ext/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/ext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/ext/docstrings.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/ext/manager_tmpl.j2
+-rw-r--r--   0 root         (0) root         (0)     3828 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/faq.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.630675 python_gitlab-4.5.0/docs/gl_objects/
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/access_requests.rst
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/appearance.rst
+-rw-r--r--   0 root         (0) root         (0)      619 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/applications.rst
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/badges.rst
+-rw-r--r--   0 root         (0) root         (0)     2409 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/boards.rst
+-rw-r--r--   0 root         (0) root         (0)      848 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/branches.rst
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/bulk_imports.rst
+-rw-r--r--   0 root         (0) root         (0)     1865 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/ci_lint.rst
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/clusters.rst
+-rw-r--r--   0 root         (0) root         (0)     3354 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/commits.rst
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/deploy_keys.rst
+-rw-r--r--   0 root         (0) root         (0)     4093 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/deploy_tokens.rst
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/deployments.rst
+-rw-r--r--   0 root         (0) root         (0)     3431 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/discussions.rst
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/draft_notes.rst
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/emojis.rst
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/environments.rst
+-rw-r--r--   0 root         (0) root         (0)     1302 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/epics.rst
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/events.rst
+-rw-r--r--   0 root         (0) root         (0)      625 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/features.rst
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/geo_nodes.rst
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/group_access_tokens.rst
+-rw-r--r--   0 root         (0) root         (0)    10727 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/groups.rst
+-rw-r--r--   0 root         (0) root         (0)     2057 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/invitations.rst
+-rw-r--r--   0 root         (0) root         (0)     7003 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/issues.rst
+-rw-r--r--   0 root         (0) root         (0)      694 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/iterations.rst
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/job_token_scope.rst
+-rw-r--r--   0 root         (0) root         (0)      490 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/keys.rst
+-rw-r--r--   0 root         (0) root         (0)     2292 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/labels.rst
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/merge_request_approvals.rst
+-rw-r--r--   0 root         (0) root         (0)     5625 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/merge_requests.rst
+-rw-r--r--   0 root         (0) root         (0)      625 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/merge_trains.rst
+-rw-r--r--   0 root         (0) root         (0)      988 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/messages.rst
+-rw-r--r--   0 root         (0) root         (0)     2671 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/milestones.rst
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/namespaces.rst
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/notes.rst
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/notifications.rst
+-rw-r--r--   0 root         (0) root         (0)     3520 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/packages.rst
+-rw-r--r--   0 root         (0) root         (0)     1240 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/pagesdomains.rst
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/personal_access_tokens.rst
+-rw-r--r--   0 root         (0) root         (0)     9572 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/pipelines_and_jobs.rst
+-rw-r--r--   0 root         (0) root         (0)     1162 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/project_access_tokens.rst
+-rw-r--r--   0 root         (0) root         (0)    22202 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/projects.rst
+-rw-r--r--   0 root         (0) root         (0)     1456 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/protected_branches.rst
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/protected_environments.rst
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/releases.rst
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/remote_mirrors.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/repositories.rst
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/repository_tags.rst
+-rw-r--r--   0 root         (0) root         (0)      970 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/resource_groups.rst
+-rw-r--r--   0 root         (0) root         (0)     3906 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/runners.rst
+-rw-r--r--   0 root         (0) root         (0)     2351 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/search.rst
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/secure_files.rst
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/settings.rst
+-rw-r--r--   0 root         (0) root         (0)      393 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/sidekiq.rst
+-rw-r--r--   0 root         (0) root         (0)     1585 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/snippets.rst
+-rw-r--r--   0 root         (0) root         (0)      357 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/statistics.rst
+-rw-r--r--   0 root         (0) root         (0)      596 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/system_hooks.rst
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/templates.rst
+-rw-r--r--   0 root         (0) root         (0)      840 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/todos.rst
+-rw-r--r--   0 root         (0) root         (0)      969 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/topics.rst
+-rw-r--r--   0 root         (0) root         (0)    11029 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/users.rst
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/variables.rst
+-rw-r--r--   0 root         (0) root         (0)     2393 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/gl_objects/wikis.rst
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6715 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)     8182 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/docs/release-notes.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.634675 python_gitlab-4.5.0/gitlab/
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.634675 python_gitlab-4.5.0/gitlab/_backends/
+-rw-r--r--   0 root         (0) root         (0)      392 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/_backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/_backends/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     5534 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/_backends/requests_backend.py
+-rw-r--r--   0 root         (0) root         (0)      249 2024-05-13 22:19:43.000000 python_gitlab-4.5.0/gitlab/_version.py
+-rw-r--r--   0 root         (0) root         (0)    13780 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/base.py
+-rw-r--r--   0 root         (0) root         (0)    12870 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/cli.py
+-rw-r--r--   0 root         (0) root         (0)    48755 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/client.py
+-rw-r--r--   0 root         (0) root         (0)     9088 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/config.py
+-rw-r--r--   0 root         (0) root         (0)     5352 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/const.py
+-rw-r--r--   0 root         (0) root         (0)     8303 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    36350 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/mixins.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/py.typed
+-rw-r--r--   0 root         (0) root         (0)     3312 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/types.py
+-rw-r--r--   0 root         (0) root         (0)     6396 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.634675 python_gitlab-4.5.0/gitlab/v4/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21455 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.650675 python_gitlab-4.5.0/gitlab/v4/objects/
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/access_requests.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/appearance.py
+-rw-r--r--   0 root         (0) root         (0)      591 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/applications.py
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/audit_events.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/award_emojis.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/badges.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/boards.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/branches.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/broadcast_messages.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/bulk_imports.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/ci_lint.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/clusters.py
+-rw-r--r--   0 root         (0) root         (0)     8214 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/commits.py
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/custom_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/deploy_keys.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/deploy_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/deployments.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/discussions.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/draft_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/environments.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/epics.py
+-rw-r--r--   0 root         (0) root         (0)     7067 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/events.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/export_import.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/features.py
+-rw-r--r--   0 root         (0) root         (0)    10283 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/files.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/geo_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/group_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)    15672 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/groups.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     9205 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/integrations.py
+-rw-r--r--   0 root         (0) root         (0)     2734 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/invitations.py
+-rw-r--r--   0 root         (0) root         (0)    10162 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/issues.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/iterations.py
+-rw-r--r--   0 root         (0) root         (0)     2622 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/job_token_scope.py
+-rw-r--r--   0 root         (0) root         (0)     9139 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/jobs.py
+-rw-r--r--   0 root         (0) root         (0)      882 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/keys.py
+-rw-r--r--   0 root         (0) root         (0)     4736 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/labels.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/ldap.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/members.py
+-rw-r--r--   0 root         (0) root         (0)     6146 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/merge_request_approvals.py
+-rw-r--r--   0 root         (0) root         (0)    17306 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/merge_requests.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/merge_trains.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/milestones.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/namespaces.py
+-rw-r--r--   0 root         (0) root         (0)     8588 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/notes.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/notification_settings.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/packages.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/pages.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/personal_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/project_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)    44127 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/projects.py
+-rw-r--r--   0 root         (0) root         (0)     3041 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/push_rules.py
+-rw-r--r--   0 root         (0) root         (0)     1972 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/releases.py
+-rw-r--r--   0 root         (0) root         (0)    11048 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/repositories.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/resource_groups.py
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/reviewers.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/runners.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/secure_files.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/settings.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/sidekiq.py
+-rw-r--r--   0 root         (0) root         (0)     6018 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/snippets.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/statistics.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/templates.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/todos.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/topics.py
+-rw-r--r--   0 root         (0) root         (0)      824 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/triggers.py
+-rw-r--r--   0 root         (0) root         (0)    21281 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/users.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/variables.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/gitlab/v4/objects/wikis.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.678675 python_gitlab-4.5.0/python_gitlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8223 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10674 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-13 22:19:49.000000 python_gitlab-4.5.0/python_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-docker.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-docs.txt
+-rw-r--r--   0 root         (0) root         (0)      255 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-lint.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-precommit.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements-test.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 22:19:49.682675 python_gitlab-4.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.654675 python_gitlab-4.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.654675 python_gitlab-4.5.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.658675 python_gitlab-4.5.0/tests/functional/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_boards.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_branches.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_bulk_imports.py
+-rw-r--r--   0 root         (0) root         (0)      927 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_current_user.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_deploy_keys.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_deploy_tokens.py
+-rw-r--r--   0 root         (0) root         (0)      743 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_epics.py
+-rw-r--r--   0 root         (0) root         (0)     7787 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     9601 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_groups.py
+-rw-r--r--   0 root         (0) root         (0)     3683 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_import_export.py
+-rw-r--r--   0 root         (0) root         (0)     3464 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_issues.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_keys.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_lazy_objects.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_merge_requests.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_packages.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_project_job_token_scope.py
+-rw-r--r--   0 root         (0) root         (0)    10796 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_projects.py
+-rw-r--r--   0 root         (0) root         (0)      710 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_push_rules.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_releases.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_repository.py
+-rw-r--r--   0 root         (0) root         (0)      944 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_services.py
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_snippets.py
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_statistics.py
+-rw-r--r--   0 root         (0) root         (0)      971 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_topics.py
+-rw-r--r--   0 root         (0) root         (0)     5007 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_users.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_variables.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/api/test_wikis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.662675 python_gitlab-4.5.0/tests/functional/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     7371 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_packages.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_projects.py
+-rw-r--r--   0 root         (0) root         (0)     3791 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_resource_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_users.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_v4.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/cli/test_cli_variables.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/conftest.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/ee-test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.662675 python_gitlab-4.5.0/tests/functional/fixtures/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/.env
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      592 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/avatar.png
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/create_license.rb
+-rw-r--r--   0 root         (0) root         (0)     1717 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/docker.py
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/invalid_auth.cfg
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/invalid_version.cfg
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/fixtures/set_token.rb
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/functional/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.662675 python_gitlab-4.5.0/tests/install/
+-rw-r--r--   0 root         (0) root         (0)      125 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/install/test_install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.662675 python_gitlab-4.5.0/tests/smoke/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/smoke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/smoke/test_dists.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/_backends/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/_backends/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/_backends/test_requests_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/base/
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/base/test_rest_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10861 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/base/test_rest_object.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/meta/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4353 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/meta/test_ensure_type_hints.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/meta/test_imports.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/meta/test_mro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.666675 python_gitlab-4.5.0/tests/unit/mixins/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/mixins/test_meta_mixins.py
+-rw-r--r--   0 root         (0) root         (0)    16409 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/mixins/test_mixin_methods.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/mixins/test_object_mixins_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 22:19:49.678675 python_gitlab-4.5.0/tests/unit/objects/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_appearance.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_applications.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_audit_events.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_badges.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_bridges.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_bulk_imports.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_ci_lint.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_commits.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_deploy_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_deployments.py
+-rw-r--r--   0 root         (0) root         (0)     5089 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_draft_notes.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_environments.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_group_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)    14054 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_groups.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_hooks.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_invitations.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_issues.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_iterations.py
+-rw-r--r--   0 root         (0) root         (0)     1226 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_job_artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     6210 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_job_token_scope.py
+-rw-r--r--   0 root         (0) root         (0)     5248 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_jobs.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_keys.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_members.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_merge_request_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_merge_requests.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_merge_trains.py
+-rw-r--r--   0 root         (0) root         (0)    12878 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_packages.py
+-rw-r--r--   0 root         (0) root         (0)     4464 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_personal_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_pipeline_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_project_access_tokens.py
+-rw-r--r--   0 root         (0) root         (0)     6454 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_project_import_export.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_project_merge_request_approvals.py
+-rw-r--r--   0 root         (0) root         (0)      824 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_project_statistics.py
+-rw-r--r--   0 root         (0) root         (0)    21091 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_projects.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_registry_repositories.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_releases.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_remote_mirrors.py
+-rw-r--r--   0 root         (0) root         (0)     1383 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_repositories.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_groups.py
+-rw-r--r--   0 root         (0) root         (0)     1717 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_iteration_events.py
+-rw-r--r--   0 root         (0) root         (0)     3424 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_label_events.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_milestone_events.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_resource_state_events.py
+-rw-r--r--   0 root         (0) root         (0)     8133 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_runners.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_secure_files.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_services.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_snippets.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_submodules.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_todos.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_topics.py
+-rw-r--r--   0 root         (0) root         (0)     8577 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_users.py
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/objects/test_variables.py
+-rw-r--r--   0 root         (0) root         (0)     7536 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      800 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12171 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)     7347 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_gitlab_auth.py
+-rw-r--r--   0 root         (0) root         (0)    25196 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_gitlab_http_methods.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_types.py
+-rw-r--r--   0 root         (0) root         (0)     6441 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tests/unit/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2024-05-13 22:19:22.000000 python_gitlab-4.5.0/tox.ini
```

### Comparing `python-gitlab-4.4.0/AUTHORS` & `python_gitlab-4.5.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/CHANGELOG.md` & `python_gitlab-4.5.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,297 @@
 # CHANGELOG
 
 
 
+## v4.5.0 (2024-05-13)
+
+### Build
+
+* build: Add &#34;--no-cache-dir&#34; to pip commands in Dockerfile
+
+This would not leave cache files in the built docker image.
+
+Additionally, also only build the wheel in the build phase.
+
+On my machine, before this PR, size is 74845395; after this PR, size is
+72617713. ([`4ef94c8`](https://github.com/python-gitlab/python-gitlab/commit/4ef94c8260e958873bb626e86d3241daa22f7ce6))
+
+### Chore
+
+* chore(deps): update all non-major dependencies ([`4f338ae`](https://github.com/python-gitlab/python-gitlab/commit/4f338aed9c583a20ff5944e6ccbba5737c18b0f4))
+
+* chore(deps): update gitlab/gitlab-ee docker tag to v16.11.2-ee.0 ([`9be48f0`](https://github.com/python-gitlab/python-gitlab/commit/9be48f0bcc2d32b5e8489f62f963389d5d54b2f2))
+
+* chore(deps): update dependency myst-parser to v3 ([`9289189`](https://github.com/python-gitlab/python-gitlab/commit/92891890eb4730bc240213a212d392bcb869b800))
+
+* chore(deps): update all non-major dependencies ([`65d0e65`](https://github.com/python-gitlab/python-gitlab/commit/65d0e6520dcbcf5a708a87960c65fdcaf7e44bf3))
+
+* chore(deps): update dependency jinja2 to v3.1.4 [security] ([`8ea10c3`](https://github.com/python-gitlab/python-gitlab/commit/8ea10c360175453c721ad8e27386e642c2b68d88))
+
+* chore(deps): update all non-major dependencies ([`1f0343c`](https://github.com/python-gitlab/python-gitlab/commit/1f0343c1154ca8ae5b1f61de1db2343a2ad652ec))
+
+* chore(deps): update gitlab/gitlab-ee docker tag to v16.11.1-ee.0 ([`1ed8d6c`](https://github.com/python-gitlab/python-gitlab/commit/1ed8d6c21d3463b2ad09eb553871042e98090ffd))
+
+* chore(deps): update all non-major dependencies ([`0e9f4da`](https://github.com/python-gitlab/python-gitlab/commit/0e9f4da30cea507fcf83746008d9de2ee5a3bb9d))
+
+* chore(deps): update gitlab/gitlab-ee docker tag to v16 ([`ea8c4c2`](https://github.com/python-gitlab/python-gitlab/commit/ea8c4c2bc9f17f510415a697e0fb19cabff4135e))
+
+* chore(deps): update all non-major dependencies ([`d5b5fb0`](https://github.com/python-gitlab/python-gitlab/commit/d5b5fb00d8947ed9733cbb5a273e2866aecf33bf))
+
+* chore(deps): update dependency pytest-cov to v5 ([`db32000`](https://github.com/python-gitlab/python-gitlab/commit/db3200089ea83588ea7ad8bd5a7175d81f580630))
+
+* chore: update `mypy` to 1.9.0 and resolve one issue
+
+mypy 1.9.0 flagged one issue in the code. Resolve the issue. Current
+unit tests already check that a `None` value returns `text/plain`. So
+function is still working as expected. ([`dd00bfc`](https://github.com/python-gitlab/python-gitlab/commit/dd00bfc9c832aba0ed377573fe2e9120b296548d))
+
+* chore(deps): update dependency black to v24.3.0 [security] ([`f6e8692`](https://github.com/python-gitlab/python-gitlab/commit/f6e8692cfc84b5af2eb6deec4ae1c4935b42e91c))
+
+* chore(deps): update all non-major dependencies ([`14a3ffe`](https://github.com/python-gitlab/python-gitlab/commit/14a3ffe4cc161be51a39c204350b5cd45c602335))
+
+* chore(deps): update all non-major dependencies ([`3c4dcca`](https://github.com/python-gitlab/python-gitlab/commit/3c4dccaf51695334a5057b85d5ff4045739d1ad1))
+
+* chore(deps): update all non-major dependencies ([`04c569a`](https://github.com/python-gitlab/python-gitlab/commit/04c569a2130d053e35c1f2520ef8bab09f2f9651))
+
+* chore: add tox `labels` to enable running groups of environments
+
+tox now has a feature of `labels` which allows running groups of
+environments using the command `tox -m LABEL_NAME`. For example
+`tox -m lint` which has been setup to run the linters.
+
+Bumped the minimum required version of tox to be 4.0, which was
+released over a year ago. ([`d7235c7`](https://github.com/python-gitlab/python-gitlab/commit/d7235c74f8605f4abfb11eb257246864c7dcf709))
+
+* chore: add py312 &amp; py313 to tox environment list
+
+Even though there isn&#39;t a Python 3.13 at this time, this is done for
+the future.  tox is already configured to just warn about missing
+Python versions, but not fail if they don&#39;t exist. ([`679ddc7`](https://github.com/python-gitlab/python-gitlab/commit/679ddc7587d2add676fd2398cb9673bd1ca272e3))
+
+* chore(deps): update python-semantic-release/python-semantic-release action to v9 ([`e11d889`](https://github.com/python-gitlab/python-gitlab/commit/e11d889cd19ec1555b2bbee15355a8cdfad61d5f))
+
+* chore(deps): update all non-major dependencies ([`3c4b27e`](https://github.com/python-gitlab/python-gitlab/commit/3c4b27e64f4b51746b866f240a1291c2637355cc))
+
+* chore(deps): update dependency furo to v2024 ([`f6fd02d`](https://github.com/python-gitlab/python-gitlab/commit/f6fd02d956529e2c4bce261fe7b3da1442aaea12))
+
+* chore(deps): update dependency pytest to v8 ([`253babb`](https://github.com/python-gitlab/python-gitlab/commit/253babb9a7f8a7d469440fcfe1b2741ddcd8475e))
+
+* chore(deps): update dependency pytest-docker to v3 ([`35d2aec`](https://github.com/python-gitlab/python-gitlab/commit/35d2aec04532919d6dd7b7090bc4d5209eddd10d))
+
+* chore: update version of `black` for `pre-commit`
+
+The version of `black` needs to be updated to be in sync with what is
+in `requirements-lint.txt` ([`3501716`](https://github.com/python-gitlab/python-gitlab/commit/35017167a80809a49351f9e95916fafe61c7bfd5))
+
+* chore(deps): update all non-major dependencies ([`7dc2fa6`](https://github.com/python-gitlab/python-gitlab/commit/7dc2fa6e632ed2c9adeb6ed32c4899ec155f6622))
+
+* chore(deps): update codecov/codecov-action action to v4 ([`d2be1f7`](https://github.com/python-gitlab/python-gitlab/commit/d2be1f7608acadcc2682afd82d16d3706b7f7461))
+
+* chore: adapt style for black v24 ([`4e68d32`](https://github.com/python-gitlab/python-gitlab/commit/4e68d32c77ed587ab42d229d9f44c3bc40d1d0e5))
+
+* chore(deps): update dependency black to v24 ([`f59aee3`](https://github.com/python-gitlab/python-gitlab/commit/f59aee3ddcfaeeb29fcfab4cc6768dff6b5558cb))
+
+* chore(deps): update all non-major dependencies ([`48726fd`](https://github.com/python-gitlab/python-gitlab/commit/48726fde9b3c2424310ff590b366b9fdefa4a146))
+
+### Documentation
+
+* docs: add FAQ about conflicting parameters
+
+We have received multiple issues lately about this. Add it to the FAQ. ([`683ce72`](https://github.com/python-gitlab/python-gitlab/commit/683ce723352cc09e1a4b65db28be981ae6bb9f71))
+
+* docs(README): tweak GitLab CI usage docs ([`d9aaa99`](https://github.com/python-gitlab/python-gitlab/commit/d9aaa994568ad4896a1e8a0533ef0d1d2ba06bfa))
+
+* docs: how to run smoke tests
+
+Signed-off-by: Tim Knight &lt;tim.knight1@engineering.digital.dwp.gov.uk&gt; ([`2d1f487`](https://github.com/python-gitlab/python-gitlab/commit/2d1f4872390df10174f865f7a935bc73f7865fec))
+
+* docs(objects): minor rst formatting typo
+
+To correctly format a code block have to use `::` ([`57dfd17`](https://github.com/python-gitlab/python-gitlab/commit/57dfd1769b4e22b43dc0936aa3600cd7e78ba289))
+
+* docs: correct rotate token example
+
+Rotate token returns a dict. Change example to print the entire dict.
+
+Closes: #2836 ([`c53e695`](https://github.com/python-gitlab/python-gitlab/commit/c53e6954f097ed10d52b40660d2fba73c2e0e300))
+
+* docs: Note how to use the Docker image from within GitLab CI
+
+Ref: #2823 ([`6d4bffb`](https://github.com/python-gitlab/python-gitlab/commit/6d4bffb5aaa676d32fc892ef1ac002973bc040cb))
+
+* docs(artifacts): Fix argument indentation ([`c631eeb`](https://github.com/python-gitlab/python-gitlab/commit/c631eeb55556920f5975b1fa2b1a0354478ce3c0))
+
+### Feature
+
+* feat(job_token_scope): support Groups in job token allowlist API  (#2816)
+
+* feat(job_token_scope): support job token access allowlist API
+
+Signed-off-by: Tim Knight &lt;tim.knight1@engineering.digital.dwp.gov.uk&gt;
+l.dwp.gov.uk&gt;
+Co-authored-by: Nejc Habjan &lt;nejc.habjan@siemens.com&gt; ([`2d1b749`](https://github.com/python-gitlab/python-gitlab/commit/2d1b7499a93db2c9600b383e166f7463a5f22085))
+
+* feat(cli): allow skipping initial auth calls ([`001e596`](https://github.com/python-gitlab/python-gitlab/commit/001e59675f4a417a869f813d79c298a14268b87d))
+
+* feat(api): allow updating protected branches (#2771)
+
+* feat(api): allow updating protected branches
+
+Closes #2390 ([`a867c48`](https://github.com/python-gitlab/python-gitlab/commit/a867c48baa6f10ffbfb785e624a6e3888a859571))
+
+### Fix
+
+* fix: Consider `scope` an ArrayAttribute in PipelineJobManager
+
+List query params like &#39;scope&#39; were not being handled correctly for
+pipeline/jobs endpoint.
+This change ensures multiple values are appended with &#39;[]&#39;, resulting in
+the correct URL structure.
+
+Signed-off-by: Guilherme Gallo &lt;guilherme.gallo@collabora.com&gt;
+
+---
+
+Background:
+If one queries for pipeline jobs with `scope=[&#34;failed&#34;, &#34;success&#34;]`
+
+One gets:
+GET /api/v4/projects/176/pipelines/1113028/jobs?scope=success&amp;scope=failed
+
+But it is supposed to get:
+GET /api/v4/projects/176/pipelines/1113028/jobs?scope[]=success&amp;scope[]=failed
+
+The current version only considers the last element of the list argument.
+
+Signed-off-by: Guilherme Gallo &lt;guilherme.gallo@collabora.com&gt; ([`c5d0404`](https://github.com/python-gitlab/python-gitlab/commit/c5d0404ac9edfbfd328e7b4f07f554366377df3f))
+
+* fix(test): use different ids for merge request, approval rule, project
+
+The original bug was that the merge request identifier was used instead of the
+approval rule identifier. The test didn&#39;t notice that because it used `1` for
+all identifiers. Make these identifiers different so that a mixup will become
+apparent. ([`c23e6bd`](https://github.com/python-gitlab/python-gitlab/commit/c23e6bd5785205f0f4b4c80321153658fc23fb98))
+
+* fix(api): fix saving merge request approval rules
+
+Closes #2548 ([`b8b3849`](https://github.com/python-gitlab/python-gitlab/commit/b8b3849b2d4d3f2d9e81e5cf4f6b53368f7f0127))
+
+* fix: user.warn() to show correct filename of issue
+
+Previously would only go to the 2nd level of the stack for determining
+the offending filename and line number. When it should be showing the
+first filename outside of the python-gitlab source code. As we want it
+to show the warning for the user of the libraries code.
+
+Update test to show it works as expected. ([`529f1fa`](https://github.com/python-gitlab/python-gitlab/commit/529f1faacee46a88cb0a542306309eb835516796))
+
+* fix(api): update manual job status when playing it ([`9440a32`](https://github.com/python-gitlab/python-gitlab/commit/9440a3255018d6a6e49269caf4c878d80db508a8))
+
+* fix(cli): allow exclusive arguments as optional (#2770)
+
+* fix(cli): allow exclusive arguments as optional
+
+The CLI takes its arguments from the RequiredOptional, which has three fields: required, optional, and exclusive. In practice, the exclusive options are not defined as either required or optional, and would not be allowed in the CLI. This changes that, so that exclusive options are also added to the argument parser.
+
+  * fix(cli): inform argument parser that options are mutually exclusive
+
+  * fix(cli): use correct exclusive options, add unit test
+
+Closes #2769 ([`7ec3189`](https://github.com/python-gitlab/python-gitlab/commit/7ec3189d6eacdb55925e8be886a44d7ee09eb9ca))
+
+### Test
+
+* test: remove approve step
+
+Signed-off-by: Tim Knight &lt;tim.knight1@engineering.digital.dwp.gov.uk&gt; ([`48a6705`](https://github.com/python-gitlab/python-gitlab/commit/48a6705558c5ab6fb08c62a18de350a5985099f8))
+
+* test: tidy up functional tests
+
+Signed-off-by: Tim Knight &lt;tim.knight1@engineering.digital.dwp.gov.uk&gt; ([`06266ea`](https://github.com/python-gitlab/python-gitlab/commit/06266ea5966c601c035ad8ce5840729e5f9baa57))
+
+* test: update api tests for GL 16.10
+
+- Make sure we&#39;re testing python-gitlab functionality,
+make sure we&#39;re not awaiting on Gitlab Async functions
+- Decouple and improve test stability
+
+Signed-off-by: Tim Knight &lt;tim.knight1@engineering.digital.dwp.gov.uk&gt; ([`4bef473`](https://github.com/python-gitlab/python-gitlab/commit/4bef47301342703f87c1ce1d2920d54f9927a66a))
+
+* test(functional): enable bulk import feature flag before test ([`b81da2e`](https://github.com/python-gitlab/python-gitlab/commit/b81da2e66ce385525730c089dbc2a5a85ba23287))
+
+* test: don&#39;t use weak passwords
+
+Newer versions of GitLab will refuse to create a user with a weak
+password. In order for us to move to a newer GitLab version in testing
+use a stronger password for the tests that create a user. ([`c64d126`](https://github.com/python-gitlab/python-gitlab/commit/c64d126142cc77eae4297b8deec27bb1d68b7a13))
+
+* test: update tests for gitlab 16.8 functionality
+
+- use programmatic dates for expires_at in tokens tests
+- set PAT for 16.8 into tests
+
+Signed-off-by: Tim Knight &lt;tim.knight1@engineering.digital.dwp.gov.uk&gt; ([`f8283ae`](https://github.com/python-gitlab/python-gitlab/commit/f8283ae69efd86448ae60d79dd8321af3f19ba1b))
+
+* test(smoke): normalize all dist titles for smoke tests ([`ee013fe`](https://github.com/python-gitlab/python-gitlab/commit/ee013fe1579b001b4b30bae33404e827c7bdf8c1))
+
+
+## v4.4.0 (2024-01-15)
+
+### Chore
+
+* chore(deps): update all non-major dependencies ([`550f935`](https://github.com/python-gitlab/python-gitlab/commit/550f9355d29a502bb022f68dab6c902bf6913552))
+
+* chore(deps): update pre-commit hook pycqa/flake8 to v7 ([`9a199b6`](https://github.com/python-gitlab/python-gitlab/commit/9a199b6089152e181e71a393925e0ec581bc55ca))
+
+* chore(deps): update dependency jinja2 to v3.1.3 [security] ([`880913b`](https://github.com/python-gitlab/python-gitlab/commit/880913b67cce711d96e89ce6813e305e4ba10908))
+
+* chore(deps): update dependency flake8 to v7 ([`20243c5`](https://github.com/python-gitlab/python-gitlab/commit/20243c532a8a6d28eee0caff5b9c30cc7376a162))
+
+* chore(deps): update all non-major dependencies ([`cbc13a6`](https://github.com/python-gitlab/python-gitlab/commit/cbc13a61e0f15880b49a3d0208cc603d7d0b57e3))
+
+* chore(ci): align upload and download action versions ([`dcca59d`](https://github.com/python-gitlab/python-gitlab/commit/dcca59d1a5966283c1120cfb639c01a76214d2b2))
+
+* chore(deps): update actions/upload-artifact action to v4 ([`7114af3`](https://github.com/python-gitlab/python-gitlab/commit/7114af341dd12b7fb63ffc08650c455ead18ab70))
+
+* chore(ci): add Python 3.13 development CI job
+
+Add a job to test the development versions of Python 3.13. ([`ff0c11b`](https://github.com/python-gitlab/python-gitlab/commit/ff0c11b7b75677edd85f846a4dbdab08491a6bd7))
+
+* chore(deps): update all non-major dependencies ([`369a595`](https://github.com/python-gitlab/python-gitlab/commit/369a595a8763109a2af8a95a8e2423ebb30b9320))
+
+### Feature
+
+* feat(api): add reviewer_details manager for mergrequest to get reviewers of merge request
+
+Those changes implements &#39;GET /projects/:id/merge_requests/:merge_request_iid/reviewers&#39; gitlab API call.
+Naming for call is not reviewers because reviewers atribute already presen in merge request response ([`adbd90c`](https://github.com/python-gitlab/python-gitlab/commit/adbd90cadffe1d9e9716a6e3826f30664866ad3f))
+
+* feat(api): support access token rotate API ([`b13971d`](https://github.com/python-gitlab/python-gitlab/commit/b13971d5472cb228f9e6a8f2fa05a7cc94d03ebe))
+
+* feat(api): support single resource access token get API ([`dae9e52`](https://github.com/python-gitlab/python-gitlab/commit/dae9e522a26041f5b3c6461cc8a5e284f3376a79))
+
+### Fix
+
+* fix(cli): support binary files with `@` notation
+
+Support binary files being used in the CLI with arguments using the
+`@` notation. For example `--avatar @/path/to/avatar.png`
+
+Also explicitly catch the common OSError exception, which is the
+parent exception for things like: FileNotFoundError, PermissionError
+and more exceptions.
+
+Remove the bare exception handling. We would rather have the full
+traceback of any exceptions that we don&#39;t know about and add them
+later if needed.
+
+Closes: #2752 ([`57749d4`](https://github.com/python-gitlab/python-gitlab/commit/57749d46de1d975aacb82758c268fc26e5e6ed8b))
+
+
 ## v4.3.0 (2023-12-28)
 
 ### Chore
 
 * chore(deps): update all non-major dependencies ([`d7bdb02`](https://github.com/python-gitlab/python-gitlab/commit/d7bdb0257a5587455c3722f65c4a632f24d395be))
 
 * chore(deps): update actions/stale action to v9 ([`c01988b`](https://github.com/python-gitlab/python-gitlab/commit/c01988b12c7745929d0c591f2fa265df2929a859))
```

### Comparing `python-gitlab-4.4.0/COPYING` & `python_gitlab-4.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/PKG-INFO` & `python_gitlab-4.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gitlab
-Version: 4.4.0
+Version: 4.5.0
 Summary: A python wrapper for the GitLab API
 Author-email: Gauvain Pocentek <gauvain@pocentek.net>
 Maintainer-email: John Villalovos <john@sodarock.com>, Max Wittig <max.wittig@siemens.com>, Nejc Habjan <nejc.habjan@siemens.com>, Roger Meier <r.meier@siemens.com>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/python-gitlab/python-gitlab
 Project-URL: Changelog, https://github.com/python-gitlab/python-gitlab/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://python-gitlab.readthedocs.io
@@ -145,14 +145,31 @@
 
 You can also mount your own config file:
 
 .. code-block:: console
 
    $ docker run -it --rm -v /path/to/python-gitlab.cfg:/etc/python-gitlab.cfg registry.gitlab.com/python-gitlab/python-gitlab:latest <command> ...
 
+Usage inside GitLab CI
+~~~~~~~~~~~~~~~~~~~~~~
+
+If you want to use the Docker image directly inside your GitLab CI as an ``image``, you will need to override
+the ``entrypoint``, `as noted in the official GitLab documentation <https://docs.gitlab.com/ee/ci/docker/using_docker_images.html#override-the-entrypoint-of-an-image>`__:
+
+.. code-block:: yaml
+
+   Job Name:
+      image:
+         name: registry.gitlab.com/python-gitlab/python-gitlab:latest
+         entrypoint: [""]
+      before_script:
+         gitlab --version
+      script:
+         gitlab <command>
+
 Building the image
 ~~~~~~~~~~~~~~~~~~
 
 To build your own image from this repository, run:
 
 .. code-block:: console
```

### Comparing `python-gitlab-4.4.0/README.rst` & `python_gitlab-4.5.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -108,14 +108,31 @@
 
 You can also mount your own config file:
 
 .. code-block:: console
 
    $ docker run -it --rm -v /path/to/python-gitlab.cfg:/etc/python-gitlab.cfg registry.gitlab.com/python-gitlab/python-gitlab:latest <command> ...
 
+Usage inside GitLab CI
+~~~~~~~~~~~~~~~~~~~~~~
+
+If you want to use the Docker image directly inside your GitLab CI as an ``image``, you will need to override
+the ``entrypoint``, `as noted in the official GitLab documentation <https://docs.gitlab.com/ee/ci/docker/using_docker_images.html#override-the-entrypoint-of-an-image>`__:
+
+.. code-block:: yaml
+
+   Job Name:
+      image:
+         name: registry.gitlab.com/python-gitlab/python-gitlab:latest
+         entrypoint: [""]
+      before_script:
+         gitlab --version
+      script:
+         gitlab <command>
+
 Building the image
 ~~~~~~~~~~~~~~~~~~
 
 To build your own image from this repository, run:
 
 .. code-block:: console
```

### Comparing `python-gitlab-4.4.0/docs/Makefile` & `python_gitlab-4.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/api/gitlab.rst` & `python_gitlab-4.5.0/docs/api/gitlab.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/api-levels.rst` & `python_gitlab-4.5.0/docs/api-levels.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/api-objects.rst` & `python_gitlab-4.5.0/docs/api-objects.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/api-usage-advanced.rst` & `python_gitlab-4.5.0/docs/api-usage-advanced.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/api-usage.rst` & `python_gitlab-4.5.0/docs/api-usage.rst`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,19 @@
 
 .. code-block:: python
 
    >>> gl.projects.list(sort='invalid value')
    ...
    GitlabListError: 400: sort does not have a valid value
 
+.. _conflicting_parameters:
+
+Conflicting Parameters
+======================
+
 You can use the ``query_parameters`` argument to send arguments that would
 conflict with python or python-gitlab when using them as kwargs:
 
 .. code-block:: python
 
    gl.user_activities.list(from='2019-01-01', iterator=True)  ## invalid
```

### Comparing `python-gitlab-4.4.0/docs/cli-examples.rst` & `python_gitlab-4.5.0/docs/cli-examples.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 .. seealso::
 
       For a complete list of objects and actions available, see :doc:`/cli-objects`.
 
 CI Lint
 -------
 
+**ci-lint has been Removed in Gitlab 16, use project-ci-lint instead**
+
 Lint a CI YAML configuration from a string:
 
-.. note:: 
+.. note::
 
    To see output, you will need to use the ``-v``/``--verbose`` flag.
 
    To exit with non-zero on YAML lint failures instead, use the ``validate``
    subcommand shown below.
 
 .. code-block:: console
@@ -35,14 +37,17 @@
 
 Validate a CI YAML configuration from a file (lints and exits with non-zero on failure):
 
 .. code-block:: console
 
    $ gitlab ci-lint validate --content @.gitlab-ci.yml
 
+Project CI Lint
+---------------
+
 Lint a project's CI YAML configuration:
 
 .. code-block:: console
 
    $ gitlab --verbose project-ci-lint create --project-id group/my-project --content @.gitlab-ci.yml
 
 Validate a project's CI YAML configuration (lints and exits with non-zero on failure):
```

### Comparing `python-gitlab-4.4.0/docs/cli-objects.rst` & `python_gitlab-4.5.0/docs/cli-objects.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/cli-usage.rst` & `python_gitlab-4.5.0/docs/cli-usage.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/conf.py` & `python_gitlab-4.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/ext/docstrings.py` & `python_gitlab-4.5.0/docs/ext/docstrings.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/ext/manager_tmpl.j2` & `python_gitlab-4.5.0/docs/ext/manager_tmpl.j2`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/access_requests.rst` & `python_gitlab-4.5.0/docs/gl_objects/access_requests.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/applications.rst` & `python_gitlab-4.5.0/docs/gl_objects/applications.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/badges.rst` & `python_gitlab-4.5.0/docs/gl_objects/badges.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/boards.rst` & `python_gitlab-4.5.0/docs/gl_objects/boards.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/branches.rst` & `python_gitlab-4.5.0/docs/gl_objects/branches.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/bulk_imports.rst` & `python_gitlab-4.5.0/docs/gl_objects/bulk_imports.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/ci_lint.rst` & `python_gitlab-4.5.0/docs/gl_objects/ci_lint.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/clusters.rst` & `python_gitlab-4.5.0/docs/gl_objects/clusters.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/commits.rst` & `python_gitlab-4.5.0/docs/gl_objects/commits.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/deploy_keys.rst` & `python_gitlab-4.5.0/docs/gl_objects/deploy_keys.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/deploy_tokens.rst` & `python_gitlab-4.5.0/docs/gl_objects/deploy_tokens.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/deployments.rst` & `python_gitlab-4.5.0/docs/gl_objects/deployments.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/discussions.rst` & `python_gitlab-4.5.0/docs/gl_objects/discussions.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/draft_notes.rst` & `python_gitlab-4.5.0/docs/gl_objects/draft_notes.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/emojis.rst` & `python_gitlab-4.5.0/docs/gl_objects/emojis.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/environments.rst` & `python_gitlab-4.5.0/docs/gl_objects/environments.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/epics.rst` & `python_gitlab-4.5.0/docs/gl_objects/epics.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/events.rst` & `python_gitlab-4.5.0/docs/gl_objects/events.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/features.rst` & `python_gitlab-4.5.0/docs/gl_objects/features.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/geo_nodes.rst` & `python_gitlab-4.5.0/docs/gl_objects/geo_nodes.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/group_access_tokens.rst` & `python_gitlab-4.5.0/docs/gl_objects/group_access_tokens.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/groups.rst` & `python_gitlab-4.5.0/docs/gl_objects/groups.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/invitations.rst` & `python_gitlab-4.5.0/docs/gl_objects/invitations.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/issues.rst` & `python_gitlab-4.5.0/docs/gl_objects/issues.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/iterations.rst` & `python_gitlab-4.5.0/docs/gl_objects/iterations.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/labels.rst` & `python_gitlab-4.5.0/docs/gl_objects/labels.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/merge_request_approvals.rst` & `python_gitlab-4.5.0/docs/gl_objects/merge_request_approvals.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/merge_requests.rst` & `python_gitlab-4.5.0/docs/gl_objects/merge_requests.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/merge_trains.rst` & `python_gitlab-4.5.0/docs/gl_objects/merge_trains.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/messages.rst` & `python_gitlab-4.5.0/docs/gl_objects/messages.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/milestones.rst` & `python_gitlab-4.5.0/docs/gl_objects/milestones.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/namespaces.rst` & `python_gitlab-4.5.0/docs/gl_objects/namespaces.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/notes.rst` & `python_gitlab-4.5.0/docs/gl_objects/notes.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/notifications.rst` & `python_gitlab-4.5.0/docs/gl_objects/notifications.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/packages.rst` & `python_gitlab-4.5.0/docs/gl_objects/packages.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/pagesdomains.rst` & `python_gitlab-4.5.0/docs/gl_objects/pagesdomains.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/personal_access_tokens.rst` & `python_gitlab-4.5.0/docs/gl_objects/personal_access_tokens.rst`

 * *Files 8% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
 Rotate a personal access token and retrieve its new value::
 
     token = gl.personal_access_tokens.get(42, lazy=True)
     token.rotate()
     print(token.token)
     # or directly using a token ID
-    new_token = gl.personal_access_tokens.rotate(42)
-    print(new_token.token)
+    new_token_dict = gl.personal_access_tokens.rotate(42)
+    print(new_token_dict)
 
 Create a personal access token for a user (admin only)::
 
     user = gl.users.get(25, lazy=True)
     access_token = user.personal_access_tokens.create({"name": "test", "scopes": "api"})
 
 .. note:: As you can see above, you can only create personal access tokens
```

### Comparing `python-gitlab-4.4.0/docs/gl_objects/pipelines_and_jobs.rst` & `python_gitlab-4.5.0/docs/gl_objects/pipelines_and_jobs.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/project_access_tokens.rst` & `python_gitlab-4.5.0/docs/gl_objects/project_access_tokens.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/projects.rst` & `python_gitlab-4.5.0/docs/gl_objects/projects.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/protected_branches.rst` & `python_gitlab-4.5.0/docs/gl_objects/protected_branches.rst`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 
     p_branches = project.protectedbranches.list()
 
 Get a single protected branch::
 
     p_branch = project.protectedbranches.get('main')
 
+Update a protected branch::
+
+    p_branch.allow_force_push = True
+    p_branch.save()
+
 Create a protected branch::
 
     p_branch = project.protectedbranches.create({
         'name': '*-stable',
         'merge_access_level': gitlab.const.AccessLevel.DEVELOPER,
         'push_access_level': gitlab.const.AccessLevel.MAINTAINER
     })
```

### Comparing `python-gitlab-4.4.0/docs/gl_objects/protected_environments.rst` & `python_gitlab-4.5.0/docs/gl_objects/protected_environments.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/releases.rst` & `python_gitlab-4.5.0/docs/gl_objects/releases.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/remote_mirrors.rst` & `python_gitlab-4.5.0/docs/gl_objects/remote_mirrors.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/repositories.rst` & `python_gitlab-4.5.0/docs/gl_objects/repositories.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/repository_tags.rst` & `python_gitlab-4.5.0/docs/gl_objects/repository_tags.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/resource_groups.rst` & `python_gitlab-4.5.0/docs/gl_objects/resource_groups.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/runners.rst` & `python_gitlab-4.5.0/docs/gl_objects/runners.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/search.rst` & `python_gitlab-4.5.0/docs/gl_objects/search.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/secure_files.rst` & `python_gitlab-4.5.0/docs/gl_objects/secure_files.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/snippets.rst` & `python_gitlab-4.5.0/docs/gl_objects/snippets.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/system_hooks.rst` & `python_gitlab-4.5.0/docs/gl_objects/system_hooks.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/templates.rst` & `python_gitlab-4.5.0/docs/gl_objects/templates.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/todos.rst` & `python_gitlab-4.5.0/docs/gl_objects/todos.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/topics.rst` & `python_gitlab-4.5.0/docs/gl_objects/topics.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/users.rst` & `python_gitlab-4.5.0/docs/gl_objects/users.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/variables.rst` & `python_gitlab-4.5.0/docs/gl_objects/variables.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/gl_objects/wikis.rst` & `python_gitlab-4.5.0/docs/gl_objects/wikis.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/make.bat` & `python_gitlab-4.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/docs/release-notes.rst` & `python_gitlab-4.5.0/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/__init__.py` & `python_gitlab-4.5.0/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/_backends/protocol.py` & `python_gitlab-4.5.0/gitlab/_backends/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     from typing import Protocol
 else:
     from typing_extensions import Protocol
 
 
 class BackendResponse(Protocol):
     @abc.abstractmethod
-    def __init__(self, response: requests.Response) -> None:
-        ...
+    def __init__(self, response: requests.Response) -> None: ...
 
 
 class Backend(Protocol):
     @abc.abstractmethod
     def http_request(
         self,
         method: str,
@@ -26,9 +25,8 @@
         json: Optional[Union[Dict[str, Any], bytes]],
         data: Optional[Union[Dict[str, Any], MultipartEncoder]],
         params: Optional[Any],
         timeout: Optional[float],
         verify: Optional[Union[bool, str]],
         stream: Optional[bool],
         **kwargs: Any,
-    ) -> BackendResponse:
-        ...
+    ) -> BackendResponse: ...
```

### Comparing `python-gitlab-4.4.0/gitlab/_backends/requests_backend.py` & `python_gitlab-4.5.0/gitlab/_backends/requests_backend.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/base.py` & `python_gitlab-4.5.0/gitlab/base.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/cli.py` & `python_gitlab-4.5.0/gitlab/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,14 +278,24 @@
         default=os.getenv("GITLAB_OAUTH_TOKEN"),
     )
     tokens.add_argument(
         "--job-token",
         help=("GitLab CI job token [env var: CI_JOB_TOKEN]"),
         required=False,
     )
+    parser.add_argument(
+        "--skip-login",
+        help=(
+            "Skip initial authenticated API call to the current user endpoint. "
+            "This may  be useful when invoking the CLI in scripts. "
+            "[env var: GITLAB_SKIP_LOGIN]"
+        ),
+        action="store_true",
+        default=os.getenv("GITLAB_SKIP_LOGIN"),
+    )
     return parser
 
 
 def _get_parser() -> argparse.ArgumentParser:
     # NOTE: We must delay import of gitlab.v4.cli until now or
     # otherwise it will cause circular import errors
     from gitlab.v4 import cli as v4_cli
@@ -364,14 +374,15 @@
     output = args.output
     fields = []
     if args.fields:
         fields = [x.strip() for x in args.fields.split(",")]
     debug = args.debug
     gitlab_resource = args.gitlab_resource
     resource_action = args.resource_action
+    skip_login = args.skip_login
 
     args_dict = vars(args)
     # Remove CLI behavior-related args
     for item in (
         "gitlab",
         "config_file",
         "verbose",
@@ -386,23 +397,24 @@
         "timeout",
         "api_version",
         "pagination",
         "user_agent",
         "private_token",
         "oauth_token",
         "job_token",
+        "skip_login",
     ):
         args_dict.pop(item)
     args_dict = {k: _parse_value(v) for k, v in args_dict.items() if v is not None}
 
     try:
         gl = gitlab.Gitlab.merge_config(vars(options), gitlab_id, config_files)
         if debug:
             gl.enable_debug()
-        if gl.private_token or gl.oauth_token:
+        if not skip_login and (gl.private_token or gl.oauth_token):
             gl.auth()
     except Exception as e:
         die(str(e))
 
     gitlab.v4.cli.run(
         gl, gitlab_resource, resource_action, args_dict, verbose, output, fields
     )
```

### Comparing `python-gitlab-4.4.0/gitlab/client.py` & `python_gitlab-4.5.0/gitlab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 _PAGINATION_URL = (
     f"https://python-gitlab.readthedocs.io/en/v{gitlab.__version__}/"
     f"api-usage.html#pagination"
 )
 
 
 class Gitlab:
-
     """Represents a GitLab server connection.
 
     Args:
         url: The URL of the GitLab server (defaults to https://gitlab.com).
         private_token: The user private token
         oauth_token: An oauth token
         job_token: A CI job token
```

### Comparing `python-gitlab-4.4.0/gitlab/config.py` & `python_gitlab-4.5.0/gitlab/config.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/const.py` & `python_gitlab-4.5.0/gitlab/const.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/exceptions.py` & `python_gitlab-4.5.0/gitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/mixins.py` & `python_gitlab-4.5.0/gitlab/mixins.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/types.py` & `python_gitlab-4.5.0/gitlab/types.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/utils.py` & `python_gitlab-4.5.0/gitlab/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 class _StdoutStream:
     def __call__(self, chunk: Any) -> None:
         print(chunk)
 
 
 def get_content_type(content_type: Optional[str]) -> str:
     message = email.message.Message()
-    message["content-type"] = content_type
+    if content_type is not None:
+        message["content-type"] = content_type
 
     return message.get_content_type()
 
 
 class MaskingFormatter(logging.Formatter):
     """A logging formatter that can mask credentials"""
 
@@ -187,16 +188,15 @@
     # Get `stacklevel` for user code so we indicate where issue is in
     # their code.
     pg_dir = pathlib.Path(__file__).parent.resolve()
     stack = traceback.extract_stack()
     stacklevel = 1
     warning_from = ""
     for stacklevel, frame in enumerate(reversed(stack), start=1):
-        if stacklevel == 2:
-            warning_from = f" (python-gitlab: {frame.filename}:{frame.lineno})"
+        warning_from = f" (python-gitlab: {frame.filename}:{frame.lineno})"
         frame_dir = str(pathlib.Path(frame.filename).parent.resolve())
         if not frame_dir.startswith(str(pg_dir)):
             break
     warnings.warn(
         message=message + warning_from,
         category=category,
         stacklevel=stacklevel,
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/cli.py` & `python_gitlab-4.5.0/gitlab/v4/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -258,14 +258,18 @@
                 sub_parser_action.add_argument(
                     f"--{x.replace('_', '-')}", required=True
                 )
             for x in mgr_cls._create_attrs.optional:
                 sub_parser_action.add_argument(
                     f"--{x.replace('_', '-')}", required=False
                 )
+            if mgr_cls._create_attrs.exclusive:
+                group = sub_parser_action.add_mutually_exclusive_group()
+                for x in mgr_cls._create_attrs.exclusive:
+                    group.add_argument(f"--{x.replace('_', '-')}")
 
         if action_name == "update":
             if cls._id_attr is not None:
                 id_attr = cls._id_attr.replace("_", "-")
                 sub_parser_action.add_argument(f"--{id_attr}", required=True)
 
             for x in mgr_cls._update_attrs.required:
@@ -276,14 +280,19 @@
 
             for x in mgr_cls._update_attrs.optional:
                 if x != cls._id_attr:
                     sub_parser_action.add_argument(
                         f"--{x.replace('_', '-')}", required=False
                     )
 
+            if mgr_cls._update_attrs.exclusive:
+                group = sub_parser_action.add_mutually_exclusive_group()
+                for x in mgr_cls._update_attrs.exclusive:
+                    group.add_argument(f"--{x.replace('_', '-')}")
+
     if cls.__name__ in cli.custom_actions:
         name = cls.__name__
         for action_name in cli.custom_actions[name]:
             # NOTE(jlvillal): If we put a function for the `default` value of
             # the `get` it will always get called, which will break things.
             action_parser = action_parsers.get(action_name)
             if action_parser is None:
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/__init__.py` & `python_gitlab-4.5.0/gitlab/v4/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/access_requests.py` & `python_gitlab-4.5.0/gitlab/v4/objects/access_requests.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/appearance.py` & `python_gitlab-4.5.0/gitlab/v4/objects/appearance.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/applications.py` & `python_gitlab-4.5.0/gitlab/v4/objects/applications.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/artifacts.py` & `python_gitlab-4.5.0/gitlab/v4/objects/artifacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/job_artifacts.html
 """
+
 from typing import Any, Callable, Iterator, Optional, TYPE_CHECKING, Union
 
 import requests
 
 from gitlab import cli
 from gitlab import exceptions as exc
 from gitlab import utils
@@ -57,15 +58,15 @@
         iterator: bool = False,
         **kwargs: Any,
     ) -> Optional[Union[bytes, Iterator[Any]]]:
         """Get the job artifacts archive from a specific tag or branch.
 
         Args:
             ref_name: Branch or tag name in repository. HEAD or SHA references
-            are not supported.
+                are not supported.
             job: The name of the job.
             job_token: Job token for multi-project pipeline triggers.
             streamed: If True the data will be processed by chunks of
                 `chunk_size` and each chunk is passed to `action` for
                 treatment
             iterator: If True directly return the underlying response
                 iterator
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/audit_events.py` & `python_gitlab-4.5.0/gitlab/v4/objects/audit_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/audit_events.html
 """
+
 from typing import Any, cast, Union
 
 from gitlab.base import RESTManager, RESTObject
 from gitlab.mixins import RetrieveMixin
 
 __all__ = [
     "AuditEvent",
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/award_emojis.py` & `python_gitlab-4.5.0/gitlab/v4/objects/award_emojis.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/badges.py` & `python_gitlab-4.5.0/gitlab/v4/objects/badges.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/boards.py` & `python_gitlab-4.5.0/gitlab/v4/objects/boards.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/branches.py` & `python_gitlab-4.5.0/gitlab/v4/objects/branches.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from typing import Any, cast, Union
 
 from gitlab.base import RESTManager, RESTObject
-from gitlab.mixins import NoUpdateMixin, ObjectDeleteMixin
+from gitlab.mixins import (
+    CRUDMixin,
+    NoUpdateMixin,
+    ObjectDeleteMixin,
+    SaveMixin,
+    UpdateMethod,
+)
 from gitlab.types import RequiredOptional
 
 __all__ = [
     "ProjectBranch",
     "ProjectBranchManager",
     "ProjectProtectedBranch",
     "ProjectProtectedBranchManager",
@@ -24,19 +30,19 @@
 
     def get(
         self, id: Union[str, int], lazy: bool = False, **kwargs: Any
     ) -> ProjectBranch:
         return cast(ProjectBranch, super().get(id=id, lazy=lazy, **kwargs))
 
 
-class ProjectProtectedBranch(ObjectDeleteMixin, RESTObject):
+class ProjectProtectedBranch(SaveMixin, ObjectDeleteMixin, RESTObject):
     _id_attr = "name"
 
 
-class ProjectProtectedBranchManager(NoUpdateMixin, RESTManager):
+class ProjectProtectedBranchManager(CRUDMixin, RESTManager):
     _path = "/projects/{project_id}/protected_branches"
     _obj_cls = ProjectProtectedBranch
     _from_parent_attrs = {"project_id": "id"}
     _create_attrs = RequiredOptional(
         required=("name",),
         optional=(
             "push_access_level",
@@ -45,12 +51,13 @@
             "allow_force_push",
             "allowed_to_push",
             "allowed_to_merge",
             "allowed_to_unprotect",
             "code_owner_approval_required",
         ),
     )
+    _update_method = UpdateMethod.PATCH
 
     def get(
         self, id: Union[str, int], lazy: bool = False, **kwargs: Any
     ) -> ProjectProtectedBranch:
         return cast(ProjectProtectedBranch, super().get(id=id, lazy=lazy, **kwargs))
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/broadcast_messages.py` & `python_gitlab-4.5.0/gitlab/v4/objects/broadcast_messages.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/bulk_imports.py` & `python_gitlab-4.5.0/gitlab/v4/objects/bulk_imports.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/ci_lint.py` & `python_gitlab-4.5.0/gitlab/v4/objects/ci_lint.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/clusters.py` & `python_gitlab-4.5.0/gitlab/v4/objects/clusters.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/commits.py` & `python_gitlab-4.5.0/gitlab/v4/objects/commits.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/container_registry.py` & `python_gitlab-4.5.0/gitlab/v4/objects/container_registry.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/custom_attributes.py` & `python_gitlab-4.5.0/gitlab/v4/objects/custom_attributes.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/deploy_keys.py` & `python_gitlab-4.5.0/gitlab/v4/objects/deploy_keys.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/deploy_tokens.py` & `python_gitlab-4.5.0/gitlab/v4/objects/deploy_tokens.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/deployments.py` & `python_gitlab-4.5.0/gitlab/v4/objects/deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/deployments.html
 """
+
 from typing import Any, cast, Dict, Optional, TYPE_CHECKING, Union
 
 from gitlab import cli
 from gitlab import exceptions as exc
 from gitlab.base import RESTManager, RESTObject
 from gitlab.mixins import CreateMixin, RetrieveMixin, SaveMixin, UpdateMixin
 from gitlab.types import RequiredOptional
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/discussions.py` & `python_gitlab-4.5.0/gitlab/v4/objects/discussions.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/draft_notes.py` & `python_gitlab-4.5.0/gitlab/v4/objects/draft_notes.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/environments.py` & `python_gitlab-4.5.0/gitlab/v4/objects/environments.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/epics.py` & `python_gitlab-4.5.0/gitlab/v4/objects/epics.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/events.py` & `python_gitlab-4.5.0/gitlab/v4/objects/events.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/export_import.py` & `python_gitlab-4.5.0/gitlab/v4/objects/export_import.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/features.py` & `python_gitlab-4.5.0/gitlab/v4/objects/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/features.html
 """
+
 from typing import Any, Optional, TYPE_CHECKING, Union
 
 from gitlab import exceptions as exc
 from gitlab import utils
 from gitlab.base import RESTManager, RESTObject
 from gitlab.mixins import DeleteMixin, ListMixin, ObjectDeleteMixin
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/files.py` & `python_gitlab-4.5.0/gitlab/v4/objects/files.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/geo_nodes.py` & `python_gitlab-4.5.0/gitlab/v4/objects/geo_nodes.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/group_access_tokens.py` & `python_gitlab-4.5.0/gitlab/v4/objects/group_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/groups.py` & `python_gitlab-4.5.0/gitlab/v4/objects/groups.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/hooks.py` & `python_gitlab-4.5.0/gitlab/v4/objects/hooks.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/integrations.py` & `python_gitlab-4.5.0/gitlab/v4/objects/integrations.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/invitations.py` & `python_gitlab-4.5.0/gitlab/v4/objects/invitations.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/issues.py` & `python_gitlab-4.5.0/gitlab/v4/objects/issues.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/iterations.py` & `python_gitlab-4.5.0/gitlab/v4/objects/iterations.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/jobs.py` & `python_gitlab-4.5.0/gitlab/v4/objects/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,18 @@
             **kwargs: Extra options to send to the server (e.g. sudo)
 
         Raises:
             GitlabAuthenticationError: If authentication is not correct
             GitlabJobPlayError: If the job could not be triggered
         """
         path = f"{self.manager.path}/{self.encoded_id}/play"
-        self.manager.gitlab.http_post(path, **kwargs)
+        result = self.manager.gitlab.http_post(path, **kwargs)
+        if TYPE_CHECKING:
+            assert isinstance(result, dict)
+        self._update_attrs(result)
 
     @cli.register_custom_action("ProjectJob")
     @exc.on_http_error(exc.GitlabJobEraseError)
     def erase(self, **kwargs: Any) -> None:
         """Erase the job (remove job artifacts and trace).
 
         Args:
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/keys.py` & `python_gitlab-4.5.0/gitlab/v4/objects/keys.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/labels.py` & `python_gitlab-4.5.0/gitlab/v4/objects/labels.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/ldap.py` & `python_gitlab-4.5.0/gitlab/v4/objects/ldap.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/members.py` & `python_gitlab-4.5.0/gitlab/v4/objects/members.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/merge_requests.py` & `python_gitlab-4.5.0/gitlab/v4/objects/merge_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/merge_requests.html
 https://docs.gitlab.com/ee/api/merge_request_approvals.html
 """
+
 from typing import Any, cast, Dict, Optional, TYPE_CHECKING, Union
 
 import requests
 
 import gitlab
 from gitlab import cli
 from gitlab import exceptions as exc
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/milestones.py` & `python_gitlab-4.5.0/gitlab/v4/objects/milestones.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/namespaces.py` & `python_gitlab-4.5.0/gitlab/v4/objects/namespaces.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/notes.py` & `python_gitlab-4.5.0/gitlab/v4/objects/notes.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/notification_settings.py` & `python_gitlab-4.5.0/gitlab/v4/objects/notification_settings.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/packages.py` & `python_gitlab-4.5.0/gitlab/v4/objects/packages.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/pages.py` & `python_gitlab-4.5.0/gitlab/v4/objects/pages.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/personal_access_tokens.py` & `python_gitlab-4.5.0/gitlab/v4/objects/personal_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/pipelines.py` & `python_gitlab-4.5.0/gitlab/v4/objects/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ListMixin,
     ObjectDeleteMixin,
     RefreshMixin,
     RetrieveMixin,
     SaveMixin,
     UpdateMixin,
 )
-from gitlab.types import RequiredOptional
+from gitlab.types import ArrayAttribute, RequiredOptional
 
 __all__ = [
     "ProjectMergeRequestPipeline",
     "ProjectMergeRequestPipelineManager",
     "ProjectPipeline",
     "ProjectPipelineManager",
     "ProjectPipelineJob",
@@ -145,14 +145,15 @@
 
 
 class ProjectPipelineJobManager(ListMixin, RESTManager):
     _path = "/projects/{project_id}/pipelines/{pipeline_id}/jobs"
     _obj_cls = ProjectPipelineJob
     _from_parent_attrs = {"project_id": "project_id", "pipeline_id": "id"}
     _list_filters = ("scope", "include_retried")
+    _types = {"scope": ArrayAttribute}
 
 
 class ProjectPipelineBridge(RESTObject):
     pass
 
 
 class ProjectPipelineBridgeManager(ListMixin, RESTManager):
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/project_access_tokens.py` & `python_gitlab-4.5.0/gitlab/v4/objects/project_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/projects.py` & `python_gitlab-4.5.0/gitlab/v4/objects/projects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/projects.html
 """
+
 from typing import (
     Any,
     Callable,
     cast,
     Dict,
     Iterator,
     List,
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/push_rules.py` & `python_gitlab-4.5.0/gitlab/v4/objects/push_rules.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/releases.py` & `python_gitlab-4.5.0/gitlab/v4/objects/releases.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/repositories.py` & `python_gitlab-4.5.0/gitlab/v4/objects/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API: https://docs.gitlab.com/ee/api/repositories.html
 
 Currently this module only contains repository-related methods for projects.
 """
+
 from typing import Any, Callable, Dict, Iterator, List, Optional, TYPE_CHECKING, Union
 
 import requests
 
 import gitlab
 from gitlab import cli
 from gitlab import exceptions as exc
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/resource_groups.py` & `python_gitlab-4.5.0/gitlab/v4/objects/resource_groups.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/reviewers.py` & `python_gitlab-4.5.0/gitlab/v4/objects/reviewers.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/runners.py` & `python_gitlab-4.5.0/gitlab/v4/objects/runners.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/secure_files.py` & `python_gitlab-4.5.0/gitlab/v4/objects/secure_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/secure_files.html
 """
+
 from typing import Any, Callable, cast, Iterator, Optional, TYPE_CHECKING, Union
 
 import requests
 
 from gitlab import cli
 from gitlab import exceptions as exc
 from gitlab import utils
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/settings.py` & `python_gitlab-4.5.0/gitlab/v4/objects/settings.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/sidekiq.py` & `python_gitlab-4.5.0/gitlab/v4/objects/sidekiq.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/snippets.py` & `python_gitlab-4.5.0/gitlab/v4/objects/snippets.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/statistics.py` & `python_gitlab-4.5.0/gitlab/v4/objects/statistics.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/tags.py` & `python_gitlab-4.5.0/gitlab/v4/objects/tags.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/templates.py` & `python_gitlab-4.5.0/gitlab/v4/objects/templates.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/todos.py` & `python_gitlab-4.5.0/gitlab/v4/objects/todos.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/topics.py` & `python_gitlab-4.5.0/gitlab/v4/objects/topics.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/triggers.py` & `python_gitlab-4.5.0/gitlab/v4/objects/triggers.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/users.py` & `python_gitlab-4.5.0/gitlab/v4/objects/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/users.html
 https://docs.gitlab.com/ee/api/projects.html#list-projects-starred-by-a-user
 """
+
 from typing import Any, cast, Dict, List, Optional, Union
 
 import requests
 
 from gitlab import cli
 from gitlab import exceptions as exc
 from gitlab import types
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/variables.py` & `python_gitlab-4.5.0/gitlab/v4/objects/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/instance_level_ci_variables.html
 https://docs.gitlab.com/ee/api/project_level_variables.html
 https://docs.gitlab.com/ee/api/group_level_variables.html
 """
+
 from typing import Any, cast, Union
 
 from gitlab.base import RESTManager, RESTObject
 from gitlab.mixins import CRUDMixin, ObjectDeleteMixin, SaveMixin
 from gitlab.types import RequiredOptional
 
 __all__ = [
```

### Comparing `python-gitlab-4.4.0/gitlab/v4/objects/wikis.py` & `python_gitlab-4.5.0/gitlab/v4/objects/wikis.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/pyproject.toml` & `python_gitlab-4.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/python_gitlab.egg-info/PKG-INFO` & `python_gitlab-4.5.0/python_gitlab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-gitlab
-Version: 4.4.0
+Version: 4.5.0
 Summary: A python wrapper for the GitLab API
 Author-email: Gauvain Pocentek <gauvain@pocentek.net>
 Maintainer-email: John Villalovos <john@sodarock.com>, Max Wittig <max.wittig@siemens.com>, Nejc Habjan <nejc.habjan@siemens.com>, Roger Meier <r.meier@siemens.com>
 License: LGPL-3.0-or-later
 Project-URL: Homepage, https://github.com/python-gitlab/python-gitlab
 Project-URL: Changelog, https://github.com/python-gitlab/python-gitlab/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://python-gitlab.readthedocs.io
@@ -145,14 +145,31 @@
 
 You can also mount your own config file:
 
 .. code-block:: console
 
    $ docker run -it --rm -v /path/to/python-gitlab.cfg:/etc/python-gitlab.cfg registry.gitlab.com/python-gitlab/python-gitlab:latest <command> ...
 
+Usage inside GitLab CI
+~~~~~~~~~~~~~~~~~~~~~~
+
+If you want to use the Docker image directly inside your GitLab CI as an ``image``, you will need to override
+the ``entrypoint``, `as noted in the official GitLab documentation <https://docs.gitlab.com/ee/ci/docker/using_docker_images.html#override-the-entrypoint-of-an-image>`__:
+
+.. code-block:: yaml
+
+   Job Name:
+      image:
+         name: registry.gitlab.com/python-gitlab/python-gitlab:latest
+         entrypoint: [""]
+      before_script:
+         gitlab --version
+      script:
+         gitlab <command>
+
 Building the image
 ~~~~~~~~~~~~~~~~~~
 
 To build your own image from this repository, run:
 
 .. code-block:: console
```

### Comparing `python-gitlab-4.4.0/python_gitlab.egg-info/SOURCES.txt` & `python_gitlab-4.5.0/python_gitlab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 tests/functional/api/test_groups.py
 tests/functional/api/test_import_export.py
 tests/functional/api/test_issues.py
 tests/functional/api/test_keys.py
 tests/functional/api/test_lazy_objects.py
 tests/functional/api/test_merge_requests.py
 tests/functional/api/test_packages.py
+tests/functional/api/test_project_job_token_scope.py
 tests/functional/api/test_projects.py
 tests/functional/api/test_push_rules.py
 tests/functional/api/test_releases.py
 tests/functional/api/test_repository.py
 tests/functional/api/test_services.py
 tests/functional/api/test_snippets.py
 tests/functional/api/test_statistics.py
```

### Comparing `python-gitlab-4.4.0/tests/conftest.py` & `python_gitlab-4.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_current_user.py` & `python_gitlab-4.5.0/tests/functional/api/test_current_user.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 def test_current_user_email(gl):
     gl.auth()
     mail = gl.user.emails.create({"email": "current@user.com"})
     assert mail in gl.user.emails.list()
 
     mail.delete()
-    assert mail not in gl.user.emails.list()
 
 
 def test_current_user_gpg_keys(gl, GPG_KEY):
     gl.auth()
     gkey = gl.user.gpgkeys.create({"key": GPG_KEY})
     assert gkey in gl.user.gpgkeys.list()
 
     # Seems broken on the gitlab side
     gkey = gl.user.gpgkeys.get(gkey.id)
+
     gkey.delete()
-    assert gkey not in gl.user.gpgkeys.list()
 
 
 def test_current_user_ssh_keys(gl, SSH_KEY):
     gl.auth()
     key = gl.user.keys.create({"title": "testkey", "key": SSH_KEY})
     assert key in gl.user.keys.list()
 
     key.delete()
-    assert key not in gl.user.keys.list()
 
 
 def test_current_user_status(gl):
     gl.auth()
     message = "Test"
     emoji = "thumbsup"
     status = gl.user.status.get()
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_epics.py` & `python_gitlab-4.5.0/tests/functional/api/test_epics.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 def test_epic_issues(epic, issue):
     assert not epic.issues.list()
 
     epic_issue = epic.issues.create({"issue_id": issue.id})
     assert epic.issues.list()
 
     epic_issue.delete()
-    assert not epic.issues.list()
 
 
 def test_epic_notes(epic):
     assert not epic.notes.list()
 
     epic.notes.create({"body": "Test note"})
     assert epic.notes.list()
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_gitlab.py` & `python_gitlab-4.5.0/tests/functional/api/test_gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     msg = gl.broadcastmessages.list(**get_all_kwargs)[0]
     assert msg.color == "#444444"
 
     msg = gl.broadcastmessages.get(msg_id)
     assert msg.color == "#444444"
 
     msg.delete()
-    assert msg not in gl.broadcastmessages.list()
 
 
 def test_markdown(gl):
     html = gl.markdown("foo")
     assert "foo" in html
 
 
@@ -147,15 +146,14 @@
 
 
 def test_hooks(gl):
     hook = gl.hooks.create({"url": "http://whatever.com"})
     assert hook in gl.hooks.list()
 
     hook.delete()
-    assert hook not in gl.hooks.list()
 
 
 def test_namespaces(gl, get_all_kwargs):
     gl.auth()
     current_user = gl.user.username
 
     namespaces = gl.namespaces.list(**get_all_kwargs)
@@ -198,15 +196,14 @@
 @pytest.mark.skip
 def test_features(gl):
     feat = gl.features.set("foo", 30)
     assert feat.name == "foo"
     assert feat in gl.features.list()
 
     feat.delete()
-    assert feat not in gl.features.list()
 
 
 def test_pagination(gl, project):
     project2 = gl.projects.create({"name": "project-page-2"})
 
     list1 = gl.projects.list(per_page=1, page=1)
     list2 = gl.projects.list(per_page=1, page=2)
@@ -248,14 +245,15 @@
     generated"""
     with pytest.warns(UserWarning, match="python-gitlab.readthedocs.io") as record:
         gl.gitlabciymls.list()
 
     assert len(record) == 1
     warning = record[0]
     assert __file__ == warning.filename
+    assert __file__ in str(warning.message)
 
 
 def test_list_page_nowarning(gl, recwarn):
     """Using `page=X` will disable the warning"""
     gl.gitlabciymls.list(page=1)
     assert not recwarn
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_groups.py` & `python_gitlab-4.5.0/tests/functional/api/test_groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 def test_groups(gl):
     # TODO: This one still needs lots of work
     user = gl.users.create(
         {
             "email": "user@test.com",
             "username": "user",
             "name": "user",
-            "password": "user_pass",
+            "password": "E4596f8be406Bc3a14a4ccdb1df80587#!1",
         }
     )
     user2 = gl.users.create(
         {
             "email": "user2@test.com",
             "username": "user2",
             "name": "user2",
-            "password": "user2_pass",
+            "password": "E4596f8be406Bc3a14a4ccdb1df80587#!#2",
         }
     )
     group1 = gl.groups.create(
         {"name": "gitlab-test-group1", "path": "gitlab-test-group1"}
     )
     group2 = gl.groups.create(
         {"name": "gitlab-test-group2", "path": "gitlab-test-group2"}
@@ -101,16 +101,17 @@
 
     # Test `user_ids` array
     result = group1.members.list(user_ids=[user.id, 99999])
     assert len(result) == 1
     assert result[0].id == user.id
 
     group1.members.delete(user.id)
-    assert user not in group1.members.list()
+
     assert group1.members_all.list()
+
     member = group1.members.get(user2.id)
     member.access_level = gitlab.const.AccessLevel.OWNER
     member.save()
     member = group1.members.get(user2.id)
     assert member.access_level == gitlab.const.AccessLevel.OWNER
 
     gl.auth()
@@ -131,15 +132,14 @@
     label.new_name = "Label:that requires:encoding"
     label.save()
     assert label.name == "Label:that requires:encoding"
     label = group.labels.get("Label:that requires:encoding")
     assert label.name == "Label:that requires:encoding"
 
     label.delete()
-    assert label not in group.labels.list()
 
 
 @pytest.mark.gitlab_premium
 @pytest.mark.xfail(reason="/ldap/groups endpoint not documented")
 def test_ldap_groups(gl):
     assert isinstance(gl.ldapgroups.list(), list)
 
@@ -190,15 +190,14 @@
     badge.image_url = "http://another.example.com"
     badge.save()
 
     badge = group.badges.get(badge.id)
     assert badge.image_url == "http://another.example.com"
 
     badge.delete()
-    assert badge not in group.badges.list()
 
 
 def test_group_milestones(group):
     milestone = group.milestones.create({"title": "groupmilestone1"})
     assert milestone in group.milestones.list()
 
     milestone.due_date = "2020-01-01T00:00:00Z"
@@ -224,15 +223,14 @@
 
     attr = group.customattributes.set("key", "value2")
     attr = group.customattributes.get("key")
     assert attr.value == "value2"
     assert attr in group.customattributes.list()
 
     attr.delete()
-    assert attr not in group.customattributes.list()
 
 
 def test_group_subgroups_projects(gl, user):
     # TODO: fixture factories
     group1 = gl.groups.list(search="group1")[0]
     group2 = gl.groups.list(search="group2")[0]
 
@@ -266,30 +264,28 @@
     wiki = group.wikis.get(wiki.slug)
     assert wiki.content == content
 
     wiki.content = "new content"
     wiki.save()
 
     wiki.delete()
-    assert wiki not in group.wikis.list()
 
 
 @pytest.mark.gitlab_premium
 def test_group_hooks(group):
     hook = group.hooks.create({"url": "http://hook.url"})
     assert hook in group.hooks.list()
 
     hook.note_events = True
     hook.save()
 
     hook = group.hooks.get(hook.id)
     assert hook.note_events is True
 
     hook.delete()
-    assert hook not in group.hooks.list()
 
 
 def test_group_transfer(gl, group):
     transfer_group = gl.groups.create(
         {"name": "transfer-test-group", "path": "transfer-test-group"}
     )
     transfer_group = gl.groups.get(transfer_group.id)
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_import_export.py` & `python_gitlab-4.5.0/tests/functional/api/test_import_export.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import time
 
 import pytest
 
 import gitlab
 
 
+# https://github.com/python-gitlab/python-gitlab/pull/2790#pullrequestreview-1873617123
 def test_group_import_export(gl, group, temp_dir):
     export = group.exports.create()
     assert export.message == "202 Accepted"
 
     # We cannot check for export_status with group export API
     time.sleep(10)
 
@@ -27,14 +28,16 @@
     time.sleep(10)
     group_import = gl.groups.get(import_path)
 
     assert group_import.path == import_path
     assert group_import.name == import_name
 
 
+# https://github.com/python-gitlab/python-gitlab/pull/2790#pullrequestreview-1873617123
+@pytest.mark.xfail(reason="test_project_import_export to be worked on in a follow up")
 def test_project_import_export(gl, project, temp_dir):
     export = project.exports.create()
     assert export.message == "202 Accepted"
 
     export = project.exports.get()
     assert isinstance(export, gitlab.v4.objects.ProjectExport)
 
@@ -64,26 +67,32 @@
         time.sleep(1)
         project_import.refresh()
         count += 1
         if count == 15:
             raise Exception("Project import taking too much time")
 
 
+# https://github.com/python-gitlab/python-gitlab/pull/2790#pullrequestreview-1873617123
+@pytest.mark.xfail(reason="test_project_remote_import to be worked on in a follow up")
 def test_project_remote_import(gl):
     with pytest.raises(gitlab.exceptions.GitlabImportError) as err_info:
         gl.projects.remote_import(
             "ftp://whatever.com/url", "remote-project", "remote-project", "root"
         )
     assert err_info.value.response_code == 400
     assert (
         "File url is blocked: Only allowed schemes are https"
         in err_info.value.error_message
     )
 
 
+# https://github.com/python-gitlab/python-gitlab/pull/2790#pullrequestreview-1873617123
+@pytest.mark.xfail(
+    reason="test_project_remote_import_s3 to be worked on in a follow up"
+)
 def test_project_remote_import_s3(gl):
     gl.features.set("import_project_from_remote_file_s3", True)
     with pytest.raises(gitlab.exceptions.GitlabImportError) as err_info:
         gl.projects.remote_import_s3(
             "remote-project",
             "aws-region",
             "aws-bucket-name",
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_issues.py` & `python_gitlab-4.5.0/tests/functional/api/test_issues.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,33 +14,28 @@
     assert {issue, issue2} == set(filtered_issues)
 
     issue2.state_event = "close"
     issue2.save()
     assert issue in project.issues.list(state="opened")
     assert issue2 in project.issues.list(state="closed")
 
-    assert isinstance(issue.user_agent_detail(), dict)
-    assert issue.user_agent_detail()["user_agent"]
     assert issue.participants()
     assert type(issue.closed_by()) == list
     assert type(issue.related_merge_requests()) == list
 
 
 def test_issue_notes(issue):
     note = issue.notes.create({"body": "This is an issue note"})
     assert note in issue.notes.list()
 
     emoji = note.awardemojis.create({"name": "tractor"})
     assert emoji in note.awardemojis.list()
 
     emoji.delete()
-    assert emoji not in note.awardemojis.list()
-
     note.delete()
-    assert note not in issue.notes.list()
 
 
 def test_issue_labels(project, issue):
     project.labels.create({"name": "label2", "color": "#aabbcc"})
     issue.labels = ["label2"]
     issue.save()
 
@@ -58,16 +53,16 @@
     assert source_issue == issue
     assert target_issue == linked_issue
 
     links = issue.links.list()
     assert links
 
     link_id = links[0].issue_link_id
+
     issue.links.delete(link_id)
-    assert not issue.links.list()
 
 
 def test_issue_label_events(issue):
     events = issue.resourcelabelevents.list()
     assert isinstance(events, list)
 
     event = issue.resourcelabelevents.get(events[0].id)
@@ -110,9 +105,7 @@
     d_note_from_get.body = "updated body"
     d_note_from_get.save()
 
     discussion = issue.discussions.get(discussion.id)
     assert discussion.attributes["notes"][-1]["body"] == "updated body"
 
     d_note_from_get.delete()
-    discussion = issue.discussions.get(discussion.id)
-    assert len(discussion.attributes["notes"]) == 1
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_keys.py` & `python_gitlab-4.5.0/tests/functional/api/test_keys.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ce/api/keys.html
 """
+
 import base64
 import hashlib
 
 
 def key_fingerprint(key: str) -> str:
     key_part = key.split()[1]
     decoded = base64.b64decode(key_part.encode("ascii"))
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_lazy_objects.py` & `python_gitlab-4.5.0/tests/functional/api/test_lazy_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import time
+
 import pytest
 
 import gitlab
 
 
 @pytest.fixture
 def lazy_project(gl, project):
@@ -23,16 +25,17 @@
 def test_save_after_lazy_get_with_path(project, lazy_project):
     lazy_project.description = "A new description"
     lazy_project.save()
     assert lazy_project.id == project.id
     assert lazy_project.description == "A new description"
 
 
-def test_delete_after_lazy_get_with_path(gl, group, wait_for_sidekiq):
+def test_delete_after_lazy_get_with_path(gl, group):
     project = gl.projects.create({"name": "lazy_project", "namespace_id": group.id})
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
     lazy_project = gl.projects.get(project.path_with_namespace, lazy=True)
     lazy_project.delete()
 
 
 def test_list_children_after_lazy_get_with_path(gl, lazy_project):
     lazy_project.mergerequests.list()
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_merge_requests.py` & `python_gitlab-4.5.0/tests/functional/api/test_merge_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import time
 
 import pytest
 
 import gitlab
 import gitlab.v4.objects
 
@@ -12,27 +13,27 @@
             "file_path": "README.rst",
             "branch": "main",
             "content": "Initial content",
             "commit_message": "Initial commit",
         }
     )
 
-    source_branch = "branch1"
+    source_branch = "branch-merge-request-api"
     project.branches.create({"branch": source_branch, "ref": "main"})
 
     project.files.create(
         {
             "file_path": "README2.rst",
             "branch": source_branch,
             "content": "Initial content",
             "commit_message": "New commit in new branch",
         }
     )
     project.mergerequests.create(
-        {"source_branch": "branch1", "target_branch": "main", "title": "MR readme2"}
+        {"source_branch": source_branch, "target_branch": "main", "title": "MR readme2"}
     )
 
 
 def test_merge_requests_get(project, merge_request):
     mr = project.mergerequests.get(merge_request.iid)
     assert mr.iid == merge_request.iid
 
@@ -68,16 +69,14 @@
     note_from_get.body = "updated body"
     note_from_get.save()
 
     discussion = mr.discussions.get(discussion.id)
     assert discussion.attributes["notes"][-1]["body"] == "updated body"
 
     note_from_get.delete()
-    discussion = mr.discussions.get(discussion.id)
-    assert len(discussion.attributes["notes"]) == 1
 
 
 def test_merge_request_labels(project):
     mr = project.mergerequests.list()[0]
     mr.labels = ["label2"]
     mr.save()
 
@@ -160,106 +159,112 @@
 
     approval_rules[0].save()
     approval_rules = project.approvalrules.list(get_all=True)
     assert len(approval_rules) == 1
     assert approval_rules[0].approvals_required == 2
 
     approval_rules[0].delete()
-    ars = project.approvalrules.list(get_all=True)
-    assert len(ars) == 0
 
 
-def test_merge_request_reset_approvals(gitlab_url, project, wait_for_sidekiq):
-    bot = project.access_tokens.create({"name": "bot", "scopes": ["api"]})
+def test_merge_request_reset_approvals(gitlab_url, project):
+    today = datetime.date.today()
+    future_date = today + datetime.timedelta(days=4)
+    bot = project.access_tokens.create(
+        {"name": "bot", "scopes": ["api"], "expires_at": future_date.isoformat()}
+    )
+
     bot_gitlab = gitlab.Gitlab(gitlab_url, private_token=bot.token)
     bot_project = bot_gitlab.projects.get(project.id, lazy=True)
 
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
+
     mr = bot_project.mergerequests.list()[0]  # type: ignore[index]
+
     assert mr.reset_approvals()
 
 
-def test_cancel_merge_when_pipeline_succeeds(
-    project, merge_request_with_pipeline, wait_for_sidekiq
-):
-    wait_for_sidekiq(timeout=60)
+def test_cancel_merge_when_pipeline_succeeds(project, merge_request_with_pipeline):
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
     # Set to merge when the pipeline succeeds, which should never happen
     merge_request_with_pipeline.merge(merge_when_pipeline_succeeds=True)
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
 
     mr = project.mergerequests.get(merge_request_with_pipeline.iid)
     assert mr.merged_at is None
     assert mr.merge_when_pipeline_succeeds is True
     cancel = mr.cancel_merge_when_pipeline_succeeds()
     assert cancel == {"status": "success"}
 
 
-def test_merge_request_merge(project, merge_request, wait_for_sidekiq):
+def test_merge_request_merge(project, merge_request):
     merge_request.merge()
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
 
     mr = project.mergerequests.get(merge_request.iid)
     assert mr.merged_at is not None
     assert mr.merge_when_pipeline_succeeds is False
     with pytest.raises(gitlab.GitlabMRClosedError):
         # Two merge attempts should raise GitlabMRClosedError
         mr.merge()
 
 
-def test_merge_request_should_remove_source_branch(
-    project, merge_request, wait_for_sidekiq
-) -> None:
+def test_merge_request_should_remove_source_branch(project, merge_request) -> None:
     """Test to ensure
     https://github.com/python-gitlab/python-gitlab/issues/1120 is fixed.
     Bug reported that they could not use 'should_remove_source_branch' in
     mr.merge() call"""
     merge_request.merge(should_remove_source_branch=True)
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
 
     # Wait until it is merged
     mr = None
     mr_iid = merge_request.iid
     for _ in range(60):
         mr = project.mergerequests.get(mr_iid)
         if mr.merged_at is not None:
             break
         time.sleep(0.5)
 
     assert mr is not None
     assert mr.merged_at is not None
     time.sleep(0.5)
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
 
     # Ensure we can NOT get the MR branch
     with pytest.raises(gitlab.exceptions.GitlabGetError):
         result = project.branches.get(merge_request.source_branch)
         # Help to debug in case the expected exception doesn't happen.
         import pprint
 
         print("mr:", pprint.pformat(mr))
         print("mr.merged_at:", pprint.pformat(mr.merged_at))
         print("result:", pprint.pformat(result))
 
 
-def test_merge_request_large_commit_message(
-    project, merge_request, wait_for_sidekiq
-) -> None:
+def test_merge_request_large_commit_message(project, merge_request) -> None:
     """Test to ensure https://github.com/python-gitlab/python-gitlab/issues/1452
     is fixed.
     Bug reported that very long 'merge_commit_message' in mr.merge() would
     cause an error: 414 Request too large
     """
     merge_commit_message = "large_message\r\n" * 1_000
     assert len(merge_commit_message) > 10_000
 
     merge_request.merge(
         merge_commit_message=merge_commit_message, should_remove_source_branch=False
     )
 
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
 
     # Wait until it is merged
     mr = None
     mr_iid = merge_request.iid
     for _ in range(60):
         mr = project.mergerequests.get(mr_iid)
         if mr.merged_at is not None:
@@ -275,25 +280,24 @@
 
 
 def test_merge_request_merge_ref(merge_request) -> None:
     response = merge_request.merge_ref()
     assert response and "commit_id" in response
 
 
-def test_merge_request_merge_ref_should_fail(
-    project, merge_request, wait_for_sidekiq
-) -> None:
+def test_merge_request_merge_ref_should_fail(project, merge_request) -> None:
     # Create conflict
     project.files.create(
         {
             "file_path": f"README.{merge_request.source_branch}",
             "branch": project.default_branch,
             "content": "Different initial content",
             "commit_message": "Another commit in main branch",
         }
     )
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
 
     # Check for non-existing merge_ref for MR with conflicts
     with pytest.raises(gitlab.exceptions.GitlabGetError):
         response = merge_request.merge_ref()
         assert "commit_id" not in response
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_packages.py` & `python_gitlab-4.5.0/tests/functional/api/test_packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API:
 https://docs.gitlab.com/ce/api/packages.html
 https://docs.gitlab.com/ee/user/packages/generic_packages
 """
+
 from collections.abc import Iterator
 
 from gitlab.v4.objects import GenericPackage
 
 package_name = "hello-world"
 package_version = "v1.0.0"
 file_name = "hello.tar.gz"
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_projects.py` & `python_gitlab-4.5.0/tests/functional/api/test_projects.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 import uuid
 
 import pytest
 
 import gitlab
 from gitlab.const import AccessLevel
 from gitlab.v4.objects.projects import ProjectStorage
@@ -41,15 +42,14 @@
     member = project.members.create(
         {"user_id": user.id, "access_level": AccessLevel.DEVELOPER}
     )
     assert member in project.members.list()
     assert member.access_level == 30
 
     member.delete()
-    assert member not in project.members.list()
 
 
 def test_project_badges(project):
     badge_image = "http://example.com"
     badge_link = "http://example/img.svg"
 
     badge = project.badges.create({"link_url": badge_link, "image_url": badge_image})
@@ -58,15 +58,14 @@
     badge.image_url = "http://another.example.com"
     badge.save()
 
     badge = project.badges.get(badge.id)
     assert badge.image_url == "http://another.example.com"
 
     badge.delete()
-    assert badge not in project.badges.list()
 
 
 @pytest.mark.skip(reason="Commented out in legacy test")
 def test_project_boards(project):
     boards = project.boards.list()
     assert boards
 
@@ -74,15 +73,14 @@
     lists = board.lists.list()
 
     last_list = lists[-1]
     last_list.position = 0
     last_list.save()
 
     last_list.delete()
-    assert last_list not in board.lists.list()
 
 
 def test_project_custom_attributes(gl, project):
     attrs = project.customattributes.list()
     assert not attrs
 
     attr = project.customattributes.set("key", "value1")
@@ -93,15 +91,14 @@
 
     attr = project.customattributes.set("key", "value2")
     attr = project.customattributes.get("key")
     assert attr.value == "value2"
     assert attr in project.customattributes.list()
 
     attr.delete()
-    assert attr not in project.customattributes.list()
 
 
 def test_project_environments(project):
     environment = project.environments.create(
         {"name": "env1", "external_url": "http://fake.env/whatever"}
     )
     environments = project.environments.list()
@@ -111,16 +108,16 @@
     environment.external_url = "http://new.env/whatever"
     environment.save()
 
     environment = project.environments.list()[0]
     assert environment.external_url == "http://new.env/whatever"
 
     environment.stop()
+
     environment.delete()
-    assert environment not in project.environments.list()
 
 
 def test_project_events(project):
     events = project.events.list()
     assert isinstance(events, list)
 
 
@@ -152,15 +149,14 @@
     hook.note_events = True
     hook.save()
 
     hook = project.hooks.get(hook.id)
     assert hook.note_events is True
 
     hook.delete()
-    assert hook not in project.hooks.list()
 
 
 def test_project_housekeeping(project):
     project.housekeeping()
 
 
 def test_project_labels(project):
@@ -180,15 +176,14 @@
     label.subscribe()
     assert label.subscribed is True
 
     label.unsubscribe()
     assert label.subscribed is False
 
     label.delete()
-    assert label not in project.labels.list()
 
 
 def test_project_label_promotion(gl, group):
     """
     Label promotion requires the project to be a child of a group (not in a user namespace)
 
     """
@@ -202,15 +197,14 @@
     label_name = "promoteme"
     promoted_label = project.labels.create({"name": label_name, "color": "#112233"})
     promoted_label.promote()
 
     assert any(label.name == label_name for label in group.labels.list())
 
     group.labels.delete(label_name)
-    assert not any(label.name == label_name for label in group.labels.list())
 
 
 def test_project_milestones(project):
     milestone = project.milestones.create({"title": "milestone1"})
     assert milestone in project.milestones.list()
 
     milestone.due_date = "2020-01-01T00:00:00Z"
@@ -251,25 +245,44 @@
     assert domain in project.pagesdomains.list()
     assert domain in gl.pagesdomains.list()
 
     domain = project.pagesdomains.get("foo.domain.com")
     assert domain.domain == "foo.domain.com"
 
     domain.delete()
-    assert domain not in project.pagesdomains.list()
 
 
-def test_project_protected_branches(project):
-    p_b = project.protectedbranches.create({"name": "*-stable"})
+def test_project_protected_branches(project, gitlab_version):
+    # Updating a protected branch is possible from Gitlab 15.6
+    # https://docs.gitlab.com/ee/api/protected_branches.html#update-a-protected-branch
+    can_update_prot_branch = gitlab_version.major > 15 or (
+        gitlab_version.major == 15 and gitlab_version.minor >= 6
+    )
+
+    p_b = project.protectedbranches.create(
+        {
+            "name": "*-stable",
+            "allow_force_push": False,
+        }
+    )
     assert p_b.name == "*-stable"
+    assert not p_b.allow_force_push
     assert p_b in project.protectedbranches.list()
 
+    if can_update_prot_branch:
+        p_b.allow_force_push = True
+        p_b.save()
+        # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+        time.sleep(5)
+
     p_b = project.protectedbranches.get("*-stable")
-    p_b.delete()
-    assert p_b not in project.protectedbranches.list()
+    if can_update_prot_branch:
+        assert p_b.allow_force_push
+
+        p_b.delete()
 
 
 def test_project_remote_mirrors(project):
     mirror_url = "https://gitlab.example.com/root/mirror.git"
 
     mirror = project.remote_mirrors.create({"url": mirror_url})
     assert mirror.url == mirror_url
@@ -296,17 +309,14 @@
     service.save()
 
     service = project.services.get("asana")
     assert service.active is True
 
     service.delete()
 
-    service = project.services.get("asana")
-    assert service.active is False
-
 
 def test_project_stars(project):
     project.star()
     assert project.star_count == 1
 
     project.unstar()
     assert project.star_count == 0
@@ -319,38 +329,36 @@
 
 
 def test_project_tags(project, project_file):
     tag = project.tags.create({"tag_name": "v1.0", "ref": "main"})
     assert tag in project.tags.list()
 
     tag.delete()
-    assert tag not in project.tags.list()
 
 
 def test_project_triggers(project):
     trigger = project.triggers.create({"description": "trigger1"})
     assert trigger in project.triggers.list()
 
     trigger.delete()
-    assert trigger not in project.triggers.list()
 
 
 def test_project_wiki(project):
     content = "Wiki page content"
     wiki = project.wikis.create({"title": "wikipage", "content": content})
     assert wiki in project.wikis.list()
 
     wiki = project.wikis.get(wiki.slug)
     assert wiki.content == content
 
     # update and delete seem broken
     wiki.content = "new content"
     wiki.save()
+
     wiki.delete()
-    assert wiki not in project.wikis.list()
 
 
 def test_project_groups_list(gl, group):
     """Test listing groups of a project"""
     # Create a subgroup of our top-group, we will place our new project inside
     # this group.
     group2 = gl.groups.create(
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_push_rules.py` & `python_gitlab-4.5.0/tests/functional/api/test_push_rules.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_releases.py` & `python_gitlab-4.5.0/tests/functional/api/test_releases.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 
     release = project.releases.get(release.tag_name)
     assert release.description == updated_description
 
 
 def test_delete_project_release(project, release):
     project.releases.delete(release.tag_name)
-    assert release not in project.releases.list()
 
 
 def test_create_project_release_links(project, release):
     release.links.create(link_data)
 
     release = project.releases.get(release.tag_name)
     assert release.assets["links"][0]["url"] == link_data["url"]
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_repository.py` & `python_gitlab-4.5.0/tests/functional/api/test_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,18 +154,16 @@
     assert discussion in commit.discussions.list()
 
     note = discussion.notes.create({"body": "first note"})
     note_from_get = discussion.notes.get(note.id)
     note_from_get.body = "updated body"
     note_from_get.save()
     discussion = commit.discussions.get(discussion.id)
-    # assert discussion.attributes["notes"][-1]["body"] == "updated body"
+
     note_from_get.delete()
-    discussion = commit.discussions.get(discussion.id)
-    # assert len(discussion.attributes["notes"]) == 1
 
 
 def test_revert_commit(project):
     commit = project.commits.list()[0]
     revert_commit = commit.revert(branch="main")
 
     expected_message = f'Revert "{commit.message}"\n\nThis reverts commit {commit.id}'
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_services.py` & `python_gitlab-4.5.0/tests/functional/api/test_services.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,11 +28,9 @@
     service_object = project.services.get(service["slug"])
     assert isinstance(service_object, gitlab.v4.objects.ProjectService)
     assert service_object.active
 
 
 def test_delete_service(project, service):
     service_object = project.services.get(service["slug"])
-    service_object.delete()
 
-    service_object = project.services.get(service["slug"])
-    assert not service_object.active
+    service_object.delete()
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_snippets.py` & `python_gitlab-4.5.0/tests/functional/api/test_snippets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 import gitlab
 
 
 def test_snippets(gl):
     snippets = gl.snippets.list(get_all=True)
     assert not snippets
 
@@ -16,33 +18,40 @@
     snippet.save()
 
     snippet = gl.snippets.get(snippet.id)
     assert snippet.title == "updated_title"
 
     content = snippet.content()
     assert content.decode() == "import gitlab"
-    assert snippet.user_agent_detail()["user_agent"]
 
     snippet.delete()
-    assert snippet not in gl.snippets.list(get_all=True)
 
 
 def test_project_snippets(project):
     project.snippets_enabled = True
     project.save()
 
     snippet = project.snippets.create(
         {
             "title": "snip1",
             "files": [{"file_path": "foo.py", "content": "initial content"}],
             "visibility": gitlab.const.VISIBILITY_PRIVATE,
         }
     )
 
-    assert snippet.user_agent_detail()["user_agent"]
+    assert snippet.title == "snip1"
+
+
+@pytest.mark.xfail(reason="Returning 404 UserAgentDetail not found in GL 16")
+def test_project_snippet_user_agent_detail(project):
+    snippet = project.snippets.list()[0]
+
+    user_agent_detail = snippet.user_agent_detail()
+
+    assert user_agent_detail["user_agent"]
 
 
 def test_project_snippet_discussion(project):
     snippet = project.snippets.list()[0]
 
     discussion = snippet.discussions.create({"body": "Discussion body"})
     assert discussion in snippet.discussions.list()
@@ -52,23 +61,20 @@
     note_from_get.body = "updated body"
     note_from_get.save()
 
     discussion = snippet.discussions.get(discussion.id)
     assert discussion.attributes["notes"][-1]["body"] == "updated body"
 
     note_from_get.delete()
-    discussion = snippet.discussions.get(discussion.id)
-    assert len(discussion.attributes["notes"]) == 1
 
 
 def test_project_snippet_file(project):
     snippet = project.snippets.list()[0]
     snippet.file_name = "bar.py"
     snippet.save()
 
     snippet = project.snippets.get(snippet.id)
     assert snippet.content().decode() == "initial content"
     assert snippet.file_name == "bar.py"
     assert snippet in project.snippets.list()
 
     snippet.delete()
-    assert snippet not in project.snippets.list()
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_topics.py` & `python_gitlab-4.5.0/tests/functional/api/test_topics.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,8 +27,7 @@
     if gitlab_version.major >= 15:
         create_dict["title"] = "my second topic title"
     topic2 = gl.topics.create(create_dict)
     merged_topic = gl.topics.merge(topic.id, topic2.id)
     assert merged_topic["id"] == topic2.id
 
     topic2.delete()
-    assert not gl.topics.list()
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_users.py` & `python_gitlab-4.5.0/tests/unit/objects/test_hooks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,209 @@
 """
-GitLab API:
-https://docs.gitlab.com/ee/api/users.html
-https://docs.gitlab.com/ee/api/users.html#delete-authentication-identity-from-user
+GitLab API: https://docs.gitlab.com/ce/api/system_hooks.html
+GitLab API: https://docs.gitlab.com/ce/api/groups.html#hooks
+GitLab API: https://docs.gitlab.com/ee/api/projects.html#hooks
 """
-import requests
 
+import re
 
-def test_create_user(gl, fixture_dir):
-    user = gl.users.create(
-        {
-            "email": "foo@bar.com",
-            "username": "foo",
-            "name": "foo",
-            "password": "foo_password",
-            "avatar": open(fixture_dir / "avatar.png", "rb"),
-        }
-    )
+import pytest
+import responses
 
-    created_user = gl.users.list(username="foo")[0]
-    assert created_user.username == user.username
-    assert created_user.email == user.email
+from gitlab.v4.objects import GroupHook, Hook, ProjectHook
 
-    avatar_url = user.avatar_url.replace("gitlab.test", "localhost:8080")
-    uploaded_avatar = requests.get(avatar_url).content
-    with open(fixture_dir / "avatar.png", "rb") as f:
-        assert uploaded_avatar == f.read()
-
-
-def test_block_user(gl, user):
-    result = user.block()
-    assert result is True
-    users = gl.users.list(blocked=True)
-    assert user in users
-
-    # block again
-    result = user.block()
-    # Trying to block an already blocked user returns None
-    assert result is None
-
-    result = user.unblock()
-    assert result is True
-    users = gl.users.list(blocked=False)
-    assert user in users
-
-    # unblock again
-    result = user.unblock()
-    # Trying to unblock an already blocked user returns False
-    assert result is False
-
-
-def test_ban_user(gl, user):
-    user.ban()
-    retrieved_user = gl.users.get(user.id)
-    assert retrieved_user.state == "banned"
-
-    user.unban()
-    retrieved_user = gl.users.get(user.id)
-    assert retrieved_user.state == "active"
-
-
-def test_delete_user(gl, wait_for_sidekiq):
-    new_user = gl.users.create(
-        {
-            "email": "delete-user@test.com",
-            "username": "delete-user",
-            "name": "delete-user",
-            "password": "delete-user-pass",
-        }
-    )
-
-    new_user.delete()
-    wait_for_sidekiq(timeout=60)
-
-    assert new_user.id not in [user.id for user in gl.users.list()]
-
-
-def test_user_projects_list(gl, user):
-    projects = user.projects.list()
-    assert isinstance(projects, list)
-    assert not projects
-
-
-def test_user_events_list(gl, user):
-    events = user.events.list()
-    assert isinstance(events, list)
-    assert not events
-
-
-def test_user_bio(gl, user):
-    user.bio = "This is the user bio"
-    user.save()
-
-
-def test_list_multiple_users(gl, user):
-    second_email = f"{user.email}.2"
-    second_username = f"{user.username}_2"
-    second_user = gl.users.create(
-        {
-            "email": second_email,
-            "username": second_username,
-            "name": "Foo Bar",
-            "password": "foobar_password",
-        }
-    )
-    assert gl.users.list(search=second_user.username)[0].id == second_user.id
-
-    expected = [user, second_user]
-    actual = list(gl.users.list(search=user.username))
-
-    assert set(expected) == set(actual)
-    assert not gl.users.list(search="asdf")
-
-
-def test_user_gpg_keys(gl, user, GPG_KEY):
-    gkey = user.gpgkeys.create({"key": GPG_KEY})
-    assert gkey in user.gpgkeys.list()
-
-    # Seems broken on the gitlab side
-    # gkey = user.gpgkeys.get(gkey.id)
-
-    gkey.delete()
-    assert gkey not in user.gpgkeys.list()
-
-
-def test_user_ssh_keys(gl, user, SSH_KEY):
-    key = user.keys.create({"title": "testkey", "key": SSH_KEY})
-    assert key in user.keys.list()
-
-    get_key = user.keys.get(key.id)
-    assert get_key.key == key.key
-
-    key.delete()
-    assert key not in user.keys.list()
-
-
-def test_user_email(gl, user):
-    email = user.emails.create({"email": "foo2@bar.com"})
-    assert email in user.emails.list()
-
-    email.delete()
-    assert email not in user.emails.list()
-
-
-def test_user_custom_attributes(gl, user):
-    attrs = user.customattributes.list()
-    assert not attrs
-
-    attr = user.customattributes.set("key", "value1")
-    assert user in gl.users.list(custom_attributes={"key": "value1"})
-    assert attr.key == "key"
-    assert attr.value == "value1"
-    assert attr in user.customattributes.list()
-
-    attr = user.customattributes.set("key", "value2")
-    attr = user.customattributes.get("key")
-    assert attr.value == "value2"
-    assert attr in user.customattributes.list()
-
-    attr.delete()
-    assert attr not in user.customattributes.list()
-
-
-def test_user_impersonation_tokens(gl, user):
-    token = user.impersonationtokens.create(
-        {"name": "token1", "scopes": ["api", "read_user"]}
-    )
-    assert token in user.impersonationtokens.list(state="active")
-
-    token.delete()
-    assert token not in user.impersonationtokens.list(state="active")
-    assert token in user.impersonationtokens.list(state="inactive")
-
-
-def test_user_identities(gl, user):
-    provider = "test_provider"
-
-    user.provider = provider
-    user.extern_uid = "1"
-    user.save()
-    assert provider in [item["provider"] for item in user.identities]
-
-    user.identityproviders.delete(provider)
-    user = gl.users.get(user.id)
-    assert provider not in [item["provider"] for item in user.identities]
+hooks_content = [
+    {
+        "id": 1,
+        "url": "testurl",
+        "push_events": True,
+        "tag_push_events": True,
+    },
+    {
+        "id": 2,
+        "url": "testurl_second",
+        "push_events": False,
+        "tag_push_events": False,
+    },
+]
+
+hook_content = hooks_content[0]
+
+
+@pytest.fixture
+def resp_hooks_list():
+    with responses.RequestsMock() as rsps:
+        rsps.add(
+            method=responses.GET,
+            url=re.compile(r"http://localhost/api/v4/((groups|projects)/1/|)hooks"),
+            json=hooks_content,
+            content_type="application/json",
+            status=200,
+        )
+        yield rsps
+
+
+@pytest.fixture
+def resp_hook_get():
+    with responses.RequestsMock() as rsps:
+        rsps.add(
+            method=responses.GET,
+            url=re.compile(r"http://localhost/api/v4/((groups|projects)/1/|)hooks/1"),
+            json=hook_content,
+            content_type="application/json",
+            status=200,
+        )
+        yield rsps
+
+
+@pytest.fixture
+def resp_hook_create():
+    with responses.RequestsMock() as rsps:
+        rsps.add(
+            method=responses.POST,
+            url=re.compile(r"http://localhost/api/v4/((groups|projects)/1/|)hooks"),
+            json=hook_content,
+            content_type="application/json",
+            status=200,
+        )
+        yield rsps
+
+
+@pytest.fixture
+def resp_hook_update():
+    with responses.RequestsMock() as rsps:
+        pattern = re.compile(r"http://localhost/api/v4/((groups|projects)/1/|)hooks/1")
+        rsps.add(
+            method=responses.GET,
+            url=pattern,
+            json=hook_content,
+            content_type="application/json",
+            status=200,
+        )
+        rsps.add(
+            method=responses.PUT,
+            url=pattern,
+            json=hook_content,
+            content_type="application/json",
+            status=200,
+        )
+        yield rsps
+
+
+@pytest.fixture
+def resp_hook_delete():
+    with responses.RequestsMock() as rsps:
+        pattern = re.compile(r"http://localhost/api/v4/((groups|projects)/1/|)hooks/1")
+        rsps.add(
+            method=responses.GET,
+            url=pattern,
+            json=hook_content,
+            content_type="application/json",
+            status=200,
+        )
+        rsps.add(
+            method=responses.DELETE,
+            url=pattern,
+            status=204,
+        )
+        yield rsps
+
+
+def test_list_system_hooks(gl, resp_hooks_list):
+    hooks = gl.hooks.list()
+    assert hooks[0].id == 1
+    assert hooks[0].url == "testurl"
+    assert hooks[1].id == 2
+    assert hooks[1].url == "testurl_second"
+
+
+def test_get_system_hook(gl, resp_hook_get):
+    data = gl.hooks.get(1)
+    assert isinstance(data, Hook)
+    assert data.url == "testurl"
+    assert data.id == 1
+
+
+def test_create_system_hook(gl, resp_hook_create):
+    hook = gl.hooks.create(hook_content)
+    assert hook.url == "testurl"
+    assert hook.push_events is True
+    assert hook.tag_push_events is True
+
+
+# there is no update method for system hooks
+
+
+def test_delete_system_hook(gl, resp_hook_delete):
+    hook = gl.hooks.get(1)
+    hook.delete()
+    gl.hooks.delete(1)
+
+
+def test_list_group_hooks(group, resp_hooks_list):
+    hooks = group.hooks.list()
+    assert hooks[0].id == 1
+    assert hooks[0].url == "testurl"
+    assert hooks[1].id == 2
+    assert hooks[1].url == "testurl_second"
+
+
+def test_get_group_hook(group, resp_hook_get):
+    data = group.hooks.get(1)
+    assert isinstance(data, GroupHook)
+    assert data.url == "testurl"
+    assert data.id == 1
+
+
+def test_create_group_hook(group, resp_hook_create):
+    hook = group.hooks.create(hook_content)
+    assert hook.url == "testurl"
+    assert hook.push_events is True
+    assert hook.tag_push_events is True
+
+
+def test_update_group_hook(group, resp_hook_update):
+    hook = group.hooks.get(1)
+    assert hook.id == 1
+    hook.url = "testurl_more"
+    hook.save()
+
+
+def test_delete_group_hook(group, resp_hook_delete):
+    hook = group.hooks.get(1)
+    hook.delete()
+    group.hooks.delete(1)
+
+
+def test_list_project_hooks(project, resp_hooks_list):
+    hooks = project.hooks.list()
+    assert hooks[0].id == 1
+    assert hooks[0].url == "testurl"
+    assert hooks[1].id == 2
+    assert hooks[1].url == "testurl_second"
+
+
+def test_get_project_hook(project, resp_hook_get):
+    data = project.hooks.get(1)
+    assert isinstance(data, ProjectHook)
+    assert data.url == "testurl"
+    assert data.id == 1
+
+
+def test_create_project_hook(project, resp_hook_create):
+    hook = project.hooks.create(hook_content)
+    assert hook.url == "testurl"
+    assert hook.push_events is True
+    assert hook.tag_push_events is True
+
+
+def test_update_project_hook(project, resp_hook_update):
+    hook = project.hooks.get(1)
+    assert hook.id == 1
+    hook.url = "testurl_more"
+    hook.save()
+
+
+def test_delete_project_hook(project, resp_hook_delete):
+    hook = project.hooks.get(1)
+    hook.delete()
+    project.hooks.delete(1)
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_variables.py` & `python_gitlab-4.5.0/tests/functional/api/test_variables.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,36 +13,33 @@
 
     variable.value = "new_value1"
     variable.save()
     variable = gl.variables.get(variable.key)
     assert variable.value == "new_value1"
 
     variable.delete()
-    assert variable not in gl.variables.list()
 
 
 def test_group_variables(group):
     variable = group.variables.create({"key": "key1", "value": "value1"})
     assert variable.value == "value1"
     assert variable in group.variables.list()
 
     variable.value = "new_value1"
     variable.save()
     variable = group.variables.get(variable.key)
     assert variable.value == "new_value1"
 
     variable.delete()
-    assert variable not in group.variables.list()
 
 
 def test_project_variables(project):
     variable = project.variables.create({"key": "key1", "value": "value1"})
     assert variable.value == "value1"
     assert variable in project.variables.list()
 
     variable.value = "new_value1"
     variable.save()
     variable = project.variables.get(variable.key)
     assert variable.value == "new_value1"
 
     variable.delete()
-    assert variable not in project.variables.list()
```

### Comparing `python-gitlab-4.4.0/tests/functional/api/test_wikis.py` & `python_gitlab-4.5.0/tests/functional/api/test_wikis.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/cli/conftest.py` & `python_gitlab-4.5.0/tests/functional/cli/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,13 +32,24 @@
         "json": {"name": "name", "path": "test-path", "id": 1},
         "content_type": "application/json",
         "status": 200,
     }
 
 
 @pytest.fixture
+def resp_current_user():
+    return {
+        "method": responses.GET,
+        "url": f"{DEFAULT_URL}/api/v4/user",
+        "json": {"username": "name", "id": 1},
+        "content_type": "application/json",
+        "status": 200,
+    }
+
+
+@pytest.fixture
 def resp_delete_registry_tags_in_bulk():
     return {
         "method": responses.DELETE,
         "url": f"{DEFAULT_URL}/api/v4/projects/1/registry/repositories/1/tags",
         "status": 202,
     }
```

### Comparing `python-gitlab-4.4.0/tests/functional/cli/test_cli.py` & `python_gitlab-4.5.0/tests/functional/cli/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,30 @@
     responses.add(**resp_get_project_in_ci)
     ret = script_runner.run(["gitlab", "project", "get", "--id", "1"])
     assert ret.success
 
 
 @pytest.mark.script_launch_mode("inprocess")
 @responses.activate
+def test_does_not_auth_on_skip_login(
+    monkeypatch, script_runner, resp_get_project, resp_current_user
+):
+    monkeypatch.setenv("GITLAB_PRIVATE_TOKEN", PRIVATE_TOKEN)
+    monkeypatch.setattr(config, "_DEFAULT_FILES", [])
+
+    resp_user = responses.add(**resp_current_user)
+    resp_project = responses.add(**resp_get_project)
+    ret = script_runner.run(["gitlab", "--skip-login", "project", "get", "--id", "1"])
+    assert ret.success
+    assert resp_user.call_count == 0
+    assert resp_project.call_count == 1
+
+
+@pytest.mark.script_launch_mode("inprocess")
+@responses.activate
 def test_private_token_overrides_job_token(
     monkeypatch, script_runner, resp_get_project
 ):
     monkeypatch.setenv("GITLAB_PRIVATE_TOKEN", PRIVATE_TOKEN)
     monkeypatch.setenv("CI_JOB_TOKEN", CI_JOB_TOKEN)
 
     resp_get_project_with_token = copy.deepcopy(resp_get_project)
```

### Comparing `python-gitlab-4.4.0/tests/functional/cli/test_cli_artifacts.py` & `python_gitlab-4.5.0/tests/functional/cli/test_cli_artifacts.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/cli/test_cli_packages.py` & `python_gitlab-4.5.0/tests/functional/cli/test_cli_packages.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/cli/test_cli_projects.py` & `python_gitlab-4.5.0/tests/functional/cli/test_cli_projects.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/cli/test_cli_repository.py` & `python_gitlab-4.5.0/tests/functional/cli/test_cli_repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,17 +27,21 @@
     assert ret.success
 
 
 def test_list_all_commits(gitlab_cli, project):
     data = {
         "branch": "new-branch",
         "start_branch": "main",
-        "commit_message": "New commit on new branch",
+        "commit_message": "chore: test commit on new branch",
         "actions": [
-            {"action": "create", "file_path": "new-file", "content": "new content"}
+            {
+                "action": "create",
+                "file_path": "test-cli-repo.md",
+                "content": "new content",
+            }
         ],
     }
     commit = project.commits.create(data)
 
     cmd = ["project-commit", "list", "--project-id", project.id, "--get-all"]
     ret = gitlab_cli(cmd)
     assert commit.id not in ret.stdout
@@ -68,34 +72,38 @@
     ]
 
     ret = gitlab_cli(cmd)
     assert ret.success
     assert ret.stdout
 
 
-def test_commit_merge_requests(gitlab_cli, project, merge_request, wait_for_sidekiq):
+def test_commit_merge_requests(gitlab_cli, project, merge_request):
     """This tests the `project-commit merge-requests` command and also tests
     that we can print the result using the `json` formatter"""
-    # Merge the MR first
+
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(30)
+
     merge_result = merge_request.merge(should_remove_source_branch=True)
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
 
     # Wait until it is merged
     mr = None
     mr_iid = merge_request.iid
     for _ in range(60):
         mr = project.mergerequests.get(mr_iid)
         if mr.merged_at is not None:
             break
         time.sleep(0.5)
 
     assert mr is not None
     assert mr.merged_at is not None
-    time.sleep(0.5)
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(5)
 
     commit_sha = merge_result["sha"]
     cmd = [
         "-o",
         "json",
         "project-commit",
         "merge-requests",
```

### Comparing `python-gitlab-4.4.0/tests/functional/cli/test_cli_resource_access_tokens.py` & `python_gitlab-4.5.0/tests/functional/cli/test_cli_resource_access_tokens.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pytest
+import datetime
 
 
 def test_list_project_access_tokens(gitlab_cli, project):
     cmd = ["project-access-token", "list", "--project-id", project.id]
     ret = gitlab_cli(cmd)
 
     assert ret.success
@@ -14,21 +14,22 @@
         "create",
         "--project-id",
         project.id,
         "--name",
         "test-token",
         "--scopes",
         "api,read_repository",
+        "--expires-at",
+        datetime.date.today().isoformat(),
     ]
     ret = gitlab_cli(cmd)
 
     assert ret.success
 
 
-@pytest.mark.skip(reason="Requires GitLab 14.7")
 def test_list_group_access_tokens(gitlab_cli, group):
     cmd = ["group-access-token", "list", "--group-id", group.id]
     ret = gitlab_cli(cmd)
 
     assert ret.success
 
 
@@ -38,11 +39,13 @@
         "create",
         "--group-id",
         group.id,
         "--name",
         "test-token",
         "--scopes",
         "api,read_repository",
+        "--expires-at",
+        datetime.date.today().isoformat(),
     ]
     ret = gitlab_cli(cmd)
 
     assert ret.success
```

### Comparing `python-gitlab-4.4.0/tests/functional/cli/test_cli_v4.py` & `python_gitlab-4.5.0/tests/functional/cli/test_cli_v4.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import datetime
 import os
 import time
 
+branch = "BRANCH-cli-v4"
+
 
 def test_create_project(gitlab_cli):
     name = "test-project1"
 
     cmd = ["project", "create", "--name", name]
     ret = gitlab_cli(cmd)
 
@@ -18,36 +21,14 @@
     cmd = ["project", "update", "--id", project.id, "--description", description]
     ret = gitlab_cli(cmd)
 
     assert ret.success
     assert description in ret.stdout
 
 
-def test_create_ci_lint(gitlab_cli, valid_gitlab_ci_yml):
-    cmd = ["ci-lint", "create", "--content", valid_gitlab_ci_yml]
-    ret = gitlab_cli(cmd)
-
-    assert ret.success
-
-
-def test_validate_ci_lint(gitlab_cli, valid_gitlab_ci_yml):
-    cmd = ["ci-lint", "validate", "--content", valid_gitlab_ci_yml]
-    ret = gitlab_cli(cmd)
-
-    assert ret.success
-
-
-def test_validate_ci_lint_invalid_exits_non_zero(gitlab_cli, invalid_gitlab_ci_yml):
-    cmd = ["ci-lint", "validate", "--content", invalid_gitlab_ci_yml]
-    ret = gitlab_cli(cmd)
-
-    assert not ret.success
-    assert "CI YAML Lint failed (Invalid configuration format)" in ret.stderr
-
-
 def test_validate_project_ci_lint(gitlab_cli, project, valid_gitlab_ci_yml):
     cmd = [
         "project-ci-lint",
         "validate",
         "--project-id",
         project.id,
         "--content",
@@ -99,15 +80,15 @@
     assert group.description == description
 
 
 def test_create_user(gitlab_cli, gl):
     email = "fake@email.com"
     username = "user1"
     name = "User One"
-    password = "fakepassword"
+    password = "E4596f8be406Bc3a14a4ccdb1df80587"
 
     cmd = [
         "user",
         "create",
         "--email",
         email,
         "--username",
@@ -211,16 +192,14 @@
     ]
     ret = gitlab_cli(cmd)
 
     assert ret.success
 
 
 def test_create_branch(gitlab_cli, project):
-    branch = "branch1"
-
     cmd = [
         "project-branch",
         "create",
         "--project-id",
         project.id,
         "--branch",
         branch,
@@ -229,15 +208,14 @@
     ]
     ret = gitlab_cli(cmd)
 
     assert ret.success
 
 
 def test_create_merge_request(gitlab_cli, project):
-    branch = "branch1"
 
     cmd = [
         "project-merge-request",
         "create",
         "--project-id",
         project.id,
         "--source-branch",
@@ -248,36 +226,36 @@
         "Update README",
     ]
     ret = gitlab_cli(cmd)
 
     assert ret.success
 
 
-def test_accept_request_merge(gitlab_cli, project, wait_for_sidekiq):
+def test_accept_request_merge(gitlab_cli, project):
     # MR needs at least 1 commit before we can merge
     mr = project.mergerequests.list()[0]
     file_data = {
         "branch": mr.source_branch,
-        "file_path": "README2",
+        "file_path": "test-cli-v4.md",
         "content": "Content",
-        "commit_message": "Pre-merge commit",
+        "commit_message": "chore: test-cli-v4 change",
     }
     project.files.create(file_data)
-    time.sleep(2)
-    wait_for_sidekiq(timeout=60)
+    # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+    time.sleep(30)
 
-    cmd = [
+    approve_cmd = [
         "project-merge-request",
         "merge",
         "--project-id",
         project.id,
         "--iid",
         mr.iid,
     ]
-    ret = gitlab_cli(cmd)
+    ret = gitlab_cli(approve_cmd)
 
     assert ret.success
 
 
 def test_create_project_label(gitlab_cli, project):
     name = "prjlabel1"
     description = "prjlabel1 description"
@@ -497,17 +475,14 @@
     ]
     ret = gitlab_cli(cmd)
 
     assert ret.success
 
 
 def test_delete_branch(gitlab_cli, project):
-    # TODO: branch fixture
-    branch = "branch1"
-
     cmd = ["project-branch", "delete", "--project-id", project.id, "--name", branch]
     ret = gitlab_cli(cmd)
 
     assert ret.success
 
 
 def test_project_upload_file(gitlab_cli, project):
@@ -586,15 +561,15 @@
     assert ret.success
     assert description in ret.stdout
 
 
 def test_create_project_deploy_token(gitlab_cli, project):
     name = "project-token"
     username = "root"
-    expires_at = "2021-09-09"
+    expires_at = datetime.date.today().isoformat()
     scopes = "read_registry"
 
     cmd = [
         "-v",
         "project-deploy-token",
         "create",
         "--project-id",
@@ -662,15 +637,15 @@
     assert ret.success
     # TODO assert not in list
 
 
 def test_create_group_deploy_token(gitlab_cli, group):
     name = "group-token"
     username = "root"
-    expires_at = "2021-09-09"
+    expires_at = datetime.date.today().isoformat()
     scopes = "read_registry"
 
     cmd = [
         "-v",
         "group-deploy-token",
         "create",
         "--group-id",
```

### Comparing `python-gitlab-4.4.0/tests/functional/cli/test_cli_variables.py` & `python_gitlab-4.5.0/tests/functional/cli/test_cli_variables.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/conftest.py` & `python_gitlab-4.5.0/tests/functional/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+import datetime
 import logging
 import pathlib
 import tempfile
 import time
 import uuid
 from subprocess import check_output
 from typing import Optional
@@ -66,25 +67,23 @@
 
 
 def reset_gitlab(gl: gitlab.Gitlab) -> None:
     """Delete resources (such as projects, groups, users) that shouldn't
     exist."""
     if helpers.get_gitlab_plan(gl):
         logging.info("GitLab EE detected")
-        # NOTE(jlvillal): By default in GitLab EE it will wait 7 days before
-        # deleting a group. Disable delayed group/project deletion.
+        # NOTE(jlvillal, timknight): By default in GitLab EE it will wait 7 days before
+        # deleting a group or project.
+        # In GL 16.0 we need to call delete with `permanently_remove=True` for projects and sub groups
+        # (handled in helpers.py safe_delete)
         settings = gl.settings.get()
         modified_settings = False
-        if settings.delayed_group_deletion:
-            logging.info("Setting `delayed_group_deletion` to False")
-            settings.delayed_group_deletion = False
-            modified_settings = True
-        if settings.delayed_project_deletion:
-            logging.info("Setting `delayed_project_deletion` to False")
-            settings.delayed_project_deletion = False
+        if settings.deletion_adjourned_period != 1:
+            logging.info("Setting `deletion_adjourned_period` to 1 Day")
+            settings.deletion_adjourned_period = 1
             modified_settings = True
         if modified_settings:
             settings.save()
 
     for project in gl.projects.list():
         for deploy_token in project.deploytokens.list():
             logging.info(
@@ -118,15 +117,15 @@
         helpers.safe_delete(topic)
     for variable in gl.variables.list():
         logging.info(f"Deleting variable: {variable.key!r}")
         helpers.safe_delete(variable)
     for user in gl.users.list():
         if user.username not in ["root", "ghost"]:
             logging.info(f"Deleting user: {user.username!r}")
-            helpers.safe_delete(user, hard_delete=True)
+            helpers.safe_delete(user)
 
 
 def set_token(container: str, fixture_dir: pathlib.Path) -> str:
     logging.info("Creating API token.")
     set_token_rb = fixture_dir / "set_token.rb"
 
     with open(set_token_rb, "r", encoding="utf-8") as f:
@@ -205,39 +204,14 @@
         logging.debug(f"Sleeping for {SLEEP_TIME}")
         time.sleep(SLEEP_TIME)
         return True
 
     return _check
 
 
-@pytest.fixture
-def wait_for_sidekiq(gl):
-    """
-    Return a helper function to wait until there are no busy sidekiq processes.
-
-    Use this with asserts for slow tasks (group/project/user creation/deletion).
-    """
-
-    def _wait(timeout: int = 30, step: float = 0.5, allow_fail: bool = False) -> bool:
-        for count in range(timeout):
-            time.sleep(step)
-            busy = False
-            processes = gl.sidekiq.process_metrics()["processes"]
-            for process in processes:
-                if process["busy"]:
-                    busy = True
-            if not busy:
-                return True
-            logging.info(f"sidekiq busy {count} of {timeout}")
-        assert allow_fail, "sidekiq process should have terminated but did not."
-        return False
-
-    return _wait
-
-
 @pytest.fixture(scope="session")
 def gitlab_token(
     check_is_alive,
     gitlab_container_name: str,
     gitlab_url: str,
     docker_services,
     fixture_dir: pathlib.Path,
@@ -372,15 +346,15 @@
 
     yield project
 
     helpers.safe_delete(project)
 
 
 @pytest.fixture(scope="function")
-def make_merge_request(project, wait_for_sidekiq):
+def make_merge_request(project):
     """Fixture factory used to create a merge_request.
 
     It will create a branch, add a commit to the branch, and then create a
     merge request against project.default_branch. The MR will be returned.
 
     When finished any created merge requests and branches will be deleted.
 
@@ -392,31 +366,33 @@
     to_delete = []
 
     def _make_merge_request(*, source_branch: str, create_pipeline: bool = False):
         # Wait for processes to be done before we start...
         # NOTE(jlvillal): Sometimes the CI would give a "500 Internal Server
         # Error". Hoping that waiting until all other processes are done will
         # help with that.
-        result = wait_for_sidekiq(timeout=60)
-        assert result is True, "sidekiq process should have terminated but did not"
+        # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+        time.sleep(30)
 
         project.refresh()  # Gets us the current default branch
+        logging.info(f"Creating branch {source_branch}")
         mr_branch = project.branches.create(
             {"branch": source_branch, "ref": project.default_branch}
         )
         # NOTE(jlvillal): Must create a commit in the new branch before we can
         # create an MR that will work.
         project.files.create(
             {
                 "file_path": f"README.{source_branch}",
                 "branch": source_branch,
                 "content": "Initial content",
                 "commit_message": "New commit in new branch",
             }
         )
+
         if create_pipeline:
             project.files.create(
                 {
                     "file_path": ".gitlab-ci.yml",
                     "branch": source_branch,
                     "content": """
 test:
@@ -432,24 +408,31 @@
             {
                 "source_branch": source_branch,
                 "target_branch": project.default_branch,
                 "title": "Should remove source branch",
                 "remove_source_branch": True,
             }
         )
-        result = wait_for_sidekiq(timeout=60)
-        assert result is True, "sidekiq process should have terminated but did not"
+
+        # Pause to let GL catch up (happens on hosted too, sometimes takes a while for server to be ready to merge)
+        time.sleep(5)
 
         mr_iid = mr.iid
         for _ in range(60):
             mr = project.mergerequests.get(mr_iid)
-            if mr.merge_status != "checking":
+            if (
+                mr.detailed_merge_status == "checking"
+                or mr.detailed_merge_status == "unchecked"
+            ):
+                time.sleep(0.5)
+            else:
                 break
-            time.sleep(0.5)
-        assert mr.merge_status != "checking"
+
+        assert mr.detailed_merge_status != "checking"
+        assert mr.detailed_merge_status != "unchecked"
 
         to_delete.extend([mr, mr_branch])
         return mr
 
     yield _make_merge_request
 
     for object in to_delete:
@@ -519,22 +502,21 @@
 @pytest.fixture(scope="module")
 def user(gl):
     """User fixture for user API resource tests."""
     _id = uuid.uuid4().hex
     email = f"user{_id}@email.com"
     username = f"user{_id}"
     name = f"User {_id}"
-    password = "fakepassword"
+    password = "E4596f8be406Bc3a14a4ccdb1df80587"
 
     user = gl.users.create(email=email, username=username, name=name, password=password)
 
     yield user
 
-    # Use `hard_delete=True` or a 'Ghost User' may be created.
-    helpers.safe_delete(user, hard_delete=True)
+    helpers.safe_delete(user)
 
 
 @pytest.fixture(scope="module")
 def issue(project):
     """Issue fixture for issue API resource tests."""
     _id = uuid.uuid4().hex
     data = {"title": f"Issue {_id}", "description": f"Issue {_id} description"}
@@ -595,29 +577,29 @@
 @pytest.fixture(scope="module")
 def deploy_token(project):
     """Deploy token fixture for project deploy token API resource tests."""
     _id = uuid.uuid4().hex
     data = {
         "name": f"token-{_id}",
         "username": "root",
-        "expires_at": "2021-09-09",
+        "expires_at": datetime.date.today().isoformat(),
         "scopes": "read_registry",
     }
 
     return project.deploytokens.create(data)
 
 
 @pytest.fixture(scope="module")
 def group_deploy_token(group):
     """Deploy token fixture for group deploy token API resource tests."""
     _id = uuid.uuid4().hex
     data = {
         "name": f"group-token-{_id}",
         "username": "root",
-        "expires_at": "2021-09-09",
+        "expires_at": datetime.date.today().isoformat(),
         "scopes": "read_registry",
     }
 
     return group.deploytokens.create(data)
 
 
 @pytest.fixture(scope="session")
```

### Comparing `python-gitlab-4.4.0/tests/functional/fixtures/avatar.png` & `python_gitlab-4.5.0/tests/functional/fixtures/avatar.png`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/fixtures/create_license.rb` & `python_gitlab-4.5.0/tests/functional/fixtures/create_license.rb`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/fixtures/docker-compose.yml` & `python_gitlab-4.5.0/tests/functional/fixtures/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/functional/fixtures/docker.py` & `python_gitlab-4.5.0/tests/functional/fixtures/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 pytest-docker fixture overrides.
 See https://github.com/avast/pytest-docker#available-fixtures.
 """
+
 import pytest
 
 
 @pytest.fixture(scope="session")
 def docker_compose_project_name():
     """Set a consistent project name to enable optional reuse of containers."""
     return "pytest-python-gitlab"
```

### Comparing `python-gitlab-4.4.0/tests/smoke/test_dists.py` & `python_gitlab-4.5.0/tests/smoke/test_dists.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 
 import pytest
 
 from gitlab._version import __title__, __version__
 
 DOCS_DIR = "docs"
 TEST_DIR = "tests"
-SDIST_FILE = f"{__title__}-{__version__}.tar.gz"
-WHEEL_FILE = f"{__title__.replace('-', '_')}-{__version__}-py{sys.version_info.major}-none-any.whl"
+DIST_NORMALIZED_TITLE = f"{__title__.replace('-', '_')}-{__version__}"
+SDIST_FILE = f"{DIST_NORMALIZED_TITLE}.tar.gz"
+WHEEL_FILE = f"{DIST_NORMALIZED_TITLE}-py{sys.version_info.major}-none-any.whl"
 PY_TYPED = "gitlab/py.typed"
 
 
 @pytest.fixture(scope="session")
 def build(tmp_path_factory: pytest.TempPathFactory):
     temp_dir = tmp_path_factory.mktemp("build")
     subprocess.run([sys.executable, "-m", "build", "--outdir", temp_dir], check=True)
     return temp_dir
 
 
 def test_sdist_includes_correct_files(build: Path) -> None:
     sdist = tarfile.open(build / SDIST_FILE, "r:gz")
-    sdist_dir = f"{__title__}-{__version__}"
 
-    docs_dir = sdist.getmember(f"{sdist_dir}/{DOCS_DIR}")
-    test_dir = sdist.getmember(f"{sdist_dir}/{TEST_DIR}")
-    readme = sdist.getmember(f"{sdist_dir}/README.rst")
-    py_typed = sdist.getmember(f"{sdist_dir}/{PY_TYPED}")
+    docs_dir = sdist.getmember(f"{DIST_NORMALIZED_TITLE}/{DOCS_DIR}")
+    test_dir = sdist.getmember(f"{DIST_NORMALIZED_TITLE}/{TEST_DIR}")
+    readme = sdist.getmember(f"{DIST_NORMALIZED_TITLE}/README.rst")
+    py_typed = sdist.getmember(f"{DIST_NORMALIZED_TITLE}/{PY_TYPED}")
 
     assert docs_dir.isdir()
     assert test_dir.isdir()
     assert py_typed.isfile()
     assert readme.isfile()
```

### Comparing `python-gitlab-4.4.0/tests/unit/_backends/test_requests_backend.py` & `python_gitlab-4.5.0/tests/unit/_backends/test_requests_backend.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/base/test_rest_manager.py` & `python_gitlab-4.5.0/tests/unit/base/test_rest_manager.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/base/test_rest_object.py` & `python_gitlab-4.5.0/tests/unit/base/test_rest_object.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/conftest.py` & `python_gitlab-4.5.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/helpers.py` & `python_gitlab-4.5.0/tests/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/meta/test_ensure_type_hints.py` & `python_gitlab-4.5.0/tests/unit/meta/test_ensure_type_hints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Ensure type-hints are setup correctly and detect if missing functions.
 
 Original notes by John L. Villalovos
 
 """
+
 import dataclasses
 import functools
 import inspect
 from typing import Optional, Type
 
 import pytest
```

### Comparing `python-gitlab-4.4.0/tests/unit/meta/test_imports.py` & `python_gitlab-4.5.0/tests/unit/meta/test_imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Ensure objects defined in gitlab.v4.objects are imported in
 `gitlab/v4/objects/__init__.py`
 
 """
+
 import pkgutil
 from typing import Set
 
 import gitlab.exceptions
 import gitlab.v4.objects
```

### Comparing `python-gitlab-4.4.0/tests/unit/meta/test_mro.py` & `python_gitlab-4.5.0/tests/unit/meta/test_mro.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,46 +38,44 @@
 
   When we are type-checking it fails to understand the class Wrongv4Object
   and thus we can't type check it correctly.
 
 Almost all classes in gitlab/v4/objects/*py were already correct before this
 check was added.
 """
+
 import inspect
 
 import pytest
 
 import gitlab.v4.objects
 
 
 def test_show_issue() -> None:
     """Test case to demonstrate the TypeError that occurs"""
 
     class RESTObject:
-        def __init__(self, manager: str, attrs: int) -> None:
-            ...
+        def __init__(self, manager: str, attrs: int) -> None: ...
 
-    class Mixin(RESTObject):
-        ...
+    class Mixin(RESTObject): ...
 
     with pytest.raises(TypeError) as exc_info:
         # Wrong ordering here
         class Wrongv4Object(RESTObject, Mixin):  # type: ignore
             ...
 
     # The error message in the exception should be:
     #   TypeError: Cannot create a consistent method resolution
     #   order (MRO) for bases RESTObject, Mixin
 
     # Make sure the exception string contains "MRO"
     assert "MRO" in exc_info.exconly()
 
     # Correctly ordered class, no exception
-    class Correctv4Object(Mixin, RESTObject):
-        ...
+    class Correctv4Object(Mixin, RESTObject): ...
 
 
 def test_mros() -> None:
     """Ensure objects defined in gitlab.v4.objects have REST* as last item in
     class definition.
 
     We do this as we need to ensure the MRO (Method Resolution Order) is
```

### Comparing `python-gitlab-4.4.0/tests/unit/mixins/test_meta_mixins.py` & `python_gitlab-4.5.0/tests/unit/mixins/test_meta_mixins.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/mixins/test_mixin_methods.py` & `python_gitlab-4.5.0/tests/unit/mixins/test_mixin_methods.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/mixins/test_object_mixins_attributes.py` & `python_gitlab-4.5.0/tests/unit/mixins/test_object_mixins_attributes.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/conftest.py` & `python_gitlab-4.5.0/tests/unit/objects/conftest.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_appearance.py` & `python_gitlab-4.5.0/tests/unit/objects/test_appearance.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_applications.py` & `python_gitlab-4.5.0/tests/unit/objects/test_applications.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_audit_events.py` & `python_gitlab-4.5.0/tests/unit/objects/test_audit_events.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_badges.py` & `python_gitlab-4.5.0/tests/unit/objects/test_badges.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API: https://docs.gitlab.com/ee/api/project_badges.html
 GitLab API: https://docs.gitlab.com/ee/api/group_badges.html
 """
+
 import re
 
 import pytest
 import responses
 
 from gitlab.v4.objects import GroupBadge, ProjectBadge
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_bridges.py` & `python_gitlab-4.5.0/tests/unit/objects/test_bridges.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ee/api/jobs.html#list-pipeline-bridges
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectPipelineBridge
 
 
 @pytest.fixture
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_bulk_imports.py` & `python_gitlab-4.5.0/tests/unit/objects/test_bulk_imports.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_ci_lint.py` & `python_gitlab-4.5.0/tests/unit/objects/test_ci_lint.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_commits.py` & `python_gitlab-4.5.0/tests/unit/objects/test_commits.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_deploy_tokens.py` & `python_gitlab-4.5.0/tests/unit/objects/test_deploy_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/deploy_tokens.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectDeployToken
 
 create_content = {
     "id": 1,
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_deployments.py` & `python_gitlab-4.5.0/tests/unit/objects/test_deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/deployments.html
 """
+
 import pytest
 import responses
 
 
 @pytest.fixture
 def resp_deployment_get():
     with responses.RequestsMock() as rsps:
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_draft_notes.py` & `python_gitlab-4.5.0/tests/unit/objects/test_draft_notes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ee/api/draft_notes.html
 """
+
 from copy import deepcopy
 
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectMergeRequestDraftNote
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_environments.py` & `python_gitlab-4.5.0/tests/unit/objects/test_environments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/environments.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectEnvironment, ProjectProtectedEnvironment
 
 
 @pytest.fixture
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_group_access_tokens.py` & `python_gitlab-4.5.0/tests/unit/objects/test_group_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_groups.py` & `python_gitlab-4.5.0/tests/unit/objects/test_groups.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_invitations.py` & `python_gitlab-4.5.0/tests/unit/objects/test_invitations.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_issues.py` & `python_gitlab-4.5.0/tests/unit/objects/test_issues.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/issues.html
 """
+
 import re
 
 import pytest
 import responses
 
 from gitlab.v4.objects import (
     GroupIssuesStatistics,
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_iterations.py` & `python_gitlab-4.5.0/tests/unit/objects/test_iterations.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_job_artifacts.py` & `python_gitlab-4.5.0/tests/unit/objects/test_job_artifacts.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_jobs.py` & `python_gitlab-4.5.0/tests/unit/objects/test_todos.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,86 @@
 """
-GitLab API: https://docs.gitlab.com/ee/api/jobs.html
+GitLab API: https://docs.gitlab.com/ce/api/todos.html
 """
+
 import pytest
 import responses
 
-from gitlab.v4.objects import ProjectJob
+from gitlab.v4.objects import Todo
+
 
-job_content = {
-    "commit": {
-        "author_email": "admin@example.com",
-        "author_name": "Administrator",
-    },
-    "coverage": None,
-    "allow_failure": False,
-    "created_at": "2015-12-24T15:51:21.880Z",
-    "started_at": "2015-12-24T17:54:30.733Z",
-    "finished_at": "2015-12-24T17:54:31.198Z",
-    "duration": 0.465,
-    "queued_duration": 0.010,
-    "artifacts_expire_at": "2016-01-23T17:54:31.198Z",
-    "tag_list": ["docker runner", "macos-10.15"],
-    "id": 1,
-    "name": "rubocop",
-    "pipeline": {
-        "id": 1,
-        "project_id": 1,
-    },
-    "ref": "main",
-    "artifacts": [],
-    "runner": None,
-    "stage": "test",
-    "status": "failed",
-    "tag": False,
-    "web_url": "https://example.com/foo/bar/-/jobs/1",
-    "user": {"id": 1},
-}
+@pytest.fixture
+def json_content():
+    return [
+        {
+            "id": 102,
+            "project": {
+                "id": 2,
+                "name": "Gitlab Ce",
+                "name_with_namespace": "Gitlab Org / Gitlab Ce",
+                "path": "gitlab-ce",
+                "path_with_namespace": "gitlab-org/gitlab-ce",
+            },
+            "author": {
+                "name": "Administrator",
+                "username": "root",
+                "id": 1,
+            },
+            "action_name": "marked",
+            "target_type": "MergeRequest",
+            "target": {
+                "id": 34,
+                "iid": 7,
+                "project_id": 2,
+                "assignee": {
+                    "name": "Administrator",
+                    "username": "root",
+                    "id": 1,
+                },
+            },
+        }
+    ]
 
 
 @pytest.fixture
-def resp_get_job():
-    with responses.RequestsMock() as rsps:
+def resp_todo(json_content):
+    with responses.RequestsMock(assert_all_requests_are_fired=False) as rsps:
         rsps.add(
             method=responses.GET,
-            url="http://localhost/api/v4/projects/1/jobs/1",
-            json=job_content,
+            url="http://localhost/api/v4/todos",
+            json=json_content,
             content_type="application/json",
             status=200,
         )
-        yield rsps
-
-
-@pytest.fixture
-def resp_cancel_job():
-    with responses.RequestsMock() as rsps:
         rsps.add(
             method=responses.POST,
-            url="http://localhost/api/v4/projects/1/jobs/1/cancel",
-            json=job_content,
+            url="http://localhost/api/v4/todos/102/mark_as_done",
+            json=json_content[0],
             content_type="application/json",
-            status=201,
+            status=200,
         )
         yield rsps
 
 
 @pytest.fixture
-def resp_retry_job():
+def resp_mark_all_as_done():
     with responses.RequestsMock() as rsps:
         rsps.add(
             method=responses.POST,
-            url="http://localhost/api/v4/projects/1/jobs/1/retry",
-            json=job_content,
-            content_type="application/json",
-            status=201,
+            url="http://localhost/api/v4/todos/mark_as_done",
+            status=204,
         )
         yield rsps
 
 
-def test_get_project_job(project, resp_get_job):
-    job = project.jobs.get(1)
-    assert isinstance(job, ProjectJob)
-    assert job.ref == "main"
-
-
-def test_cancel_project_job(project, resp_cancel_job):
-    job = project.jobs.get(1, lazy=True)
-
-    output = job.cancel()
-    assert output["ref"] == "main"
+def test_todo(gl, resp_todo):
+    todo = gl.todos.list()[0]
+    assert isinstance(todo, Todo)
+    assert todo.id == 102
+    assert todo.target_type == "MergeRequest"
+    assert todo.target["assignee"]["username"] == "root"
 
+    todo.mark_as_done()
 
-def test_retry_project_job(project, resp_retry_job):
-    job = project.jobs.get(1, lazy=True)
 
-    output = job.retry()
-    assert output["ref"] == "main"
+def test_todo_mark_all_as_done(gl, resp_mark_all_as_done):
+    gl.todos.mark_all_as_done()
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_keys.py` & `python_gitlab-4.5.0/tests/unit/objects/test_keys.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/keys.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import Key
 
 key_content = {"id": 1, "title": "title", "key": "ssh-keytype AAAAC3Nza/key comment"}
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_members.py` & `python_gitlab-4.5.0/tests/unit/objects/test_members.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ee/api/members.html
 """
+
 import pytest
 import responses
 
 from gitlab.const import AccessLevel
 from gitlab.v4.objects import GroupBillableMember
 
 billable_members_content = [
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_merge_request_pipelines.py` & `python_gitlab-4.5.0/tests/unit/objects/test_merge_request_pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ee/api/merge_requests.html#list-mr-pipelines
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectMergeRequestPipeline
 
 pipeline_content = {
     "id": 1,
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_merge_requests.py` & `python_gitlab-4.5.0/tests/unit/objects/test_merge_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API:
 https://docs.gitlab.com/ce/api/merge_requests.html
 https://docs.gitlab.com/ee/api/deployments.html#list-of-merge-requests-associated-with-a-deployment
 """
+
 import re
 
 import pytest
 import responses
 
 from gitlab.v4.objects import (
     ProjectDeploymentMergeRequest,
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_merge_trains.py` & `python_gitlab-4.5.0/tests/unit/objects/test_merge_trains.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/merge_trains.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectMergeTrain
 
 mr_content = {
     "id": 110,
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_packages.py` & `python_gitlab-4.5.0/tests/unit/objects/test_packages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/packages.html
 """
+
 import re
 
 import pytest
 import responses
 
 from gitlab import exceptions as exc
 from gitlab.v4.objects import (
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_personal_access_tokens.py` & `python_gitlab-4.5.0/tests/unit/objects/test_personal_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_pipeline_schedules.py` & `python_gitlab-4.5.0/tests/unit/objects/test_pipeline_schedules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/pipeline_schedules.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectPipelineSchedulePipeline
 
 pipeline_content = {
     "id": 48,
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_pipelines.py` & `python_gitlab-4.5.0/tests/unit/objects/test_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ee/api/pipelines.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import (
     ProjectPipeline,
     ProjectPipelineTestReport,
     ProjectPipelineTestReportSummary,
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_project_access_tokens.py` & `python_gitlab-4.5.0/tests/unit/objects/test_project_access_tokens.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_project_import_export.py` & `python_gitlab-4.5.0/tests/unit/objects/test_project_import_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/project_import_export.html
 """
+
 import pytest
 import responses
 
 
 @pytest.fixture
 def resp_import_project():
     content = {
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_project_merge_request_approvals.py` & `python_gitlab-4.5.0/tests/unit/objects/test_project_merge_request_approvals.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pytest
 import responses
 
 import gitlab
 from gitlab.mixins import UpdateMethod
 
-approval_rule_id = 1
+approval_rule_id = 7
 approval_rule_name = "security"
 approvals_required = 3
 user_ids = [5, 50]
 group_ids = [5]
 
 new_approval_rule_name = "new approval rule"
 new_approval_rule_user_ids = user_ids
@@ -92,71 +92,71 @@
         "approval_rules_overwritten": False,
         "rules": approval_state_rules,
     }
 
     with responses.RequestsMock(assert_all_requests_are_fired=False) as rsps:
         rsps.add(
             method=responses.GET,
-            url="http://localhost/api/v4/projects/1/merge_requests/1/approval_rules",
+            url="http://localhost/api/v4/projects/1/merge_requests/3/approval_rules",
             json=mr_ars_content,
             content_type="application/json",
             status=200,
         )
         rsps.add(
             method=responses.GET,
-            url="http://localhost/api/v4/projects/1/merge_requests/1/approval_rules/1",
+            url="http://localhost/api/v4/projects/1/merge_requests/3/approval_rules/7",
             json=mr_ars_content[0],
             content_type="application/json",
             status=200,
         )
         rsps.add(
             method=responses.GET,
-            url="http://localhost/api/v4/projects/1/merge_requests/1/approval_state",
+            url="http://localhost/api/v4/projects/1/merge_requests/3/approval_state",
             json=mr_approval_state_content,
             content_type="application/json",
             status=200,
         )
 
         new_mr_ars_content = dict(mr_ars_content[0])
         new_mr_ars_content["name"] = new_approval_rule_name
         new_mr_ars_content["approvals_required"] = new_approval_rule_approvals_required
 
         rsps.add(
             method=responses.POST,
-            url="http://localhost/api/v4/projects/1/merge_requests/1/approval_rules",
+            url="http://localhost/api/v4/projects/1/merge_requests/3/approval_rules",
             json=new_mr_ars_content,
             content_type="application/json",
             status=200,
         )
 
         updated_mr_ars_content = copy.deepcopy(mr_ars_content[0])
         updated_mr_ars_content["eligible_approvers"] = [
             mr_ars_content[0]["eligible_approvers"][0]
         ]
 
-        updated_mr_ars_content[
-            "approvals_required"
-        ] = updated_approval_rule_approvals_required
+        updated_mr_ars_content["approvals_required"] = (
+            updated_approval_rule_approvals_required
+        )
 
         rsps.add(
             method=responses.PUT,
-            url="http://localhost/api/v4/projects/1/merge_requests/1/approval_rules/1",
+            url="http://localhost/api/v4/projects/1/merge_requests/3/approval_rules/7",
             json=updated_mr_ars_content,
             content_type="application/json",
             status=200,
         )
         yield rsps
 
 
 @pytest.fixture
 def resp_delete_mr_approval_rule():
     with responses.RequestsMock() as rsps:
         rsps.add(
             method=responses.DELETE,
-            url="http://localhost/api/v4/projects/1/merge_requests/1/approval_rules/1",
+            url="http://localhost/api/v4/projects/1/merge_requests/3/approval_rules/7",
             status=204,
         )
         yield rsps
 
 
 def test_project_approval_manager_update_method_post(project):
     """Ensure the
@@ -166,28 +166,28 @@
     assert isinstance(
         approvals, gitlab.v4.objects.merge_request_approvals.ProjectApprovalManager
     )
     assert approvals._update_method is UpdateMethod.POST
 
 
 def test_list_merge_request_approval_rules(project, resp_mr_approval_rules):
-    approval_rules = project.mergerequests.get(1, lazy=True).approval_rules.list()
+    approval_rules = project.mergerequests.get(3, lazy=True).approval_rules.list()
     assert len(approval_rules) == 1
     assert approval_rules[0].name == approval_rule_name
     assert approval_rules[0].id == approval_rule_id
     repr(approval_rules)  # ensure that `repr()` doesn't raise an exception
 
 
 def test_delete_merge_request_approval_rule(project, resp_delete_mr_approval_rule):
-    merge_request = project.mergerequests.get(1, lazy=True)
+    merge_request = project.mergerequests.get(3, lazy=True)
     merge_request.approval_rules.delete(approval_rule_id)
 
 
 def test_update_merge_request_approvals_set_approvers(project, resp_mr_approval_rules):
-    approvals = project.mergerequests.get(1, lazy=True).approvals
+    approvals = project.mergerequests.get(3, lazy=True).approvals
     assert isinstance(
         approvals,
         gitlab.v4.objects.merge_request_approvals.ProjectMergeRequestApprovalManager,
     )
     assert approvals._update_method is UpdateMethod.POST
     response = approvals.set_approvers(
         updated_approval_rule_approvals_required,
@@ -199,15 +199,15 @@
     assert response.approvals_required == updated_approval_rule_approvals_required
     assert len(response.eligible_approvers) == len(updated_approval_rule_user_ids)
     assert response.eligible_approvers[0]["id"] == updated_approval_rule_user_ids[0]
     assert response.name == approval_rule_name
 
 
 def test_create_merge_request_approvals_set_approvers(project, resp_mr_approval_rules):
-    approvals = project.mergerequests.get(1, lazy=True).approvals
+    approvals = project.mergerequests.get(3, lazy=True).approvals
     assert isinstance(
         approvals,
         gitlab.v4.objects.merge_request_approvals.ProjectMergeRequestApprovalManager,
     )
     assert approvals._update_method is UpdateMethod.POST
     response = approvals.set_approvers(
         new_approval_rule_approvals_required,
@@ -218,15 +218,15 @@
     assert response.approvals_required == new_approval_rule_approvals_required
     assert len(response.eligible_approvers) == len(new_approval_rule_user_ids)
     assert response.eligible_approvers[0]["id"] == new_approval_rule_user_ids[0]
     assert response.name == new_approval_rule_name
 
 
 def test_create_merge_request_approval_rule(project, resp_mr_approval_rules):
-    approval_rules = project.mergerequests.get(1, lazy=True).approval_rules
+    approval_rules = project.mergerequests.get(3, lazy=True).approval_rules
     data = {
         "name": new_approval_rule_name,
         "approvals_required": new_approval_rule_approvals_required,
         "rule_type": "regular",
         "user_ids": new_approval_rule_user_ids,
         "group_ids": group_ids,
     }
@@ -234,38 +234,38 @@
     assert response.approvals_required == new_approval_rule_approvals_required
     assert len(response.eligible_approvers) == len(new_approval_rule_user_ids)
     assert response.eligible_approvers[0]["id"] == new_approval_rule_user_ids[0]
     assert response.name == new_approval_rule_name
 
 
 def test_update_merge_request_approval_rule(project, resp_mr_approval_rules):
-    approval_rules = project.mergerequests.get(1, lazy=True).approval_rules
+    approval_rules = project.mergerequests.get(3, lazy=True).approval_rules
     ar_1 = approval_rules.list()[0]
     ar_1.user_ids = updated_approval_rule_user_ids
     ar_1.approvals_required = updated_approval_rule_approvals_required
     ar_1.save()
 
     assert ar_1.approvals_required == updated_approval_rule_approvals_required
     assert len(ar_1.eligible_approvers) == len(updated_approval_rule_user_ids)
     assert ar_1.eligible_approvers[0]["id"] == updated_approval_rule_user_ids[0]
 
 
 def test_get_merge_request_approval_rule(project, resp_mr_approval_rules):
-    merge_request = project.mergerequests.get(1, lazy=True)
+    merge_request = project.mergerequests.get(3, lazy=True)
     approval_rule = merge_request.approval_rules.get(approval_rule_id)
     assert isinstance(
         approval_rule,
         gitlab.v4.objects.merge_request_approvals.ProjectMergeRequestApprovalRule,
     )
     assert approval_rule.name == approval_rule_name
     assert approval_rule.id == approval_rule_id
 
 
 def test_get_merge_request_approval_state(project, resp_mr_approval_rules):
-    merge_request = project.mergerequests.get(1, lazy=True)
+    merge_request = project.mergerequests.get(3, lazy=True)
     approval_state = merge_request.approval_state.get()
     assert isinstance(
         approval_state,
         gitlab.v4.objects.merge_request_approvals.ProjectMergeRequestApprovalState,
     )
     assert not approval_state.approval_rules_overwritten
     assert len(approval_state.rules) == 1
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_project_statistics.py` & `python_gitlab-4.5.0/tests/unit/objects/test_project_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/project_statistics.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectAdditionalStatistics
 
 
 @pytest.fixture
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_projects.py` & `python_gitlab-4.5.0/tests/unit/objects/test_projects.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_registry_repositories.py` & `python_gitlab-4.5.0/tests/unit/objects/test_registry_repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ee/api/container_registry.html
 """
+
 import re
 
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectRegistryRepository, RegistryRepository
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_releases.py` & `python_gitlab-4.5.0/tests/unit/objects/test_releases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/releases/index.html
 https://docs.gitlab.com/ee/api/releases/links.html
 """
+
 import re
 
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectReleaseLink
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_remote_mirrors.py` & `python_gitlab-4.5.0/tests/unit/objects/test_remote_mirrors.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_repositories.py` & `python_gitlab-4.5.0/tests/unit/objects/test_repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/repositories.html
 https://docs.gitlab.com/ee/api/repository_files.html
 """
+
 from urllib.parse import quote
 
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectFile
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_resource_groups.py` & `python_gitlab-4.5.0/tests/unit/objects/test_resource_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 GitLab API:
 https://docs.gitlab.com/ee/api/resource_groups.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import ProjectResourceGroup, ProjectResourceGroupUpcomingJob
 
-from .test_jobs import job_content
+from .test_jobs import failed_job_content
 
 resource_group_content = {
     "id": 3,
     "key": "production",
     "process_mode": "unordered",
     "created_at": "2021-09-01T08:04:59.650Z",
     "updated_at": "2021-09-01T08:04:59.650Z",
@@ -46,15 +47,15 @@
 
 @pytest.fixture
 def resp_list_upcoming_jobs():
     with responses.RequestsMock() as rsps:
         rsps.add(
             method=responses.GET,
             url="http://localhost/api/v4/projects/1/resource_groups/production/upcoming_jobs",
-            json=[job_content],
+            json=[failed_job_content],
             content_type="application/json",
             status=200,
         )
         yield rsps
 
 
 def test_list_project_resource_groups(project, resp_list_resource_groups):
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_resource_iteration_events.py` & `python_gitlab-4.5.0/tests/unit/objects/test_resource_iteration_events.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_resource_label_events.py` & `python_gitlab-4.5.0/tests/unit/objects/test_resource_label_events.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_resource_milestone_events.py` & `python_gitlab-4.5.0/tests/unit/objects/test_resource_milestone_events.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_resource_state_events.py` & `python_gitlab-4.5.0/tests/unit/objects/test_resource_state_events.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_runners.py` & `python_gitlab-4.5.0/tests/unit/objects/test_runners.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_secure_files.py` & `python_gitlab-4.5.0/tests/unit/objects/test_secure_files.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_services.py` & `python_gitlab-4.5.0/tests/unit/objects/test_services.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_snippets.py` & `python_gitlab-4.5.0/tests/unit/objects/test_snippets.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_statistics.py` & `python_gitlab-4.5.0/tests/unit/objects/test_statistics.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_submodules.py` & `python_gitlab-4.5.0/tests/unit/objects/test_submodules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GitLab API: https://docs.gitlab.com/ce/api/repository_submodules.html
 """
+
 import pytest
 import responses
 
 
 @pytest.fixture
 def resp_update_submodule():
     content = {
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_topics.py` & `python_gitlab-4.5.0/tests/unit/objects/test_topics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 GitLab API:
 https://docs.gitlab.com/ce/api/topics.html
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import Topic
 
 name = "GitLab"
 topic_title = "topic title"
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_users.py` & `python_gitlab-4.5.0/tests/unit/objects/test_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 GitLab API:
 https://docs.gitlab.com/ce/api/users.html
 https://docs.gitlab.com/ee/api/projects.html#list-projects-starred-by-a-user
 """
+
 import pytest
 import responses
 
 from gitlab.v4.objects import StarredProject, User, UserMembership, UserStatus
 
 from .test_projects import project_content
```

### Comparing `python-gitlab-4.4.0/tests/unit/objects/test_variables.py` & `python_gitlab-4.5.0/tests/unit/objects/test_variables.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/test_config.py` & `python_gitlab-4.5.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/test_exceptions.py` & `python_gitlab-4.5.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/test_gitlab.py` & `python_gitlab-4.5.0/tests/unit/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/test_gitlab_auth.py` & `python_gitlab-4.5.0/tests/unit/test_gitlab_auth.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/test_gitlab_http_methods.py` & `python_gitlab-4.5.0/tests/unit/test_gitlab_http_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,14 +596,15 @@
         result = gl.http_list("/projects", iterator=False)
     assert len(caught_warnings) == 1
     warning = caught_warnings[0]
     assert isinstance(warning.message, UserWarning)
     message = str(warning.message)
     assert "Calling a `list()` method" in message
     assert "python-gitlab.readthedocs.io" in message
+    assert __file__ in message
     assert __file__ == warning.filename
     assert isinstance(result, list)
     assert len(result) == 20
     assert len(responses.calls) == 1
 
 
 @responses.activate
```

### Comparing `python-gitlab-4.4.0/tests/unit/test_types.py` & `python_gitlab-4.5.0/tests/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tests/unit/test_utils.py` & `python_gitlab-4.5.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-gitlab-4.4.0/tox.ini` & `python_gitlab-4.5.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 [tox]
-minversion = 1.6
+minversion = 4.0
 skipsdist = True
 skip_missing_interpreters = True
-envlist = py311,py310,py39,py38,flake8,black,twine-check,mypy,isort,cz,pylint
+envlist = py313,py312,py311,py310,py39,py38,black,isort,flake8,mypy,twine-check,cz,pylint
+
+# NOTE(jlvillal): To use a label use the `-m` flag.
+# For example to run the `func` label group of environments do:
+#   tox -m func
+labels =
+    lint = black,isort,flake8,mypy,pylint,cz
+    unit = py313,py312,py311,py310,py39,py38
+# func is the functional tests. This is very time consuming.
+    func = cli_func_v4,api_func_v4
 
 [testenv]
 passenv =
   DOCKER_HOST
   FORCE_COLOR
   GITHUB_ACTIONS
   GITHUB_WORKSPACE
@@ -76,16 +85,18 @@
 
 [flake8]
 exclude = .git,.venv,.tox,dist,doc,*egg,build,
 max-line-length = 88
 # We ignore the following because we use black to handle code-formatting
 # E203: Whitespace before ':'
 # E501: Line too long
+# E701: multiple statements on one line (colon)
+# E704: multiple statements on one line (def)
 # W503: Line break occurred before a binary operator
-ignore = E203,E501,W503
+extend-ignore = E203,E501,E701,E704,W503
 per-file-ignores =
     gitlab/v4/objects/__init__.py:F401,F403
 
 [testenv:docs]
 deps = -r{toxinidir}/requirements-docs.txt
 commands = sphinx-build -n -W --keep-going -b html docs build/sphinx/html
```

