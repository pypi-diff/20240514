# Comparing `tmp/juntagrico_assignment_request-1.5.0.tar.gz` & `tmp/juntagrico-assignment-request-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juntagrico_assignment_request-1.5.0.tar", last modified: Tue Feb  8 17:04:06 2022, max compression
+gzip compressed data, was "juntagrico-assignment-request-1.6.0.tar", last modified: Mon Jan  8 05:23:52 2024, max compression
```

## Comparing `juntagrico_assignment_request-1.5.0.tar` & `juntagrico-assignment-request-1.6.0.tar`

### file list

```diff
@@ -1,64 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.054573 juntagrico_assignment_request-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6135 2022-02-08 17:04:06.054573 juntagrico_assignment_request-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4602 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.046573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.046573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/admins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/admins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/admins/assignment_request_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.046573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/dao/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/dao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/dao/assignmentrequestdao.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.050573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/entity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7888 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/entity/assignment_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     2810 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/juntagricoapp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.050573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/mailer/
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/mailer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/mailer/adminnotification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/mailer/membernotification.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.050573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3229 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.038573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.050573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/
--rwxr-xr-x   0 runner    (1001) docker     (121)      772 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/edit_assignment_request.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     3706 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/list_assignment_requests.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.054573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/confirmed_assignment_request_mail.txt
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/edited_assignment_request_mail.txt
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/new_assignment_request_mail.txt
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/notify_original_approver_mail.txt
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/rejected_assignment_request_mail.txt
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/responded_assignment_request_mail.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.054573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/snippets/assignment_request_summary.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.054573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/menu/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/menu/assignment_request_admin_menu.html
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/menu/assignment_request_user_menu.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     4249 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/request_assignment.html
--rwxr-xr-x   0 runner    (1001) docker     (121)      805 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/respond_assignment_request.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.054573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templatetags/assignment_request_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5949 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 17:04:06.046573 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6135 2022-02-08 17:04:04.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-02-08 17:04:06.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 17:04:04.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-08 17:04:04.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-02-08 17:04:04.000000 juntagrico_assignment_request-1.5.0/juntagrico_assignment_request.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-02-08 17:04:06.058573 juntagrico_assignment_request-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-02-08 17:03:53.000000 juntagrico_assignment_request-1.5.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.581544 juntagrico-assignment-request-1.6.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7651 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      228 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/MANIFEST.in
+-rw-r--r--   0 dave      (1000) dave      (1000)    14762 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4602 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/README.md
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.569543 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/
+-rw-rw-r--   0 dave      (1000) dave      (1000)       22 2024-01-08 05:23:29.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2024-01-08 05:07:34.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admin.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.569543 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admins/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admins/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1480 2024-01-08 05:07:34.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admins/assignment_request_admin.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1723 2024-01-08 05:08:09.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/apps.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2770 2024-01-08 05:04:55.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/forms.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1718 2024-01-08 05:07:34.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/hack.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.573544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      696 2024-01-08 03:15:40.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1656 2024-01-08 04:43:28.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/adminnotification.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1105 2024-01-08 04:43:28.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/membernotification.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.573544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2587 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1676 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3229 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      775 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     8794 2024-01-08 04:25:20.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/models.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.565543 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.573544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/
+-rwxrwxr-x   0 dave      (1000) dave      (1000)      772 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/edit.html
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     3750 2024-01-08 03:55:44.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/list.html
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.565543 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      900 2024-01-08 04:07:56.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/edited.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      910 2024-01-08 04:07:56.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/new.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      794 2024-01-08 04:08:44.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/notify_original_approver.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      603 2024-01-08 04:08:44.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/confirmed.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      733 2024-01-08 04:08:45.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/rejected.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      652 2024-01-08 04:07:56.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/responded.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/snippets/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      310 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/snippets/summary.txt
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     4265 2024-01-08 03:54:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/request.html
+-rwxrwxr-x   0 dave      (1000) dave      (1000)      805 2024-01-08 02:40:58.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/respond.html
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/menu/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      422 2024-01-08 04:47:19.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/menu/admin_menu.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)      496 2024-01-08 04:52:43.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/menu/user_menu.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)      910 2024-01-08 03:59:41.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/urls.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      570 2024-01-08 03:15:40.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/utils.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5577 2024-01-08 05:04:55.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/views.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-01-08 05:23:52.577544 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/
+-rw-r--r--   0 dave      (1000) dave      (1000)    14762 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2316 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       21 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       30 2024-01-08 05:23:52.000000 juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1470 2024-01-08 05:16:43.000000 juntagrico-assignment-request-1.6.0/pyproject.toml
+-rw-rw-r--   0 dave      (1000) dave      (1000)       42 2024-01-08 05:22:32.000000 juntagrico-assignment-request-1.6.0/requirements.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2024-01-08 05:23:52.581544 juntagrico-assignment-request-1.6.0/setup.cfg
```

### Comparing `juntagrico_assignment_request-1.5.0/LICENSE` & `juntagrico-assignment-request-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `juntagrico_assignment_request-1.5.0/README.md` & `juntagrico-assignment-request-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/admins/assignment_request_admin.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/admins/assignment_request_admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from django.forms import ModelForm, URLField
 from django.urls import reverse
 
 from juntagrico.admins import BaseAdmin
 from juntagrico.util.admin import MyHTMLWidget
 from juntagrico.config import Config
 
-from juntagrico_assignment_request.dao.assignmentrequestdao import AssignmentRequestDao
-from juntagrico_assignment_request.entity.assignment_request import AssignmentRequest
+from juntagrico_assignment_request.models import AssignmentRequest
+from juntagrico_assignment_request.utils import all_approvers
 
 
 class AssignmentRequestAdminForm(ModelForm):
     class Meta:
         model = AssignmentRequest
         fields = '__all__'
 
     def __init__(self, *a, **k):
         super().__init__(*a, **k)
-        self.fields['approver'].queryset = AssignmentRequestDao.all_approvers()
+        self.fields['approver'].queryset = all_approvers()
         instance = k.get('instance')
         self.fields['assignment_link'].initial = self.get_assignment_link(instance)
 
     @staticmethod
     def get_assignment_link(instance):
         if instance is None:
             return ''
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/entity/assignment_request.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,35 @@
-from datetime import datetime, date
+from datetime import datetime, date, time as datetime_time
 import time
 
 from django.db import models
+from django.db.models import Q
+from django.utils.timezone import get_default_timezone
 from django.utils.translation import gettext as _
 from django.core.validators import MinValueValidator
 from juntagrico.entity.location import Location
 
 from juntagrico.entity.member import Member
 from juntagrico.entity.jobs import Assignment, ActivityArea, JobType, RecuringJob
 
 from juntagrico.config import Config
+from juntagrico.util.temporal import start_of_business_year
+
+
+class AssignmentQueryset(models.QuerySet):
+    def pending(self):
+        # assignment requests that have not been replied yet or ar from the current business year
+        start = datetime.combine(start_of_business_year(), datetime_time.min, tzinfo=get_default_timezone())
+        return self.filter(Q(status=AssignmentRequest.REQUESTED) | Q(job_time__gte=start))
+
+    def for_approver(self, member):
+        # assignment requests that are requested to this member
+        if member.user.has_perm('juntagrico_assignment_request.notified_on_unapproved_assignments'):
+            return self.filter(Q(approver=member) | Q(approver__isnull=True))
+        return self.filter(approver=member)
 
 
 class AssignmentRequest(models.Model):
     """
     A request to get an assignment
     """
 
@@ -58,14 +74,16 @@
                                 help_text=_("Optional"))
 
     status = models.CharField(max_length=2, choices=REQUEST_STATUS, default=REQUESTED,
                               help_text=_('Hier "Bestätigt" auswählen, um die Anfrage anzunehmen'))
     response = models.TextField(_('Antwort'), blank=True, null=True,
                                 help_text=_("Rückmeldung an " + Config.vocabulary('member') + ". Kann leer bleiben."))
 
+    objects = AssignmentQueryset.as_manager()
+
     def __str__(self):
         return _('%s Anfrage #%s') % (Config.vocabulary('assignment'), self.id)
 
     def is_confirmed(self):
         return self.status == self.CONFIRMED
 
     def is_rejected(self):
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/forms.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from django.forms import ModelForm
 from django.utils.translation import gettext_lazy as _
 from django.utils.translation import gettext
 from django.urls import reverse
 
-from juntagrico_assignment_request.dao.assignmentrequestdao import AssignmentRequestDao
-from juntagrico_assignment_request.models import AssignmentRequest
-
 from crispy_forms.helper import FormHelper
 from crispy_forms.layout import Layout, Submit, HTML
 from crispy_forms.bootstrap import FormActions
 
+from juntagrico_assignment_request.models import AssignmentRequest
+from juntagrico_assignment_request.utils import all_approvers
+
 
 class AssignmentRequestForm(ModelForm):
     class Meta:
         model = AssignmentRequest
         fields = ('job_time', 'amount', 'duration', 'approver',
                   'activityarea', 'location', 'description')
         labels = {
             "amount": _("Anzahl Einsätze"),
             "approver": _("Abgesprochen mit"),
             "activityarea": _("Tätigkeitsbereich"),
         }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.fields['approver'].queryset = AssignmentRequestDao.all_approvers()
+        self.fields['approver'].queryset = all_approvers()
         self.fields['amount'].widget.attrs['min'] = 1
         self.fields['job_time'].widget.format = '%d.%m.%Y %H:%M'
         self.fields['job_time'].widget.attrs['placeholder'] = _('TT.MM.JJJJ HH:MM')
         self.helper = FormHelper()
         self.helper.form_class = 'form-horizontal'
         self.helper.label_class = 'col-md-3'
         self.helper.field_class = 'col-md-9'
@@ -59,10 +59,10 @@
         self.helper.field_class = 'col-md-9'
         self.helper.layout = Layout(
             'amount', 'duration', 'activityarea', 'location', 'response',
             FormActions(
                 Submit('confirm', _('Bestätigen'), css_class='btn-success'),
                 Submit('reject', _('Ablehnen'), css_class='btn-danger'),
                 Submit('submit', _('Nur Antwort senden'), css_class='btn-warning'),
-                HTML('<a href="' + reverse('ar-list-assignment-requests') + '" class="btn">' + gettext("Abbrechen") + '</a>'),
+                HTML('<a href="' + reverse('juntagrico-assignment-request:list') + '" class="btn">' + gettext("Abbrechen") + '</a>'),
             )
         )
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/mailer/__init__.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from juntagrico.config import Config
 
-from juntagrico_assignment_request.dao.assignmentrequestdao import AssignmentRequestDao
+from juntagrico_assignment_request.utils import all_notified_on_unapproved_assignments
 
 '''
 Server generated Emails
 '''
 
 
 def get_approver_emails(assignment_request):
     receivers = []
     if assignment_request.approver:
         # Notify approver if defined
         receivers.append(assignment_request.approver.email)
     else:
         # Otherwise inform all that should be notified on unapproved assignments
-        for notified in AssignmentRequestDao.all_notified_on_unapproved_assignments():
+        for notified in all_notified_on_unapproved_assignments():
             receivers.append(notified.email)
     if not receivers:
         # Nobody? Send it to the info mail then
         receivers.append(Config.info_email())
     return receivers
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/mailer/adminnotification.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/adminnotification.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from django.template.loader import get_template
 
 from juntagrico.mailer import EmailSender, base_dict
 from juntagrico.config import Config
 
 from juntagrico_assignment_request.mailer import get_approver_emails
-from juntagrico_assignment_request.config import AssignmentRequestConfig
 
 
 def content_render(assignment_request, template, **kwargs):
     kwargs.update({'assignment_request': assignment_request})
     d = base_dict(kwargs)
-    plaintext = get_template(AssignmentRequestConfig.emails(template))
+    plaintext = get_template('assignment_request/mails/admin/' + template + '.txt')
     return plaintext.render(d)
 
 
 def request_created(assignment_request):
     EmailSender.get_sender(Config.organisation_name() + ' - Neue ' + Config.vocabulary('assignment') + '-Anfrage',
-                           content_render(assignment_request, 'new_assignment_request_mail'))\
+                           content_render(assignment_request, 'new'))\
         .send_to(get_approver_emails(assignment_request))
 
 
 def request_handled_by_other_approver(assignment_request, new_approver):
     """
     notify original approver, if another approver handled the request
     """
     if assignment_request.approver and assignment_request.approver != new_approver:
         EmailSender.get_sender(Config.organisation_name() + ' - ' + Config.vocabulary('assignment') + '-Anfrage erledigt',
-                               content_render(assignment_request, 'notify_original_approver_mail',
+                               content_render(assignment_request, 'notify_original_approver',
                                               new_approver=new_approver))\
             .send_to(get_approver_emails(assignment_request))
 
 
 def request_changed(assignment_request):
     EmailSender.get_sender(Config.organisation_name() + ' - ' + Config.vocabulary('assignment') + '-Anfrage bearbeitet',
-                           content_render(assignment_request, 'edited_assignment_request_mail'))\
+                           content_render(assignment_request, 'edited'))\
         .send_to(get_approver_emails(assignment_request))
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/mailer/membernotification.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/mailer/membernotification.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from django.utils.translation import gettext as _
 from django.template.loader import get_template
 
 from juntagrico.mailer import EmailSender, base_dict
 from juntagrico.config import Config
 
-from juntagrico_assignment_request.config import AssignmentRequestConfig
-
 
 def request_handled(assignment_request):
     d = base_dict({'assignment_request': assignment_request})
 
     if assignment_request.is_confirmed():
         subject = _('{} bestätigt').format(Config.vocabulary('assignment'))
-        content = get_template(AssignmentRequestConfig.emails('confirmed_assignment_request_mail')).render(d)
+        content = get_template('assignment_request/mails/member/confirmed.txt').render(d)
     elif assignment_request.is_rejected():
         subject = _('{} nicht bestätigt').format(Config.vocabulary('assignment'))
-        content = get_template(AssignmentRequestConfig.emails('rejected_assignment_request_mail')).render(d)
+        content = get_template('assignment_request/mails/member/rejected.txt').render(d)
     else:
         subject = _('Rückfrage zu deinem/r {}').format(Config.vocabulary('assignment'))
-        content = get_template(AssignmentRequestConfig.emails('responded_assignment_request_mail')).render(d)
+        content = get_template('assignment_request/mails/member/responded.txt').render(d)
 
     EmailSender.get_sender(Config.organisation_name() + ' - ' + subject, content,
                            reply_to=[assignment_request.approver.email]).send_to(assignment_request.member.email)
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py`

 * *Files identical despite different names*

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py`

 * *Files identical despite different names*

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py`

 * *Files identical despite different names*

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py`

 * *Files identical despite different names*

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/models.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/hack.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from django.db.models import signals
-from juntagrico.entity.jobs import JobType, Assignment, RecuringJob
+from juntagrico_assignment_request.models import AssignmentRequest
 
-from juntagrico_assignment_request.entity.assignment_request import AssignmentRequest
-
-signals.pre_save.connect(AssignmentRequest.pre_save, sender=AssignmentRequest)
+"""
+This hack ensures that the jobs from assignment request can not be manipulated.
+In the future juntagrico should offer ways to create custom job models in addons and make this hack obsolete.
+"""
 
 
 def bulk_save(elements):
     for element in elements:
         element.save()
         print(f'Resaved {element}')
 
@@ -40,12 +40,7 @@
     """
     if hasattr(instance, 'assignmentrequest'):
         ar = instance.assignmentrequest
         instance.member = ar.member
         instance.amount = ar.get_amount()
         instance.job = ar.get_matching_job()
         print(f'restored {instance} using {ar}')
-
-
-signals.post_save.connect(post_save_job_type, sender=JobType)
-signals.post_save.connect(post_save_recuringjob, sender=RecuringJob)
-signals.pre_save.connect(pre_save_assignment, sender=Assignment)
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/edit_assignment_request.html` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/edit.html`

 * *Files identical despite different names*

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/list_assignment_requests.html` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/list.html`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             {% endif %}
         </h3>
     </div>
 {% endblock %}
 {% block content %}
     {% if archive %}
     <div class="col-md-12 mb-4">
-        <a href="{% url 'ar-list-assignment-requests' %}">{% trans "Zurück zu den offenen Anfragen" %}</a>
+        <a href="{% url 'juntagrico-assignment-request:list' %}">{% trans "Zurück zu den offenen Anfragen" %}</a>
     </div>
     {% endif %}
     <div class="col-md-12 mb-4">
         {% if assignment_requests %}
         <table id="filter-table" class="list table" style="display: table;">
             <thead>
                 <tr>
@@ -58,15 +58,15 @@
                                 <a href="{% url 'job' assignment_request.assignment.job.id %}">{{ assignment_request.get_status_display }}</a>
                             {% else %}
                                 {{ assignment_request.get_status_display }}
                             {% endif %}
                         </td>
                         <td class="text-nowrap">
                             {% if not assignment_request.is_confirmed and not assignment_request.is_rejected %}
-                            <a href="{% url 'ar-respond-assignment-request' assignment_request.id %}" class="btn btn-success">Beantworten</a>
+                            <a href="{% url 'juntagrico-assignment-request:respond' assignment_request.id %}" class="btn btn-success">Beantworten</a>
                             {% endif %}
                         </td>
                     </tr>
                     <tr class="ar-assignment-request-description">
                         <td colspan="4">
                             <p>{% trans "Beschreibung" %}: {{ assignment_request.description }}</p>
                             {% if assignment_request.response %}<p>{% trans "Antwort" %}: {{ assignment_request.response }}</p>{% endif %}
@@ -77,13 +77,13 @@
         </table>
         {% else %}
             {% trans "Keine offenen Anfragen an dich" %}
         {% endif %}
     </div>
     <div class="col-md-12 mb-4">
     {% if archive %}
-        <a href="{% url 'ar-list-assignment-requests' %}">{% trans "Zurück zu den offenen Anfragen" %}</a>
+        <a href="{% url 'juntagrico-assignment-request:list' %}">{% trans "Zurück zu den offenen Anfragen" %}</a>
     {% else %}
-        <a href="{% url 'ar-list-archive' %}">{% trans "Beantwortete Anfragen anzeigen" %}</a>
+        <a href="{% url 'juntagrico-assignment-request:archive' %}">{% trans "Beantwortete Anfragen anzeigen" %}</a>
     {% endif %}
     </div>
 {% endblock %}
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/confirmed_assignment_request_mail.txt` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/confirmed.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 Soeben hat {{ assignment_request.approver }} deine Anfrage angenommen.
 {% if assignment_request.response %}
 Antwort: "{{ assignment_request.response }}"
 {% endif %}
 
 Es geht um folgende/n/s {% vocabulary 'assignment' %}:
     {{ serverurl }}{% url 'job' assignment_request.assignment.job.id %}
-{% include "assignment_request/mails/snippets/assignment_request_summary.txt" %}
+{% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.description %}
 Du hattest bei der Anfrage folgende Mitteilung hinterlassen:
 "{{ assignment_request.description }}"
 {% endif %}
 {% endblock %}
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/edited_assignment_request_mail.txt` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/edited.txt`

 * *Files 27% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 {% block content %}
   {% vocabulary "assignment" as v_assignment %}
   {% vocabulary "assignment_pl" as v_assignment_pl %}
 Soeben hat {{ assignment_request.member }} die {{ v_assignment }}-Anfrage bearbeitet:
 "{{ assignment_request.description }}"
 
     Anzahl: {{ assignment_request.amount }}
-{% include "assignment_request/mails/snippets/assignment_request_summary.txt" %}
+{% include "assignment_request/mails/snippets/summary.txt" %}
 
 {% if assignment_request.approver %}
 Laut {{ assignment_request.member }} wurde das mit dir abgesprochen.
 {% else %}
 {{ assignment_request.member }} hat keine Referenzperson angegeben.
 {% endif %}
 
 Bestätige ohne Kommentar
-{{ serverurl }}{% url 'ar-confirm-assignment-request' assignment_request.id %}
+{{ serverurl }}{% url 'juntagrico-assignment-request:confirm' assignment_request.id %}
 oder schreibe zuerst eine Antwort an {{ assignment_request.member }}:
-{{ serverurl }}{% url 'ar-respond-assignment-request' assignment_request.id %}
+{{ serverurl }}{% url 'juntagrico-assignment-request:respond' assignment_request.id %}
 {% endblock %}
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/new_assignment_request_mail.txt` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/new.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 {% load juntagrico.config %}
 {% block content %}
   {% vocabulary "assignment" as v_assignment %}
   {% vocabulary "assignment_pl" as v_assignment_pl %}
 Soeben hat {{ assignment_request.member }} {{ assignment_request.amount }} {{ v_assignment_pl }} mit folgender Mitteilung beantragt:
 "{{ assignment_request.description }}"
 
-{% include "assignment_request/mails/snippets/assignment_request_summary.txt" %}
+{% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.approver %}
     Laut {{ assignment_request.member }} wurde das mit dir abgesprochen.
 {% else %}
     {{ assignment_request.member }} hat keine Referenzperson angegeben.
 {% endif %}
 
 Bestätige ohne Kommentar
-{{ serverurl }}{% url 'ar-confirm-assignment-request' assignment_request.id %}
+{{ serverurl }}{% url 'juntagrico-assignment-request:confirm' assignment_request.id %}
 oder schreibe zuerst eine Antwort an {{ assignment_request.member }}:
-{{ serverurl }}{% url 'ar-respond-assignment-request' assignment_request.id %}
+{{ serverurl }}{% url 'juntagrico-assignment-request:respond' assignment_request.id %}
 {% endblock %}
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/notify_original_approver_mail.txt` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/admin/notify_original_approver.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 {% if assignment_request.response %}
 Entscheidung: {{ assignment_request.get_status_display }}
 Antwort: "{{ assignment_request.response }}"{% endif %}
 
 {{ assignment_request.member }} hatte zuletzt dich als Referenzperson angegeben.
 
 Es geht um folgende/n/s {% vocabulary 'assignment' %}:
-{% include "assignment_request/mails/snippets/assignment_request_summary.txt" %}
+{% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.description %}
 Beschreibung:
 "{{ assignment_request.description }}"
 {% endif %}
 
 {% endblock %}
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/rejected_assignment_request_mail.txt` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/rejected.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% extends "mails/email.txt" %}
 {% load juntagrico.config %}
 {% block content %}
 Soeben hat {{ assignment_request.approver }} deine Anfrage mit folgender Begründung abgelehnt:
 "{{ assignment_request.response }}"
 
 Es geht um folgende/n/s {% vocabulary 'assignment' %}:
-{% include "assignment_request/mails/snippets/assignment_request_summary.txt" %}
+{% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.description %}
 Du hattest bei der Anfrage folgende Mitteilung hinterlassen:
 "{{ assignment_request.description }}"
 {% endif %}
 
 Du kannst hier deine Anfrage anpassen:
-{{ serverurl }}{% url 'ar-edit-assignment-request' assignment_request.id %}
+{{ serverurl }}{% url 'juntagrico-assignment-request:edit' assignment_request.id %}
 Oder sie hier löschen:
-{{ serverurl }}{% url 'ar-delete-assignment-request' assignment_request.id %}
+{{ serverurl }}{% url 'juntagrico-assignment-request:delete' assignment_request.id %}
 {% endblock %}
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/mails/responded_assignment_request_mail.txt` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/mails/member/responded.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% extends "mails/email.txt" %}
 {% load juntagrico.config %}
 {% block content %}
 Soeben hat {{ assignment_request.approver }} eine Rückfrage auf deine Anfrage verfasst:
 "{{ assignment_request.response }}"
 
 Es geht um folgende/n/s {% vocabulary 'assignment' %}:
-{% include "assignment_request/mails/snippets/assignment_request_summary.txt" %}
+{% include "assignment_request/mails/snippets/summary.txt" %}
 {% if assignment_request.description %}
 Du hattest bei der Anfrage folgende Mitteilung hinterlassen:
 "{{ assignment_request.description }}"
 {% endif %}
 
 Du kannst auf die Rückfrage antworten, indem du hier die Anfrage anpasst:
-{{ serverurl }}{% url 'ar-edit-assignment-request' assignment_request.id %}
+{{ serverurl }}{% url 'juntagrico-assignment-request:edit' assignment_request.id %}
 {% endblock %}
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/request_assignment.html` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/request.html`

 * *Files 6% similar despite different names*

```diff
@@ -63,18 +63,18 @@
                             {% if assignment_request.assignment.job %}
                                 <a href="{% url 'job' assignment_request.assignment.job.id %}">{{ assignment_request.get_status_display }}</a>
                             {% else %}
                                 {{ assignment_request.get_status_display }}
                             {% endif %}
                         </td>
                         <td class="text-nowrap">
-                            <a href="{% url 'ar-edit-assignment-request' assignment_request.id %}"
+                            <a href="{% url 'juntagrico-assignment-request:edit' assignment_request.id %}"
                                class="edit"><i class="fas fa-pen"></i></a>
                             {% if not assignment_request.is_confirmed %}
-                            <a href="{% url 'ar-delete-assignment-request' assignment_request.id %}"
+                            <a href="{% url 'juntagrico-assignment-request:delete' assignment_request.id %}"
                                onclick="return confirm('{% trans 'Bist du sicher, dass du die Anfrage löschen möchtest' %}');"
                                class="delete"><i class="fas fa-trash"></i></a>
                             {% endif %}
                         </td>
                     </tr>
                     <tr class="ar-assignment-request-description">
                         <td colspan="3">
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/templates/assignment_request/respond_assignment_request.html` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/templates/assignment_request/respond.html`

 * *Files identical despite different names*

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request/views.py` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from datetime import date
 
 from django.contrib.auth.decorators import login_required, permission_required
-from django.db.models import Q
 from django.shortcuts import render, redirect, get_object_or_404
 from juntagrico.view_decorators import highlighted_menu
 
-from juntagrico_assignment_request.dao.assignmentrequestdao import AssignmentRequestDao
 from juntagrico_assignment_request.forms import AssignmentRequestForm, AssignmentResponseForm
 from juntagrico_assignment_request.mailer import membernotification, adminnotification
 from juntagrico_assignment_request.models import AssignmentRequest
 
 
 @login_required
 @highlighted_menu('request_assignment')
@@ -22,35 +20,35 @@
     assignment_request_form = AssignmentRequestForm(request.POST or None)
     if request.method == 'POST' and assignment_request_form.is_valid():
         # Create request
         assignment_request = assignment_request_form.instance
         assignment_request.member = member
         assignment_request.save()
         adminnotification.request_created(assignment_request)
-        return redirect('ar-assignment-requested')
+        return redirect('juntagrico-assignment-request:requested')
 
     renderdict = {
-        'assignment_requests': AssignmentRequestDao.current_requests_by_member(member),
+        'assignment_requests': AssignmentRequest.objects.filter(member=member).pending(),
         'form': assignment_request_form,
         'sent': sent
     }
-    return render(request, "assignment_request/request_assignment.html", renderdict)
+    return render(request, "assignment_request/request.html", renderdict)
 
 
 @login_required
 def delete_request_assignment(request, request_id):
     """
     Delete an assignment request
     """
 
     assignment_request = get_object_or_404(AssignmentRequest, id=request_id)
     if assignment_request.member == request.user.member\
             and not assignment_request.assignment:
         assignment_request.delete()
-    return redirect('ar-request-assignment')
+    return redirect('juntagrico-assignment-request:request')
 
 
 @login_required
 @highlighted_menu('request_assignment')
 def edit_request_assignment(request, request_id):
     """
     Edit and assignment request
@@ -61,48 +59,42 @@
     assignment_request_form = AssignmentRequestForm(request.POST or None, instance=assignment_request)
     if request.method == 'POST' and assignment_request_form.is_valid():
         # edit request
         assignment_request = assignment_request_form.instance
         assignment_request.status = AssignmentRequest.REQUESTED
         assignment_request.save()
         adminnotification.request_changed(assignment_request)
-        return redirect('ar-assignment-requested')
+        return redirect('juntagrico-assignment-request:requested')
 
     renderdict = {
         'form': assignment_request_form,
     }
-    return render(request, "assignment_request/edit_assignment_request.html", renderdict)
-
-
-def filter_approver(user):
-    if user.has_perm('juntagrico_assignment_request.notified_on_unapproved_assignments'):
-        return Q(approver=user.member) | Q(approver__isnull=True)
-    return Q(approver=user.member)
+    return render(request, "assignment_request/edit.html", renderdict)
 
 
 @permission_required('juntagrico_assignment_request.can_confirm_assignments')
 def list_assignment_requests(request):
     """
     List assignment requests
     """
-    ar = AssignmentRequest.objects.filter(status=AssignmentRequest.REQUESTED).filter(filter_approver(request.user))
+    ar = AssignmentRequest.objects.filter(status=AssignmentRequest.REQUESTED).for_approver(request.user.member)
     renderdict = {
         'assignment_requests': ar,
     }
-    return render(request, "assignment_request/list_assignment_requests.html", renderdict)
+    return render(request, "assignment_request/list.html", renderdict)
 
 
 @permission_required('juntagrico_assignment_request.can_confirm_assignments')
 def list_archive(request):
-    ar = AssignmentRequest.objects.exclude(status=AssignmentRequest.REQUESTED).filter(filter_approver(request.user))
+    ar = AssignmentRequest.objects.exclude(status=AssignmentRequest.REQUESTED).for_approver(request.user.member)
     renderdict = {
         'assignment_requests': ar,
         'archive': True
     }
-    return render(request, "assignment_request/list_assignment_requests.html", renderdict)
+    return render(request, "assignment_request/list.html", renderdict)
 
 
 @permission_required('juntagrico_assignment_request.can_confirm_assignments')
 def respond_assignment_request(request, request_id):
     """
     Confirm or reject an assignment request
     """
@@ -116,21 +108,21 @@
             assignment_request.status = AssignmentRequest.CONFIRMED
         elif 'reject' in request.POST:
             assignment_request.status = AssignmentRequest.REJECTED
         adminnotification.request_handled_by_other_approver(assignment_request, request.user.member)
         assignment_request.approver = request.user.member
         assignment_request.save()
         membernotification.request_handled(assignment_request)
-        return redirect('ar-list-assignment-requests')
+        return redirect('juntagrico-assignment-request:list')
 
     renderdict = {
         'assignment_request': assignment_request,
         'form': assignment_response_form,
     }
-    return render(request, "assignment_request/respond_assignment_request.html", renderdict)
+    return render(request, "assignment_request/respond.html", renderdict)
 
 
 @permission_required('juntagrico_assignment_request.can_confirm_assignments')
 def confirm_assignment_request(request, request_id):
     """
     Confirm an assignment request directly
     """
@@ -140,8 +132,8 @@
         assignment_request.response = ''
         assignment_request.status = AssignmentRequest.CONFIRMED
         adminnotification.request_handled_by_other_approver(assignment_request, request.user.member)
         # overwrite approver in any case to actual approver
         assignment_request.approver = request.user.member
         assignment_request.save()
         membernotification.request_handled(assignment_request)
-    return redirect('ar-list-assignment-requests')
+    return redirect('juntagrico-assignment-request:list')
```

### Comparing `juntagrico_assignment_request-1.5.0/juntagrico_assignment_request.egg-info/SOURCES.txt` & `juntagrico-assignment-request-1.6.0/juntagrico_assignment_request.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
-setup.cfg
-setup.py
 juntagrico_assignment_request/__init__.py
 juntagrico_assignment_request/admin.py
 juntagrico_assignment_request/apps.py
-juntagrico_assignment_request/config.py
 juntagrico_assignment_request/forms.py
-juntagrico_assignment_request/juntagricoapp.py
+juntagrico_assignment_request/hack.py
 juntagrico_assignment_request/models.py
 juntagrico_assignment_request/urls.py
+juntagrico_assignment_request/utils.py
 juntagrico_assignment_request/views.py
 juntagrico_assignment_request.egg-info/PKG-INFO
 juntagrico_assignment_request.egg-info/SOURCES.txt
 juntagrico_assignment_request.egg-info/dependency_links.txt
 juntagrico_assignment_request.egg-info/requires.txt
 juntagrico_assignment_request.egg-info/top_level.txt
 juntagrico_assignment_request/admins/__init__.py
 juntagrico_assignment_request/admins/assignment_request_admin.py
-juntagrico_assignment_request/dao/__init__.py
-juntagrico_assignment_request/dao/assignmentrequestdao.py
-juntagrico_assignment_request/entity/__init__.py
-juntagrico_assignment_request/entity/assignment_request.py
 juntagrico_assignment_request/mailer/__init__.py
 juntagrico_assignment_request/mailer/adminnotification.py
 juntagrico_assignment_request/mailer/membernotification.py
 juntagrico_assignment_request/migrations/0001_squashed_0006_auto_20191020_2203.py
 juntagrico_assignment_request/migrations/0002_fix_naming_and_relation.py
 juntagrico_assignment_request/migrations/0003_change_assignment_helptext.py
 juntagrico_assignment_request/migrations/0004_auto_20211207_1101.py
 juntagrico_assignment_request/migrations/__init__.py
-juntagrico_assignment_request/templates/assignment_request/edit_assignment_request.html
-juntagrico_assignment_request/templates/assignment_request/list_assignment_requests.html
-juntagrico_assignment_request/templates/assignment_request/request_assignment.html
-juntagrico_assignment_request/templates/assignment_request/respond_assignment_request.html
-juntagrico_assignment_request/templates/assignment_request/mails/confirmed_assignment_request_mail.txt
-juntagrico_assignment_request/templates/assignment_request/mails/edited_assignment_request_mail.txt
-juntagrico_assignment_request/templates/assignment_request/mails/new_assignment_request_mail.txt
-juntagrico_assignment_request/templates/assignment_request/mails/notify_original_approver_mail.txt
-juntagrico_assignment_request/templates/assignment_request/mails/rejected_assignment_request_mail.txt
-juntagrico_assignment_request/templates/assignment_request/mails/responded_assignment_request_mail.txt
-juntagrico_assignment_request/templates/assignment_request/mails/snippets/assignment_request_summary.txt
-juntagrico_assignment_request/templates/assignment_request/menu/assignment_request_admin_menu.html
-juntagrico_assignment_request/templates/assignment_request/menu/assignment_request_user_menu.html
-juntagrico_assignment_request/templatetags/__init__.py
-juntagrico_assignment_request/templatetags/assignment_request_config.py
+juntagrico_assignment_request/templates/assignment_request/edit.html
+juntagrico_assignment_request/templates/assignment_request/list.html
+juntagrico_assignment_request/templates/assignment_request/request.html
+juntagrico_assignment_request/templates/assignment_request/respond.html
+juntagrico_assignment_request/templates/assignment_request/mails/admin/edited.txt
+juntagrico_assignment_request/templates/assignment_request/mails/admin/new.txt
+juntagrico_assignment_request/templates/assignment_request/mails/admin/notify_original_approver.txt
+juntagrico_assignment_request/templates/assignment_request/mails/member/confirmed.txt
+juntagrico_assignment_request/templates/assignment_request/mails/member/rejected.txt
+juntagrico_assignment_request/templates/assignment_request/mails/member/responded.txt
+juntagrico_assignment_request/templates/assignment_request/mails/snippets/summary.txt
+juntagrico_assignment_request/templates/menu/admin_menu.html
+juntagrico_assignment_request/templates/menu/user_menu.html
```

